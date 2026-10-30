# Endpoint Security

## Review goal

Review how endpoint security capabilities are configured and managed in Intune.

The goal is to understand whether security policies have a clear purpose,
appropriate assignments, and are still aligned with the organization's
security requirements.

## Review checklist

### Microsoft Defender Antivirus

- [ ] Review Microsoft Defender Antivirus policies
- [ ] Review real-time protection settings
- [ ] Review cloud-delivered protection settings
- [ ] Review potentially unwanted application (PUA) protection
- [ ] Review scheduled and configured scan settings
- [ ] Review antivirus exclusions
- [ ] Review security intelligence update configuration
- [ ] Review policy assignments and exclusions
- [ ] Identify overlapping or conflicting antivirus configurations

### Microsoft Defender Firewall

- [ ] Review Microsoft Defender Firewall policies
- [ ] Review firewall configuration for Domain, Private, and Public profiles
- [ ] Review inbound and outbound firewall rules
- [ ] Review custom firewall rules
- [ ] Review firewall rule assignments
- [ ] Identify rules or exceptions that are no longer required

### Attack Surface Reduction

- [ ] Review Attack Surface Reduction (ASR) rules
- [ ] Review the configured action for each ASR rule
- [ ] Review ASR rule exclusions
- [ ] Review assignment scope and exclusions
- [ ] Identify rules configured in Audit or Warn mode that should be reviewed
- [ ] Review whether ASR configuration is duplicated across different policies

### Disk Encryption

- [ ] Review BitLocker policies
- [ ] Review encryption requirements
- [ ] Review recovery key configuration
- [ ] Review recovery key availability and operational processes
- [ ] Review assignment scope and exclusions
- [ ] Identify devices that are not encrypted as expected

### Account Protection

- [ ] Review Account Protection policies
- [ ] Review Windows Hello for Business configuration
- [ ] Review Windows Local Administrator Password Solution (Windows LAPS) configuration
- [ ] Review local account and local group configuration where applicable
- [ ] Review assignment scope and exclusions
- [ ] Identify overlapping account protection configurations

### Endpoint Detection and Response

- [ ] Review Microsoft Defender for Endpoint integration
- [ ] Review Endpoint Detection and Response (EDR) policies
- [ ] Review onboarding configuration
- [ ] Review assignment scope and exclusions
- [ ] Identify devices that are expected to be onboarded but are not

### General policy review

- [ ] Review ownership of endpoint security policies
- [ ] Review policy naming conventions
- [ ] Review assignments and exclusions
- [ ] Review configuration conflicts
- [ ] Identify duplicate or overlapping security settings
- [ ] Identify policies that no longer appear to be required
- [ ] Review whether exceptions are documented
- [ ] Review whether security configuration changes have a defined process

## Questions to ask

- What security controls are expected to be managed through Intune?
- Who owns the endpoint security configuration?
- Can the purpose of each security policy be explained?
- Are security settings configured in multiple places?
- Are policy assignments intentional and easy to understand?
- Are exclusions documented and periodically reviewed?
- Are antivirus exclusions still required?
- Are firewall exceptions still required?
- Are ASR rules configured according to an intentional strategy?
- Are devices encrypted as expected?
- Is Windows LAPS used for managing local administrator passwords?
- Are devices onboarded to Microsoft Defender for Endpoint as expected?
- Are there security policies that nobody can explain anymore?
- Is there a process for reviewing security settings when Microsoft introduces new capabilities?

## Areas that deserve extra attention

### Exclusions

Security exclusions often deserve additional review.

For each exclusion, consider documenting:

- Why does the exclusion exist?
- Who requested it?
- What systems or users require it?
- Is it still required?
- What is the impact of removing it?

### Overlapping configuration

Similar security settings can sometimes be configured through different
policy types.

When reviewing the environment, identify settings that may be managed through:

- Endpoint Security policies
- Settings Catalog policies
- Security Baselines
- Legacy configuration profiles
- Other management mechanisms

The goal is not necessarily to eliminate every overlap, but to understand
where a setting is managed and why.

### Assignments

A security policy is only useful if it reaches the intended devices or users.

Review:

- Included groups
- Excluded groups
- Assignment filters
- Broad assignments such as All Users or All Devices
- Exceptions that may have accumulated over time

An administrator should be able to explain not only what a security policy
configures, but also why it is assigned to its current scope.

## Review outcome

### 🟢 Good

Security policies have a clear purpose, appropriate assignments, documented
exceptions, and work as intended.

### 🟡 Review

The configuration may be valid, but settings, assignments, exclusions,
ownership, or documentation should be reviewed.

### 🔴 Action

The configuration presents a clear security or operational issue that
requires remediation.

## Notes

Use this section to document observations during the review.

### Findings

- 

### Recommendations

- 

### Follow-up

- 
