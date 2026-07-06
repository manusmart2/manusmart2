# SOC Projects Portfolio

A collection of hands-on security operations projects built while transitioning from QA to SOC Analyst. Each project includes documentation, queries/scripts, MITRE ATT&CK mappings, and investigation templates.

## Priority Projects (Start Here)

These five align closest with entry-level SOC Analyst responsibilities:

| # | Project | Description |
|---|---------|-------------|
| 1 | [SOC Home Lab](SOC-Home-Lab/) | Splunk + Sysmon + Windows/Kali attack simulation lab |
| 2 | [Splunk Detection Lab](Splunk-Detection-Lab/) | 15 detection rules with dashboards and MITRE mapping |
| 3 | [Phishing Investigation](Phishing-Investigation/) | 5 case studies with header/URL/malware analysis |
| 4 | [Python Security Scripts](Python-Security-Scripts/) | Automation for IOC checks, log parsing, VT lookups |
| 5 | [Incident Response](Incident-Response/) | End-to-end phishing-to-compromise case study |

## Additional Projects

| Project | Description |
|---------|-------------|
| [Threat Hunting](Threat-Hunting/) | Hypothesis-driven hunts for encoded PowerShell, lateral movement |
| [Malware Analysis](Malware-Analysis/) | Static analysis workflow with IOC reporting |
| [Network Forensics](Network-Forensics/) | Wireshark PCAP analysis for DNS, HTTP, SMB |
| [Vulnerability Assessment](Vulnerability-Assessment/) | Nmap/Nessus scans with CVSS-prioritized reports |

## Repository Structure

```
SOC-Projects/
├── SOC-Home-Lab/
├── Splunk-Detection-Lab/
│   ├── detections/          # SPL detection queries
│   └── dashboards/          # Dashboard specs
├── Phishing-Investigation/
│   └── case-studies/
├── Malware-Analysis/
│   └── reports/
├── Threat-Hunting/
│   └── hunts/
├── Python-Security-Scripts/
│   ├── ioc_checker.py
│   ├── log_parser.py
│   ├── failed_login_detector.py
│   ├── hash_calculator.py
│   ├── virustotal_lookup.py
│   └── suspicious_ip_checker.py
├── Incident-Response/
│   └── case-studies/
├── Network-Forensics/
│   └── analysis/
└── Vulnerability-Assessment/
    └── reports/
```

## What Each Project Includes

- **README.md** — Objectives, tools, setup, and findings
- **Detection queries / scripts** — Runnable SPL and Python
- **Sample data** — Sanitized logs and datasets (no live malware)
- **MITRE ATT&CK mappings** — Technique IDs where applicable
- **Screenshots** — Add your lab screenshots to each project's `screenshots/` folder

## Skills Demonstrated

- Windows Event Log analysis (4624, 4625, 4688, 7045)
- Sysmon endpoint telemetry (Event IDs 1, 3, 7, 10, 11)
- Splunk SPL detection engineering
- Phishing email forensics (SPF, DKIM, DMARC)
- Static malware analysis and IOC extraction
- Python security automation
- Incident response documentation
- Network traffic analysis
- Vulnerability assessment and risk prioritization

## Disclaimer

- Malware samples are analyzed **statically only** using safe repositories (e.g., MalwareBazaar, VirusTotal)
- Never execute unknown malware on your host or production network
- All log data in this repo is **synthetic or sanitized**
