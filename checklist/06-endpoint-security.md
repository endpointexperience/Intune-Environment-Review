# Endpoint Security

## Review goal

Review the endpoint security configuration to understand how devices are
protected, identify configuration gaps or overlaps, and verify that security
settings reflect the organization's current requirements.

## Review checklist

### Microsoft Defender Antivirus

- [ ] Review Microsoft Defender Antivirus configuration
- [ ] Review real-time protection settings
- [ ] Review cloud-delivered protection settings
- [ ] Review potentially unwanted application (PUA) protection
- [ ] Review configured antivirus exclusions
- [ ] Review scheduled and on-demand scan configuration

### Microsoft Defender Firewall

- [ ] Review firewall configuration for Domain, Private, and Public profiles
- [ ] Review inbound and outbound firewall rules
- [ ] Review firewall exclusions and exceptions
- [ ] Identify legacy or duplicate firewall configurations

### Disk Encryption

- [ ] Review BitLocker policies
- [ ] Review encryption method configuration
- [ ] Review recovery key configuration and availability
- [ ] Review silent encryption configuration
- [ ] Identify devices that are not encrypted as expected

### Attack Surface Reduction

- [ ] Review configured Attack Surface Reduction rules
- [ ] Review rule modes such as Audit, Warn, and Block
- [ ] Review ASR exclusions
- [ ] Identify rules that remain in Audit mode without a documented reason
- [ ] Review whether rule configuration still reflects current requirements

### Account Protection

- [ ] Review account protection policies
- [ ] Review Windows Hello for Business configuration
- [ ] Review Windows LAPS configuration
- [ ] Review local administrator management
- [ ] Review membership of local security groups where applicable

## Questions to ask

- Is there a clear endpoint security strategy?
- Are security settings managed consistently?
- Are there overlapping policies configuring the same settings?
- Are exclusions documented and still required?
- Can administrators explain why specific security controls are configured?
- Are settings left in Audit mode intentionally?
- Are legacy policies still targeting devices?
- Are security policies assigned to the intended users or devices?

## Review outcome

### 🟢 Good

Security controls have a clear purpose, are appropriately assigned, and
work as intended.

### 🟡 Review

The configuration may be valid, but its purpose, assignment, exclusions,
or documentation should be reviewed.

### 🔴 Action

The configuration presents a security concern or requires remediation.
