<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Step 1
- Step 2
- Step 3
- Step 4

<h2>Actions and Observations</h2>

<p>
<img src="https://imgur.com/zbRi6u9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
1. I log in to the Azure portal and navigate to the section for managing Azure Resource Groups.
I select the "Create" button to initiate the creation of a new resource group.
In the creation form, I provide a name for the resource group and choose the desired region and subscription.
After entering the necessary details, I proceed by clicking on the "Review + Create" button to review the configuration.
Once the review is complete and there are no errors, I finalize the process by clicking on the "Create" button to create the resource group.
Next, I move to the Virtual Machines section within the Azure portal.
I click on the "Create" button to begin creating a new Windows 10 Virtual Machine (VM).
During the VM creation, I select the previously created resource group, assign a name to the VM, and configure the desired settings.
While creating the VM, I enable the creation of a new Virtual Network (Vnet) and Subnet.
After setting up all the necessary options, I proceed by clicking on the "Review + Create" button to review the VM configuration.
Once the review is complete, I click on the "Create" button to create the Windows 10 VM.</p>
<br />

<p>
<img src="https://imgur.com/8GxbZoC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
2. I repeat the process to create a Linux (Ubuntu) VM, selecting the previously created resource group and Vnet during the VM creation.
After successfully creating the VMs, I navigate to the Network Watcher section in the Azure portal.
Within Network Watcher, I observe and analyze the Virtual Network (Vnet), ensuring its settings and connectivity are as intended.</p>
<br />

<p>
<img src="https://imgur.com/QL6xxYf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. To begin, I establish a Remote Desktop connection to the Windows 10 VM I created earlier.
Once connected to the Windows 10 VM, I proceed to download and install Wireshark, a network protocol analyzer.</p>
<br />


<p>
<img src="https://imgur.com/8gLgzk4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. I generated both Window 10 and Linux (Ubuntu) VM map from azure portal.
</p>
<br />

<p>
<img src="https://imgur.com/L7vRtqV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/QC720cm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src=".png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/tkFY59C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/YZBQF1R.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/0celQQl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/C1tCLYx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
9Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/7nEMAsN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
10Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/0CFxnIb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
11Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/Q9RD79X.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
12Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/tMOUEj0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
13Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/1xeVYzh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
14Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/r8lzW72.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
15Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/YHW3z2h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
16Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/BRzmWjJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
17Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/dwb0YyG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
18Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/p5zMmhn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
19Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/RZ26onD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
20Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/KUi95aC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
21Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />


<p>
<img src="https://imgur.com/G62L6mY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
26Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/9lXhZVM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
27Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://imgur.com/tRIl43A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
28Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src=".png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
29Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src=".png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
30Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

