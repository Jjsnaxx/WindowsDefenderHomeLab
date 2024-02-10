<h1>Configuring Windows Firewall Rules & Windows Antivirus</h1>


<h2>Objective</h2>

This lab aims to demonstrate:

1. How to review Windows Security Virus and threat protection, Update threat definitions and run Windows Antivirus quick scan.
2. How to; configure, add and remove firewall rules using Microsoft Windows Defender Firewall advanced security
   
<br />


<h2>Utilities Used</h2>

- Windows Defender Antivirus
- Windows Defender Firewall

<h2>Environments Used </h2>

- <b>Windows 10</b> 

<h2>Lab walk-through:</h2>

<p align="center">
   
From the start menu type in Virus and Threat Protection and open the program: <br/>
<img src="https://i.imgur.com/d143tVE.png" height="80%" width="80%" alt="Launch Windows Antivirus"/>
<br />
<br />
Once open some important features to note:
- Current Threats: Shows if there are any threats on your current device. You can see when the last scan occurred, how long the scan took, and how many files were scanned. Here you can also click the button to start a quick scan or access scan options to run a full scan or a custom scan.
- Virus and Threat Protection Settings: Here you can configure your protection level, opt to send sample files to Microsoft, exclude files or folders from scans, or temporarily stop your protection.
- Virus & threat protection updates: Here, you can view the last time your virus definitions were updated. You can also opt to manually check for updates.
- Ransomware protection: Here, you can choose to enable controlled folder access. This protects memory, files, and folders from unauthorized changes.  
<img src="https://i.imgur.com/fE62DL1.png" height="80%" width="80%" alt="Virus and Threat Protection Page"/>
<br />
<br />
Under Scan Options you can choose to what type of scan to complete: <br/>
<img src="https://i.imgur.com/p99Yq7P.png" height="80%" width="80%" alt="Scan Options"/>
<br />
<br />
Under Virus and Threat Protection here are the options, unless you have 3rd party Anti-virus applications installed it is advised to have Real Time Protection switched on:  <br/>
<img src="https://i.imgur.com/ur98KFB.png" height="80%" width="80%" alt="Protection Settings"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
