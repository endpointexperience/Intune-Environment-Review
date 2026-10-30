# Device Compliance

## Review goal

Understand how device compliance is used in the environment and verify that
compliance policies reflect the organization's actual requirements for a
trusted device.

The goal is not simply to check whether compliance policies exist, but to
understand what they evaluate, who they apply to, and how noncompliant
devices are handled.

## Review checklist

### Compliance policies

- [ ] Review all existing compliance policies
- [ ] Review which platforms are covered by compliance policies
- [ ] Identify platforms or device types without an intended compliance policy
- [ ] Review settings configured in each compliance policy
- [ ] Identify overlapping or potentially redundant compliance policies
- [ ] Review policy assignments
- [ ] Review exclusions from compliance policies
- [ ] Review whether assignment logic is still relevant
- [ ] Identify old or unused compliance policies

### Compliance settings

- [ ] Review device health requirements
- [ ] Review operating system version requirements
- [ ] Review encryption requirements
- [ ] Review password and authentication requirements where applicable
- [ ] Review security-related requirements such as firewall, antivirus, and antispyware
- [ ] Review whether configured requirements can be reliably evaluated on the targeted devices

### Actions for noncompliance

- [ ] Review actions for noncompliance
- [ ] Review when devices are marked noncompliant
- [ ] Review configured grace periods
- [ ] Review additional actions configured for noncompliant devices
- [ ] Verify that remediation timelines reflect the organization's requirements

### Devices and compliance state

- [ ] Review noncompliant devices
- [ ] Review devices with compliance evaluation errors
- [ ] Review devices that have not recently reported a compliance state
- [ ] Investigate recurring compliance failures
- [ ] Review whether device ownership or management type affects the intended compliance approach

### Conditional Access relationship

- [ ] Identify Conditional Access policies that require compliant devices
- [ ] Understand what access is affected when a device becomes noncompliant
- [ ] Review whether compliance policies and Conditional Access policies support the same security objectives
- [ ] Review exclusions that could affect the expected enforcement
- [ ] Verify that compliance requirements do not create unintended access scenarios

## Questions to ask

- What does "compliant" actually mean in this organization?
- Which device conditions are considered important enough to affect compliance?
- Does every compliance requirement have a clear reason?
- Are all managed platforms covered as intended?
- Are there overlapping policies that make troubleshooting unnecessarily difficult?
- Are exclusions documented and still required?
- What happens when a device becomes noncompliant?
- How much time does a user have to remediate a noncompliant device?
- Does becoming noncompliant affect access through Conditional Access?
- Are compliance failures regularly reviewed?
- Are there compliance settings that nobody can explain anymore?

## Things worth investigating

During a review, pay particular attention to:

- Compliance policies without clear ownership or purpose
- Policies with very broad assignments
- Large or unexplained exclusion groups
- Different policies evaluating the same requirement in different ways
- Long grace periods without a documented reason
- Devices repeatedly switching between compliant and noncompliant
- Compliance requirements that no longer reflect the organization's security requirements
- A disconnect between Intune compliance and Conditional Access enforcement

These findings do not automatically mean that the configuration is wrong.
They are signals that the configuration deserves a closer look.

## Review outcome

### 🟢 Good

The compliance configuration has a clear purpose, policies are intentionally
assigned, requirements reflect current organizational needs, and the impact
of noncompliance is understood.

### 🟡 Review

The configuration may be valid, but there are policies, assignments,
exclusions, requirements, or remediation timelines that should be reviewed
or better documented.

### 🔴 Action

The configuration contains a clear issue that could affect compliance
evaluation, device security, or the organization's intended access controls.

## Notes

Use this section to document observations from the environment review.

### Good

- 

### Review

- 

### Action

- 
