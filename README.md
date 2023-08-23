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

