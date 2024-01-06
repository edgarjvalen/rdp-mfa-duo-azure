<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Setting Up MFA and Protecting RDP Using Duo (Server 2022)</h1>

<h2>Description</h2>
In this lab, we'll create two VMs in the same VNET—one as a Domain Controller (DC) with a static IP offering Active Directory services, and the other as a Client machine. The client will join the domain, and its DNS settings will be configured to use the DC as the primary DNS server. The project involves establishing an Active Directory system for centralized user credential oversight and network traffic management. By routing all internet traffic through the main server (Active Directory) via organization devices (Clients), administrators can monitor network activity and detect suspicious logs. Additionally, the project includes a PowerShell script to generate 1,000 users and showcases a device within the organization's domain, ensuring efficient management of user credentials and network traffic.
<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Project Diagram</h2>

<p align="center">
<img src="https://i.imgur.com/BcRNcBi.png" height="80%" width="80%" alt="9"/><br />
</p>

<h2>Step 1: Setup</h2>

First, using Azure, create a Resource Group. Now, create 2 Virtual Machines(VMs). One will be the Domain Controller and the other will be the Client. To create the Domain Controller, give the VM a name as well as assign it to the Resource Group created before. 

<img src="https://i.imgur.com/uYfHMQG.png" height="70%" width="70%" alt="9"/><br />

Now for the image use Windows Server 2022. It is recommended for the size to use 2 vcpus.

<img src="https://i.imgur.com/FNoA7m0.png" height="70%" width="70%" alt="9"/><br />

Give the admin log in credentials that can be remembered or just write them down in notepad. Now, click "Next" until reaching the "Networking" tab. Take note of the "Virtual Network" created. This will be important when creating the Client VM. Check the box under Licensing then "Review and create" the VM.

<h2>Conclusion</h2>

Active Directory is crucial for organizations to effectively control their network traffic and prevent unauthorized access to internal networks or leakage of information to external parties. Understanding and learning about Active Directory is a fundamental principle for all IT professionals, regardless of their specific roles. Hope you found this blog both informative and valuable.

