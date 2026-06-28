# Enterprise Evidence Collection and Validation Standard

**Document ID:** EFSAF-EVD-001

**Version:** 1.0

**Status:** Approved

**Classification:** Enterprise Standard

**Framework:** Enterprise Firewall Security Assessment Framework (EFSAF)

**Owner:** EFSAF Project

**Review Cycle:** Annual or Following Significant Framework Changes

**Effective Date:** June 2026

---

# Document Control

| Field            | Value                                                     |
| ---------------- | --------------------------------------------------------- |
| Document Title   | Enterprise Evidence Collection and Validation Standard    |
| Document ID      | EFSAF-EVD-001                                             |
| Version          | 1.0                                                       |
| Status           | Approved                                                  |
| Classification   | Enterprise Standard                                       |
| Framework        | Enterprise Firewall Security Assessment Framework (EFSAF) |
| Owner            | EFSAF Project                                             |
| Review Frequency | Annual                                                    |
| Applies To       | All EFSAF Assessment Modules                              |
| Supersedes       | None                                                      |
| Next Review      | June 2027                                                 |

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
4. Evidence Governance
5. Evidence Management Principles
6. Roles and Responsibilities
7. Evidence Lifecycle
8. Evidence Classification
9. Evidence Quality Model
10. Evidence Assurance Model

> **Note:** Collection methods, validation techniques, chain of custody, integrity verification, evidence templates, reporting requirements, and appendices are defined in subsequent parts of this standard.

---

# 1. Purpose

The **Enterprise Evidence Collection and Validation Standard (EFSAF-EVD-001)** establishes the mandatory requirements for the identification, collection, validation, protection, classification, management, and presentation of evidence obtained during Enterprise Firewall Security Assessments performed under the Enterprise Firewall Security Assessment Framework (EFSAF).

Evidence forms the foundation of every assessment finding. Consequently, no observation, recommendation, or risk rating shall be considered valid unless it is supported by sufficient, verifiable, and traceable evidence collected in accordance with this standard.

This document ensures that evidence collected by different assessors remains consistent, defensible, reproducible, and suitable for technical review, executive reporting, compliance activities, and future reassessments.

---

# 2. Scope

This standard applies to all evidence collected throughout the EFSAF assessment lifecycle, regardless of deployment model, vendor, or technology platform.

The standard governs evidence produced during, but not limited to:

* Architecture Reviews
* Management Plane Reviews
* Rule Base Reviews
* NAT Reviews
* VPN Reviews
* Logging & Monitoring Reviews
* Threat Prevention Reviews
* High Availability Reviews
* Identity and Authentication Reviews
* Certificate and PKI Reviews
* Cloud Firewall Assessments
* SD-WAN Security Assessments
* Future EFSAF assessment modules

Evidence obtained from manual reviews, automated tools, APIs, management consoles, configuration exports, log analysis, packet captures, cloud services, and third-party security platforms shall comply with this standard.

---

# 3. Objectives

The objectives of this standard are to:

* Establish a consistent evidence collection methodology.
* Ensure evidence integrity throughout the assessment lifecycle.
* Support objective and repeatable technical assessments.
* Improve the quality and reliability of assessment findings.
* Enable independent validation of reported observations.
* Maintain traceability between evidence, findings, and recommendations.
* Support regulatory, compliance, and audit activities.
* Standardize evidence handling across all EFSAF modules.
* Reduce assessor subjectivity through documented validation procedures.
* Improve long-term maintainability of assessment records.

---

# 4. Evidence Governance

Evidence governance defines the organizational controls necessary to ensure that evidence remains accurate, complete, protected, and trustworthy throughout its lifecycle.

Evidence shall be managed as a controlled assessment asset rather than supporting documentation.

The governance model is based on the following principles:

* Accountability
* Integrity
* Confidentiality
* Traceability
* Repeatability
* Auditability
* Standardization
* Controlled Change Management

Any modification to collected evidence after acquisition shall be documented and justified. Original evidence shall be preserved whenever possible.

---

## 4.1 Governance Objectives

Evidence governance seeks to ensure that:

* Every finding is supported by documented evidence.
* Evidence remains attributable to its original source.
* Evidence is protected against unauthorized modification.
* Evidence can be independently verified.
* Evidence remains available throughout the assessment lifecycle.
* Evidence handling practices satisfy organizational and regulatory requirements.

