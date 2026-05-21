# Access Review

## Purpose

This access review checks whether each simulated user has access that matches their department and job function.

## Access Review Table

| User | Department | Current Role | Risk Level | Review Decision |
|---|---|---|---|---|
| Alice HR | HR | `HR_ReadOnly` | Low | Keep access |
| Brian Finance | Finance → Security | `Security_Advisor` | Medium | Removed `Finance_User` and assigned `Security_Advisor` |
| David IT | IT | `IT_Admin` | Medium | Verify admin approval due to privileged access |
| Emma Security | Security | `Security_Advisor` | Low | Keep access |
| Carla Sales | Sales | `Sales_User` | High | Blocked account due to termination scenario |

## Findings

- Alice HR has appropriate read-only access for an HR user.
- Brian Finance had a role change and should no longer keep old Finance access.
- David IT has privileged access through the `IT_Admin` role and should be reviewed regularly.
- Emma Security has appropriate security review access.
- Carla Sales represents a terminated user and should be blocked or disabled immediately.

## Recommendations

- Review privileged accounts monthly.
- Remove old roles when users change departments.
- Block or disable terminated users immediately.
- Require MFA for privileged accounts when available.
- Use role-based access instead of assigning permissions individually.
- Document access approvals and role changes.