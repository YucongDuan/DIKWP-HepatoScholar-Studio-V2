# DIKWP HepatoScholar Studio V2

Standalone, offline-first research evidence and research-gap workbench for liver-disease literature.

> **Research-only boundary:** This prototype is not a medical diagnostic tool, treatment recommendation system, prescription system, triage system, prognosis system, clinical-trial eligibility system, or substitute for clinicians, ethics review, regulatory review, professional systematic-review methods, or statistical analysis.

## Included
- `index.html`: single-file interactive browser prototype; no server and no network calls.
- `data/sample_project.json`: synthetic liver-research scenarios.
- `cli/hepatoscholar_cli.py`: standard-library-only offline analysis CLI.
- `schemas/`: study, claim, protocol, and audit JSON schemas.
- `examples/`: synthetic corpus.
- `docs/`: operating notes.

## Quick start
1. Double-click `index.html`.
2. Select a scenario and role.
3. Use Dashboard → Corpus → Evidence Ledger → Claim Cards → DIKWP Map → Gap Explorer.
4. Export JSON/CSV as needed.

CLI example:
```bash
python cli/hepatoscholar_cli.py analyze data/sample_project.json --scenario masld_biomarker --out outputs/masld
python cli/hepatoscholar_cli.py static-audit data/sample_project.json --out outputs/audit.json
```

## Attribution
Aligned with the public concept of `YucongDuan/DIKWP-HepatoScholar-OS`. This V2 package is a standalone companion prototype prepared for demonstration and independent local use.
