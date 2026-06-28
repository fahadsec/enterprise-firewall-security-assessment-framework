# EFSAF-CMX-001

# Enterprise Control Mapping Matrix

**Version:** 1.0
**Status:** Official Standard
**Classification:** Enterprise
**Owner:** EFSAF Project
**Applies To:** All Enterprise Firewall Security Assessments

---

# Part 1 — Foundation, Mapping Methodology & Control Framework

---

# 1. Purpose

The Enterprise Firewall Security Assessment Framework (EFSAF) Control Mapping Matrix (CMX) establishes the authoritative relationship between EFSAF assessment controls and internationally recognized cybersecurity frameworks, standards, regulatory requirements, and industry best practices.

The Control Mapping Matrix serves as the official compliance crosswalk for EFSAF and enables organizations to demonstrate that firewall security assessment activities support broader enterprise security governance objectives.

This document shall provide:

* Complete traceability between EFSAF controls and external standards.
* A repeatable mapping methodology.
* Audit-ready evidence alignment.
* Compliance reporting consistency.
* Security control interoperability.
* Enterprise governance support.
* Risk-based assessment traceability.
* Future extensibility for emerging security frameworks.

---

# 2. Objectives

The objectives of this document are to ensure that every EFSAF assessment control:

* Shall support one or more internationally recognized security controls.
* Shall be traceable to enterprise security objectives.
* Shall be measurable.
* Shall be repeatable.
* Shall produce defensible assessment evidence.
* Shall support regulatory compliance activities.
* Shall enable management reporting.
* Shall support enterprise risk management.
* Shall integrate with GRC programs.
* Shall facilitate independent auditing.

---

# 3. Scope

This document applies to every assessment performed under EFSAF, including but not limited to:

* Enterprise Firewall Security Reviews
* Firewall Configuration Assessments
* Security Architecture Reviews
* Network Segmentation Reviews
* Rule Base Optimization Assessments
* Compliance Assessments
* Internal Security Audits
* External Security Audits
* MSSP Security Reviews
* Managed Firewall Services
* Government Security Assessments
* Critical Infrastructure Assessments
* Cloud Firewall Reviews
* Hybrid Infrastructure Reviews
* Zero Trust Readiness Assessments

The mapping defined within this document shall apply regardless of:

* Firewall vendor
* Deployment model
* Infrastructure size
* Geographic location
* Industry sector
* Regulatory jurisdiction

---

# 4. Intended Audience

This document is intended for:

## Primary Audience

* Firewall Security Assessors
* Enterprise Security Consultants
* Security Architects
* Security Engineers
* Internal Auditors
* External Auditors
* Compliance Officers
* GRC Professionals
* Security Managers
* CISOs

## Secondary Audience

* MSSPs
* Consulting Organizations
* Regulatory Bodies
* Enterprise Risk Teams
* Government Agencies
* Critical Infrastructure Operators
* Security Operations Centers
* IT Governance Teams

---

# 5. Normative References

The following standards form the primary basis for EFSAF control mapping.

## International Standards

### ISO/IEC

* ISO/IEC 27001:2022
* ISO/IEC 27002:2022

---

### NIST

* NIST Cybersecurity Framework (CSF) 2.0
* NIST SP 800-53 Revision 5
* NIST SP 800-207 (Zero Trust Architecture)

---

### CIS

* CIS Controls Version 8

---

### PCI Security Standards

* PCI DSS Version 4.0

---

### SOC

* SOC 2 Trust Services Criteria

---

### Industrial Control Systems

* IEC 62443 Series

---

### Threat Intelligence Frameworks

* MITRE ATT&CK

---

### Defensive Frameworks

* MITRE D3FEND

---

### Attack Pattern Frameworks

* CAPEC

---

### Application Security References

* OWASP ASVS (Infrastructure-Relevant Controls)

---

### Software Weakness References

* CWE Configuration Weaknesses

---

# 6. EFSAF Control Mapping Principles

Every mapping defined within this document shall adhere to the following principles.

---

## Principle 1 — Traceability

Every EFSAF assessment control shall be traceable to one or more recognized security standards.

Traceability shall include:

* Assessment Activity
* Security Objective
* Applicable Framework
* Compliance Requirement
* Evidence Produced
* Assessment Report Section

---

## Principle 2 — Repeatability

Independent assessors following EFSAF shall obtain substantially equivalent mapping outcomes under similar assessment conditions.

The mapping methodology shall minimize assessor subjectivity through standardized control definitions and documented evaluation criteria.

---

## Principle 3 — Vendor Neutrality

Mappings shall never depend upon:

* Vendor-specific features
* Proprietary terminology
* Vendor marketing claims
* Product licensing tiers

Mappings shall instead reference universal security objectives and implementation outcomes.

---

## Principle 4 — Technology Agnosticism

The mapping model shall support:

* Hardware Firewalls
* Virtual Firewalls
* Cloud Firewalls
* Container Firewalls
* Kubernetes Network Policies
* SD-WAN Firewalls
* Next-Generation Firewalls
* Web Application Firewalls (where applicable)
* Secure Access Service Edge (SASE)
* Zero Trust Network Access (ZTNA)

---

## Principle 5 — Evidence-Based Assessment

Every mapped control shall produce verifiable evidence.

Acceptable evidence includes:

* Configuration exports
* Screenshots
* Command outputs
* API responses
* Audit logs
* Event records
* SIEM data
* Architecture diagrams
* Change records
* Approval documentation
* Backup verification
* Packet captures (where appropriate)

---

## Principle 6 — Risk Alignment

Every mapped control shall contribute to one or more organizational risk reduction objectives.

Risk categories shall include:

* Confidentiality
* Integrity
* Availability
* Compliance
* Operational
* Financial
* Regulatory
* Business Continuity
* Third-Party Risk
* Insider Threat
* Cyber Resilience

---

## Principle 7 — Audit Defensibility

Mappings shall be sufficiently documented such that an independent auditor can:

* Verify assessment procedures.
* Reproduce evidence collection.
* Validate control applicability.
* Confirm compliance assertions.
* Review assessment conclusions.

---

# 7. Control Mapping Methodology

EFSAF adopts a structured multi-layer mapping methodology.

Every control progresses through standardized mapping stages.

```
EFSAF Control
        │
        ▼
Security Objective
        │
        ▼
Assessment Procedure
        │
        ▼
Evidence Collection
        │
        ▼
Risk Mapping
        │
        ▼
Framework Mapping
        │
        ▼
Compliance Mapping
        │
        ▼
Reporting Reference
```

Each stage shall be documented.

---

# 8. Mapping Levels

EFSAF defines four mapping levels.

| Level   | Description                | Required    |
| ------- | -------------------------- | ----------- |
| Level 1 | Direct Control Mapping     | Yes         |
| Level 2 | Security Objective Mapping | Yes         |
| Level 3 | Compliance Mapping         | Yes         |
| Level 4 | Threat Mapping             | Recommended |

---

## Level 1 — Direct Control Mapping

Direct mapping identifies explicit alignment between EFSAF controls and external framework controls.

Example:

