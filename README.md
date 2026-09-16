# Microsoft-AZ-800-Windows-Server-Hybrid-Core-Infrastructure-Study-Guide
AZ-800 study guide covering AD DS, hybrid identity, Windows Server management, Azure Arc, virtualization, containers, networking, storage, PowerShell, and practical labs.
# Microsoft AZ-800: Administering Windows Server Hybrid Core Infrastructure Study Guide

> **Important:** Microsoft has announced that AZ-800 will retire on **September 30, 2026, at 5:00 PM Central Standard Time**. Verify Microsoft's current certification and exam availability before scheduling. [1]

## Introduction

This repository is an independent study guide for **Microsoft AZ-800: Administering Windows Server Hybrid Core Infrastructure**.

It focuses on administering Windows Server across on-premises and hybrid environments, including Active Directory Domain Services, hybrid identity, Azure Arc, Windows Admin Center, virtualization, containers, networking, storage, and Windows Server management.

The current English exam objectives were updated January 21, 2026. [1][2]

## Exam Overview

| Item | Information |
|---|---|
| Vendor | Microsoft |
| Exam | AZ-800 |
| Certification | Microsoft Certified: Windows Server Hybrid Administrator Associate |
| Purpose | Administer Windows Server core infrastructure in on-premises and hybrid environments |
| Target candidates | Windows Server Hybrid Administrators |
| Recommended background | Several years of Windows Server experience |
| Passing score | 700 or greater |
| Listed duration | Verify current Microsoft scheduling information |
| Current listed price | $165 USD* |
| Languages | English, Japanese, Chinese (Simplified), German, French, Spanish, Portuguese (Brazil) |
| Current retirement date | September 30, 2026 |

*Microsoft notes that pricing depends on the country or region where the exam is proctored and may be subject to taxes. [1]

AZ-800 is one of the required exams for the Windows Server Hybrid Administrator Associate certification. Microsoft currently lists AZ-800, AZ-801, and AZ-802 as required exams for that certification. [3]

## Who Should Take It?

AZ-800 is designed for administrators responsible for Windows Server infrastructure in on-premises and hybrid environments.

Useful experience includes:

- Windows Server administration
- Active Directory
- Networking
- PowerShell
- Virtualization
- Storage
- Azure administration
- Microsoft Entra ID
- Hybrid identity
- Security administration

## Exam Objectives / Domains

Microsoft's current skills measured are:

### 1. Deploy and Manage Active Directory Domain Services — 30–35%

Study:

- Domain controllers
- On-premises domain controllers
- Azure-based domain controllers
- Read-only domain controllers
- FSMO roles
- Forests and domains
- Trusts
- AD DS sites
- Replication
- Users and groups
- Service accounts
- Windows Server domain joining
- Microsoft Entra Domain Services
- Microsoft Entra ID
- Microsoft Entra Connect Sync
- Microsoft Entra Cloud Sync
- Microsoft Entra Connect Health
- Hybrid authentication
- Staged rollout
- Group Policy
- Group Policy Preferences

### 2. Manage Windows Servers and Workloads in a Hybrid Environment — 10–15%

Focus on:

- Windows Admin Center
- Windows Admin Center in Azure
- Azure Arc
- Azure Policy
- Azure Update Manager
- Azure Monitor
- Azure VM administration
- PowerShell remoting
- Windows Server management
- Hybrid server management
- Azure integration

### 3. Manage Virtual Machines and Containers — 15–20%

Understand:

- Hyper-V
- Azure virtual machines
- VM configuration
- VM networking
- VM storage
- Windows containers
- Container images
- Container networking
- Container management
- Azure IaaS integration

### 4. Implement and Manage Networking Infrastructure — 15–20%

Study:

- IPv4 and IPv6
- DNS
- DHCP
- Windows Server networking
- Azure networking
- VNets
- Subnets
- Network Security Groups
- VPN
- Routing
- Hybrid connectivity
- Network troubleshooting

### 5. Manage Storage and File Services — 15–20%

Review:

- Storage Spaces
- Storage Spaces Direct
- SMB
- SMB security
- SMB compression
- SMB encryption
- DFS
- DFS Replication
- File Server Resource Manager
- Windows Server file shares
- Azure Storage integration
- Azure File Sync

These domains and percentages reflect Microsoft's skills measured as of January 21, 2026. [2]

## Detailed Study Notes

### Active Directory Domain Services

Understand the core AD DS hierarchy:

**Forest → Domain → OU → Users/Groups/Computers**

Know:

- Domain controllers
- Global Catalog
- FSMO roles
- Sites
- Replication
- Trusts
- Group Policy

For troubleshooting, understand DNS, replication, authentication, and time synchronization dependencies.

### FSMO Roles

Know the five roles:

- Schema Master
- Domain Naming Master
- RID Master
- PDC Emulator
- Infrastructure Master

Understand when role transfer or seizure may be appropriate and the risks involved.