---

# 5. Evidence Management Principles

The following principles govern all evidence activities performed under EFSAF.

## 5.1 Accuracy

Evidence shall accurately represent the observed system state at the time of collection.

Evidence shall not be edited, manipulated, or selectively presented in a manner that changes its meaning or technical interpretation.

---

## 5.2 Completeness

Evidence shall provide sufficient information to support the associated finding without requiring assumptions.

Where additional context is necessary, supplementary evidence shall be collected.

---

## 5.3 Authenticity

Assessors shall verify that collected evidence originates from the intended source.

Evidence shall include sufficient metadata to identify:

* Source system
* Collection date and time
* Assessment module
* Collection method
* Assessor (where applicable)

---

## 5.4 Integrity

Evidence shall remain protected against unauthorized alteration throughout its lifecycle.

Integrity controls may include:

* Read-only storage
* Cryptographic hashing
* Access controls
* Version control
* Audit logging

---

## 5.5 Traceability

Every evidence item shall be traceable to:

* Assessment engagement
* EFSAF control
* Assessment module
* Finding identifier
* Risk assessment
* Final recommendation

Evidence that cannot be traced to a documented finding should not be retained within the assessment evidence repository.

---

## 5.6 Repeatability

Independent assessors should be able to reproduce assessment conclusions using the documented evidence and collection methodology.

Repeatability is a key requirement for quality assurance and peer review.

---

## 5.7 Confidentiality

Evidence frequently contains sensitive organizational information.

Appropriate safeguards shall be implemented to prevent unauthorized disclosure of:

* Administrative accounts
* IP addressing information
* Security policies
* Cryptographic material
* Certificates
* Firewall configurations
* Internal network architecture
* Authentication information

Evidence shall be handled according to the organization's information classification policy.

---

# 6. Roles and Responsibilities

Evidence management requires clearly defined ownership and accountability.

| Role                       | Responsibilities                                                                                                            |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Assessment Lead            | Approves evidence collection strategy, validates evidence completeness, and authorizes evidence inclusion in final reports. |
| Security Assessor          | Collects, documents, validates, and references assessment evidence.                                                         |
| Technical Reviewer         | Independently verifies evidence quality, authenticity, and relevance.                                                       |
| Quality Assurance Reviewer | Confirms compliance with EFSAF evidence standards.                                                                          |
| System Owner               | Provides access to systems, validates environmental context, and assists in evidence interpretation where necessary.        |
| Risk Owner                 | Reviews evidence supporting identified risks before risk acceptance decisions.                                              |

Segregation of duties should be maintained wherever practical to preserve assessment independence.

---

# 7. Evidence Lifecycle

Evidence shall be managed through a controlled lifecycle.

```text
Identify
      │
      ▼
Collect
      │
      ▼
Validate
      │
      ▼
Classify
      │
      ▼
Reference
      │
      ▼
Protect
      │
      ▼
Use
      │
      ▼
Archive
      │
      ▼
Dispose
```

Each stage shall be documented to preserve traceability and support future reassessment.

---

## 7.1 Identify

Determine the evidence required to validate assessment objectives.

---

## 7.2 Collect

Acquire evidence using approved collection techniques while preserving system integrity and minimizing operational impact.

---

## 7.3 Validate

Confirm that the evidence is complete, authentic, and relevant to the identified observation.

---

## 7.4 Classify

Assign an appropriate evidence classification and sensitivity level.

---

## 7.5 Reference

Associate each evidence item with the corresponding EFSAF control, assessment module, and finding identifier.

---

## 7.6 Protect

Safeguard evidence against unauthorized modification, disclosure, or loss.

---

## 7.7 Archive

Retain evidence according to organizational retention requirements and EFSAF governance standards.

---

## 7.8 Dispose

Securely dispose of evidence when retention requirements have expired and disposal has been authorized.

---

# 8. Evidence Classification

Evidence shall be classified according to its technical purpose.

The following categories are defined.

