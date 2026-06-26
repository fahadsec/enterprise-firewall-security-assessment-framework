# Enterprise Firewall Review Checklist

Architecture Review (42 Checks)

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

Management Plane Security (30 Checks)

# Management Plane Security

## Administrative Access

- [ ] Verify HTTPS is enabled.
- [ ] Verify SSH is enabled.
- [ ] Verify Telnet is disabled.
- [ ] Verify HTTP is disabled.
- [ ] Verify insecure management protocols are disabled.

## Authentication

- [ ] Verify MFA is enabled for administrators.
- [ ] Verify TACACS+ or RADIUS authentication is configured.
- [ ] Verify local accounts are limited.
- [ ] Verify default accounts are disabled.
- [ ] Verify RBAC is implemented.

## Access Control

- [ ] Verify management access is restricted to trusted IP addresses.
- [ ] Verify management interface is not Internet accessible.
- [ ] Verify administrative access is limited to management networks.
- [ ] Verify out-of-band management is implemented where possible.
- [ ] Verify administrator login banners are configured.

## Password Security

- [ ] Verify password complexity policy is enforced.
- [ ] Verify password expiration is configured.
- [ ] Verify account lockout policy is enabled.
- [ ] Verify inactive administrator accounts are disabled.
- [ ] Verify shared administrator accounts are avoided.

## Configuration Security

- [ ] Verify configuration backups are scheduled.
- [ ] Verify backups are encrypted.
- [ ] Verify backup restoration has been tested.
- [ ] Verify configuration changes are logged.

## Monitoring

- [ ] Verify administrator login events are logged.
- [ ] Verify failed login attempts are logged.
- [ ] Verify privilege changes are logged.
- [ ] Verify configuration changes are audited.
- [ ] Verify logs are forwarded to SIEM.
- [ ] Verify NTP is configured for accurate timestamps.


---

NAT Review (25 Checks)

# NAT Review

## NAT Design

- [ ] Verify NAT policies have documented business justification.
- [ ] Verify NAT rules follow least privilege.
- [ ] Verify NAT rule order is correct.
- [ ] Verify unnecessary NAT rules are removed.

## Source NAT

- [ ] Verify Source NAT is configured only where required.
- [ ] Verify dynamic NAT configuration is appropriate.
- [ ] Verify PAT usage follows business requirements.
- [ ] Verify source address translation is documented.

## Destination NAT

- [ ] Verify Destination NAT is configured only for approved services.
- [ ] Verify inbound NAT follows default-deny principles.
- [ ] Verify public services are limited to authorized hosts.

## Rule Hygiene

- [ ] Verify unused NAT rules are removed.
- [ ] Verify disabled NAT rules are reviewed.
- [ ] Verify duplicate NAT rules are removed.
- [ ] Verify shadow NAT rules are identified.

## Security

- [ ] Verify NAT rules do not bypass security inspection.
- [ ] Verify security policies exist for translated traffic.
- [ ] Verify logging is enabled for translated sessions.
- [ ] Verify critical systems are not unnecessarily exposed.

## Documentation

- [ ] Verify public IP mappings are documented.
- [ ] Verify private IP mappings are documented.
- [ ] Verify change history is maintained.
- [ ] Verify temporary NAT rules are removed.

## Best Practices

- [ ] Verify bidirectional NAT is used only where required.
- [ ] Verify NAT complies with organizational standards.


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
