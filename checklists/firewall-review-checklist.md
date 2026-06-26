# Enterprise Firewall Review Checklist

Architecture Review (57 Checks)

# Architecture Review

## Network Architecture
- [ ] Verify firewall placement protects all required network security boundaries.
- [ ] Verify firewall deployment follows defense-in-depth architecture.
- [ ] Verify all inbound and outbound traffic traverses the firewall where required.
- [ ] Verify no unauthorized firewall bypass paths exist.
- [ ] Verify security inspection occurs before traffic reaches critical assets.
- [ ] Verify network choke points are protected by firewall enforcement.
- [ ] Verify firewall deployment aligns with the approved enterprise network architecture.

## Network Segmentation
- [ ] Verify security zones are clearly defined and documented.
- [ ] Verify network segmentation follows business and security requirements.
- [ ] Verify production, development, testing, and management networks are segregated.
- [ ] Verify critical assets are isolated from user and public networks.
- [ ] Verify DMZ architecture is implemented where required.
- [ ] Verify east-west traffic is controlled using security policies.
- [ ] Verify trust relationships between zones follow least privilege.

## Interface Configuration
- [ ] Verify all interfaces are documented.
- [ ] Verify unused interfaces are administratively disabled.
- [ ] Verify interface descriptions are configured.
- [ ] Verify interface IP addressing follows organizational standards.
- [ ] Verify VLAN assignments are correct.
- [ ] Verify sub-interfaces are securely configured.
- [ ] Verify Layer 2 and Layer 3 interface configuration matches the approved design.

## Security Zones
- [ ] Verify every interface belongs to the correct security zone.
- [ ] Verify zone naming follows organizational standards.
- [ ] Verify management interfaces are placed in dedicated management zones.
- [ ] Verify management traffic is isolated from production traffic.
- [ ] Verify unnecessary trust relationships do not exist between security zones.

## High Availability
- [ ] Verify High Availability (HA) is configured where required.
- [ ] Verify HA peers are running the same software version.
- [ ] Verify HA synchronization is healthy.
- [ ] Verify HA heartbeat links are secured.
- [ ] Verify HA failover has been successfully tested.
- [ ] Verify HA failover events generate monitoring alerts.
- [ ] Verify split-brain protection is configured.
- [ ] Verify session synchronization is enabled where supported.

## Routing
- [ ] Verify static routes are documented.
- [ ] Verify dynamic routing authentication is enabled.
- [ ] Verify default routes are appropriate.
- [ ] Verify route redistribution is controlled.
- [ ] Verify asymmetric routing risks have been assessed.
- [ ] Verify routing design minimizes the attack surface.

## Resilience
- [ ] Verify redundant uplinks are configured where required.
- [ ] Verify redundant WAN connectivity is protected by firewall policies.
- [ ] Verify redundant power supplies are operational.
- [ ] Verify critical links are monitored.
- [ ] Verify no single points of failure exist within the firewall deployment.

## Infrastructure Protection
- [ ] Verify firewall management is performed through dedicated administrative jump hosts where required.
- [ ] Verify management interfaces are never directly exposed to the Internet.
- [ ] Verify cloud, on-premises, and hybrid connectivity follow consistent security architecture.
- [ ] Verify DDoS protection is implemented where Internet-facing services require it.


## Documentation
- [ ] Verify architecture diagrams are up to date.
- [ ] Verify firewall inventory is up to date and maintained.
- [ ] Verify network topology is updated and documented.
- [ ] Verify architecture changes are tracked through change management.

## Best Practices
- [ ] Verify management traffic is separated from production traffic.
- [ ] Verify IPv6 architecture has been reviewed where deployed.
- [ ] Verify third-party connectivity is documented and periodically reviewed.
- [ ] Verify firewall architecture is reviewed periodically against enterprise security standards.
- [ ] Verify architecture supports future scalability and business growth requirements.


---

Management Plane Security (61 Security Checks)

# Management Plane Security

## Administrative Access
- [ ] Verify HTTPS is enabled for web-based management.
- [ ] Verify SSH is enabled for CLI management.
- [ ] Verify HTTP is disabled.
- [ ] Verify Telnet is disabled.
- [ ] Verify insecure management protocols are disabled.
- [ ] Verify management access is restricted to approved protocols only.

