# Virtual-Private-Networks-Observing-IP-Addresses
This tutorial observes how a computer's public IPv4 address can be changed 
  <br />
by using either Azure virtual machines (VMs) or ProtonVPN (a virtual private network service).
<h2>Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
- Remote Desktop
- whatismyipaddress.com
- ProtonVPN (VPN service)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- 

<h2>Overview of Main Steps</h2>
- Step 1: On your computer: browse to whatismyipaddress.com.
  <br />
- Step 2: Make a resource group.
  <br />
- Step 3: Make a Windows 10 VM in a region different from your computer.
  <br />
- Step 4: On your VM browse to whatismyipaddress.com.
  <br />
- Step 5: Sign up for ProtonVPN.
  <br />
- Step 6: Download ProtonVPN to your VM.
  <br />
- Step 7: On your VM connect to a VPN server in a region different from your VM.
  <br />
- Step 8: Through the VPN, browse to whatismyipaddress.com.

<h2>Actions and Observations</h2>


<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/18e31ec6-ba88-4de3-942d-d68ca24b7376" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
You can see your computer's IPv4 address by browsing to whatismyipaddress.com.
   <br />
The site will show your IPv4 address & the region your computer is in.
    <br />
    <br />
(I've redacted my IPv4 address, Internet Service Provider, & city location for privacy).
</p>
<br />



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
Select the VM.
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
You must then repeat the steps from the previous 2 pictures to use Remote Dektop to access your VM. 
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
Open Microsoft Edge web browser.
  <br />
Decline all Windows offers to sign in & bring your data (because this project is temporary & requires none of that sign-up).

</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/9b775f59-63fc-4138-a1fe-d7711160c3bf" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the top search bar search: whatismyipaddress.com, then open the site.
  <br />
  <br />
The website should confirm the geographic region of your VM is the same as where you first set it.
  <br />
The site of course also confirms the IPv4 address of the VM differs from your computer's. 
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/2f2f64ca-424f-4cc2-bb75-86898ad5aefb" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
On your computer (not your Azure VM), go to protonvpn.com.
  <br />
On top right, select: Create Account.
   <br />
On bottom right, select: Get Proton Free (if you want the free version).
  <br />
Continue with free.
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/55b06138-a007-4824-b6ec-c13708a14c13" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
You will need to set up an account by providing an email address & a password.
   <br />
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/0607f39f-0465-45a3-8e70-d0392bacf6ab" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
Use remote desktop to sign into your VM.
  <br />
Go to protonvpn.com and sign into your protonvpn account.
  <br />
On the Left select: downloads.
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/b67100a7-b0cb-4788-9fd5-cc7b0587a374" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
Download Windows, Download ProtonVPN.
   <br />
Open downloads in file explorer.
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/cd41ef2b-3e62-4ca1-ade8-cc65c4b0ea37" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
Run the ProtonVPN download, Select "OK" to English
   <br />
Select "Next", "Install"
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/5813c6f3-38cb-49ec-9dec-7bc7fc54de80" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
Select "Automatically close the applications", "Next",
   <br />
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/3844bfc5-caa9-4b94-a399-764985fedd5c" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
Select "cancel", "yes", "finish".
   <br />
</p>
<br />



<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/fb90fd63-8a20-4d8b-afa5-052859d0b754" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
Exit the file explorer & the web browser window.
   <br />
Open the ProtonVPN app on the left, sign in, & skip the tour.
</p>
<br />


<p>
<img src="https://github.com/EthanZSu/vpn-and-ips/assets/168872181/4eee3978-f1d6-4545-9ad0-0e76aed01ba0" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
You can quick-connect to a VPN server in another region different from  your VM's region.
   <br />
Then open Microsoft Edge again & go to whatismyipaddress.com.
    <br />
The site confirms the IPv4 address & country of the VPN server used differs from your original VM's. 
</p>
<br />


<p>
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
   <br />
</p>
<br />
