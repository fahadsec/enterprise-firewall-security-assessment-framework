# Enterprise Firewall VPN Security Review Checklist

## Overview

This checklist evaluates remote access and site-to-site VPN deployments to ensure secure connectivity, strong authentication, and modern cryptographic protection.

## Objectives

- Validate VPN security.
- Review cryptographic configuration.
- Secure remote access.
- Assess tunnel monitoring.
- Reduce unauthorized access risk.

## Scope

This assessment covers:

- VPN Configuration
- Remote Access VPN
- Site-to-Site VPN
- Cryptography
- Authentication
- Tunnel Security
- VPN Monitoring
- VPN Lifecycle Management

## Standards & References

- CIS Benchmarks
- NIST CSF
- CIS Controls v8
- ISO/IEC 27001
- PCI DSS

## Intended Audience

- Security Engineers
- Firewall Administrators
- Security Consultants
- Security Auditors

---

# VPN Security Review Checklist
### VPN Security Review (63 Security Checks)
## VPN Governance (5 Checks)
- [ ] Verify every VPN connection has a documented business justification.
- [ ] Verify every VPN connection has an assigned business owner.
- [ ] Verify VPN changes follow the organization's change management process.
- [ ] Verify VPN configurations are periodically reviewed and recertified.
- [ ] Verify unused or obsolete VPN tunnels are removed.

## VPN Architecture (6 Checks)
- [ ] Verify only approved VPN technologies are deployed.
- [ ] Verify VPN gateways are hardened according to organizational standards.
- [ ] Verify VPN architecture follows the principle of least privilege.
- [ ] Verify backup VPN tunnels are configured where required.
- [ ] Verify VPN routing follows the approved network architecture.
- [ ] Verify Internet-facing VPN gateways are protected by appropriate security controls.

## Cryptography (8 Checks)
- [ ] Verify IKEv2 is used where supported.
- [ ] Verify IKEv1 is disabled unless explicitly required for compatibility.
- [ ] Verify strong encryption algorithms (AES-256 or organizationally approved equivalents) are configured.
- [ ] Verify deprecated encryption algorithms are disabled.
- [ ] Verify SHA-1 and other deprecated hashing algorithms are not used unless formally approved.
- [ ] Verify Perfect Forward Secrecy (PFS) is enabled.
- [ ] Verify strong Diffie-Hellman groups are configured.
- [ ] Verify weak ciphers and insecure protocols are disabled.

## Authentication & Authorization (7 Checks)
- [ ] Verify Multi-Factor Authentication (MFA) is enabled for remote access VPN users.
- [ ] Verify certificate-based authentication is implemented where applicable.
- [ ] Verify VPN authentication integrates with centralized identity services (LDAP, RADIUS, TACACS+, SAML, etc.) where applicable.
- [ ] Verify VPN user access follows the principle of least privilege.
- [ ] Verify shared VPN accounts are prohibited.
- [ ] Verify disabled user accounts cannot authenticate to the VPN.
- [ ] Verify privileged VPN access requires additional authorization where applicable.

## Remote Access VPN (7 Checks)
- [ ] Verify remote VPN users can access only authorized network segments.
- [ ] Verify split tunneling is disabled unless explicitly approved.
- [ ] Verify endpoint posture or compliance validation is enforced where supported.
- [ ] Verify idle session timeout is configured.
- [ ] Verify maximum VPN session lifetime is configured.
- [ ] Verify VPN sessions terminate immediately when user accounts are disabled.
- [ ] Verify remote access VPN configurations are periodically reviewed.

## Site-to-Site VPN (6 Checks)
- [ ] Verify peer IP addresses are documented.
- [ ] Verify peer authentication is securely configured.
- [ ] Verify VPN routing permits only authorized networks.
- [ ] Verify encryption domains are correctly defined.
- [ ] Verify unnecessary networks are not advertised through VPN tunnels.
- [ ] Verify redundant site-to-site VPN tunnels are periodically tested.

## Tunnel Security (6 Checks)
- [ ] Verify VPN tunnels are continuously monitored.
- [ ] Verify Dead Peer Detection (DPD) or equivalent keepalive mechanisms are enabled where supported.
- [ ] Verify tunnel rekey intervals comply with organizational standards.
- [ ] Verify tunnel failures generate alerts.
- [ ] Verify unauthorized VPN peers are rejected.
- [ ] Verify VPN tunnels do not bypass firewall security inspection without formal approval.

## Certificate Management (5 Checks)
- [ ] Verify VPN certificates are issued by a trusted Certificate Authority.
- [ ] Verify VPN certificates are renewed before expiration.
- [ ] Verify certificate revocation checking (CRL or OCSP) is enabled where supported.
- [ ] Verify expired or revoked certificates cannot be used for VPN authentication.
- [ ] Verify private keys associated with VPN certificates are securely protected.

## Logging & Monitoring (7 Checks)
- [ ] Verify successful VPN logins are logged.
- [ ] Verify failed VPN authentication attempts are logged.
- [ ] Verify VPN logs are forwarded to the SIEM or centralized log management platform.
- [ ] Verify abnormal VPN login locations generate alerts where supported.
- [ ] Verify impossible-travel VPN events are monitored where supported.
- [ ] Verify repeated failed VPN login attempts generate alerts.
- [ ] Verify VPN log retention complies with organizational policy.

##  Compliance & Best Practices (6 Checks)
- [ ] Verify VPN implementation complies with organizational security standards.
- [ ] Verify VPN implementation aligns with CIS Benchmarks where applicable.
- [ ] Verify VPN implementation supports NIST Cybersecurity Framework requirements where applicable.
- [ ] Verify VPN implementation supports ISO/IEC 27001:2022 security controls where applicable.
- [ ] Verify VPN implementation supports PCI DSS 4.0 requirements where applicable.
- [ ] Verify documented VPN exceptions are formally approved and periodically reviewed.


---
