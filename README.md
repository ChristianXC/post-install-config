
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

- Configure Roles/Departments/Teams
- Allow Ticket Creation Settings
- Configure Agents/Users
- Set Up SLAs
- Set Up Help Topics

<hr>

<h2>Admin Panel vs Agent Panel</h2>
<ul>
    <li><strong>Admin Panel</strong>: Used by administrators to manage system configurations, roles, departments, teams, SLA, and help topics.</li>
    <img src="https://github.com/user-attachments/assets/66f3c4e7-569a-4a6e-bea1-9b398116249d">
    <li><strong>Agent Panel</strong>: Used by agents to interact with tickets and assist users.</li>
    <img src="https://github.com/user-attachments/assets/c60bdcea-d01b-411a-aec9-643b5fa0090e">
</ul>

<hr>

<h2>Configure Roles</h2>
<img src="https://github.com/user-attachments/assets/ffc44800-d1b2-4b10-89e8-de4b81dbe21b">
<ol>
    <li>Navigate to <strong>Admin Panel -> Agents -> Roles</strong>.</li>
    <li>Add a new role:</li>
    <ul>
        <li><strong>Name:</strong> Supreme Admin</li>
    </ul>
</ol>

<hr>

<h2>Configure Departments</h2>
<img src="https://github.com/user-attachments/assets/06b1cfa7-e728-4d9b-8162-624f243ad9ae">
<ol>
    <li>Navigate to <strong>Admin Panel -> Agents -> Departments</strong>.</li>
    <li>Add departments to define ticket visibility and responsibilities:</li>
    <ul>
        <li><strong>SysAdmins:</strong> Handles system administration tickets.</li>
        <li><strong>Help Desk:</strong> Handles general help desk queries.</li>
        <li><strong>Networking:</strong> Handles network-related issues.</li>
    </ul>
</ol>

<hr>

<h2>Configure Teams</h2>
<img src="https://github.com/user-attachments/assets/d3910e60-573e-4c10-a577-53b4fe25b3ad">
<ol>
    <li>Navigate to <strong>Admin Panel -> Agents -> Teams</strong>.</li>
    <li>Add teams to group agents across different departments:</li>
    <ul>
        <li><strong>Name:</strong> Online Banking</li>
        <li>Pull agents from various departments to collaborate.</li>
    </ul>
</ol>

<hr>

<h2>Allow Ticket Creation Settings</h2>
<img src="https://github.com/user-attachments/assets/7d6230b6-ca96-4a9e-8412-e976a931feb8">
<ol>
    <li>Navigate to <strong>Admin Panel -> Settings -> User Settings</strong>.</li>
    <li>Configure ticket creation options:</li>
    <ul>
        <li><strong>Unregistered users can create tickets:</strong> Uncheck to restrict ticket creation.</li>
        <li><strong>Require registration:</strong> Enable to mandate user registration and login for ticket creation.</li>
    </ul>
</ol>

<hr>

<h2>Configure Agents</h2>
<img src="https://github.com/user-attachments/assets/a54ae354-ca81-4df0-93c5-3f40f5927999">
<ol>
    <li>Navigate to <strong>Admin Panel -> Agents -> Add New</strong>.</li>
    <li>Add new agents and assign departments:</li>
    <ul>
        <li><strong>Jane:</strong> Department - SysAdmins</li>
        <li><strong>John:</strong> Department - Support</li>
    </ul>
</ol>

<hr>

<h2>Configure Users</h2>
<img src="https://github.com/user-attachments/assets/26f7697e-6851-4147-aa06-854f28e91061">
<ol>
    <li>Navigate to <strong>Agent Panel -> Users -> Add New</strong>.</li>
    <li>Add new end users:</li>
    <ul>
        <li><strong>Karen</strong></li>
        <li><strong>Ken</strong></li>
    </ul>
</ol>

<hr>

<h2>Configure SLA Plans</h2>
<img src="https://github.com/user-attachments/assets/946725f4-5d9d-42c7-a6b4-6251c197307e">
<ol>
    <li>Navigate to <strong>Admin Panel -> Manage -> SLA</strong>.</li>
    <li>Add Service Level Agreements (SLA) to define response times:</li>
    <ul>
        <li><strong>Sev-A:</strong> Grace Period - 1 hour, Schedule - 24/7</li>
        <li><strong>Sev-B:</strong> Grace Period - 4 hours, Schedule - 24/7</li>
        <li><strong>Sev-C:</strong> Grace Period - 8 hours, Schedule - Business Hours</li>
    </ul>
</ol>

<hr>

<h2>Configure Help Topics</h2>
<img src="https://github.com/user-attachments/assets/77af9d0b-7e54-4039-abee-bf15014b827f">
<ol>
    <li>Navigate to <strong>Admin Panel -> Manage -> Help Topics</strong>.</li>
    <li>Add help topics to categorize tickets created by users:</li>
    <ul>
        <li>Business Critical Outage</li>
        <li>Personal Computer Issues</li>
        <li>Equipment Request</li>
        <li>Password Reset</li>
        <li>Other</li>
    </ul>
</ol>

<hr>

<h2>Conclusion</h2>
<p>By following this guide, you can set up and configure osTicket for both administrative and operational use, ensuring roles, departments, teams, and SLAs align with your organization’s needs. Document these configurations for future reference or troubleshooting.</p>
