# OS-Ticket-Configuration-
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites]https://www.youtube.com/watch?v=fWX1Lj-rOa0

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Installation Files https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6

<h2>Installation Steps</h2>

- Create Virtual Machine in Azure
- Install/Enable IIS in Windows With CGI
- Download and install PHP Manager for IIS
- Download and install the Rewrite Module
- Create the directory C:\PHP
- Download PHP 7.3.8
- Download and install VC_redist.x86.exe.
- Download and install MySQL 5.5.62

# OS Ticket Installation Steps



![image](https://github.com/user-attachments/assets/df01ab9f-44ad-4fa4-b27c-7a5bfe4bc0b1)



1. Today we are going to give a fast and simple tutorial for configuring OS Ticket our first step is to create a virtual environment in Microsoft Azure. Follow the parameters below to configure your virtual machine.
 
- Windows 10, 4 vCPUs
- Name: osticket-vm
- Username: labuser
- Password: osTicketPassword1!



![image](https://github.com/user-attachments/assets/7f7ebc56-e770-4aaf-9a0b-3817761727dc)

2. Now we remote desktop into the (VM) virtual machine by using the username or password from step 1
- Username: labuser
- Password: osTicketPassword1!



![image](https://github.com/user-attachments/assets/02f017e2-793d-4d9a-9bd9-67c3e4abe687)

3. Once the (VM) boots up head to the control panel settings and look for the programs tab Within the tab you will find a list of programs but we are only searching for {IIS & CGI}


![image](https://github.com/user-attachments/assets/2fd7ea20-3247-4295-93bb-52774d40deb0)

4. Turn Windows features on or off-> Internet Information Services->World Wide Web->Application Development features->CGI

![image](https://github.com/user-attachments/assets/f1cc7a35-aeff-4a9d-878d-d1a20d9a103d)

5. Next, download/install PHP Manager & Rewrite Module 

Here is the [link](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)

6. Once the download is completed, we will create a folder from the file explorer tab. The new folder will be located in the (C :) drive and named PHP. 

![image](https://github.com/user-attachments/assets/af8132a7-3b01-4d77-a9ba-9eb04cafab93)

![image](https://github.com/user-attachments/assets/c8b7e497-10af-4572-b23a-ab52eb98805a)


<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
