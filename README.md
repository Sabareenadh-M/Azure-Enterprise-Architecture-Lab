# Azure Enterprise Architecture Lab

[![Platform](https://img.shields.io/badge/Platform-Microsoft%20Azure-0078D4?logo=microsoft-azure&logoColor=white)](https://azure.microsoft.com/)
[![Focus](https://img.shields.io/badge/Focus-Enterprise%20Architecture-4B5563)](#project-structure)
[![Status](https://img.shields.io/badge/Status-Completed%20Lab%20Series-16A34A)](#demo--walkthrough)
[![Docs](https://img.shields.io/badge/Documentation-Per%20Project-2563EB)](#project-structure)

This repository showcases a multi-stage Azure enterprise lab that progresses from secure cloud networking to Active Directory, domain-integrated workloads, and hybrid cloud identity/backup integration.

## Project Overview

The lab is organized into four practical projects that simulate a realistic enterprise setup:

1. **Secure Hub-and-Spoke Azure networking** with Bastion-based administration
2. **Active Directory Domain Controller deployment** on Windows Server in Azure
3. **Domain-joined workstation and IIS member server integration**
4. **Hybrid cloud operations** using Microsoft Entra ID Connect and Azure Backup (MARS)

Each project folder includes a detailed README with step-by-step implementation notes and screenshots.

## Screenshots / Visuals

> ⚠️ **Top-level featured visuals are not added yet.**
>
> To showcase this repository on your profile/portfolio, add 1–3 highlight images (architecture diagram, topology, and hybrid flow) under:
> `assets/featured/`
>
> Suggested filenames:
> - `assets/featured/architecture-overview.png`
> - `assets/featured/network-topology.png`
> - `assets/featured/hybrid-identity-backup.png`

## Demo / Walkthrough

Use this path to review the lab end-to-end:

1. Start with **Project 1** to understand the secure network foundation  
   → [`Project 1 Hub and Spoke/README.md`](./Project%201%20Hub%20and%20Spoke/README.md)
2. Continue to **Project 2** for AD DS domain setup  
   → [`Project-2-Creating-AD-in-a-VM/README.md`](./Project-2-Creating-AD-in-a-VM/README.md)
3. Review **Project 3** for domain-joined clients/servers and IIS validation  
   → [`Project-3-Workstations-and-Web-Servers/README.md`](./Project-3-Workstations-and-Web-Servers/README.md)
4. Finish with **Project 4** for hybrid identity sync and backup recovery  
   → [`Project-4-Hybrid-Cloud-Integration/README.md`](./Project-4-Hybrid-Cloud-Integration/README.md)

## Project Structure

```text
Azure-Enterprise-Architecture-Lab/
├── Project 1 Hub and Spoke/
│   └── README.md
├── Project-2-Creating-AD-in-a-VM/
│   └── README.md
├── Project-3-Workstations-and-Web-Servers/
│   └── README.md
└── Project-4-Hybrid-Cloud-Integration/
    └── README.md
```

## Suggested GitHub Topics / Tags

Use these repository topics for discoverability:

- `azure`
- `enterprise-architecture`
- `hub-and-spoke`
- `azure-networking`
- `azure-bastion`
- `active-directory`
- `windows-server`
- `iis`
- `entra-id`
- `hybrid-cloud`
- `azure-backup`
- `cloud-lab`

