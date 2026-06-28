# Enterprise Risk Assessment Methodology

**Document ID:** EFSAF-RISK-001

**Version:** 1.0

**Status:** Approved

**Classification:** Enterprise Standard

**Framework:** Enterprise Firewall Security Assessment Framework (EFSAF)

**Owner:** EFSAF Project

**Review Cycle:** Annual or Following Significant Framework Changes

**Effective Date:** June 2026

---

# Document Control

| Field            | Value                                  |
| ---------------- | -------------------------------------- |
| Document Title   | Enterprise Risk Assessment Methodology |
| Document ID      | EFSAF-RISK-001                         |
| Version          | 1.0                                    |
| Status           | Approved                               |
| Classification   | Enterprise Standard                    |
| Framework        | EFSAF                                  |
| Owner            | EFSAF Project                          |
| Review Frequency | Annual                                 |
| Applies To       | All EFSAF Assessment Modules           |
| Supersedes       | None                                   |
| Next Review      | June 2027                              |

---

# Revision History

| Version | Date      | Author        | Description                |
| ------- | --------- | ------------- | -------------------------- |
| 1.0     | June 2026 | EFSAF Project | Initial Enterprise Release |

---

# Table of Contents

1. Purpose
2. Scope
3. Objectives
4. Risk Management Philosophy
5. Guiding Principles
6. Governance
7. Roles and Responsibilities
8. Assessment Lifecycle Overview
9. Risk Management Lifecycle
10. Enterprise Risk Domains

> **Note:** Additional sections (risk scoring model, matrices, calculations, treatment, reporting, appendices, etc.) are defined in subsequent parts of this document.

---

# 1. Purpose

The **Enterprise Risk Assessment Methodology (EFSAF-RISK-001)** establishes the standardized methodology for identifying, evaluating, prioritizing, documenting, communicating, and managing security risks identified during Enterprise Firewall Security Assessments conducted under the Enterprise Firewall Security Assessment Framework (EFSAF).

The methodology provides a consistent and repeatable approach for translating technical observations into measurable business risk, enabling organizations to make informed remediation and governance decisions.

This standard ensures that every finding produced by EFSAF is evaluated using the same criteria, regardless of technology platform, deployment model, organizational size, or industry sector.

The methodology is designed to support both technical practitioners and executive stakeholders by presenting risk in a manner that is technically accurate, operationally relevant, and aligned with business objectives.

---

# 2. Scope

This methodology applies to every assessment module within the Enterprise Firewall Security Assessment Framework.

Including but not limited to:

* Architecture Review
* Management Plane Review
* Rule Base Review
* NAT Review
* VPN Review
* Logging & Monitoring Review
* Threat Prevention Review
* High Availability Review
* Certificate & PKI Review
* Administrative Access Review
* Identity Integration Review
* Cloud Firewall Assessment
* SD-WAN Security Review
* Zero Trust Validation
* Future EFSAF assessment modules

The methodology applies throughout the complete assessment lifecycle, including:

* Planning
* Evidence Collection
* Technical Validation
* Finding Development
* Risk Assessment
* Report Generation
* Remediation Validation
* Executive Reporting

---

# 3. Objectives

The objectives of this methodology are to:

* Establish a uniform enterprise-wide risk evaluation process.
* Ensure consistency across all EFSAF assessments.
* Prioritize findings based on measurable risk rather than subjective opinion.
* Align technical findings with business impact.
* Support executive decision-making through standardized reporting.
* Facilitate regulatory and compliance assessments.
* Enable repeatable assessments across different environments.
* Improve transparency and traceability of security findings.
* Reduce inconsistency between assessors.
* Support continuous improvement of organizational security posture.

---

# 4. Risk Management Philosophy

EFSAF adopts a **risk-based assessment philosophy** rather than a checklist-driven approach.

A configuration deviation, missing security control, or architectural weakness does not inherently represent organizational risk. Risk exists only when a validated technical condition has the potential to adversely affect business objectives through a credible threat scenario.

Accordingly, EFSAF evaluates findings in the context of:

* Technical exposure
* Business impact
* Operational dependency
* Security architecture
* Existing compensating controls
* Environmental context
* Regulatory obligations
* Asset criticality

This philosophy ensures that assessments focus on material risk rather than simply identifying deviations from recommended configurations.

---

