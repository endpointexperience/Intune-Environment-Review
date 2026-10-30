# Security Baselines

## Review goal

Review how security baselines are used in the Intune environment and verify
that deployed settings are intentional, understood, and aligned with the
organization's security requirements.

Security baselines should not simply be deployed and forgotten. Settings,
assignments, exclusions, conflicts, and changes over time should all be part
of the review.

## Review checklist

- [ ] Identify all security baseline profiles currently in use
- [ ] Review which security baseline templates are being used
- [ ] Review profile assignments
- [ ] Review exclusions from baseline assignments
- [ ] Review settings that differ from the baseline defaults
- [ ] Verify that deviations from the baseline are intentional
- [ ] Review settings configured elsewhere in Intune that overlap with baseline settings
- [ ] Review policy conflicts and deployment errors
- [ ] Identify baseline profiles that are no longer required
- [ ] Review whether older baseline profiles should be replaced or updated
- [ ] Verify that baseline changes are tested before broad deployment
- [ ] Review whether exceptions and deviations are documented
- [ ] Verify that the organization understands which security controls are provided by the baseline and which are managed elsewhere

## Questions to ask

- Which security baselines are currently deployed?
- Why was each baseline introduced?
- Which users or devices receive the baseline?
- Are there devices or users excluded from the baseline? Why?
- Have any baseline settings been changed from their default values?
- Can those changes be explained and justified?
- Are the same settings configured in other Intune policies?
- Are there policy conflicts that need to be investigated?
- Are older baseline profiles still required?
- What happens when Microsoft releases an updated baseline?
- How are baseline changes tested before production deployment?
- Are exceptions documented and periodically reviewed?
- Does the current baseline still reflect the organization's security requirements?

## Things to look for

### Unexplained deviations

A setting that differs from the baseline is not automatically a problem.

The important part is understanding why the deviation exists and whether
the reason is still valid.

### Overlapping configuration

Security settings may be configured through multiple policy types.

Review whether baseline settings overlap with settings configured through
Endpoint Security, Settings Catalog, or other configuration policies.

The goal should be to understand which policy is responsible for each
security control and avoid unnecessary configuration complexity.

### Old baseline profiles

Review whether older baseline profiles are still actively required.

Do not assume that a baseline should remain unchanged simply because it has
been deployed successfully for a long time.

### Broad assignments

Review baselines assigned broadly to users or devices.

Make sure exclusions and exceptions are understood and that the targeting
still reflects the intended device population.

### Exceptions without documentation

Exceptions are sometimes necessary.

The concern is not the existence of an exception, but an exception where
nobody can explain why it exists or whether it is still required.

## Review outcome

### 🟢 Good

Security baselines have clear ownership and purpose.

Assignments and exclusions are understood, deviations are intentional,
and potentially overlapping settings are known.

Baseline changes are reviewed and tested before broad deployment.

### 🟡 Review

Security baselines are deployed and generally working, but some settings,
assignments, exclusions, deviations, or overlapping policies require
further review or documentation.

### 🔴 Action

Security baseline configuration contains unexplained settings, significant
policy conflicts, unnecessary or outdated profiles, or exceptions that
cannot be justified.

Configuration should be reviewed and remediated where appropriate.

## Notes

Security baselines should be treated as a starting point for security
configuration rather than a substitute for understanding the individual
settings.

The goal of this review is not to determine whether an environment follows
every baseline setting exactly.

The goal is to understand the configuration, its purpose, and any deliberate
deviations from it.
