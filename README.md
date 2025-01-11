# Networking-Between-Two-Virtual-Machines

<p align="center">

</p>

This tutorial shows how to network between two virtual machines using Wireshark and PowerShell.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)


<h2>Operating Systems Used </h2>

- Windows 11</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure Account
- Internet Connection
- Computer or Laptop


<h2>Connection Steps</h2>
<p>
Create a second virtual machine, but use Ubuntu as an Operating system instead of Windows.
</p>

<p float="left">
<img src="https://imgur.com/j1EK62e.png" height="80%" width="80%"/>
</p>
<p>
Now, you can remotely connect to the Windows virtual machine, not the Ubuntu one. Once there, search for Wireshark on the virtual machine browser and download the installer.
</p>

<p>
<img src="https://imgur.com/ZxlcLzw.png" height="80%" width="80%"/>
</p>

<p>
Install Wireshark and choose the default settings In the installer.
</p>

<p>
<img src="https://imgur.com/ZbELFGW.png" height="80%" width="80%"/>
</p>

<p>
Select Ethernet, which is highlighted blue, and click on the sharkfin button in the top left.
</p>

<p>
<img src="https://imgur.com/2AoFaaj.png" height="80%" width="80%"/>
</p>

<p>
Now you can monitor all the network traffic on the windows virtual machine.
</p>

<p>
<img src="https://imgur.com/2Tbp5RJ.png" height="80%" width="80%"/>
</p>

<p>
We can filter the kind of traffic we can see. If we type ICMP, for example, only ICMP packets will appear.
</p>

<p>
<img src="https://imgur.com/yUMPaRP.png" height="80%" width="80%"/>
</p>

<p>
Open up Powershell, which you can type in the search bar. Grab the private IP address of the Ubuntu virtual machine located on the virtual machine page in Azure. Type ping and then the private IP address in Powershell. Now we can see the ICMP traffic traveling between the two virtual machines.
</p>

<p>
<img src="https://imgur.com/Knycbqg.png" height="80%" width="80%"/>
</p>

<p>
<img src="https://imgur.com/vmzRSNB.png" height="80%" width="80%"/>
</p>

<p>
Now, let's try something else. Ping the Virtual machine again, but add -t after the private IP address. Now the Windows virtual machine is constantly pinging the Ubuntu virtual machine. We can stop this by messing with the firewall of the Ubuntu VM. 
</p>

<p>
<img src="https://imgur.com/XRVEb79.png" height="80%" width="80%"/>
</p>

<p>
Click on the resource group containing the Ubuntu virtual machine. Select the network security group of the virtual machine or nsg. Click on the settings option on the left and select inbound security rules. 
</p>

<p>
<img src="https://imgur.com/Hi2eoEi.png" height="80%" width="80%"/>
</p>

<p>
<img src="https://imgur.com/fKfrCxj.png" height="80%" width="80%"/>
</p>




<br />
