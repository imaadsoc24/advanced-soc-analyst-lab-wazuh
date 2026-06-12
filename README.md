# Advanced SOC Analyst Investigation Lab

## Overview

This project documents a hands-on SOC investigation and threat hunting exercise conducted using Wazuh, Sysmon, Wireshark, VirusTotal, and MITRE ATT&CK.

The objective of the lab was to investigate suspicious endpoint activity, validate indicators, analyze process execution events, review network communications, and correlate alerts from multiple security tools to understand the complete attack path.

Rather than analyzing alerts individually, the investigation focused on building context across endpoint, network, and threat intelligence data to determine how different events were related.

---

## Tools Used

- Wazuh SIEM
- Sysmon
- Wireshark
- VirusTotal
- MITRE ATT&CK Framework

---

## Investigation Activities

- Endpoint monitoring and alert analysis
- Sysmon process creation investigation
- PowerShell execution analysis
- Parent-child process tracing
- File Integrity Monitoring (FIM) review
- DNS traffic analysis
- HTTPS/TLS communication analysis
- VirusTotal reputation validation
- MITRE ATT&CK technique mapping
- Threat hunting and IOC validation

---

## Key Findings

### Suspicious Command Execution
A Windows command shell process was identified and investigated through Sysmon process creation events.

### PowerShell Activity Analysis
Multiple PowerShell execution events were reviewed, including process relationships and execution behavior.

### File Creation Monitoring
Suspicious files created within monitored directories were analyzed through Sysmon and File Integrity Monitoring events.

### Network Investigation
Wireshark was used to analyze DNS queries, TLS handshakes, and outbound HTTPS communications.

### Threat Intelligence Correlation
Files and indicators were validated through VirusTotal integration to determine reputation and detection status.

### MITRE ATT&CK Mapping
Observed activity was mapped to relevant MITRE ATT&CK tactics and techniques to provide additional context during the investigation.

---

## Skills Demonstrated

- Security Monitoring
- Log Analysis
- Threat Hunting
- Incident Investigation
- IOC Validation
- Network Traffic Analysis
- Endpoint Detection Analysis
- MITRE ATT&CK Mapping
- Security Event Correlation

---

## Screenshots

Investigation screenshots and supporting evidence are available in the **Screenshots** directory.

---

## Key Takeaway

One of the most valuable lessons from this lab was understanding how individual alerts become significantly more meaningful when correlated together. Reviewing endpoint events, network telemetry, and threat intelligence as part of a single investigation provides a much clearer picture than analyzing isolated alerts.

This exercise strengthened practical SOC investigation skills, threat hunting methodology, and security event correlation techniques commonly used by security analysts in real-world environments.
