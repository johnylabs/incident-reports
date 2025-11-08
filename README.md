# 🧾 incident-reports

Structured SOC incident reports from my lab environments  
(Wazuh, Suricata, lab-core-network, ug-aws-hybrid-soc-lab, etc.).

Each report is a **full story** from detection → triage → containment → recovery → lessons learned, written like a real SOC case.

This repo is for:

- Practicing **professional-grade incident reporting**
- Building a portfolio of **realistic SOC cases**
- Feeding future tools (e.g. `ai-soc-runbook-qa`) with high-quality examples

---

## 🎯 Goals

- Use a **consistent format** for every incident:
  - Executive summary
  - Scope / impact
  - Timeline
  - Root cause
  - MITRE ATT&CK mapping
  - Remediation + lessons learned
- Store **supporting evidence** in a clean structure:
  - Log extracts
  - Screenshots
  - Diagrams
- Link incidents back to:
  - Threat hunting (`threat-hunting`)
  - Detections (`soc-alert-automation`)
  - Architecture (`lab-core-network`, `ug-aws-hybrid-soc-lab`)

---

## 📂 Repository Structure

```text
incident-reports/
├── README.md
├── docs/
│   ├── methodology.md              # how I write and review incidents
│   ├── report-lifecycle.md         # from detection to post-incident review
│   └── severity-matrix.md          # how I grade severity/priority
├── templates/
│   ├── report-template.md          # main incident report template
│   ├── timeline-template.md        # detailed timeline template
│   └── customer-summary-template.md# 1-page non-technical summary format
├── cases/
│   ├── 2025-01-lab-ssh-bruteforce/
│   │   ├── report.md               # full narrative incident report
│   │   ├── timeline.md             # minute-by-minute SOC view
│   │   ├── mitre-mapping.md        # ATT&CK techniques + detection notes
│   │   └── evidence/
│   │       ├── logs/
│   │       │   ├── wazuh-alerts.json
│   │       │   └── suricata-events.json
│   │       └── screenshots/
│   │           ├── wazuh-dashboard.png
│   │           └── kibana-timeline.png
│   ├── 2025-02-dns-tunneling-lab/
│   │   ├── report.md
│   │   ├── timeline.md
│   │   ├── mitre-mapping.md
│   │   └── evidence/
│   │       ├── logs/
│   │       └── screenshots/
│   └── 2025-XX-<short-name>/
│       └── ...                     # same structure for future incidents
└── exports/
    ├── redacted/
    │   ├── 2025-01-lab-ssh-bruteforce-redacted.pdf
    │   └── 2025-02-dns-tunneling-lab-redacted.pdf
    └── metrics/
        └── incident-metrics.csv    # for tracking counts/MTTR/etc.