**#  Cyber Security Internship – Task 4**
## Task Title:
**Setup and Use a Firewall on Linux using UFW**

## Objective:
Configure and test basic firewall rules to allow or block traffic using UFW (Uncomplicated Firewall) on a Kali Linux system.

## System Used:
- **OS**: Kali Linux
- **Firewall Tool**: UFW

## 🛠Steps Performed:

1. **Enabled UFW:**
   ```bash
   sudo ufw enable
   ```
2. **Checked Firewall Status:**
   ```bash
   sudo ufw status verbose
   ```
3. **Allowed SSH (port 22):**
   ```bash
   sudo ufw allow 22
   ```
4. **Blocked Telnet (port 23):**
   ```bash
   sudo ufw deny 23
   ```
5. **Tested Connection to Port 23:**
   ```bash
   telnet localhost 23
   ```
   - Output: `Connection refused`

6. **Removed Telnet Rule (Restore):**
   ```bash
   sudo ufw delete deny 23
   ```
## Files Included:
- `firewall_report.txt`: A text summary of steps and commands used
- `Screenshot of UFW(1).png`: Terminal output screenshot

## Key Learnings:
- How UFW manages incoming and outgoing traffic
- Why blocking insecure ports like 23 (Telnet) is important
- Use of firewall rules to enhance system security

## Status:
**Task Completed Successfully**