## Authentication and Authorization
- [ ] Verify Multi-Factor Authentication (MFA) is enabled for all administrative accounts.
- [ ] Verify TACACS+, RADIUS, or LDAP authentication is configured where applicable.
- [ ] Verify Role-Based Access Control (RBAC) is implemented.
- [ ] Verify administrator permissions follow the principle of least privilege.
- [ ] Verify local administrator accounts are limited to emergency use.
- [ ] Verify default or vendor-supplied accounts are disabled or renamed.
- [ ] Verify administrator accounts are individually assigned (shared accounts are prohibited).

## Access Control
- [ ] Verify management access is restricted to authorized management networks.
- [ ] Verify management interfaces are not directly accessible from the Internet.
- [ ] Verify out-of-band management is implemented where required.
- [ ] Verify administrative jump servers are used where required.
- [ ] Verify administrator login banners display authorized use warnings.
- [ ] Verify API access is restricted to authorized systems.

## Password and Account Security
- [ ] Verify password complexity requirements are enforced.
- [ ] Verify password expiration complies with organizational policy.
- [ ] Verify account lockout is configured after repeated failed login attempts.
- [ ] Verify inactive administrator accounts are disabled or removed.
- [ ] Verify privileged account reviews are performed periodically.
- [ ] Verify emergency administrator accounts are documented and monitored.
- [ ] Verify administrator account lifecycle follows joiner, mover, and leaver procedures.

## Management Services
- [ ] Verify only required management services are enabled.
- [ ] Verify unused management services are disabled.
- [ ] Verify SNMPv1 and SNMPv2 are disabled.
- [ ] Verify only SNMPv3 is enabled where SNMP is required.
- [ ] Verify secure NTP is configured using trusted time sources.
- [ ] Verify DNS servers used for management are trusted and documented.

## Session Security
- [ ] Verify administrator sessions automatically timeout after inactivity.
- [ ] Verify concurrent administrator session limits are configured.
- [ ] Verify failed authentication attempts generate security alerts.
- [ ] Verify administrator login notifications are enabled where supported.
- [ ] Verify administrative sessions are encrypted.

## Configuration Security
- [ ] Verify configuration backups are performed regularly.
- [ ] Verify configuration backups are encrypted.
- [ ] Verify backup restoration procedures are tested periodically.
- [ ] Verify configuration changes require formal approval.
- [ ] Verify configuration changes are logged and auditable.
- [ ] Verify firmware and software upgrades follow the organization's change management process.
- [ ] Verify software integrity is validated before installation.

## Logging & Monitoring
- [ ] Verify successful administrator logins are logged.
- [ ] Verify failed administrator login attempts are logged.
- [ ] Verify privilege escalation events are logged.
- [ ] Verify administrator logout events are logged.
- [ ] Verify configuration changes are logged.
- [ ] Verify management logs are forwarded to a centralized SIEM or log management platform.
- [ ] Verify management log retention complies with organizational requirements.

## Certificates & Cryptography
- [ ] Verify management certificates are issued by a trusted Certificate Authority.
- [ ] Verify expired or self-signed certificates are replaced where organizational policy requires.
- [ ] Verify weak SSL/TLS protocols are disabled.
- [ ] Verify strong cryptographic algorithms are used for management access.
- [ ] Verify cryptographic certificates are renewed before expiration.

## Best Practices
- [ ] Verify administrative access is reviewed periodically.
- [ ] Verify management plane security complies with organizational hardening standards.
- [ ] Verify management plane configuration aligns with CIS Benchmarks where applicable.
- [ ] Verify administrative activities are periodically audited.
- [ ] Verify documented exceptions are formally approved and reviewed.

---
Rule Base Security Review (82 Security Checks)
# Rule Base Review

## Rule Governance 
- [ ] Verify every firewall rule has a documented business justification.
- [ ] Verify every firewall rule has an assigned business owner.
- [ ] Verify every firewall rule references an approved change request or ticket.
- [ ] Verify every firewall rule has a defined review or recertification date.
- [ ] Verify firewall rule changes follow the organization's change management process.
- [ ] Verify firewall rules are reviewed after major infrastructure or application changes.
- [ ] Verify policy recertification is performed at least annually.

## Rule Hygience
- [ ] Verify unused or zero-hit firewall rules are identified and removed after validation.
- [ ] Verify disabled firewall rules are reviewed periodically and removed if no longer required.
- [ ] Verify duplicate firewall rules are identified and eliminated.
- [ ] Verify shadowed or redundant firewall rules are identified and corrected.
- [ ] Verify obsolete firewall rules are removed.
- [ ] Verify temporary or emergency firewall rules have an expiration date and are removed after use.
- [ ] Verify firewall rule hit counts are reviewed periodically.
- [ ] Verify cleanup recommendations are documented and implemented.

