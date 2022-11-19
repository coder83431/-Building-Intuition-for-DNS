<p align="center">
<img src="https://imgur.com/UV1HfFn.png" alt="osTicket logo"/>
</p>

<h1>Building Intuition For DNS- Prerequisites and Installation </h1>
This lab, we are inspecting DNS A-Records on a server. DNS A-Records will also be created and deleted as well. Concepts such as CNAME records and Root hints will be explored as well. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Command Line
- Microsoft Active Directory 

<h2>Operating Systems Used </h2>

- Windows 10</b> (version 22H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure 
- Two VM (virtual machienes) algready settedup and working: We will call them Client-1 and DC-1
- Microsoft Active Discovery installed on the DC-1 controller and promoted to a domamin controller
-The Client-1 vm is connected to the DC-1 VM which has Active Directory installed on it.

<h2>Installation Steps</h2>


<p>  
<img src = "https://imgur.com/1SgVJYL.png" " height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>

<p>Overview</p>

<p>
<img src = "https://imgur.com/3pGrBzA.png" " height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
 <p>

1. Connect into DC-1 as your domain admin account (mydomain.com\jane_admin). Additionally, connect into Client-1 as an admin (mydomain\jane_admin)


</p>                                                                                                    
   
   
   
<p>
<img src= "https://i.imgur.com/Pk3J6Rk.png" " height="80%" width="80%" alt="Disk Sanitization Steps" />
</p>

<p>
                                                                                                 
                                                                                                 
                                                                                                 
<br />

<p>
<img src="https://imgur.com/knE8v1T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
2. From Client-1 try to ping “mainframe” notice that it fails

</p>
<br />

<p>
<img src="https://i.imgur.com/PB1vmBe.png" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4. Install/ Enable IIS (Internet Information Services). Windows Control Pannel < Programs and Feautures
</p>
<br />

<p>
<img src="https://i.imgur.com/yt4ZPAk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5. Install "Microsoft Web Platform Installer".
      - Add "MySQL 5.5"
      - Add All Simple Versions Of X86PHP Up Until 7.3
</p>
<br />

<p>
<img src="https://i.imgur.com/8ob8uQq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6. Install osTicket v1.15.8.
</p>
<br />

<p>
<img src="https://i.imgur.com/SbhSS6V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7. Go Back To IIS, Sites->Default->osTicket, Double click PHP Manager, Enable PHP_imap.dll, Enable PHP_intl.dll, Enable PHP_opcache.dll
</p>
<br />

<p>
<img src="https://i.imgur.com/wVSvcC6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8. Rename File To OST-Config.PHP And Assign Permissions To File.
</p>
<br />

<p>
<img src="https://i.imgur.com/U0zZqC1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
9. Continue Setting Up OsTicket In Browser.
  -Name Help Desk
  -Add Default Email
</p>
<br />

<p>
<img src="https://i.imgur.com/IdTzZWd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
10. Download And Install HeidiSQL.
</p>
<br />

<p>
<img src="https://i.imgur.com/0LOpcLJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
11. OsTicket Is Ready. 
</p>
<br />
