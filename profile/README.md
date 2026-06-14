# KariosOS

[![License: AGPLv3](https://img.shields.io/badge/License-AGPLv3-blue.svg)]()
[![Hypervisor: bhyve](https://img.shields.io/badge/Hypervisor-bhyve-red.svg)]()
[![Storage: ZFS](https://img.shields.io/badge/Storage-ZFS-green.svg)]()
[![Category: Infrastructure OS](https://img.shields.io/badge/Category-Infrastructure%20OS-orange.svg)]()
[![API: First](https://img.shields.io/badge/API-First-brightgreen.svg)]()

**KariosOS** is an open-source **Infrastructure Operating System (IaOS)** designed for building and operating modern private clouds, edge environments, and enterprise datacenters.

KariosOS unifies virtualization, storage, networking, IP address management, Kubernetes orchestration, DNS/DHCP services, observability, and automation into a single platform with a common API and management experience.

Instead of assembling and maintaining dozens of disconnected infrastructure products, operators can manage their entire environment through a unified control plane.

---

## Why KariosOS?

### Infrastructure as an Operating System

KariosOS treats infrastructure as a single operating system rather than a collection of independent tools.

Compute, storage, networking, security, observability, and automation operate through a common platform, simplifying deployment and day-to-day operations.

### Enterprise Virtualization with bhyve

KariosOS is built around the native **bhyve hypervisor**, providing lightweight, high-performance virtualization for modern workloads.

Capabilities include:

- Virtual Machines
- Templates & Cloning
- Snapshots
- Resource Management
- API-Driven Provisioning
- Multi-Node Infrastructure Management

### ZFS-Native Storage

Storage is integrated directly into the platform through **ZFS**, enabling:

- Snapshots
- Replication
- Data Integrity
- Storage Pool Management
- Automated Provisioning

### Unified Operations

Manage infrastructure from a single platform:

- Virtual Machines
- Containers & Kubernetes
- Networking
- IP Address Management
- DNS & DHCP
- Storage
- Monitoring
- Datacenter Inventory

### API First

Every capability exposed through the user interface is available through APIs and automation workflows.

### Open Source

KariosOS Community Edition is developed openly and welcomes community participation.

---

## Quick Start

Download the latest KariosOS release from the Releases page.

### Installation

1. Download the [latest ISO](https://s3.us-east-1.amazonaws.com/amzn-kariosbsd-14.3/kariosbsd-14.3-custom.iso)
2. Boot the installer
3. Complete onboarding
4. Access the KariosOS web interface
5. Start deploying infrastructure

Detailed installation instructions are available in [INSTALL.md](INSTALL.md).

---

## Core Capabilities

### Virtualization

- bhyve Virtual Machines
- VM Templates
- Snapshots & Cloning
- Resource Scheduling
- Infrastructure Provisioning

### Networking & IPAM

- IP Address Management
- VLAN Management
- VRF Management
- DNS Automation
- DHCP Automation
- Datacenter Inventory

### Kubernetes

- Kubernetes Cluster Provisioning
- Cluster Lifecycle Management
- Integrated Infrastructure Services

### Storage

- ZFS Native Storage
- Snapshots
- Replication
- Pool Management
- Automated Storage Provisioning

### Observability

- Metrics Collection
- Dashboards
- Capacity Monitoring
- Infrastructure Health Monitoring

### Automation

- REST APIs
- Event-Driven Workflows
- External Integrations
- Infrastructure Automation

---

## Architecture

KariosBSD is composed of multiple open-source projects that together form the platform.

| Repository | Description |
|------------|-------------|
| [karios-apis](https://github.com/karios-os/karios-apis) | Infrastructure orchestration APIs |
| [karios-web](https://github.com/karios-os/karios-web) | Web management interface |
| [karios-ipam](https://github.com/karios-os/karios-ipam) | IPAM and DDI orchestration |
| [karios-common](https://github.com/karios-os/karios-common) | Shared platform libraries |

Each repository contains its own development, build, and deployment documentation.

---

## Documentation

Documentation includes:

- Installation Guides
- Administration Guides
- API References
- Architecture Documentation
- Hardware Compatibility Lists (HCL)
- Troubleshooting Guides
- Upgrade Guides

---

## Community

We welcome operators, developers, infrastructure engineers, and contributors.

### Get Involved

- Report bugs through GitHub Issues
- Submit feature requests
- Participate in Discussions
- Improve Documentation
- Contribute Code

---

## Licensing & Commercial Use

KariosBSD is available under a dual-licensing model.

### Community Edition

Licensed under the:

**GNU Affero General Public License v3 (AGPLv3)**

If you modify KariosBSD and provide it as a network-accessible service, the AGPL requires those modifications to be made available under the same license.

See LICENSE for complete terms.

### Commercial Licensing

Organizations requiring:

- AGPL exemptions
- Private modifications
- Enterprise support
- OEM redistribution rights
- White-label options

may obtain a commercial license.

---

## Support Options

### Community Support

- GitHub Discussions
- Community Forums
- Documentation

### Professional Support

- Business Hours Support
- Deployment Assistance
- Architecture Reviews

### Enterprise Support

- 24x7 Support
- Emergency Response
- Dedicated Engineering Assistance
- Long-Term Maintenance

---

## Security

Security is a core design principle of KariosBSD.

Please do not report vulnerabilities through public GitHub issues.

---

## Contributing

We welcome contributions from the community.

Before contributing:

1. Sign the Contributor License Agreement (CLA)
2. Submit a Pull Request

All submissions are reviewed by project maintainers.

---

## Trademarks

"KariosBSD", "Karios", and associated logos may be protected trademarks.

---

## License

Copyright © Karios Project

Licensed under the GNU Affero General Public License v3.0.

See LICENSE for complete terms.