# 5. Guiding Principles

The Enterprise Risk Assessment Methodology is governed by the following principles.

## 5.1 Evidence-Based Assessment

Risk determinations shall be supported by verifiable technical evidence. Assumptions, speculation, or unvalidated observations shall not be used to justify risk ratings.

---

## 5.2 Consistency

Equivalent technical conditions shall result in equivalent risk evaluations when assessed under comparable business and operational contexts.

---

## 5.3 Contextual Evaluation

Risk shall be evaluated within the context of the assessed environment. Factors such as network segmentation, exposure, asset value, compensating controls, and business function shall be considered before assigning a final rating.

---

## 5.4 Repeatability

Independent assessors applying this methodology to the same validated evidence should arrive at substantially similar conclusions.

---

## 5.5 Traceability

Every risk rating shall be traceable to:

* Supporting evidence
* Applicable EFSAF control
* Assessment module
* Technical observation
* Business impact analysis
* Recommended remediation

---

## 5.6 Transparency

The methodology, assumptions, scoring criteria, and supporting rationale shall be documented sufficiently to enable independent review.

---

## 5.7 Business Alignment

Risk prioritization shall support organizational objectives by emphasizing issues with the greatest potential impact to confidentiality, integrity, availability, operational resilience, regulatory compliance, and business continuity.

---

# 6. Governance

The Enterprise Risk Assessment Methodology shall be governed under the overall EFSAF framework governance model.

Governance activities include:

* Periodic methodology review.
* Validation against emerging threats.
* Alignment with recognized industry standards.
* Review of scoring consistency.
* Maintenance of assessment quality.
* Approval of methodology updates.
* Version control and change management.

Changes to this methodology shall undergo technical review before publication to ensure backward compatibility and consistency across assessment modules.

---

# 7. Roles and Responsibilities

Effective risk assessment requires clearly defined responsibilities.

| Role                       | Primary Responsibilities                                                                            |
| -------------------------- | --------------------------------------------------------------------------------------------------- |
| Assessment Lead            | Directs the assessment, validates scope, and approves technical findings.                           |
| Security Assessor          | Performs technical evaluation, collects evidence, and documents observations.                       |
| Technical Reviewer         | Independently reviews findings, scoring consistency, and evidence quality.                          |
| Quality Assurance Reviewer | Verifies compliance with EFSAF standards and documentation requirements.                            |
| System Owner               | Provides technical context, validates environmental information, and supports remediation planning. |
| Risk Owner                 | Accepts ownership of identified risks and determines appropriate treatment strategies.              |
| Executive Sponsor          | Reviews overall assessment results and authorizes strategic remediation initiatives.                |

Segregation of duties should be maintained wherever practicable to preserve assessment independence and objectivity.

---

# 8. Assessment Lifecycle Overview

Risk assessment is performed as part of the broader EFSAF assessment lifecycle.

```text
Assessment Planning
        │
        ▼
Scope Definition
        │
        ▼
Evidence Collection
        │
        ▼
Technical Validation
        │
        ▼
Finding Development
        │
        ▼
Risk Assessment
        │
        ▼
Peer Review
        │
        ▼
Quality Assurance
        │
        ▼
Report Generation
        │
        ▼
Executive Review
        │
        ▼
Remediation Planning
        │
        ▼
Risk Revalidation
        │
        ▼
Assessment Closure
```

This lifecycle ensures that risk is assessed only after evidence has been validated and findings have undergone technical and quality review.

---

# 9. Risk Management Lifecycle

Within the assessment lifecycle, the risk management process follows a structured sequence.

```text
Identify
   │
   ▼
Validate
   │
   ▼
Analyze
   │
   ▼
Score
   │
   ▼
Review
   │
   ▼
Approve
   │
   ▼
Report
   │
   ▼
Treat
   │
   ▼
Reassess
   │
   ▼
Close
```

Each stage shall be documented to maintain traceability and support audit requirements.

---

# 10. Enterprise Risk Domains

To ensure consistent classification across all EFSAF modules, identified risks shall be assigned to one or more enterprise risk domains.

The initial domains include:

* Architecture Risk
* Management Plane Risk
* Access Control Risk
* Rule Base Risk
* Network Segmentation Risk
* NAT Risk
* VPN Risk
* Threat Prevention Risk
* Logging and Monitoring Risk
* Identity and Authentication Risk
* Administrative Access Risk
* Certificate and Cryptographic Risk
* Compliance Risk
* Operational Risk
* Availability and Resilience Risk
* Cloud Security Risk
* Third-Party Integration Risk