```
EFSAF-MGMT-001

↓

NIST SP 800-53 AC-17

↓

ISO 27001 A.8

↓

CIS Control 4

↓

PCI DSS Requirement 7
```

---

## Level 2 — Security Objective Mapping

This level identifies which enterprise security objective is supported.

Examples include:

* Least Privilege
* Secure Administration
* Network Segmentation
* Secure Configuration
* Change Management
* Secure Monitoring
* Threat Detection
* Secure Logging
* Availability
* Resilience

---

## Level 3 — Compliance Mapping

Compliance mapping links controls to regulatory obligations.

Examples include:

* PCI DSS
* SOC 2
* ISO Audits
* Government Security Baselines
* Critical Infrastructure Regulations
* Industry Governance Requirements

---

## Level 4 — Threat Mapping

Threat mapping links controls to known attacker behaviors.

Examples include:

* MITRE ATT&CK
* MITRE D3FEND
* CAPEC
* CWE
* OWASP ASVS

---

# 9. Mapping Granularity Model

EFSAF defines three mapping granularities.

## Coarse Mapping

One EFSAF domain maps to an external framework domain.

Example:

```
Architecture Review

↓

NIST Protect Function
```

---

## Standard Mapping

One EFSAF control maps to multiple framework controls.

Example:

```
MGMT-004

↓

ISO

↓

NIST

↓

PCI

↓

SOC2

↓

CIS
```

---

## Fine-Grained Mapping

Individual assessment procedures map directly to specific framework requirements.

Example:

```
Assessment Step

↓

Evidence

↓

Framework Control

↓

Audit Requirement

↓

Report Section
```

Fine-grained mapping shall be used wherever regulatory precision or audit traceability is required.

---

# 10. Control Classification Model

Each EFSAF control shall be classified using standardized metadata to support consistent mapping, reporting, and governance.

| Attribute                      | Description                                     |
| ------------------------------ | ----------------------------------------------- |
| Control ID                     | Unique EFSAF identifier                         |
| Control Name                   | Official control title                          |
| Assessment Domain              | Functional review area                          |
| Security Objective             | Intended security outcome                       |
| Risk Category                  | Primary risk addressed                          |
| Control Type                   | Preventive, Detective, Corrective, Compensating |
| Assessment Procedure Reference | Linked methodology section                      |
| Evidence Requirements          | Required supporting artifacts                   |
| Applicable Standards           | Mapped frameworks and standards                 |
| Compliance References          | Regulatory and audit mappings                   |
| Threat References              | MITRE, CAPEC, CWE, OWASP mappings               |
| Expected Security Outcome      | Desired post-assessment state                   |
| Assessment Frequency           | Recommended review cadence                      |
| Control Criticality            | Critical, High, Medium, Low                     |
| Scoring Weight Reference       | Link to EFSAF-SCORE-001                         |
| Reporting Reference            | Link to EFSAF-REP-001 sections                  |

---

**End of Part 1**

**Part 2** will introduce the **Enterprise Control Relationship Model, Traceability Framework, Coverage Matrix Architecture, Domain-to-Framework Crosswalk, and the beginning of the comprehensive control mapping tables for all EFSAF assessment domains.**
# EFSAF-CMX-001

# Enterprise Control Mapping Matrix

**Version:** 1.0
**Status:** Official Standard
**Classification:** Enterprise
**Document:** Part 2 of 4

---

# 11. Control Relationship Model

## 11.1 Overview

Enterprise firewall security controls do not operate independently. Every control within EFSAF shall be considered part of an interconnected control ecosystem in which preventive, detective, corrective, and governance controls collectively reduce organizational risk.

Accordingly, the Enterprise Control Mapping Matrix shall preserve both **horizontal** (peer-domain) and **vertical** (control-to-framework) relationships to maintain complete traceability throughout the assessment lifecycle.

The relationship model shall enable assessors to determine:

* Upstream dependencies
* Downstream impacts
* Control inheritance
* Shared evidence
* Risk propagation
* Compliance overlap
* Cross-domain influence
* Residual risk implications

---

## 11.2 Control Relationship Categories

Each EFSAF control shall be classified using one or more relationship types.

| Relationship Type    | Description                                                    |
| -------------------- | -------------------------------------------------------------- |
| Parent Control       | Higher-level governance or architectural control               |
| Supporting Control   | Enhances implementation effectiveness                          |
| Dependent Control    | Requires another control before assessment                     |
| Compensating Control | Provides equivalent protection where primary control is absent |
| Detective Control    | Identifies violations or attacks                               |
| Preventive Control   | Prevents unauthorized activity                                 |
| Corrective Control   | Restores secure operational state                              |
| Governance Control   | Supports policy, oversight, and compliance                     |
| Monitoring Control   | Continuously validates effectiveness                           |
| Assurance Control    | Produces audit evidence                                        |

---

## 11.3 Enterprise Control Dependency Model

```text
Enterprise Governance
          │
          ▼
Security Architecture
          │
          ▼
Firewall Platform
          │
          ▼
Management Security
          │
          ▼
Rule Base Security
          │
          ▼
NAT Security
          │
          ▼
VPN Security
          │
          ▼
Threat Prevention
          │
          ▼
Logging & Monitoring
          │
          ▼
Continuous Assurance
          │
          ▼
Compliance Reporting
```

Failure of upstream controls shall be considered when evaluating downstream control effectiveness.

---

# 12. EFSAF Domain Mapping Architecture

## 12.1 Enterprise Assessment Domains

The following assessment domains comprise the complete EFSAF assessment model.

| Domain ID | Assessment Domain           | Primary Objective               |
| --------- | --------------------------- | ------------------------------- |
| ARCH      | Architecture Review         | Secure firewall architecture    |
| MGMT      | Management Plane Review     | Secure administration           |
| RULE      | Rule Base Review            | Least privilege enforcement     |
| NAT       | NAT Review                  | Secure address translation      |
| VPN       | VPN Review                  | Secure remote connectivity      |
| LOG       | Logging & Monitoring Review | Visibility and accountability   |
| TP        | Threat Prevention Review    | Attack prevention and detection |

---

## 12.2 Domain Objectives

### Architecture Review

Primary objectives include:

* Secure network segmentation
* High availability
* Defense-in-depth
* Trust boundary enforcement
* Security zone validation
* Resilience

---

### Management Plane Review

Objectives include:

* Administrative security
* Authentication
* Authorization
* Secure management protocols
* Administrative accountability
* Configuration integrity

---

### Rule Base Review

Objectives include:

* Least privilege
* Controlled access
* Rule optimization
* Shadow rule detection
* Cleanup of obsolete rules
* Secure traffic authorization

---

### NAT Review

Objectives include:

* Address translation integrity
* Secure exposure reduction
* Public service protection
* Translation consistency
* Documentation accuracy

---

### VPN Review

Objectives include:

* Confidential communications
* Secure authentication
* Encryption assurance
* Tunnel integrity
* Remote access governance

---

### Logging & Monitoring Review

Objectives include:

* Event collection
* Security visibility
* Incident detection
* Log integrity
* SIEM integration
* Monitoring coverage

