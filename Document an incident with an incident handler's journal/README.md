# Incident Handler's Journal

A journal documenting my experience while handling various security incidents.

> 📄 **Deliverable:** The completed incident handler's journal: [`Document_an_incident_with_an_incident_handler's_journal.pdf`](./docs/Document_an_incident_with_an_incident_handler's_journal.pdf)

| **Date:** 7/28/2026 | Entry: #1 |
|---|---|
| **Description** | [A ransomware security](./docs/Incident_01_Scenario_Ransomware_attack.pdf) incident at a small health care clinic caused by targeted phishing emails on multiple employees. |
| **Tool(s) used**| None |
| **The 5 W's** | • **Who:** A group of unethical hackers<br>• **What:** A ransomware security incident which encrypted medical data, resulting in an operation shutdown.<br>• **When:** Tuesday, approximately 9:00AM<br>• **Where:** At a health care clinic<br>• **Why:** Financial gain |
| **Additional notes** | • How much is the ransom?<br>• Could a decryption key be brute forced to avoid paying the ransom?<br>• What was the content of the email to prompt the file download? |

---

| **Date:** 7/30/2026 | Entry: #2 |
|---|---|
| **Description** | [A Trojan malware security incident](./docs/Incident_02_Scenario_Investigate_a_suspicious_file_hash.pdf) caused by a password-protected spreadsheet attachment in a phishing email. |
| **Tool(s) used**| VirusTotal |
| **The 5 W's** | • **Who:** BlackTech<br>• **What:** An employee downloaded and opened a password-protected spreadsheet attachment containing a malicious payload, which executed unauthorized executable files on the company computer.<br>• **When:**<br>&nbsp;&nbsp;&nbsp;&nbsp;◦ 1:11 PM: Email received.<br>&nbsp;&nbsp;&nbsp;&nbsp;◦ 1:13 PM: Attachment downloaded and opened.<br>&nbsp;&nbsp;&nbsp;&nbsp;◦ 1:15 PM: Executable files generated.<br>&nbsp;&nbsp;&nbsp;&nbsp;◦ 1:20 PM: IDS alert sent to the SOC.<br>• **Where:** A financial services company<br>• **Why:** Cyber espionage |
| **Additional notes** | • Sha256 Hash: 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b<br>• This malware is specifically linked to BlackTech, a state-linked cyber espionage group. |

---

| **Date:** 8/1/2026 | Entry: #3 |
|---|---|
| **Description** | Investigated a [SOC ticket](./docs/Incident_03_Alert_Ticket.pdf) and executed [playbook](./docs/Incident_03_Playbook.pdf) procedures for a [phishing alert](./docs/Incident_03_Scenario_Phishing_Incident.pdf) involving an employee who downloaded a password-protected malicious file containing a Trojan. |
| **Tool(s) used**| VirusTotal |
| **The 5 W's** | • **Who:** BlackTech<br>• **What:** An employee received a phishing email from a spoofed sender containing a password-protected malicious executable file disguised as a resume. <br>• **When:** July 20, 2022 at 09:30:14 AM<br>• **Where:** A financial services company<br>• **Why:** Cyber espionage |
| **Additional notes** | • The Sha256 Hash, 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b, is a trojan malware linked to BlackTech |

---

| **Date:** 8/1/2026 | Entry: #4 |
|---|---|
| **Description** | Based on a review of the incident's [final report](./docs/Incident_04_Final_Report.pdf), an [unethical hacker exfiltrated customer data](./docs/Incident_04_Scenario_Data_Exfiltration.pdf), emailing an employee demanding $25,000 in exchange for the data to not be posted on a forum, a follow-up email was sent to the same employee, this time with a sample of data and an increase in demand to $50,000. |
| **Tool(s) used**| None |
| **The 5 W's** | • **Who:** An unethical hacker<br>• **What:** Data exfiltration<br>• **When:**<br>&nbsp;&nbsp;&nbsp;&nbsp;◦ December 22, 2022 at 3:13 PM PT: First extortion email received by employee<br>&nbsp;&nbsp;&nbsp;&nbsp;◦ December 28, 2022: Second email received with data sample and increased demand; security team notified.<br>• **Where:** Mid-sized retail company<br>• **Why:** Financial gain |
| **Additional notes** | • How will the current attacker be held accountable?<br>• Will the ransom be paid?<br>• If the ransom is paid, how would the attacker be entrusted to not post the data publicly.<br> |

---

| **Reflections / Notes** | **1) Were there any specific activities that were challenging for you? Why or why not?**<br>tcpdump was the most challenging tool because, despite my comfort with the command line, it was difficult to remember the available flags required to isolate specific network traffic. For instance, correctly applying flags like -nn to disable name resolution is critical for detailed packet analysis while ensuring that threat actors are not alerted to an investigation. This complexity makes it easy to struggle with getting the exact output needed. I believe that the more I practice with this, it will become second nature just like using a command line normally.<br><br>**2) Has your understanding of incident detection and response changed since taking this course?**<br>My understanding of incident detection and response has changed significantly throughout this course. Before taking it, my knowledge was limited to basic Intrusion Detection Systems. Now, I have a much deeper understanding of the structured incident response lifecycle and how to analyze threats professionally. I have learned that the incident response lifecycle is a non-linear process where steps often overlap, requiring not only threat detection but also performing root-cause investigations and participating in post-incident reviews to improve future defenses.<br><br>**3) Was there a specific tool or concept that you enjoyed the most? Why?**<br>I enjoyed learning how hash values serve as unique references for known malicious files, allowing the identification of specific samples of malware even if the file names are changed. Tools like VirusTotal interested me because it utilizes crowdsourcing to compile threat intelligence from the global security community, providing valuable information on whether an artifact is considered malicious. |
|---|---|

## Repository Structure & Supporting Files

```text
document-an-incident-with-an-incident-handler's-journal/
├── README.md
└── docs/
    ├── Document_an_incident_with_an_incident_handler's_journal.pdf
    ├── Incident_01_Scenario_Ransomware_attack.pdf
    ├── Incident_02_Scenario_Investigate_a_suspicious_file_hash.pdf
    ├── Incident_03_Alert_Ticket.pdf
    ├── Incident_03_Playbook.pdf
    ├── Incident_03_Scenario_Phishing_Incident.pdf
    ├── Incident_04_Final_Report.pdf
    └── Incident_04_Scenario_Data_Exfiltration.pdf
