

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.
<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents (workers)
- Configure Users (customers)
- Configure Service Level Agreements (SLA)
- Configure Help Topics

<h2>Configuration Steps</h2>
<p>
<img src="https://i.imgur.com/KDy5leq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First things first, let log into osTicket as an administrator.  We created this in the osTicket installation repository.
</p>
<br />

<p>
<img src="https://i.imgur.com/5gtUeEy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Under the 'Admin Panel,' Go to Agents -> Roles -> Add New Role.
</p>
<br />

<p>
<img src="https://i.imgur.com/msi0OOx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We are going to give this role Supreme Admin status. Under the Permissions tab, we're going to check all the boxes under Tickets, Tasks, and Knoweledge base and select 'Add Role' when complete. We've now just configured a new role! 
</p>
<br />

<p>
<img src="https://i.imgur.com/7kfGMx9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/7kfGMx9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within the Admin Panel, go to Agents -> Departments -> Add New Department.
</p>
<br />

<p>
<img src="https://i.imgur.com/MU8eWMh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will leave default settings for this example and select 'System Administrators' as the name of this department and select 'Create Department'
</p>
<br />

<p>
<img src="https://i.imgur.com/6mjEWw3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/YSvPXai.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the Admin Panel, go to Agents -> Teams -> Add New Team.
</p>
<br />

<p>
<img src="https://i.imgur.com/jd1DX2u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
These teams will be named Level I or II support. 
</p>
<br />

<p>
<img src="https://i.imgur.com/gpakN2V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
When complete, select 'Create Team'. Repeat the same actions when you create the other Level Support Team and add its members.
</p>
<br />

<p>
<img src="https://i.imgur.com/UNsxKXx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now go to Admin Panel -> Settings -> Users -> ensure Registration Method is 'Public', this will allow all registered users to create tickets. 
</p>
<br />

<p>
<img src="https://i.imgur.com/D5L6pRw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to Admin Panel -> Agents -> Agents -> Add New Agent
</p>
<br />

<p>
<img src="https://i.imgur.com/JOhtH0K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Fill in the Agent's contact information under the 'Account' Tab
</p>
<br />

<p>
<img src="https://i.imgur.com/7YdGiek.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the 'Access' Tab you can assign the Agent to a primary department depending on their role such as the 'Supreme Admin' role we created before. You can extend their access by assigning them to additional departments as well. Here we assigned Jane Doe to the Supreme Admin role and assigned John doe a tech support role. Also, within the permissions tab, this will grant the permission to work on and resolve tickets. Unfortunatly I did not get a screenshot of this.
</p>
<br />


<p>
<img src="https://i.imgur.com/SrIdAfd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we will switch over to the Agent Panel -> Users -> Add New User
</p>
<br />

<p>
<img src="https://i.imgur.com/hlbQ3sv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Fill in the new user's information and select 'Add User'. We'll create a few proxy users for our examples.
</p>
<br />

<p>
<img src="https://i.imgur.com/2aKbDnq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we will switch back to the Admin Panel -> Manage -> SLA -> Add New SLA Plan
</p>
<br />

<p>
<img src="https://i.imgur.com/nsOIDBq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<br />

<p>
<img scr="https://i.imgur.com/NthHVaS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This SLA is named SEV-A for Level of Severity A (as being the top-most priority and requiring the most immediate resolution). For this example the Grace Period is 1 hour within a 24/7 Schedule. This means any day of the week, 24/7, this ticket must be responded to within 1 hour. You can create additional SLA Plans by following the same steps and adjusting the grace period and/or schedule. Then select 'Add Plan' to create the plan.
</p>
<br />

<p>
<img src="https://i.imgur.com/VPiMlI1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Still within the Admin Panel, go to -> Manage -> Help Topics -> Add New Help Topic 
</p>
<br />

<p>
<img src="https://i.imgur.com/ZvEk3zx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We will name our Help Topic 'Business Critical Outage,' active status and the type should be 'Public.' The Parent Topic is the level of criticality, the topic should go to its respective level based on the organization. We will create a few different topics with different priority levels.
</p>
<br />

<p>
There is a way to configure emails to be sent to a specific address users can use with forms and the system will automatically generate a ticket for them. Multiple Dusinesses and orginazations operate this way for effectivness.
</p>
