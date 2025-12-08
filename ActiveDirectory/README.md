# Active Directory Lab

## Overview
This lab demonstrates my practical experience with deploying and managing a Windows Server Active Directory environment.  
It includes domain creation, user and group management, OU structure design, and Group Policy configuration.

---

## 1. Domain Setup
- Installed Windows Server 2022 as Domain Controller  
- Created domain: **lab.local**  
- Configured DNS service  
- Enabled automatic DHCP addressing for test machines  

**Tools used:**
- Server Manager  
- Active Directory Domain Services  
- DNS Manager  

---

## 2. Organizational Unit (OU) Structure
Created a clean, realistic structure:

- **Users**
  - IT  
  - HR  
  - Management  
  - Temporary Users  

- **Computers**
  - Workstations  
  - Laptops  

---

## 3. User & Group Management
Examples:

- Created 15 test users  
- Created security groups:
  - IT-Admins  
  - HR-Staff  
  - VPN-Users  
  - Finance-ReadOnly  

**Tasks performed:**
- Password resets  
- Unlocking accounts  
- Modifying group membership  
- Applying least privilege principles  

---

## 4. Group Policy Objects (GPO)
Implemented and tested:

### ✔ Password & Security Policy
- Minimum password length  
- Lockout policy  
- Disable guest accounts  

### ✔ Desktop Environment Policy
- Custom wallpaper  
- Hide control panel  
- Map network drives  

### ✔ Software Restrictions
- Block unwanted .exe files  
- Allow only approved applications  

---

## 5. Testing Environment
I set up test Windows 10 / 11 VMs to validate:

- AD join  
- GPO application  
- Network drive mapping  
- Permissions and access control  

---

## Screenshots
_(Will be added soon)_  
- ADUC (Active Directory Users and Computers)  
- OU structure  
- GPO configuration  
- Domain join confirmation  

---

## Summary
This lab demonstrates practical experience in:
- Deploying Active Directory  
- Managing users and groups  
- Designing OU structures  
- Configuring and testing GPO  
- Troubleshooting Windows domain issues  

More advanced labs will be added soon.

