# Dependency Mapping Sample Files

This folder contains **synthetic examples** illustrating what agentless dependency mapping typically requires and produces.  
⚠️ **Note:** These are **not outputs of the Stage-0 baseline** (which only needs vCenter + backup CSVs). They are included here for context, to show why Stage-0 is faster and how dependency mapping adds value later.

## Files

- **dependency-mapping-inputs-checklist.md**  
  A short Markdown checklist of typical inputs, setup, and outputs for agentless dependency mapping.  
  (e.g., NetFlow/sFlow, vTAP, 7–14 day collection window, communication matrix export)

- **example-communication-matrix.csv**  
  A small synthetic communication matrix (6 VMs × common ports) showing VM-to-VM flows, ports, and observations.  
  (e.g., WEB01 → APP01 TCP 443, APP01 → DB01 TCP 1433, nightly jobs, backup traffic)

## How this relates to Stage-0

- **Stage-0 baseline (this repo’s Google Sheets tool)** uses only vCenter + backup CSV exports.  
- It produces per-VM readiness (Red/Yellow/Green) with reasons and rollups in under an hour.  
- **Agentless dependency mapping (Stage-1)** is slower and more resource-intensive, but adds cross-VM context for migration wave design and pilot planning.  

Together they form part of a **migration readiness journey**:  
1. Stage-0 = quick, CSV-based baseline.  
2. Stage-1 = vendor-led assessment with dependency mapping, performance, and cost/TCO analysis.

---

These files are here to make the distinction clearer and to give IT teams and vendors a shared starting point when discussing Stage-0 vs Stage-1 activities.
