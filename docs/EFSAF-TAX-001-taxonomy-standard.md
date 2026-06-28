# EFSAF-TAX-001

# Enterprise Assessment Taxonomy Standard

**Document ID:** EFSAF-TAX-001

**Version:** 1.0

**Status:** Approved

**Classification:** Internal Enterprise Standard

**Framework:** Enterprise Firewall Security Assessment Framework (EFSAF)

---

# Part 1 — Foundation, Governance and Taxonomy Architecture

---

# 1. Purpose

This standard establishes the official enterprise taxonomy used throughout the Enterprise Firewall Security Assessment Framework (EFSAF).

The taxonomy defines a common language, hierarchical structure, identifier model, metadata architecture, and object relationships used by all EFSAF assessment modules, evidence repositories, risk assessments, reporting artifacts, dashboards, automation components, and governance processes.

A standardized taxonomy ensures that assessment outputs remain consistent, traceable, measurable, machine-readable, and scalable across multiple organizations, business units, geographic regions, cloud environments, firewall vendors, and future framework releases.

This document serves as the authoritative reference for all EFSAF naming conventions and classification requirements.

---

# 2. Objectives

The Enterprise Assessment Taxonomy shall:

* Establish a single authoritative classification model.
* Standardize terminology throughout EFSAF.
* Eliminate ambiguity in assessment reporting.
* Improve consistency between assessment teams.
* Enable enterprise-scale reporting.
* Support audit traceability.
* Enable automation.
* Facilitate evidence correlation.
* Support risk aggregation.
* Improve dashboard standardization.
* Enable long-term framework scalability.
* Maintain backward compatibility across framework versions.

---

# 3. Scope

This standard applies to every component of EFSAF including, but not limited to:

* Assessment modules
* Security controls
* Review procedures
* Findings
* Risks
* Recommendations
* Evidence
* Compliance mappings
* Reports
* Metrics
* Dashboards
* Automation workflows
* Assessment repositories
* Version control
* API integrations
* Future EFSAF extensions

The taxonomy shall be used consistently regardless of:

* Firewall vendor
* Deployment model
* Enterprise size
* Industry sector
* Geographic location
* Cloud provider
* Managed service provider
* Assessment methodology

---

# 4. Governance Principles

The taxonomy shall operate according to the following governance principles.

## 4.1 Single Source of Truth

Each taxonomy object shall have only one authoritative definition.

Duplicate terminology shall not exist.

---

## 4.2 Stability

Identifiers shall remain stable throughout the lifecycle of the framework.

Published identifiers shall never be reused.

Deprecated identifiers shall remain reserved.

---

## 4.3 Consistency

Equivalent security concepts shall always use identical terminology across all EFSAF documents.

No module shall define conflicting terminology.

---

## 4.4 Traceability

Every taxonomy object shall support complete lifecycle traceability.

Traceability shall exist between:

* Control
* Assessment
* Evidence
* Finding
* Risk
* Recommendation
* Report
* Compliance mapping

---

## 4.5 Extensibility

The taxonomy shall support future expansion without requiring structural redesign.

New:

* technologies
* firewall vendors
* cloud providers
* security domains
* assessment modules
* compliance frameworks

shall integrate without modifying existing taxonomy objects.

---

## 4.6 Vendor Neutrality

No taxonomy definition shall depend upon vendor-specific terminology.

Vendor-specific terminology shall only appear within implementation guidance.

The core taxonomy shall remain technology independent.

---

# 5. Taxonomy Architecture

EFSAF uses a hierarchical enterprise taxonomy composed of multiple logical layers.

```
Framework

    ↓

Domain

    ↓

Assessment Area

    ↓

Control Family

    ↓

Control

    ↓

Assessment Procedure

    ↓

Evidence

    ↓

Finding

    ↓

Risk

    ↓

Recommendation

    ↓

Report
```

Each layer represents a progressively more detailed level of assessment.

Higher-level objects govern lower-level objects.

Lower-level objects inherit applicable metadata from their parent objects.

---

# 6. Enterprise Taxonomy Layers

## Layer 1 — Framework

Represents the complete Enterprise Firewall Security Assessment Framework.

Example:

EFSAF

---

## Layer 2 — Domain

Represents a major assessment discipline.

Examples include:

* Architecture
* Management
* Policy
* NAT
* VPN
* Logging
* Threat Prevention
* High Availability
* Compliance
* Operations

