# Dependency Mapping Inputs Checklist (Agentless)

This checklist outlines typical inputs and steps for **agentless dependency mapping** during a Stage‑1 assessment.  
**Note:** Stage‑0 (your CSV‑based baseline) does **not** require these items; it uses only vCenter + backup exports. This list is here to clarify why Stage‑0 is faster to run first.

## Data sources
- Network flow telemetry: NetFlow/sFlow/IPFIX from ToR/aggregation switches or firewalls
- Hypervisor/cloud flow logs (e.g., vDS port mirroring, NSX/flow logs, VPC/VTAP equivalents)
- Packet capture/vTAP/span (selective, as needed)
- Name resolution: DNS logs or forward lookups (to resolve service names)
- Inventory context: vCenter export (names/UUIDs/cluster/host), CMDB (optional)

## Collection window
- **Recommended:** 7–14 days minimum to capture daily/weekly jobs
- Extend to 30 days if month‑end/quarter‑end jobs are critical
- Avoid maintenance windows that suppress normal traffic

## Access & deployment
- Read‑only access to flow sources (switch/firewall/cloud account)
- Lightweight collectors or virtual appliances if required
- Document IP ranges/subnets to include; exclude noisy infra as needed (e.g., backups, monitoring)

## Normalization
- Resolve VM names/IPs to a consistent key (prefer vCenter name or UUID)
- Tag common infra services (AD/DC, DNS, NTP, backups) to avoid false “app dependencies”
- Deduplicate symmetric flows; aggregate by port/protocol

## Outputs (typical)
- Communication matrix (VM/Service ↔ VM/Service with ports/protocols, volume/observations)
- Suggested application groups (move sets) with “must‑move‑together” notes
- Exceptions list: latent/rare flows requiring extended collection
- Export formats: CSV/JSON for ingestion into planning tools

## Quick sanity checks
- Are directory services and DNS showing as shared infra (not binding unrelated apps)?
- Did we capture at least one full change window/deploy cycle?
- Are there unmanaged IPs or appliances that need naming/resolution?

---
**Reminder:** Stage‑0 = CSV‑based, first‑hour baseline (vCenter + backup exports). Dependency mapping is a Stage‑1 activity used to plan waves and reduce risk.
