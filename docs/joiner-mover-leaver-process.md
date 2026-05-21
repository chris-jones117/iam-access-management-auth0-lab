# Joiner-Mover-Leaver Process

## Purpose

The joiner-mover-leaver process documents how user access should be handled when employees join the company, change roles, or leave the company.

## Joiner: New Employee

Scenario:

Alice joins the HR department.

Steps:

1. Create the user account.
2. Assign the `HR_ReadOnly` role.
3. Verify role assignment.
4. Document approval and access reason.

Security goal:

Give the new user only the access required for their job function.

## Mover: Role or Department Change

Scenario:

Brian moves from Finance to a Security review role.

Steps:

1. Review current access.
2. Remove the `Finance_User` role.
3. Assign the `Security_Advisor` role.
4. Document the role change.
5. Confirm the user does not keep unnecessary old access.

Security goal:

Prevent permission buildup when users change roles.

## Leaver: Employee Termination

Scenario:

Carla leaves the company.

Steps:

1. Block or disable the user account.
2. Remove active access if required.
3. Document the offboarding action.
4. Review recent login activity if available.

Security goal:

Prevent former users from accessing company systems after termination.

## Why This Matters

Joiner-mover-leaver workflows are important because user access changes over time. Without proper review, users may keep old permissions they no longer need, creating unnecessary security risk.