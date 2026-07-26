
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This project shows how I set up a web-based help desk system (osTicket) using a virtual computer in the cloud.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)
- PHP
- MySQL
- osTicket

<h2>Operating Systems Used </h2>

- Windows 11</b> 

<h2>List of Prerequisites</h2>

- Access to Microsoft Azure: You need to be able to create and manage virtual machines.
- Basic Understanding of Virtual Machines: Knowing how to set up a Windows 10 VM with appropriate specs (at least 2 vCPUs and 8GB RAM).
- Familiarity with Remote Desktop (RDP): Required to connect to your VM.
- Basic Windows Navigation Skills: To install software, browse files, and change settings within the VM.
  

<h2>Installation Steps</h2>

<p>
<img <img width="1920" height="970" alt="Screenshot 2026-07-25 201707" src="https://github.com/user-attachments/assets/cf66c4a8-9f47-4f85-97e4-0e9e62a6fb3d" />

</p>
<p>
Open the Microsoft Azure Portal by entering https://portal.azure.com in your web browser. This is the main website used to sign in and manage Azure cloud services.
</p>
<br />

<p>
<img <img width="1920" height="970" alt="Screenshot 2026-07-25 202021" src="https://github.com/user-attachments/assets/17773fa8-3eda-485a-a05d-e9aa815db083" />

</p>
<p>
Sign in using your Microsoft account credentials. If you dont have an account, select Create one to register a new Microsoft account before proceeding to the Azure portal.
</p>
<br />

<p>
<img width="1067" height="1033" alt="image" src="https://github.com/user-attachments/assets/0427ae32-0824-4e35-a50f-168cf849b86f" />

</p>
<p>
Configured PHP within IIS using the PHP Manager extension. This screenshot shows the PHP Manager window after successfully registering the PHP executable located in C:\PHP. This setup enables the web server to process PHP scripts, which is required for running applications like osTicket.
</p>
<br />

<p>
<img width="1658" height="977" alt="image" src="https://github.com/user-attachments/assets/5294bc27-cd52-4628-a67f-4398d98a2107" />

</p>
<p>
Accessed the osTicket web installer initial setup screen through the web browser on the virtual machine. This screenshot shows the beginning of the installation process, where core help desk details, admin credentials, and database settings are entered to configure and deploy the osTicket ticketing system.
</p>
<br />

<p>
<img width="1167" height="738" alt="image" src="https://github.com/user-attachments/assets/70ef0cd3-6e8f-4c62-b941-4fd8cad85f8d" />

</p>
<p>
Created a new MySQL database named “osTicket” using HeidiSQL, as shown in this screenshot. This step establishes a dedicated database to store all ticketing system data, user accounts, and configurations required for the osTicket application to operate.
</p>
<br />

<p>
<img width="1387" height="973" alt="image" src="https://github.com/user-attachments/assets/faa79040-7808-485f-8751-0f3d5d47e808" />

</p>
<p>
Successfully logged into the osTicket admin dashboard for the first time after installation. This screenshot shows the main interface where tickets, users, and system settings are managed, confirming that osTicket was installed and configured correctly on the virtual machine.
</p>
<br />


