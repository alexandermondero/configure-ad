<p align="center">
<img src="https://i.imgur.com/HANzbyW.png" alt="osTicket logo"/>
</p>

<h1>Active Directory</h1>
This tutorial outlines the deployment of Active Directory within a virtual machine using Microsoft Azure.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
- Windows Server 2022

<h2>Active Directory Deployment and Installation Steps</h2>

<p>
<img src="https://i.imgur.com/5QvVOuF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I first created 2 virtual machines in Microsoft Azure. The first virtual machine will be a domain controller named DC-1 and will be using Windows Server 2022. The second machine is a client on the network and will be named Client-1. Client-1 will be using Windows 10.
</p>
<br />

<p>
<img src="https://i.imgur.com/dN3JrVK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/uU7rexv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Daq5Idj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To ensure connectivity between the client and the domain controller I pinged DC-1 within the Client-1's virtual machine using Microsoft Remote Desktop. Since the ping request timed out at first, I went into the domain controller to enable ICMPv4 on the local windows firewall. After that was completed, I had a successful ping to DC-1.
</p>
<br />

<p>
<img src="https://i.imgur.com/nLtf8aD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, I installed Active Directory in the DC-1 virtual machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/3pQdini.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now that we have Active Directory installed I created an admin account named jane_admin.
</p>
<br />

<p>
<img src="https://i.imgur.com/3pQdini.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally, created users in the _EMPLOYEES folder that I created.
</p>
<br />