---

### Threat Prevention Review

Objectives include:

* Intrusion prevention
* Malware prevention
* Application awareness
* Threat intelligence
* Attack detection
* Security enforcement

---

# 13. Crosswalk Methodology

## 13.1 Purpose

The crosswalk methodology establishes a standardized process for mapping EFSAF controls to multiple external standards without introducing ambiguity or duplication.

Each EFSAF control shall be evaluated against:

* Security objective
* Control intent
* Required implementation
* Assessment evidence
* Risk addressed
* Expected security outcome

Only after these attributes are verified shall external framework mappings be assigned.

---

## 13.2 Mapping Process

```text
EFSAF Control
        │
        ▼
Control Objective
        │
        ▼
Assessment Activity
        │
        ▼
Evidence Produced
        │
        ▼
Risk Addressed
        │
        ▼
Applicable Framework Controls
        │
        ▼
Compliance Requirements
        │
        ▼
Assessment Report
```

---

## 13.3 Mapping Confidence Levels

Each mapping shall include a confidence level.

| Level       | Description                 |
| ----------- | --------------------------- |
| Direct      | Explicitly equivalent       |
| Strong      | Closely aligned objective   |
| Moderate    | Partial objective alignment |
| Informative | Supporting reference only   |

Mappings identified as **Informative** shall not be used as the sole basis for compliance assertions.

---

# 14. Traceability Framework

## 14.1 Traceability Principles

Every EFSAF control shall maintain end-to-end traceability from assessment initiation through reporting.

Traceability shall include:

* Control identifier
* Assessment procedure
* Evidence references
* Risk findings
* Scoring references
* Compliance mappings
* Final report references

---

## 14.2 Enterprise Traceability Chain

```text
Assessment Scope
        │
        ▼
EFSAF Domain
        │
        ▼
EFSAF Control
        │
        ▼
Assessment Procedure
        │
        ▼
Evidence Collection
        │
        ▼
Finding
        │
        ▼
Risk Rating
        │
        ▼
Framework Mapping
        │
        ▼
Compliance Mapping
        │
        ▼
Final Report
```

Every assessment artifact shall be traceable throughout this chain.

---

# 15. Coverage Matrix

## 15.1 Purpose

The Coverage Matrix demonstrates how EFSAF collectively addresses major cybersecurity frameworks.

The matrix provides enterprise stakeholders with visibility into assessment coverage while identifying areas requiring supplemental assessments.

---

## 15.2 Framework Coverage Matrix

| EFSAF Domain      | ISO 27001 | ISO 27002 | NIST CSF 2.0 | NIST 800-53 | CIS v8 | PCI DSS 4.0 | SOC 2   | IEC 62443 | Zero Trust |
| ----------------- | --------- | --------- | ------------ | ----------- | ------ | ----------- | ------- | --------- | ---------- |
| Architecture      | ✓         | ✓         | ✓            | ✓           | ✓      | ✓           | ✓       | ✓         | ✓          |
| Management        | ✓         | ✓         | ✓            | ✓           | ✓      | ✓           | ✓       | ✓         | ✓          |
| Rule Base         | ✓         | ✓         | ✓            | ✓           | ✓      | ✓           | ✓       | ✓         | ✓          |
| NAT               | ✓         | ✓         | ✓            | ✓           | ✓      | ✓           | Partial | Partial   | ✓          |
| VPN               | ✓         | ✓         | ✓            | ✓           | ✓      | ✓           | ✓       | ✓         | ✓          |
| Logging           | ✓         | ✓         | ✓            | ✓           | ✓      | ✓           | ✓       | ✓         | ✓          |
| Threat Prevention | ✓         | ✓         | ✓            | ✓           | ✓      | Partial     | Partial | ✓         | ✓          |

---

## 15.3 Threat Framework Coverage Matrix

| EFSAF Domain      | MITRE ATT&CK | MITRE D3FEND | CAPEC   | CWE     | OWASP ASVS |
| ----------------- | ------------ | ------------ | ------- | ------- | ---------- |
| Architecture      | ✓            | ✓            | Partial | Partial | Partial    |
| Management        | ✓            | ✓            | ✓       | ✓       | ✓          |
| Rule Base         | ✓            | ✓            | ✓       | ✓       | ✓          |
| NAT               | Partial      | Partial      | Partial | Partial | Partial    |
| VPN               | ✓            | ✓            | ✓       | Partial | Partial    |
| Logging           | ✓            | ✓            | Partial | Partial | Partial    |
| Threat Prevention | ✓            | ✓            | ✓       | ✓       | ✓          |

---

# 16. Domain-to-Framework Crosswalk

## 16.1 Architecture Review Crosswalk

| Mapping Attribute | Reference                                                              |
| ----------------- | ---------------------------------------------------------------------- |
| Primary Objective | Secure Network Architecture                                            |
| Risk Category     | Architecture Risk                                                      |
| ISO 27001         | Network Security, Segmentation, Infrastructure Protection              |
| ISO 27002         | Secure Network Controls                                                |
| NIST CSF          | Govern, Protect                                                        |
| NIST SP 800-53    | System & Communications Protection (SC), Configuration Management (CM) |
| CIS Controls      | Network Infrastructure Management                                      |
| PCI DSS           | Network Security Controls                                              |
| SOC 2             | Security                                                               |
| IEC 62443         | Zones and Conduits                                                     |
| Zero Trust        | Trust Boundary Enforcement                                             |

---

## 16.2 Management Plane Review Crosswalk

| Mapping Attribute | Reference                                                                              |
| ----------------- | -------------------------------------------------------------------------------------- |
| Primary Objective | Secure Administration                                                                  |
| Risk Category     | Administrative Risk                                                                    |
| ISO 27001         | Access Control                                                                         |
| ISO 27002         | Privileged Access Management                                                           |
| NIST CSF          | Protect                                                                                |
| NIST SP 800-53    | Access Control (AC), Identification & Authentication (IA), Audit & Accountability (AU) |
| CIS Controls      | Account Management                                                                     |
| PCI DSS           | Administrative Access Controls                                                         |
| SOC 2             | Security                                                                               |
| IEC 62443         | Identity and Authentication                                                            |
| Zero Trust        | Continuous Verification                                                                |

---

## 16.3 Rule Base Review Crosswalk

| Mapping Attribute | Reference                   |
| ----------------- | --------------------------- |
| Primary Objective | Least Privilege Enforcement |
| Risk Category     | Access Control Risk         |
| ISO 27001         | Access Restrictions         |
| ISO 27002         | Access Control Policies     |
| NIST CSF          | Protect                     |
| NIST SP 800-53    | AC Family                   |
| CIS Controls      | Access Control Management   |
| PCI DSS           | Firewall Rule Management    |
| SOC 2             | Security                    |
| IEC 62443         | Traffic Restriction         |
| Zero Trust        | Least Privilege             |

---

## 16.4 NAT Review Crosswalk

