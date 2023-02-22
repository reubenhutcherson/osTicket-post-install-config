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

- If you need help installing osTicket, please see my tutorial [here](https://github.com/reubenhutcherson//osTicket-prereqs-installation)
- You can sign in using this link: http://localhost/osTicket/scp) 

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
  
  
  <h3>Step 6: Configure Agents</h3>

-  Make sure you are in admin panel (check top right to see which panel you are in)
- Select the Agents tab -> Add New Agents
	- Name: Jane Doe
	- Email : jane.doe@osticket.com
	- Username: jane.doe
	- Click set password and uncheck box that says "send the agent a password reset email
		- Set your password to anything you like
		- uncheck box that says "require password change at next login
		- Select set
		
<p align="center">
<img src="https://i.imgur.com/l0XG75R.jpg" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/XSGnlrL.jpg" height="70%" width="70%" alt="Azure Free Services"/>
</p>

- Select Access tab 
	- Under Primary Department 
		- Select department dropdown menu -> System Administrators
		- Select Role dropdown menu -> Supreme Admin
	- Extended Accesss 
		- Select Department -> Support -> Add -> Supreme Admin
- Select Teams tab
	- Select team dropdown menu -> Level II Support
	- Select Add
- Select Create	

	
<p align="center">
<img src="https://i.imgur.com/L8CaX8T.jpg" height="70%" width="70%" alt="Azure Free Account"/> <img src="https://i.imgur.com/vYMfiX5.jpg" height="70%" width="70%" alt="Azure Free Services"/>
</p>

- Create another agent named John.
	- Follow same steps as above except make some changes to Primary Department
		- Select department dropdown menu -> Support
		- Select Role dropdown menu -> View only
	- Extended Accesss 
		- Select Department -> Support -> Save Changes
		
<p align="center">
<img src="https://i.imgur.com/Pm9TGyW.jpg" height="70%" width="70%" alt="Azure Free Account"/><img src="https://i.imgur.com/bJI6W4U.jpg" height="70%" width="70%" alt="Azure Free Account"/>  
</p>
 

<h3>Step 7: Configure Users
</h3>

- Make sure you are in Agent panel (check top right to see which panel you are in)
	- If the top right says "admin" you are in the agent panel
	
<p align="center">
<img src="https://i.imgur.com/u3eSpGW.jpg" height="80%" width="80%" alt="Azure Free Account"/>		
	
- Select Users tab to create user
	- Email Address: Karen@osticket.com
	- Full Name - Karen Karen
	- Select Add User
	
<p align="center">
<img src="https://i.imgur.com/kCvY5od.jpg" height="80%" width="80%" alt="Azure Free Account"/>			
	
 - Select user tab again to create another user
	- Email Address: Ken@osticket.com
	- Full Name - Ken Ken
	- Select Add User

<p align="center">
<img src="https://i.imgur.com/1zBfFKL.jpg" height="80%" width="80%" alt="Azure Free Account"/>
	
	
<h3>Step 8:  Configure Service Level Agreements (SLA)
</h3>

- Make sure you are in admin panel (check top right to see which panel you are in)
- Select Manage tab -> SLA -> Add New SLA Plan (We are creating 3)
	- Name: SEV-A 			
	- Grace Period: 1
	- Schedule dropdown menu: 24/7
	- Select Add Plan

<p align="center">
<img src="https://i.imgur.com/mwF6Cic.jpg" height="80%" width="80%" alt="Azure Free Account"/>
	
- Name: SEV-B
- Grace Period: 4
- Schedule dropdown menu: 24/7
- Select Add Plan
	
<p align="center">
<img src="https://i.imgur.com/3Q8oi3h.jpg" height="80%" width="80%" alt="Azure Free Account"/>
	
- Name: SEV-C 
- Grace Period: 8
- Schedule dropdown menu: Monday - Friday 8AM - 5PM with U.S Holidays
- Select Add Plan

<p align="center">
<img src="https://i.imgur.com/S9KalEE.jpg" height="80%" width="80%" alt="Azure Free Account"/>
	
	
<h3>Step 9:   Configure Help Topics
</h3>

-  Make sure you are in admin panel (check top right to see which panel you are in)
- Select Manage tab -> Help Topics -> Add New Help Topic (We will be adding 4)
	- Business Critical Outage
	- Personal Computer Issues
	- Equipment Request
	- Password Reset
- Select Add Topic for each topic

<p align="center">
<img src="https://i.imgur.com/Vh0YvW5.jpg" height="80%" width="80%" alt="Azure Free Account"/>
	
	
Congratulations! You have set up osTicket succesfully! Click [here](https://github.com/reubenhutcherson/ticket-lifecycle) to move on to the final part of this tutorial series! 