## Rule Design & Optimization 
- [ ] Verify firewall policies follow the principle of least privilege.
- [ ] Verify firewall rule order follows the principle of "most specific rules first."
- [ ] Verify firewall rule naming follows organizational standards.
- [ ] Verify policy comments clearly describe the business purpose.
- [ ] Verify duplicate address objects are consolidated.
- [ ] Verify duplicate service objects are consolidated.
- [ ] Verify expired business exceptions are removed.
- [ ] Verify application groups are used where supported.

## Source & Destination Validation
- [ ] Verify Any-to-Any rules are identified, documented, approved, and minimized.
- [ ] Verify overly broad source address objects are avoided.
- [ ] Verify overly broad destination address objects are avoided.
- [ ] Verify security zones are correctly referenced within firewall policies.
- [ ] Verify inter-zone communication follows the principle of least privilege.
- [ ] Verify address groups are used where appropriate.
- [ ] Verify firewall rules do not expose unauthorized internal networks.

 ## Service & Application Control
- [ ] Verify overly permissive service definitions (Any Service) are avoided.
- [ ] Verify only required ports and protocols are permitted.
- [ ] Verify application-based policies are used instead of port-based rules where supported.
- [ ] Verify high-risk services (Telnet, FTP, SMB, RDP, SSH, SNMP, LDAP, etc.) are restricted to authorized systems only.
- [ ] Verify risky applications are explicitly controlled.
- [ ] Verify encrypted applications are inspected where organizational policy permits.
- [ ] Verify application overrides are documented and justified.
- [ ] Verify service groups are used where appropriate.

## Access Control & Least Privilege
- [ ] Verify inbound Internet-to-internal access follows a default-deny approach.
- [ ] Verify outbound Internet access is restricted according to business requirements.
- [ ] Verify public-facing services are limited to approved systems only.
- [ ] Verify inter-zone traffic is explicitly authorized.
- [ ] Verify deny rules exist for unauthorized traffic.
- [ ] Verify Geo-IP restrictions are implemented where business requirements allow.
- [ ] Verify firewall policies do not grant unnecessary administrative access.
- [ ] Verify privileged access follows the principle of least privilege.

## Critical Asset Protection
- [ ] Verify direct access to critical infrastructure is restricted.
- [ ] Verify Domain Controllers are protected by dedicated security policies.
- [ ] Verify management servers are accessible only from authorized management networks.
- [ ] Verify backup servers are protected by dedicated firewall policies.
- [ ] Verify SIEM and logging infrastructure are protected.
- [ ] Verify administrative services are never directly exposed to the Internet.

## Security Profiles & Inspection
- [ ] Verify IPS/Threat Prevention profiles are applied where required.
- [ ] Verify Anti-Malware profiles are applied where required.
- [ ] Verify URL Filtering profiles are applied where required.
- [ ] Verify DNS Security profiles are applied where supported.
- [ ] Verify File Blocking policies are configured where required.
- [ ] Verify SSL/TLS Inspection is implemented where appropriate.
- [ ] Verify firewall policies do not bypass security inspection without documented approval.

## Logging & Monitoring
- [ ] Verify appropriate logging is enabled for all security-relevant firewall rules.
- [ ] Verify critical allow rules are logged.
- [ ] Verify critical deny rules are logged.
- [ ] Verify firewall logs are forwarded to a centralized SIEM or log management platform.
- [ ] Verify firewall log retention complies with organizational requirements.
- [ ] Verify logging configurations are periodically reviewed.

## Object Management
- [ ] Verify address objects follow organizational naming standards.
- [ ] Verify service objects follow organizational naming standards.
- [ ] Verify object groups are used where appropriate.
- [ ] Verify unused address objects are removed.
- [ ] Verify unused service objects are removed.
- [ ] Verify orphaned objects are identified and removed.

## Policy Exceptions
- [ ] Verify all firewall policy exceptions are documented.
- [ ] Verify policy exceptions have formal business approval.
- [ ] Verify policy exceptions have an expiration date.
- [ ] Verify policy exceptions are periodically reviewed.
- [ ] Verify expired policy exceptions are removed.

