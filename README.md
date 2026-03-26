# SOC Home Lab with Wazuh SIEM

## Overview
This project demonstrates a Security Operations Center (SOC) home lab built using Wazuh SIEM. The lab simulates real-world attack scenarios and analyzes how security events are detected and logged.

## Lab Setup
- SIEM: Wazuh (Ubuntu)
- Victim Machine: Windows
- Attacker Machine: Kali Linux

## Network
- SIEM: 192.168.116.129
- Victim: 192.168.116.128
- Attacker: 192.168.116.130

## Attacks Simulated

### 1. SMB Brute Force Attack
- Repeated login attempts against Windows using SMB
- Generated multiple failed logon events
- Detected in Wazuh with severity escalation (level 5 → 10)

### 2. RDP Brute Force Attack
- Simulated login attempts using Hydra
- Generated authentication failure logs
- Detected in Wazuh as repeated logon failures

## Detection & Analysis
- Monitored events using Wazuh dashboard
- Analyzed Windows Event ID 4625 (failed logon)
- Identified attacker IP and target account
- Observed escalation in alert severity

## Screenshots
(Add screenshots here)

## Skills Demonstrated
- SIEM monitoring (Wazuh)
- Log analysis and alert investigation
- Attack simulation (SMB, RDP)
- Basic incident detection and analysis
