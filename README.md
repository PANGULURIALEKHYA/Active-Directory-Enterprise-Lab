# Active Directory Enterprise Lab

| | |
|---|---|
| **Title** | Active Directory Enterprise Lab |
| **Description** | Enterprise-style Active Directory project demonstrating Windows Server domain administration, organizational unit management, user and security group administration, domain joining, and centralized authentication. |
| **Author** | Alekhya Panguluri |

---

# Introduction

This project demonstrates the deployment and administration of a Windows Active Directory environment using Windows Server and a Windows 10 client.

The lab simulates a small enterprise environment where users, departments, security groups, and workstations are centrally managed through Active Directory Domain Services (AD DS).

A Windows 10 client was successfully joined to the domain and domain-user authentication was tested and verified.

---

# Skills Used

- Active Directory Domain Services (AD DS)
- Windows Server Administration
- Domain Controller Configuration
- DNS Configuration
- Active Directory Users and Computers (ADUC)
- Organizational Unit (OU) Management
- User Account Administration
- Security Group Management
- Group Membership Administration
- Windows Domain Joining
- Domain Authentication
- Identity and Access Management

---

# Lab Environment

| Component | Configuration |
|---|---|
| **Virtualization** | Oracle VirtualBox |
| **Domain Controller** | Windows Server |
| **Client Machine** | Windows 10 |
| **Domain** | apex.local |
| **Domain Controller Name** | AD-DC01 |
| **Services** | Active Directory Domain Services (AD DS), DNS |

---

# Active Directory Structure

The `apex.local` domain was configured with an enterprise-style organizational structure.

Organizational Units were created for:

- HR
- Finance
- IT
- Sales
- Servers
- Workstations
- Security Groups

This structure demonstrates how Active Directory can organize and centrally manage users, computers, groups, and other resources.

---

# User Account Management

Multiple domain user accounts were created and organized within departmental Organizational Units.

The HR OU, for example, contains domain users including:

- Ava Taylor
- Emma Brown
- Emma Murphy
- Liam Moore
- Noah Wilson
- Olivia Davis

This demonstrates centralized user account creation and administration using Active Directory Users and Computers.

---

# Security Group Management

Security groups were created to provide department-based and role-based account management.

Configured groups include:

- `Finance_Users`
- `HR_Users`
- `IT_Admins`
- `Sales_Users`

Users were assigned to appropriate security groups to simulate enterprise access management.

---

# Group Membership Validation

The `HR_Users` security group was configured with the appropriate HR domain accounts.

Group membership was verified through Active Directory Users and Computers, demonstrating centralized management of user access through security groups.

---

# Domain Client Integration

A Windows 10 workstation was successfully connected to the `apex.local` Active Directory domain.

Domain authentication was validated using a domain user account.

The following command was used:

`whoami`

The authenticated identity returned:

`apex\emma.murphy`

Domain membership was additionally verified using:

`systeminfo | findstr /B /C:"Domain"`

Result:

`Domain: apex.local`

This confirms that the Windows 10 workstation was successfully joined to the Active Directory domain.

---

# Project Outcomes

The lab successfully demonstrated:

- Deployment of Active Directory Domain Services
- Configuration of a Windows Server Domain Controller
- DNS integration
- Creation of an enterprise-style OU structure
- Centralized domain user administration
- Creation and management of security groups
- Assignment of users to departmental groups
- Windows 10 domain integration
- Successful domain-user authentication
- Verification of domain membership

---

# Project Evidence

Technical evidence from the lab is available in the **screenshots** folder.

The screenshots demonstrate:

1. Domain user login verification
2. Domain membership verification
3. Active Directory organizational structure
4. HR domain user accounts
5. Active Directory security groups
6. HR security group membership
7. Active Directory Domain Services running on the Domain Controller

---

# Documentation

Detailed project documentation is available in the **docs** folder.

The technical report contains additional information about the lab architecture, configuration, implementation, testing, and project results.

---

# Conclusion

This project provided hands-on experience with Active Directory administration in a simulated enterprise environment.

The completed lab demonstrates practical knowledge of Windows Server, Active Directory Domain Services, organizational units, user and group administration, domain integration, and centralized identity management.
