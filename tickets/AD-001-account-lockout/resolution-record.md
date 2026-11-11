AD-001 — Resolution Record

1. Ticket Information

Field| Details
Ticket ID| AD-001
Category| Identity and Access Management
Priority| High
User| Sarah Mokoena
Department| Accounts
Support Level| L1
Final Status| Resolved
Resolution Type| User access restored

2. Reported Issue

The user was unable to access her Windows workstation because her account was locked.

The user confirmed that she had changed her password the previous day and still had Outlook and Microsoft Teams signed in on her mobile device.

3. Resolution Actions

1. Investigated the recent password change.
2. Identified potentially outdated credentials on the mobile device as a possible contributing factor.
3. Guided the user through updating Outlook mobile credentials.
4. Asked the user to retry access.
5. Confirmed successful Outlook access.
6. Confirmed successful Windows workstation access.

4. Resolution Verification

Verification| Result
Outlook mobile access| Successful
Windows workstation access| Successful
Immediate access issue| Resolved
Active Directory lockout status independently verified| Not confirmed
Original lockout source identified| Not confirmed

5. Root Cause Assessment

Suspected contributing factor: Outdated authentication credentials associated with the mobile Outlook application.

Root cause: Not conclusively established.

The successful restoration of access after updating Outlook credentials supports this as a possible contributing factor, but does not independently prove it caused the original lockout.

6. Preventive Recommendations

- Update saved credentials after changing an account password.
- Check mobile devices and applications for outdated authentication sessions.
- Avoid repeatedly attempting to sign in when an account is locked.
- Escalate recurring lockouts for investigation.
- Review domain controller Event ID 4740 when investigating the source of account lockouts.

7. Closure Notes

The user confirmed successful access to Outlook and the Windows workstation.

The immediate business impact was resolved, and the incident was marked as resolved.

If the account becomes locked again, further investigation should identify the originating device or authentication source before attributing the cause.

8. Final Outcome

Ticket status: Resolved.

User access: Restored.

Root cause: Unconfirmed.

Outstanding action: None required for immediate access restoration. Further investigation recommended if the issue recurs.