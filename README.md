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



1. Today, we are going to give a fast and simple tutorial for configuring OS Ticket. Our first step is to create a virtual environment in Microsoft Azure. Follow the parameters below to configure your virtual machine.
 
- Windows 10, 4 vCPUs
- Name: osticket-vm
- Username: labuser
- Password: osTicketPassword1!



![image](https://github.com/user-attachments/assets/7f7ebc56-e770-4aaf-9a0b-3817761727dc)

2. Now we remote desktop into the (VM) virtual machine by using the username or password from step 1
- Username: labuser
- Password: osTicketPassword1!



![image](https://github.com/user-attachments/assets/02f017e2-793d-4d9a-9bd9-67c3e4abe687)

3. Once the (VM) boots up head to the control panel settings and look for the programs tab. Within the tab, you will find a list of programs but we are only searching for {IIS & CGI}


![image](https://github.com/user-attachments/assets/2fd7ea20-3247-4295-93bb-52774d40deb0)

4. Turn Windows features on or off > Internet Information Services > World Wide Web > Application Development features > CGI

![image](https://github.com/user-attachments/assets/f1cc7a35-aeff-4a9d-878d-d1a20d9a103d)

5. Next, download/install PHP Manager & Rewrite Module 

Here is the [link](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)

6. Once the download is completed, we will create a folder from the file explorer tab. The new folder will be in the (C:) drive and named PHP. 

![image](https://github.com/user-attachments/assets/af8132a7-3b01-4d77-a9ba-9eb04cafab93)

![image](https://github.com/user-attachments/assets/c8b7e497-10af-4572-b23a-ab52eb98805a)

7. We will unzip PHP 7.3.8 into the “C:\PHP” folder. In non-technical terms, we extract the content from one file to another. 

![image](https://github.com/user-attachments/assets/7ebd3087-c18c-401e-bef2-eac92ef16bb8)

8. Download & Install VC redist.x86.exe. 

![image](https://github.com/user-attachments/assets/1f5bd3f6-52f7-42dc-bbad-6b622b3276e3)


9. Install MySQL 5.5.62 (follow the steps provided below)

- Typical Setup
- Launch Configuration Wizard (after installation)
- Standard Configuration

![image](https://github.com/user-attachments/assets/31415b2b-77e8-4914-8bca-9b0766ebe8f5)
![image](https://github.com/user-attachments/assets/24498a28-eeef-42b6-9af3-774840a70c54)
![image](https://github.com/user-attachments/assets/f61fdb68-7f47-4d72-919e-af64147d9827)

10. Open IIS as an Admin/Register PHP from within IIS, follow the below example to reload IIS.

Open PHP Manager->Register new PHP ENTER: C:->PHP->php-cgi.exe. Now restart the server.
Reload IIS (Open IIS, Stop and Start the server)

![image](https://github.com/user-attachments/assets/f5fdb55f-0f4c-4429-a9f8-3382a495ddc2)

11. Install osTicket v1.15.8 / unzip osTicket v1.15.8. and copy the “upload” folder into “c:\inetpub\wwwroot” Once completed restart the server.
![image](https://github.com/user-attachments/assets/bd7b5170-c03a-45a8-a087-29cc263f9127)
![image](https://github.com/user-attachments/assets/324c8f37-55a4-4605-881d-aa4a062d46d3)

12. Once the server has been restarted, we can download the necessary extension to get OS Ticket to run. Foll0w the below steps in (IIS) to enable the extensions.

IIS > OS Ticket > PHP Manager>Enable extensions: php_opcache.dil, phpImap.dll, phpintl.dll. Refresh the osTicket tab in your Internet Explorer.

![image](https://github.com/user-attachments/assets/808f107c-9b32-4556-b36b-7051a08fb53c)

13. Next rename the file "Ostsampleconfig" to "Ost-config". Follow the example below to find the necessary file. 

Browse > wwwroot > include > Ostsampleconfig

![image](https://github.com/user-attachments/assets/c572d85c-89e4-476b-9796-ecf9fc89d54d)

14. In "ost-config" we will follow the below example to remove permissions.

Open properties > security > advanced > disable inheritance > remove all permissions > then select everyone & apply

![image](https://github.com/user-attachments/assets/cb8795a4-1b4b-4f7d-9903-a9638f7a2ce8)

15. Download/install heidi from this [link](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6).

![image](https://github.com/user-attachments/assets/ef9a8a61-c973-41be-8a7b-23331bcdd606)

Now we get to the fun part, open OS Ticket in your browser and begin to fill out the installation requirments.


