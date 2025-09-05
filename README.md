# Sentinel Homelab — Cad Mendes

> **Resumo (PT-PT):** Laboratório do Microsoft Sentinel com **1 regra KQL (RDP brute force)**, nota de triagem e captura de ecrã (ambiente de **LAB**). Demonstra configuração de SIEM, deteção e resposta operacional a incidentes para funções SOC L1/L2.

**What**: Small SOC lab in Microsoft Sentinel with one analytics rule (RDP brute force), a short L1 triage note, and one incident screenshot (**LAB**, sanitized).

**Why**: Proves hands-on SIEM setup, KQL detection, and incident handling for SOC L1/L2 roles.

## How to run (quick)
1. Import KQL from `/detections/rdp-bruteforce.kql` into Sentinel Analytics Rules.
2. Trigger a benign test in a lab VM (several failed RDP logons → one success).
3. Use `/playbooks/rdp-triage.md` for L1 steps and note the disposition.
4. Save one sanitized incident screenshot in `/screenshots/incident.png` (watermark “LAB”).

## Files
- `detections/rdp-bruteforce.kql` — correlates failed→successful RDP (LogonType 10).
- `playbooks/rdp-triage.md` — 10–12 line L1 triage.
- `screenshots/incident.png` — sanitized, LAB-watermarked image.

## Next
- Add **PowerShell Encoded** & **Impossible Travel** rules.
- Add **Windows Event cheat-sheet** and **Sigma→KQL** mapping for one rule.

**Author**: Cad Mendes , UK • [LinkedIn](https://www.linkedin.com/) • Portfolio: https://github.com/CadMendes
