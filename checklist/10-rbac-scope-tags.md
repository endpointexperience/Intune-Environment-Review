# RBAC & Scope Tags

## Review goal

Review how administrative access is delegated within Intune and whether
administrators have the permissions and visibility they actually need.

The goal is not simply to identify who has access, but to understand how
that access is granted, scoped, and maintained over time.

## Review checklist

- [ ] Review built-in Intune role assignments
- [ ] Review custom Intune RBAC roles
- [ ] Review users and groups assigned to administrative roles
- [ ] Review whether assigned permissions are still required
- [ ] Identify administrators with broader permissions than necessary
- [ ] Review the use of Microsoft Entra roles that provide access to Intune
- [ ] Review Scope Tags and their intended purpose
- [ ] Review which objects are associated with Scope Tags
- [ ] Review Scope Groups used in role assignments
- [ ] Verify that Scope Tags provide the intended administrative visibility
- [ ] Identify unused or obsolete Scope Tags
- [ ] Review administrative access for support and service desk teams
- [ ] Review administrative access for external or temporary administrators
- [ ] Identify role assignments without clear ownership or purpose
- [ ] Review whether administrative responsibilities are documented

## Questions to ask

- Who can currently administer Intune?
- Why does each administrator or administrative group need its assigned permissions?
- Could any administrator perform their role with fewer permissions?
- Are built-in roles being used where appropriate?
- Are custom roles still required and understood?
- Who owns and maintains custom RBAC roles?
- Are Scope Tags being used for a clear administrative purpose?
- Do Scope Tags still reflect the organization's current administrative model?
- Are Scope Groups and Scope Tags configured as intended?
- Can support teams see and manage only the resources required for their role?
- Are there old role assignments for people or teams that no longer require access?
- Is temporary or external administrative access periodically reviewed?
- Is the current RBAC design understandable to someone taking over the environment?

## Things to look for

During the review, pay particular attention to:

- Administrative access that is broader than the person's responsibilities
- Custom roles that closely overlap with built-in roles
- Custom roles that no longer have a clear owner
- Scope Tags without a clear purpose
- Role assignments that no longer appear to be required
- Administrative groups with unclear ownership
- Support teams with permissions beyond their operational requirements
- A complex RBAC design that is difficult to explain or maintain
- Differences between the intended administrative model and the actual configuration

## Review outcome

### 🟢 Good

Administrative access has a clear purpose, permissions reflect actual
responsibilities, and the RBAC and Scope Tag design is understood and
maintained.

### 🟡 Review

The configuration may be valid, but some roles, permissions, Scope Tags,
or assignments should be reviewed or better documented.

### 🔴 Action

Administrative access is unnecessarily broad, obsolete access exists,
or the current RBAC design creates a clear security or operational concern.

## Review notes

Use this section to document findings specific to the environment.

### What works well

- 

### What should be reviewed

- 

### Actions

- 

## Useful Microsoft documentation

- [Role-based access control with Microsoftintune-service/fundamentals/role-based-access-control
- https://learn.microsoft.com/en-us/intune/intune-service/fundamentals/scope-tags

---

The objective isn't to make every Intune environment use the same RBAC
structure.

The objective is to make sure administrative access is intentional,
understood, and appropriate for the responsibilities of each administrator.
