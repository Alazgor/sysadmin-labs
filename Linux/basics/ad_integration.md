# Linux integration with Active Directory (basic)

## What I did
- Joined Linux VM to Active Directory using realm
- Verified domain membership
- Tested domain users login

## Commands used
- kinit user@CORP.LOCAL
- ### Kerberos authentication test

After joining the Linux system to Active Directory, Kerberos authentication was verified using:

```bash
kinit user@CORP.LOCAL
klist
```

- timedatectl
- realm list
- realm discover domain.local
- realm join domain.local -U admin_user
- id domainuser@domain.local

## Notes
- Initial join was successful
- Some issues with DNS and time sync occurred
- Issues were resolved by checking:
  - resolv.conf
  - chrony / time synchronization
  
### Kerberos notes

- Kerberos uses time-sensitive tickets (TGT)
- Correct DNS and time sync are mandatory
- Authentication is ticket-based, passwords are not transmitted
- Used by Active Directory for secure authentication

