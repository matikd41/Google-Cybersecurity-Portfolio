# Incident Report Analysis

As a cybersecurity analyst for a multimedia agency, I conducted an incident report analysis following a Denial-of-Service (DoS) attack that disrupted internal network operations for two hours. Using the NIST Cybersecurity Framework to analyze the incident [scenario](./docs/Scenario.pdf), I evaluated the event, documented the mitigation steps, and outlined long-term defensive recommendations.

> 📄 **Deliverable:** The complete formatted PDF report: [`Incident_report_analysis.pdf`](./docs/Incident_report_analysis.pdf)

---

| Section | Details |
|---|---|
| **Summary** | The company's network services suddenly stopped responding due to an incoming flood of ICMP packets and normal network traffic could not access any network resources. The cybersecurity team found the disruption was caused by a DoS attack through a flood of incoming ICMP packets. The team responded by blocking the attack and stopping all non-critical network services to allow for critical network service to be restored. |
| **Identify** | A malicious actor had sent a flood of ICMP pings into the company's network through an unconfigured firewall. |
| **Protect** | The team implemented a new firewall rule to limit the rate of incoming ICMP packets. The team also implemented an IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics. |
| **Detect** | The team implemented a source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets along with a network monitoring software to detect abnormal traffic patterns. |
| **Respond** | During the attack, the team blocked all incoming ICMP traffic, taking non-critical services offline to preserve critical services, and then restoring critical services once contained. Going forward, the team will also conduct periodic log analysis to catch abnormal patterns early and escalate findings to senior staff. |
| **Recover** | The team will verify that no data was lost during the outage, confirm all services are back to normal operation, document the incident along with updating playbooks or baseline configurations if needed. Management and stakeholders will be contacted for any further actions. |

### Reflections/Notes

The team should also segment the network, separating non-critical services from critical services, if this has not been done already. If a DoS attack were to happen again, the entire network won't be taken out of operation.

---

## Repository Structure & Supporting Files

```text
incident-report-analysis/
└── docs/
    ├── Scenario.pdf
    └── Incident_report_analysis.pdf
```
- [`docs/Scenario.pdf`](./docs/Scenario.pdf) — Original activity scenario
- [`docs/Incident_report_analysis.pdf`](./docs/Incident_report_analysis.pdf) — Complete formatted report

