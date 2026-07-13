# Threat-Detection-Home-Lab

A self-built SOC lab simulating real-world attacks and detecting them 
using Sysmon, Windows Event Logs, and the Wazuh SIEM platform.

## Architecture
- **Attacker**: Kali Linux VM (Nmap, Hydra)
- **Victim**: Windows 11 VM with Sysmon (SwiftOnSecurity config)
- **SIEM**: Wazuh Manager + Dashboard (Kali Linux)
- Network: VirtualBox internal network (192.168.56.0/24) + NAT for internet access

## What I Built
1. Deployed and configured Sysmon on Windows for deep endpoint visibility
2. Installed Wazuh SIEM (indexer, manager, dashboard) on Kali Linux
3. Connected Windows as a monitored Wazuh agent
4. Simulated real attacker behavior:
   - Nmap reconnaissance scan
   - SMB brute-force attempt via Hydra
5. Verified and correlated attack activity in Wazuh's Discover module

## Screenshots
[Overview Dashboard]
<img width="1920" height="1200" alt="VirtualBox_kali linux 1_12_07_2026_23_30_19" src="https://github.com/user-attachments/assets/949ae2a4-6b12-4a3e-8393-863a732df562" />
[Agent Connected]
<img width="1920" height="1200" alt="VirtualBox_kali linux 1_12_07_2026_23_31_35" src="https://github.com/user-attachments/assets/1a5f8525-6481-49d5-97de-5116d241f953" />
[Log Correlation]
<img width="1920" height="1200" alt="VirtualBox_kali linux 1_12_07_2026_23_40_31" src="https://github.com/user-attachments/assets/a34d70c3-9c55-4ab6-a27b-9fe6459cd3ac" />
[Sysmon Live Logging]
<img width="1920" height="1200" alt="VirtualBox_kali linux 1_12_07_2026_23_25_40" src="https://github.com/user-attachments/assets/e191866d-d1db-4f20-8a3a-5626346a06ef" />


## Key Skills Demonstrated
SIEM deployment · Log analysis · Detection engineering · Network 
troubleshooting · Windows/Linux administration · Incident documentation

## What I'd Improve Next
- Custom Wazuh detection rules for stealthier scans
- MITRE ATT&CK technique mapping
- Automated alerting (email/Slack webhook)