These domains provide the foundation for standardized reporting, trend analysis, compliance mapping, and executive dashboards across the EFSAF framework.

---

## End of Part 1

**Part 2** will introduce the core of the methodology:

* EFSAF Enterprise Risk Model (ERM)
* Risk Scoring Framework
* Scoring Factors and Weightings
* Likelihood Assessment Model
* Impact Assessment Model
* Exposure Assessment
* Exploitability Assessment
* Detectability Assessment
* Asset Criticality
* Risk Calculation Formula
* Initial Risk Matrix

# 11. EFSAF Enterprise Risk Model (ERM)

## 11.1 Overview

The **EFSAF Enterprise Risk Model (ERM)** provides the standardized methodology for evaluating security findings identified during Enterprise Firewall Security Assessments.

Unlike vulnerability-centric scoring systems that primarily assess software weaknesses, the EFSAF ERM is designed specifically for **enterprise firewall security assessments**, where risk is influenced by technical configuration, architectural design, operational context, business dependency, and existing security controls.

The model evaluates both the technical characteristics of a finding and its potential business impact, ensuring that risk ratings accurately reflect the organization's security posture rather than configuration deviations alone.

The ERM is intended to:

* Standardize risk evaluation across all EFSAF modules.
* Reduce assessor subjectivity.
* Improve consistency between assessments.
* Prioritize remediation based on measurable risk.
* Support executive decision-making through defensible scoring.

---

## 11.2 Risk Assessment Process

Every EFSAF finding shall be evaluated using the following sequence.

```text
Validated Evidence
        │
        ▼
Technical Analysis
        │
        ▼
Threat Evaluation
        │
        ▼
Business Context Assessment
        │
        ▼
Risk Scoring
        │
        ▼
Peer Validation
        │
        ▼
Final Risk Rating
```

A finding shall not receive a final risk rating until all preceding activities have been completed.

---

# 12. Risk Scoring Framework

## 12.1 Risk Dimensions

Each finding shall be evaluated across six primary dimensions.

| Dimension        | Description                                                                                                           |
| ---------------- | --------------------------------------------------------------------------------------------------------------------- |
| Likelihood       | Probability that the identified condition could be exploited or result in an adverse event.                           |
| Technical Impact | Potential effect on confidentiality, integrity, availability, and security architecture.                              |
| Business Impact  | Potential effect on business operations, regulatory obligations, financial objectives, and organizational reputation. |
| Exposure         | Degree to which the affected asset or service is accessible to threat actors.                                         |
| Exploitability   | Difficulty associated with successfully exploiting the identified weakness.                                           |
| Detectability    | Likelihood that exploitation or misuse would be detected by existing monitoring capabilities.                         |

Each dimension shall be assessed independently before calculating the overall risk rating.

---

## 12.2 Scoring Scale

All scoring dimensions use a standardized five-point scale.

| Score | Rating    | Description                                      |
| ----: | --------- | ------------------------------------------------ |
|     1 | Very Low  | Minimal impact or highly unlikely.               |
|     2 | Low       | Limited impact or unlikely.                      |
|     3 | Moderate  | Credible impact requiring management attention.  |
|     4 | High      | Significant impact requiring timely remediation. |
|     5 | Very High | Severe impact requiring immediate attention.     |

This scale ensures consistency across all EFSAF assessment modules.

---

# 13. Likelihood Assessment

Likelihood represents the probability that the identified condition could realistically result in a security event within the assessed environment.

Likelihood shall be evaluated using technical evidence, threat intelligence, deployment context, and exposure.

| Score | Assessment Criteria                                                                   |
| ----: | ------------------------------------------------------------------------------------- |
|     1 | Exploitation is highly improbable under current conditions.                           |
|     2 | Exploitation is possible but requires uncommon circumstances.                         |
|     3 | Exploitation is reasonably possible using known techniques.                           |
|     4 | Exploitation is likely given current exposure and threat landscape.                   |
|     5 | Exploitation is highly probable or already actively observed in similar environments. |

Likelihood should never be based solely on theoretical attack scenarios.

---

