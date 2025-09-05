# Incident — RDP Brute Force (LAB, sample data)

**When (UTC):** 2025-09-05 14:22  
**Severity:** Medium  
**Entities:** `Account=LAB\cad`, `Host=WIN-LAB01`, `IP=203.0.113.42`  

**L1 Triage (summary)**
1) Multiple 4625 (fail) → 4624 (success), LogonType 10  
2) Source IP ASN benign; lab user only  
3) Containment if prod: reset creds, block IP, tighten RDP exposure  
**Disposition:** Benign (LAB)
