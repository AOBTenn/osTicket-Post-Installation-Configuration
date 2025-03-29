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
 <p> 
</p>

![image](https://github.com/user-attachments/assets/b8a0a16a-18d9-492d-93e3-b9eca5669332)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/92aa8792-6bd6-48bd-a8f8-478b53b88f16)
 <p> 
</p>

2. Acknowledge Agent vs Admin panel  
 <p> 
</p>

Admin webpage -> Sign in as admin -> Admin panel -> Agent panel

![image](https://github.com/user-attachments/assets/7eeface6-2228-4786-b4e5-a095f33507bc)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/486071fe-2ba4-4c6a-9591-871231976ed5)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/6403fbde-143d-4a5e-8820-626e80fcf40d)
 <p> 
</p>

3. Configure Roles
 <p> 
</p>

Admin Login Page -> Admin Panel -> Agents -> Roles -> Add New Role -> Type "Supreme Admin" -> Permissions -> Check all the boxes -> Add Role
 <p> 
</p>

![image](https://github.com/user-attachments/assets/c88cd158-5ee3-4221-b331-a223e99ed207)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/4b67e5ab-95e4-432a-ac01-07187479cd36)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/f3e3a003-1e10-45bd-b172-06f82f4dbbe2)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/a6874e44-fa6c-4664-8796-ea84b55183dc)
 <p> 
</p>

4. Configure Departments
 <p> 
</p>

Admin Login Page -> Admin Panel -> Agents -> Departments -> Add New Department -> For Parent select "Top Level Department" -> For Name type "SysAdmins" -> Create
 <p> 
</p>

![image](https://github.com/user-attachments/assets/1653c26d-e825-4116-9a2e-48dd5394947b)
 <p> 
</p>

Admin Login Page -> Admin Panel -> Agents (in the top row, not second row) -> Departments -> Maintenance -> Delete -> Save
 <p> 
</p>

![image](https://github.com/user-attachments/assets/1cca647a-cf5d-469b-b643-3a72b7f70c1d)
 <p> 
</p>

6. Configure Teams
 <p> 
</p>

Ad <p> 
</p>
min Login Page -> Admin Panel -> Agents -> Teams -> Add New Team -> For Name type "Online Banking" -> Create

![image](https://github.com/user-attachments/assets/39d4d901-f4bf-41c7-b36e-9b72adb4e456)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/53dee0ae-9b68-4c2a-ba5a-0da2a27bd8cb)
 <p> 
</p>

7. Allow anyone to create tickets
 <p> 
</p>

Admin Login Page -> Admin Panel -> Settings -> Users -> *Note* Make sure the box next to "Registration Required" is unchecked -> Save 
 <p> 
</p>

![image](https://github.com/user-attachments/assets/ec467781-1996-4de4-8f85-7749c9d2f0dd)
 <p> 
</p>

8. Configure Agents (Create workers)
 <p> 
</p>

Admin Login Page -> Admin Panel -> Agents -> Add New Agents -> Enter Name -> Enter Email address -> Enter Username -> Set Password -> Uncheck top box -> Enter Password in both boxes -> Unckeck bottom box -> Update -> Access tab -> For Primary dept. "Support/SysAdmins" -> For Roles "Supreme Admin" -> Teams tab -> Online Banking -> Create -> Save to notepad
 <p> 
</p>

![image](https://github.com/user-attachments/assets/c29ec573-2224-4408-bb8c-8ef28601419e)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/1307b1a9-750e-4391-9ac0-1ac213ae6cf8)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/66b866cf-fc1b-4b05-bff3-03e78c25d815)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/5376e259-6518-4487-aa66-0d35bc0560e3)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/43bc501d-a4cf-414e-92db-042082c5bb29)
 <p> 
</p>

Admin Login Page -> Admin Panel -> Agents -> Add New Agents -> Enter Name -> Enter Email address -> Enter Username -> Set Password -> Uncheck top box -> Enter Password in both boxes -> Unckeck bottom box -> Update -> Access tab -> For Primary dept. "Support" -> For Roles "All Access" -> Create -> Save to notepad
 <p> 
</p>

![image](https://github.com/user-attachments/assets/7ad97cf2-07ba-4af7-8547-32cf2184d34d)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/09ea5d5c-1c36-4abb-987d-3be56992617f)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/b68a12a6-5b2c-4e4d-80d4-25be9d7516bf)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/4b5a1c04-e914-4864-b107-82278b0c44d3)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/3c6f3612-f84b-416c-be4e-4e2748ae6fc2)
 <p> 
</p>

9. Re-Configure Teams
<p> 
</p>

Admin Login Page -> Admin Panel -> Agents -> Teams -> Select Team -> Members -> Select Agent -> Add -> Save
 <p> 
</p>

![image](https://github.com/user-attachments/assets/cb3705b1-2599-42c4-b219-2bfa406b4efa)
 <p> 
</p>

Admin Login Page -> Admin Panel -> Agents -> Teams -> Select Team -> Members -> Select Agent -> Add -> Save
 <p> 
</p>

![image](https://github.com/user-attachments/assets/48664fb5-575f-4b5e-8499-cd6a97e446fd)
 <p> 
</p>

10. Configure Users (Create End Users)
 <p> 
</p>

Admin Login Page -> Agent Panel -> Users -> Add User -> Enter email address -> Enter Name -> Create -> Save to notepad -> *Repeat to Create another End User*
 <p> 
</p>

![image](https://github.com/user-attachments/assets/24db842d-4f47-44d1-9c38-ffef62574004)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/ffdabdd5-be72-4452-b41b-1a07fc632ea7)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/bb08d14f-46ba-4042-b52d-fd1b7937f23e)
 <p> 
</p>

11. Configure SLA (Create SLAs)
 <p> 
</p>

Admin Login Page -> Admin Panel -> Manage -> SLA -> Add New SLA -> Enter Name -> Enter Grace Period -> Select Scheduale -> Add plan -> *Repeat to Create Two more SLAs for a total of Three SLAs*
 <p> 
</p>

![image](https://github.com/user-attachments/assets/4b794586-a4df-42a7-9313-c21acb51b4f4)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/ba5ea2ff-0319-44c2-ba70-9dc250f2538c)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/76bfc716-7bd2-45ee-8aaa-5ed5abf20954)
 <p> 
</p>

12. Configure Help Topics (Create Help Topics)
 <p> 
</p>

Admin Login Page -> Admin Panel -> Manage -> Help Topics -> Add New Help Topic -> Enter Name -> Choose Parent Topic -> Add Topic -> *Repeat to Create Four more Help Topics for a total of five Help Topics*
 <p> 
</p>

![image](https://github.com/user-attachments/assets/0451205c-d3d8-42c7-9a1e-836f60a3bd59)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/30a30e27-a221-47aa-bb8c-3be8fe0e4cda)
 <p> 
</p>

![image](https://github.com/user-attachments/assets/ca037cab-2be9-4e4d-9e0d-060a8e44524b)
 <p> 
</p>

Congratulatons on finishing the modifications needed to use the osTicket software in a simulated real world application. Now you can move on to practice creating and solving tickets.


