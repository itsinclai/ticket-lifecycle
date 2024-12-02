<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

<p>
This section focuses on resolving a critical ticket from intake to resolution, showcasing how Jane, an agent in the Online Banking Department, handles the ticket lifecycle. The scenario involves troubleshooting a major system outage affecting mobile and online banking platforms.
</p>
<b><p> Stage 1: Intake </p></b>

<p>
An end-user submits a ticket stating, "The entire mobile/online banking system is down. Customers cannot access the banking platform." 
</p>

![image](https://github.com/user-attachments/assets/51db1a64-51a8-4076-9b97-0c2fd183b509)

<p>
As an End-User:
  
- Create a new ticket with the following details:
- Title: Entire mobile/online banking system is down.
- Description: "Customers cannot access the mobile or online banking platform. Please investigate urgently."
</p>

<p> 
Now we’re going to set Properties to the ticket given the severity of the problem:
  
- Sev-A (1 hour, 24/7)
- Online Banking Department
</p>

![image](https://github.com/user-attachments/assets/b436f611-4116-4ad3-9be7-1c3d7b4368b2)

<b><p>Stage 2: Assignment and Prioritization</p></b>

As John (Help Desk Agent), access the newly created ticket in the agent panel. Here you can review the ticket’s default properties:
- Priority: Defaults to “Normal.”
- SLA: Defaults to the system’s standard SLA.
- Assigned To: Unassigned.

![image](https://github.com/user-attachments/assets/32851a94-993a-4416-9c97-154cc3207aa9)

Keep in mind the initial ticket properties provide a baseline but might not reflect the severity or urgency of the issue. Adjusting these properties ensures the right team handles the problem within an appropriate timeframe.

- Update the ticket to reflect the urgency of the outage:
- Priority: Change to Sev-A (1-hour SLA, 24/7 schedule).
- Department: Assign to the Online Banking Department.
- Add a comment to the ticket thread explaining the changes:
- Example: “Ticket updated to Sev-A priority due to the critical nature of the outage. Assigned to Online Banking Department for resolution.”
- Assign the ticket to the Online Banking Team.

![image](https://github.com/user-attachments/assets/bf87ace5-4da2-494b-b5cb-4b7894125939)

Next, we will log out of John and then login as Jane and work the ticket to completion.

<p><b>Stage 3: Working the Issue</p></b>
  
- As Jane (Online Banking Agent), log in to the system as Jane and navigate to the ticket queue.
- Locate the ticket assigned to the Online Banking Department.

Jane notices that while the ticket is assigned to her department, it isn’t yet assigned to a specific agent. 

This setup allows the department’s team members to decide who will handle the issue based on availability and expertise.

- Assign the ticket to yourself to take full ownership. The agent taking ownership becomes the primary point of contact for resolving the issue.

![image](https://github.com/user-attachments/assets/d586abbf-b917-4470-94bf-30c751ad7a10)

- Begin investigating the issue:
- Open the ticket thread to review all previous comments and actions.
- Use the information provided to hypothesize possible causes of the outage.

![image](https://github.com/user-attachments/assets/3da1493e-68c3-44f4-b3e3-f585fd082715)

<b><p>Stage 4: Troubleshooting</p></b>

As Jane, simulate backend troubleshooting:
- Access the system logs to identify anomalies coinciding with the reported outage.
- Confirm that a recent system update caused unexpected errors in the application server.
- Roll back the recent update to restore the system to its previous stable state.
- Verify functionality by conducting tests:
- Check if customers can now log in to the online banking platform.
- Simulate mobile app transactions to confirm end-to-end functionality.

![image](https://github.com/user-attachments/assets/6a2bc764-c7c7-43cb-b779-947b131ce2f6)

<b><p>Stage 5: Resolution and Documentation</b></p>

![image](https://github.com/user-attachments/assets/3b481473-45f2-4cdd-a6c1-698e04f728fc)

- As Jane update the ticket status to Resolved.
- Add a resolution note summarizing the work completed.
- Example: “Identified that a recent update caused the outage. Rolled back the update, tested functionality, and confirmed that the mobile and online banking platforms are operational.”
- Use osTicket’s built-in email functionality to inform the user that the issue has been resolved.
- Include the resolution details in the email for transparency.

Closing the loop with the end-user ensures they are informed of the resolution. Documentation within the ticket ensures traceability for future reference.








