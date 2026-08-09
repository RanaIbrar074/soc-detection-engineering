# Antivirus Alert Monitoring

## Overview

Centralized monitoring of antivirus and endpoint-security alerts through Wazuh to provide SOC visibility into malware detections, suspicious files, and endpoint security events.

## Detection Objectives

- Malware detection monitoring
- Suspicious file detection
- Antivirus alerts
- Quarantined threat monitoring
- Endpoint security events
- Detection severity monitoring
- Affected endpoint identification
- Correlation with other security events

## Monitoring Workflow

```text
Antivirus / Endpoint Security
          ↓
Windows Endpoint
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
