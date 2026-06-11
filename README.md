# HomeLab — Virtual Enterprise Network

## Overview
A virtual enterprise network built in Oracle VirtualBox simulating 
a real-world enterprise environment. Designed to demonstrate 
networking, identity management, and security skills for 
Network Engineer and SOC Analyst roles.

## Network Topology
*(Diagram coming soon)*

## VM Inventory
| VM | OS | IP | Role |
|---|---|---|---|
| OPNsense-FW | FreeBSD | 192.168.10.1 | Firewall / Router |
| WinServer2022-DC | Windows Server 2022 | 192.168.10.10 | AD, DNS, DHCP |
| Ubuntu-Client01 | Ubuntu 26.04 LTS | 192.168.10.20 | Domain Client |

## Technologies Demonstrated
- OPNsense firewall with LAN/DMZ segmentation and firewall rules
- Active Directory Domain Services with OU structure and GPOs
- DNS and DHCP managed via Windows Server 2022
- Ubuntu Linux domain-joined workstation via realmd/SSSD
- OpenVPN remote access tunnel *(in progress)*

## Key Configurations
- AD Domain: homelab.local
- LAN Subnet: 192.168.10.0/24
- DMZ Subnet: 192.168.20.0/24
- DHCP Range: 192.168.10.100 - 192.168.10.200

## GPOs Configured
- Password-Policy: 12 char minimum, complexity required
- HR-LockScreen-Policy: 5 minute timeout
- HR-Block-USB: Removable storage denied for HR OU

## Lessons Learned
*(Update this as I go)*