### Hybrid Identity

Understand how on-premises AD DS integrates with Microsoft Entra ID.

Review:

- Microsoft Entra Connect Sync
- Microsoft Entra Cloud Sync
- Authentication
- Password synchronization
- Connect Health
- Microsoft Entra Domain Services
- Staged rollout

### Group Policy

Understand:

- GPOs
- GPO links
- Security filtering
- Group Policy Preferences
- Processing order
- Troubleshooting

Use Group Policy to centrally manage Windows Server and domain-joined systems.

### Windows Admin Center and Azure Arc

Windows Admin Center provides browser-based Windows Server administration.

Azure Arc extends Azure management capabilities to servers outside Azure.

Understand how these tools support:

**Inventory → Management → Monitoring → Policy → Updates**

### Virtualization

Review Hyper-V concepts:

- Virtual switches
- Virtual disks
- VM configuration
- Checkpoints
- Dynamic memory
- Live migration
- VM storage

Understand the differences between managing Windows Server VMs on-premises and Azure VMs.

### Containers

Understand:

- Container images
- Containers
- Isolation
- Networking
- Storage
- Windows container management

Know when containerization is appropriate compared with traditional VMs.

### Networking

A strong networking foundation is essential.

Review:

- DNS
- DHCP
- IP addressing
- Routing
- VNets
- Subnets
- NSGs
- VPN
- Hybrid connectivity

For troubleshooting, verify DNS resolution, routing, firewall rules, ports, and authentication dependencies systematically.

### Storage and File Services

Understand:

- Storage Spaces
- Storage Spaces Direct
- SMB
- DFS
- DFS Replication
- FSRM
- Azure File Sync

Choose storage technology based on capacity, performance, availability, synchronization, and management requirements.

## Important Concepts

Revise:

- AD DS
- Domain controllers
- FSMO
- Forests
- Domains
- Trusts
- AD sites
- Replication
- RODC
- Service accounts
- Group Policy
- Microsoft Entra ID
- Microsoft Entra Domain Services
- Entra Connect Sync
- Entra Cloud Sync
- Connect Health
- Hybrid identity
- Windows Admin Center
- Azure Arc
- Azure Policy
- Azure Update Manager
- Azure Monitor
- PowerShell
- Hyper-V
- Azure VMs
- Windows containers
- DNS
- DHCP
- VNets
- Subnets
- NSGs
- VPN
- Routing
- Storage Spaces
- Storage Spaces Direct
- SMB
- DFS
- DFS Replication
- FSRM
- Azure File Sync

## Practical Examples / Labs

Use only systems and Azure resources you are authorized to administer.

1. Build a small Windows Server AD DS lab.
2. Promote a server to a domain controller.
3. Create users, groups, and OUs.
4. Configure and troubleshoot Group Policy.
5. Configure AD DS sites and replication.
6. Examine and manage FSMO roles in a lab.
7. Deploy a Windows Server VM in Azure.
8. Connect a Windows Server to Microsoft Entra-based services.
9. Configure a test hybrid identity environment.
10. Install Windows Admin Center.
11. Connect a server to Azure Arc.
12. Apply an Azure Policy to an Arc-enabled server.
13. Configure Azure Update Manager.
14. Create a Hyper-V virtual machine.
15. Configure a virtual switch.
16. Deploy and manage a Windows container.
17. Configure DNS and DHCP.
18. Create Azure VNet and subnet configurations.
19. Configure a test VPN/hybrid network.
20. Create SMB file shares.
21. Configure DFS/DFS Replication in a lab.
22. Explore Storage Spaces.
23. Configure Azure File Sync in a test environment.

## Study Strategy

Use Microsoft Learn and the official AZ-800 study guide as primary resources.

Combine:

- Windows Server documentation
- Microsoft Learn modules
- Azure documentation
- AD DS labs
- PowerShell practice
- Windows Admin Center
- Azure Arc
- Hyper-V
- Networking labs
- Storage and file-service labs
- Microsoft's free Practice Assessment
- Microsoft's exam sandbox

Microsoft recommends training and hands-on experience before taking the exam. [2]

Prioritize troubleshooting and architecture scenarios rather than memorizing administrative commands alone.

## 30-Day Study Plan

**Days 1–5:** AD DS architecture, domain controllers, FSMO, forests, domains, trusts, sites, and replication.

**Days 6–9:** Users, groups, service accounts, hybrid identity, Entra Connect Sync, Cloud Sync, Domain Services, and authentication.

**Days 10–12:** Group Policy, Group Policy Preferences, Windows Admin Center, and PowerShell administration.

**Days 13–16:** Azure Arc, Azure Policy, Update Manager, Azure Monitor, and hybrid server management.

**Days 17–20:** Hyper-V, Azure VMs, VM networking, VM storage, and Windows containers.

**Days 21–24:** DNS, DHCP, IPv4/IPv6, routing, VNets, subnets, NSGs, VPN, and hybrid networking.

