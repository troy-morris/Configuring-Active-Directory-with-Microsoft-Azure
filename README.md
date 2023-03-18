<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of Active Directory within Azure Virtual Machines.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Configuring Virtual Machines (Domain Controller and Client)
- Install Active Directory Domain Services and Add Client VM to Domain
- Create Admin and Normal accounts in Active Directory Users and Computers
- Setup Remote Desktop for Non-Admin users on Client VM

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/a43FW3E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/MzywsdV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In these photos you can see I have created a Virtual Machine for the Domain Controller and the Client "pc" to be used in this demo. Both VM's are configure to be on the same Virtual Network within Azure.
</p>
<br />

<p>
<img src="https://i.imgur.com/ZT2r1TS.png"  height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here we have Active Directory Domain Services installed and our Domain configured for our Client VM to join.
</p>
<br />

<p>
<img src="https://i.imgur.com/wVcvYuj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/Rrdr9AV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
For this demo, I created one Admin account and used a script to create 100 User accounts with randomly generated names.
</p>
<br />

<p>
<img src="https://i.imgur.com/UbdOHVo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/o1Wo9Er.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In these last two photos I have setup Remote Desktop access to the Client VM for users on the Domain. Also, I have given permission to non-Admin accounts to have remote access to the Client VM.
