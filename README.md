# SOC-Home-Lab
A functional SOC Home Lab featuring an ELK/Wazuh SIEM integration, automated telemetry collection, and simulated attack-defense scenarios to demonstrate threat detection and incident response.

# SOC Home Lab: Threat Detection & SIEM Integration

## Objective
The goal of this project was to build a functional Security Operations Center (SOC) environment to observe real-time telemetry, analyze security events, and strengthen my understanding of the **Incident Response** lifecycle.

## Tools & Technologies Used
- **SIEM:** Wazuh / Splunk / ELK Stack (Pick one)
- **Virtualization:** Oracle VirtualBox / VMware
- **Endpoint:** Windows 10 (Target) & Ubuntu Server (Manager)
- **Attack Tool:** Kali Linux (Nmap, Metasploit)
- **Network:** Internal Virtual Network (Host-only)

## Lab Architecture
1. **The Manager:** [Wazuh Manager] - Centralized log collection and analysis.
2. **The Agent:** [Windows 10] - Configured with Sysmon for deep event logging.
3. **The Attacker:** [Kali Linux] - Used to simulate brute-force and port scanning.

## Key Activities & Screenshots
### 1. Endpoint Monitoring
*Configured Sysmon to track process creation and network connections.*
[INSERT SCREENSHOT OF SYSMON LOGS HERE]

### 2. Threat Detection
*Simulated a Brute Force attack from Kali. Below is the SIEM dashboard showing the triggered 'Multiple Failed Login' alerts.*
[INSERT SCREENSHOT OF SIEM ALERT HERE]

### 3. Incident Analysis
*Identified the Source IP of the attacker and documented the 'Indicator of Compromise' (IOC).*

## Lessons Learned
- Gained hands-on experience with **log ingestion** and parsing.
- Learned the importance of **Sysmon** for visibility into Windows environments.
- Developed a workflow for triaging alerts based on severity.
