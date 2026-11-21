# Secure University Portal

**Course:** IT463 — Secure Software Design, Majmaah University.  
**Role:** Team member.  
**Deliverable:** Academic security design and presentation.

## Design goal

Define access to university records through roles and permissions, with server-side authorization for every protected request.

## Design coverage

- Student, Instructor, Administrator and Security Auditor roles.
- Least privilege, ownership checks and separation of duties.
- Authentication versus authorization; MFA as an authentication control.
- Role/permission matrix and centralized authorization flow.
- Threat/control mapping, including privilege escalation, unauthorized access, session hijacking and log tampering.
- Audit logging and proposed append-only records.

## Proposed validation examples

| Scenario | Expected behavior |
| --- | --- |
| Student views own grades | Permit and log |
| Student changes an ID to access another student's grades | Deny |
| Instructor grades an unassigned course | Deny |
| Administrator attempts to alter an audit event | Deny |
| Expired or revoked token is replayed | Deny and require reauthentication |

Source: `SECURE_UNIVERSITY_PORTAL_edited.pdf`. These are designed test scenarios, not execution results. No deployed university system or completed penetration test is claimed.

**Skills:** RBAC, secure design, threat modeling, access-control reasoning and test-case design.

[Project catalogue](README.md)