**Days 25–27:** Storage Spaces, Storage Spaces Direct, SMB, DFS, DFS Replication, FSRM, and Azure File Sync.

**Days 28–29:** Complete an end-to-end Windows Server hybrid lab and troubleshoot deliberately introduced failures.

**Day 30:** Review weak domains, complete Microsoft's Practice Assessment, use the exam sandbox, and verify the current retirement information.

## Common Mistakes

- Treating AD DS and Microsoft Entra ID as identical
- Ignoring DNS when troubleshooting AD DS
- Confusing FSMO role transfer with seizure
- Misunderstanding AD DS sites and replication
- Applying overly broad Group Policies
- Ignoring permissions in hybrid environments
- Confusing Azure Arc with Azure VM management
- Choosing VMs when containers are more appropriate, or vice versa
- Ignoring routing and NSGs during network troubleshooting
- Confusing DFS Replication with a backup solution
- Choosing storage without considering performance and availability
- Memorizing PowerShell commands without understanding their purpose
- Studying outdated AZ-800 objectives

## Exam-Day Tips

- Read the complete scenario before choosing an answer.
- Identify whether the requirement concerns identity, management, compute, networking, or storage.
- Pay attention to whether the environment is on-premises, Azure, or hybrid.
- For troubleshooting questions, identify dependencies before changing configuration.
- Consider security, availability, performance, and administrative effort.
- Eliminate solutions that do not satisfy a stated requirement.
- Manage time carefully and revisit flagged questions when possible.
- Microsoft requires a score of **700 or greater** to pass. [1][2]

Because Microsoft has announced AZ-800's retirement for September 30, 2026, verify the current exam schedule and any transition guidance before booking. [1]

## Final Checklist

- [ ] Understand AD DS architecture
- [ ] Know FSMO roles
- [ ] Understand trusts, sites, and replication
- [ ] Can manage users and groups
- [ ] Understand service accounts
- [ ] Can configure Group Policy
- [ ] Understand hybrid identity
- [ ] Know Entra Connect Sync and Cloud Sync
- [ ] Understand Windows Admin Center
- [ ] Know Azure Arc
- [ ] Understand Azure Policy and Update Manager
- [ ] Can manage Hyper-V and Azure VMs
- [ ] Understand Windows containers
- [ ] Comfortable with DNS and DHCP
- [ ] Understand Azure networking
- [ ] Know VPN and hybrid connectivity
- [ ] Understand SMB, DFS, and DFS Replication
- [ ] Understand Storage Spaces
- [ ] Know Azure File Sync
- [ ] Completed hands-on labs
- [ ] Completed Microsoft's Practice Assessment
- [ ] Reviewed the current AZ-800 study guide
- [ ] Checked Microsoft's retirement information

## Official Resources

- AZ-800 Exam:
  https://learn.microsoft.com/credentials/certifications/exams/az-800/
- AZ-800 Study Guide:
  https://learn.microsoft.com/credentials/certifications/resources/study-guides/az-800
- Windows Server Hybrid Administrator Associate:
  https://learn.microsoft.com/credentials/certifications/windows-server-hybrid-administrator/
- Windows Server Documentation:
  https://learn.microsoft.com/windows-server/
- Azure Documentation:
  https://learn.microsoft.com/azure/
- Azure Arc:
  https://learn.microsoft.com/azure/azure-arc/
- Windows Admin Center:
  https://learn.microsoft.com/windows-server/manage/windows-admin-center/
- Microsoft Entra ID:
  https://learn.microsoft.com/entra/identity/
- Hyper-V:
  https://learn.microsoft.com/windows-server/virtualization/hyper-v/
- Windows Containers:
  https://learn.microsoft.com/virtualization/windowscontainers/
- Microsoft Learn:
  https://learn.microsoft.com/training/

Always verify the latest AZ-800 study guide, exam availability, retirement date, pricing, languages, and certification requirements before registering.

## Voucher / Discount

**Learn SecByte, an official Microsoft reseller partner**, provides certification voucher options and discounts where available.

Learn SecByte's official Black Friday offer provides up to 70% off selected Microsoft exam vouchers.

AZ-800 voucher:

https://learn.secbyte.org/vouchers/microsoft-az-800

Check the current offer and availability before purchasing. Do not assume this specific exam is 70% off unless the current offer explicitly states it. Voucher pricing and availability may change.

## Disclaimer

This is an **independent/community study guide** and is not an official Microsoft certification document. Microsoft, Windows Server, Azure, Microsoft Entra, Azure Arc, Windows Admin Center, and related trademarks belong to Microsoft.

Candidates should verify current exam information, objectives, pricing, policies, retirement status, and voucher availability directly with Microsoft.

This repository does **not** contain exam dumps, leaked questions, or recalled exam questions. It is intended for legitimate education, hands-on learning, and certification preparation only.