| Category                 | Description                                                                          |
| ------------------------ | ------------------------------------------------------------------------------------ |
| Configuration Evidence   | Configuration exports, XML files, CLI outputs, API responses.                        |
| Visual Evidence          | Screenshots, dashboards, management interfaces, topology diagrams.                   |
| Log Evidence             | Traffic logs, threat logs, authentication logs, system logs, audit logs.             |
| Network Evidence         | Packet captures, flow records, protocol analysis.                                    |
| Cloud Evidence           | Cloud-native security logs, API responses, cloud configuration exports.              |
| Third-Party Evidence     | SIEM reports, vulnerability assessments, DDI platforms, EDR outputs.                 |
| Supporting Documentation | Architecture diagrams, change records, approved procedures, technical documentation. |

An evidence item may belong to multiple categories where appropriate.

---

# 9. Evidence Quality Model

Evidence quality directly affects the reliability of assessment findings.

Every evidence item should be assigned one of the following quality levels.

| Quality Level | Description                                                                                                        |
| ------------- | ------------------------------------------------------------------------------------------------------------------ |
| Excellent     | Complete, independently verifiable, current, and directly supports the finding without additional assumptions.     |
| Good          | Sufficient to support the finding with only minor supplementary context required.                                  |
| Acceptable    | Supports the finding but contains limitations that should be documented.                                           |
| Limited       | Partial evidence requiring additional validation before conclusions can be finalized.                              |
| Insufficient  | Does not adequately support the associated finding and shall not be used as the sole basis for risk determination. |

Only **Excellent**, **Good**, and **Acceptable** evidence should normally support finalized findings.

---

# 10. Evidence Assurance Model

Evidence assurance provides confidence that collected evidence remains suitable for decision-making.

Evidence should satisfy the following criteria:

| Assurance Requirement | Description                                                     |
| --------------------- | --------------------------------------------------------------- |
| Authentic             | Originates from a trusted source.                               |
| Accurate              | Represents the observed environment without distortion.         |
| Complete              | Contains sufficient context to support the associated finding.  |
| Relevant              | Directly relates to the assessment objective.                   |
| Timely                | Reflects the assessed environment during the engagement period. |
| Traceable             | Can be linked to findings, controls, and recommendations.       |
| Reviewable            | Can be independently validated by another assessor.             |

Evidence failing to meet these assurance requirements should be supplemented or replaced before the associated finding is finalized.

---

## End of Part 1

**Part 2** defines the operational standards for evidence acquisition and validation, including:

* Configuration Evidence Standards
* Screenshot Evidence Standards
* CLI Output Standards
* API Evidence Standards
* Firewall Log Evidence
* Packet Capture Standards
* Cloud Platform Evidence
* Third-Party Security Tool Evidence
* Evidence Validation Methodology
* Collection Best Practices
* Evidence Collection Checklists

## Part 2 – Evidence Collection Standards and Validation Methodology

---

# 11. Evidence Collection Methodology

## 11.1 Overview

Evidence collection shall be conducted using a structured, repeatable, and minimally intrusive methodology designed to preserve system integrity while obtaining sufficient information to support assessment findings.

Evidence collection shall:

* Follow the approved assessment scope.
* Minimize operational impact.
* Avoid unauthorized system modification.
* Preserve evidence integrity.
* Support independent validation.
* Be fully documented.

Evidence shall be collected only after confirming appropriate authorization from the system owner or designated representative.

---

## 11.2 Collection Workflow

All evidence collection activities shall follow the standardized EFSAF workflow.

```text
Assessment Scope Approved
        │
        ▼
Identify Required Evidence
        │
        ▼
Select Collection Method
        │
        ▼
Collect Evidence
        │
        ▼
Validate Evidence
        │
        ▼
Classify Evidence
        │
        ▼
Assign Evidence ID
        │
        ▼
Secure Storage
        │
        ▼
Reference in Findings
```

This workflow ensures consistency and traceability across all EFSAF engagements.

---

# 12. Configuration Evidence Standards

Configuration evidence provides direct insight into the security posture of the assessed firewall or related infrastructure.

Typical sources include:

* Running configuration exports
* Candidate configurations
* XML configuration files
* Backup configuration files
* Policy exports
* Routing tables
* Interface configurations
* High Availability configurations

Configuration evidence shall:

* Be exported directly from the management interface, CLI, or approved API.
* Include the date and time of collection.
* Preserve original formatting.
* Avoid manual modification.
* Be stored in its native format where possible.