## Compliance & Best Practices
- [ ] Verify firewall policies comply with organizational security standards.
- [ ] Verify firewall policies align with CIS Benchmarks where applicable.
- [ ] Verify firewall policies support NIST Cybersecurity Framework requirements where applicable.
- [ ] Verify firewall policies support ISO/IEC 27001 security controls where applicable.
- [ ] Verify firewall policies support PCI DSS requirements where applicable.
- [ ] Verify documented deviations are formally approved and risk accepted.



NAT Review (56 Checks)

# NAT Review

## NAT Governance
- [ ] Verify every NAT policy has a documented business justification.
- [ ] Verify every NAT policy has an assigned business owner.
- [ ] Verify NAT changes follow the organization's change management process.
- [ ] Verify NAT policies are periodically reviewed and recertified.
- [ ] Verify temporary NAT policies have an expiration date and are removed when no longer required.

## NAT Design
- [ ] Verify NAT is implemented only where required.
- [ ] Verify NAT design follows the principle of least privilege.
- [ ] Verify NAT rule order is correct.
- [ ] Verify bidirectional NAT is implemented only where justified.
- [ ] Verify overlapping NAT policies do not exist.
- [ ] Verify NAT implementation aligns with the approved network architecture.
- [ ] Verify NAT does not bypass established network segmentation.

## Source NAT
- [ ] Verify Source NAT is configured only for approved traffic.
- [ ] Verify Dynamic Source NAT configuration follows business requirements.
- [ ] Verify PAT (Port Address Translation) is used appropriately.
- [ ] Verify Source NAT does not unnecessarily hide user accountability where logging is required.
- [ ] Verify Source NAT policies are documented.

## Destination NAT
- [ ] Verify Destination NAT is configured only for approved services.
- [ ] Verify inbound Destination NAT follows a default-deny approach.
- [ ] Verify public-facing services are limited to authorized systems.
- [ ] Verify Destination NAT does not expose unauthorized internal hosts.
- [ ] Verify inbound published services are protected by appropriate firewall security policies.
- [ ] Verify exposed management services are prohibited unless formally approved.

## Security Validation
- [ ] Verify NAT rules are associated with corresponding security policies.
- [ ] Verify NAT does not bypass IPS, Anti-Malware, or other security inspection.
- [ ] Verify translated traffic is inspected by appropriate security profiles.
- [ ] Verify internal IP addressing is not unnecessarily exposed.
- [ ] Verify critical infrastructure is not published through NAT without formal approval.
- [ ] Verify Internet-facing services are regularly reviewed.
- [ ] Verify NAT policies do not create unintended access paths.

## Rule Hygiene
- [ ] Verify unused NAT policies are removed after validation.
- [ ] Verify disabled NAT policies are periodically reviewed.
- [ ] Verify duplicate NAT policies are eliminated.
- [ ] Verify shadowed or redundant NAT policies are corrected.
- [ ] Verify obsolete NAT policies are removed.
- [ ] Verify NAT policy hit counts are reviewed periodically.

## Object Management
- [ ] Verify NAT address objects follow organizational naming standards.
- [ ] Verify translated address objects are documented.
- [ ] Verify unused translated address objects are removed.
- [ ] Verify public IP allocations are periodically reviewed.
- [ ] Verify NAT policy comments clearly identify business purpose.

## Logging & Monitoring
- [ ] Verify logging is enabled for security-relevant translated sessions.
- [ ] Verify critical NAT events are forwarded to the SIEM.
- [ ] Verify NAT translation failures are monitored.
- [ ] Verify abnormal NAT activity generates security alerts where supported.
- [ ] Verify NAT logs are retained according to organizational policy.

## Documentation
- [ ] Verify public-to-private IP mappings are documented.
- [ ] Verify private-to-public IP mappings are documented.
- [ ] Verify NAT architecture diagrams are current.
- [ ] Verify NAT policy changes are documented.
- [ ] Verify NAT exceptions are formally approved and documented.

## Compliance & Best Practices
- [ ] Verify NAT implementation complies with organizational security standards.
- [ ] Verify NAT implementation aligns with CIS Benchmarks where applicable.
- [ ] Verify NAT implementation supports NIST Cybersecurity Framework requirements where applicable.
- [ ] Verify NAT implementation supports ISO/IEC 27001 security controls where applicable.
- [ ] Verify NAT implementation supports PCI DSS requirements where applicable.
---

VPN Security Review (63 Checks)

