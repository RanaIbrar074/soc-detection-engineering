# SOC Detection Engineering

A practical portfolio documenting **Security Operations Center (SOC) detection engineering, security monitoring, threat investigation, alert enrichment, endpoint telemetry, network detection, and security automation**.

This project is based on hands-on experience working with SIEM/XDR technologies and integrating multiple security data sources into a centralized monitoring and investigation workflow.

> ⚠️ **Security & Privacy Disclaimer**
>
> This repository contains sanitized examples, generalized architectures, and security methodologies.
>
> No confidential company information, production credentials, internal IP addresses, hostnames, customer information, proprietary configurations, or sensitive security data are included.

---

## 🛡️ SOC Detection & Monitoring Architecture

```text
                         ┌─────────────────────────┐
                         │        ENDPOINTS        │
                         │                         │
                         │ Windows / Linux Systems │
                         └────────────┬────────────┘
                                      │
                                      ▼
                         ┌─────────────────────────┐
                         │     SECURITY TELEMETRY  │
                         │                         │
                         │ • Sysmon                │
                         │ • Wazuh Agent           │
                         │ • Antivirus Logs        │
                         │ • USB / Device Events   │
                         │ • System Events         │
                         └────────────┬────────────┘
                                      │
                                      ▼
              ┌──────────────────────────────────────────┐
              │                 WAZUH                    │
              │              SIEM / XDR                  │
              │                                          │
              │ • Log Collection                         │
              │ • Detection Rules                        │
              │ • Correlation                            │
              │ • Alerting                               │
              │ • Endpoint Monitoring                    │
              │ • Active Response                        │
              └───────────────┬──────────────────────────┘
                              │
              ┌───────────────┼────────────────┐
              │               │                │
              ▼               ▼                ▼
      ┌──────────────┐ ┌──────────────┐ ┌──────────────┐
      │   Suricata   │ │ VirusTotal   │ │  Antivirus   │
      │     IDS      │ │ Threat Intel │ │    Alerts    │
      └──────┬───────┘ └──────┬───────┘ └──────┬───────┘
             │                │                │
             └────────────────┼────────────────┘
                              ▼
                    ┌─────────────────────┐
                    │  ALERT ENRICHMENT   │
                    │                     │
                    │ • IOC Analysis      │
                    │ • Reputation Checks  │
                    │ • Context Enrichment │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │  AI-ASSISTED SOC    │
                    │                     │
                    │ Ollama + Qwen3-4B    │
                    │ Local AI Analysis    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │     SOC ANALYST     │
                    │                     │
                    │ • Triage            │
                    │ • Investigation     │
                    │ • Validation        │
                    │ • Response          │
                    │ • Documentation     │
                    └─────────────────────┘