Where sensitive information is redacted for reporting purposes, the original evidence shall be retained in the protected evidence repository.

---

# 13. Screenshot Evidence Standards

Screenshots provide visual confirmation of observed configurations and system states.

Screenshots should:

* Clearly display the relevant configuration or event.
* Include sufficient surrounding context.
* Display timestamps where available.
* Show system identifiers where appropriate.
* Maintain readable resolution.
* Avoid unnecessary cropping.

Where multiple screenshots are required to support a finding, they shall be logically sequenced and individually referenced.

Annotated copies may be used in reports; however, original unmodified screenshots shall be retained.

---

# 14. Command-Line Interface (CLI) Evidence

CLI output often provides the most authoritative evidence for firewall assessments.

Examples include:

* Security policy listings
* NAT rules
* VPN configuration
* Interface status
* Routing tables
* Certificate information
* User accounts
* System version
* High Availability status

CLI evidence shall:

* Capture the complete command output.
* Record the executed command.
* Preserve terminal formatting.
* Include hostname and prompt where practical.
* Avoid truncation.

Commands that modify system configuration shall not be executed solely for evidence collection unless explicitly authorized.

---

# 15. Log Evidence Standards

Logs provide objective evidence of system activity and security events.

Examples include:

* Traffic logs
* Threat prevention logs
* Authentication logs
* Administrative audit logs
* System logs
* Configuration change logs
* VPN logs
* URL filtering logs
* DNS security logs

Collected logs should include:

* Timestamp
* Event type
* Source
* Destination
* Action
* Severity
* User (where applicable)
* Session identifier (if available)

Log collection shall preserve original timestamps and avoid filtering unless required by the assessment scope.

---

# 16. Packet Capture (PCAP) Standards

Packet captures provide network-level evidence supporting firewall behavior and traffic analysis.

Packet captures may be collected to validate:

* Rule matching
* NAT translation
* VPN encapsulation
* Application identification
* Threat detection
* Network connectivity
* DNS behavior
* SSL/TLS negotiation

Packet captures shall include:

* Collection interface
* Capture duration
* Applied capture filters
* Time synchronization
* Collection method

Capture scope should be limited to the minimum required to satisfy assessment objectives.

---

# 17. API Evidence Standards

Many enterprise firewall platforms expose management information through APIs.

API evidence may include:

* Configuration exports
* Security policy objects
* Administrative accounts
* Device status
* System inventory
* Logging configuration
* Certificate information

API responses shall:

* Be collected using authenticated sessions.
* Preserve original JSON or XML formatting.
* Record the request endpoint.
* Record the response timestamp.
* Record API version where available.

Sensitive authentication tokens shall never be included in assessment reports.

---

# 18. Cloud Platform Evidence

Cloud-native firewall assessments require evidence from cloud management platforms.

Examples include:

* Virtual firewall configurations
* Security groups
* Network ACLs
* Route tables
* Cloud logging services
* IAM policies
* Cloud-native threat detection
* Cloud audit logs

Cloud evidence should include:

* Cloud provider
* Region
* Resource identifier
* Collection timestamp
* Subscription or account identifier (where appropriate)

Cloud evidence shall be validated against the deployed environment.

---

# 19. Third-Party Security Tool Evidence

EFSAF assessments may rely on supporting evidence from approved security platforms.

Examples include:

* SIEM
* SOAR
* Vulnerability scanners
* DNS security platforms
* Endpoint Detection and Response (EDR)
* Network Detection and Response (NDR)
* Threat Intelligence Platforms
* Configuration management systems

Third-party evidence shall:

* Identify the originating platform.
* Include collection timestamps.
* Preserve original formatting where possible.
* Be independently validated before supporting High or Critical findings.

Third-party evidence supplements, but does not replace, direct technical validation.

---

# 20. Evidence Validation Methodology

Evidence shall be validated before it is used to support an assessment finding.

Validation confirms:

* Authenticity
* Accuracy
* Completeness
* Relevance
* Timeliness

Validation activities may include:

* Cross-checking multiple evidence sources.
* Comparing CLI output with management interface data.
* Reviewing configuration exports against live system status.
* Confirming timestamps.
* Verifying consistency across logs.

