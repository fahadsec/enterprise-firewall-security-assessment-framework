# Enterprise Firewall Review Checklist

## Architecture Review
- [ ] High Availability (HA) configured and operational
- [ ] Management interface isolated from untrusted networks
- [ ] Security zones properly defined
- [ ] Zone-to-zone traffic follows least privilege
- [ ] Routing configuration reviewed
- [ ] Network segmentation implemented
- [ ] Internet-facing interfaces identified
- [ ] Administrative access restricted

## Management Plane Security
- [ ] HTTPS enabled for management
- [ ] SSH access restricted
- [ ] Telnet disabled
- [ ] Default accounts removed or disabled
- [ ] MFA enabled for administrators
- [ ] TACACS+/RADIUS configured
- [ ] Role-Based Access Control (RBAC) implemented
- [ ] Management access allowed only from trusted IPs
- [ ] Password policy reviewed
- [ ] Configuration backup enabled

## Rule Base Review
- [ ] Any-to-Any rules identified
- [ ] Unused rules identified
- [ ] Disabled rules reviewed
- [ ] Shadowed rules identified
- [ ] Duplicate rules identified
- [ ] Temporary rules reviewed
- [ ] Rule naming standards followed
- [ ] Business justification available
- [ ] Rule hit counts reviewed
- [ ] Cleanup recommendations documented

## NAT

## VPN

## Authentication

## Logging

## Threat Prevention

## High Availability

## Best Practices
