# SOC-Ticket-Handling-Simulation
Simulated SOC ticket handling using Splunk detections and Zammad tickets

This project simulates a **Security Operations Center (SOC)** incident management workflow using the open-source platform **Zammad**. It replicates how SOC analysts document, investigate, and escalate cybersecurity incidents triggered by real-world detections.

---

##  Project Highlights

Realistic SOC workflow using open-source Zammad ticketing platform
Each ticket includes MITRE ATT&CK mapping, detection logic, and analyst summary
Exported tickets in structured **JSON format** for resume or GitHub portfolio use
Ideal for **SOC1/SOC2** resume demonstration or lab documentation

---

## What's Inside

Each ticket includes:

- **Incident Title**  
- **Detection Logic (e.g., SPL queries)**  
- **Mapped MITRE ATT&CK Technique & Tactic**  
- **Analyst Summary and Recommendations**  
- **Ticket Metadata** (priority, state, timestamps)

---

##  Platform: Zammad

Zammad is an open-source ticketing and helpdesk platform with:

- Web UI for SOC simulation
- Role-based access control
- REST API for ticket management and export
- Tagging, custom fields, priority levels

---

##  Sample Incident Tickets

| Ticket ID | Incident Title                                          | MITRE Technique | Description |
|-----------|----------------------------------------------------------|------------------|-------------|
| 57002     | **Office Spawning PowerShell Detected**                 | T1059.001        | Detects suspicious parent-child behavior (e.g., `WINWORD.exe` → `powershell.exe`) indicating possible macro-based payload execution. |
| 57003     | **Suspicious LSASS Access by Non-Standard Tool**        | T1003.001        | Flags unauthorized tools accessing LSASS memory (via Sysmon Event ID 10). Common indicator of credential dumping attempts. |
| 57004     | **Domain Mismatch in Windows Logon Events**             | T1078            | Detects domain mismatch during login (`EventCode 4624`) — potential account misuse or lateral movement. |

---

