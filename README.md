# Infrastructure Configuration Drift & Compliance Validation (Sanitized Demo)

Demonstration of a security-adjacent infrastructure validation workflow using synthetic data.  
The project showcases DNS/IP lifecycle analysis, configuration drift detection, outcome classification, and action-oriented dispositions designed to support safe operational decision-making.  
**All data is fictional and created solely for demonstration purposes.**

---

## What this demonstrates
- **Configuration drift identification** using DNS resolution and basic reachability signals
- **Outcome classification** (e.g., OK / DNS_FAIL / NO_RESPONSE)
- **Action-oriented disposition** (e.g., Keep/Active, Needs DNS Review, Candidate Stale, Needs Manual Verify)
- **Audit-friendly reporting** via a readable Excel workbook with legend/explanations

---

## Repo contents
- `src/` — Python script used to perform validation
- `demo/` — Sanitized Excel output (and optional synthetic input)
- `docs/` — Optional screenshots and diagrams

---

## How to run (demo)
> The script expects a CSV with columns similar to: `IP Address` and/or `Name`.

Example:
```bash
python3 src/check_ip_domain_sanitized_demo.py demo/demo_input.csv -o demo/results_colorcoded_sanitized_demo.xlsx
