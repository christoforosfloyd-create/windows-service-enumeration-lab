# Windows Service Enumeration Lab

## Objective
Build a Windows and Kali Linux lab in VirtualBox and perform host discovery and service enumeration.

## Lab Environment

- Host OS: Windows 10
- Hypervisor: VirtualBox
- Target VM: Windows 11 Pro
- Attacker VM: Kali Linux
- Network: Host-Only Adapter

## Tools Used

- Nmap
- PowerShell
- Windows Defender Firewall
- VirtualBox

## Network Configuration

| Device | IP Address |
|---------|-------------|
| Kali Linux | 192.168.56.101 |
| Windows 11 | 192.168.56.102 |

## Initial Nmap Scan

The initial scan showed:

- Host reachable
- All ports filtered
- Windows Firewall blocking enumeration

## Service Enumeration Results

Open ports discovered:

- 135/tcp - Microsoft RPC
- 139/tcp - NetBIOS
- 445/tcp - SMB

## SMB Findings

- SMB Version: 3.1.1
- SMB Signing: Enabled and Required

## Security Assessment

SMB services were exposed for testing purposes. SMB signing was enabled, reducing the risk of SMB relay attacks.

## Skills Demonstrated

- Virtualization
- Windows Administration
- Linux Administration
- Networking
- Nmap Enumeration
- Security Analysis
