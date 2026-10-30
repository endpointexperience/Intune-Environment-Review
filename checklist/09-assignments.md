# Assignments

## Review goal

Review how policies, applications, scripts, and other Intune configurations
are targeted to users and devices.

The goal is to understand whether the assignment strategy is intentional,
easy to maintain, and possible for another administrator to understand.

Assignments often become more complex as an Intune environment grows.
Groups, exclusions, filters, and exceptions may all be valid, but the
reason behind them should be clear.

## Review checklist

### Assignment strategy

- [ ] Review the overall assignment strategy
- [ ] Identify configurations assigned to All Users
- [ ] Identify configurations assigned to All Devices
- [ ] Review configurations using individual Entra ID groups
- [ ] Review user-based versus device-based assignments
- [ ] Identify inconsistent targeting approaches
- [ ] Review whether the assignment strategy is documented
- [ ] Verify that assignment choices still match the intended purpose

### Groups

- [ ] Review groups used specifically for Intune assignments
- [ ] Identify groups with unclear names or purpose
- [ ] Review dynamic groups used for targeting
- [ ] Review whether assignment groups are still required
- [ ] Identify configurations relying on unnecessarily complex group structures
- [ ] Review group ownership where appropriate

### Assignment filters

- [ ] Identify configurations using Intune Assignment Filters
- [ ] Review the purpose of each filter
- [ ] Review filter rules and targeted device properties
- [ ] Confirm that filters are still required
- [ ] Review whether filters could simplify existing group-based targeting
- [ ] Identify filters with unclear naming or purpose

### Exclusions

- [ ] Review configurations using excluded groups
- [ ] Understand why each exclusion exists
- [ ] Identify permanent exceptions that were originally intended to be temporary
- [ ] Review whether excluded users or devices still require the exception
- [ ] Verify that important exclusions are documented
- [ ] Identify exclusion groups with unclear ownership or purpose

### Conflicting and overlapping assignments

- [ ] Identify policies targeting the same users or devices
- [ ] Review configurations that manage similar settings
- [ ] Review assignments that may create unexpected policy overlap
- [ ] Investigate known configuration conflicts
- [ ] Review applications with overlapping required and available assignments
- [ ] Verify that administrators can determine which configurations apply to a device

### Maintainability

- [ ] Identify assignments that are difficult to explain
- [ ] Identify legacy groups or targeting methods that are no longer required
- [ ] Review naming conventions for assignment groups and filters
- [ ] Review whether exceptions have an owner
- [ ] Review whether temporary assignments have become permanent
- [ ] Identify opportunities to simplify the assignment model

## Questions to ask

When reviewing assignments, ask:

- Why is this configuration assigned to these users or devices?
- Should this target users or devices?
- Could All Users or All Devices be appropriate instead?
- Could an Assignment Filter simplify the targeting?
- Why does this exclusion exist?
- Is the exclusion still required?
- Who owns the exception?
- Is this group used anywhere else?
- Could another administrator understand this assignment without additional context?
- Are multiple configurations targeting the same population?
- Are we using different assignment approaches for similar configurations?
- Is complexity providing real value, or has it simply accumulated over time?

## Things worth investigating

Not everything identified during a review is necessarily a problem.

However, these situations may deserve additional investigation:

### Large numbers of assignment groups

Many dedicated assignment groups can make it difficult to understand what
actually applies to a user or device.

Review whether some targeting could be simplified using broader assignments
and Assignment Filters where appropriate.

### Undocumented exclusions

An exclusion may be completely valid.

The important part is understanding why it exists and whether the reason is
still relevant.

An exclusion that nobody can explain should be reviewed.

### Temporary exceptions

Temporary deployment groups and exclusions have a tendency to remain after
their original purpose has disappeared.

Review whether temporary exceptions are still required.

### Different targeting strategies for similar configurations

If similar policies use completely different assignment approaches, review
whether that complexity is necessary.

Consistency can make the environment easier to operate and troubleshoot.

### Assignment complexity

Complex targeting is not automatically bad.

Sometimes business, security, device, or application requirements require
complex assignments.

The important question is whether the complexity is intentional and
understood.

## Review outcome

### 🟢 Good

The assignment strategy has a clear purpose and administrators can explain
how configurations reach users and devices.

Groups, filters, and exclusions are used intentionally and unnecessary
complexity has been minimized.

### 🟡 Review

The assignments may work as intended, but some targeting decisions,
exceptions, groups, or filters need additional review or documentation.

There may also be opportunities to simplify the assignment model.

### 🔴 Action

Assignments contain clear problems that require attention.

Examples could include unexplained exclusions, obsolete targeting,
unintended assignments, known conflicts, or assignment structures that can
no longer be reliably understood.

## Key takeaway

The goal isn't to have the fewest possible groups, filters, or exclusions.

The goal is to have an assignment model that administrators can understand,
maintain, and explain.

**If nobody can explain why an assignment exists, it deserves a review.**
