🐧 Linux Administration Labs

This section collects common Linux administration tasks and troubleshooting steps.

🔑 Users & Permissions

useradd, usermod, passwd

groups, chown, chmod

sudo configuration: /etc/sudoers

🔥 Services & Systemctl

Examples:

systemctl status ssh
systemctl restart nginx
systemctl enable firewalld

📦 Package Management

Ubuntu / Debian:

apt update
apt install package


RHEL / Rocky:

dnf install package

🧱 Firewall (ufw / firewalld)
ufw enable
ufw allow 22
firewall-cmd --add-service=ssh --permanent

📄 Logs & Monitoring
journalctl -xe
tail -f /var/log/syslog
df -h
top / htop

🌐 Networking
ip addr
ip route
nmcli d
ping / traceroute

🔒 SSH Hardening

Disable root login

Use key-based auth

Change default port

🎯 Next Tasks

Add screenshots

Add 1–2 full Linux projects

Add bash scripts
