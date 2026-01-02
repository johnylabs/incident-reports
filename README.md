# SOC Incident Reports

This repository contains **realistic, end-to-end SOC incident investigations** based on alerts generated in lab environments (Wazuh, Suricata, cloud logs).

Each case documents how I work as a SOC analyst from **initial alert → investigation → escalation → resolution**, following Tier 1–2 SOC workflows.

---

## What This Demonstrates

Each incident report shows:

- Alert triage and validation  
- Evidence collection and correlation  
- Timeline reconstruction  
- MITRE ATT&CK technique mapping  
- Clear written communication for escalation and reporting  

The reports are written to mirror **operational SOC documentation** used by security teams.

---

## Repository Structure

incident-reports/
├── README.md
├── docs/
│   ├── methodology.md
│   ├── report-lifecycle.md
│   └── severity-matrix.md
├── templates/
│   ├── report-template.md
│   ├── timeline-template.md
│   └── customer-summary-template.md
├── cases/
│   ├── 2025-01-lab-ssh-bruteforce/
│   │   ├── report.md
│   │   ├── timeline.md
│   │   ├── mitre-mapping.md
│   │   └── evidence/
│   │       ├── logs/
│   │       └── screenshots/
│   └── 2025-XX-/
└── exports/
└── redacted/
