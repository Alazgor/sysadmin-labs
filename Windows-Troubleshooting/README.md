🔧 1. Outlook Not Connecting to Exchange / M365

Symptoms:

“Trying to connect…”

Emails not sending

Slow startup

Diagnosis & Fix:

Check connection: Ctrl + right click Outlook → Test Email AutoConfiguration

Clear cached credentials

Reset Outlook profile

Check firewall / proxy

Confirm Autodiscover & DNS records

📌 Outcome: Restored stable Outlook connectivity.

🔧 2. No Internet / Limited Access (Windows 10/11)

Steps:

ipconfig /flushdns

Reset TCP/IP: netsh int ip reset

Check DHCP lease

Restart network services:
netsh winsock reset

Update network drivers

🔧 3. Printer Not Working / Offline

Steps:

Reinstall driver

Reset spooler:

net stop spooler
del C:\Windows\System32\spool\PRINTERS\* /Q
net start spooler


Re-add printer via TCP/IP port

Check permissions

🔧 4. RDP Not Working

Check that RDP service is enabled

Firewall rule: Remote Desktop – User Mode

Verify port 3389 listening:
netstat -ano | find "3389"

Check Network Level Authentication

🔧 5. Slow PC Performance

Solutions used:

Disable startup apps

Scan for disk errors

Clear temp files

Check Windows Update issues

Verify RAM & SSD health (CrystalDiskInfo)

🔧 6. Account / Password Issues (AD & Local)

Reset password via AD

Unlock user

Check GPO restrictions

Replication issues: repadmin /replsummary

🧰 Tools Used

Event Viewer

Windows Admin Center

PowerShell

Remote Desktop

AnyDesk / TeamViewer

ServiceNow, Jira, FreshService (ticketing)
