# Lessons Learned

## What I Learned

This lab helped me understand how identity and access management teams manage users, roles, and account lifecycle events.

I practiced creating users, creating roles, assigning access based on job function, reviewing privileged access, simulating a role change, and documenting an account disablement scenario.

## Key Takeaways

- IAM focuses on making sure the right users have the right access at the right time.
- Role-Based Access Control helps simplify access management by assigning permissions through roles instead of individual users.
- Least privilege reduces risk by limiting users to only the access they need.
- Privileged roles, such as `IT_Admin`, require extra review because they create higher security risk.
- Users who change departments should have old access removed before new access is assigned.
- Terminated users should be blocked or disabled quickly to prevent unauthorized access.
- Documentation is important for audits, compliance, and accountability.

## Skills Practiced

- Auth0 dashboard navigation
- User creation
- Role creation
- Role assignment
- Access review documentation
- Joiner-mover-leaver workflow documentation
- Least-privilege access planning
- Privileged access review

## Challenges

One challenge was translating real IAM concepts into a simple lab environment. Auth0 roles were used to simulate department-based access and show how role assignments can support least privilege.

Another challenge was documenting the workflows clearly so that someone reviewing the project could understand the purpose of each user, role, and access decision.

## How This Applies to Security Work

In real organizations, IAM analysts help manage user access, review permissions, process access requests, disable accounts, and reduce unnecessary privileges.

This lab simulates those responsibilities at a beginner level and shows practical understanding of identity lifecycle management.

## Next Improvements

- Add MFA configuration screenshots if available.
- Add Auth0 log screenshots showing login or account events.
- Add a sample access request form.
- Add a sample offboarding checklist.
- Compare Auth0 IAM concepts with Microsoft Entra ID or Okta.
- Create a small web app that uses Auth0 login and role-based page access.