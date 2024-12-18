<img src=https://github.com/user-attachments/assets/5343bd46-54fb-4ee6-94c1-b4c0bad1cec3>
<br />
<br />

<h1>osTicket - Prerequisites and Installation</h1>
This section focuses on setting up the osTicket environment using an Azure-hosted Windows 10 VM. Key steps include installing required components like IIS, PHP, MySQL, and configuring osTicket to run on the VM. The goal is to provide the foundation for a fully operational ticketing system..<br />
<br />
<br />

<h2>Environments and Technologies Used</h2>
  - Microsoft Azure (Virtual Machines)
  - Remote Desktop
  - osTicket
  - Internet Information Services (IIS)
<br />
<br />

<h2>Operating Systems Used </h2>
  - Windows 10</b> (21H2)
<br />
<br />

<h2>List of Prerequisites</h2>
- Install / Enable IIS in Windows WITH CGI
- Install PHP Manager, Rewrite Module, PHP 7.3.8, Visual C++ Redistributable, and MySQL.
- Set up the database using HeidiSQL:
<br />
<br />

<h2>Installation Steps</h2>
1. Create an Azure Windows 10 Virtual Machine (VM):
  - Name: osticket-vm
  - Specs: 4 vCPUs, Username: labuser, Password: osTicketPassword1!

2. Install necessary components:
  - Enable IIS with CGI support.
  - Install PHP Manager, Rewrite Module, PHP 7.3.8, Visual C++ Redistributable, and MySQL.

3. Configure IIS:
  - Register PHP with C:\PHP\php-cgi.exe.
  - Reload IIS.

4. Install osTicket:
  - Unzip osTicket-v1.15.8.zip into C:\inetpub\wwwroot and rename the folder to osTicket.
  - Configure ost-config.php and assign permissions.
  - Complete the installation wizard in a browser.

5. Set up the database using HeidiSQL:
  - Create a session with root/root credentials.
  - Create a database called osTicket.