Findings shall not rely on unvalidated evidence.

---

# 21. Evidence Correlation

Single evidence items rarely provide sufficient context for enterprise findings.

Assessors should correlate evidence from multiple sources.

Example:

```text
Running Configuration
        │
        ▼
Firewall Logs
        │
        ▼
Threat Prevention Events
        │
        ▼
Packet Capture
        │
        ▼
Assessment Finding
```

Correlated evidence improves confidence and reduces the likelihood of inaccurate conclusions.

---

# 22. Evidence Collection Best Practices

Assessors should adhere to the following practices:

* Collect evidence as close as possible to the time of observation.
* Preserve original evidence.
* Minimize impact on production systems.
* Avoid unnecessary privileged actions.
* Record collection methods.
* Validate evidence immediately after collection.
* Document environmental assumptions.
* Protect sensitive information.
* Use standardized naming conventions.
* Store evidence in approved repositories.

---

# 23. Evidence Collection Checklist

The following checklist should be completed before finalizing evidence collection.

| Verification Item               | Status |
| ------------------------------- | ------ |
| Assessment scope confirmed      | ✓      |
| Required authorization obtained | ✓      |
| Evidence source identified      | ✓      |
| Collection method documented    | ✓      |
| Evidence validated              | ✓      |
| Evidence classified             | ✓      |
| Evidence ID assigned            | ✓      |
| Secure storage confirmed        | ✓      |
| Sensitive information protected | ✓      |
| Traceability established        | ✓      |

Completion of this checklist helps ensure consistency across all EFSAF assessments.

---

## End of Part 2

# Enterprise Evidence Collection and Validation Standard

**Document ID:** EFSAF-EVD-001

## Part 3 – Evidence Integrity, Protection, Traceability, and Quality Assurance

---

# 24. Evidence Integrity

## 24.1 Purpose

Evidence integrity ensures that assessment evidence remains complete, accurate, authentic, and protected from unauthorized modification throughout its lifecycle.

Integrity is fundamental to maintaining confidence in assessment findings and supporting independent technical validation, compliance reviews, and audit activities.

Evidence that cannot demonstrate integrity shall not be used as the sole basis for assessment findings.

---

## 24.2 Integrity Objectives

Evidence integrity controls shall ensure that evidence remains:

* Complete
* Authentic
* Accurate
* Unmodified
* Traceable
* Reviewable
* Reproducible

---

## 24.3 Integrity Controls

Organizations should implement appropriate controls including:

| Control               | Purpose                           |
| --------------------- | --------------------------------- |
| Read-only storage     | Prevent unauthorized modification |
| Cryptographic hashing | Verify evidence integrity         |
| Access logging        | Record all evidence access        |
| Version control       | Preserve historical copies        |
| Backup                | Prevent accidental loss           |
| Encryption            | Protect sensitive evidence        |
| Audit trail           | Maintain accountability           |

---

# 25. Cryptographic Integrity Verification

Where practical, critical evidence files should be protected using cryptographic hash functions.

Recommended algorithms:

* SHA-256
* SHA-384
* SHA-512

MD5 and SHA-1 shall not be used for integrity verification due to known cryptographic weaknesses.

Example Evidence Record

| Field          | Example                    |
| -------------- | -------------------------- |
| Evidence ID    | EVD-RULE-001               |
| File           | RunningConfig.xml          |
| Hash Algorithm | SHA-256                    |
| Hash Value     | Recorded during collection |
| Verified       | Yes                        |

Hash values should be generated immediately after evidence collection.

---

# 26. Chain of Custody

## 26.1 Purpose

The Chain of Custody documents the complete history of evidence from acquisition through disposal.

It provides assurance that evidence has remained under controlled management throughout its lifecycle.

---

## 26.2 Chain of Custody Workflow

```text
Evidence Created
        │
        ▼
Evidence Collected
        │
        ▼
Evidence Validated
        │
        ▼
Evidence Stored
        │
        ▼
Evidence Reviewed
        │
        ▼
Evidence Referenced
        │
        ▼
Evidence Archived
        │
        ▼
Evidence Disposed
```

---

## 26.3 Required Metadata

Each evidence item should record:

| Metadata               | Required |
| ---------------------- | -------- |
| Evidence ID            | Yes      |
| Collection Date        | Yes      |
| Collection Time        | Yes      |
| Assessor               | Yes      |
| Source Device          | Yes      |
| Assessment Module      | Yes      |
| Collection Method      | Yes      |
| Classification         | Yes      |
| Storage Location       | Yes      |
| Integrity Verification | Yes      |

---

# 27. Evidence Repository

Evidence shall be stored within an approved repository.

Repository requirements include:

* Role-based access control
* Encryption at rest
* Backup protection
* Version history
* Audit logging
* Search capability
* Controlled deletion
* Secure archival

The repository shall support long-term evidence preservation while preventing unauthorized modification.

---

# 28. Evidence Access Control

Evidence frequently contains highly sensitive organizational information.

Access should follow the Principle of Least Privilege.

Typical permissions include:

| Role               | Access            |
| ------------------ | ----------------- |
| Assessment Lead    | Full              |
| Security Assessor  | Assigned evidence |
| Technical Reviewer | Read-only         |
| QA Reviewer        | Read-only         |
| Executive Sponsor  | Report only       |
| System Owner       | As approved       |

All access should be logged.

---

# 29. Evidence Version Management

Evidence versions shall be controlled.

Original evidence shall never be overwritten.

Recommended lifecycle:

```text
Original Evidence
        │
        ▼
Working Copy
        │
        ▼
Reviewed Copy
        │
        ▼
Published Reference
```

Every modification shall be documented.

---

# 30. Evidence Traceability

Every evidence item shall maintain complete traceability.

```text
Evidence ID
      │
      ▼
EFSAF Module
      │
      ▼
Control ID
      │
      ▼
Finding
      │
      ▼
Risk Assessment
      │
      ▼
Recommendation
      │
      ▼
Compliance Mapping
```

This relationship enables end-to-end validation of every assessment conclusion.

---

# 31. Evidence Review Process

Collected evidence shall undergo structured review before supporting finalized findings.

Review objectives include:

* Technical accuracy
* Completeness
* Authenticity
* Relevance
* Integrity
* Classification
* Traceability

High and Critical findings should undergo independent evidence review.

---

# 32. Quality Assurance

Quality Assurance confirms compliance with EFSAF-EVD-001.

Review areas include:

| QA Activity           | Purpose                              |
| --------------------- | ------------------------------------ |
| Collection Review     | Verify collection process            |
| Validation Review     | Confirm evidence authenticity        |
| Classification Review | Verify classification                |
| Integrity Review      | Confirm no unauthorized modification |
| Traceability Review   | Verify mapping to findings           |
| Documentation Review  | Confirm completeness                 |

Assessments should not proceed to reporting until QA activities have been completed.

---

# 33. Non-Conforming Evidence

Evidence shall be classified as Non-Conforming if it:

* Cannot be authenticated.
* Is incomplete.
* Has been modified without authorization.
* Lacks sufficient context.
* Cannot be traced to its source.
* Is inconsistent with validated system state.

Non-Conforming evidence shall not support finalized findings unless independently validated through alternative sources.

---

# 34. Evidence Exceptions

Occasionally, assessors may be unable to obtain ideal evidence due to operational constraints.

Examples include:

* Restricted administrative access.
* Production system limitations.
* Regulatory restrictions.
* Third-party ownership.
* Legacy infrastructure.

All evidence exceptions shall document:

* Reason
* Impact
* Alternative validation method
* Risk introduced
* Assessment Lead approval

---

# 35. Evidence Audit Trail

Every evidence item should maintain an audit trail recording:

* Collection
* Validation
* Access
* Review
* Modification (where permitted)
* Publication
* Archive
* Disposal

Audit records improve accountability and support future investigations.

---

# 36. Evidence Quality Metrics

Organizations should monitor evidence quality using measurable indicators.

Recommended metrics include:

| KPI                   | Description                                                 |
| --------------------- | ----------------------------------------------------------- |
| Evidence Completeness | Percentage of findings supported by complete evidence       |
| Validation Rate       | Percentage of evidence independently validated              |
| Traceability Coverage | Percentage of evidence mapped to findings                   |
| QA Pass Rate          | Percentage of evidence passing QA without rework            |
| Exception Rate        | Percentage of findings requiring evidence exceptions        |
| Review Completion     | Percentage of High/Critical findings independently reviewed |