# 14. Technical Impact Assessment

Technical Impact measures the potential effect of successful exploitation on the security architecture.

Assessors shall consider:

* Confidentiality
* Integrity
* Availability
* Authentication
* Authorization
* Network Segmentation
* Security Visibility
* Administrative Control
* Lateral Movement
* Privilege Escalation

Scoring guidance:

| Score | Assessment Criteria                                                  |
| ----: | -------------------------------------------------------------------- |
|     1 | Negligible technical impact.                                         |
|     2 | Limited degradation of security controls.                            |
|     3 | Noticeable impact affecting one or more security objectives.         |
|     4 | Significant degradation of enterprise security posture.              |
|     5 | Complete compromise of critical security controls or infrastructure. |

---

# 15. Business Impact Assessment

Business Impact measures the potential effect of a finding on organizational objectives.

Assessors should consider:

* Business continuity
* Financial loss
* Regulatory exposure
* Customer trust
* Service availability
* Operational disruption
* Contractual obligations
* Strategic objectives

Scoring guidance:

| Score | Assessment Criteria                                                                  |
| ----: | ------------------------------------------------------------------------------------ |
|     1 | No meaningful business impact.                                                       |
|     2 | Minor operational inconvenience.                                                     |
|     3 | Moderate disruption requiring management involvement.                                |
|     4 | Major disruption affecting critical business services.                               |
|     5 | Severe enterprise-wide impact with significant financial or regulatory consequences. |

---

# 16. Exposure Assessment

Exposure evaluates the accessibility of the affected asset or service.

Assessors should evaluate:

* Internet exposure
* Third-party connectivity
* Administrative accessibility
* Network segmentation
* Trust relationships
* Remote access capability
* Cloud connectivity
* Shared infrastructure

Scoring guidance:

| Score | Assessment Criteria                                    |
| ----: | ------------------------------------------------------ |
|     1 | Fully isolated with multiple protective layers.        |
|     2 | Limited exposure within trusted internal networks.     |
|     3 | Accessible to authorized enterprise users.             |
|     4 | Broad organizational exposure or partner connectivity. |
|     5 | Directly Internet-facing or publicly accessible.       |

---

# 17. Exploitability Assessment

Exploitability measures the effort, capability, and prerequisites required to successfully exploit the identified weakness.

Assessment factors include:

* Required skill level
* Availability of attack tools
* Authentication requirements
* Privilege requirements
* User interaction
* Complexity of exploitation
* Known exploitation techniques
* Threat actor capability

| Score | Assessment Criteria                                                |
| ----: | ------------------------------------------------------------------ |
|     1 | Extremely difficult to exploit.                                    |
|     2 | Requires advanced expertise and significant effort.                |
|     3 | Exploitable by experienced attackers using established techniques. |
|     4 | Easily exploitable with publicly available tools or methods.       |
|     5 | Trivial to exploit with minimal effort or automation.              |

---

# 18. Detectability Assessment

Detectability evaluates the organization's ability to identify exploitation attempts or successful compromise using existing monitoring and response capabilities.

Assessment considerations include:

* Firewall logging
* Threat prevention alerts
* SIEM integration
* Security monitoring
* Alert fidelity
* Incident response maturity
* Log retention
* Visibility gaps

| Score | Assessment Criteria                                  |
| ----: | ---------------------------------------------------- |
|     1 | Immediate and highly reliable detection.             |
|     2 | High probability of timely detection.                |
|     3 | Detection dependent on manual review or correlation. |
|     4 | Low probability of timely detection.                 |
|     5 | Exploitation unlikely to be detected.                |

---

# 19. Asset Criticality Assessment

Not all firewall assets present equal organizational risk. Risk scoring shall therefore incorporate the criticality of the affected asset.

Assessors should consider:

* Business function
* Data sensitivity
* Network location
* Service dependency
* Regulatory significance
* Availability requirements
* Operational importance

Recommended classification:

| Level    | Description                                                              |
| -------- | ------------------------------------------------------------------------ |
| Critical | Enterprise core infrastructure supporting essential business operations. |
| High     | Major business services with significant operational dependency.         |
| Moderate | Departmental or supporting services.                                     |
| Low      | Limited business impact if unavailable.                                  |

Asset criticality influences remediation prioritization and executive reporting but shall not replace the underlying technical risk evaluation.

---

