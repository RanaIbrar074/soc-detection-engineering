# Threat Intelligence & IOC Enrichment

## Overview

Threat intelligence is used to enrich SOC alerts and provide additional context during security investigations.

This workflow can help analysts investigate suspicious files, hashes, IP addresses, domains, and URLs associated with security alerts.

## Intelligence Workflow

```text
Wazuh Alert
      ↓
Suspicious Indicator
      ↓
Indicator Extraction
      ↓
Threat Intelligence Lookup
      ↓
Reputation / Detection Results
      ↓
Alert Enrichment
      ↓
SOC Analyst Investigation
      ↓
Final Assessment
