# osTicket-Post-Installation-Configuration
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h2>Discription </h2>

This tutorial outlines the necessary configurations after installation to properly simulate a real world enviroment of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
  
<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- osTicket v1.15.8


<h2>Configuration Steps</h2>

1. Open admin/analyst login page http://localhost/osTicket/scp/login.php -> Open end user login page http://localhost/osTicket 

![image](https://github.com/user-attachments/assets/b8a0a16a-18d9-492d-93e3-b9eca5669332)
![image](https://github.com/user-attachments/assets/92aa8792-6bd6-48bd-a8f8-478b53b88f16)

2. Acknowledge Agent vs Admin panel  

Admin webpage -> Sign in as admin -> Admin panel -> Agent panel

![image](https://github.com/user-attachments/assets/7eeface6-2228-4786-b4e5-a095f33507bc)
![image](https://github.com/user-attachments/assets/486071fe-2ba4-4c6a-9591-871231976ed5)
![image](https://github.com/user-attachments/assets/6403fbde-143d-4a5e-8820-626e80fcf40d)

3. Configure Roles
   Admin Login Page -> Admin Panel -> Agents -> Roles -> Add New Role -> Type "Supreme Admin" -> Permissions -> Check all the boxes -> Add Role

4. Configure Departments
   Admin Login Page -> Admin Panel -> Agents -> Departments -> Add New Department -> For Parent select "Top Level Department" -> For Name type "SysAdmins" -> Create
   Admin Login Page -> Admin Panel -> Agents (in the top row, not second row) -> Departments -> Maintenance -> Delete -> Save

5. Configure Teams
    Admin Login Page -> Admin Panel -> Agents -> Teams -> Add New Team -> For Name type "Omline Banking" -> Create

6. Allow anyone to create tickets
   Admin Login Page -> Admin Panel -> Settings -> Users -> *Note* Make sure the box next to "Registration Required" is unchecked -> Save 

7. Configure Agents (Create workers)
   Admin Login Page -> Admin Panel -> Agents -> Add New Agents -> Enter Name -> Enter Email address -> Enter Username -> Set Password -> Uncheck top box -> Enter Password in both boxes -> Unckeck bottom box -> Update -> Access tab -> For Primary dept. "Support/SysAdmins" -> For Roles "Supreme Admin"  
   -> Teams tab -> Online Banking -> Create -> Save to notepad

   Admin Login Page -> Admin Panel -> Agents -> Add New Agents -> Enter Name -> Enter Email address -> Enter Username -> Set Password -> Uncheck top box -> Enter Password in both boxes -> Unckeck bottom box -> Update -> Access tab -> For Primary dept. "Support" -> For Roles "All Access" -> Create
   -> Save to notepad

8. Re-Configure Teams
    Admin Login Page -> Admin Panel -> Agents -> Teams -> Select Team -> Members -> Select Agent -> Add -> Save

   Admin Login Page -> Admin Panel -> Agents -> Teams -> Select Team -> Members -> Select Agent -> Add -> Save

9. Configure Users (Create End Users)
   Admin Login Page -> Agent Panel -> Users -> Add User -> Enter email address -> Enter Name -> Create -> Save to notepad -> *Repeat to Create another End User*

10. Configure SLA (Create SLAs)
   Admin Login Page -> Admin Panel -> Manage -> SLA -> Add New SLA -> Enter Name -> Enter Grace Period -> Select Scheduale -> Add plan -> *Repeat to Create Two more SLAs for a total of Three SLAs*

11. Configure Help Topics (Create Help Topics)
    Admin Login Page -> Admin Panel -> Manage -> Help Topics -> Add New Help Topic -> Enter Name -> Choose Parent Topic -> Add Topic -> *Repeat to Create Four more Help Topics for a total of five Help Topics*

Congratulatons on finishing the modifications needed to use the osTicket software in a simulated real world application. Now you can move on to practice creating and solving tickets.


