AD-001 — Active Directory Account Lockout

1. Ticket Information

Field| Details
Ticket ID| AD-001
Category| Identity and Access Management
Priority| High
Status| Resolved
Support Level| Level 1
User| Sarah Mokoena
Department| Accounts
Operating System| Windows 11
Issue Type| Account Lockout

2. Incident Description

Sarah Mokoena reported that she could no longer sign in to her Windows workstation because her account appeared to be locked.

During the initial investigation, the user confirmed that she had changed her password the previous day.

She also reported that Outlook and Microsoft Teams remained signed in on her mobile device.

These details raised the possibility that an application or device was still attempting to authenticate using outdated credentials.

3. Business Impact

- User could not access her workstation.
- Access to normal work activities was disrupted.
- Potential interruption to Accounts Department operations.
- Repeated authentication attempts could cause further account lockouts.

4. Initial Investigation

The L1 technician:

1. Confirmed the affected user's identity.
2. Established that the account was experiencing a lockout.
3. Asked whether the password had recently been changed.
4. Established that the password had been changed the previous day.
5. Identified that Outlook and Teams remained signed in on the user's mobile device.

5. Troubleshooting Performed

The investigation focused on identifying whether an application or device was continuing to use outdated authentication credentials.

The user was advised to address potentially stale credentials on the mobile device.

Sarah updated the credentials associated with Outlook mobile.

Following this action, she successfully accessed Outlook and her Windows workstation.

6. Technical Findings

Confirmed observations:

- The account was inaccessible during the incident.
- The user had changed her password the previous day.
- Outlook and Teams remained signed in on her mobile device.
- Updating Outlook mobile credentials was followed by successful access to Outlook and the workstation.

Suspected contributing factor:

Outdated credentials associated with the mobile Outlook application may have contributed to repeated authentication failures.

Not conclusively established:

The original source of the account lockout was not verified through domain controller security logs.

7. Resolution

The user updated Outlook mobile credentials and subsequently regained access to Outlook and the Windows workstation.

The immediate access issue was resolved.

8. Recommended Verification

For a complete enterprise investigation, an authorised technician should:

- Confirm the account is no longer locked in Active Directory.
- Review domain controller Security Event ID 4740.
- Identify the source workstation or device associated with the lockout, where recorded.
- Check for other applications or services using outdated credentials.
- Confirm that no further lockouts occur.

9. Final Status

Status: Resolved — User access restored.

Suspected contributing factor: Potential stale credentials on the mobile device.

Root cause: Not conclusively established.

10. Skills Demonstrated

- Active Directory fundamentals.
- Account lockout troubleshooting.
- Identity and access management.
- Microsoft 365 support.
- User communication.
- Authentication troubleshooting.
- Incident documentation.
- Evidence-based reporting.