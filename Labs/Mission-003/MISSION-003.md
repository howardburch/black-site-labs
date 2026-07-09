# Mission #003 - Active Directory Domain Services (AD DS)

## Objective

Transform a standalone Windows Server 2025 virtual machine into the first Domain Controller for the BlackSite Labs enterprise environment by deploying Active Directory Domain Services (AD DS), configuring DNS, and creating the `blacksite.local` Active Directory forest.

---

## Environment

Host OS:
- Windows 11

Hypervisor:
- Oracle VirtualBox 7.2

Guest OS:
- Windows Server 2025 Standard Evaluation

Server Name:
- WS2025-DC01

Domain:
- blacksite.local

Forest:
- blacksite.local

Resources Allocated:
- 4 vCPUs
- 8 GB RAM
- 100 GB Dynamic VDI

---

## Technologies Used

- Active Directory Domain Services (AD DS)
- DNS
- Kerberos Authentication
- LDAP
- SYSVOL
- Global Catalog
- Windows Server Manager
- PowerShell
- Oracle VirtualBox

---

## Tasks Completed

- Verified Windows Server baseline configuration
- Created pre-installation virtual machine snapshot
- Installed Active Directory Domain Services (AD DS)
- Installed required AD DS management tools
- Promoted Windows Server to a Domain Controller
- Created a new Active Directory forest
- Created the `blacksite.local` domain
- Configured integrated DNS
- Configured Directory Services Restore Mode (DSRM)
- Verified successful Domain Controller promotion
- Logged into the BLACKSITE domain
- Verified Active Directory Users and Computers (ADUC)
- Verified DNS installation and Active Directory management tools
- Created post-installation snapshot

---

## Enterprise Concepts Learned

This mission introduced several core enterprise identity management concepts:

- Active Directory
- Domain Controllers
- Forests and Domains
- Authentication vs Authorization
- Kerberos
- LDAP
- DNS integration
- SYSVOL
- Global Catalog
- Active Directory Management Tools
- Windows Server Roles vs Features

---

## Outcome

The Windows Server 2025 virtual machine was successfully promoted to the first Domain Controller for the BlackSite Labs enterprise environment.

The server now provides:

- Centralized Identity Management
- Domain Authentication
- DNS Services
- Kerberos Authentication
- LDAP Directory Services
- Active Directory Database
- Enterprise Management Consoles

The `blacksite.local` forest is now operational and serves as the foundation for all future BlackSite Labs infrastructure.

Snapshots Created:

- Mission003-Before-ADDS
- Mission003-DomainController

---

## Lessons Learned

- Installing AD DS alone does not create a Domain Controller; the server must be promoted afterward.
- Active Directory relies on DNS to locate Domain Controllers and directory services.
- Forests provide the highest security and administrative boundary in Active Directory.
- Authentication verifies identity, while authorization determines access to resources.
- Server Roles define a server's primary function, while Features provide supporting capabilities.
- Proper documentation, snapshots, and validation are essential parts of enterprise change management.

---

## Next Mission

Mission #004 - Active Directory Organizational Units, Users, and Groups

The next mission will build the logical structure of the enterprise by creating Organizational Units (OUs), security groups, user accounts, and administrative delegation within the newly created Active Directory environment.