These metrics help drive continuous improvement in assessment quality.

---

# End of Part 3

**Document ID:** EFSAF-EVD-001

## Part 4 – Operational Standards, Templates, Governance, and Appendices

---

# 37. Evidence Naming Convention

## 37.1 Purpose

A standardized naming convention ensures evidence remains uniquely identifiable, searchable, and traceable throughout the assessment lifecycle.

Every evidence item shall be assigned a unique identifier at the time of collection.

---

## 37.2 Evidence Identifier Structure

The recommended EFSAF evidence identifier format is:

```text
EVD-<MODULE>-<CONTROL>-<SEQUENCE>
```

### Examples

| Evidence ID      | Description                                          |
| ---------------- | ---------------------------------------------------- |
| EVD-MGMT-001-001 | Management Plane evidence for Control 001            |
| EVD-RULE-014-003 | Third evidence item supporting Rule Base Control 014 |
| EVD-VPN-008-002  | VPN evidence supporting Control 008                  |
| EVD-LOG-021-001  | Logging & Monitoring evidence                        |

Evidence identifiers shall remain unique within an assessment engagement.

---

# 38. File Naming Standard

Evidence files should follow a consistent naming format.

```text
<Client>_<Device>_<Module>_<EvidenceType>_<YYYYMMDD>_<Sequence>
```

### Examples

```text
ABCBank_FW01_RULE_Config_20260628_001.xml

ABCBank_FW01_LOG_Traffic_20260628_001.csv

ABCBank_FW01_VPN_Screenshot_20260628_002.png

ABCBank_FW01_MGMT_CLI_20260628_001.txt
```

This convention simplifies indexing, retrieval, and long-term maintenance.

---

# 39. Screenshot Annotation Standard

Annotated screenshots improve clarity without replacing the original evidence.

Annotations may include:

* Highlight boxes
* Arrows
* Callout labels
* Finding references

Annotations shall:

* Clearly identify the relevant observation.
* Avoid obscuring original information.
* Preserve readability.
* Be applied only to working copies.

Original screenshots shall always remain unmodified.

---

# 40. Evidence Referencing Standard

Every assessment finding shall explicitly reference supporting evidence.

Minimum reference fields:

| Field             | Required |
| ----------------- | -------- |
| Evidence ID       | Yes      |
| Evidence Type     | Yes      |
| Collection Date   | Yes      |
| Assessment Module | Yes      |
| Finding ID        | Yes      |

Example:

```text
Finding ID:
RULE-014

Supporting Evidence:

EVD-RULE-014-001

Running Configuration Export

Collected:
28 June 2026
```

---

# 41. Evidence Register

Each assessment engagement should maintain a centralized Evidence Register.

Recommended fields:

| Field               |
| ------------------- |
| Evidence ID         |
| Assessment Module   |
| Control ID          |
| Finding ID          |
| Evidence Type       |
| Source              |
| Collection Method   |
| Assessor            |
| Collection Date     |
| Classification      |
| Quality Rating      |
| Integrity Verified  |
| Repository Location |
| Review Status       |

The Evidence Register serves as the authoritative inventory of all collected evidence.

---

# 42. Chain of Custody Register

Organizations should maintain a Chain of Custody Register for critical evidence.

Recommended fields:

| Field          |
| -------------- |
| Evidence ID    |
| Collected By   |
| Date           |
| Time           |
| Source Device  |
| Hash Value     |
| Repository     |
| Access History |
| Reviewer       |
| Archive Date   |

This register provides accountability and supports audit requirements.

---

# 43. Evidence Validation Checklist

Before evidence supports a finalized finding, assessors should verify:

| Validation Requirement     | Status |
| -------------------------- | ------ |
| Source verified            | ✓      |
| Collection authorized      | ✓      |
| Evidence complete          | ✓      |
| Integrity confirmed        | ✓      |
| Classification assigned    | ✓      |
| Metadata recorded          | ✓      |
| Traceability established   | ✓      |
| Reviewer approval obtained | ✓      |

Completion of this checklist helps ensure consistent evidence quality.

---

# 44. Evidence Retention