# 20. Weighting Methodology

To promote consistency across assessments, EFSAF assigns relative weighting to each scoring dimension.

| Dimension        | Weight |
| ---------------- | -----: |
| Technical Impact |    30% |
| Business Impact  |    25% |
| Likelihood       |    20% |
| Exposure         |    10% |
| Exploitability   |    10% |
| Detectability    |     5% |

These weightings reflect the principle that enterprise firewall assessments should prioritize business and technical consequences over exploitability alone.

---

# 21. Preliminary Risk Calculation

The preliminary risk score shall be calculated using the weighted scoring model defined above.

```text
Preliminary Risk Score =

(Likelihood × 0.20)

+

(Technical Impact × 0.30)

+

(Business Impact × 0.25)

+

(Exposure × 0.10)

+

(Exploitability × 0.10)

+

(Detectability × 0.05)
```

The resulting score provides the **Inherent Risk Rating** before considering compensating controls, risk acceptance, or residual risk adjustments.

---

## End of Part 2

In **Part 3**, we'll elevate the methodology further by introducing:

* Inherent vs. Residual Risk
* Compensating Controls Framework
* Risk Modifiers
* Business Context Adjustments
* 5×5 Enterprise Risk Matrix
* Risk Severity Classification
* Risk Treatment Strategies (Mitigate, Transfer, Accept, Avoid)
* Risk Acceptance Authority
* Exception Management
* Executive Risk Prioritization

# 22. Inherent Risk and Residual Risk

## 22.1 Overview

EFSAF distinguishes between **Inherent Risk** and **Residual Risk** to ensure that risk ratings accurately reflect the organization's operational environment.

A technical finding may initially represent a significant security concern; however, existing security controls, architectural safeguards, operational procedures, and monitoring capabilities may reduce the actual level of organizational risk.

Accordingly, every finding shall be evaluated in two stages:

1. **Inherent Risk** – The level of risk assuming no compensating controls are in place.
2. **Residual Risk** – The level of risk remaining after considering validated compensating controls and environmental safeguards.

Residual Risk represents the value reported to management and used for remediation prioritization.

---

## 22.2 Inherent Risk

Inherent Risk reflects the maximum realistic risk associated with a validated finding before considering any mitigating factors.

Examples include:

* Administrative access without MFA.
* Overly permissive security policy.
* Publicly exposed management interface.
* Weak cryptographic configuration.
* Disabled threat prevention profiles.

The Inherent Risk score shall be derived solely from the EFSAF Risk Scoring Framework.

---

## 22.3 Residual Risk

Residual Risk represents the remaining exposure after validated compensating controls have been assessed.

Examples of compensating controls include:

* Network segmentation.
* Privileged Access Management (PAM).
* Jump servers or bastion hosts.
* IP-based administrative restrictions.
* Multi-layer authentication.
* Security monitoring and alerting.
* Security Operations Center (SOC) oversight.
* Change management controls.

Residual Risk shall never exceed the calculated Inherent Risk.

---

# 23. Compensating Controls Assessment

## 23.1 Purpose

Compensating controls are security measures that reduce the likelihood or impact of exploitation without directly eliminating the identified finding.

Their effectiveness shall be evaluated before assigning the final Residual Risk.

---

## 23.2 Evaluation Criteria

Each compensating control shall be assessed based on:

| Evaluation Factor         | Description                                    |
| ------------------------- | ---------------------------------------------- |
| Design Effectiveness      | Is the control appropriately designed?         |
| Implementation            | Is the control fully implemented?              |
| Operational Effectiveness | Is it functioning as intended?                 |
| Coverage                  | Does it protect the affected asset or process? |
| Sustainability            | Can it be maintained over time?                |
| Monitoring                | Is the control continuously monitored?         |

Controls that are planned but not implemented shall not influence Residual Risk.

---

## 23.3 Examples

| Finding                                 | Compensating Control                                                                   |
| --------------------------------------- | -------------------------------------------------------------------------------------- |
| Firewall management interface lacks MFA | Administrative access restricted through isolated management network and PAM solution. |
| Broad security rule                     | Additional segmentation firewall prevents unauthorized lateral movement.               |
| Weak cryptographic configuration        | Traffic protected through dedicated VPN gateway using stronger cryptographic controls. |
| Disabled logging profile                | Independent network monitoring and SIEM provide equivalent visibility.                 |

