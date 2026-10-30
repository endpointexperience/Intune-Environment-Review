# Applications

## Review goal

Understand how applications are packaged, assigned, maintained, and monitored in the Intune environment.

The goal is not only to verify that applications are deployed successfully, but also to understand whether the current application strategy is intentional, maintainable, and easy to troubleshoot.

## Review checklist

### Application inventory

- [ ] Review applications currently managed through Intune
- [ ] Identify applications that are no longer required
- [ ] Identify duplicate or legacy application packages
- [ ] Review which application types are being used
- [ ] Review whether application ownership is clear
- [ ] Identify applications without a clear purpose or owner

### Win32 applications

- [ ] Review Win32 app install and uninstall commands
- [ ] Review detection rules
- [ ] Review requirement rules
- [ ] Review dependencies
- [ ] Review supersedence relationships
- [ ] Verify that uninstall behavior is defined where appropriate
- [ ] Review application packaging standards and consistency
- [ ] Identify old application versions that may still be deployed

### Assignments

- [ ] Review Required application assignments
- [ ] Review Available application assignments
- [ ] Review uninstall assignments
- [ ] Review user versus device targeting
- [ ] Review exclusions
- [ ] Review the use of Assignment Filters
- [ ] Identify applications assigned to unnecessarily broad groups
- [ ] Identify conflicting or difficult-to-understand assignments

### Microsoft 365 Apps

- [ ] Review Microsoft 365 Apps deployment configuration
- [ ] Review update channel strategy
- [ ] Review installed applications and configuration choices
- [ ] Verify that existing deployments still match current requirements

### Microsoft Store apps

- [ ] Review Microsoft Store applications managed through Intune
- [ ] Identify Store applications that are no longer required
- [ ] Review assignments for Store applications

### Application lifecycle

- [ ] Review how new application versions are introduced
- [ ] Review how old versions are removed
- [ ] Review how application updates are handled
- [ ] Identify applications that require manual maintenance
- [ ] Review whether business-critical applications have a clear owner
- [ ] Review whether application retirement is part of the lifecycle
- [ ] Identify applications that have not been reviewed recently

### Monitoring and troubleshooting

- [ ] Review application installation failures
- [ ] Identify applications with recurring deployment issues
- [ ] Review failed or pending installations
- [ ] Review whether detection rules accurately reflect application state
- [ ] Review whether common deployment issues are documented

## Questions to ask

- Why is each application deployed through Intune?
- Who owns and maintains the application?
- How is the application updated?
- How is an old version replaced or removed?
- Are Required and Available assignments intentional?
- Are applications targeted to users or devices for a clear reason?
- Are exclusions still required?
- Could Assignment Filters simplify the targeting strategy?
- Are detection and requirement rules easy to understand?
- Are dependencies and supersedence relationships still relevant?
- Are failed deployments actively reviewed?
- Are there applications in Intune that nobody maintains anymore?

## Things to look out for

Examples of findings that may deserve additional review:

- Multiple packages for different versions of the same application
- Old applications that are still assigned
- Required applications with very broad assignments
- Complex combinations of groups and exclusions
- Detection rules that are difficult to understand or maintain
- Applications without an uninstall strategy
- Dependencies or supersedence relationships that are no longer relevant
- Applications without a clear owner
- Applications that repeatedly fail to install
- Different packaging approaches without a clear reason
- Manual update processes for applications that change frequently

These findings do not automatically mean that the configuration is incorrect. They are indicators that the configuration may deserve a closer look.

## Review outcome

### 🟢 Good

The application has a clear purpose and owner.

Packaging, detection, requirements, assignments, and lifecycle decisions are understood and work as intended.

### 🟡 Review

The application may be working correctly, but parts of its packaging, assignment, ownership, or lifecycle should be reviewed or better documented.

### 🔴 Action

The application configuration presents a clear issue, is no longer required, causes deployment problems, or requires remediation.

## Notes

Use this section to document environment-specific observations.

### Findings

- 

### Recommended actions

- 

### Follow-up

- 