| Mapping Attribute | Reference                   |
| ----------------- | --------------------------- |
| Primary Objective | Secure Address Translation  |
| Risk Category     | Exposure Risk               |
| ISO 27001         | Network Protection          |
| ISO 27002         | Network Security Controls   |
| NIST CSF          | Protect                     |
| NIST SP 800-53    | SC Family                   |
| CIS Controls      | Network Management          |
| PCI DSS           | Boundary Protection         |
| SOC 2             | Security                    |
| IEC 62443         | Network Segmentation        |
| Zero Trust        | External Exposure Reduction |

---

## 16.5 VPN Review Crosswalk

| Mapping Attribute | Reference                     |
| ----------------- | ----------------------------- |
| Primary Objective | Secure Remote Connectivity    |
| Risk Category     | Remote Access Risk            |
| ISO 27001         | Secure Communications         |
| ISO 27002         | Cryptographic Controls        |
| NIST CSF          | Protect                       |
| NIST SP 800-53    | AC, SC, IA                    |
| CIS Controls      | Secure Remote Access          |
| PCI DSS           | Remote Administrative Access  |
| SOC 2             | Security                      |
| IEC 62443         | Secure Communication Channels |
| Zero Trust        | Verified Connections          |

---

## 16.6 Logging & Monitoring Review Crosswalk

| Mapping Attribute | Reference                     |
| ----------------- | ----------------------------- |
| Primary Objective | Accountability and Visibility |
| Risk Category     | Detection Risk                |
| ISO 27001         | Logging                       |
| ISO 27002         | Monitoring Activities         |
| NIST CSF          | Detect                        |
| NIST SP 800-53    | AU Family                     |
| CIS Controls      | Audit Log Management          |
| PCI DSS           | Logging Requirements          |
| SOC 2             | Monitoring Controls           |
| IEC 62443         | Security Event Monitoring     |
| Zero Trust        | Continuous Monitoring         |

---

## 16.7 Threat Prevention Review Crosswalk

| Mapping Attribute | Reference                     |
| ----------------- | ----------------------------- |
| Primary Objective | Active Threat Defense         |
| Risk Category     | Cyber Threat Risk             |
| ISO 27001         | Malware Protection            |
| ISO 27002         | Threat Detection              |
| NIST CSF          | Detect, Respond               |
| NIST SP 800-53    | SI Family                     |
| CIS Controls      | Malware Defenses              |
| PCI DSS           | Malware Protection            |
| SOC 2             | Security Monitoring           |
| IEC 62443         | System Integrity              |
| Zero Trust        | Adaptive Security Enforcement |

---

# 17. Control Identifier Convention

To ensure consistency across all EFSAF documentation, every mapped control shall follow a standardized identifier format.

| Domain                  | Prefix | Example        |
| ----------------------- | ------ | -------------- |
| Architecture Review     | ARCH   | EFSAF-ARCH-001 |
| Management Plane Review | MGMT   | EFSAF-MGMT-001 |
| Rule Base Review        | RULE   | EFSAF-RULE-001 |
| NAT Review              | NAT    | EFSAF-NAT-001  |
| VPN Review              | VPN    | EFSAF-VPN-001  |
| Logging & Monitoring    | LOG    | EFSAF-LOG-001  |
| Threat Prevention       | TP     | EFSAF-TP-001   |

Each identifier shall remain stable across future versions of EFSAF to preserve audit traceability and historical reporting integrity.

---

**End of Part 2**

**Part 3** will provide the **comprehensive Enterprise Control Mapping Matrix**, including detailed control-by-control mappings with Control ID, Objective, Assessment Procedure Reference, Evidence Requirements, ISO 27001/27002, NIST CSF 2.0, NIST SP 800-53 Rev. 5, CIS Controls v8, PCI DSS v4.0, SOC 2, IEC 62443, Zero Trust, MITRE ATT&CK, MITRE D3FEND, CAPEC, CWE, Assessment Frequency, Criticality, Scoring Reference, and Reporting Reference for all EFSAF assessment domains.
# EFSAF-CMX-001

# Enterprise Control Mapping Matrix

**Version:** 1.0
**Status:** Official Standard
**Classification:** Enterprise
**Document:** Part 3 of 4

---

# 18. Enterprise Control Mapping Matrix

## 18.1 Overview

This section contains the official Enterprise Control Mapping Matrix for EFSAF assessment controls.

Each control shall be uniquely identifiable, traceable, measurable, and auditable. The mappings defined herein establish the relationship between EFSAF assessment activities and internationally recognized cybersecurity frameworks.

Unless otherwise specified, all mappings shall be interpreted as **Direct** or **Strong** alignments in accordance with the Mapping Confidence Model defined in Section 13.

---

# 18.2 Control Mapping Record Structure

Every EFSAF control shall be documented using the following standardized schema.

| Field                          | Description                                  |
| ------------------------------ | -------------------------------------------- |
| Control ID                     | Unique EFSAF control identifier              |
| Control Name                   | Official control title                       |
| Domain                         | EFSAF assessment domain                      |
| Control Objective              | Intended security outcome                    |
| Assessment Procedure Reference | EFSAF-METH-001 / EFSAF-EXEC-001 reference    |
| Risk Category                  | Primary organizational risk addressed        |
| Evidence Requirements          | Mandatory assessment artifacts               |
| Applicable Standards           | Mapped standards and frameworks              |
| Compliance References          | Regulatory control references                |
| Threat References              | MITRE ATT&CK, D3FEND, CAPEC, CWE, OWASP ASVS |
| Expected Security Outcome      | Desired operational state                    |
| Assessment Frequency           | Recommended review cadence                   |
| Control Criticality            | Critical / High / Medium / Low               |
| Scoring Weight Reference       | EFSAF-SCORE-001                              |
| Reporting Reference            | EFSAF-REP-001                                |

---

# 18.3 Architecture Review Control Mappings

## EFSAF-ARCH-001 — Firewall Architecture Design

| Attribute                      | Mapping                                                                                           |
| ------------------------------ | ------------------------------------------------------------------------------------------------- |
| Control Objective              | Verify that firewall deployment aligns with approved enterprise architecture and trust boundaries |
| Assessment Procedure Reference | EFSAF-METH-001 §Architecture Review / EFSAF-EXEC-001 Phase 2                                      |
| Risk Category                  | Architecture Risk                                                                                 |
| Evidence Requirements          | Network diagrams, topology, asset inventory, segmentation design                                  |
| ISO/IEC 27001:2022             | Network Security, Infrastructure Protection                                                       |
| ISO/IEC 27002:2022             | Network Controls                                                                                  |
| NIST CSF 2.0                   | Govern (GV), Protect (PR)                                                                         |
| NIST SP 800-53 Rev. 5          | SC, PL, CA                                                                                        |
| CIS Controls v8                | Controls 1, 12, 13                                                                                |
| PCI DSS v4.0                   | Requirement 1                                                                                     |
| SOC 2                          | Security                                                                                          |
| IEC 62443                      | Zones and Conduits                                                                                |
| Zero Trust                     | Trust Boundary Enforcement                                                                        |
| MITRE ATT&CK                   | Initial Access, Lateral Movement (Defensive Mapping)                                              |
| MITRE D3FEND                   | Network Segmentation                                                                              |
| CAPEC                          | Network Boundary Bypass Patterns                                                                  |
| CWE                            | Improper Network Configuration                                                                    |
| Expected Security Outcome      | Secure, resilient network architecture                                                            |
| Assessment Frequency           | Annual or after major architectural changes                                                       |
| Criticality                    | Critical                                                                                          |
| Scoring Weight                 | Very High                                                                                         |
| Reporting Reference            | Executive Summary, Architecture Findings                                                          |

