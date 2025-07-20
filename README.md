<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Be able to configure roles, departments, teams, agents, users, SLA, and help topics for your ticketing system

<h2>Configuration Steps</h2>

<p>
Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 

End Users osTicket URL:
http://localhost/osTicket 

Acknowledge Agent Panel vs Admin Panel

Configure Roles (for grouping permissions):
  - Admin Panel -> Agents -> Roles
    - Supreme Admin

<img src="https://i.imgur.com/Lw3D6A0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
  - Admin Panel -> Agents -> Departments
    - SysAdmins

<img src="https://i.imgur.com/LP2Mzz4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Configure Teams
  - Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
    - Online Banking

<img src="https://i.imgur.com/hdTe1rd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Allow anyone to create tickets
  - Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
    - Registration Required: Require registration and login to create tickets 

<img src="https://i.imgur.com/gwSlbao.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Configure Agents (workers)
  - Admin Panel -> Agents -> Add New
    - Jane (Dept: SysAdmins)
    - John (Dept: Support)

<img src="https://i.imgur.com/STpBSx2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Configure Users (customers)
  - Agent Panel -> Users -> Add New
    - Karen
    - Ken

<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Configure SLA
  - Admin Panel -> Manage -> SLA
    - Sev-A (Grace Period: 1 hour, Schedule: 24/7)
    - Sev-B (Grace Period: 4 hours, Schedule: 24/7)
    - Sev-C (Grace Period: 8 hours, Business Hours)

<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Configure Help Topics (For when users create a ticket)
  - Admin Panel -> Manage -> Help Topics
    - Business Critical Outage
    - Personal Computer Issues
    - Equipment Request
    - Password Reset
    - Other

<img src="https://i.imgur.com/nIWW6qi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
