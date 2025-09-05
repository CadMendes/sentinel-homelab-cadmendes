# RDP Brute Force — L1 Triage

Scope:
- RDP brute force (4625→4624) on LogonType 10 (RemoteInteractive).

Validate:
- Source IP ASN/geo; user/account status; MFA state; recent password resets.

Contain:
- Reset/disable affected account; block offending IP; enforce MFA if not enabled.

Eradicate:
- Reduce external RDP exposure; harden GPO/firewall; review lockout thresholds.

Lessons learned:
- Tune thresholds to reduce FPs; add suppression for known scanners; consider Just-in-Time access.

Notes:
- This is a **LAB** scenario; do not reuse screenshots or data from production without approval.
