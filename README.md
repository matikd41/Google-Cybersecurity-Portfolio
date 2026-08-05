# Google Cybersecurity Portfolio

This repository contains portfolio activities completed as part of the [Google Cybersecurity Professional Certificate](https://www.coursera.org/google-certificates/cybersecurity-certificate). Each activity applies hands-on cybersecurity skills to a realistic scenario; from SQL log analysis and Linux permission management to risk assessments and incident response using the NIST Cybersecurity Framework.

Each folder contains its own README with the scenario, my approach, and supporting documentation such as screenshots, reference PDFs, and completed deliverables.

## 📁 Portfolio Activities

| Activity | Link |
|---|---|
| Apply filters to SQL queries | [View Project](./Apply%20filters%20to%20SQL%20queries) |
| Use Linux commands to manage file permissions | [View Project](./Use%20Linux%20commands%20to%20manage%20file%20permissions) |
| Vulnerability Assessment Report | [View Project](./Vulnerability%20Assessment%20Report) |
| Use the NIST Cybersecurity Framework to respond to incidents | [View Project](./Use%20the%20NIST%20Cybersecurity%20Framework%20to%20respond%20to%20a%20security%20incident) |
| Conduct a security audit | [View Project](./Conduct%20a%20security%20audit) |
| Incident handler's journal | [View Project](./Incident%20handler's%20journal) |

---

## 🛠️ Skills Demonstrated

### SQL & Database Querying
* **Log & Activity Analysis:** Wrote filtered SQL queries (`WHERE`, `AND`, `OR`, `LIKE` wildcards) to isolate suspicious access logs and investigate potential unauthorized activity.
* **Anomaly Detection:** Queried relational databases to detect after-hours logins, geographic anomalies, and policy violations.
* **Data Sanitization Handling:** Utilized wildcard operators and pattern matching to handle inconsistent data entry and ensure complete investigative coverage.

### Linux & Access Control
* **Permissions Analysis:** Read and interpreted Linux permission strings (`ls -l`) to identify security misconfigurations and overly permissive access rights.
* **Least Privilege Enforcement:** Applied `chmod` with symbolic notation to restrict user, group, and world permissions on sensitive files and hidden directories.

### Risk Assessment & Security Auditing
* **Audit Scope & Asset Inventory:** Defined IT security audit parameters, asset inventories, and organizational risk baselines.
* **Compliance Gap Analysis:** Evaluated organizational security controls against compliance frameworks including PCI DSS, GDPR, and SOC standards.
* **Vulnerability & Risk Matrix Evaluation:** Conducted vulnerability assessments using NIST SP 800-30 frameworks to assign qualitative risk scores and prioritize remediation steps.

### Incident Response & Security Frameworks
* **NIST Lifecycle Execution:** Applied the NIST Cybersecurity Framework (CSF) to structure end-to-end incident handling from detection through post-incident review.
* **Dynamic Incident Management:** Managed overlapping, non-linear incident response phases across live containment, investigation, and root-cause analysis.

### Threat Intelligence & Malware Analysis
* **Artifact & Reputation Verification:** Performed SHA-256 file hash analysis using VirusTotal to verify malicious verdicts and assess threat intelligence reports.
* **Threat Actor Correlation:** Correlated Indicators of Compromise (IoCs) with threat actor tactics, techniques, and motivations (distinguishing financial extortion from cyber espionage).

### Network Traffic Analysis
* **Packet Capture & Filtering:** Used `tcpdump` via command line to capture network traffic and isolate specific packet streams for forensic analysis.

### Phishing & Social Engineering Analysis
* **Email Artifact Triage:** Analyzed email metadata, spoofed senders, display name discrepancies, and malicious attachments (`.exe`, password-protected spreadsheets).
* **SOC Playbook Execution:** Executed standardized SOC phishing playbooks to triage alerts, write structured ticket comments, and manage L1-to-L2 escalations.

### Incident Documentation & Technical Writing
* **Chronological Logging:** Maintained structured incident handler logs using the 5 W's framework (Who, What, When, Where, Why) to build accurate attack timelines.
* **Technical & Executive Reporting:** Authored post-incident reports, executive summaries, and stakeholder-facing remediation strategies.

---

## Structure
```text
Google-Cybersecurity-Portfolio
├── README.md
├──apply-filters-to-sql-queries/
|    ├── README.md
|    └── docs/
|        ├── Scenario.pdf
|        ├── Table_formats.pdf
|        └── screenshots/
|            ├── Retrieve_after_hours_failed_login_attempts.png
|            ├── Retrieve_login_attempts_on_specific_dates.png
|            ├── Retrieve_login_attempts_outside_of_Mexico.png
|            ├── Retrieve_employees_in_Marketing.png
|            ├── Retrieve_employees_in_Finance_or_Sales.png
|            └── Retrieve_all_employees_not_in_IT.png
├──botium-toys-it-security-audit/
|    ├── README.md
|    └── docs/
|        ├── Scenario.pdf
|        ├── Botium_Toys_Scope_goals_and_risk_assessment_report.pdf
|        └── Controls_and_compliance_checklist.pdf
├──incident-handler's-journal/
|    ├── README.md
|    └── docs/
|        ├── Document_an_incident_with_an_incident_handler's_journal.pdf
|        ├── Incident_01_Scenario_Ransomware_attack.pdf
|        ├── Incident_02_Scenario_Investigate_a_suspicious_file_hash.pdf
|        ├── Incident_03_Alert_Ticket.pdf
|        ├── Incident_03_Playbook.pdf
|        ├── Incident_03_Scenario_Phishing_Incident.pdf
|        ├── Incident_04_Final_Report.pdf
|        └── Incident_04_Scenario_Data_Exfiltration.pdf
├──use-linux-commands-to-manage-file-permissions/
|    ├── README.md
|    └── docs/
|        ├── Current_file_permissions.pdf
|        ├── Scenario.pdf
|        └── screenshots/
|            ├── Check_file_and_directory_details.png
|            ├── Change_file_permissions.png
|            ├── Change_file_permissions_on_a_hidden_file.png
|            └── Change_directory_permissions.png
├──incident-report-analysis/
|    └── docs/
|        ├── Scenario.pdf
|        └── Incident_report_analysis.pdf
└──vulnerability-assessment-report/
    ├── README.md
    └── docs/
        ├── NIST_SP_800-30_Rev._1.pdf
        ├── Scenario.pdf
        └── Vulnerability_assessment_report.pdf
```
        