Domains provide logical separation between enterprise security functions.

---

## Layer 3 — Assessment Area

Represents a focused assessment category inside a domain.

Example:

Management

↓

Administrative Access

↓

Authentication Controls

↓

Role Management

---

## Layer 4 — Control Family

Groups related security controls.

Example:

Administrative Authentication

contains

* MFA
* Password Policy
* Identity Federation
* Account Lockout
* Session Security

---

## Layer 5 — Security Control

Represents an individual security requirement.

Controls are the primary unit of assessment.

Every control shall possess:

* unique identifier
* title
* description
* assessment objective
* evidence requirements
* associated risks
* recommendations
* mappings
* ownership metadata

---

## Layer 6 — Assessment Procedure

Defines the activities required to evaluate a control.

Procedures may include:

* configuration review
* interview
* log analysis
* packet inspection
* evidence validation
* configuration comparison
* command execution
* API verification
* automation validation

---

## Layer 7 — Evidence

Represents supporting artifacts demonstrating the state of a control.

Evidence may include:

* firewall configuration
* screenshots
* API responses
* exported policies
* logs
* packet captures
* management console data
* authentication records
* certificates
* audit reports

Evidence requirements are governed by EFSAF-EVD-001.

---

## Layer 8 — Finding

Represents the outcome of an assessment.

Each finding shall identify:

* assessment result
* affected control
* supporting evidence
* impact
* observations
* root cause
* associated risks

---

## Layer 9 — Risk

Represents the evaluated business and security impact resulting from a finding.

Risk evaluation shall comply with EFSAF-RISK-001.

---

## Layer 10 — Recommendation

Represents the corrective action necessary to remediate a finding.

Recommendations shall be:

* technically accurate
* actionable
* measurable
* prioritized
* risk aligned

---

## Layer 11 — Report

Represents the formal assessment deliverable.

Reports aggregate:

* findings
* risks
* evidence
* recommendations
* compliance mappings
* executive summaries
* technical observations
* assessment metrics

---

# 7. Taxonomy Design Principles

The EFSAF taxonomy shall satisfy the following enterprise design principles.

## Deterministic

Every object shall have one unique classification.

---

## Hierarchical

Objects shall inherit metadata from parent classifications where applicable.

---

## Modular

Individual domains shall evolve independently while maintaining interoperability.

---

## Machine Readable

The taxonomy shall support structured processing by:

* Governance platforms
* SIEM solutions
* GRC platforms
* Reporting engines
* Security orchestration tools
* Automation pipelines
* Future EFSAF APIs

---

## Human Readable

Naming conventions shall remain understandable by:

* Security engineers
* Firewall administrators
* Auditors
* Consultants
* Compliance teams
* Executive stakeholders

---

**End of Part 1**

The next section (**Part 2**) will define the **official EFSAF identifier architecture, naming conventions, metadata schema, object IDs, versioning model, and enterprise classification standards** used consistently across every EFSAF document.


**Part 2 — Identifier Architecture, Naming Conventions and Metadata Standard**

---

# 8. Enterprise Identifier Architecture

## 8.1 Purpose

A standardized identifier architecture shall be used throughout EFSAF to uniquely identify every framework object.

The identifier architecture enables:

* Global uniqueness
* Lifecycle traceability
* Enterprise reporting
* Automation compatibility
* API integration
* Configuration management
* Evidence correlation
* Risk aggregation
* Compliance mapping
* Version control

Each identifier shall remain immutable for the lifetime of the object.

Identifiers shall not contain business-specific, vendor-specific, customer-specific, or environment-specific information.

---

# 8.2 Identifier Design Principles

All identifiers shall satisfy the following principles:

* Globally unique
* Human-readable
* Machine-readable
* Immutable
* Vendor-neutral
* Hierarchical
* Predictable
* Scalable
* Backward compatible
* Automation-friendly

---

# 8.3 Reserved Identifier Prefixes

The following prefixes are reserved for official EFSAF objects.

| Prefix | Object Type          |
| ------ | -------------------- |
| EFSAF  | Framework            |
| DOM    | Assessment Domain    |
| AREA   | Assessment Area      |
| CF     | Control Family       |
| CTRL   | Security Control     |
| PROC   | Assessment Procedure |
| EVD    | Evidence Item        |
| FIND   | Assessment Finding   |
| RISK   | Risk Record          |
| REC    | Recommendation       |
| MAP    | Compliance Mapping   |
| REP    | Assessment Report    |
| MET    | Assessment Metric    |
| TAX    | Taxonomy Object      |
| REF    | Reference Object     |

