# Wazuh Active Response

## Overview

Wazuh Active Response can be used to automatically execute predefined response actions when specific security events or detection rules are triggered.

This capability helps reduce response time by allowing the SOC environment to react to selected threats automatically while maintaining analyst oversight.

## Response Workflow

```text
Security Event
      ↓
Wazuh Detection Rule
      ↓
Alert Generated
      ↓
Active Response Trigger
      ↓
Automated Response
      ↓
SOC Analyst Review
      ↓
Investigation / Follow-up
