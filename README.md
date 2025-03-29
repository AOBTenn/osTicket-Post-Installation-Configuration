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

![image](https://github.com/user-attachments/assets/c88cd158-5ee3-4221-b331-a223e99ed207)
![image](https://github.com/user-attachments/assets/4b67e5ab-95e4-432a-ac01-07187479cd36)
![image](https://github.com/user-attachments/assets/f3e3a003-1e10-45bd-b172-06f82f4dbbe2)
![image](https://github.com/user-attachments/assets/a6874e44-fa6c-4664-8796-ea84b55183dc)

4. Configure Departments
   Admin Login Page -> Admin Panel -> Agents -> Departments -> Add New Department -> For Parent select "Top Level Department" -> For Name type "SysAdmins" -> Create

![image](https://github.com/user-attachments/assets/1653c26d-e825-4116-9a2e-48dd5394947b)

   Admin Login Page -> Admin Panel -> Agents (in the top row, not second row) -> Departments -> Maintenance -> Delete -> Save

![image](https://github.com/user-attachments/assets/1cca647a-cf5d-469b-b643-3a72b7f70c1d)

6. Configure Teams
    Admin Login Page -> Admin Panel -> Agents -> Teams -> Add New Team -> For Name type "Omline Banking" -> Create

![image](https://github.com/user-attachments/assets/39d4d901-f4bf-41c7-b36e-9b72adb4e456)

![image](https://github.com/user-attachments/assets/53dee0ae-9b68-4c2a-ba5a-0da2a27bd8cb)

7. Allow anyone to create tickets
Admin Login Page -> Admin Panel -> Settings -> Users -> *Note* Make sure the box next to "Registration Required" is unchecked -> Save 

![image](https://github.com/user-attachments/assets/ec467781-1996-4de4-8f85-7749c9d2f0dd)

8. Configure Agents (Create workers)
Admin Login Page -> Admin Panel -> Agents -> Add New Agents -> Enter Name -> Enter Email address -> Enter Username -> Set Password -> Uncheck top box -> Enter Password in both boxes -> Unckeck bottom box -> Update -> Access tab -> For Primary dept. "Support/SysAdmins" -> For Roles "Supreme Admin" -> Teams tab -> Online Banking -> Create -> Save to notepad

![image](https://github.com/user-attachments/assets/c29ec573-2224-4408-bb8c-8ef28601419e)
![image](https://github.com/user-attachments/assets/1307b1a9-750e-4391-9ac0-1ac213ae6cf8)
![image](https://github.com/user-attachments/assets/66b866cf-fc1b-4b05-bff3-03e78c25d815)
![image](https://github.com/user-attachments/assets/5376e259-6518-4487-aa66-0d35bc0560e3)
![image](https://github.com/user-attachments/assets/43bc501d-a4cf-414e-92db-042082c5bb29)

  Admin Login Page -> Admin Panel -> Agents -> Add New Agents -> Enter Name -> Enter Email address -> Enter Username -> Set Password -> Uncheck top box -> Enter Password in both boxes -> Unckeck bottom box -> Update -> Access tab -> For Primary dept. "Support" -> For Roles "All Access" -> Create -> Save to notepad

![image](https://github.com/user-attachments/assets/7ad97cf2-07ba-4af7-8547-32cf2184d34d)
![image](https://github.com/user-attachments/assets/09ea5d5c-1c36-4abb-987d-3be56992617f)
![image](https://github.com/user-attachments/assets/b68a12a6-5b2c-4e4d-80d4-25be9d7516bf)
![image](https://github.com/user-attachments/assets/4b5a1c04-e914-4864-b107-82278b0c44d3)

9. Re-Configure Teams
    
Admin Login Page -> Admin Panel -> Agents -> Teams -> Select Team -> Members -> Select Agent -> Add -> Save

![image](https://github.com/user-attachments/assets/cb3705b1-2599-42c4-b219-2bfa406b4efa)

Admin Login Page -> Admin Panel -> Agents -> Teams -> Select Team -> Members -> Select Agent -> Add -> Save

![image](https://github.com/user-attachments/assets/48664fb5-575f-4b5e-8499-cd6a97e446fd)

10. Configure Users (Create End Users)
   Admin Login Page -> Agent Panel -> Users -> Add User -> Enter email address -> Enter Name -> Create -> Save to notepad -> *Repeat to Create another End User*

![image](https://github.com/user-attachments/assets/24db842d-4f47-44d1-9c38-ffef62574004)
![image](https://github.com/user-attachments/assets/ffdabdd5-be72-4452-b41b-1a07fc632ea7)

11. Configure SLA (Create SLAs)
   Admin Login Page -> Admin Panel -> Manage -> SLA -> Add New SLA -> Enter Name -> Enter Grace Period -> Select Scheduale -> Add plan -> *Repeat to Create Two more SLAs for a total of Three SLAs*

12. Configure Help Topics (Create Help Topics)
    Admin Login Page -> Admin Panel -> Manage -> Help Topics -> Add New Help Topic -> Enter Name -> Choose Parent Topic -> Add Topic -> *Repeat to Create Four more Help Topics for a total of five Help Topics*

Congratulatons on finishing the modifications needed to use the osTicket software in a simulated real world application. Now you can move on to practice creating and solving tickets.


