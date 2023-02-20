<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket -  Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure
- Virtual Machine
- osTicket 


<h2>Good Things to Know</h2>

 - Click on specific positions for a better understanding!
 	- [Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)
	- [Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)
	- [Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html) 
	- [Agents](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)
	- [Users](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html).
	- [Service Level Agreement(SLA)](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)

<h2>Installation Steps</h2>

<h3>Step 1: Open osTicket and log in using credentials from installation tutorial </h3>

- If you need help installing osTicket, please see my tutorial [here](https://github.com/reubenhutcherson/osticket-prereqs)

<p align="center">
<img src="https://i.imgur.com/0xN5pmy.jpg" height="80%" width="80%" alt="Azure Free Account"/>	

  <h3>Step 2: Configure Roles </h3>

- Make sure you are in admin panel (check top right to see which panel you are in)
	- If the top right says "agent" you are in the admin panel
- Select the Agents tab -> Roles -> Add New Role
	- Name : Supreme Admin
	- Select Permissions tab and check every box under the "Tickets", "Tasks" and "Knowledgebase" section
- Select Add Role
	
  
<p align="center">
<img src="https://i.imgur.com/vXq7Gx7.jpg" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/50dn3Ve.jpg" height="70%" width="70%" alt="Azure Free Services"/> <img src="https://i.imgur.com/7DWDkFN.jpg" height="70%" width="70%" alt="Azure Free Services"/>
</p>


<h3>Step 3: Configure Departments</h3>

- Make sure you are in admin panel (check top right to see which panel you are in)
- Select the Agents tab -> Departments -> Add New Department 
	- Name: System Admins
- Select Create Dept. 

<p align="center">
<img src="https://i.imgur.com/aOi1azp.jpg" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/y2UkjzX.jpg" height="70%" width="70%" alt="Azure Free Services"/> <img src="https://i.imgur.com/vgLScra.jpg" height="70%" width="70%" alt="Azure Free Services"/>
</p>


<h3>Step 4:  Configure Teams
</h3>

- Make sure you are in admin panel (check top right to see which panel you are in)
- Select the Agents tab -> Teams -> Add New Team
	- Name: Level II Support 
- Select create team. 
	
<p align="center">
<img src="https://i.imgur.com/jouJYDV.jpg" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/n8oJik8.jpg" height="70%" width="70%" alt="Azure Free Services"/>
</p>


<h3>Step 5: Allow anyone to create tickets</h3>

 Make sure you are in admin panel (check top right to see which panel you are in)
- Select the Settings -> User Settings
	- Make sure box is unchecked: 
		- Registration Required: Require registration and login to create tickets 
		
<p align="center">
<img src="https://i.imgur.com/eoTUu1t.jpg" height="80%" width="80%" alt="Azure Free Account"/>
  
  
  

