<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Azure Virtual Machine Set-up to Facilitate Inspecting Traffic Between VMs</h1>
In this tutorial, we will deploy virtual machines to allow for the eventual inspection of network traffic between VMs. A Microsoft Azure account/subscription will be required. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10 (22H2)
- Ubuntu Server 24.04

<h2>High-Level Steps</h2>

- Create a Resource Group
- Create a Windows 10 Virtual Machine
- Create a Virtual Network and Subnet
- Create a Linux Ubuntu Virtual machine

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/QEC1rPQ.png" height="80%" width="80%" alt="RG Creation"/>
</p>
<p>
Go to portal.azure.com. Either select "Resource Group" from Azure Services or begin typing "Resource Group" in the search bar at the top. Click "+ Create." Give your Resource Group a name, and select the region in which you want your Resource Group to reside. Select "Review + create," and allow sufficient time for its creation (notice the notification bell at that top of the page). This Resource Group will contain the following resources.
</p>
<br />

<p>
<img src="https://i.imgur.com/Zsu0Zbe.png" height="80%" width="80%" alt="VM Creation with Region"/>
<img src="https://i.imgur.com/8RwZS3K.png" height="80%" width="80%" alt="VM Creation by Type"/>  
</p>
<p>
While still in Azure, select "Virtual Machine" from Azure Services, if shown, or begin typing "Virtual Machine" in the search bar at the top. Click "+ Create" and select the "Azure virtual machine" option. Make sure the correct Subscription is shown, in the event you have more than one, and select the Resource Group in which you want your VM to reside. Give your VM a name (e.g., VM-1), and select a region. You are able to select a different region than the Resource Group if all machine sizes are not available, but your VMs and virtual network must be in the same region to ensure reliable communication. For "Image," select the type of VM you are creating from the drop-down menu. For this demonstration, select either Windows 10 Pro or Ubuntu Server 24.04 (free services eligible). You'll repeat similar steps to create either VM, and the order is unimportant. For "Size," select enough vcpus and memory to meet your needs; more speed costs more money. When creating the Windows VM, set the username and password (use something you'll remember). When creating the Ubuntu Server VM, click the "Password" radio button for "Authentication type" and create a username/password. Most default settings would be fine for the purpose of exploring network activity.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