Additional prefixes may be introduced only through an approved framework revision.

---

# 8.4 Identifier Format

Identifiers shall use the following structure:

`<Object Prefix>-<Domain Code>-<Numeric Identifier>`

Example:

```
CTRL-MGT-001
CTRL-RUL-042
CTRL-VPN-018
PROC-LOG-006
EVD-TP-014
RISK-NAT-003
```

Numeric identifiers shall use fixed three-digit numbering.

Leading zeros shall always be preserved.

---

# 8.5 Domain Codes

Official domain abbreviations shall remain consistent across all framework components.

| Domain               | Code |
| -------------------- | ---- |
| Architecture         | ARC  |
| Management Plane     | MGT  |
| Rule Base            | RUL  |
| NAT                  | NAT  |
| VPN                  | VPN  |
| Logging & Monitoring | LOG  |
| Threat Prevention    | TP   |
| High Availability    | HA   |
| Compliance           | CMP  |
| Operations           | OPS  |
| Cloud Security       | CLD  |
| Identity Integration | IAM  |

New domain codes shall require governance approval.

---

# 8.6 Identifier Lifecycle

Every identifier shall progress through a controlled lifecycle.

States include:

* Draft
* Approved
* Active
* Deprecated
* Retired
* Archived

Identifiers shall never be reassigned.

Deprecated identifiers shall remain permanently reserved.

Retired identifiers shall remain searchable for historical traceability.

---

# 8.7 Version Independence

Object identifiers shall remain independent of document versions.

Example:

```
CTRL-RUL-015
```

The identifier remains unchanged regardless of whether it appears in EFSAF v1.0, v2.0, or future releases.

Version information shall be maintained separately.

---

# 9. Enterprise Naming Standard

## 9.1 General Rules

Names shall be:

* Precise
* Concise
* Unambiguous
* Vendor-neutral
* Security-focused
* Consistent throughout the framework

Names shall describe the security objective rather than a specific implementation.

Example:

Correct:

```
Administrative Multi-Factor Authentication
```

Incorrect:

```
Palo Alto MFA Profile
```

---

## 9.2 Naming Conventions

Object names shall use Title Case.

Examples:

* Administrative Session Management
* Rule Lifecycle Governance
* Logging Integrity Verification
* VPN Cryptographic Configuration

Abbreviations should be avoided unless universally recognized.

---

## 9.3 Terminology Standardization

A single approved term shall be used for each concept.

Examples:

Use:

* Firewall Rule
* Administrative Account
* Security Policy
* Evidence Item
* Risk Rating
* Configuration Baseline

Avoid interchangeable synonyms within official documentation.

---

# 10. Metadata Standard

## 10.1 Purpose

Every taxonomy object shall contain standardized metadata.

Metadata enables:

* Reporting
* Automation
* Filtering
* Search
* Analytics
* Compliance mapping
* Risk correlation
* Governance

---

## 10.2 Mandatory Metadata Attributes

Each taxonomy object shall include, where applicable:

| Attribute                | Requirement                  |
| ------------------------ | ---------------------------- |
| Identifier               | Mandatory                    |
| Name                     | Mandatory                    |
| Description              | Mandatory                    |
| Version                  | Mandatory                    |
| Status                   | Mandatory                    |
| Owner                    | Mandatory                    |
| Domain                   | Mandatory                    |
| Assessment Area          | Mandatory                    |
| Control Family           | Mandatory (where applicable) |
| Criticality              | Mandatory                    |
| Priority                 | Mandatory                    |
| Applicable Technologies  | Mandatory                    |
| Evidence Requirement     | Mandatory                    |
| Risk Reference           | Mandatory                    |
| Recommendation Reference | Mandatory                    |
| Compliance Mapping       | Optional                     |
| Related Objects          | Optional                     |
| Parent Object            | Optional                     |
| Child Objects            | Optional                     |
| Creation Date            | Mandatory                    |
| Last Review Date         | Mandatory                    |

---

# 10.3 Metadata Quality Requirements

Metadata shall be:

* Accurate
* Complete
* Current
* Consistent
* Validated
* Machine-readable
* Auditable

