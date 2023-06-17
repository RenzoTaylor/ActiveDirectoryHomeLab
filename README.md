<h1>Active Directory Lab</h1>

<h2>Description</h2>
<b>Follow along with me in this simple walkthrough as I stand up a virtual Active Directory environment which is designed to provide an ideal platform for simulating real world Active Directory deployments.
</b>
<br />
<br />

<h2>What You'll Need:</h2>

- <b>An internet accessible workstation that can run the required VMs</b> 
- <b>Virtualization hypervisor such as Hyper-V, VMware, or Virtualbox</b>
- <b>Pfsense ISO</b> 
- <b>Kali Linux ISO</b> 
- <b>Windows 10 ISO</b> 
- <b>Windows server 2019 ISO</b> 
<br />
<h2>Choosing Our Hypervisor</h2>

 - <b>For this walkthrough, I’ll be using VMware Workstation 16 Pro as my hypervisor, but you should certainly be able to use any hypervisor of your choice and attain the same results. It's worth mentioning that this guide doesn't go over the actual installation of VMware, however there are a ton of videos available via Youtube that will walk you through the process. [Download VMware Workstation Player](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html)
</b>
<br />
<h2>Configuring pfsense</h2>

 - <b>I know this a homelab that many of you may end up nuking after you're done experimenting but I figured it would be a good learning experience to implement a solution that provides security by monitoring and controlling incoming and outgoing network traffic, so we’ll be using pfsense for that purpose and once it’s configured, we’ll be able to access the web interface from the Kali machine. [Download The pfsense ISO](https://www.pfsense.org/download/)
</b>
<br />
<p align="center">
Click "Create a New Virtual Machine" and keep the recommended configuration, select Next: <br/>
<img src="https://imgur.com/FBdl64q.png" height="35%" width="35%" alt="pfsense"/>
<br />
<br />
Navigate to the location where you saved the iSO file, select it and click Next:  <br/>
<img src="https://imgur.com/usTDSlj.png" height="35%" width="35%" alt="pfsense"/>
<br />
<br />
 Rename Virtual Machine to "pfsense":  <br/>
<img src="https://imgur.com/HNLkRM3.png" height="35%" width="35%" alt="pfsense"/>
 <br />
<br />
 Keep the default disk size and make sure the "Split virtual disk into multiple files" option is selected; click Next:  <br/>
<img src="https://imgur.com/oEh2ogC.png" height="35%" width="35%" alt="pfsense"/>
<br />
<br />
Select "Customize Hardware":  <br/>
<img src="https://imgur.com/2uVZov0.png" height="35%" width="35%" alt="pfsense"/>
<br />
<br />
For this virtual machine, 2GB of memory will suffice:  <br/>
<img src="https://imgur.com/Kxsl4Pp.png" height="35%" width="35%" alt="pfsense"/>
<br />
<br />
Add 3 networks adapters and assign each of them with a VMnet interface as shown below:  <br/>
<img src="https://imgur.com/ahm7EKJ.png" height="35%" width="35%" alt="pfsense"/>
 <br />
<img src="https://imgur.com/WI64YCX.png" height="35%" width="35%" alt="pfsense"/>
<br />
<br />
Once pfsense is powered on you'll be brought to the following screen, accept all defaults and allow pfsense to reboot:  <br/>
<img src="https://imgur.com/RUjRvNY.png" height="35%" width="35%" alt="pfsense"/>



</p>
</b>


