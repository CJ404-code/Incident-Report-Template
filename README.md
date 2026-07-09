# Incident-Report-Template

1. Report Title:
Short and descriptive title (e.g., "Suspicious PowerShell Execution on Finance Server")

2. Date of Report:
YYYY-MM-DD

3. Reported By:
Name or Analyst ID

4. Severity Level:
Low / Medium / High / Critical

5. Summary of Findings:
Brief description of what was discovered.
Example: "An unusual PowerShell script was detected on FIN-SRV01. The script attempted to download and execute a file from an external IP address."

6. Investigation Timeline:

[Time (UTC) | Event Description]

[10:42 | Alert triggered by Microsoft Defender for Endpoint]

[10:45 | Initial triage confirmed suspicious script]

[11:00 | Network logs reviewed for outbound traffic]

[11:15 | Host isolated and forensic copy acquired]

7. Who, What, When, Where, Why, How





Who: User or system involved (e.g., SYSTEM on FIN-SRV01)



What: What happened (e.g., suspicious process execution)



When: Date/time activity occurred (e.g., 2025-06-17 10:42 UTC)



Where: Affected asset or location (e.g., Finance server FIN-SRV01)



Why: (If known) Reason or threat actor’s intent (e.g., likely initial access)



How: Method used (e.g., PowerShell + curl to fetch payload)

8. MITRE ATT&CK Techniques:
Map behaviors to MITRE (e.g., T1059.001 - PowerShell, T1105 - Ingress Tool Transfer)

9. Impact Assessment:
What was affected and what’s the risk?
Example: "No sensitive data exfiltration observed. Potential for lateral movement if not contained."

10. Recommendations / Next Steps:





Block IP (if applicable): 194.35.XX.XX



Add hash abc123... to EDR blocklist



Apply patch KBXXXXXX on FIN-SRV01

11. Attachments / Evidence:





Screenshots, raw logs, hash values, PCAP files, etc.

12. Report Status:
Open / Closed / Escalated

13. Reviewed By:
Second analyst, lead, or SOC supervisor signature/date
