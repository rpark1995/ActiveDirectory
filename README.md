<h1>Active Directory Home Lab - Add Roles and Users</h1>

<h2>Description</h2>
In this lab, I am going to demonstrate how to add roles and features in Active Directory. The two roles I will add are Active Directory Domain Services and DNS (Domain Name Server).
<br />


<h2>Software Used</h2>

- <b>Virtual VM VirtualBox</b> 

<h2>Operating Systems Used </h2>

- <b>Windows Server 2019</b>

<h2>Program walk-through:</h2>

<p align="center">
First, open Server Manager and click on the Manage option in the upper-right corner. Under the dropdown menu, click on 'Add Roles and Features'. Alternatively, you can simply click on 'Add Roles and Features' on the home page. : <br />
<img src="https://i.imgur.com/UuRYCvf.png" height="80%" width="80%" alt="Change System Name"/>
<br />
<br />
After clicking on 'Add Roles and Features', a box will open and display the 'Before You Begin' part. Click on 'Next'. This will then take you to the 'Installation Type' part. You want to choose 'Role-based or feature-based installation' to add a role or feature. This option will be chosen most of the time. Click on 'Next'. :<br />
<img src="https://i.imgur.com/B8OsKiK.png" height="80%" width="80%" alt="Change System Name"/>
<br />
<br />
Now you are in the 'Server Selection' part. This portion displays the virtual machine's information, like name, IP address, and Operating System. There is nothing that needs to be done so click on 'Next'. :  <br/>
<img src="https://i.imgur.com/KrfpYiw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The next part is 'Server Roles', where you can select roles for your virtual machine. The first checkbox you want to select is 'Active Directory Domain Services'. Another box will open and display all the features that are included with the Active Directory Domain Services. Click on 'Add Features'. Next, select the 'DNS' checkbox. Again, another box will open, displaying all the features, and click on 'Add features'. Now, you have both Domain Services and DNS roles added to your virtual machine. Click on 'Next'. : <br/>
<img src="https://i.imgur.com/DUalFyD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
This will now take you to 'Features'. You do not need to add any additional features in this section so click on 'Next'. :  <br/>
<img src="https://i.imgur.com/f8C0Xv5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The next two sections ('AD DS' and 'DNS Server') do not require any action so click on next for both sections. This will then take you to the 'Confirmation' section, which displays the roles you just added and want to install. First, check the checkbox next to 'Restart the destination server automatically if required'. Then, click on 'Install' and wait for the installation process to complete. This will take some time and the system will automatically restart. :  <br/>
<img src="https://i.imgur.com/D80zygd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once the installation is complete, you will see a notification on the flag icon (located upper-right corner). Click on that icon and a dropdown menu will appear. Select 'Promote this server to a domain controller', which will allow you to configure the server. :  <br/>
<img src="https://i.imgur.com/zkhZGUo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
After clicking on 'Promote this server to a domain controller', a box should open. This will take you to 'Deployment Configuration'. In this section, select 'Add a new forest'. Next, type the root domain name in the textbox for the new forest. In my case, I used 'mydomain.com'. :  <br/>
<img src="https://i.imgur.com/XxnC5g3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
In the 'Domain Controller Options' section, type in a password for the Directory Services Restore Mode. Use a password that is easy to remember. This is necessary if you want to restore the AD from backup. Click 'Next'. :  <br/>
<img src="https://i.imgur.com/M4OJvvH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
In 'Additional Options', the NET BIOS name will be verified. Nothing needs to be done, so click on 'Next' to accept the name. :  <br/>
<img src="https://i.imgur.com/IY4AdO9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br />
<br />
In 'Paths', this will display the default database, log files, and SYSVOL folders. Again, othing needs to be done, so click on 'Next'. :  <br/>
<img src="https://i.imgur.com/MkxB76r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <br />
<br />
The wizard will perform some prerequisite checks to ensure AD can be installed on the server. In this case, the server passed all the checks. There were a few warnings, but that is normal and ok as long as the test passed. Click 'Install' to configure AD on the server. The machine will restart automatically. :
<img src="https://i.imgur.com/0cuunFV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
Once restarted, you will need to log in with the domain administrator account. Notice how the username displays 'MYDOMAIN\Administrator'. You will log in using the password you created while creating a virtual machine. :  <br/>
<img src="https://i.imgur.com/PTf1YhN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
   <br/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
