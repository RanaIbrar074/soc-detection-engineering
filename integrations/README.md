# SOC Integrations

## Overview

This section documents security integrations used to enhance the SOC monitoring and investigation workflow.

The integrations connect Wazuh with endpoint telemetry, network security, threat intelligence, notifications, and local AI-assisted analysis.

## Integration Architecture

```text
Security Sources
       ↓
Wazuh
       ↓
Detection & Correlation
       ↓
┌───────────────────────────────┐
│        SOC Integrations       │
│                               │
│ • VirusTotal                  │
│ • Suricata                    │
│ • Antivirus                   │
│ • Sysmon                      │
│ • Ollama + Qwen3-4B           │
│ • Notification / Automation   │
└───────────────┬───────────────┘
                ↓
         SOC Analyst
