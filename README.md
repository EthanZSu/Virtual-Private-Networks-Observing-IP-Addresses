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
   <br />
</p>
<br />



<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
   <br />
</p>
<br />
