<h1>Active Directory Lab</h1>


 ### [Download VMware Workstation Player](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html)


<h2>Description</h2>
<b>Follow along with me in this simple walkthrough as I stand up a virtual Active Directory environment which is designed to provide an ideal platform for simulating real world Active Directory deployments.
</b>
<br />
<br />
The script is used in this demo where I setup Azure Sentinel (SIEM) and connect it to a live virtual machine acting as a honey pot.
We will observe live attacks (RDP Brute Force) from all around the world. I will use a custom PowerShell script to
look up the attackers Geolocation information and plot it on an Azure Sentinel Map!
<br />
<br />

<p align="center">
<img src="https://i.imgur.com/3d3CEwZ.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>What You'll Need</h2>

- <b>An internet accessible workstation that can run the required VMs</b> 
- <b>Virtualization hypervisor such as Hyper-V, VMware, or Virtualbox</b>
- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer
- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer
- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer
- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from China coming in; Custom logs being output with geodata</h2>

<p align="center">
<img src="https://i.imgur.com/LhDCRz4.jpeg" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map of incoming attacks after 24 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://i.imgur.com/krRFrK5.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
