# Azure AD / Entra ID Lab

## Overview
This lab demonstrates my hands-on experience with cloud identity management in Azure AD / Entra ID.
It includes user and group management, MFA configuration, Conditional Access policies,
device registration, and basic Intune integration.

---

## 1. Tenant Setup
- Created a personal test tenant  
- Configured default domain settings  
- Added admin and standard test accounts  
- Configured global security defaults  

**Tools used:**  
Azure Portal → Entra ID, Security, Conditional Access  

---

## 2. User & Group Management

### Created test users such as:
- alice.hr@lab.onmicrosoft.com  
- bob.it@lab.onmicrosoft.com  
- test.user01–10  

### Created groups:
- **Security groups:** IT-Admins, HR-Staff, VPN-Users  
- **Microsoft 365 groups** for collaboration  

### Tasks performed:
- Assigning roles  
- Resetting passwords  
- Managing licenses (Microsoft 365 trial)  
- Applying least privilege principles  

---

## 3. MFA (Multi-Factor Authentication)

Configured MFA for:
- Individual users  
- Specific groups  
- Security defaults  

### Tested authentication methods:
- Microsoft Authenticator app  
- SMS  
- Backup codes  

### Tested scenarios:
- First-time MFA registration  
- MFA reset for a locked-out user  

---

## 4. Conditional Access Policies

Created and tested:
### ✔ Block legacy authentication  
- Prevents insecure sign-ins  
- Applied to all users except break-glass account  

### ✔ Require MFA for admins  
- Protects privileged roles  

### ✔ Location-based access  
- Block sign-ins from outside Lithuania  
- Allow trusted IP addresses  

### ✔ Require compliant device  
- Tested with basic Intune setup  

Each policy was validated using sign-in logs.

---

## 5. Device Registration & Intune (basic)

### Tested:
- Azure AD Join  
- Hybrid Azure AD Join (lab)  
- Viewing device information in Entra ID  
- Assigning a simple Intune compliance policy  

Compliance settings tested:
- Require password  
- Block rooted/jailbroken  
- Minimum OS version  

---

## 6. Sign-in Logs & Security Monitoring

Reviewed:
- User sign-in logs  
- Conditional Access outcomes  
- MFA results  
- Risky sign-ins (if any)  

Practiced interpreting errors:
- “MFA required but not configured”  
- “Blocked by Conditional Access”  
- “Legacy authentication blocked”  

---

## Screenshots  
_(Will be added soon)_  
- Azure portal dashboard  
- User management view  
- MFA registration  
- Conditional Access policies  
- Sign-in logs  

---

## Summary

This lab demonstrates practical experience in:  
- Cloud identity management  
- MFA deployment  
- Conditional Access policy design  
- User & group administration  
- Device registration & compliance  
- Troubleshooting cloud authentication  

More advanced Intune and automation labs will be added soon.
