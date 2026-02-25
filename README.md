<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Deploy a windows server VM in Azure
- Install Active Directory Domain Services (AD DS)
- Configure DNS and Networking
- Create and Manage Domain Objects

<h2>Deployment and Configuration Steps</h2>

<p>
<img width="1030" height="482" alt="image" src="https://github.com/user-attachments/assets/7c5db8ee-3127-4755-918b-b844f4de769d" />
</p>
<p>
In this phase we are deploying a windows server VM in Azure. Some steps tp get this started is:creating a virtual network, creating a subnet, configuring a network security group, and finally deploying the VM.
</p>
<br />

<p>
<img width="591" height="423" alt="image" src="https://github.com/user-attachments/assets/b5330351-f443-45f2-985b-90e416a1b8dc" />
</p>
<p>
In the next phase we will be installing active directory domain services. We can start by opening server manager, adding the role "Active directory domain services, after installation you'll click "promote this server to a domain controller", finally create a domain name and password.
</p>
<br />

<p>
<img width="631" height="446" alt="image" src="https://github.com/user-attachments/assets/4fb07573-4534-474a-9320-31e9e4000f39" />
</p>
<p>
In this step we will be configuring DNS and Networking. We can start by setting the DNS sever to itself and configure the Azure VNet DNS setting to point to the Domain Controller. Also make sure all neccesary ports are allowed.
</p>
<br />

<p>
  <img width="789" height="448" alt="image" src="https://github.com/user-attachments/assets/3194480b-3ba0-43f3-8236-5da3c08772e7" />
</p>
<p>
Finally in this step you will be creating and managing domain objects. Some of these objects are creating Organizational Units, creating users, creating groups, and applying group policy objects. 
</p>
<br />