---

## EFSAF-ARCH-002 — Network Segmentation

| Attribute         | Mapping                                                            |
| ----------------- | ------------------------------------------------------------------ |
| Control Objective | Validate logical and physical segmentation between trust zones     |
| Risk Category     | Segmentation Risk                                                  |
| Evidence          | Zone definitions, routing tables, VLAN mappings, firewall policies |
| ISO 27001         | Access Control                                                     |
| ISO 27002         | Segregation of Networks                                            |
| NIST CSF          | Protect                                                            |
| NIST SP 800-53    | SC-7                                                               |
| CIS v8            | Controls 12 & 13                                                   |
| PCI DSS           | Requirement 1                                                      |
| Zero Trust        | Micro-Segmentation                                                 |
| MITRE ATT&CK      | Lateral Movement Mitigation                                        |
| D3FEND            | Segment Network                                                    |
| Expected Outcome  | Controlled east-west and north-south traffic                       |
| Frequency         | Quarterly                                                          |
| Criticality       | Critical                                                           |

---

## EFSAF-ARCH-003 — High Availability

| Attribute         | Mapping                                                               |
| ----------------- | --------------------------------------------------------------------- |
| Control Objective | Verify resilient firewall deployment without single points of failure |
| Risk Category     | Availability Risk                                                     |
| Evidence          | HA configuration, failover tests, redundancy documentation            |
| ISO               | Availability Controls                                                 |
| NIST              | CP, SC                                                                |
| CIS               | Infrastructure Resilience                                             |
| PCI DSS           | Availability Support                                                  |
| Expected Outcome  | Continuous firewall service during failures                           |
| Frequency         | Semi-Annual                                                           |
| Criticality       | High                                                                  |

---

# 18.4 Management Plane Review Control Mappings

## EFSAF-MGMT-001 — Administrative Access Security

| Attribute           | Mapping                                                 |
| ------------------- | ------------------------------------------------------- |
| Control Objective   | Ensure administrative interfaces are securely protected |
| Procedure Reference | Management Plane Review                                 |
| Risk Category       | Privileged Access Risk                                  |
| Evidence            | Administrator accounts, MFA settings, AAA configuration |
| ISO 27001           | Access Control                                          |
| ISO 27002           | Privileged Access                                       |
| NIST CSF            | Protect                                                 |
| NIST SP 800-53      | AC, IA                                                  |
| CIS v8              | Controls 5 & 6                                          |
| PCI DSS             | Requirement 7                                           |
| SOC 2               | Security                                                |
| IEC 62443           | Identification & Authentication                         |
| Zero Trust          | Continuous Identity Verification                        |
| MITRE ATT&CK        | Valid Accounts                                          |
| D3FEND              | Multi-factor Authentication                             |
| CAPEC               | Credential Abuse                                        |
| CWE                 | Improper Access Control                                 |
| Expected Outcome    | Hardened administrative access                          |
| Frequency           | Quarterly                                               |
| Criticality         | Critical                                                |

---

## EFSAF-MGMT-002 — Secure Management Protocols

| Attribute         | Mapping                                                |
| ----------------- | ------------------------------------------------------ |
| Control Objective | Verify only encrypted management protocols are enabled |
| Evidence          | SSH, HTTPS, SNMPv3 configuration                       |
| Risk Category     | Configuration Risk                                     |
| NIST 800-53       | SC-8, SC-13                                            |
| ISO 27002         | Secure Communications                                  |
| CIS               | Secure Configuration                                   |
| PCI DSS           | Secure Administrative Access                           |
| Expected Outcome  | Confidential management traffic                        |
| Criticality       | High                                                   |

---

## EFSAF-MGMT-003 — AAA Integration

| Attribute         | Mapping                                               |
| ----------------- | ----------------------------------------------------- |
| Control Objective | Validate centralized authentication and authorization |
| Evidence          | RADIUS/TACACS+/LDAP integration                       |
| NIST              | IA, AC                                                |
| CIS               | Account Management                                    |
| Zero Trust        | Identity-Centric Access                               |
| MITRE             | Credential Access Mitigation                          |
| Criticality       | High                                                  |

---

# 18.5 Rule Base Review Control Mappings

## EFSAF-RULE-001 — Least Privilege Policy

| Attribute         | Mapping                                            |
| ----------------- | -------------------------------------------------- |
| Control Objective | Ensure firewall policies implement least privilege |
| Risk Category     | Access Control Risk                                |
| Evidence          | Rule exports, policy reviews                       |
| ISO               | Access Restrictions                                |
| NIST              | AC                                                 |
| CIS               | Access Control Management                          |
| PCI DSS           | Requirement 1                                      |
| Zero Trust        | Least Privilege                                    |
| MITRE ATT&CK      | Defense Against Lateral Movement                   |
| D3FEND            | Policy Enforcement                                 |
| Expected Outcome  | Only authorized communications permitted           |
| Frequency         | Quarterly                                          |
| Criticality       | Critical                                           |

---

## EFSAF-RULE-002 — Shadow Rule Detection

| Attribute         | Mapping                                         |
| ----------------- | ----------------------------------------------- |
| Control Objective | Identify ineffective or shadowed firewall rules |
| Evidence          | Rule analysis reports                           |
| Risk Category     | Operational Risk                                |
| NIST              | CM                                              |
| CIS               | Secure Configuration                            |
| Expected Outcome  | Optimized rule base                             |
| Criticality       | High                                            |

---

## EFSAF-RULE-003 — Unused Rule Review

| Attribute         | Mapping                                    |
| ----------------- | ------------------------------------------ |
| Control Objective | Identify obsolete or unused firewall rules |
| Evidence          | Hit counters, policy statistics            |
| Risk Category     | Security Debt                              |
| ISO               | Configuration Management                   |
| PCI DSS           | Firewall Maintenance                       |
| Expected Outcome  | Reduced attack surface                     |
| Frequency         | Quarterly                                  |

---

# 18.6 NAT Review Control Mappings

## EFSAF-NAT-001 — Public Address Exposure

| Attribute         | Mapping                                          |
| ----------------- | ------------------------------------------------ |
| Control Objective | Validate exposure of internal assets through NAT |
| Evidence          | NAT tables, external IP mappings                 |
| Risk Category     | Exposure Risk                                    |
| ISO               | Network Protection                               |
| NIST              | SC                                               |
| PCI DSS           | Requirement 1                                    |
| Zero Trust        | Minimize Exposure                                |
| Expected Outcome  | Controlled external exposure                     |
| Criticality       | High                                             |

---

## EFSAF-NAT-002 — NAT Rule Consistency

