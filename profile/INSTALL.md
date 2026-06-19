# Installing KariosBSD from the ISO

This guide walks through installing KariosBSD from the prebuilt ISO image
onto a physical (bare-metal) machine.

> **Note**: KariosBSD is designed to run on bare metal, not as a guest VM —
> it acts as the hypervisor host for bhyve VMs and jails, so it needs direct
> access to the underlying hardware.

## 1. Download the ISO

Download the latest image:

- [kariosbsd-14.3-custom.iso](https://s3.us-east-1.amazonaws.com/amzn-kariosbsd-14.3/kariosbsd-14.3-custom.iso)

## 2. Write the ISO to a USB drive

This will erase the target drive — double check the device name before
running this:

```bash
# macOS
diskutil list
sudo dd if=kariosbsd-14.3-custom.iso of=/dev/rdiskN bs=1m

# Linux
lsblk
sudo dd if=kariosbsd-14.3-custom.iso of=/dev/sdX bs=4M status=progress conv=fsync
```

## 3. Boot the target machine from USB

Plug the USB drive into the target machine and boot from it (you may need to
change the boot order / boot device in BIOS or UEFI settings).

## 4. Run the installer

KariosBSD uses the standard FreeBSD `bsdinstall` installer. Follow the
on-screen prompts:

1. Select your keyboard layout.
2. Enter a hostname for the machine. (Follow sub-domain FQDN standards here)
3. Select the components you want to install (defaults are fine for most
   setups).
4. Choose a partitioning scheme (e.g. **Auto (ZFS)** is recommended).
5. Confirm the disk layout and proceed with the install. The installer will
   copy the base system to disk.
6. Set the `root` password when prompted.
7. Configure the network interface with a **static IP address** (do not use
   DHCP). KariosBSD installs Technitium, which acts as the DHCP server for
   the network — the network you install on should have **no other DHCP
   server** running, and the KariosBSD host itself must have a static IP so
   it can reliably serve DHCP/DNS for the rest of the network.
8. Set the system clock / timezone.
9. Choose which services to enable on startup.
10. When prompted for "Final Configuration" / additional users, you can
    create a non-root user account if desired.
11. Exit the installer and reboot when prompted. Remove the USB drive before
    the system reboots.

## 5. First boot

After reboot, log in at the console with the `root` (or other) credentials
you set during installation.

SSH into the node or work directly at the console, then run:

1. Install Ansible:
   ```sh
   pkg install py311-ansible
   ```

2. Run the bootstrap script:
   ```sh
   ./bootstrap.sh
   ```

## Troubleshooting

- **Machine won't boot from USB**: check that the boot order in your
  BIOS/UEFI settings prioritizes the USB device, and that "Secure Boot" is
  disabled if it prevents booting unsigned media.
- **Network not working after install**: log in as `root` and run
  `sysrc ifconfig_<interface>=DHCP` (replace `<interface>` with your NIC
  name, e.g. `em0`), then `service netif restart`.
- **Need to redo the install**: reboot from the USB drive again and re-run
  through the installer steps above.
