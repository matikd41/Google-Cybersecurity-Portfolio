# Botium Toys: IT Security Audit

As part of an internal IT security audit for Botium Toys, a small U.S. toy retailer with a growing online presence, I assessed the company's assets, identified control and compliance gaps, and provided recommendations to improve their security posture. Cross referencing the [scenario](./docs/Scenario.pdf) and the [scope, goals, and risk assessment report](./docs/Botium_Toys_Scope_goals_and_risk_assessment_report.pdf), I completed a controls and compliance checklist and delivered targeted recommendations to the IT department.

> 📄 **Deliverable:** The completed checklist and recommendations: [`Controls_and_compliance_checklist.pdf`](./docs/Controls_and_compliance_checklist.pdf)

---

## Audit Overview

The audit scope covered Botium Toys' employee equipment, internal network, and systems with the goal of assessing existing assets and completing a controls and compliance checklist to identify gaps in their security posture.

The risk assessment report identified inadequate asset management and missing controls, and assigned the company an overall risk score of 8/10. Full asset inventory, NIST CSF control recommendations, and detailed risk commentary are available in the linked report.

---

## Controls Assessment Checklist

| Control | In Place? | Comment |
|---|---|---|
| Least Privilege | No |
| Disaster recovery plans | No |
| Password policies | No | Exists, but requirements are insufficient |
| Separation of duties | No |
| Firewall | Yes |
| Intrusion detection system (IDS) | No |
| Backups | No |
| Antivirus software | Yes |
| Manual monitoring, maintenance, and intervention for legacy systems  | No | Monitored, but no set schedule to classify as regular maintenance |
| Encryption | No |
| Password management system | No |
| Locks (offices, storefront, warehouse) | Yes |
| Closed-circuit television (CCTV) surveillance | Yes |
| Fire detection/prevention (fire alarm, sprinkler system, etc.)  | Yes |

## Compliance Checklist

**Payment Card Industry Data Security Standard (PCI DSS)**

| Best Practice | Adhered To? |
|---|---|
| Only authorized users have access to customers’ credit card information. | No |
| Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment.  | No |
| Implement data encryption procedures to better secure credit card transaction touchpoints and data.  | No |
| Adopt secure password management policies. | No |

**General Data Protection Regulation (GDPR)**

| Best Practice | Adhered To? |
|---|---|
| E.U. customers’ data is kept private/secured.  | No |
| There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach. | Yes |
| Ensure data is properly classified and inventoried. | No |
| Enforce privacy policies, procedures, and processes to properly document and maintain data.  | Yes |

**System and Organization Controls (SOC Type 1, SOC Type 2)**

| Best Practice | Adhered To? | Comments |
|---|---|---|
| User access policies are established. | No |
| Sensitive data (PII/SPII) is confidential/private. | No |
| Data integrity ensures the data is consistent, complete, accurate, and has been validated.  | Yes |
| Data is available to individuals authorized to access it. | No | Principle of least privilege is not in place, unauthorized individuals have access to all data |

---

## Recommendations

To address Botium Toys' current high risk situation, the IT department should prioritize optimizing its security architecture by enforcing strict access controls. Implementing the principles of least privilege, this means that employees should only have minimum access to accomplish a task. Another design principle is separation of duties, this is to ensure that critical actions require multiple people to avoid the abuse of power. These controls are crucial for SOC compliance, as current employee access to internal data and customer PII/SPII presents a significant risk.

To further strengthen the security posture, Botium Toys must implement data encryption to protect credit card details during processing and storage, which fulfills PCI DSS requirements and ensures the confidentiality and integrity of data. Additionally, deploying an Intrusion Detection System alongside an existing firewall follows the “defense in depth” principle by creating multiple layers of security to monitor threats in real time.

To improve operational resilience, the company must establish disaster recovery plans and automated regular backups, which are essential components of business continuity. The IT department should also address its legacy systems, while the systems are monitored and maintained, no mention that a schedule is in place for such procedures. 

---

## Repository Structure & Supporting Files

```text
botium-toys-it-security-audit/
├── README.md
└── docs/
    ├── Scenario.pdf
    ├── Botium_Toys_Scope_goals_and_risk_assessment_report.pdf
    └── Controls_and_compliance_checklist.pdf
```
- [`docs/Scenario.pdf`](./docs/Scenario.pdf) — Original activity scenario prompt
- [`docs/Controls_and_compliance_checklist.pdf`](./docs/Controls_and_compliance_checklist.pdf) — Completed audit checklist and security recommendations (Deliverable)
- [`docs/Botium_Toys_Scope_goals_and_risk_assessment_report.pdf`](./docs/Botium_Toys_Scope_goals_and_risk_assessment_report.pdf) — Reference audit scope, asset list, and risk report

