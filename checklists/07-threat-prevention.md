# Enterprise Firewall Threat Prevention Review Checklist

## Overview

This checklist evaluates the effectiveness of firewall threat prevention technologies used to detect, inspect, and block malicious network activity.

## Objectives

- Validate threat prevention configuration.
- Reduce malware exposure.
- Verify advanced security inspection.
- Improve attack prevention capabilities.

## Scope

This assessment covers:

- Intrusion Prevention System (IPS)
- Anti-Malware
- Anti-Spyware
- DNS Security
- URL Filtering
- File Blocking
- SSL/TLS Inspection
- Application Identification
- Threat Intelligence
- Security Profile Management

## Standards & References

- CIS Benchmarks
- NIST CSF
- CIS Controls v8
- ISO/IEC 27001
- PCI DSS

## Intended Audience

- Security Engineers
- SOC Analysts
- Security Consultants
- Security Auditors

--- 

# Threat Prevention Review Checklist (76 Security Checks)

## Threat Prevention Governance (5 Checks)
- [ ] Verify threat prevention policies have documented business justification.
- [ ] Verify threat prevention profiles are reviewed periodically.
- [ ] Verify security exceptions are documented and formally approved.
- [ ] Verify temporary security exceptions have an expiration date.
- [ ] Verify threat prevention changes follow change management procedures.

## IPS / Vulnerability Protection (8 Checks)
- [ ] Verify IPS/Vulnerability Protection profiles are enabled.
- [ ] Verify IPS profiles are applied to all applicable security policies.
- [ ] Verify critical and high-severity signatures are configured to block where organizational policy permits.
- [ ] Verify medium and low-severity signatures are configured according to organizational risk appetite.
- [ ] Verify custom IPS signatures are documented and maintained.
- [ ] Verify IPS exceptions are reviewed periodically.
- [ ] Verify IPS signature updates are automatically installed.
- [ ] Verify IPS effectiveness is periodically validated.

## Anti-Malware / Antivirus (6 Checks)
- [ ] Verify Anti-Malware profiles are enabled.
- [ ] Verify Anti-Malware inspection is applied to applicable traffic.
- [ ] Verify malware signature updates are automatic.
- [ ] Verify malware detection actions follow organizational policy.
- [ ] Verify malware exceptions are documented and approved.
- [ ] Verify Anti-Malware effectiveness is periodically reviewed.

## Anti-Spyware & Botnet Protection (7 Checks)
- [ ] Verify Anti-Spyware profiles are enabled.
- [ ] Verify command-and-control (C2) communication is detected and blocked where supported.
- [ ] Verify botnet protection is enabled.
- [ ] Verify DNS-based malware detection is enabled where supported.
- [ ] Verify spyware signature updates are current.
- [ ] Verify outbound malicious communications generate alerts.
- [ ] Verify Anti-Spyware profiles are applied to applicable policies.

## DNS Security (6 Checks)
- [ ] Verify DNS Security profiles are enabled where supported.
- [ ] Verify malicious domains are blocked.
- [ ] Verify newly registered or suspicious domains are monitored according to organizational policy.
- [ ] Verify DNS tunneling detection is enabled where supported.
- [ ] Verify DNS Security updates are automatic.
- [ ] Verify DNS Security events are logged.

## URL Filtering (7 Checks)
- [ ] Verify URL Filtering profiles are enabled.
- [ ] Verify malicious websites are blocked.
- [ ] Verify phishing websites are blocked.
- [ ] Verify high-risk URL categories are restricted according to organizational policy.
- [ ] Verify custom URL categories are documented and maintained.
- [ ] Verify URL Filtering profiles are applied to applicable policies.
- [ ] Verify URL Filtering events are logged.

## File Blocking & Sandboxing (7 Checks)
- [ ] Verify File Blocking profiles are enabled.
- [ ] Verify executable files are restricted according to organizational policy.
- [ ] Verify high-risk file types are controlled.
- [ ] Verify sandbox integration (e.g., WildFire, FortiSandbox, Secure Malware Analytics) is enabled where available.
- [ ] Verify unknown files are submitted for sandbox analysis where supported.
- [ ] Verify sandbox verdicts are enforced.
- [ ] Verify file inspection events are logged.

## SSL/TLS Decryption (6 Checks)
- [ ] Verify SSL/TLS Decryption is enabled where organizational policy permits.
- [ ] Verify inbound and outbound decryption policies are documented.
- [ ] Verify decryption exclusions are documented and approved.
- [ ] Verify expired and untrusted certificates are handled according to organizational policy.
- [ ] Verify weak SSL/TLS protocols are blocked.
- [ ] Verify decryption events are logged.

## Security Profile Management (6 Checks)
- [ ] Verify security profiles follow organizational naming standards.
- [ ] Verify security profiles are consistently applied.
- [ ] Verify unused security profiles are removed.
- [ ] Verify profile changes are documented.
- [ ] Verify profile updates are reviewed periodically.
- [ ] Verify security profiles are backed up with firewall configurations.

## Threat Intelligence & Updates (6 Checks)
- [ ] Verify threat intelligence updates are automatically downloaded.
- [ ] Verify dynamic block lists are updated regularly where supported.
- [ ] Verify signature update failures generate alerts.
- [ ] Verify threat prevention licensing is valid and monitored.
- [ ] Verify security content versions are periodically reviewed.
- [ ] Verify update rollback procedures are documented.

## Logging & Alerting (6 Checks)
- [ ] Verify threat prevention events are logged.
- [ ] Verify high-severity threat detections generate alerts.
- [ ] Verify malware detections are forwarded to the SIEM.
- [ ] Verify IPS detections are forwarded to the SIEM.
- [ ] Verify sandbox verdicts are logged.
- [ ] Verify repeated threat events trigger security notifications.

## Compliance & Best Practices (6 Checks)
- [ ] Verify threat prevention implementation complies with organizational security standards.
- [ ] Verify threat prevention aligns with CIS Benchmarks where applicable.
- [ ] Verify threat prevention supports NIST Cybersecurity Framework requirements where applicable.
- [ ] Verify threat prevention supports ISO/IEC 27001:2022 security controls where applicable.
- [ ] Verify threat prevention supports PCI DSS 4.0 requirements where applicable.
- [ ] Verify documented exceptions are formally approved and periodically reviewed.
