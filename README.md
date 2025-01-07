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
Wireshark is software that allows us to see and monitor IP packets and network traffic. We are going to use this along with Powershell to ping and communicate with the ubuntu virtual machine.
</p>

<p>
Wireshark is software that allows us to see and monitor IP packets and network traffic. We are going to use this along with Powershell to ping and communicate with the ubuntu virtual machine.
</p>

<p>
Select Ethernet and click on the bluefin button in the top left. We can now filter various forms of network traffic. Type ICMP.
</p>

<p>
Select Ethernet and click on the bluefin button in the top left. We can now filter various forms of network traffic. Type ICMP.
</p>


<br />