Evidence shall be retained in accordance with organizational policy, contractual obligations, and applicable regulatory requirements.

Retention periods should consider:

* Legal requirements
* Audit requirements
* Internal governance
* Customer obligations
* Regulatory frameworks
* Assessment lifecycle

Where no formal policy exists, organizations should define retention periods before commencing assessments.

---

# 45. Secure Disposal

Upon expiration of retention requirements, evidence shall be securely disposed of using approved methods.

Examples include:

* Cryptographic erasure
* Secure deletion
* Physical destruction of removable media
* Approved archival disposal procedures

Disposal activities should be documented for audit purposes.

---

# 46. Confidentiality and Information Handling

Evidence collected during firewall security assessments frequently contains sensitive information.

Examples include:

* Firewall configurations
* Administrative credentials (masked or excluded where possible)
* Internal IP addressing
* VPN configurations
* Routing information
* Security policies
* Cryptographic certificates
* Network topology

Evidence shall be handled according to the organization's information classification policy and shared only with authorized personnel.

---

# 47. Integration with EFSAF Assessment Modules

This standard applies to every EFSAF assessment module.

Including:

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

All findings generated by these modules shall comply with the evidence collection, validation, integrity, and traceability requirements defined in EFSAF-EVD-001.

---

# 48. Integration with Other EFSAF Standards

EFSAF-EVD-001 operates alongside the following framework standards:

* **EFSAF-RISK-001** – Enterprise Risk Assessment Methodology
* **EFSAF-TAX-001** – EFSAF Taxonomy (planned)
* **EFSAF-COMP-001** – Compliance Mapping Standard (planned)
* **EFSAF-STD-001** – Documentation Standard (planned)

Together, these standards establish a complete governance model for assessment execution, evidence management, risk evaluation, and reporting.

---

# 49. References

This standard aligns with the principles and practices described in:

* CIS Controls v8
* CIS Benchmarks
* NIST Cybersecurity Framework (CSF)
* NIST SP 800-53
* ISO/IEC 27001:2022
* PCI DSS v4.0
* SOC 2 Trust Services Criteria
* SWIFT Customer Security Programme (CSP)

Organizations should consult the latest published versions of these standards when implementing evidence management processes.

---

# Appendix A – Sample Evidence Register

| Evidence ID      | Module           | Finding  | Type                 | Quality   | Status   |
| ---------------- | ---------------- | -------- | -------------------- | --------- | -------- |
| EVD-MGMT-001-001 | Management Plane | MGMT-001 | CLI Output           | Excellent | Approved |
| EVD-RULE-014-001 | Rule Base        | RULE-014 | Configuration Export | Excellent | Approved |
| EVD-VPN-008-001  | VPN              | VPN-008  | Screenshot           | Good      | Approved |

---

# Appendix B – Sample Chain of Custody Register

| Evidence ID      | Collected By      | Date        | Integrity        | Reviewer           | Status   |
| ---------------- | ----------------- | ----------- | ---------------- | ------------------ | -------- |
| EVD-MGMT-001-001 | Security Assessor | 28-Jun-2026 | SHA-256 Verified | Technical Reviewer | Complete |
| EVD-RULE-014-001 | Security Assessor | 28-Jun-2026 | SHA-256 Verified | QA Reviewer        | Complete |

---

# Appendix C – Evidence Validation Workflow

```text
Evidence Required
        │
        ▼
Evidence Collected
        │
        ▼
Integrity Verification
        │
        ▼
Classification
        │
        ▼
Quality Review
        │
        ▼
Technical Validation
        │
        ▼
Peer Review
        │
        ▼
Referenced in Finding
        │
        ▼
Archived
```

---

# Conclusion

The **Enterprise Evidence Collection and Validation Standard (EFSAF-EVD-001)** establishes a consistent, defensible, and auditable approach for managing evidence throughout the Enterprise Firewall Security Assessment lifecycle. By defining governance, collection methods, validation requirements, integrity controls, traceability, quality assurance, and operational standards, EFSAF ensures that every assessment finding is supported by reliable evidence and can withstand technical review, executive scrutiny, and regulatory audit.

This standard is mandatory for all current and future EFSAF assessment modules and serves as the authoritative reference for evidence management across the framework.

---
