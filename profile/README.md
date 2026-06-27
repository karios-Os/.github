# KariosOS

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)]()
[![Hypervisor: bhyve](https://img.shields.io/badge/Hypervisor-bhyve-red.svg)]()
[![Storage: ZFS](https://img.shields.io/badge/Storage-ZFS-green.svg)]()
[![Category: Infrastructure OS](https://img.shields.io/badge/Category-Infrastructure%20OS-orange.svg)]()
[![API: First](https://img.shields.io/badge/API-First-brightgreen.svg)]()

**KariosOS** is an open-source **Infrastructure Operating System (IaOS)** designed for building and operating modern private clouds, edge environments, and enterprise datacenters.

KariosOS unifies virtualization, storage, networking, IP address management, Kubernetes orchestration, DNS/DHCP services, observability, and automation into a single platform with a common API and management experience.

Instead of assembling and maintaining dozens of disconnected infrastructure products, operators can manage their entire environment through a unified control plane.

We built this because we believe modern infrastructure shouldn't be locked behind restrictive corporate licensing or bloated roadmaps. Whether you are an agile startup architecting your first production environment or a global enterprise scaling to millions of concurrent users, KariosOS is engineered to grow with you.

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

Find the documentation [here](https://karios-os.github.io/docs/getting-started/index.html).

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

## Open Source Promise: Apache 2.0 & No CLAs

Great infrastructure software is a collaborative effort. If you contribute your time and expertise to the community, you should retain the rights to your work.

**100% Apache 2.0 License.** No restrictive copyleft traps, no sudden licensing rug-pulls. Use, modify, embed, and run KariosOS anywhere you see fit.

**Zero CLAs.** We will never ask you to sign your copyright over to us. We use the industry-standard Developer Certificate of Origin (DCO) — the same model as the Linux kernel. You simply add a `Signed-off-by` line to your commits. If you write the code, you own the code.

No developer should have to ask their legal department for permission to open a pull request.

---

## How We Keep the Lights On

KariosOS is an Open Core company. The core OS, high-performance routing engine, and APIs are licensed under Apache 2.0 and will remain free forever. We do not artificially throttle performance, cap resources, or cripple the open-source tier to force an upgrade — we want the community ecosystem to thrive unhindered.

We fund the project by selling what we call the "enterprise glue" and providing engineering firepower to teams running mission-critical infrastructure:

- **24x7x365 Production Support** — A direct line to the core engineering team when your cluster goes down at 3 AM on a Sunday. A forum post isn't going to save the day; we will.
- **Enterprise Integrations** — Specialized plugins for SAML/SSO, Active Directory, advanced RBAC, and FIPS compliance modules.
- **Customized Modules** — Purpose-built modules for proprietary hardware, legacy network topologies, or unique data pipelines.
- **Professional Coding Services** — Our core engineers embed directly with your team to design, build, deploy, and scale your KariosOS infrastructure from day one.

> If you are a hacker or a startup, KariosOS is completely free. If you are a Fortune 500 bank that needs someone to call at 3:00 AM, you pay us.

---

## Security

Security is a core design principle of KariosBSD.

Please do not report vulnerabilities through public GitHub issues.

---

## Contributing

We welcome contributions from the community. PRs are officially welcome — no lawyers required.

Before contributing, read [CONTRIBUTING.md](../CONTRIBUTING.md). The short version: sign your commits with `git commit -s` and open a PR.

Every PR uses the [Pull Request Template](../PULL_REQUEST_TEMPLATE.md) automatically — it includes the DCO sign-off checklist and review requirements.

All submissions are reviewed by project maintainers.

---

## Trademarks

"KariosBSD", "Karios", and associated logos may be protected trademarks.

---

## Legal & Licensing

| Document | Description |
|----------|-------------|
| [LICENSE](../LICENSE) | Apache License 2.0 — the full license terms for KariosOS |
| [NOTICE](../NOTICE) | Copyright notice and third-party attribution |
| [CONTRIBUTING.md](../CONTRIBUTING.md) | How to contribute, DCO sign-off guide, and PR process |
| [PULL_REQUEST_TEMPLATE.md](../PULL_REQUEST_TEMPLATE.md) | Checklist applied automatically to every pull request |
| [FREEBSD-COPYRIGHT-NOTICE.txt](../FREEBSD-COPYRIGHT-NOTICE.txt) | FreeBSD copyright notice and attribution |

Copyright © 2026 KariosOS Contributors. Licensed under the Apache License, Version 2.0.