Incomplete metadata shall not be published within an official EFSAF release.

---

# 10.4 Metadata Ownership

Every taxonomy object shall have a designated owner responsible for:

* Accuracy
* Maintenance
* Version updates
* Classification
* Governance compliance
* Change management

Ownership shall be documented within framework governance records.

---

# 11. Classification Attributes

Each object shall support standardized classification attributes.

Examples include:

## Security Criticality

* Critical
* High
* Medium
* Low
* Informational

---

## Assessment Status

* Not Started
* In Progress
* Complete
* Validated
* Exception Approved

---

## Evidence Status

* Requested
* Collected
* Verified
* Rejected
* Expired
* Archived

---

## Control Implementation Status

* Implemented
* Partially Implemented
* Planned
* Not Implemented
* Not Applicable

---

## Review Frequency

* Continuous
* Daily
* Weekly
* Monthly
* Quarterly
* Semi-Annual
* Annual
* Event Driven

---

# 12. Taxonomy Relationships

Taxonomy objects shall maintain explicit parent-child relationships.

Examples include:

```
Framework
    └── Domain
          └── Assessment Area
                └── Control Family
                      └── Security Control
                            └── Assessment Procedure
                                  └── Evidence
                                        └── Finding
                                              └── Risk
                                                    └── Recommendation
```

Relationship integrity shall be preserved across all framework releases.

No child object shall exist without a valid parent relationship unless explicitly designated as a root object.

---

# 13. Validation Requirements

Before publication, every taxonomy object shall be validated to ensure:

* Identifier uniqueness
* Naming standard compliance
* Metadata completeness
* Parent-child relationship integrity
* Version consistency
* Traceability references
* Governance approval
* Classification accuracy

Objects failing validation shall not be incorporated into an official EFSAF release until all deficiencies have been resolved.


**Part 3 — Enterprise Control Hierarchy, Object Relationships and Traceability Standard**

---

# 14. Enterprise Control Hierarchy

## 14.1 Purpose

The EFSAF control hierarchy establishes the authoritative structure used to organize all security assessment controls within the framework.

A standardized hierarchy enables:

* Consistent assessment execution
* Standardized reporting
* Risk aggregation
* Compliance mapping
* Enterprise analytics
* Assessment scalability
* Cross-domain traceability
* Automation compatibility

Every assessment control shall exist within the defined hierarchical model.

---

## 14.2 Hierarchical Structure

The official EFSAF control hierarchy shall follow the structure below.

```text
Framework
    └── Domain
          └── Assessment Area
                └── Control Family
                      └── Security Control
                            └── Assessment Procedure
                                  └── Evidence Requirement
                                        └── Assessment Finding
                                              └── Risk
                                                    └── Recommendation
```

Each hierarchical level inherits governance attributes from its parent while maintaining its own unique metadata.

---

## 14.3 Hierarchy Design Principles

The hierarchy shall satisfy the following principles:

* Single inheritance model
* Logical decomposition
* Non-overlapping control ownership
* Clear parent-child relationships
* Stable organizational structure
* Vendor-neutral representation
* Automation-friendly design
* Audit traceability
* Long-term extensibility

A security control shall belong to one primary Control Family only.

Cross-domain relationships shall be represented through references rather than duplicate control definitions.

---

# 15. Control Family Standard

## 15.1 Purpose

Control Families organize related controls into logical security capabilities.

They provide:

* Consistent organization
* Standardized reporting
* Simplified navigation
* Enterprise metrics
* Governance ownership

---

## 15.2 Control Family Characteristics

Each Control Family shall contain:

* Unique identifier
* Official name
* Business objective
* Security objective
* Scope definition
* Applicable technologies
* Related domains
* Parent Assessment Area
* Associated controls
* Governance owner

---

## 15.3 Example Hierarchy

```text
Domain
    Management Plane

Assessment Area
    Administrative Security

Control Family
    Administrative Authentication

Security Controls
    MFA Enforcement
    Password Policy
    Account Lockout
    Identity Federation
    Session Timeout
```

This structure shall remain consistent throughout all EFSAF modules.

---

# 16. Object Relationship Model

## 16.1 Relationship Principles

Every taxonomy object shall explicitly define its relationship with other objects.

Relationships shall be:

* Documented
* Validated
* Traceable
* Machine-readable
* Non-ambiguous

