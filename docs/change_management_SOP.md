# Change Management Standard Operating Procedure (SOP)

This SOP defines the process for initiating, reviewing, approving, and implementing changes within operational and IT environments.  
It ensures that all changes are controlled, communicated, and executed in a way that minimizes risk and service disruption.

---

## Purpose

The purpose of this procedure is to provide a structured and repeatable process for managing all operational and technical changes.  
It establishes accountability, documentation, and evaluation standards for each stage of the change lifecycle.

This SOP supports:
- The [Operations Management Policy](../policies/OPERATIONS_MANAGEMENT_POLICY.md)  
- The [Risk Register](../templates/RISK_REGISTER_TEMPLATE.md)  
- The [Incident Response Guide](../procedures/INCIDENT_RESPONSE_GUIDE.md)

---

## Scope

This SOP applies to all changes that may impact production systems, business operations, security posture, or compliance status, including:

- Application updates or patch deployments  
- Infrastructure modifications (servers, networks, or databases)  
- Configuration changes in SCCM, AD, ServiceNow, or similar tools  
- Vendor system integrations or new software installations  
- Policy, process, or workflow updates impacting service delivery  

---

## Definitions

| **Term** | **Definition** |
|-----------|----------------|
| **Change** | Any modification to systems, services, configurations, or procedures that could affect stability or performance. |
| **Change Request (CR)** | A formal submission for approval to implement a change. |
| **Change Advisory Board (CAB)** | A cross-functional review body responsible for evaluating, approving, or rejecting proposed changes. |
| **Emergency Change** | A high-priority change required to resolve critical incidents or prevent imminent business disruption. |

---

## Roles and Responsibilities

| **Role** | **Responsibility** |
|-----------|--------------------|
| **Change Requestor** | Submits the change request with all required documentation and risk assessment. |
| **Change Manager** | Reviews and coordinates all changes, chairs CAB meetings, and ensures adherence to policy. |
| **CAB Members** | Evaluate the impact, risk, and readiness of proposed changes and approve or reject requests. |
| **Implementation Team** | Executes the approved change according to the defined plan and timeline. |
| **Service Desk / Monitoring** | Monitors the environment post-implementation and reports anomalies or rollbacks. |

---

## Change Lifecycle

### **1. Initiation**
- Submit a Change Request (CR) in the approved tracking tool (e.g., ServiceNow, Jira, or internal register).  
- Include:
  - Change description and justification  
  - Business impact and affected systems  
  - Implementation plan and rollback procedure  
  - Risk level (linked to [Risk Register](../templates/RISK_REGISTER_TEMPLATE.md))  
  - Proposed schedule and testing requirements  

---

### **2. Review and Assessment**
- The Change Manager verifies completeness and assesses:
  - **Risk Rating**: Low, Medium, High  
  - **Change Type**: Standard, Normal, or Emergency  
  - **Dependency Analysis**: Conflicts with ongoing initiatives or scheduled downtime  
- High-impact or cross-functional changes are presented to the **CAB** for approval.  

---

### **3. Approval**
| **Change Type** | **Approval Authority** | **CAB Review Required** |
|------------------|------------------------|--------------------------|
| Standard | Pre-approved by Change Manager | No |
| Normal | Change Manager and CAB | Yes |
| Emergency | Incident Manager or Senior IT Lead | As soon as practicable post-implementation |

All approvals must be documented within the CR record, including reviewer names, dates, and any conditions for approval.

---

### **4. Implementation**
- Execute the change according to the approved implementation plan.  
- Validate all backups and pre-checks before proceeding.  
- Communicate downtime or service impact notifications to stakeholders.  
- Update monitoring dashboards and documentation immediately following implementation.  

---

### **5. Validation and Review**
- Perform post-implementation testing to confirm expected results.  
- If unsuccessful, execute the rollback plan immediately.  
- Document results, lessons learned, and any residual risks.  
- Update the Risk Register for new or modified risk items.  

---

### **6. Closure**
- The Change Manager reviews evidence of successful implementation.  
- Mark the CR as *Closed* in the tracking system.  
- Attach final validation results, approvals, and lessons learned.  
- Include any new risks or incidents in the monthly CAB report.  

---

## Risk and Impact Scoring

| **Likelihood** | **Impact** | **Score (L×I)** | **Risk Level** |
|----------------|-------------|------------------|----------------|
| 1 | 1–3 | 1–3 | Low |
| 2 | 4–6 | 4–6 | Medium |
| 3 | 7–9 | 7–9 | High |
| 4 | 10–12 | 10–12 | Very High |

> Refer to the [SAM_RISK_REGISTER.md](../templates/SAM_RISK_REGISTER.md) for detailed scoring methodology and examples.

---

## Emergency Change Process

1. Identify the critical issue and determine necessity for immediate change.  
2. Notify the Change Manager or Incident Manager.  
3. Document the CR as “Emergency” and proceed with expedited approval.  
4. Implement the change with active communication to all impacted parties.  
5. Conduct a post-implementation review within 24 hours.  
6. Update the CAB and Risk Register accordingly.  

---

## Documentation and Audit Requirements

- All changes must have associated CR numbers and approval records.  
- Implementation plans, rollback procedures, and validation results must be stored in the designated repository (e.g., `/changes/` folder or ticket system).  
- Quarterly audits will verify:
  - Documentation completeness  
  - Approval compliance  
  - Post-implementation results  

---

## Review and Governance

| **Review Cycle** | Quarterly or after major incidents |
|------------------|------------------------------------|
| **Owner** | Change Manager / Operations Governance Lead |
| **Approver** | Operations Director / IT Governance Committee |
| **Next Review Date** | _YYYY-MM-DD_ |

---

## References

- ISO/IEC 20000-1 — IT Service Management  
- ISO 27001 — Information Security Controls (Change Control)  
- ITIL 4 — Change Enablement  
- COBIT 2019 — DSS06 Manage Changes  
- NIST SP 800-128 — Security-Focused Configuration Management  

---

_© 2025 IT Asset & Risk Management Suite — Licensed under the [MIT License](../LICENSE)_