Compensating controls shall be documented within the assessment report.

---

# 24. Risk Modifiers

Certain organizational characteristics may increase or decrease the significance of a finding.

EFSAF refers to these characteristics as **Risk Modifiers**.

Examples include:

* Internet-facing services.
* Highly sensitive data.
* Regulatory obligations.
* Third-party dependencies.
* High availability requirements.
* Multi-tenant environments.
* Cloud-native deployments.
* Operational technology (OT/ICS).
* Critical infrastructure.

Risk Modifiers shall be considered during the final review process but shall not replace evidence-based scoring.

---

# 25. Business Context Assessment

The same technical finding may represent different levels of organizational risk depending on the business environment.

Assessors shall consider:

* Industry sector.
* Business function.
* Data classification.
* Regulatory requirements.
* Customer impact.
* Service criticality.
* Geographic considerations.
* Operational dependencies.

Illustrative examples:

| Environment                      | Relative Business Risk |
| -------------------------------- | ---------------------- |
| Internet banking platform        | Very High              |
| Healthcare patient records       | Very High              |
| Critical infrastructure          | Very High              |
| Enterprise ERP                   | High                   |
| Internal development environment | Moderate               |
| Laboratory network               | Low to Moderate        |

Business Context shall influence remediation prioritization and executive reporting.

---

# 26. Enterprise Risk Matrix

EFSAF adopts a standardized **5 × 5 Enterprise Risk Matrix**.

```text
                    IMPACT

              1    2    3    4    5

Likelihood 5   M    H    H    C    C

Likelihood 4   M    M    H    H    C

Likelihood 3   L    M    M    H    H

Likelihood 2   L    L    M    M    H

Likelihood 1   L    L    L    M    M
```

Legend:

* **C** – Critical
* **H** – High
* **M** – Medium
* **L** – Low

The matrix provides an additional validation mechanism and shall be used alongside the weighted scoring methodology.

---

# 27. Risk Severity Classification

The final Residual Risk shall be assigned one of the following classifications.

| Score      | Severity      | Required Action                                            |
| ---------- | ------------- | ---------------------------------------------------------- |
| 9.0 – 10.0 | Critical      | Immediate remediation and executive notification.          |
| 7.0 – 8.9  | High          | Prioritized remediation with management oversight.         |
| 4.0 – 6.9  | Medium        | Planned remediation within defined timelines.              |
| 1.0 – 3.9  | Low           | Address during normal operational activities.              |
| 0          | Informational | No immediate remediation required; monitor as appropriate. |

Organizations may define remediation timelines according to internal risk management policies.

---

# 28. Risk Treatment Strategies

Every validated finding shall be assigned an approved treatment strategy.

| Strategy | Description                                                                           |
| -------- | ------------------------------------------------------------------------------------- |
| Mitigate | Implement controls to reduce the identified risk.                                     |
| Avoid    | Eliminate the activity or condition creating the risk.                                |
| Transfer | Shift responsibility through contractual, insurance, or managed service arrangements. |
| Accept   | Formally acknowledge and accept the remaining Residual Risk.                          |
| Monitor  | Continuously observe the condition while no immediate action is taken.                |

The selected strategy shall be documented within the final assessment report.

---

# 29. Risk Acceptance

Risk acceptance is a management decision and shall be formally documented.

Risk acceptance should include:

* Risk identifier.
* Business justification.
* Risk owner.
* Approval authority.
* Acceptance period.
* Review date.
* Supporting evidence.
* Residual Risk.
* Compensating controls.

Acceptance does not eliminate the need for ongoing monitoring.

---

# 30. Risk Exceptions

Where remediation is not immediately feasible, organizations may document a Risk Exception.

Each exception shall include:

* Finding reference.
* Technical justification.
* Business justification.
* Exception owner.
* Expiration date.
* Review schedule.
* Planned remediation roadmap.
* Executive approval (where required).

Expired exceptions shall be reassessed.

---

# 31. Risk Prioritization

Remediation priority shall be determined using multiple factors rather than severity alone.

Priority should consider:

* Residual Risk.
* Asset Criticality.
* Internet exposure.
* Regulatory obligations.
* Active exploitation.
* Business dependency.
* Ease of remediation.
* Availability of compensating controls.