Implicit relationships shall not be relied upon for governance or automation purposes.

---

## 16.2 Relationship Types

The following relationship types are approved.

| Relationship | Description                           |
| ------------ | ------------------------------------- |
| Parent Of    | Hierarchical ownership                |
| Child Of     | Hierarchical dependency               |
| References   | Logical association                   |
| Depends On   | Operational dependency                |
| Supports     | Functional relationship               |
| Validates    | Evidence verification relationship    |
| Mitigates    | Risk reduction relationship           |
| Maps To      | Compliance or framework mapping       |
| Implements   | Technical implementation relationship |
| Supersedes   | Version replacement relationship      |

Additional relationship types shall require governance approval.

---

## 16.3 Relationship Integrity

Every relationship shall satisfy the following requirements:

* Source object exists
* Target object exists
* Relationship type is valid
* Circular references are prohibited
* Duplicate relationships are prohibited
* Deprecated objects shall not become new parent objects

Relationship validation shall occur during every framework release.

---

# 17. Traceability Framework

## 17.1 Purpose

Traceability ensures that every assessment activity can be followed from governance requirements through technical validation and reporting.

Traceability supports:

* Internal audits
* Regulatory reviews
* Assessment quality assurance
* Evidence validation
* Risk justification
* Executive reporting
* Historical analysis

---

## 17.2 End-to-End Traceability Model

Every assessment shall support complete traceability.

```text
Framework
      ↓
Domain
      ↓
Assessment Area
      ↓
Control Family
      ↓
Security Control
      ↓
Assessment Procedure
      ↓
Evidence
      ↓
Finding
      ↓
Risk
      ↓
Recommendation
      ↓
Report
```

No assessment artifact shall exist outside the traceability chain.

---

## 17.3 Traceability Requirements

Each Security Control shall be traceable to:

* Assessment Domain
* Assessment Area
* Control Family
* Assessment Procedure
* Evidence
* Findings
* Risks
* Recommendations
* Applicable Reports
* Compliance References (where applicable)

Every traceability link shall remain valid throughout the object lifecycle.

---

# 18. Dependency Management

## 18.1 Dependency Principles

Certain controls depend upon the implementation or validation of other controls.

Dependencies shall be documented to ensure:

* Correct assessment sequencing
* Accurate reporting
* Reliable risk analysis
* Automation consistency

---

## 18.2 Dependency Categories

Dependencies may include:

### Functional Dependency

One control requires another control to function correctly.

Example:

Administrative MFA depends upon centralized identity services.

---

### Operational Dependency

Assessment procedures require completion of another procedure.

Example:

Configuration integrity review requires successful configuration export.

---

### Evidence Dependency

One finding requires evidence collected elsewhere.

Example:

Risk validation depends upon verified log evidence.

---

### Compliance Dependency

A regulatory requirement references multiple EFSAF controls.

---

## 18.3 Dependency Rules

Dependencies shall:

* Be explicitly documented
* Be version controlled
* Avoid circular references
* Be validated during framework maintenance

---

# 19. Metadata Inheritance

## 19.1 Purpose

Metadata inheritance reduces duplication while maintaining consistency.

Child objects may inherit selected metadata from parent objects.

Inherited metadata shall remain synchronized unless explicitly overridden.

---

## 19.2 Inheritable Attributes

Examples include:

* Domain
* Assessment Area
* Governance Owner
* Classification
* Version
* Review Frequency
* Applicable Technologies
* Reporting Category

Child-specific attributes shall remain independently managed.

---

## 19.3 Override Rules

Overrides shall only be permitted where justified.

Permitted overrides include:

* Assessment Procedure
* Evidence Requirements
* Implementation Guidance
* Technology Applicability

Core identifiers and governance classifications shall not be overridden.

---

# 20. Cross-Document Linkage Standard

## 20.1 Purpose

EFSAF documents shall maintain formal references to related standards.

Cross-document linkage promotes consistency and eliminates conflicting guidance.

---

## 20.2 Mandatory References

Where applicable, documents shall reference:

* EFSAF-RISK-001 — Enterprise Risk Assessment Methodology
* EFSAF-EVD-001 — Enterprise Evidence Collection and Validation Standard
* Relevant Assessment Modules
* Governance Standards
* Future EFSAF Enterprise Standards

Referenced documents shall be cited using their official document identifiers.

---

# 21. Taxonomy Consistency Controls

