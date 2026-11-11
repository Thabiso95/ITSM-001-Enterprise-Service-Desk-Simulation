Incident Report — IT-004: Outlook Desktop Authentication Failure

1. Ticket Information

- Ticket ID: IT-004
- Date Logged: 11 November 2026
- Time Logged: 11:20
- Reported By: Sarah Williams
- Department: Human Resources
- Device: Dell Latitude 5420
- Operating System: Windows 11
- Application: Microsoft Outlook Desktop
- Priority: Medium
- Status: Resolved
- Resolution Level: Level 1

2. Incident Description

The employee reported that she could not access her work email through the Microsoft Outlook desktop application. Outlook repeatedly prompted her to sign in, but authentication attempts were unsuccessful.

The employee confirmed that she could access her mailbox through Outlook Web. She had also restarted her workstation, but this did not resolve the issue.

3. Investigation and Findings

During the initial investigation, the employee confirmed that she had changed her Microsoft 365 password the previous day.

Since Outlook Web accepted the updated password while the desktop application continued prompting for authentication, stale credentials or an outdated authentication session were considered a likely contributing factor.

4. Troubleshooting and Resolution

The employee was advised to:

1. Sign out of the Outlook desktop application.
2. Close the application completely.
3. Reopen Outlook.
4. Sign in using the updated Microsoft 365 password.

The employee followed the recommended steps. Outlook accepted the updated credentials and successfully connected to the mailbox.

5. Resolution Verification

The employee confirmed that:

- Outlook desktop successfully connected.
- Existing emails were visible.
- A test email was sent successfully.

A separate inbound-email test was not documented as having been performed.

6. Root Cause Assessment

Likely contributing cause: The password change may have left Outlook desktop using stale authentication credentials or an outdated authentication session.

The exact authentication mechanism was not independently verified.

7. Final Outcome

The employee regained access to Outlook desktop after signing out and authenticating with the updated credentials.

The successful outbound test email provided additional confirmation that the application was functioning.

Final Status: Resolved and closed at Level 1.

Escalation: Not required.