<h1>(Proton) VPN Deployment, Exploration Within Local (Azure) Virtual Machine</h1>
This tutorial outlines deploying and exploring a (Proton) VPN within a local (Azure) Virtual Machine. Although there are many other sources of VPNs, we'll be using Proton VPN for this example. 

VPNs (Virtual Private Networks) enhance privacy, security, and accessibility online. They encrypt your internet traffic, protecting sensitive data from hackers, especially on public WiFi. VPNs also allow bypassing geography restrictions to access region-specific content/resources, and prevent ISP tracking.

VPNs are preferred in cases such as securing remote work connections, accessing geo-blocked content (i.e. streaming services), and protecting data on public WiFi.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machine)
- Proton VPN
- Remote Desktop

<h2>Prerequisites</h2>

- Microsoft Azure Subscription/Account
- Proton VPN Subscription/Account

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)


<h2>Deployment and Exploration Step-By-Step</h2>

<p>
</p>
<p>

![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20075908.png)
      Beginning this lab, as stated above, we will first create a VM in Azure using Windows 10 for our Proton VPN. So for starters with this example, log into your Azure account > go to virtual machines > click on 'create' to create the VM. I will name our example VM "VPN-VM". However, feel free to name your VM, or any other part of this example whatever you're comfortable with naming it. :)
   
   A few of our Azure VM's settings are as follows: Region - East US, Image - Windows 10 v22H2-Gen2, Size - Standard D2s v3 (2 virtual cpus, 8GiB memory). The remaining settings are pretty much set for this example. Your settings should look similar to the settings in the photo(s) below:

   ![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20082103.png)

   Go ahead and create the VM. Once you have it created, your screen should resemble a similar screen to the photo below. 

   ![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20091639.png)

   To verify that you've created the VM, search for your virtual machine resources and it should be listed similarly to the photo below. Also, take note that our example VM, "VPN-VM" IP Address is "172.174.247.167".

   ![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20091736.png)
   ![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20094237.png)

   Now that our VM is created, we will next log into our VM using Remote Desktop. So, open Remote Desktop and enter the IP Address of the VM, in this example, I'll enter "172.174.247.167". If you're using Windows, your Remote Desktop should look similar to the below photo.

   ![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20092250.png)

   Once you've clicked on "Connect", it will take you to the following screen (below):

   ![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20092415.png)
   ![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20092541.png)

   In this case, I'm signing in using the account created with the VM, in which I named "DeAndre VPN", but again, feel free to name the account VM, VM, Azure resource group, or any other part whatever you'd like to name them. So near the bottom, click on "More choices" > then click "use a different account" if you're not using your default account, but utilizing the VM account.

   ![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20092830.png)

   Once you continue with your selected account, you should see a screen similar to the screen below:

   ![image alt](https://github.com/djl1024/test-pics/blob/7539a8178f8fcc4bcc13686c1ff5d7e5d4d3a175/Screenshot%202025-01-02%20092856.png)

   Click "Yes" to continue. You should then be taken into your local VM. After accessing our example "VPN-VM", I was taken to the screen below:

 ![image alt](https://www5.lunapic.com/editor/newsave.php)

   Congrats! You've created and launched your VM! To verify or double check that the IP Address is still the same IP Address, "172.174.247.167", we can visit whatsmyipaddress.com for another source informing us of the IP Address. As you can see below, our IP Address still stands at "172.174.247.167" based on whatsmyipaddress.com.

   pic phone whatsmyipaddress before vpn ![image alt](

   Now, really quickly, we will explore Amazon.com under our normal VM IP Address. Once I landed on Amazon's website, it seemed to be the same Amazon we're all used to, in English language (see below photo).

   pic phone amazon last ![image alt](
   
   Now we need to set up our VPN. You can start by opening your (Proton) VPN. So once you've downloaded Proton VPN's software and created a subscription, open the app and you should be taken to a screen similar to the screen below:

   pic phone proton not set ![image alt](

   To activate Proton's VPN, we can do so rather quickly by clicking on "Quick Connect", but the VPNs location will be randomly selected (free subscription plan). I believe ProtonVPN allows you a choice on their paid plans, but for this example, I'm using their free plan.

   After that, you should now have the VPN successfully connected! It should notify you ("Connected") near the top of the screen, like in the photos below:

   pic phone vpn connected 1 ![image alt](
   pic phone vpn connected 2 (close up) ![image alt](

In this example, it says our VPN is located in the Netherlands, with our new example VPN IP Address as "89.38.99.79". We will now double-check our new IP Address at the website we used earlier, whatsmyipaddress.com.

After revisiting whatsmyipaddress.com, we can see that now, with our VPN connected, our IP Address is our VPN IP Address "89.38.99.79", according to whatsmyipaddress.com. But, whatsmyipaddress.com says that our VPN is located in Muscat, Oman, a smaller Middle-Eastern country located next to Saudi Arabia! (See photo below)

pic phone whatsmyipaddress new ip ![image alt](

To find out once and for all, we will revisit Amazon.com using our example VPN within our VM, IP Address "89.38.99.79", and see what it brings us (see photo below).

pic phone amazon dutch ![image alt](

Upon revisiting Amazon.com using our VPN, we can see that we landed on Amazon's home page, but the words are in Dutch (language). Based on this small exploration, we probably can safely say that our VPN is definitely located in the Netherlands, just as ProtonVPN said, instead of the Arabic location given to us by whatsmyipaddress.com.

Nonetheless, this concludes our (Proton) VPN test on our Azure virtual machine. I hope this helps and certainly hope you've enjoyed our VPN deployment and exploration experiment! Until next project!
   
   
</p>
<br />
