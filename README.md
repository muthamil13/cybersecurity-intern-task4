# cybersecurity-intern-task4
# Firewall Configuration on Kali Linux using UFW

## Objective
The objective of this task is to configure basic firewall rules using UFW (Uncomplicated Firewall) on Kali Linux, specifically to block inbound traffic on port 23 (Telnet) and allow SSH access (Port 22).

## Steps Taken

1. **Install UFW**:
   - Checked if UFW was installed with `ufw --version`.
   - Installed UFW using `sudo apt install ufw`.

2. **Check Current UFW Status**:
   - Ran `sudo ufw status verbose` to verify the current firewall status.

3. **Block Telnet (Port 23)**:
   - Added a rule to block incoming traffic on port 23 using `sudo ufw deny in 23`.
   - Tested the rule using the `telnet` command and confirmed that the connection was refused.

4. **Allow SSH (Port 22)**:
   - Added a rule to allow incoming SSH traffic on port 22 using `sudo ufw allow 22`.

5. **Remove Telnet Block Rule**:
   - Removed the Telnet block rule using `sudo ufw delete deny in 23`.
   - Verified the removal with `sudo ufw status`.

## Screenshots/Configuration File

### Firewall Rules After Configuration:
```bash
sudo ufw status