To preserve framework integrity, taxonomy objects shall be periodically reviewed to verify:

* Hierarchical consistency
* Relationship accuracy
* Traceability completeness
* Metadata integrity
* Identifier uniqueness
* Dependency validity
* Cross-reference accuracy
* Governance compliance

Non-conforming objects shall be corrected through the formal EFSAF change management process before inclusion in an official framework release.

**Part 4 — Governance, Lifecycle Management, Version Control and Quality Assurance**

---

# 22. Taxonomy Governance

## 22.1 Purpose

The EFSAF taxonomy shall be governed through a formal governance process to ensure long-term consistency, stability, accuracy, and enterprise scalability.

Governance activities shall ensure that all taxonomy objects remain aligned with the strategic objectives of the Enterprise Firewall Security Assessment Framework.

---

## 22.2 Governance Objectives

Taxonomy governance shall:

* Maintain a single authoritative taxonomy.
* Prevent duplicate object definitions.
* Preserve identifier integrity.
* Ensure terminology consistency.
* Govern framework evolution.
* Maintain backward compatibility.
* Support enterprise reporting.
* Enable automation and API integration.
* Protect assessment traceability.
* Improve long-term maintainability.

---

## 22.3 Governance Authority

The designated EFSAF Governance Authority shall be responsible for:

* Taxonomy approval
* Identifier allocation
* Naming convention enforcement
* Metadata governance
* Version approval
* Framework consistency
* Quality assurance oversight
* Change approval
* Release authorization
* Exception management

No taxonomy modification shall become effective without governance approval.

---

# 23. Taxonomy Lifecycle Management

## 23.1 Lifecycle Overview

Every taxonomy object shall progress through a controlled lifecycle.

The lifecycle ensures that changes are managed consistently and remain fully traceable.

---

## 23.2 Lifecycle States

Approved lifecycle states are:

```text
Draft

↓

Under Review

↓

Approved

↓

Published

↓

Active

↓

Deprecated

↓

Retired

↓

Archived
```

Objects shall transition sequentially unless an approved governance exception exists.

---

## 23.3 Draft State

During the Draft state:

* identifiers may be reserved;
* metadata may be incomplete;
* technical review is permitted; and
* publication is prohibited.

Draft objects shall not be referenced by production assessment documentation.

---

## 23.4 Review State

During review, governance shall verify:

* naming compliance;
* identifier uniqueness;
* metadata completeness;
* relationship integrity;
* traceability;
* version accuracy;
* alignment with existing standards.

Objects failing review shall return to the Draft state.

---

## 23.5 Published State

Published taxonomy objects become official framework components.

Published objects shall:

* receive governance approval;
* remain immutable except through formal change control; and
* be available for enterprise assessments.

---

## 23.6 Deprecation

Objects may be deprecated when:

* superseded by improved taxonomy;
* replaced by newer standards;
* no longer applicable;
* consolidated into another object.

Deprecated objects shall remain searchable for historical assessments.

---

## 23.7 Retirement

Retired objects shall no longer be used in new assessments.

Historical references shall remain valid for audit and reporting purposes.

Retired identifiers shall never be reassigned.

---

# 24. Version Control Standard

## 24.1 Purpose

Version control provides a controlled mechanism for managing taxonomy evolution while preserving compatibility across framework releases.

---

## 24.2 Version Format

EFSAF taxonomy versions shall use the following format:

```text
Major.Minor.Revision
```

Examples:

```text
1.0.0

1.1.0

1.2.3

2.0.0
```

---

## 24.3 Major Versions

Major versions shall indicate significant framework changes, including:

* structural redesign;
* governance model changes;
* taxonomy architecture modifications;
* breaking compatibility changes.

---

## 24.4 Minor Versions

Minor versions shall indicate:

* new assessment domains;
* additional controls;
* metadata enhancements;
* reporting improvements;
* non-breaking feature additions.

---

## 24.5 Revision Versions

Revision releases shall include:

* editorial corrections;
* clarification updates;
* formatting improvements;
* reference corrections;
* non-functional documentation updates.

Revision releases shall not modify assessment requirements.

---

# 25. Change Management

## 25.1 Change Control Principles

All taxonomy changes shall be:

* documented;
* reviewed;
* approved;
* version controlled;
* traceable;
* auditable.

Uncontrolled modifications are prohibited.

---