| Attribute         | Mapping                                          |
| ----------------- | ------------------------------------------------ |
| Control Objective | Verify translation consistency and documentation |
| Evidence          | NAT configuration, design documentation          |
| Risk Category     | Operational Risk                                 |
| Expected Outcome  | Accurate and secure translation policies         |
| Frequency         | Annual                                           |

---

# 18.7 VPN Review Control Mappings

## EFSAF-VPN-001 — VPN Authentication

| Attribute         | Mapping                                      |
| ----------------- | -------------------------------------------- |
| Control Objective | Verify strong user and device authentication |
| Evidence          | MFA configuration, VPN authentication logs   |
| ISO               | Authentication Controls                      |
| NIST              | IA                                           |
| CIS               | Secure Remote Access                         |
| PCI DSS           | Requirement 8                                |
| Zero Trust        | Verify Explicitly                            |
| MITRE             | Credential Access Mitigation                 |
| Expected Outcome  | Authenticated remote access only             |
| Criticality       | Critical                                     |

---

## EFSAF-VPN-002 — Encryption Strength

| Attribute         | Mapping                                    |
| ----------------- | ------------------------------------------ |
| Control Objective | Validate approved cryptographic algorithms |
| Evidence          | VPN proposals, cipher suites               |
| NIST              | SC                                         |
| ISO               | Cryptographic Controls                     |
| PCI DSS           | Strong Cryptography                        |
| Expected Outcome  | Confidential remote communications         |
| Frequency         | Semi-Annual                                |

---

## EFSAF-VPN-003 — Tunnel Lifecycle Management

| Attribute         | Mapping                                              |
| ----------------- | ---------------------------------------------------- |
| Control Objective | Verify tunnel monitoring, expiration, and governance |
| Evidence          | Tunnel inventory, uptime reports                     |
| Risk Category     | Availability Risk                                    |
| Expected Outcome  | Controlled VPN lifecycle                             |

---

# 18.8 Logging & Monitoring Review Control Mappings

## EFSAF-LOG-001 — Security Logging

| Attribute         | Mapping                                     |
| ----------------- | ------------------------------------------- |
| Control Objective | Ensure comprehensive firewall event logging |
| Evidence          | Log configuration, log samples              |
| ISO               | Logging                                     |
| NIST              | AU                                          |
| CIS               | Audit Log Management                        |
| PCI DSS           | Requirement 10                              |
| SOC 2             | Monitoring                                  |
| MITRE D3FEND      | Log Collection                              |
| Expected Outcome  | Complete security visibility                |
| Criticality       | Critical                                    |

---

## EFSAF-LOG-002 — Time Synchronization

| Attribute         | Mapping                                     |
| ----------------- | ------------------------------------------- |
| Control Objective | Validate accurate timestamps across devices |
| Evidence          | NTP configuration                           |
| NIST              | AU                                          |
| PCI DSS           | Time Synchronization                        |
| Expected Outcome  | Reliable forensic timelines                 |
| Frequency         | Quarterly                                   |

---

## EFSAF-LOG-003 — SIEM Integration

| Attribute         | Mapping                                                        |
| ----------------- | -------------------------------------------------------------- |
| Control Objective | Verify forwarding of security events to centralized monitoring |
| Evidence          | SIEM dashboards, forwarding configuration                      |
| NIST              | SI, AU                                                         |
| CIS               | Security Monitoring                                            |
| Expected Outcome  | Centralized detection capability                               |
| Criticality       | High                                                           |

---

# 18.9 Threat Prevention Review Control Mappings

## EFSAF-TP-001 — Intrusion Prevention

| Attribute         | Mapping                                               |
| ----------------- | ----------------------------------------------------- |
| Control Objective | Validate IPS deployment and operational effectiveness |
| Evidence          | IPS policies, signature updates                       |
| ISO               | Threat Detection                                      |
| NIST              | SI                                                    |
| CIS               | Malware Defenses                                      |
| MITRE ATT&CK      | Exploitation Mitigation                               |
| MITRE D3FEND      | Intrusion Detection                                   |
| CAPEC             | Exploitation Patterns                                 |
| Expected Outcome  | Detection and blocking of malicious activity          |
| Criticality       | Critical                                              |

---

## EFSAF-TP-002 — Malware Protection

| Attribute         | Mapping                                     |
| ----------------- | ------------------------------------------- |
| Control Objective | Verify anti-malware inspection capabilities |
| Evidence          | Malware profiles, update status             |
| NIST              | SI                                          |
| PCI DSS           | Malware Protection                          |
| Expected Outcome  | Prevention of malicious file delivery       |
| Criticality       | High                                        |

---

## EFSAF-TP-003 — Threat Intelligence Integration

| Attribute         | Mapping                                           |
| ----------------- | ------------------------------------------------- |
| Control Objective | Validate use of current threat intelligence feeds |
| Evidence          | Feed status, update logs                          |
| ISO               | Threat Intelligence                               |
| NIST CSF          | Detect                                            |
| MITRE ATT&CK      | Threat-Informed Defense                           |
| MITRE D3FEND      | Intelligence Enrichment                           |
| Expected Outcome  | Adaptive protection against emerging threats      |
| Frequency         | Continuous                                        |
| Criticality       | High                                              |

---

# 19. Enterprise Mapping Coverage Summary

| Domain                  | Representative Controls | Primary Framework Coverage                     |
| ----------------------- | ----------------------- | ---------------------------------------------- |
| Architecture Review     | ARCH-001 to ARCH-003    | ISO, NIST, CIS, PCI DSS, IEC 62443, Zero Trust |
| Management Plane Review | MGMT-001 to MGMT-003    | ISO, NIST, CIS, PCI DSS, SOC 2                 |
| Rule Base Review        | RULE-001 to RULE-003    | ISO, NIST, CIS, PCI DSS, Zero Trust            |
| NAT Review              | NAT-001 to NAT-002      | ISO, NIST, PCI DSS                             |
| VPN Review              | VPN-001 to VPN-003      | ISO, NIST, CIS, PCI DSS, Zero Trust            |
| Logging & Monitoring    | LOG-001 to LOG-003      | ISO, NIST, CIS, PCI DSS, SOC 2                 |
| Threat Prevention       | TP-001 to TP-003        | ISO, NIST, CIS, MITRE ATT&CK, D3FEND           |

---

**End of Part 3**

**Part 4** will complete the document with the **Gap Identification Methodology, Compliance Reporting Guidance, Control Validation Process, Cross-Framework Correlation Matrix, Future Framework Extensibility Model, Governance and Maintenance Requirements, Appendices, and the consolidated master cross-reference matrix**, bringing **EFSAF-CMX-001** to a fully enterprise-grade, audit-ready standard suitable for consulting firms, MSSPs, and large enterprise environments.
# EFSAF-CMX-001

# Enterprise Control Mapping Matrix

**Version:** 1.0
**Status:** Official Standard
**Classification:** Enterprise
**Document:** Part 4 of 4 (Final)

---

# 20. Gap Identification Methodology

## 20.1 Purpose

The Enterprise Control Mapping Matrix shall support systematic identification of gaps between the current firewall security posture and applicable cybersecurity frameworks, organizational policies, and regulatory requirements.

