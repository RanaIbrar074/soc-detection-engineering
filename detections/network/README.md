# Network Threat Detection

## Overview

Network security monitoring and threat detection using network telemetry and IDS alerts integrated into the SOC monitoring workflow.

This detection capability provides visibility into suspicious network activity, reconnaissance, malicious traffic, and potential network-based threats.

## Detection Objectives

- Network intrusion detection
- Port scanning detection
- Network reconnaissance monitoring
- Suspicious connection detection
- Malicious traffic detection
- IDS alert monitoring
- Unusual communication patterns
- Correlation of network events with endpoint activity

## Monitoring Workflow

```text
Network Traffic
       ↓
Suricata IDS
       ↓
Network Security Events
       ↓
Wazuh Agent / Log Collection
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
