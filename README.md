# Sentinel Homelab — Cad Mendes

![status](https://img.shields.io/badge/evidence-text--only-blue) ![last updated](https://img.shields.io/badge/updated-today-success)
> **LAB only:** synthetic/sample data; no production data is included.

> **Resumo (PT-PT):** Laboratório do Microsoft Sentinel com **1 regra KQL (RDP brute force)** e evidência **sem screenshots**: registo de incidente, amostra de resultados e diagrama. Demonstra SIEM, deteção e triagem L1.

**What**: Small SOC lab in Microsoft Sentinel focusing on one analytics rule (RDP brute force) with **text-first evidence** (no images).

**Why**: Proves SIEM setup, KQL detection, and incident handling for SOC L1/L2 roles.

## Architecture
```mermaid
flowchart LR
  A["Lab VM (Windows + Sysmon)"] --> B["Azure Monitor Agent"]
  B --> C["Log Analytics Workspace"]
  C --> D["Microsoft Sentinel"]
  D --> E["Analytics Rule: RDP brute force (KQL)"]
  E --> F["Incident + Entities"]

