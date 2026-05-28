# SOC Lab — Wazuh + ELK Stack

Blue Team home lab focused on threat detection, log correlation and security monitoring using Wazuh SIEM and ELK Stack.

---

## Overview

This laboratory was built to simulate a basic SOC (Security Operations Center) environment for monitoring and investigating Windows security events.

The environment includes:
- Wazuh SIEM
- ELK Stack
- Windows Event Monitoring
- MITRE ATT&CK Mapping
- Threat Detection
- Authentication Monitoring

---

## Technologies Used

- Wazuh
- ELK Stack
- Ubuntu Server
- Windows 10
- VirtualBox

---

## Security Capabilities

- Log Analysis
- Event Correlation
- Threat Detection
- Authentication Monitoring
- MITRE ATT&CK Mapping
- Security Event Monitoring

---

## Sysmon + Wazuh Threat Hunting

This section demonstrates the integration between Sysmon and Wazuh SIEM for endpoint telemetry collection and threat detection.

### Objective

Monitor suspicious PowerShell activity and analyze process creation events using Sysmon Event ID 1.

### Simulated Activity

```powershell
powershell -w hidden -ep bypass
```

### Detection Pipeline

Windows Endpoint
→ Sysmon
→ Wazuh Agent
→ Wazuh SIEM
→ MITRE ATT&CK Mapping

### Detection Results

* PowerShell execution detected
* Sysmon Event ID 1 generated
* Wazuh SIEM correlated the event
* MITRE ATT&CK technique identified
* Threat Hunting performed through Wazuh Dashboard

### MITRE ATT&CK Techniques

* T1059.001 — PowerShell

### Skills Practiced

* Threat Hunting
* Endpoint Telemetry Analysis
* SIEM Monitoring
* Event Correlation
* PowerShell Detection
* MITRE ATT&CK Analysis
* Detection Engineering

### Screenshots

#### Sysmon Event ID 1

#### Wazuh SIEM Dashboard

#### Security Alerts and MITRE Mapping

## Screenshots

### Wazuh Dashboard
<img width="100%" src="./Captura de tela 2026-05-28 094956.png">

---

### Security Events Monitoring
<img width="100%" src="./Captura de tela 2026-05-28 095444.png">

---

## Future Improvements

- Brute Force Simulation
- Custom Detection Rules
- Active Directory Integration
- Incident Response Scenarios
- Sysmon Integration

---

## Author

Gustavo Braga

