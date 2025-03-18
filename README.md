<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Network File Shares and Permissions</h1>
This tutorial outlines setting permissions on files to give or deny access to files.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/J414ouX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  Created three folders in Domain Controller's C:\ drive called "read-access", "write-access", and "no-access". By sharing the folder we are able to set permissions for the contents of each folder
</p>
<p>

</p>
<br />

<p>
<img src="https://i.imgur.com/Z8h8XE5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Setting read only permissions for the "read-access" folder. Domain Users will be able to read the contents of "read-access" folder but will not be able to create or change any of the contents. 
</p>
<br />

<p>
<img src="https://i.imgur.com/o25fO8K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Tried creating a text document in the "read-access" folder from a Domain User in the Client computer and it was denied since the permissions are set to read only.
</p>
<br />
