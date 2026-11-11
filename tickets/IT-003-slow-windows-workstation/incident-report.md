IT-003 — Slow Windows Workstation

1. Incident Details

Field| Details
Ticket ID| IT-003
Date| 11 November 2026
Time Logged| 10:30
Reported By| Michael Dlamini
Department| Finance
Device| Dell OptiPlex 7090
Operating System| Windows 11
Priority| Medium (provisional)
Assigned Level| Level 1 Service Desk
Status| Resolved
Escalation| Not required

2. Incident Description

The user reported that their workstation had been running unusually slowly since the previous day.

Microsoft Excel and Outlook were taking longer than usual to open, and the computer occasionally froze for several seconds. The user had already restarted the workstation twice, but the problem persisted.

The issue was affecting the user's ability to complete normal work activities.

3. Investigation

The technician instructed the user to open Windows Task Manager using Ctrl + Shift + Esc.

The Processes tab was reviewed to identify applications consuming significant CPU and memory resources.

Initial observations included:

- Excel: 18% CPU and 1,250 MB memory.
- Chrome: 12% CPU and 1,100 MB memory.
- Outlook: 7% CPU and 680 MB memory.
- Overall memory utilisation: 82%.

The technician suspected that multiple open applications and unused workbooks or browser tabs could be contributing to the performance issue.

4. Corrective Action

The user was instructed to:

1. Save all current work.
2. Close Excel and Chrome.
3. Reopen Excel and load only the active workbook.
4. Close Excel before reopening Chrome.
5. Restore only the browser tab required for current work.
6. Review Task Manager again after reopening each application.

Following these steps, resource utilisation decreased:

- Excel reopened: 4% CPU and 720 MB memory; overall memory utilisation decreased to 68%.
- Chrome reopened: 5% CPU and 650 MB memory; overall memory utilisation decreased to 65%.

The user reported that the workstation was noticeably faster.

5. Resolution and Verification

The user confirmed that the workstation was responding better and that Excel and Chrome were functioning more smoothly.

The corrective action resolved the reported performance symptoms during the simulated investigation.

No escalation to Level 2 support was necessary.

6. Root Cause Assessment

Excessive resource consumption associated with multiple open applications, workbooks and browser tabs was identified as the likely contributing factor.

The precise underlying cause was not independently established.

7. Preventive Recommendations

The user was advised to:

- Save work regularly.
- Close applications that are no longer required.
- Avoid keeping unnecessary browser tabs and Excel workbooks open.
- Monitor CPU and memory utilisation if the performance issue returns.

8. Final Outcome

Status: Resolved

The workstation's performance improved following application management and resource-utilisation checks. The user confirmed the improvement, and the ticket was closed at Level 1 without escalation.