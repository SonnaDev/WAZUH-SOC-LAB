# WAZUH-SOC-LAB
A hands-on project focused on deploying an open-source SIEM (Wazuh) to monitor, detect, and analyze security events on a Windows endpoint.

# 🛡️ Building a Security Operations Center (SOC) Lab with Wazuh

<img width="1872" height="562" alt="waz_cap" src="https://github.com/user-attachments/assets/a101fb16-3278-4d47-8d0d-23749904ce14" />
<img width="1917" height="896" alt="sev_dash" src="https://github.com/user-attachments/assets/4b6af2b7-556b-4da7-8d03-41af4f176f95" />
<img width="1915" height="908" alt="login_cap" src="https://github.com/user-attachments/assets/53949167-8836-45e6-b6bd-e3fb66b7218e" />
<img width="1897" height="675" alt="home_cap" src="https://github.com/user-attachments/assets/d1c87f5a-054f-403a-906d-d74750489dd7" />
<img width="1052" height="205" alt="cap_flag" src="https://github.com/user-attachments/assets/bcf3c7f7-162f-4c5d-8ba1-ceb682ff0b6a" />

## 🏗️ Architecture
- **SIEM/Manager:** Ubuntu Server 22.04 LTS (Running Wazuh Manager, Indexer, and Dashboard)
- **Endpoint (Victim):** Windows 11 Home/Pro (Running Wazuh Agent)
- **Network:** Isolated VirtualBox Network

## 🛠️ Key Tasks Performed
- **SIEM Deployment:** Installed and configured the Wazuh stack on an Ubuntu Linux server.
- **Troubleshooting:** Resolved "API Connection Down" errors by analyzing system logs (`journalctl`) and optimizing VM resource allocation (increasing RAM to 8GB).
- **Agent Enrollment:** Deployed the Wazuh agent to a Windows host via PowerShell with administrative privileges.
- **Threat Simulation:** Conducted a successful brute-force simulation (logon failures) to verify real-time alerting.

## 📊 Results & Evidence
*Insert screenshots here:*
1. **Agent Status:** Screenshot showing the 'Active' green status for your Windows agent.
2. **Security Events:** Screenshot showing the dashboard spike from your failed login test.

## 🧠 Lessons Learned
- Importance of resource management in virtualized security environments.
- Understanding the flow of telemetry from an endpoint to a centralized dashboard.
- Practical experience with Windows Event IDs (specifically Event ID 4625 for logon failure).
