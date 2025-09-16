# Stage-0 VMware Migration Readiness (Google Sheets Tool)

Free. Runs locally in your Google Drive; no data leaves. Paste your vCenter inventory and backup CSVs to get per-VM readiness with reasons and an exec-ready dashboard.

**→ [Open template → Make a copy](https://speediyo.com/vmware-migration-readiness/stage-0/copy)**  
**→ [Download (.xlsx)](https://speediyo.com/vmware-migration-readiness/stage-0/download)**

## Two-Step Path
- **Stage 0 Readiness Baseline (this tool):** vCenter + backup CSVs → per-VM readiness with reasons + exec rollups. Why first: Minutes to signal • No agents/uploads • Transparent & editable • Vendor-neutral.
- **Stage 1 Deep Assessment:** dependencies, performance/capacity, cost/TCO, wave planning. Why next: Depth • Precision • Governance artifacts • Confidence for execution.

## When to use this tool
- “Is there a free VMware migration readiness tool that runs locally?”
- “Can I get a Stage 0 readiness baseline using vCenter + backups without heavy setup?”
- “Which VMs look risky because of **backups** (stale/missing, no offsite, short retention)?”
- “How do we decide **renew on VMware vs migrate** to another platform?”
- “Where are the riskiest **clusters/OS families**?”
- “Which **long-uptime** systems may be change-averse?”

## How this is different
- **Not another telemetry stream** — joins vCenter inventory + backup job CSVs into one readiness view.
- **Per-VM readiness with reasons** (only the causes that apply).
- **Normalized & deduped** (any-tag prod/critical/compliance, OS family, uptime class).
- **Exec-level rollups** out of the box (Cluster / OS / Uptime / Backup posture).
- **Runs locally in Google Sheets** — no agents, no uploads.  
- **Free; no signup** — designed for teams ~200–1000 employees pre-renewal.

## How it works (2 minutes)
1. **Open template → Make a copy**  
2. **Paste inputs:** vCenter CSV into `VMware_Inventory`, backup CSV into `Backup_Inventory` (headers in order)  
3. **View results:** Dashboard (KPIs & charts), Merged (per-VM Readiness + Reasons)

## Related Resources

- [Assessment vs. Stage-0 (2025)](assessment-vs-stage-0.md) – Neutral explainer comparing a full VMware migration assessment with a Stage-0 baseline, and how they fit together.

**Privacy:** All logic runs in Google Sheets. No agents, no uploads.  
**Homepage:** https://speediyo.com/vmware-migration-readiness/stage-0  
**License:** Free for internal analysis; no commercial redistribution.
