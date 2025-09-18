# Cloud Assessment Sample Files

This folder contains **synthetic examples** showing what cloud provider assessment tools typically require for **rightsizing and cost/TCO estimation**.  
⚠️ **Note:** These are **not outputs of the Stage-0 baseline** (which only needs vCenter + backup CSVs). They are provided for context, to illustrate how Stage-0 results can feed into cloud assessment steps.

## Files

- **cloud-assessment-checklist.md**  
  A Markdown checklist of typical inputs and metrics cloud assessment tools use for rightsizing and cost/TCO.  
  (e.g., vCPU peak utilization, memory utilization, disk IOPS, network throughput, HA/DR requirements)

- **sample-rightsizing-inventory.csv**  
  A small synthetic VM inventory (6 VMs) including CPU, memory, disk, network, and HA/DR attributes.  
  This shows the type of dataset cloud assessment tools ingest to generate instance mappings and pricing.

## How this relates to Stage-0

- **Stage-0 baseline (this repo’s Google Sheets tool)** requires only vCenter + backup exports and produces readiness bands (R/Y/G) with reasons and rollups.  
- **Cloud provider assessment tools (Stage-1+)** require extended performance and availability metrics to generate rightsizing recommendations, cost/TCO scenarios, and modernization options.  

Together they form part of a **migration readiness journey**:  
1. Stage-0 = quick, CSV-based readiness baseline.  
2. Cloud assessment = Stage-1+ sizing and TCO analysis, often vendor-led.  

---

These examples are provided so IT teams and vendors can see **where Stage-0 ends and cloud assessments begin**, and how the two steps connect in a VMware migration assessment.
