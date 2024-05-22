# Virtual-Private-Networks-Observing-IP-Addresses

<h2>Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop
- whatismyipaddress.com
- ProtonVPN (VPN service)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- 

<h2>Overview of Main Steps</h2>

- Step 1: Make a resource group.
- Step 2: Make a Windows 10 virtual machine 
- Step 3: 
- Step 4: 
- Step 5: 

<h2>Actions and Observations</h2>


<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/cc31898d-d321-4209-a715-cb41763fbf54"80%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
First, a new resource group must be made where a virtual machine will be placed  in.
  <br />
In the top search bar search: resource group, and then in top left click "create".
  <br />
  <br />
Name the new resource group.
  <br />
Also select which subscription account to place the resource group under.
  <br />
And pick which geographic region you want the resource group in.
  <br />
  <br />
Organizational tags are optional.
  <br />
Create the resource group.
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/b35a234e-e2bd-46c6-8beb-e4648ea4bbe0" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the top search bar search: virtual machines, then click "create", then "Azure Virtual Machine".
  <br />
  <br />
For this virtual machine: Select a subsciption account, the resource group just made, & a geographic region different from where your PC is located.
  <br />
Name this VM.
  <br />
The above redundancy & security settings will suffice.
  <br />
The image (VM's operating system) will be Windows 10 Pro, ver. 22H2
  <br />
VM architecture x64 will suffice.
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/e0cd223a-85cf-4f6e-9465-f208d1d3909b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select size "2 vcpus" (2 virtual CPU's).
  <br />
Set up administrator account info for the VM: the username & password.
  <br />
Public inbound ports must allow selected ports, and allow RDP 3389 (for remote desktop to the VM).
  <br />
Scroll down & confirm you have the appropriate Windows 10/11 license.
  <br />
  <br />
Then create the VM.
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/5ac8f989-0888-406f-82d6-e3b1589bfb35" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
In your Windows computer bottom search bar type: Remote Desktop Connection.
  <br />
In the top center search bar search: Virtual Machines.
  <br />
Select the Windows VM.
  <br />
Copy the Public IP address on the right side into the Remote Desktop Connection & Connect.
  <br />
Enter the administrator account credentials for the VM: the username & password.
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/EthanZSu-azure-network-protocols/assets/168872181/6badce6b-9266-484e-bcda-c518839ca625" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click "yes" on the pop-up.
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/EthanZSu-azure-network-protocols/assets/168872181/e5f17491-cd13-4f1f-aae8-e10d06d17f00" height="150%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the event you see this pop-up "mtsc.exe - Entry Point Not Found",
  <br />
Drag the pop-up to the top right corner & quickly exit it & the remote desktop window.
  <br />
If the pop-up is still there, simply click "OK".
  <br />
  <br />
You must then repeat the steps from the previous 2 pictures to use Remote Dektop to access your Windows VM. 
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/EthanZSu-azure-network-protocols/assets/168872181/53752c9d-3d12-406a-8bd4-afd176f117e7" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select "No" to all the privacy setting (as none of those features will be needed).
<br />
Then accept.
<br />
On the right click "yes" to the network pop-up "do you want... your PC to be discoverable by other... devices on this network?"
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/EthanZSu-azure-network-protocols/assets/168872181/f719dad4-a1e0-4cff-9a3f-64eec8d693f8" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
If there is any Windows promotional pop-up, exit it.
  <br />
Decline all Windows offers to sign in & bring your data (because this project is temporary & requires none of that sign-up).

</p>
<br />



<p>
<img src="https://github.com/EthanZSu/EthanZSu-azure-network-protocols/assets/168872181/48fdecf6-a66c-4371-aa08-832fb3aea4bc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open Microsoft Edge web browser.
  <br />
In the top search bar search "wireshark download" & go to the wireshark.org site.
</p>
<br />





<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
   <br />
</p>
<br />
