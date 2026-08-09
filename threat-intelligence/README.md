# Threat Intelligence & IOC Enrichment

## Overview

Threat intelligence is used to enrich SOC alerts and provide additional context during security investigations.

This workflow helps analysts investigate suspicious:

- File hashes
- IP addresses
- Domains
- URLs
- Email indicators
- Malware-related artifacts
- Network indicators

The objective is not to automatically label every indicator as malicious. Instead, indicators are enriched with external reputation and contextual information so that analysts can make better-informed decisions.

---

## Intelligence Workflow

```text
Wazuh Alert
     |
     v
Suspicious Indicator
     |
     v
Indicator Extraction
     |
     v
Threat Intelligence Lookup
     |
     v
Reputation / Detection Results
     |
     v
Analyst Validation
     |
     +----------------------+
     |                      |
     v                      v
 Malicious              Benign / Unknown
     |                      |
     v                      v
Incident Escalation     Continue Monitoring
     |
     v
Response / Containment
