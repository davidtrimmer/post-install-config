<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Log in to Admin Portal
- Configure Roles, Departments, and Teams
- Configure Agents who will work tickets (Jane and John)
- Configure Users who will submit tickets (Karen/Ken) 
- Configure SLA's and Help Topics

<h2>Configuration Steps</h2>
<p>
  After getting the osTicket software downloaded, it is time to log in so we can begin configuring osTicket. 
</p>
<p>
  <img width="404" alt="Screenshot 2025-03-18 at 5 20 09 PM" src="https://github.com/user-attachments/assets/3775cc8c-3c2a-449b-908b-437c371ddb3a" />
</p>
<br />
<p>
After logging in, it is time to configure our Roles, Departments, and Teams. Here, I am configuring the "SysAdmin" Department that we will later add our Agents to. 
</p>
<p>
  <img width="962" alt="Screenshot 2025-03-18 at 5 22 20 PM" src="https://github.com/user-attachments/assets/fccad6fc-1a8f-402f-aab4-85a5916a9690" />
  <img width="959" alt="Screenshot 2025-03-18 at 5 22 51 PM" src="https://github.com/user-attachments/assets/95f5acb9-5dc3-47c3-845a-144ef4c7e6f0" />
  <img width="964" alt="Screenshot 2025-03-18 at 5 24 08 PM" src="https://github.com/user-attachments/assets/95ae55c6-4dd5-48c6-bbc9-c2a1c2a9f20b" />
</p>
<p>
  First, go to Agents -> Roles -> Add New Role -> Create Name (Supreme Admin) -> Give Permissions -> OK
  This will create our first role of "Supreme Admin"
</p>
<br />
<p>
  Next, we will create the SysAdmins Department. Admin Panel -> Agents -> Departments -> SysAdmins
</p>
<p>
  <img width="963" alt="Screenshot 2025-03-18 at 5 32 16 PM" src="https://github.com/user-attachments/assets/be607f1a-a6ac-4b8c-a92c-adc8d42ac435" />
  <img width="959" alt="Screenshot 2025-03-18 at 5 32 31 PM" src="https://github.com/user-attachments/assets/2d55c7bc-9b8c-4799-bc26-e940a5b02ba7" />
</p>
<br/>
<p>
  Next, we will configure the Teams. Admin Panel -> Agents -> Teams (Pull Agents from different Departments) -> Online Banking
</p>
<p>
  <img width="961" alt="Screenshot 2025-03-18 at 5 37 47 PM" src="https://github.com/user-attachments/assets/8c6066ae-10ea-44cc-8a77-099559149b40" />
<img width="969" alt="Screenshot 2025-03-18 at 5 38 09 PM" src="https://github.com/user-attachments/assets/d2d786d7-d18a-476b-8384-79081b8a9892" />
</p>
<br/>
<p>
  Next, we will allow anyone to create tickets. Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
</p>
<p>
  <img width="966" alt="Screenshot 2025-03-18 at 5 42 16 PM" src="https://github.com/user-attachments/assets/f93c8e54-9278-4662-9cd8-622bdc2a4728" />
</p>
<br/>
<p>
  Next, we will create our Agents. They will be John and Jane Doe. Jane will be apart of the SysAdmins and the Online Banking team with Supreme Admin access. John will be apart of the Support team and granted unlimited access. 
</p>
<p>
  <img width="975" alt="Screenshot 2025-03-18 at 5 44 23 PM" src="https://github.com/user-attachments/assets/d0207dee-b239-45be-8f1e-c4d868ccceb3" />
  <img width="964" alt="Screenshot 2025-03-18 at 5 46 30 PM" src="https://github.com/user-attachments/assets/c4d1c51e-7461-451e-8588-c5baa959444a" />
  <img width="956" alt="Screenshot 2025-03-18 at 5 46 38 PM" src="https://github.com/user-attachments/assets/6c1958e4-2556-465c-80c2-0190868792b3" />
<img width="968" alt="Screenshot 2025-03-18 at 5 48 06 PM" src="https://github.com/user-attachments/assets/a9f19eae-ead9-4dc2-b78d-8dfab45adaee" />
</p>
<br/>
<p>
 Next, we will configure our end users. Go to: Agent Panel -> Users -> Create New
</p>
<p>
  <img width="949" alt="Screenshot 2025-03-18 at 5 56 07 PM" src="https://github.com/user-attachments/assets/83b8c995-6a7f-4f52-82d4-5d831d5108c1" />
</p>
<br/>
<p>
Last two steps are to configure the SLA and Help Topics. These range from Sev-A-Sev-C based on the level of importance a ticket needs to be closed. Help Topics vary based on what the user is seeking help for. Admin Panel -> Manage -> SLA
</p>
<p>
  Then add the following SLA to each SLA. 
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)
</p>
<p>
 <img width="966" alt="Screenshot 2025-03-18 at 5 42 16 PM" src="https://github.com/user-attachments/assets/ccb21291-740a-4935-8a03-b7da2a42c9a4" />
  <img width="968" alt="Screenshot 2025-03-18 at 6 03 15 PM" src="https://github.com/user-attachments/assets/8d455431-1663-4926-93e7-b41343fd011d" />
</p>
<br />
<p>
  Lastly, we will configure Help Topics. Admin Panel -> Manage -> Help Topics . These are used when the end user fills out a ticket. We can use the following Topics: 
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other 
</p>
<p>
  <img width="960" alt="Screenshot 2025-03-18 at 6 12 52 PM" src="https://github.com/user-attachments/assets/dc340ee0-fab6-4c68-a71e-53c9c8f5ea29" />
  <img width="962" alt="Screenshot 2025-03-18 at 6 16 08 PM" src="https://github.com/user-attachments/assets/6b533471-90cc-4658-887b-4ac92f7e585e" />
</p>
<br/>
<p>
  Congrats, we can now create and work tickets in osTicket!
</p>
<br/>

