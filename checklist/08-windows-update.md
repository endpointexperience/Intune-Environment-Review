# Windows Update

## Review goal

Review how Windows updates are managed across the environment and verify that
the update strategy is intentional, understandable, and aligned with the
organization's requirements.

The goal is not only to review individual policy settings, but also to
understand the overall update strategy and how different update policies
work together.

## Review checklist

### Update strategy

- [ ] Review the overall Windows update strategy
- [ ] Identify which devices are managed through Windows Update for Business
- [ ] Review whether Windows Autopatch is being used
- [ ] Identify devices that may be managed through another update solution
- [ ] Review how production and test devices are separated
- [ ] Verify that the update strategy has clear ownership

### Update rings

- [ ] Review all Update Ring policies
- [ ] Review Update Ring assignments
- [ ] Review deferral settings
- [ ] Review deadline settings
- [ ] Review restart behavior
- [ ] Review active hours configuration
- [ ] Review user experience settings
- [ ] Identify overlapping or unnecessary Update Ring policies
- [ ] Review exclusions from Update Ring policies

### Feature updates

- [ ] Review Feature Update policies
- [ ] Review Feature Update assignments
- [ ] Verify which Windows versions are currently targeted
- [ ] Identify devices not targeted by the expected Feature Update policy
- [ ] Review how new Windows releases are introduced
- [ ] Review whether Feature Update policies align with the intended device lifecycle
- [ ] Review exclusions and exceptions

### Quality updates

- [ ] Review Quality Update policies
- [ ] Review how expedited quality updates are handled
- [ ] Review assignments and exclusions
- [ ] Verify that administrators understand when expedited updates should be used

### Driver updates

- [ ] Review Driver Update policies
- [ ] Review whether driver updates are managed or left to the default update behavior
- [ ] Review Driver Update assignments
- [ ] Review manually approved or declined drivers where applicable
- [ ] Verify that the driver update approach is intentional

### Assignments

- [ ] Review groups used for Windows Update assignments
- [ ] Review exclusions
- [ ] Review the use of assignment filters
- [ ] Identify devices targeted by multiple update policies
- [ ] Verify that pilot and production assignments are easy to understand
- [ ] Review whether old assignment groups are still required

### Monitoring

- [ ] Review Windows Update reporting
- [ ] Identify devices that are behind the expected Windows version
- [ ] Review devices with update failures
- [ ] Review devices that have not completed expected updates
- [ ] Review whether update issues are actively followed up
- [ ] Verify that there is a process for investigating recurring update problems

## Questions to ask

- What is the intended Windows update strategy?
- Which devices receive updates first?
- How are updates validated before broader deployment?
- Can administrators easily explain the difference between pilot and production assignments?
- Which Windows versions should currently exist in the environment?
- How are new Windows feature releases introduced?
- How are urgent security updates handled?
- How are driver updates managed?
- Are there devices intentionally excluded from normal update policies?
- Are those exclusions documented and still required?
- Who is responsible for monitoring update compliance and failures?
- What happens when a device repeatedly fails to update?
- Are there policies or assignment groups that were created for old requirements and are no longer needed?

## Things to look for

During the review, pay particular attention to:

- Policies with unclear ownership or purpose
- Multiple policies targeting the same devices without a clear reason
- Old pilot or deployment groups that are still being used
- Large or unexplained exclusions
- Devices significantly behind the intended Windows version
- Update failures that are not being investigated
- Differences between the documented update strategy and the actual Intune configuration
- Settings that administrators are unable to explain

## Review outcome

### 🟢 Good

The update strategy has a clear purpose, policies and assignments are easy to
understand, and administrators can explain how updates move through the
environment.

### 🟡 Review

The configuration may be working, but parts of the update strategy, policy
structure, assignments, exclusions, or documentation should be reviewed.

### 🔴 Action

The update configuration presents a clear issue, devices are not receiving
updates as intended, or the current configuration requires remediation.

## Notes

Windows update requirements vary between organizations.

Avoid treating individual settings as universally correct or incorrect without
understanding the organization's requirements, device population, operational
processes, and risk tolerance.

The purpose of this review is to understand whether the current configuration
is intentional and whether it achieves the organization's intended update
strategy.
