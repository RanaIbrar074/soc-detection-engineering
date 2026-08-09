# AI-Assisted SOC Analysis

## Overview

Local AI-assisted security analysis using Ollama and Qwen3-4B to support SOC analysts during alert triage, investigation, and security-event analysis.

## Objectives

- Alert summarization
- Security-event interpretation
- Investigation assistance
- Detection analysis
- IOC analysis
- Investigation notes
- Natural-language analysis of security telemetry
- Faster initial alert triage

## Architecture

```text
Wazuh Alert
     ↓
Alert / Event Data
     ↓
AI Processing
     ↓
Ollama
     ↓
Qwen3-4B
     ↓
AI-Assisted Analysis
     ↓
SOC Analyst Validation
     ↓
Investigation / Response