Gap analysis shall be evidence-driven, repeatable, and risk-based to ensure consistent assessment outcomes across all EFSAF engagements.

---

## 20.2 Gap Classification Model

Every identified gap shall be assigned one of the following classifications.

| Classification           | Description                                         | Typical Action                              |
| ------------------------ | --------------------------------------------------- | ------------------------------------------- |
| **Compliant**            | Control fully implemented and operating effectively | Maintain and monitor                        |
| **Partially Compliant**  | Control implemented with deficiencies               | Remediate identified weaknesses             |
| **Non-Compliant**        | Required control absent or ineffective              | Immediate remediation                       |
| **Not Applicable (N/A)** | Control legitimately outside assessment scope       | Document justification                      |
| **Compensated**          | Alternative control provides equivalent protection  | Validate compensating control effectiveness |

---

## 20.3 Gap Severity Matrix

| Severity      | Business Impact                                                     | Recommended Timeline      |
| ------------- | ------------------------------------------------------------------- | ------------------------- |
| Critical      | Enterprise compromise, regulatory failure, major service disruption | Immediate (0–7 days)      |
| High          | Significant security exposure                                       | 30 days                   |
| Medium        | Increased operational or security risk                              | 60–90 days                |
| Low           | Minor weakness or optimization opportunity                          | Planned maintenance cycle |
| Informational | Observation only                                                    | No mandatory remediation  |

---

## 20.4 Gap Analysis Workflow

```text
Assessment Activity
        │
        ▼
Evidence Collection
        │
        ▼
Control Validation
        │
        ▼
Framework Crosswalk
        │
        ▼
Gap Identification
        │
        ▼
Risk Evaluation
        │
        ▼
Compliance Impact Analysis
        │
        ▼
Recommendations
        │
        ▼
Executive Reporting
```

---

# 21. Compliance Reporting Guidance

## 21.1 General Requirements

Compliance reports generated under EFSAF shall:

* Be evidence-based.
* Clearly identify assessment scope.
* Reference applicable EFSAF controls.
* Identify mapped external frameworks.
* Document all findings.
* Include risk ratings.
* Include remediation recommendations.
* Maintain traceability to collected evidence.

---

## 21.2 Required Compliance Reporting Elements

Each assessment report should include the following sections.

| Section                | Purpose                                        |
| ---------------------- | ---------------------------------------------- |
| Executive Summary      | High-level assessment outcome                  |
| Assessment Scope       | Systems, locations, and boundaries reviewed    |
| Assessment Methodology | Reference to EFSAF-METH-001 and EFSAF-EXEC-001 |
| Framework Mapping      | Applicable standards and regulations           |
| Findings Summary       | Consolidated assessment results                |
| Risk Register          | Prioritized findings                           |
| Evidence Register      | Supporting artifacts                           |
| Compliance Matrix      | Framework alignment                            |
| Recommendations        | Corrective actions                             |
| Management Response    | Customer feedback (optional)                   |
| Appendix               | Detailed mappings and evidence references      |

---

## 21.3 Compliance Assertion Principles

Assessors shall not state that an organization is fully compliant with a framework solely because EFSAF controls have been successfully assessed.

Instead, reports shall indicate that:

* EFSAF assessment activities support applicable control requirements.
* Additional organizational, procedural, or governance controls may be required to achieve full compliance.
* Final compliance determinations remain the responsibility of the relevant regulatory, certification, or audit authority.

---

# 22. Control Validation Process

## 22.1 Validation Objectives

Control validation ensures that mapped controls are:

* Correctly implemented.
* Operating effectively.
* Producing reliable evidence.
* Meeting intended security objectives.

---

## 22.2 Validation Lifecycle

```text
Control Definition
        │
        ▼
Assessment Execution
        │
        ▼
Evidence Verification
        │
        ▼
Technical Validation
        │
        ▼
Framework Mapping Review
        │
        ▼
Quality Assurance Review
        │
        ▼
Final Reporting
```

---

## 22.3 Validation Criteria

Each mapped control shall be evaluated against the following criteria.

| Criterion        | Description                                     |
| ---------------- | ----------------------------------------------- |
| Applicability    | Control is relevant to assessment scope         |
| Completeness     | Required control components are implemented     |
| Effectiveness    | Control performs intended function              |
| Evidence Quality | Evidence is authentic, complete, and verifiable |
| Repeatability    | Independent assessors can reproduce results     |
| Traceability     | Findings map to frameworks and reports          |

---

# 23. Cross-Framework Correlation Matrix

The following matrix illustrates how EFSAF domains align across major security frameworks.

| EFSAF Domain            | ISO/IEC 27001 | NIST CSF 2.0 | NIST SP 800-53 | CIS v8 | PCI DSS 4.0 | SOC 2   | IEC 62443 | Zero Trust            | MITRE ATT&CK                |
| ----------------------- | ------------- | ------------ | -------------- | ------ | ----------- | ------- | --------- | --------------------- | --------------------------- |
| Architecture Review     | ✓             | ✓            | ✓              | ✓      | ✓           | ✓       | ✓         | ✓                     | Indirect                    |
| Management Plane Review | ✓             | ✓            | ✓              | ✓      | ✓           | ✓       | ✓         | ✓                     | Credential Defense          |
| Rule Base Review        | ✓             | ✓            | ✓              | ✓      | ✓           | ✓       | ✓         | ✓                     | Lateral Movement Mitigation |
| NAT Review              | ✓             | ✓            | ✓              | ✓      | ✓           | Partial | Partial   | ✓                     | Exposure Reduction          |
| VPN Review              | ✓             | ✓            | ✓              | ✓      | ✓           | ✓       | ✓         | ✓                     | Initial Access Mitigation   |
| Logging & Monitoring    | ✓             | ✓            | ✓              | ✓      | ✓           | ✓       | ✓         | Continuous Monitoring | Detection Support           |
| Threat Prevention       | ✓             | ✓            | ✓              | ✓      | ✓           | Partial | ✓         | Adaptive Enforcement  | Attack Detection            |

---

# 24. Framework Coverage Assurance

EFSAF shall maintain mappings that collectively support the following security functions.

| Security Function        | Covered by EFSAF |
| ------------------------ | ---------------- |
| Governance               | ✓                |
| Asset Protection         | ✓                |
| Access Control           | ✓                |
| Secure Administration    | ✓                |
| Network Segmentation     | ✓                |
| Secure Communications    | ✓                |
| Threat Prevention        | ✓                |
| Logging & Monitoring     | ✓                |
| Incident Detection       | ✓                |
| Configuration Management | ✓                |
| Risk Management          | ✓                |
| Compliance Reporting     | ✓                |
| Continuous Improvement   | ✓                |

---

# 25. Future Framework Extensibility

## 25.1 Extensibility Principles

The EFSAF Control Mapping Matrix is designed to evolve alongside the cybersecurity landscape.

Future framework integrations shall:

* Preserve existing control identifiers.
* Maintain backward compatibility where practical.
* Avoid duplicate mappings.
* Include documented version history.
* Undergo peer review before publication.