This ensures that remediation efforts are aligned with organizational priorities.

---

# 32. Executive Risk Reporting

Executive reporting should provide a concise view of organizational risk without requiring detailed technical knowledge.

Recommended metrics include:

* Total findings by severity.
* Risk distribution by assessment module.
* Top enterprise risks.
* High-risk assets.
* Remediation progress.
* Outstanding risk exceptions.
* Compliance impact.
* Trend analysis across assessment periods.

Reports should focus on enabling informed strategic decisions rather than presenting raw technical data.

---

## End of Part 3

**Part 4** will complete **EFSAF-RISK-001** with:

* Risk Review & Quality Assurance Process
* Peer Review Requirements
* Documentation Standards for Findings
* Integration with EFSAF Modules
* Compliance Framework Mapping
* Risk Reporting Templates
* Metrics & KPIs
* Continuous Improvement Process
* References
* Appendices
* Enterprise Risk Assessment Workflow
* Final Governance Statements

# 33. Risk Review and Quality Assurance

## 33.1 Purpose

Risk assessments shall undergo an independent quality assurance process before publication to ensure consistency, technical accuracy, and alignment with the EFSAF methodology.

Quality assurance reduces assessor bias, improves repeatability, and ensures that executive decisions are based on reliable information.

---

## 33.2 Quality Assurance Objectives

The review process shall verify that:

* Assessment scope has been correctly applied.
* Evidence supports every documented finding.
* Risk scoring follows the EFSAF methodology.
* Business context has been appropriately considered.
* Recommendations are technically feasible.
* Compliance references are accurate.
* Documentation meets EFSAF standards.
* Reports are complete and internally consistent.

---

## 33.3 Quality Review Checklist

Every assessment should validate the following:

| Review Area                 | Verification |
| --------------------------- | ------------ |
| Scope Validation            | ✓            |
| Evidence Completeness       | ✓            |
| Finding Accuracy            | ✓            |
| Risk Scoring Consistency    | ✓            |
| Business Impact Validation  | ✓            |
| Technical Impact Validation | ✓            |
| Compliance Mapping          | ✓            |
| Recommendation Quality      | ✓            |
| Executive Summary Accuracy  | ✓            |
| Report Formatting           | ✓            |

---

# 34. Peer Review

## 34.1 Independent Technical Review

All High and Critical findings should undergo independent technical review by a qualified reviewer who was not the primary assessor.

Peer review should validate:

* Technical accuracy.
* Evidence sufficiency.
* Risk calculations.
* Severity assignments.
* Recommended remediation.
* Consistency with previous assessments.

---

## 34.2 Escalation

Where reviewers disagree on risk classification, the issue should be escalated to the Assessment Lead or Framework Owner for final determination.

The rationale for the final decision should be documented to maintain auditability.

---

# 35. Finding Documentation Requirements

Every EFSAF finding shall include, at a minimum:

| Field                 | Required            |
| --------------------- | ------------------- |
| Finding ID            | Yes                 |
| Control ID            | Yes                 |
| Assessment Module     | Yes                 |
| Finding Title         | Yes                 |
| Observation           | Yes                 |
| Technical Description | Yes                 |
| Supporting Evidence   | Yes                 |
| Inherent Risk         | Yes                 |
| Residual Risk         | Yes                 |
| Business Impact       | Yes                 |
| Technical Impact      | Yes                 |
| Compensating Controls | Yes (if applicable) |
| Recommended Action    | Yes                 |
| Validation Method     | Yes                 |
| Compliance References | Yes                 |

This standardized structure ensures traceability and facilitates automated reporting.

---

# 36. Integration with EFSAF Assessment Modules

The Enterprise Risk Assessment Methodology serves as the common risk evaluation standard across all current and future EFSAF assessment modules.

The methodology applies uniformly to:

* Architecture Review
* Management Plane Review
* Rule Base Review
* NAT Review
* VPN Review
* Logging & Monitoring Review
* Threat Prevention Review
* High Availability Review
* Identity & Authentication Review
* Certificate & PKI Review
* Cloud Firewall Security Review
* SD-WAN Security Review
* Zero Trust Assessment
* Future EFSAF modules

Each module shall reference **EFSAF-RISK-001** when assigning risk ratings to identified findings.

---

# 37. Compliance Integration

Risk assessments should support organizational compliance objectives by mapping findings to applicable regulatory and industry frameworks.

