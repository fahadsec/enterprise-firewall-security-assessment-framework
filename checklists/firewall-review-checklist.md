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

VPN Security Review (30 Checks)

# VPN Security

## VPN Configuration

- [ ] Verify VPN business justification is documented.
- [ ] Verify only approved VPN types are used.
- [ ] Verify VPN gateways are hardened.
- [ ] Verify unnecessary VPN tunnels are removed.

## Cryptography

- [ ] Verify strong encryption algorithms are used.
- [ ] Verify SHA-1 and other deprecated algorithms are not used.
- [ ] Verify Perfect Forward Secrecy (PFS) is enabled.
- [ ] Verify strong Diffie-Hellman groups are configured.
- [ ] Verify weak ciphers are disabled.

## Authentication

- [ ] Verify MFA is enabled for remote access VPN.
- [ ] Verify certificate-based authentication is used where possible.
- [ ] Verify shared credentials are prohibited.
- [ ] Verify VPN user access follows least privilege.

## Tunnel Security

- [ ] Verify split tunneling is disabled unless approved.
- [ ] Verify idle session timeout is configured.
- [ ] Verify VPN session lifetime is limited.
- [ ] Verify tunnel monitoring is enabled.

## Site-to-Site VPN

- [ ] Verify peer IP addresses are documented.
- [ ] Verify peer authentication is secure.
- [ ] Verify routing over VPN is restricted.
- [ ] Verify backup VPN tunnels are tested.

## Monitoring

- [ ] Verify VPN events are logged.
- [ ] Verify failed VPN logins are monitored.
- [ ] Verify VPN logs are forwarded to SIEM.
- [ ] Verify anomalous VPN activity is monitored.

## Best Practices

- [ ] Verify VPN configurations are reviewed periodically.
- [ ] Verify inactive VPN accounts are removed.
- [ ] Verify inactive VPN tunnels are removed.
- [ ] Verify VPN changes follow change management.
- [ ] Verify VPN documentation is current.
- [ ] Verify VPN complies with organizational standards.


---

## Authentication

## Logging

## Threat Prevention

## High Availability

## Best Practices