# VPN Security
## VPN Governance
- [ ] Verify every VPN connection has a documented business justification.
- [ ] Verify every VPN connection has an assigned business owner.
- [ ] Verify VPN changes follow the organization's change management process.
- [ ] Verify VPN configurations are periodically reviewed and recertified.
- [ ] Verify unused or obsolete VPN tunnels are removed.

## VPN Architecture
- [ ] Verify only approved VPN technologies are deployed.
- [ ] Verify VPN gateways are hardened according to organizational standards.
- [ ] Verify VPN architecture follows the principle of least privilege.
- [ ] Verify backup VPN tunnels are configured where required.
- [ ] Verify VPN routing follows the approved network architecture.
- [ ] Verify Internet-facing VPN gateways are protected by appropriate security controls.

## Cryptography
- [ ] Verify IKEv2 is used where supported.
- [ ] Verify IKEv1 is disabled unless explicitly required for compatibility.
- [ ] Verify strong encryption algorithms (AES-256 or organizationally approved equivalents) are configured.
- [ ] Verify deprecated encryption algorithms are disabled.
- [ ] Verify SHA-1 and other deprecated hashing algorithms are not used unless formally approved.
- [ ] Verify Perfect Forward Secrecy (PFS) is enabled.
- [ ] Verify strong Diffie-Hellman groups are configured.
- [ ] Verify weak ciphers and insecure protocols are disabled.

## Authentication & Authorization
- [ ] Verify Multi-Factor Authentication (MFA) is enabled for remote access VPN users.
- [ ] Verify certificate-based authentication is implemented where applicable.
- [ ] Verify VPN authentication integrates with centralized identity services (LDAP, RADIUS, TACACS+, SAML, etc.) where applicable.
- [ ] Verify VPN user access follows the principle of least privilege.
- [ ] Verify shared VPN accounts are prohibited.
- [ ] Verify disabled user accounts cannot authenticate to the VPN.
- [ ] Verify privileged VPN access requires additional authorization where applicable.

## Remote Access VPN
- [ ] Verify remote VPN users can access only authorized network segments.
- [ ] Verify split tunneling is disabled unless explicitly approved.
- [ ] Verify endpoint posture or compliance validation is enforced where supported.
- [ ] Verify idle session timeout is configured.
- [ ] Verify maximum VPN session lifetime is configured.
- [ ] Verify VPN sessions terminate immediately when user accounts are disabled.
- [ ] Verify remote access VPN configurations are periodically reviewed.

## Site-to-Site VPN
- [ ] Verify peer IP addresses are documented.
- [ ] Verify peer authentication is securely configured.
- [ ] Verify VPN routing permits only authorized networks.
- [ ] Verify encryption domains are correctly defined.
- [ ] Verify unnecessary networks are not advertised through VPN tunnels.
- [ ] Verify redundant site-to-site VPN tunnels are periodically tested.

## Tunnel Security
- [ ] Verify VPN tunnels are continuously monitored.
- [ ] Verify Dead Peer Detection (DPD) or equivalent keepalive mechanisms are enabled where supported.
- [ ] Verify tunnel rekey intervals comply with organizational standards.
- [ ] Verify tunnel failures generate alerts.
- [ ] Verify unauthorized VPN peers are rejected.
- [ ] Verify VPN tunnels do not bypass firewall security inspection without formal approval.

## Certificate Management
- [ ] Verify VPN certificates are issued by a trusted Certificate Authority.
- [ ] Verify VPN certificates are renewed before expiration.
- [ ] Verify certificate revocation checking (CRL or OCSP) is enabled where supported.
- [ ] Verify expired or revoked certificates cannot be used for VPN authentication.
- [ ] Verify private keys associated with VPN certificates are securely protected.

## Logging & Monitoring
- [ ] Verify successful VPN logins are logged.
- [ ] Verify failed VPN authentication attempts are logged.
- [ ] Verify VPN logs are forwarded to the SIEM or centralized log management platform.
- [ ] Verify abnormal VPN login locations generate alerts where supported.
- [ ] Verify impossible-travel VPN events are monitored where supported.
- [ ] Verify repeated failed VPN login attempts generate alerts.
- [ ] Verify VPN log retention complies with organizational policy.

