AD-001 — Troubleshooting Log

Ticket Reference

Field| Details
Ticket ID| AD-001
User| Sarah Mokoena
Department| Accounts
Priority| High
Support Level| L1
Issue| Active Directory Account Lockout

Troubleshooting Timeline

Step| Action| Observation / Result
1| Received user report| User unable to sign in to workstation
2| Confirmed account issue| Account reported as locked
3| Asked about recent password changes| User confirmed password changed the previous day
4| Investigated other signed-in devices| Outlook and Teams remained signed in on mobile
5| Identified possible stale credentials| Mobile application authentication required investigation
6| Guided user through credential update| User updated Outlook mobile credentials
7| Tested access| User successfully accessed Outlook
8| Confirmed workstation access| User successfully accessed Windows workstation
9| Assessed incident status| Immediate access issue resolved

Technical Assessment

The recent password change and continued mobile application sessions suggested that outdated credentials may have contributed to the lockout.

Updating Outlook mobile credentials was followed by successful access.

However, the original lockout source was not conclusively identified.

Additional Verification Recommended

For a complete investigation, an authorised technician should:

1. Verify the account's current lockout status in Active Directory.
2. Review domain controller Security Event ID 4740.
3. Identify the reported caller computer or lockout source, where available.
4. Check other devices and applications for outdated credentials.
5. Monitor for additional failed authentication attempts.
6. Confirm that the account remains accessible.

Actions Not Confirmed

The following actions were not performed or verified during this simulation:

- Direct Active Directory administrative unlock.
- Review of domain controller Event ID 4740.
- Identification of the precise originating device.
- Review of all other authentication sources.

Final Result

Immediate issue: Resolved.

User access: Restored.

Suspected contributing factor: Potential stale credentials in mobile Outlook.

Confirmed root cause: Not established.

Further investigation: Recommended if the account experiences another lockout.

---

Technician Notes

The successful restoration of access should not be confused with confirmation of the underlying root cause.

Accurate documentation must distinguish between confirmed observations, suspected causes and recommended follow-up actions.