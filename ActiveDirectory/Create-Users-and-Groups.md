# Create Users, Organizational Units and Groups in Active Directory

## Goal  
Set up a basic AD structure with separate OUs for departments and create users with correct group membership.

---

## Steps  

### 1. Create new Organizational Units
```powershell
New-ADOrganizationalUnit -Name "Users" -Path "DC=lab,DC=local"
New-ADOrganizationalUnit -Name "IT" -Path "OU=Users,DC=lab,DC=local"
New-ADOrganizationalUnit -Name "HR" -Path "OU=Users,DC=lab,DC=local"
```

### 2. Create security groups
```powershell
New-ADGroup -Name "IT-Admins" -GroupScope Global -Path "OU=IT,OU=Users,DC=lab,DC=local"
New-ADGroup -Name "HR-Staff" -GroupScope Global -Path "OU=HR,OU=Users,DC=lab,DC=local"
```

### 3. Create users
```powershell
New-ADUser -Name "John Doe" -SamAccountName jdoe -AccountPassword (Read-Host -AsSecureString) -Enabled $true -Path "OU=IT,OU=Users,DC=lab,DC=local"
Add-ADGroupMember -Identity "IT-Admins" -Members jdoe
```

### 4. Result

- Proper OU structure  
- Users with roles  
- Groups for access control
