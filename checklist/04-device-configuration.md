# Device Configuration

## Review goal

Review how device configuration policies are designed, assigned, and maintained.

The goal is to understand whether the current configuration is intentional,
easy to manage, and still reflects the organization's requirements.

## Review checklist

- [ ] Review existing device configuration policies
- [ ] Review Settings Catalog policies
- [ ] Review older or legacy configuration profiles that may still be in use
- [ ] Review policy naming conventions
- [ ] Identify duplicate or overlapping configuration
- [ ] Review configuration conflicts
- [ ] Review policies with errors or unexpected deployment results
- [ ] Review policy assignments
- [ ] Review assignment exclusions
- [ ] Review the use of Assignment Filters
- [ ] Identify policies with no active assignments
- [ ] Identify policies that may no longer be required
- [ ] Review configuration applied broadly to All Users or All Devices
- [ ] Review custom settings such as OMA-URI configurations
- [ ] Review whether configuration belongs in Device Configuration or another Intune workload
- [ ] Verify that important configuration decisions are documented

## Questions to ask

- What is each policy intended to achieve?
- Can administrators explain why the policy exists?
- Are naming conventions consistent and easy to understand?
- Are multiple policies configuring the same or related settings?
- Are old profiles still required?
- Are any policies producing conflicts or errors?
- Are assignments broader than necessary?
- Are exclusions still required?
- Could Assignment Filters simplify the current assignment design?
- Are there policies without active assignments that can be removed?
- Are custom configurations still required?
- Is there configuration that nobody can explain anymore?
- Is important configuration documented somewhere other than in the Intune portal?

## Things worth investigating

During the review, pay particular attention to:

### Policy overlap

Look for multiple policies that configure the same or related settings.

The existence of multiple policies is not automatically a problem, but the
reason for the design should be understood.

### Legacy configuration

Review older profiles and configurations that may have remained in the
environment as Intune has evolved.

Determine whether they are still needed or whether the configuration should
be redesigned.

### Assignments

A technically correct policy can still create problems when it is assigned
incorrectly.

Review:

- Included groups
- Excluded groups
- All Users and All Devices assignments
- Assignment Filters
- User versus device targeting

Detailed assignment review is also covered in the
[Assignments](09-assignments.md) checklist.

### Configuration conflicts

Investigate conflicts rather than simply accepting them as part of the
environment.

Determine which policies configure the affected setting and whether the
overlap is intentional.

### Custom configuration

Pay extra attention to custom settings and configurations such as OMA-URI.

Ask whether:

- The configuration is still required
- The original reason for implementing it is known
- There is now a more appropriate way to configure the setting
- The configuration has an owner
- The configuration is documented

## Review outcome

### 🟢 Good

Device configuration policies have clear purposes, understandable
assignments, and no unexplained overlap or legacy configuration.

### 🟡 Review

The configuration may work as intended, but some policies, assignments,
conflicts, or older configurations require further investigation or better
documentation.

### 🔴 Action

Configuration has identified issues that require remediation, such as
unintended conflicts, incorrect assignments, obsolete configuration, or
settings that no longer meet the organization.

## Notes

A successful review does not necessarily result in fewer policies.

The goal is to understand the configuration and ensure that every policy has
a reason to exist.

**If you can't explain why a configuration exists, it's worth reviewing.**