---

## 25.2 Candidate Frameworks

Future versions of EFSAF may include mappings to:

* NIS2 Directive
* DORA (Digital Operational Resilience Act)
* HIPAA Security Rule
* HITRUST CSF
* COBIT 2019
* CSA Cloud Controls Matrix (CCM)
* Australian Essential Eight
* CMMC
* National or sector-specific regulatory baselines

---

## 25.3 Versioning Requirements

When framework updates occur:

1. Review affected mappings.
2. Identify deprecated references.
3. Validate revised mappings.
4. Update documentation.
5. Publish change log.
6. Retain historical mappings for audit purposes.

---

# 26. Governance and Maintenance

## 26.1 Ownership

The EFSAF Project Governance Team shall maintain the Enterprise Control Mapping Matrix.

Responsibilities include:

* Reviewing framework revisions.
* Updating mappings.
* Approving new control relationships.
* Maintaining version control.
* Coordinating peer reviews.
* Publishing official releases.

---

## 26.2 Review Frequency

| Activity                   | Frequency                     |
| -------------------------- | ----------------------------- |
| Editorial Review           | Annually                      |
| Framework Alignment Review | Upon major framework release  |
| Technical Peer Review      | Annually                      |
| Quality Assurance Review   | Before every official release |
| Version Publication        | As required                   |

---

## 26.3 Change Management

Changes to the matrix shall be:

* Documented.
* Version controlled.
* Peer reviewed.
* Technically validated.
* Approved by project governance before publication.

---

# 27. Assessment Integration

The Enterprise Control Mapping Matrix shall be used in conjunction with:

* **EFSAF-METH-001** — Enterprise Firewall Security Assessment Methodology
* **EFSAF-EXEC-001** — Enterprise Firewall Security Assessment Execution Guide
* **EFSAF-SCORE-001** — Enterprise Scoring Standard
* **EFSAF-RISK-001** — Risk Rating Standard
* **EFSAF-EVD-001** — Evidence Collection Standard
* **EFSAF-REP-001** — Reporting Standard
* **EFSAF-MAP-001** — Assessment Mapping Standard
* **EFSAF-TMP-001** — Enterprise Assessment Templates

Collectively, these documents establish a complete, repeatable, and auditable enterprise firewall security assessment methodology.

---

# Appendix A — Master Control Cross-Reference

| EFSAF Domain                | Primary Objective             | Primary Risk             | Primary Evidence                                      | Primary Framework Families         |
| --------------------------- | ----------------------------- | ------------------------ | ----------------------------------------------------- | ---------------------------------- |
| Architecture Review         | Secure Architecture           | Architecture Risk        | Network diagrams, topology, segmentation design       | ISO, NIST, CIS, PCI DSS, IEC 62443 |
| Management Plane Review     | Secure Administration         | Privileged Access Risk   | AAA configuration, MFA, management settings           | ISO, NIST, CIS, SOC 2              |
| Rule Base Review            | Least Privilege               | Unauthorized Access Risk | Firewall policies, rule analysis                      | ISO, NIST, PCI DSS, Zero Trust     |
| NAT Review                  | Secure Address Translation    | Exposure Risk            | NAT tables, translation policies                      | ISO, NIST, PCI DSS                 |
| VPN Review                  | Secure Remote Connectivity    | Remote Access Risk       | VPN configuration, authentication logs                | ISO, NIST, CIS, Zero Trust         |
| Logging & Monitoring Review | Visibility and Accountability | Detection Risk           | Logs, SIEM events, audit trails                       | ISO, NIST, PCI DSS, SOC 2          |
| Threat Prevention Review    | Active Threat Defense         | Cyber Threat Risk        | IPS policies, threat intelligence, malware protection | ISO, NIST, MITRE ATT&CK, D3FEND    |

---

# Appendix B — Control Metadata Requirements

Each EFSAF control record shall include, at a minimum:

* Control Identifier
* Control Name
* Assessment Domain
* Security Objective
* Assessment Procedure Reference
* Risk Category
* Evidence Requirements
* Applicable Standards
* Compliance References
* MITRE ATT&CK Mapping (where applicable)
* MITRE D3FEND Mapping (where applicable)
* CAPEC Mapping (where applicable)
* CWE Mapping (where applicable)
* Expected Security Outcome
* Assessment Frequency
* Control Criticality
* Scoring Weight
* Reporting Reference
* Version
* Last Review Date

---

# Appendix C — Key Performance Indicators (KPIs)

Organizations using EFSAF should monitor the following metrics to measure assessment maturity and control effectiveness.

| KPI                             | Description                                                 |
| ------------------------------- | ----------------------------------------------------------- |
| Framework Coverage              | Percentage of applicable external controls mapped by EFSAF  |
| Control Assessment Completion   | Percentage of planned controls assessed                     |
| Evidence Completeness           | Percentage of controls with complete supporting evidence    |
| Critical Findings Rate          | Number of critical findings per assessment                  |
| Mean Time to Remediation (MTTR) | Average time to close identified findings                   |
| Repeat Finding Rate             | Percentage of findings recurring across assessment cycles   |
| Compliance Alignment            | Percentage of EFSAF controls aligned to required frameworks |
| Control Validation Success Rate | Percentage of controls validated without exceptions         |
| Reporting Timeliness            | Percentage of reports delivered within agreed timelines     |

---

# Appendix D — Normative Requirements Summary

The following requirements are mandatory for all official EFSAF assessments:

* Every assessment **shall** use the official EFSAF control identifiers.
* Every assessed control **shall** maintain end-to-end traceability from procedure to evidence and report.
* Every control **shall** be mapped to applicable international standards where relevant.
* Every finding **shall** include supporting evidence.
* Every risk rating **shall** follow **EFSAF-RISK-001**.
* Every score **shall** follow **EFSAF-SCORE-001**.
* Every report **shall** conform to **EFSAF-REP-001**.
* Every mapping **should** be reviewed whenever a referenced framework is materially revised.
* Compensating controls **may** be accepted where they provide demonstrably equivalent protection and are fully documented.
* Historical mappings **shall** be retained to support audits, regulatory reviews, and longitudinal security assessments.

---

# Document Completion

**EFSAF-CMX-001 — Enterprise Control Mapping Matrix** is now complete.

This document serves as the **authoritative compliance crosswalk** for the Enterprise Firewall Security Assessment Framework (EFSAF), providing:

* A standardized methodology for mapping firewall assessment controls to international cybersecurity frameworks.
* End-to-end traceability from assessment procedures through evidence, risk, scoring, and reporting.
* Cross-framework alignment with ISO/IEC 27001/27002, NIST CSF 2.0, NIST SP 800-53 Rev. 5, CIS Controls v8, PCI DSS v4.0, SOC 2, IEC 62443, Zero Trust Architecture, MITRE ATT&CK, MITRE D3FEND, CAPEC, and CWE.
* A governance model supporting version control, maintenance, and future extensibility.
* An audit-ready structure suitable for enterprise security teams, MSSPs, consulting organizations, GRC professionals, and independent assessors.

**End of EFSAF-CMX-001**

