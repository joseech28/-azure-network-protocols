<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />





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
<img src="https://imgur.com/8gLgzk4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. I generated both Window 10 and Linux (Ubuntu) VM map from azure portal.
</p>
<br />

<p>
<img src="https://imgur.com/QL6xxYf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4. To begin, I establish a Remote Desktop connection to the Windows 10 VM I created earlier.
Once connected to the Windows 10 VM, I proceed to download and install Wireshark, a network protocol analyzer.
</p>
<br />

<p>
<img src="https://imgur.com/G62L6mY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5.  Wireshark network protocol analyzer.
</p>
<br />

<p>
<img src="https://imgur.com/9lXhZVM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6. After installing Wireshark, I apply a filter to display only ICMP traffic, which includes ping requests and replies.
</p>
<br />

<p>
<img src="https://imgur.com/L7vRtqV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7. I obtain the private IP address of the Ubuntu VM and attempt to ping it from within the Windows 10 VM.
</p>
<br />

<p>
<img src="https://imgur.com/QC720cm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8. While monitoring Wireshark, I observe the ping requests and replies, allowing me to analyze the network traffic.
Next, I open a command line or PowerShell within the Windows 10 VM and attempt to ping a public website, such as www.google.com.
I focus on Wireshark to observe the network traffic, specifically examining ICMP traffic related to the ping activity.</p>
<br />

<p>
<img src="https://imgur.com/tkFY59C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
9. To create a perpetual/non-stop ping, I initiate continuous pinging from the Windows 10 VM to the Ubuntu VM.
</p>
<br />

<p>
<img src="https://imgur.com/C1tCLYx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
10 In the Azure portal, I access the Network Security Group (NSG) associated with the Ubuntu VM and disable incoming (inbound) ICMP traffic.
</p>
<br />


<p>
<img src="https://imgur.com/0CFxnIb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
11. Returning to the Windows 10 VM, I continue observing the ICMP traffic in Wireshark and the command line ping activity.
  Simultaneously, I monitor the command line ping activity in the Windows 10 VM to verify that it has resumed functioning.
</p>
<br />

<p>
<img src="https://imgur.com/Q9RD79X.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
12. If the re-enabled ICMP traffic is functioning correctly, I can verify its successful restoration by observing both Wireshark and the command line ping activity.
Finally, I can stop the ping activity by terminating the command when I have finished observing and analyzing the ICMP traffic.
</p>
<br />


<p>
<img src="https://imgur.com/1xeVYzh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
13. Upon returning to Wireshark, I apply a filter to display only SSH traffic. This allows me to focus specifically on the Secure Shell (SSH) protocol and its related network traffic. By applying the filter, I can:
Analyze the SSH traffic between the Windows 10 VM and the Ubuntu VM.</p>
<br />

<p>
<img src="https://imgur.com/r8lzW72.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
14. I establish an SSH connection to the Ubuntu Virtual Machine using its private IP address. By initiating the SSH connection, I can remotely access and control the Ubuntu VM from the Windows 10 VM. This allows me to perform various tasks, execute commands, and manage the Ubuntu VM's configuration.</p>
<br />

<p>
<img src="https://imgur.com/YHW3z2h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
15. Once authenticated, I gain remote access to the command-line interface of the Ubuntu VM.
From here, I can execute Linux commands, modify system configurations, install software packages, and perform other administrative tasks on the Ubuntu VM.</p>
<br />

<p>
<img src="https://imgur.com/BRzmWjJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
16. As I observe the SSH traffic in Wireshark, I notice a continuous stream of SSH packets being captured. The traffic appears as a constant flow of data, indicating the ongoing communication between the Windows 10 VM and the Ubuntu VM through the SSH protocol. This continuous stream of SSH traffic is expected since the SSH connection provides a live and interactive session between the two machines.</p>
<br />

<p>
<img src="https://imgur.com/dwb0YyG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
17. By executing the 'exit' command, I signal the termination of the SSH session and disconnect from the Ubuntu VM. This action closes the remote connection and returns me to the command prompt or terminal session of the Windows 10 VM.</p>
<br />

<p>
<img src="https://imgur.com/p5zMmhn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
18. I open a command prompt or PowerShell window within my Windows 10 VM. From there, I run the command "ipconfig /renew" to attempt to obtain a new IP address for my VM. As I execute this command, I switch back to Wireshark and observe the DHCP traffic that starts appearing in the captured packets. The DHCP traffic includes the DHCP Discover, Offer, Request, and Acknowledge messages exchanged between my Windows 10 VM and the DHCP server. This indicates the dynamic IP address allocation process taking place and confirms the communication between the VM and the DHCP server.


</p>
<br />

<p>
<img src="https://imgur.com/RZ26onD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
19. I switch back to Wireshark and apply a filter to display only DNS traffic. This helps me focus on the DNS-related packets captured by Wireshark.
</p>
<br />

<p>
<img src="https://imgur.com/KUi95aC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
20. Next, I open a command prompt or PowerShell window within my Windows 10 VM. From there, I use the "nslookup" command to perform DNS queries for both "google.com" and "disney.com" to retrieve their respective IP addresses. As I execute these commands, I observe the DNS traffic being displayed in Wireshark. The captured packets include DNS queries and responses exchanged between my Windows 10 VM and the DNS server, revealing the DNS resolution process and the IP addresses associated with the queried domain names.
</p>
<br />


<p>
<img src="https://imgur.com/zY1bO0k.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
21. I return to Wireshark and apply a filter to display only RDP (Remote Desktop Protocol) traffic by specifying the TCP port 3389. By filtering for RDP traffic, I narrow down the captured packets to only those related to the RDP protocol.
</p>
<br />

<p>
<img src="https://imgur.com/vCcws0r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 22. I immediately notice a continuous stream of traffic appearing in Wireshark. The reason behind this non-stop "spamming" of traffic is that the RDP protocol is designed to provide a live stream of data from one computer to another. It constantly transmits data, even when there is no specific activity or interaction occurring between the two machines. This continuous flow of packets allows for a seamless remote desktop experience, as it ensures that the remote desktop session is constantly updated with the latest screen information and user input. In conclusion, the non-stop RDP traffic observed in Wireshark is a characteristic of the protocol's design to provide a continuous and interactive remote desktop experience. The constant stream of packets allows for seamless screen sharing and user interaction between the client and server, ensuring a smooth remote desktop session.

\</p>
<br />


