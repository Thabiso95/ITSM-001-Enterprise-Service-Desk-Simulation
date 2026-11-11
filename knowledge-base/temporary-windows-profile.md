KB-001 — Troubleshooting a Temporary Windows Profile

1. Overview

A temporary Windows profile may load when Windows cannot access or initialise a user's normal profile during sign-in.

When this happens, the user may see an unfamiliar desktop, missing personal settings or apparently unavailable desktop files.

A temporary profile should not be treated as evidence that the original user data has been deleted.

2. Common Symptoms

- Windows displays a temporary profile notification.
- Desktop layout and settings appear different.
- Previously available desktop files are missing.
- Applications may not retain user-specific settings.
- The issue may persist across multiple sign-in attempts.

3. Initial L1 Checks

Before attempting remediation:

1. Confirm the affected user's identity.
2. Confirm the workstation and Windows version.
3. Establish when the problem started.
4. Ask whether the user recently restarted the device or installed updates.
5. Confirm whether Windows displayed a temporary profile notification.
6. Determine whether important work is currently unsaved.
7. Advise the user to avoid saving important files in the temporary profile.

4. Basic Troubleshooting

If there is no unsaved work:

1. Ask the user to save or safely close any open applications.
2. Perform a controlled sign-out.
3. Allow Windows to return to the sign-in screen.
4. Ask the user to sign in again.
5. Confirm whether the normal profile loads.

If the temporary profile persists, stop basic troubleshooting and consider escalation.

5. Advanced Diagnostics

The following checks may be performed by authorised technicians with appropriate permissions.

Event Viewer

1. Open Event Viewer.
2. Navigate to Windows Logs.
3. Select Application.
4. Review events associated with User Profile Service.
5. Check relevant timestamps and error descriptions.

Relevant Event IDs

Event ID| Investigation relevance
1511| Windows logged the user on with a temporary profile
1515| Windows backed up the user profile

These events provide useful investigation leads. They should be interpreted alongside surrounding events and other available evidence.

6. Escalation Criteria

Escalate to L2 support when:

- The temporary profile persists after a controlled sign-out and sign-in.
- The original profile appears damaged or inaccessible.
- User data may be at risk.
- Advanced profile diagnostics or registry investigation are required.
- The technician lacks the permissions needed for safe remediation.

7. Actions to Avoid

Unless authorised and supported by an appropriate recovery plan:

- Do not delete the user's original profile directory.
- Do not make unverified registry modifications.
- Do not overwrite the original profile.
- Do not assume missing desktop files have been permanently deleted.
- Do not attempt backup restoration without assessing the existing data.

8. Post-Resolution Verification

After remediation:

1. Confirm the user can sign in normally.
2. Verify that the correct desktop profile loads.
3. Confirm expected desktop files and settings are available.
4. Ask the user to test relevant applications.
5. Confirm that the temporary profile notification no longer appears.
6. Document the remediation and user confirmation in the ticket.

9. Related Ticket

- IT-001 — Temporary Windows Profile

10. Keywords

Windows 11, Temporary Profile, User Profile Service, Event Viewer, Desktop Support, L1 Troubleshooting, L2 Escalation