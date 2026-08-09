# PowerShell Activity Detection

## Overview

Monitoring PowerShell activity on Windows endpoints to identify suspicious command execution, script activity, and potential abuse of PowerShell within the SOC environment.

## Detection Objectives

- PowerShell execution monitoring
- Suspicious command-line activity
- Script execution monitoring
- Encoded or obfuscated PowerShell activity
- Unusual PowerShell usage
- Correlation with other endpoint events
- Identification of potential malicious execution

## Monitoring Workflow

```text
Windows Endpoint
       ↓
PowerShell Activity
       ↓
Sysmon / Windows Telemetry
       ↓
Wazuh Agent
       ↓
Wazuh Manager
       ↓
Detection / Correlation
       ↓
Wazuh Dashboard
       ↓
SOC Alert
       ↓
Analyst Investigation
