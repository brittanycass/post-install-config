
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

### Table of Contents
1. [Configure Roles](#configure-roles)
2. [Configure Departments](#configure-departments)
3. [Configure Teams](#configure-teams)
4. [Allow Anyone to Create Tickets](#allow-anyone-to-create-tickets)
5. [Configure Agents](#configure-agents)
6. [Configure Users](#configure-users)
7. [Configure SLA](#configure-sla)
8. [Configure Help Topics](#configure-help-topics)

### 1. Configure Roles
- **Log in:** `Use the credentials you create during prereq & configuration`

![image](https://github.com/user-attachments/assets/912cf994-6c04-45a1-aebb-2e0f56c5c064)

<p </p>


- **Navigate to:** `Admin Panel -> Agents -> Roles`
- **Create Role:** `Supreme Admin`
<p align="center"><img src="https://i.imgur.com/dMCodFe.png"/></p> 
<p align="center"><img src="https://i.imgur.com/CjaY7Q4.png"/></p>

- **Click:** `Permissions`
- **Tickets:** `Check all boxes`
- **Tasks:** `Check all boxes`
- **Knowledges:** `Check all boxes`
- **Click:** `Add Role`
<p align="center"><img src="https://i.imgur.com/O41mfcc.png"/></p>
<p align="center"><img src="https://i.imgur.com/EfgwCIK.png"/></p>
<p align="center"><img src="https://i.imgur.com/K6S8yYM.png"/></p>

### 2. Configure Departments
- **Navigate to:** `Admin Panel -> Agents -> Departments`
- **Create Department:** `System Administrators`
 <p align="center"><img src="https://i.imgur.com/fqROXPN.png"/></p>

 ![image](https://github.com/user-attachments/assets/f7372462-49d3-45bd-9116-fc9da34493ca)


![image](https://github.com/user-attachments/assets/2225695a-7f71-4048-903c-4771cb1ad861)

</p>

### 3. Configure Teams
- **Navigate to:** `Admin Panel -> Agents -> Teams`
- **Create Teams:**
  - `Level I Support`
  - `Level II Support`
<p align="center"><img src="https://i.imgur.com/ZEhlAPW.png"/></p>

![image](https://github.com/user-attachments/assets/83e7924c-16c7-4e5d-81ff-3c6c41d36da9)


### 4. Allow Anyone to Create Tickets
- **Navigate to:** `Admin Panel -> Settings -> User Settings`
- **Set Registration Required:** `Uncheck Require registration and login to create tickets`
  
  ![image](https://github.com/user-attachments/assets/a1a5929e-2042-495d-b095-7bc730b7409e)

 </p>

### 5. Configure Agents (Workers)
- **Navigate to:** `Admin Panel -> Agents -> Add New`
- **Add Agents:** `Jane Doe`
- - Name: `Jane Doe`
  - Email Address: `jane.doe@osticket.com`
  - Username: `jane.doe`
  - Click: `Set Password`
  - Uncheck: `Send the agent a password reset email`
  - Password: *`Your osTicket Login Password`*
  - Uncheck: `Require password change at next login`
  - Click: `Set`

    ![image](https://github.com/user-attachments/assets/d7e57ad4-8cfd-4768-bf15-8abc799a3405)

    
![image](https://github.com/user-attachments/assets/42318123-d930-495a-8eda-ad50eba7402f)

- **Go to:** `Access Tab`
  - Primary Department
  - Department: `System Administrators`
  - Role: `Supreme Admin`
  
    ![image](https://github.com/user-attachments/assets/c7aed269-9b20-498b-9389-829d3132e45b)

 
-  **Go to:** `Permissions Tab`
   - Check ALL boxes
   - 
     ![image](https://github.com/user-attachments/assets/57afd8e6-2c12-496e-ac84-401f377e5fcc)


-  **Go to:** `Teams Tab`
   - Assigned Teams: `Level II Support`
   - Click: `Create`

   ![image](https://github.com/user-attachments/assets/bf597264-8c45-44e4-ba2e-e6940457462b)



### 6. Configure Users (Customers)
- **Navigate to:** `Agent Panel -> Users -> Add New`
- **Add Users:** `Karen` & `Ken`
- Email Address: `Karen@osticket.com`
- Full Name: `Karen Karen`
- Click: `Add User
  <p align="center"><img src="https://i.imgur.com/7vN2ud9.png"/></p>
  <p align="center"><img src="https://i.imgur.com/2JUxLrt.png"/></p>

:memo: **Note:** Repeat the same steps for Ken


### 7. Configure SLA
- **Navigate to:** `Admin Panel -> Manage -> SLA`
- **Create SLA Plans:**
  - `Sev-A (1 hour, 24/7)`
  - `Sev-B (4 hours, 24/7)`
  - `Sev-C (8 hours, business hours)`
<p align="center"><img src="https://i.imgur.com/nXCMQsK.png"/></p> 
<p align="center"><img src="https://i.imgur.com/rR1VM3s.png"/></p>

### 8. Configure Help Topics
- **Navigate to:** `Admin Panel -> Manage -> Help Topics`
- **Create Help Topics:**
  - `Business Critical Outage`
  - `Personal Computer Issues`
  - `Equipment Request`
  - `Password Reset`
  <p align="center"><img src="https://i.imgur.com/ZGr9N3z.png"/></p>

### :bulb: **Tips:**
- Ensure each setup step is correctly saved before moving to the next step.
- Consult the osTicket [official documentation](https://docs.osticket.com/) for further details.


