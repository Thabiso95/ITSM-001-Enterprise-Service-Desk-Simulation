KB-002 — Active Directory Account Lockout Troubleshooting

1. Overview

An Active Directory account lockout occurs when an account exceeds the configured threshold for unsuccessful authentication attempts.

Account lockout policies help protect organisational accounts against repeated password-guessing attempts and unauthorised access.

Common causes include:

- Incorrect passwords.
- Outdated credentials stored on devices.
- Background authentication attempts.
- Scheduled tasks or services using old passwords.
- Repeated unsuccessful sign-in attempts.
- Potential malicious authentication activity.

2. Common Symptoms

- User cannot sign in to their workstation.
- Windows reports that the account is locked.
- Microsoft 365 applications repeatedly request credentials.
- Outlook or mobile applications experience authentication issues.
- Account becomes locked again shortly after being unlocked.

3. Initial L1 Investigation

Before taking action:

1. Verify the user's identity according to organisational procedures.
2. Confirm the affected username and device.
3. Establish whether the account is locked or the password is simply incorrect.
4. Ask whether the password was recently changed.
5. Determine whether the user has other devices signed in.
6. Ask whether the problem occurs on multiple devices.
7. Establish whether other colleagues are experiencing similar issues.

4. Basic Troubleshooting

Step 1 — Stop Repeated Sign-in Attempts

Advise the user not to repeatedly enter passwords while the account is locked.

Repeated attempts may prolong the problem or trigger further lockouts.

Step 2 — Investigate Saved Credentials

Check for potentially outdated credentials in:

- Outlook.
- Microsoft Teams.
- Mobile email applications.
- VPN clients.
- Mapped network drives.
- Windows Credential Manager.
- Other applications using the affected account.

Only update or remove credentials using approved organisational procedures.

Step 3 — Confirm Password Synchronisation

If the password was recently changed, establish whether all relevant devices and applications are using the updated credentials.

Step 4 — Test Access

After authorised remediation, ask the user to retry sign-in.

Confirm access to the workstation and relevant applications.

5. Active Directory Administrative Checks

An authorised technician with the required permissions may:

1. Open Active Directory Users and Computers.
2. Locate the affected user account.
3. Review the account's lockout status.
4. Confirm whether an administrative unlock is appropriate.
5. Monitor for recurring lockouts.

Never unlock an account repeatedly without investigating why it continues to become locked.

6. Security Event Investigation

Event ID 4740 — A User Account Was Locked Out

Domain controller Security Event ID 4740 can help identify when an account was locked.

Investigators should review:

- Affected account.
- Event timestamp.
- Caller computer name, where recorded.
- Related authentication events.
- Other available domain controller logs.

The event may help identify the originating computer, but additional investigation may be required to establish the exact cause.

7. Escalation Criteria

Escalate to L2 or the appropriate security team when:

- The account repeatedly locks after being unlocked.
- The source of authentication failures cannot be identified.
- Multiple accounts experience unexpected lockouts.
- There are indications of suspicious authentication activity.
- A service account or business-critical account is affected.
- Administrative permissions are required.

8. Security Considerations

An account lockout is not automatically evidence of an attack.

However, repeated or unusual authentication failures should not be dismissed without investigation.

Look for:

- Unusual login locations.
- Repeated failures across multiple accounts.
- Unexpected authentication sources.
- Password-spraying indicators.
- Unrecognised devices.
- Suspicious activity involving privileged accounts.

Follow organisational incident-response procedures when malicious activity is suspected.

9. Post-Resolution Verification

Before closing the ticket:

1. Confirm the account is accessible.
2. Verify workstation access.
3. Verify relevant Microsoft 365 applications.
4. Confirm whether the lockout has recurred.
5. Record the actions performed.
6. Document confirmed findings separately from suspected causes.
7. Escalate outstanding security concerns.

10. Related Ticket

- AD-001 — Active Directory Account Lockout

11. Keywords

Active Directory, Account Lockout, Event ID 4740, Password Troubleshooting, Windows Authentication, Microsoft 365, Identity and Access Management, Service Desk L1, L2 Escalation