##  Compliance & Best Practices
- [ ] Verify VPN implementation complies with organizational security standards.
- [ ] Verify VPN implementation aligns with CIS Benchmarks where applicable.
- [ ] Verify VPN implementation supports NIST Cybersecurity Framework requirements where applicable.
- [ ] Verify VPN implementation supports ISO/IEC 27001:2022 security controls where applicable.
- [ ] Verify VPN implementation supports PCI DSS 4.0 requirements where applicable.
- [ ] Verify documented VPN exceptions are formally approved and periodically reviewed.


---

Logging & Monitoring Review (60 Checks)
# Logging & Monitoring 
## Logging Configuration (7 Checks)
- [ ] Verify logging is enabled for all security-relevant firewall policies.
- [ ] Verify both successful and denied connections are logged where required.
- [ ] Verify administrator authentication events are logged.
- [ ] Verify administrator logout events are logged.
- [ ] Verify configuration changes are logged.
- [ ] Verify system events are logged.
- [ ] Verify log severity levels are configured according to organizational standards.

## Log Collection (6 Checks)
- [ ] Verify firewall logs are forwarded to a centralized log management platform.
- [ ] Verify log forwarding uses secure protocols where supported.
- [ ] Verify all log types (Traffic, Threat, System, Configuration, Authentication, VPN, NAT) are collected.
- [ ] Verify log forwarding failures generate alerts.
- [ ] Verify redundant log collectors are configured where required.
- [ ] Verify log collection continues during firewall failover where supported.

## Log Integrity & Retention (6 Checks)
- [ ] Verify log retention complies with organizational policy.
- [ ] Verify log retention complies with regulatory requirements.
- [ ] Verify logs are protected against unauthorized modification or deletion.
- [ ] Verify archived logs are securely stored.
- [ ] Verify log integrity validation is implemented where supported.
- [ ] Verify log storage capacity is monitored.

## SIEM Integration (7 Checks)
- [ ] Verify firewall logs are integrated with the organization's SIEM.
- [ ] Verify firewall events are correctly parsed by the SIEM.
- [ ] Verify event normalization is functioning correctly.
- [ ] Verify event correlation rules include firewall events.
- [ ] Verify high-risk firewall events generate security alerts.
- [ ] Verify firewall assets are correctly identified in the SIEM.
- [ ] Verify log ingestion health is continuously monitored.

## Monitoring & Alerting (7 Checks)
- [ ] Verify repeated administrator login failures generate alerts.
- [ ] Verify HA failover events generate alerts.
- [ ] Verify VPN failures generate alerts.
- [ ] Verify threat prevention detections generate alerts.
- [ ] Verify excessive denied traffic generates alerts.
- [ ] Verify excessive configuration changes generate alerts.
- [ ] Verify critical system failures generate alerts.

## Time Synchronization (5 Checks)
- [ ] Verify NTP is configured.
- [ ] Verify trusted NTP servers are used.
- [ ] Verify system time is synchronized across security devices.
- [ ] Verify time synchronization failures generate alerts.
- [ ] Verify log timestamps are accurate and consistent.

## Audit & Compliance (5 Checks)
- [ ] Verify audit logs cannot be disabled by unauthorized users.
- [ ] Verify audit trails support forensic investigations.
- [ ] Verify log review activities are documented.
- [ ] Verify periodic log reviews are performed.
- [ ] Verify logging complies with organizational security standards.

## Operational Monitoring (6 Checks)
- [ ] Verify CPU utilization is monitored.
- [ ] Verify memory utilization is monitored.
- [ ] Verify disk utilization is monitored.
- [ ] Verify interface utilization is monitored.
- [ ] Verify session utilization is monitored.
- [ ] Verify hardware health events are monitored.

## Incident Response Support (5 Checks)
- [ ] Verify logs contain sufficient information for incident investigations.
- [ ] Verify firewall logs support threat hunting activities.
- [ ] Verify critical security events are retained for forensic analysis.
- [ ] Verify incident response teams have access to required firewall logs.
- [ ] Verify firewall logging supports root cause analysis.

## Best Practices (6 Checks)
- [ ] Verify logging and monitoring configurations are periodically reviewed.
- [ ] Verify logging follows the principle of minimum required data loss.
- [ ] Verify logging configurations align with CIS Benchmarks where applicable.
- [ ] Verify logging supports NIST Cybersecurity Framework requirements where applicable.
- [ ] Verify logging supports ISO/IEC 27001:2022 security controls where applicable.
- [ ] Verify logging supports PCI DSS 4.0 requirements where applicable.

Threat Prevention Review (76 Checks)
# Threat Prevention
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
