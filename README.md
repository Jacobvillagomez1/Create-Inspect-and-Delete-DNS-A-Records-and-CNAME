# Create-Inspect-and-Delete-DNS-A-Records-and-CNAME
<p align="center">
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1>Create Inspect and Delete DNS A Records and CNAME</h1>
In this tutorial, going off On-premises Active Directory Deployed in the Cloud (Azure) [https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs] we will Create Inspect and Delete DNS A Records and CNAME in DC-1 VM . <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Active Directory Domain Services
- SEver Manager
- DNS Manager
- Command Prompt (Admin)


<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>High-Level Steps</h2>

- Log into Cilent-1 and DC-1 VM from [https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs]
- Go to DC-1 VM/ DNS Manager/ Forward Lookup Zones / Create A Record
- Open Cilent-1 VM ping A Record from DC-1
- Flush DNS and Display DNS on Cilent-1
- Open DC-1 VM and change the name of the A Record
- Open Cilent-1 VM Ping the new name of A Record
- Go back to DC-1 VM and create a CNAME
- Open Cilent-1 VM and Ping CNAME
- Go back to DC-1 VM and see Root Hints File


<h2>Actions and Observations</h2>

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/ab091d4c-4b4b-4034-9488-9f27b0d25530"/>
</p>
<p>
First we need to log back into Cilent-1 and DC-1 from [https://github.com/Jacobvillagomez1/Configuring-On-premises-Active-Directory-within-Azure-VMs] using Remote Desktop Connection. Copy the Public IP and log into the VM indivudally.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/bec682f8-0a86-44ff-bfdb-a083311cb3ee"/>
</p>
<p>
Next open Cilent-1 VM and search for Command Prompt in the search bar.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/d1a70743-8702-48d7-9a00-b46170cc8f56"/>
</p>
<p>
Once CMD loads you will see you are under jane_admin.
</p>
<br />


<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/2dd0e5ea-5405-432b-be96-7efd8a6efeae"/>
</p>
<p>
Then Open DC-1 VM and click Tools on the top right side of Server Manager. Then select DNS.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/9de400d1-86fe-406e-99c0-0b2d98e49862"/>
</p>
<p>
Next click the DC-1 File.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/255b41c0-10d4-4b3a-9c39-5b580aec51ce"/>
</p>
<p>
Then click Forward Lookup Zones.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/38e34221-4a9b-431f-95f1-d61ab2d9f8a8"/>
</p>
<p>
Next double click mydomain.com folder
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/76996c4c-101c-4a68-bb45-5abc4de56b87"/>
</p>
<p>
We are now going to create a New Host A Record. To do this right click anywhere on the screen and click New Host (A or AAAA)...
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/db33009c-73c2-46b3-a7e1-55fbfce70897"/>
</p>
<p>
Now in the Name section we can type mainframe and for IP Address we can type the same IP as dc-1 IP which is 10.0.0.4. Once those are both typed in click add host.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/e75975e3-8c5e-40fd-a8e6-355318e4e679"/>
</p>
<p>
Once you added the host click ok.
</p>
<br />

<p>
<img src="https://github.com/Jacobvillagomez1/Create-Inspect-and-Delete-DNS-A-Records-and-CNAME/assets/143027686/c99db801-f0d9-4bd8-bbd7-d39e4a15a9e6"/>
</p>
<p>
Then click done to finish the process.
</p>
<br />

