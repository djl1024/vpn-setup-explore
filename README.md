<h1>(Proton) VPN Deployment, Exploration Within Local (Azure) Virtual Machine</h1>
This tutorial outlines deploying and exploring a (Proton) VPN within a local (Azure) Virtual Machine. Although there are many other sources of VPNs, we'll be using Proton VPN for this example. 

VPNs (Virtual Private Networks) enhance privacy, security, and accessibility online. They encrypt your internet traffic, protecting sensitive data from hackers, especially on public WiFi. VPNs also allow bypassing geography restrictions to access region-specific content/resources, and prevent ISP tracking.

VPNs are preferred in cases such as securing remote work connections, accessing geo-blocked content (i.e. streaming services), and protecting data on public WiFi<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machine)
- Proton VPN
- Remote Desktop

<h2>Prerequisites</h2>

- Microsoft Azure Subscription/Account
- Proton VPN Subscription/Account

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)


<h2>Deployment and Configuration Steps</h2>

<p>
</p>
<p>

1st pic create 1
   
   Beginning this lab, as stated above, we will first create a VM in Azure using Windows 10 for our Proton VPN. So for starters with this example, log into your Azure account > go to virtual machines > click on create the VM.
   
   A few of our Azure VM's settings are as follows: Region - East US, Image - Windows 10 v22H2-Gen2, Size - Standard D2s v3 (2 virtual cpus, 8GiB memory). The remaining settings are pretty much set for this example. Your settings should look similar to the settings in the photo(s) below:

   pic settings 1

   pic validation 1

   Go ahead and create the VM. Once you have it created, your screen should resemble a similar screen to the photo below:

   pic deploy complete 1

   Now that our VM is created, we will next log into our VM using Remote Desktop.

   
</p>
<br />
