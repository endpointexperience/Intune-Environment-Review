# Tenant & Administration

## Review goal

Understand the fundamental configuration of the Intune tenant and verify
that administrative decisions are intentional, documented, and still
relevant.

## Review checklist

- [ ] Review tenant status and connector health
- [ ] Review Intune licensing relevant to the environment
- [ ] Review administrator roles
- [ ] Review role assignments
- [ ] Review custom Intune RBAC roles
- [ ] Review Scope Tags
- [ ] Review enrollment-related tenant settings
- [ ] Review Apple, Android and Windows connectors that are in use
- [ ] Identify configuration that no longer appears to be required

## Questions to ask

- Who is responsible for the Intune environment?
- Who currently has administrative access?
- Are administrative permissions broader than necessary?
- Are custom roles and Scope Tags still required?
- Are connectors actively used and maintained?
- Are important tenant-level decisions documented?
- Is there configuration nobody can explain anymore?

## Review outcome

### 🟢 Good

The configuration has a clear purpose, appropriate ownership and works
as intended.

### 🟡 Review

The configuration may be valid, but its purpose, ownership or documentation
should be reviewed.

### 🔴 Action

The configuration presents a clear issue or requires remediation.
