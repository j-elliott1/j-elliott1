# Risk Register

This Risk Register identifies potential risks that may affect the success of the project or operation. It is designed to be updated throughout the project lifecycle to monitor, mitigate, and communicate key risks.

---

## Risk Register Overview

| **Field** | **Description** |
|------------|-----------------|
| **Project/Repo Name** | _Enter project or repository name here_ |
| **Prepared By** | _Name / Role_ |
| **Last Updated** | _YYYY-MM-DD_ |
| **Version** | _v1.0_ |

---

## Risk Log

| ID | Risk Description | Category | Likelihood | Impact | Risk Rating (L×I) | Mitigation Strategy | Contingency Plan | Owner | Status | Review Date |
|----|------------------|-----------|-------------|---------|-------------------|--------------------|------------------|--------|----------|--------------|
| R-01 | Lack of clarity in software license ownership could result in compliance audit penalties. | Compliance / Legal | High | High | 9 | Maintain a centralized license inventory and audit trail. | Escalate to SAM lead for corrective action. | SAM Manager | Open | 2025-11-01 |
| R-02 | Delays in vendor data collection due to unresponsive third-party contacts. | Vendor / Operational | Medium | Medium | 6 | Send early reminders and establish SLAs for vendor responses. | Escalate to Procurement. | Project Manager | Monitoring | 2025-11-01 |
| R-03 | Incomplete documentation of IT assets leading to data inaccuracies. | Data / Operational | High | High | 9 | Implement data validation and quarterly review. | Cross-verify with SCCM or discovery tools. | Asset Analyst | Open | 2025-11-15 |
| R-04 | Key personnel unavailable during project milestones. | Resource | Medium | High | 8 | Maintain backup coverage and knowledge sharing. | Reassign temporary responsibilities. | Team Lead | Open | 2025-11-10 |
| R-05 | Security breach due to outdated software or patching gaps. | Security | Low | Very High | 10 | Enforce automated patch compliance reporting. | Initiate emergency patch cycle. | Security Team | Mitigated | 2025-11-20 |

---

## Risk Scoring Matrix

| **Likelihood** | **Impact** | **Score (L×I)** | **Risk Level** |
|----------------|-------------|------------------|----------------|
| 1 | 1–3 | 1–3 | Low |
| 2 | 4–6 | 4–6 | Medium |
| 3 | 7–9 | 7–9 | High |
| 4 | 10–12 | 10–12 | Very High |

> _Tip: Use consistent scales for Likelihood (1–4) and Impact (1–3) or modify to suit your organization._

---

## Risk Management Notes

- **Review Frequency:** Monthly or after major project milestones  
- **Change Control:** All updates should be versioned via Git commits  
- **Reference:** [ISO 31000:2018 – Risk Management Principles](https://www.iso.org/standard/65694.html)

---

_© 2025 Your Organization — Licensed under the [MIT License](../LICENSE)_