Common mappings include:

* CIS Controls v8
* CIS Benchmarks
* NIST Cybersecurity Framework (CSF)
* NIST SP 800-53
* ISO/IEC 27001:2022
* PCI DSS v4.0
* SOC 2 Trust Services Criteria
* SWIFT Customer Security Programme (CSP)

Compliance mapping enhances audit readiness but does not replace technical risk assessment.

---

# 38. Reporting Requirements

EFSAF assessment reports should include:

* Executive Summary
* Scope
* Methodology
* Risk Overview
* Findings Summary
* Detailed Findings
* Compliance Mapping
* Risk Heat Map
* Remediation Roadmap
* Appendices

Executive reports should emphasize strategic risk and remediation priorities, while technical reports should provide sufficient detail for implementation teams.

---

# 39. Key Risk Metrics and Performance Indicators

Organizations should monitor key metrics to evaluate the effectiveness of their firewall security program.

Recommended indicators include:

* Number of findings by severity.
* Mean time to remediate (MTTR).
* Percentage of Critical findings remediated within target timelines.
* Repeat findings across assessment cycles.
* Percentage of findings with approved compensating controls.
* Compliance coverage.
* Residual risk trends.
* Outstanding risk exceptions.
* Assessment completion rates.

Trend analysis across multiple assessment cycles provides valuable insight into organizational security maturity.

---

# 40. Continuous Improvement

The Enterprise Risk Assessment Methodology should evolve to address:

* Emerging threat techniques.
* New firewall technologies.
* Changes in industry standards.
* Regulatory updates.
* Lessons learned from assessments.
* Customer feedback.
* Advancements in enterprise security architecture.

Methodology updates should follow the EFSAF governance process and be version-controlled.

---

# 41. References

This methodology is informed by recognized industry guidance, including:

* CIS Controls v8
* CIS Benchmarks
* NIST Cybersecurity Framework (CSF)
* NIST SP 800-53
* ISO/IEC 27001:2022
* PCI DSS v4.0
* SOC 2 Trust Services Criteria
* SWIFT Customer Security Programme (CSP)

Organizations should reference the latest published versions of these standards when performing assessments.

---

# Appendix A – Enterprise Risk Assessment Workflow

```text
Assessment Planning
        │
        ▼
Scope Definition
        │
        ▼
Evidence Collection
        │
        ▼
Technical Validation
        │
        ▼
Finding Development
        │
        ▼
Inherent Risk Assessment
        │
        ▼
Compensating Controls Review
        │
        ▼
Residual Risk Assessment
        │
        ▼
Peer Review
        │
        ▼
Quality Assurance
        │
        ▼
Executive Reporting
        │
        ▼
Remediation Planning
        │
        ▼
Risk Revalidation
        │
        ▼
Assessment Closure
```

---

# Appendix B – Risk Rating Summary

| Severity      | Score Range | Recommended Action                          |
| ------------- | ----------: | ------------------------------------------- |
| Critical      |    9.0–10.0 | Immediate action and executive notification |
| High          |     7.0–8.9 | Prioritized remediation                     |
| Medium        |     4.0–6.9 | Planned remediation                         |
| Low           |     1.0–3.9 | Routine remediation                         |
| Informational |           0 | Monitoring only                             |

---

# Appendix C – Relationship to Other EFSAF Standards

This methodology forms part of the broader Enterprise Firewall Security Assessment Framework and should be used in conjunction with:

* **EFSAF-STD-001** – Documentation Standard
* **EFSAF-EVD-001** – Evidence Collection Guide
* **EFSAF-TAX-001** – EFSAF Taxonomy
* **EFSAF-COMP-001** – Compliance Mapping Standard

These documents collectively define how findings are documented, evidenced, classified, scored, and aligned with industry frameworks.

---

# Conclusion

The **Enterprise Risk Assessment Methodology (EFSAF-RISK-001)** establishes a standardized, evidence-driven approach for evaluating security findings identified during Enterprise Firewall Security Assessments. By combining technical analysis, business context, governance, quality assurance, and consistent reporting, the methodology enables organizations to prioritize remediation efforts based on measurable risk and informed decision-making.

All EFSAF assessment modules shall apply this methodology to ensure consistency, repeatability, and enterprise-grade reporting across the framework.

---
