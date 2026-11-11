IT-003 — Troubleshooting Log

Ticket Information

Field| Details
Ticket ID| IT-003
Technician| Level 1 Service Desk
Date| 11 November 2026
Start Time| 10:30
Device| Dell OptiPlex 7090
Operating System| Windows 11

Troubleshooting Record

Step| Action Performed| Observation / Result
1| Obtained the user's description of the performance issue.| User reported slow application startup and intermittent freezing.
2| Asked the user whether the workstation had been restarted.| User confirmed two restarts had already been attempted without improvement.
3| Opened Task Manager using Ctrl + Shift + Esc.| Overall CPU usage fluctuated between 35% and 45%; memory utilisation was 82%.
4| Reviewed the Processes tab.| Excel was using 18% CPU and 1,250 MB memory. Chrome was using 12% CPU and 1,100 MB memory.
5| Asked the user to save work and close Excel and Chrome.| Both applications were closed before being reopened individually.
6| Reopened Excel with only the active workbook.| Excel usage decreased to 4% CPU and 720 MB memory. Overall memory utilisation decreased to 68%.
7| Closed Excel and reopened Chrome with only the required browser tab.| Chrome usage was 5% CPU and 650 MB memory. Overall memory utilisation decreased to 65%.
8| Asked the user to assess workstation performance.| User confirmed noticeable improvement and smoother application response.

Technical Findings

- Initial overall memory utilisation: 82%.
- Memory utilisation after reopening Excel: 68%.
- Memory utilisation after reopening Chrome: 65%.
- Excel and Chrome showed lower resource consumption after being reopened with only active work selected.
- The results supported excessive application resource consumption as a likely contributing factor.

Corrective Action

The user was advised to save work and close unnecessary applications, workbooks and browser tabs.

Applications were reopened individually with only the required work loaded.

Escalation Assessment

No escalation was required.

The reported performance symptoms improved following Level 1 troubleshooting, and the user confirmed the improvement.

Final Status

Resolved — Level 1 Support

The user was provided with preventive guidance to reduce unnecessary application usage and minimise the likelihood of recurrence.