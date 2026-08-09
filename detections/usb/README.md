# USB & Removable Device Monitoring

## Overview

Monitoring USB and removable-device activity on endpoints to provide SOC visibility into device connections and potential file/data transfer activity.

This detection capability is designed to help SOC analysts identify and investigate potentially suspicious activity involving removable storage devices.

## Detection Objectives

- USB device connection
- USB device removal
- Removable storage activity
- File-copy activity
- Suspicious file transfers
- Potential data-transfer activity
- Endpoint events associated with removable devices

## Monitoring Workflow

```text
USB / Removable Device
          ↓
Windows Endpoint
          ↓
Endpoint Telemetry
          ↓
Wazuh Agent
          ↓
Wazuh Manager
          ↓
Detection Rule
          ↓
SOC Alert
          ↓
Analyst Investigation
