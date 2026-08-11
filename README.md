
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
<img <img width="1920" height="970" alt="Screenshot 2026-07-25 202658" src="https://github.com/user-attachments/assets/aedba7b6-0c71-4d15-863e-7c7b0c18e439" />
 

</p>
<p>
After logging into the Microsoft Azure portal, find and click on ‘Virtual Machines’ tab located to left in the navigation menu.
</p>
<br />

<p>
<img <img width="1920" height="968" alt="Screenshot 2026-07-25 203640" src="https://github.com/user-attachments/assets/32ade8d0-b771-4da2-9474-cf9dd79a867e" />

</p>
<p>
Click the ‘+ Add’ button to start creating a new Virtual Machine. The virtual machine is going to allow us to host and manage an isolated Windows environment for installing and configuring osTicket as a help desk ticketing system. 
</p>
<br />

<p>
<img <img width="1920" height="964" alt="Screenshot 2026-07-25 210447" src="https://github.com/user-attachments/assets/34f3c38a-6e16-45c1-971c-1252e9a13e18" />

</p>
<p>
Select your subscription to manage delpoyed resources and costs and create a new resource group. For this demo name it something easy to remember, like ‘osTicket Resource Group. The resource group was created to organize all componets of the osTicket deployment, including the virtual machine, storage, and networking resoures, making management easier.
</p>
<br />

<p>
<img <img width="1920" height="968" alt="Screenshot 2026-07-25 212609" src="https://github.com/user-attachments/assets/1e823092-b1ff-4839-99c0-fdff66662087" />
 

</p>
<p>
Set the Virtual Machine name as ‘osticket-vm’, then select and choose a region (like ‘East US’), and select an image (pick either ‘Windows 10/11’). Configuring these basic settings provides a familiar Windows environment used for configuring the osTicket help desk system and testing IT support tools. 

</p>
<br />

<p>
<img width="1142" height="576" alt="Screenshot 2026-08-11 015750" src="https://github.com/user-attachments/assets/b2ab6a46-9701-479d-b9aa-8a5896f3bce7" />
 

</p>
<p>
Choose a size for your Virtual Machine, with at least 2 virtual CPUs and at least 4 GB of RAM. This ensures your virtual machine runs smoothly and efficiently. 
</p>
<br />

<p>
<img width="1920" height="967" alt="Screenshot 2026-07-25 215608" src="https://github.com/user-attachments/assets/c56a1a74-2d87-43e6-8d78-7e65e50ec68b" />


</p>
<p>
Create a username and a strong password. Make a note of them for later access. 
</p>
<br />

<p>
<img width="1920" height="967" alt="Screenshot 2026-07-25 220533" src="https://github.com/user-attachments/assets/082c1872-13b5-4fcf-98e3-b715c8133f9f" />
 

</p>
<p>
Select which virtual machine network ports are accessible from the public internet. In this demo we will use RDP 3389, make sure the licensing boxed is checked confirming your are in Windows 10/11 compliance. 
</p>
<br />

<p>
<img width="1920" height="966" alt="Screenshot 2026-07-25 221330" src="https://github.com/user-attachments/assets/3cbfe6bd-71a4-47b0-88bc-1f7d18b60b64" />
 

</p>
<p>
Accept the default networking options or create a new virtual network. Click next to continue. 
</p>
<br />

<p>
<img width="1215" height="582" alt="Screenshot 2026-08-11 025833" src="https://github.com/user-attachments/assets/f0a65667-d320-43a8-afe0-e6080eb8ae00" />

 

</p>
<p>
Review your settings. If everything looks good, click ‘Create’ to launch your new Virtual Machine
</p>
<br />

<p>
<img width="1920" height="969" alt="Screenshot 2026-07-25 224129" src="https://github.com/user-attachments/assets/2328a48a-c650-4e15-85bf-b3d13620ac04" />
 

</p>
<p>
Once created, find your VM in the list. Note the status of the VM as actively running along with the public IP address for connecting later.
</p>
<br />

<p>
<img width="1387" height="973" alt="image" src="https://github.com/user-attachments/assets/faa79040-7808-485f-8751-0f3d5d47e808" />

</p>
<p>
Successfully logged into the osTicket admin dashboard for the first time after installation. This screenshot shows the main interface where tickets, users, and system settings are managed, confirming that osTicket was installed and configured correctly on the virtual machine.
</p>
<br />

<p>
<img width="1387" height="973" alt="image" src="https://github.com/user-attachments/assets/faa79040-7808-485f-8751-0f3d5d47e808" />

</p>
<p>
Successfully logged into the osTicket admin dashboard for the first time after installation. This screenshot shows the main interface where tickets, users, and system settings are managed, confirming that osTicket was installed and configured correctly on the virtual machine.
</p>
<br />

<p>
<img width="1387" height="973" alt="image" src="https://github.com/user-attachments/assets/faa79040-7808-485f-8751-0f3d5d47e808" />

</p>
<p>
Successfully logged into the osTicket admin dashboard for the first time after installation. This screenshot shows the main interface where tickets, users, and system settings are managed, confirming that osTicket was installed and configured correctly on the virtual machine.
</p>
<br />

<p>
<img width="1387" height="973" alt="image" src="https://github.com/user-attachments/assets/faa79040-7808-485f-8751-0f3d5d47e808" />

</p>
<p>
Successfully logged into the osTicket admin dashboard for the first time after installation. This screenshot shows the main interface where tickets, users, and system settings are managed, confirming that osTicket was installed and configured correctly on the virtual machine.
</p>
<br />

<p>
<img width="1387" height="973" alt="image" src="https://github.com/user-attachments/assets/faa79040-7808-485f-8751-0f3d5d47e808" />

</p>
<p>
Successfully logged into the osTicket admin dashboard for the first time after installation. This screenshot shows the main interface where tickets, users, and system settings are managed, confirming that osTicket was installed and configured correctly on the virtual machine.
</p>
<br />

<p>
<img width="1387" height="973" alt="image" src="https://github.com/user-attachments/assets/faa79040-7808-485f-8751-0f3d5d47e808" />

</p>
<p>
Successfully logged into the osTicket admin dashboard for the first time after installation. This screenshot shows the main interface where tickets, users, and system settings are managed, confirming that osTicket was installed and configured correctly on the virtual machine.
</p>
<br />
