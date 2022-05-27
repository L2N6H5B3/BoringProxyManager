# BoringProxyManager
Manage BoringProxy Tunnels with a Windows Service



## Preparation (required if you have a flakey connection)
1. SSH into Ubuntu / Linux Server in the cloud
2. Add the following to /etc/sysctl.conf:
```
# TCP SYN Flood Protection
net.ipv4.tcp_syncookies = 1
net.ipv4.tcp_max_syn_backlog = 2048
net.ipv4.tcp_synack_retries = 3
```
3. Restart

## Installation
1. Note the names of tunnels you wish to monitor
