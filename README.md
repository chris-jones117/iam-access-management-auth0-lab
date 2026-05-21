# IAM Access Management Lab with Auth0

## Project Overview

This project demonstrates basic identity and access management concepts using Auth0. The lab simulates a small organization where users are created, roles are assigned, access is reviewed, and common IAM workflows are documented.

The goal of this lab is to practice beginner IAM and cybersecurity concepts such as user provisioning, role-based access control, least privilege, joiner-mover-leaver workflows, privileged access review, and account disablement.

## Tools Used

- Auth0
- Browser-based IAM dashboard
- Role-Based Access Control
- Markdown documentation
- GitHub

## Lab Objectives

- Create simulated users in Auth0
- Create department-based roles
- Assign users to roles based on job function
- Simulate a new hire workflow
- Simulate a role change workflow
- Simulate an offboarding workflow
- Document an access review
- Apply least-privilege principles

## Simulated Organization

Company: CoyoteTech Solutions

Departments:

- HR
- Finance
- IT
- Security
- Sales

## Users Created

| User | Email | Department | Initial Role |
|---|---|---|---|
| Alice HR | `alice.hr@example.com` | HR | `HR_ReadOnly` |
| Brian Finance | `brian.finance@example.com` | Finance | `Finance_User` |
| David IT | `david.it@example.com` | IT | `IT_Admin` |
| Emma Security | `emma.security@example.com` | Security | `Security_Advisor` |
| Carla Sales | `carla.sales@example.com` | Sales | `Sales_User` |

## Roles Created

| Role | Purpose |
|---|---|
| `HR_ReadOnly` | Read-only access for HR resources |
| `Finance_User` | Standard finance department access |
| `IT_Admin` | Administrative IT access |
| `Security_Advisor` | Security review and audit access |
| `Sales_User` | Standard sales department access |

## IAM Workflows Practiced

### New Hire Workflow

Alice HR was created as a new user and assigned the `HR_ReadOnly` role based on department need.

### Mover Workflow

Brian Finance was moved from `Finance_User` access to `Security_Advisor` access to simulate a department or job role change. The old role was removed before assigning the new role to follow least-privilege principles.

### Leaver Workflow

Carla Sales was blocked/disabled to simulate an employee termination and prevent future access.

## Security Concepts Practiced

- Identity and Access Management
- Role-Based Access Control
- Least Privilege
- User Provisioning
- Role Assignment
- Privileged Access Review
- Account Disablement
- Joiner-Mover-Leaver Lifecycle
- Access Review Documentation

## Screenshots

| Screenshot | Description |
|---|---|
| `users-created.png` | Simulated users created in Auth0 |
| `roles-created.png` | Department-based roles created for RBAC |
| `david-user-details.png` | Example user profile for IT/admin user |
| `david-admin-role.png` | IT_Admin role assigned to David |
| `brian-role-change.png` | Mover workflow showing Brian’s role change |
| `carla-blocked.png` | Leaver workflow showing Carla blocked/disabled |

## Key Findings

- Users were assigned access based on job role.
- The `IT_Admin` role represents privileged access and should be reviewed regularly.
- Role changes should include removal of old access before adding new access.
- Blocked or disabled accounts help prevent access after termination.
- Documentation is important for accountability and audit readiness.

## Project Outcome

This lab demonstrates the ability to configure basic IAM workflows, assign roles, review user access, document least-privilege decisions, and simulate common identity lifecycle processes.