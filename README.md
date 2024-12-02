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
A critical issue arises: customers cannot access the mobile and online banking platform, disrupting operations. Jane will guide us through the ticket lifecycle, leveraging osTicket to track, assign, and resolve the problem efficiently.
</p>
<b><p> Stage 1: Intake </p></b>

<p>
The lifecycle begins with the end-user reporting the issue. They create a ticket titled, "The entire mobile/online banking system is down." In the description, the end-user provides the details: 
</p>
<p>"Customers cannot access the mobile or online banking platform. Please investigate urgently."</p>

![image](https://github.com/user-attachments/assets/51db1a64-51a8-4076-9b97-0c2fd183b509)

<p>
This step is essential to formally document the problem, allowing the support team to respond effectively.

Once submitted, the ticket appears in the system with default properties:

- Priority: Normal
- SLA: Default SLA
- Assigned To: Unassigned
- At this point, the urgency of the problem has not been reflected in the ticket's properties.
</p>

![image](https://github.com/user-attachments/assets/b436f611-4116-4ad3-9be7-1c3d7b4368b2)

<b><p>Stage 2: Assignment and Prioritization</p></b>

The next step involves John, a help desk agent, reviewing and updating the ticket properties to reflect its severity. John logs into osTicket, accesses the new ticket, and observes its default settings. Recognizing the critical nature of the outage, he updates the properties:

- Changes Priority to Sev-A (1-hour SLA, 24/7 schedule).
- Assigns the ticket to the Online Banking Department for resolution.

![image](https://github.com/user-attachments/assets/32851a94-993a-4416-9c97-154cc3207aa9)

John also adds a comment to the ticket thread for clarity:
"Ticket updated to Sev-A priority due to the critical nature of the outage. Assigned to Online Banking Department for resolution."

With these updates, John assigns the ticket to the Online Banking Team, ensuring it reaches the appropriate group for action. After completing his part, John logs out, leaving the next steps to Jane.

![image](https://github.com/user-attachments/assets/bf87ace5-4da2-494b-b5cb-4b7894125939)

<p><b>Stage 3: Working the Issue</p></b>
  
Now, Jane, an agent in the Online Banking Department, logs into osTicket. Navigating to her department’s queue, she identifies the ticket and observes that it is not yet assigned to a specific agent.

This setup allows the team to delegate tasks based on availability and expertise. Jane assigns the ticket to herself, taking full ownership of the problem. Ownership ensures accountability and makes Jane the primary point of contact for resolving the issue.

![image](https://github.com/user-attachments/assets/d586abbf-b917-4470-94bf-30c751ad7a10)

She begins her investigation by reviewing the ticket thread for previous comments and actions. Using the information provided, Jane suspects the problem may be linked to a recent system update.

![image](https://github.com/user-attachments/assets/3da1493e-68c3-44f4-b3e3-f585fd082715)

<b><p>Stage 4: Troubleshooting</p></b>

Jane initiates backend troubleshooting to identify and resolve the issue. First, she accesses the system logs to pinpoint anomalies coinciding with the reported outage. The logs confirm that a recent system update introduced errors in the application server, causing the platform to go offline.

To resolve the issue, Jane rolls back the update, restoring the system to its previous stable state. Afterward, she conducts thorough testing to verify functionality:

- Confirms customers can log in to the online banking platform.
- Simulates mobile app transactions to ensure end-to-end functionality is restored.

![image](https://github.com/user-attachments/assets/6a2bc764-c7c7-43cb-b779-947b131ce2f6)

With the issue resolved, Jane proceeds to the final stage.

<b><p>Stage 5: Resolution and Documentation</b></p>

![image](https://github.com/user-attachments/assets/3b481473-45f2-4cdd-a6c1-698e04f728fc)

To close the ticket, Jane updates its status to Resolved and adds a detailed resolution note:
"Identified that a recent update caused the outage. Rolled back the update, tested functionality, and confirmed that the mobile and online banking platforms are operational."

Jane uses osTicket’s built-in email functionality to notify the end-user. In her email, she outlines the resolution process, providing transparency and building trust with the user.

Proper documentation within the ticket ensures that the solution is traceable, serving as a reference for similar issues in the future.