```
- [`docs/Document_an_incident_with_an_incident_handler's_journal.pdf`](./docs/Document_an_incident_with_an_incident_handler's_journal.pdf) — Completed Incident Handler's Journal
- [`docs/Incident_01_Scenario_Ransomware_attack.pdf`](./docs/Incident_01_Scenario_Ransomware_attack.pdf) — Entry 1 Scenario Prompt
- [`docs/Incident_02_Scenario_Investigate_a_suspicious_file_hash.pdf`](./docs/Incident_02_Scenario_Investigate_a_suspicious_file_hash.pdf) — Entry 2 Scenario Prompt
- [`docs/Incident_03_Alert_Ticket.pdf`](./docs/Incident_03_Alert_Ticket.pdf) — Entry 3 Deliverable Completed SOC Alert Ticket
- [`docs/Incident_03_Playbook.pdf`](./docs/Incident_03_Playbook.pdf) — Reference Phishing Response Playbook v1.0
- [`docs/Incident_03_Scenario_Phishing_Incident.pdf`](./docs/Incident_03_Scenario_Phishing_Incident.pdf) — Entry 3 Scenario Prompt
- [`docs/Incident_04_Final_Report.pdf`](./docs/Incident_04_Final_Report.pdf) — Entry 4 Post-Incident Final Report
- [`docs/Incident_04_Scenario_Data_Exfiltration.pdf`](./docs/Incident_04_Scenario_Data_Exfiltration.pdf) — Entry 4 Scenario Prompt