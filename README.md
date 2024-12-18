<img src=https://github.com/user-attachments/assets/5343bd46-54fb-4ee6-94c1-b4c0bad1cec3>
<br />
<br />

<h1>osTicket - Prerequisites and Installation</h1>

This section focuses on setting up the osTicket environment using an Azure-hosted Windows 10 VM. Key steps include installing required components like IIS, PHP, MySQL, and configuring osTicket to run on the VM. The goal is to provide the foundation for a fully operational ticketing system.<br />
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
- Install PHP Manager, Rewrite Module, PHP 7.3.8, Visual C++ Redistributable, and MySQL
- Set up the database using HeidiSQL
<br />
<br />

<h2>Installation Steps</h2>

1. Create an Azure Windows 10 Virtual Machine (VM):
  - Name: osticket-vm
  - Log into the virtual machine via Remote Desktop
    <img src=https://github.com/user-attachments/assets/1fee14b8-4f39-46e7-9bfb-647fe97b96f9>
<br />
<br />

2. Install necessary components:
  - Enable IIS with CGI support.<br />
      <img src=https://github.com/user-attachments/assets/2ef5c469-f022-45ee-b3e2-a4924e19d480>
  - Install PHP Manager, Rewrite Module, PHP 7.3.8, Visual C++ Redistributable, and MySQL<br />
      <img src=https://github.com/user-attachments/assets/86bd41b4-5408-48b9-8c4f-b48e7e2586c3>
<br />
<br />

3. Configure IIS:
  - Create the directory C:\PHP<br />
    <img src=https://github.com/user-attachments/assets/817df80b-ba57-4509-8e78-c71cd9c869ea>
  - Register PHP with C:\PHP\php-cgi.exe<br />
      <img src=https://github.com/user-attachments/assets/7bca8873-5a8b-44e3-aac7-3d896ad5df2d>
  - Reload IIS
<br />
<br />

4. Install osTicket:
  - Unzip osTicket-v1.15.8.zip into C:\inetpub\wwwroot and rename the folder to osTicket<br />
      <img src=https://github.com/user-attachments/assets/68e0ee3c-0607-4531-a55e-21e70565f93c>
  - Configure ost-config.php and assign permissions<br />
      <img src=https://github.com/user-attachments/assets/51d25d2c-0dc4-49c6-8499-f5217d319c37>
  - Complete the installation wizard in a browser<br />
      <img src=https://github.com/user-attachments/assets/363aec85-5a70-4a3c-9cbd-2772e5c334ba>
<br />
<br />

5. Set up the database using HeidiSQL:
  - Create a session with root/root credentials<br />
      <img src=https://github.com/user-attachments/assets/b86e87ff-a29e-4316-a46d-27e1da170a01>
  - Create a database called osTicket<br />
      <img src=https://github.com/user-attachments/assets/ee0ad552-7859-49b0-af85-a9c773e77b88>
<br />
<br />

6. Continue Setting up osTicket in the browser
  - MySQL Database: osTicket | MySQL Username: root | MySQL Password: root<br />
    <img src=https://github.com/user-attachments/assets/b538d49a-37ee-4552-a4a8-c2c77ddd58bb>
  - Click "Install Now"<br />
    <img src=https://github.com/user-attachments/assets/bba5abd5-13f3-4d17-8a66-1d27f9a392d7>
<br />
<br />
