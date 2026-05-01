# nxc-sweep
Bash wrapper for NetExec to quickly validate compromised credentials across SMB, WinRM, RDP, MSSQL, and FTP

Instead of manually testing services one by one, this script utilizes `netcat` to pre-check port states speeding up the enumeration process. It then fires `NetExec (nxc)` across all active protocols, instantly highlighting the specified user's privileges for each.


## Features
- **Quick Port Validation:** Uses `nc` to verify port status before checking the protocol with `nxc`
- **Protocol Suite:** Automatically sweeps `SMB`, `WinRM`, `RDP`, `MSSQL`,** and `FTP`.
- **Versatile Targeting:** Seamless use in both **Active Directory** and standalone **Windows** environments
- **Dynamic Flag Passing:** Pass any native NetExec flags (e.g., `--local-auth`) directly through the wrapper
- **Clean Output:** Preserves native NetExec color coding for easy readability of (Pwn3d!) and share permissions


## Installation
For system-wide accessibility, use this one-liner to download the script, apply execution permissions, and move it into your $PATH:
```
test
```