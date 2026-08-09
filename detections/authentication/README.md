# Authentication & Brute-Force Detection

## Overview

Monitoring authentication activity across endpoints to identify repeated failed logins, potential brute-force attempts, suspicious authentication behavior, and account-related security events within the SOC.

## Detection Objectives

- Failed authentication monitoring
- Brute-force detection
- Repeated login failures
- Successful login after multiple failures
- Suspicious account activity
- Authentication anomalies
- Correlation with endpoint activity
- Identification of potentially compromised accounts

## Monitoring Workflow

```text
Windows / Linux Endpoint
          ↓
Authentication Events
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
