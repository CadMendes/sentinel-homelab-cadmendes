# Sentinel Homelab — Cad Mendes

![status](https://img.shields.io/badge/evidence-text--only-blue) ![last updated](https://img.shields.io/badge/updated-today-success)

> **Resumo (PT-PT):** Laboratório do Microsoft Sentinel com **1 regra KQL (RDP brute force)** e evidência **sem screenshots**: registo de incidente, amostra de resultados e diagrama. Demonstra SIEM, deteção e triagem L1.

**What**: Small SOC lab in Microsoft Sentinel focusing on one analytics rule (RDP brute force) with **text-first evidence** (no images).

**Why**: Proves SIEM setup, KQL detection, and incident handling for SOC L1/L2 roles.

## Architecture
```mermaid
%% see diagrams/architecture.mmd
flowchart LR
  A[Lab VM (Windows + Sysmon)] --> B[Azure Monitor Agent]
  B --> C[Log Analytics Workspace]
  C --> D[Microsoft Sentinel]
  D --> E[Analytics Rule<br/>RDP brute force (KQL)]
  E --> F[Incident + Entities]


## Evidence (no images)
- `INCIDENT.md` — filled LAB incident summary  
- `results/rdp-bruteforce-sample.md` — sample query output table  
- `detections/rdp-bruteforce.kql` — the KQL used by the rule

<details>
<summary>How this was generated (LAB)</summary>

- Triggered benign pattern: several failed RDP logons then one success.  
- Scope limited to LAB; no production data.  
- After test, access tightened and lab closed.
</details>

**Author**: Cad Mendes — UK • Portfolio: https://github.com/CadMendes