## 25.2 Change Categories

Approved change categories include:

### Corrective Changes

Correction of errors without changing framework intent.

### Adaptive Changes

Support for new technologies, deployment models, or enterprise requirements.

### Preventive Changes

Improvements that reduce future inconsistencies or governance risks.

### Perfective Changes

Enhancements that improve clarity, usability, scalability, or maintainability.

---

## 25.3 Change Records

Each approved change shall include:

* Change Identifier
* Change Description
* Business Justification
* Technical Justification
* Impact Assessment
* Affected Objects
* Approval Authority
* Version Reference
* Approval Date
* Implementation Date

Complete change history shall be permanently retained.

---

# 26. Taxonomy Quality Assurance

## 26.1 Quality Objectives

Quality assurance activities shall verify that taxonomy objects remain:

* complete;
* accurate;
* consistent;
* traceable;
* interoperable;
* maintainable;
* automation-ready.

---

## 26.2 Quality Validation Criteria

Prior to release, each taxonomy object shall be validated for:

* identifier uniqueness;
* naming convention compliance;
* metadata completeness;
* relationship integrity;
* traceability completeness;
* lifecycle status;
* governance approval;
* version consistency;
* documentation quality.

Objects failing validation shall not be published.

---

## 26.3 Periodic Review

The taxonomy shall undergo periodic governance review to verify:

* continued business relevance;
* framework alignment;
* terminology consistency;
* obsolete objects;
* metadata accuracy;
* cross-document consistency;
* enterprise scalability.

Review frequency shall be defined by the EFSAF governance program.

---

# 27. Compliance Enforcement

## 27.1 Mandatory Compliance

All official EFSAF publications shall comply with this taxonomy standard.

Compliance is mandatory for:

* Assessment Modules
* Enterprise Standards
* Assessment Templates
* Evidence Repositories
* Risk Registers
* Reporting Templates
* Automation Components
* Dashboard Definitions
* API Schemas
* Future Framework Extensions

---

## 27.2 Non-Conformance

Non-conformance includes, but is not limited to:

* duplicate identifiers;
* inconsistent terminology;
* missing metadata;
* invalid relationships;
* broken traceability;
* unauthorized object creation;
* uncontrolled version changes;
* undocumented taxonomy modifications.

Non-conforming content shall be corrected before release.

---

## 27.3 Exception Management

Exceptions shall:

* be formally documented;
* include business justification;
* identify associated risks;
* receive governance approval;
* define review and expiration dates.

Exceptions shall not permanently replace established taxonomy requirements.

---

# 28. Records Management

Governance records associated with the taxonomy shall include:

* Version history
* Change logs
* Approval records
* Identifier registry
* Object registry
* Metadata registry
* Relationship registry
* Traceability matrix
* Exception register
* Retirement register
* Audit records

Records shall be retained in accordance with the organization's records retention policy.

---

# 29. Future Compatibility

The EFSAF taxonomy has been designed to support future expansion while preserving compatibility with existing implementations.

Future releases may introduce:

* additional assessment domains;
* new security technologies;
* cloud-native assessment models;
* zero trust assessment controls;
* software-defined networking components;
* AI-assisted assessment capabilities;
* automation extensions;
* machine-readable schema definitions;
* API-based taxonomy services.

Such enhancements shall extend the taxonomy without invalidating previously approved identifiers or governance records.

---

# 30. Summary

The Enterprise Assessment Taxonomy Standard establishes the authoritative classification model for the Enterprise Firewall Security Assessment Framework.

By defining standardized identifiers, naming conventions, metadata requirements, hierarchical structures, object relationships, governance processes, lifecycle controls, and quality assurance requirements, this standard provides the foundation for consistent, repeatable, and scalable enterprise firewall security assessments.

Compliance with this standard ensures that all EFSAF components operate as an integrated framework, enabling accurate traceability, reliable reporting, automation readiness, and long-term maintainability across diverse technologies, organizational structures, and future framework releases.

---

# End of Document

**Document ID:** EFSAF-TAX-001

**Title:** Enterprise Assessment Taxonomy Standard

**Version:** 1.0

**Status:** Approved

**Classification:** Internal Enterprise Standard

**Framework:** Enterprise Firewall Security Assessment Framework (EFSAF)

**Next Enterprise Standard:** **EFSAF-GOV-001 — Enterprise Governance and Framework Management Standard**

