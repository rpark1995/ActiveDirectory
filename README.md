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
First, open Server Manager and click on the Manage option in the upper-right corner. Under the dropdown menu, click on 'Add Roles and Features'. Alternatively, you can simply click on 'Add Roles and Features' on the home page.: <br />
<img src="https://i.imgur.com/UuRYCvf.png" height="80%" width="80%" alt="Change System Name"/>
<br />
After clicking on 'Add Roles and Features', a box will open and display the 'Before You Begin' part. Click on 'Next'. This will then take you to the 'Installation Type' part. You want to choose 'Role-based or feature-based installation' to add a role or feature. This option will be chosen most of the time. Click on 'Next'.:<br />
<img src="https://i.imgur.com/B8OsKiK.png" height="80%" width="80%" alt="Change System Name"/>
<br />
<br />
Now you are in the 'Server Selection' part. This portion displays the virtual machine's information, like name, IP address, and Operating System. There is nothing that needs to be done so click on 'Next'.:  <br/>
<img src="https://i.imgur.com/KrfpYiw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The next part is 'Server Roles', where you can select roles for your virtual machine. The first checkbox you want to select is 'Active Directory Domain Services'. Another box will open and display all the features that are included with the Active Directory Domain Services. Click on 'Add Features'. Next, select the 'DNS' checkbox. Again, another box will open, displaying all the features, and click on 'Add features'. Now, you have both Domain Services and DNS features added to your virtual machine. Click on 'Next'.: <br/>
<img src="https://i.imgur.com/DUalFyD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
