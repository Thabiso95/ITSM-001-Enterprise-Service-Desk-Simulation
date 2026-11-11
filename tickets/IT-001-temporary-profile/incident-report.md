IT-001 — Temporary Windows Profile

1. Ticket Information

Field| Details
Ticket ID| IT-001
Category| Windows Support
Priority| High
Status| Escalated to Level 2
Support Level| Level 1
User| J. Rivera
Department| Accounts Payable
Operating System| Windows 11
Device| Dell OptiPlex 7090
Issue Type| User Profile / Login

2. Incident Description

The user reported that after restarting their workstation, Windows loaded a desktop that appeared unfamiliar. Previously available desktop files and settings appeared to be missing.

During initial communication, the user confirmed that Windows displayed a notification indicating that they had signed in using a temporary profile.

The incident raised concerns about access to the user's normal desktop environment and locally stored files.

3. Business Impact

- User could not access their normal desktop environment.
- Previously available desktop files and settings appeared unavailable.
- Normal work activities were potentially disrupted.
- Risk of data loss or additional changes if the temporary profile was used.

4. Initial Investigation

The L1 technician:

1. Confirmed the user's identity and affected workstation.
2. Asked whether the issue started after a restart.
3. Established that Windows had displayed a temporary profile notification.
4. Confirmed that the normal desktop environment had not loaded.
5. Advised the user to avoid saving important work in the temporary profile.

5. Troubleshooting Performed

A controlled sign-out and sign-in was performed after checking for unsaved work.

The user continued to experience the temporary profile issue after signing in again.

The persistence of the problem indicated that basic sign-in recovery had not resolved the incident.

Further investigation was required.

6. Technical Findings

The following checks were identified for further investigation by the appropriate support level:

- Windows Event Viewer.
- Windows Logs → Application.
- User Profile Service events.
- Event ID 1511: Windows logged the user on with a temporary profile.
- Event ID 1515: Windows backed up the user profile.

These event IDs are investigation leads, not confirmed findings from this simulation.

7. Resolution and Escalation

Final L1 outcome: Escalated to Level 2 support.

Reason for escalation:

- Temporary profile persisted after a controlled sign-out and sign-in.
- Further profile-level diagnostics were required.
- Potential impact on the user's files and normal working environment.

The L1 technician did not attempt registry modifications, profile-directory deletion, or manual profile restoration.

8. Data Protection Considerations

- User was advised not to save important work in the temporary profile.
- No profile folders or registry entries were deleted.
- No backup restoration was attempted without further investigation.
- Further recovery actions were left to the appropriate support level.

9. Final Status

Status: Escalated to L2 — Pending further investigation.

The issue was not conclusively resolved at L1. The underlying cause of the temporary profile loading remains unconfirmed.

10. Skills Demonstrated

- Incident identification.
- Windows 11 troubleshooting.
- User communication.
- Data protection awareness.
- Basic Windows profile diagnostics.
- Appropriate escalation.
- Technical documentation.

---

Portfolio note: This is a fictional service desk simulation. No real user accounts or enterprise systems were involved.