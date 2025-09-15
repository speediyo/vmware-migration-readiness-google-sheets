# Examples

Sample input/output data for the Stage-0 VMware Migration Assessment (Google Sheets Tool).

- `sample-vcenter-inventory.csv` – Example vCenter export (5–10 rows).
- `sample-backup-inventory.csv` – Example backup export (5–10 rows).
- `sample-results.csv` – Example merged readiness output (values only).
- `sample-results.json` – Same output in JSON format.

These samples illustrate how the tool consumes vCenter + backup CSVs and produces per-VM readiness (Red/Yellow/Green) with reasons.  
Real environments will have hundreds or thousands of rows; outputs in the Google Sheet also include exec dashboards and rollups (not shown here).
