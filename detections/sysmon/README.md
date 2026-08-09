# Sysmon Endpoint Telemetry

## Overview

Sysmon provides detailed Windows endpoint telemetry that can be collected and analyzed through Wazuh for security monitoring, detection engineering, and SOC investigations.

## Detection Objectives

- Process creation monitoring
- Command-line activity monitoring
- Parent-child process analysis
- Network connection monitoring
- File activity monitoring
- Suspicious process detection
- PowerShell activity monitoring
- Endpoint event correlation
- Security investigation support

## Monitoring Workflow

```text
Windows Endpoint
       ↓
Sysmon
       ↓
Sysmon Event Logs
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
