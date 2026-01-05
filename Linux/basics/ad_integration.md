# Linux integration with Active Directory (basic)

## What I did
- Joined Linux VM to Active Directory using realm
- Verified domain membership
- Tested domain users login

## Commands used
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
