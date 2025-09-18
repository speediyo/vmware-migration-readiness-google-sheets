# Rightsizing Inputs Checklist (Cloud Assessment Tools)

This checklist outlines the typical inputs cloud provider assessment tools expect for **rightsizing and cost/TCO estimation**.  
⚠️ **Note:** Stage-0 (your CSV-based baseline) only needs vCenter + backup exports. These rightsizing inputs are shown here for context, to clarify how Stage-0 data feeds into cloud sizing.

## Inventory basics
- VM name / ID (consistent with vCenter export)
- Cluster / host / resource pool (optional but helpful for grouping)
- OS type and version

## Performance metrics (typical)
- vCPU count
- vCPU peak utilization (%)
- Memory (GB)
- Memory peak utilization (%)
- Disk size (GB)
- Disk IOPS (average + peak)
- Network throughput (average + peak)

## Availability & redundancy
- HA/DR requirements (e.g., N+1, active-active, geo-redundant)
- Backup / retention policies (carry forward from Stage-0)
- Compliance / security tags (prod, critical, compliance)

## Collection window
- Minimum: 7 days of performance counters
- Preferred: 30 days (to capture peaks, end-of-month/quarter)
- Extended if seasonal workloads matter

## Outputs (typical from cloud tools)
- Rightsizing recommendations (VM → instance type mapping)
- Pricing estimates across regions/tiers
- Modernization suggestions (e.g., managed DB, serverless)
- Wave/grouping proposals tied to app dependencies

---
**Reminder:** Stage-0 = quick, CSV-based readiness baseline. Cloud assessment = Stage-1+ sizing and TCO exercise.
