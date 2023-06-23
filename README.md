

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
We are going to give this role Supreme Admin status. Under the Permissions tab, we're going to check all the boxes under Tickets, Tasks, and Knoweledge base and select 'Add Role' when complete. We've now just configured a new role. 
</p>
<br />

<p>
<img src="https://i.imgur.com/WjtpdU3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within the Admin Panel, go to Agents -> Departments -> Add New Department.
</p>
<br />

<p>
<img src="https://i.imgur.com/HA7d4pL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We have not specifically configured some data such as 'manager' and 'SLA' yet so we will leave default settings for this example and select 'System Administrators' as the name of this department and select 'Create Department'
</p>
<br />

<p>
<img src="https://i.imgur.com/0Q1SRUl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within the Admin Panel, go to Agents -> Teams -> Add New Team.
</p>
<br />

<p>
<img src="https://i.imgur.com/8yjB1dL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This team will be named Level I or II support. 
</p>
<br />

<p>
<img src="https://i.imgur.com/Rmaz85P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Again, we have not specifically configured individual members but so we will leave blank for now. When complete, select 'Create Team'. Repeat the same actions when you create the other Level Support Team and add its respective members.
</p>
<br />

<p>
<img src="https://i.imgur.com/qyU3L4u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to Admin Panel -> Settings -> Users -> ensure Registration Method is 'Public' and this will allow all registered users to create tickets. 
</p>
<br />

<p>
<img src="https://i.imgur.com/oqNJsp7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to Admin Panel -> Agents -> Agents -> Add New Agent
</p>
<br />

<p>
<img src="https://i.imgur.com/D8SGhF8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Fill in the Agent's contact information under the 'Account' Tab
</p>
<br />

<p>
<img src="https://i.imgur.com/xmKoAIs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the 'Access' Tab you can assign the Agent to a primary department depending on their skills/credentials with a role such as the 'Supreme Admin' role we created before. You can extend their access by assigning them to additional departments as well. 
</p>
<br />

<p>
<img src="https://i.imgur.com/FyYKqhq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally in the 'Permissions' Tab, this permits the Agent actions they may take to resolve tickets created by users. 
</p>
<br />

<p>
<img src="https://i.imgur.com/mwNfbBc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Agent Panel -> Users -> Add New User
</p>
<br />

<p>
<img src="https://i.imgur.com/TeUw52G.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Fill in the new user's information and select 'Add User' 
</p>
<br />

<p>
<img src="https://i.imgur.com/gbRH57s.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Admin Panel -> Manage -> SLA -> Add New SLA Plan
</p>
<br />

<p>
<img src="https://i.imgur.com/L7tLzWI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This SLA is named SEV-A for Level of Severity A (as being the top-most priority and requiring the most immediate resolution). For this example the Grace Period is 1 hour within a 24/7 Schedule. That means any day of the week/year, this ticket must be responded to within an hour. You can create additional SLA Plans (Levels of Severity) by following the same steps and adjusting the grace period and schedule. Then select 'Add Plan' to create the plan.
</p>
<br />

<p>
<img src="https://i.imgur.com/RUnQInI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Admin Panel -> Manage -> Help Topics -> Add New Help Topic 
</p>
<br />

<p>
<img src="https://i.imgur.com/aqVUXgL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Give the Help Topic the name 'Business Critical Outage,' active status and type should be 'Public.' The Parent Topic is the level of criticality the topic belongs and should go to its respective level based on the organization and its needs. 
</p>
<br />

<p>
There is a way to configure emails to be sent to a specific address users can use with forms and the system will automatically generate a ticket for them. Many organizations do this for efficiency. 
</p>
