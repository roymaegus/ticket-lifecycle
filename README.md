<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Virtual Machine of Windows 10
- Microsoft Remote Desktop
- IIS (Internet Information Service)


<h2>Installation Steps</h2>
<h4>Step 1 -  Download osTicket from the Installation Files Folder</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>Step 2 - Extract and copy “upload” folder to c:\inetpub\wwwroot</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>Step 3 - Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />
<p>

<h4>Reload IIS (Open IIS, Stop and Start the server)</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Go to sites -> Default -> osTicket</h2>
On the right, click “Browse *:80”
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />


<h2>Enable extensions</h2>
<h4>Go back to IIS, sites -> Default -> osTicket</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>Double-click PHP Manager</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>

<h4>Click “Enable or disable an extension”</h4>
<p>- Enable: php_imap.dll</p>
<p>- Enable: php_intl.dll</p>
<p>- Enable: php_opcache.dll</p>
<p>- Refresh the osTicket site in your browse, observe the changes</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Rename: ost-config.php</h2>
<h4>- From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>- From: To: C:\inetpub\wwwroot\osTicket\include\ost-config.php</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />


<h2>Assign Permissions</h2>
<h4>- Disable inheritance -> Remove All</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>- New Permissions -> Everyone -> All</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />


<h2>Continue Setting up osTicket in the browser (click Continue)</h2>
<h4>- Name Helpdesk</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>- Default email (receives email from customers)</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />


<h2>From the Installation Files, download and install HeidiSQL</h2>
<h4>- Open Heidi SQL</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>- Create a new session, root/Password1</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />
<h4>- Connect to the session</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />
<h4>- Create a database called “osTicket”</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />


<h2>Continue Setting up osticket in the browser</h2>
<h4>- MySQL Database: osTicket</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>- MySQL Username: root</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>- MySQL Password: Password1</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<h4>- Click “Install Now!”</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />


<h2>Congratulations, hopefully it is installed with no errors!</h2>
<h4>- Browse to your help desk login page: http://localhost/osTicket/scp/login.php</h4>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />
