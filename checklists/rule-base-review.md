# Rule Base Security Review (82 Security Checks)

## Rule Governance (7 Checks)
- [ ] Verify every firewall rule has a documented business justification.
- [ ] Verify every firewall rule has an assigned business owner.
- [ ] Verify every firewall rule references an approved change request or ticket.
- [ ] Verify every firewall rule has a defined review or recertification date.
- [ ] Verify firewall rule changes follow the organization's change management process.
- [ ] Verify firewall rules are reviewed after major infrastructure or application changes.
- [ ] Verify policy recertification is performed at least annually.

## Rule Hygience (8 Checks)
- [ ] Verify unused or zero-hit firewall rules are identified and removed after validation.
- [ ] Verify disabled firewall rules are reviewed periodically and removed if no longer required.
- [ ] Verify duplicate firewall rules are identified and eliminated.
- [ ] Verify shadowed or redundant firewall rules are identified and corrected.
- [ ] Verify obsolete firewall rules are removed.
- [ ] Verify temporary or emergency firewall rules have an expiration date and are removed after use.
- [ ] Verify firewall rule hit counts are reviewed periodically.
- [ ] Verify cleanup recommendations are documented and implemented.

## Rule Design & Optimization (8 Checks)
- [ ] Verify firewall policies follow the principle of least privilege.
- [ ] Verify firewall rule order follows the principle of "most specific rules first."
- [ ] Verify firewall rule naming follows organizational standards.
- [ ] Verify policy comments clearly describe the business purpose.
- [ ] Verify duplicate address objects are consolidated.
- [ ] Verify duplicate service objects are consolidated.
- [ ] Verify expired business exceptions are removed.
- [ ] Verify application groups are used where supported.

## Source & Destination Validation (7 Checks)
- [ ] Verify Any-to-Any rules are identified, documented, approved, and minimized.
- [ ] Verify overly broad source address objects are avoided.
- [ ] Verify overly broad destination address objects are avoided.
- [ ] Verify security zones are correctly referenced within firewall policies.
- [ ] Verify inter-zone communication follows the principle of least privilege.
- [ ] Verify address groups are used where appropriate.
- [ ] Verify firewall rules do not expose unauthorized internal networks.

 ## Service & Application Control (8 Checks)
- [ ] Verify overly permissive service definitions (Any Service) are avoided.
- [ ] Verify only required ports and protocols are permitted.
- [ ] Verify application-based policies are used instead of port-based rules where supported.
- [ ] Verify high-risk services (Telnet, FTP, SMB, RDP, SSH, SNMP, LDAP, etc.) are restricted to authorized systems only.
- [ ] Verify risky applications are explicitly controlled.
- [ ] Verify encrypted applications are inspected where organizational policy permits.
- [ ] Verify application overrides are documented and justified.
- [ ] Verify service groups are used where appropriate.

## Access Control & Least Privilege (8 Checks)
- [ ] Verify inbound Internet-to-internal access follows a default-deny approach.
- [ ] Verify outbound Internet access is restricted according to business requirements.
- [ ] Verify public-facing services are limited to approved systems only.
- [ ] Verify inter-zone traffic is explicitly authorized.
- [ ] Verify deny rules exist for unauthorized traffic.
- [ ] Verify Geo-IP restrictions are implemented where business requirements allow.
- [ ] Verify firewall policies do not grant unnecessary administrative access.
- [ ] Verify privileged access follows the principle of least privilege.

## Critical Asset Protection (6 Checks)
- [ ] Verify direct access to critical infrastructure is restricted.
- [ ] Verify Domain Controllers are protected by dedicated security policies.
- [ ] Verify management servers are accessible only from authorized management networks.
- [ ] Verify backup servers are protected by dedicated firewall policies.
- [ ] Verify SIEM and logging infrastructure are protected.
- [ ] Verify administrative services are never directly exposed to the Internet.

## Security Profiles & Inspection (7 Checks)
- [ ] Verify IPS/Threat Prevention profiles are applied where required.
- [ ] Verify Anti-Malware profiles are applied where required.
- [ ] Verify URL Filtering profiles are applied where required.
- [ ] Verify DNS Security profiles are applied where supported.
- [ ] Verify File Blocking policies are configured where required.
- [ ] Verify SSL/TLS Inspection is implemented where appropriate.
- [ ] Verify firewall policies do not bypass security inspection without documented approval.

## Logging & Monitoring (6 Checks)
- [ ] Verify appropriate logging is enabled for all security-relevant firewall rules.
- [ ] Verify critical allow rules are logged.
- [ ] Verify critical deny rules are logged.
- [ ] Verify firewall logs are forwarded to a centralized SIEM or log management platform.
- [ ] Verify firewall log retention complies with organizational requirements.
- [ ] Verify logging configurations are periodically reviewed.

## Object Management (6 Checks)
- [ ] Verify address objects follow organizational naming standards.
- [ ] Verify service objects follow organizational naming standards.
- [ ] Verify object groups are used where appropriate.
- [ ] Verify unused address objects are removed.
- [ ] Verify unused service objects are removed.
- [ ] Verify orphaned objects are identified and removed.

## Policy Exceptions (5 Checks)
- [ ] Verify all firewall policy exceptions are documented.
- [ ] Verify policy exceptions have formal business approval.
- [ ] Verify policy exceptions have an expiration date.
- [ ] Verify policy exceptions are periodically reviewed.
- [ ] Verify expired policy exceptions are removed.

## Compliance & Best Practices (6 Checks)
- [ ] Verify firewall policies comply with organizational security standards.
- [ ] Verify firewall policies align with CIS Benchmarks where applicable.
- [ ] Verify firewall policies support NIST Cybersecurity Framework requirements where applicable.
- [ ] Verify firewall policies support ISO/IEC 27001 security controls where applicable.
- [ ] Verify firewall policies support PCI DSS requirements where applicable.
- [ ] Verify documented deviations are formally approved and risk accepted.
