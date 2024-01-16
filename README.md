<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> 

<h2>List of Prerequisites</h2>

- Create a resource group and Windows 10 virtual machine with 2CPUs
- Download installation files (https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)
- Open IIS as admin
- Register PHP
- Reload IIS
- Install OsTicket
- Reload OsTicket
- Go to sites -> default -> osTicket -> browse *:80
- Go to sites -> default -> osTicket -> Enable or disable an extension”
[X] Enable: php_imap.dll
[X] Enable: php_intl.dll
[X] Enable: php_opcache.dll
- Rename: from C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to C:\inetpub\wwwroot\osTicket\include\ost-config.php
- Go to ost-config.php -> properties -> security -> Disable inheritance -> Remove all -> New permissions -> Everyone -> All permissions
- Continue osTicket Setup in browser

<h2>Installation Steps</h2>

<p>
<img src=https://i.imgur.com/XEebItf.png height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install / Enable IIS in Windows VIA the Control Panel -> Programs -> Turn Windows Features on/off.
Select Internet Information Services -> Web Management Tools -> IIS Management Console	[X] IIS Management Console.
Next choose CGI and Common HTTP Features by selecting 
World Wide Web Services -> Application Development Features ->
[X] CGI
[X] Common HTTP Features.

</p>
<br />

<p>
<img src=https://i.imgur.com/fr9mWFk.png height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS -> Register PHP Manager -> Reload IIS by restarting the server
</p>
<br />

<p>
<img src=https://i.imgur.com/Sc2jM5k.png height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Setup Complete!
</p>
<br />
