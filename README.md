<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configurations</h1>
This lab demonstrates the necessary changes I made to configure osTicket into a functioning ticketing system that mimics real-world IT support workflows. These configurations help simulate a professional service desk environment where roles, teams, and priorities are clearly defined.

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machine)</li>
  <li>Remote Desktop Connection</li>
  <li>osTicket</li>
</ul>

<h2>Operating System Used</h2>
<ul>
  <li>Windows 10 Pro (21H2)</li>
</ul>

<h2>Configuration Steps</h2>

<p>
<img src="https://github.com/Herkamal/post-install-config/blob/main/roles.png" height="80%" width="80%" alt="Supreme Admin Role"/>
</p>
<p>
After the installation of osTicket, the first step was to create a custom role called <b>Supreme Admin</b>. This role is granted full access to all functions and management features in osTicket. The role was created under the Admin panel in the <b>Agents > Roles</b> section, allowing agents assigned to it to have unrestricted administrative privileges throughout the system.
</p>

<p>
<img src="https://github.com/Herkamal/post-install-config/blob/main/departments.png" height="80%" width="80%" alt="Departments"/>
</p>
<p>
Next, I created a new department named <b>System Administrators</b>. Departments help organize agents into functional groups for better ticket routing and escalation. This was configured in the <b>Agents > Departments</b> menu of the Admin panel.
</p>

<p>
<img src="https://github.com/Herkamal/post-install-config/blob/main/teams.png" height="80%" width="80%" alt="Teams"/>
</p>
<p>
I then set up a new team labeled <b>Online banking</b>. Teams allow agents from different departments to collaborate. This team supports more advanced issues that go beyond first-level troubleshooting. It was added through the <b>Agents > Teams</b> section in the Admin panel.
</p>

<p>
<img src="https://github.com/Herkamal/post-install-config/blob/main/Agents.png" height="80%" width="80%" alt="Agents"/>
</p>
<p>
To simulate a live support environment, I created two new agents: <b>Jane Doe</b> and <b>John Doe</b>. These agents are assigned roles and departments so they can manage and respond to incoming tickets. Agent creation was done under <b>Agents > Add New Agent</b>.
</p>

<p>
<img src="https://github.com/Herkamal/post-install-config/blob/main/users.png" height="80%" width="80%" alt="Users"/>
</p>
<p>
I added a new user named <b>Karen</b> to simulate an end-user submitting a support ticket. This allows for testing of the full ticket workflow—from user creation to issue resolution. Users were added from the Agent panel under the <b>Users</b> tab.
</p>

<p>
<img src="https://github.com/Herkamal/post-install-config/blob/main/SLA.png" height="80%" width="80%" alt="SLA"/>
</p>
<p>
I configured <b>Service Level Agreements (SLAs)</b> to define the expected response and resolution times based on ticket priority. SEV-A, SEV-B, and SEV-C were created to represent high, medium, and low priority tickets respectively. SLAs were set under the Admin panel via <b>Manage > SLA</b>.
</p>

<p>
<img src="https://github.com/Herkamal/post-install-config/blob/main/help-topic.png" height="80%" width="80%" alt="Help Topics"/>
</p>
<p>
Finally, I set up multiple <b>Help Topics</b> to guide users when submitting tickets. These topics include Business Critical Outage, Personal Computer Issues, Equipment Reset, and Password Request. This helps categorize issues for better ticket routing. Help Topics were added through <b>Admin Panel > Manage > Help Topics</b>.
</p>

<h2>osTicket Configurations are Complete</h2>
<p>
With all the necessary configurations completed, osTicket is now fully functional as a support ticketing system. I am able to simulate a real-world IT support process, from user submission to agent response, team collaboration, and ticket prioritization based on impact.
</p>
