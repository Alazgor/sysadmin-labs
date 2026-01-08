- Rocky Linux with 2 NICs (NAT + Host-only)
- DHCP on both interfaces
- Default route via NAT
- Internal network for AD / lab communication
- resolvectl warning explained (systemd-resolved not used)

#code

- ip a
- ip route
- nmcli device status
- cat /etc/resolv.conf
