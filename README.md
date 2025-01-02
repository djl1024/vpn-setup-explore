<h1>Proton VPN Deployment, Exploration Within Local (Azure) Virtual Machine</h1>
This tutorial outlines the deployment and exploration of a (Proton) VPN within a local (Azure) Virtual Machine. There are many other sources of VPNs, but for this example, we'll be using Proton VPN. 

VPNs (Virtual Private Networks) are useful for enhancing privacy, security, and accessibility online. They encrypt your internet traffic, protecting sensitive data from hackers,especially on public WiFi. VPNs also allow bypassing geography restrictions to access region-specific content/resources, avoid censorship, and prevent ISP tracking.

VPNs are preferred in cases such as:
   -Securing remote work connections
   -Accessing geo-blocked content (i.e. streaming services)
   -Protecting data on public WiFi<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machine)
- Proton VPN
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)


<h2>Deployment and Configuration Steps</h2>

<p>
</p>
<p>
In this lab we will create two VMs in the same VNET. One will be a Domain Controller, the other will be a Client machine. We will change the DC to a static IP because its offering Active Directory services to the client machine. Client machine will be joined to the domain. We will control the DNS settings on the client machine, the client machine will use the DC as its DNS server. 
</p>
<br />
