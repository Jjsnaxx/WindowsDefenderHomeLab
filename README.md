<h1>Configuring Windows Firewall Rules & Windows Antivirus</h1>


<h2>Objective</h2>

This lab aims to demonstrate:

1. How to review Windows Security Virus and threat protection, Update threat definitions and run Windows Antivirus quick scan.
2. Configure Microsoft Windows Defender Firewall with advanced security to allow the connection for Key Management Service on the Domain and Private network and Deny the connection for Key Management Service on the Public network.
   
<br />


<h2>Utilities Used</h2>

- Windows Defender Antivirus
- Windows Defender Firewall

<h2>Environments Used </h2>

- <b>Windows 10</b> 

<h2>Windows Defender Antivirus Walkthrough:</h2>
<br />

<p align="center">
   
From the start menu type in Virus and Threat Protection and open the program: <br/>
<img src="https://i.imgur.com/d143tVE.png" height="80%" width="80%" alt="Launch Windows Antivirus"/>
<br />
<br />
Once open some important features to note:
- Current Threats/Scan options
- Virus and Threat Protection Settings
- Virus & threat protection updates
- Ransomware protection
<img src="https://i.imgur.com/fE62DL1.png" height="80%" width="80%" alt="Virus and Threat Protection Page"/>
<br />
<br />
Scan Options: Here you can choose to what type of scan you wish to complete, it also shows if there are any threats on your current device. You can see when the last scan occurred, how long the scan took, and how many files were scanned. Here you can also click the button to start a quick scan or access scan options to run a full scan or a custom scan. <br/>
<img src="https://i.imgur.com/p99Yq7P.png" height="80%" width="80%" alt="Scan Options"/>
<br />
<br />
Virus and Threat Protection: Here you can configure your level of protection, opt to send sample files to Microsoft, exclude files or folders from scans, or temporarily stop your protection. Unless you have 3rd party Anti-virus applications installed it is advised to have Real Time Protection switched on <br/>
<img src="https://i.imgur.com/ur98KFB.png" height="80%" width="80%" alt="Inbound Rules"/>
<br />
<br />
Virus and Threat Protection Updates: Windows Security uses security intelligence, also known as definitions, to identify known threats. These definitions include information about known threats. These definitions are updated automatically, but if you suspect a problem with your system, you should ensure that threat definitions are up-to-date before you run a scan.  <br/>
<img src="https://i.imgur.com/yqyhBCJ.png" height="80%" width="80%" alt="Updating Threat Definitions"/>
<br />
<br />
Ransomeware Protection: Here, you can choose to enable controlled folder access. This protects memory, files, and folders from unauthorized changes. <br/>
<img src="https://i.imgur.com/QzlISjw.png" height="80%" width="80%" alt="Ransomeware Protection"/>

<h2>Windows Defender Firewall Walkthrough:</h2>
<br />
From the start menu type in Virus and Threat Protection and open the program: <br/>
<img src="https://i.imgur.com/bNmaAEC.png" height="80%" width="80%" alt="Launch Windows Firewall"/>
<br />
<br />
Here's what it should look like: <br/>
<img src="https://i.imgur.com/UN4boV4.png" height="80%" width="80%" alt="Firewall and Network Protection"/>
<br />
<br />
Next we want to select advanced security: <br/>
<img src="https://i.imgur.com/DUJGZsD.png" height="80%" width="80%" alt="Advanced Security"/>
<br />
<br />
Select inbound rules. Rules with a green tick next to them indicates that rule is enable to allow inbound communication. Rules without the tick mean they are available for use but not enabled. <br/>
<img src="https://i.imgur.com/qD87M1z.png" height="80%" width="80%" alt="Inbound Rules"/>
<br />
<br />
Scroll to the Key Management Service inbound rule, the policy is currently not enabled. If enabled, the rule would allow communication.
Double-click this rule. 
<br/>
<img src="https://i.imgur.com/D3UoIwh.png" height="80%" width="80%" alt="KMS"/>
<br />
<br />
Click on advanced and untick the box "Public" because we want to allow communication only with the domain and private networks <br/>
<img src="https://i.imgur.com/LjcmCMy.png" height="80%" width="80%" alt="Untick Public"/>
<br />
<br />
Now we will create an inbound rule that blocks communication with the public network. Since the new rule will be similar to the last, we will copy the existing rule. Right-click the Key Management Service (TCP-In) inbound rule and click Copy. Press Ctrl+V to paste.  <br/>
<img src="https://i.imgur.com/i2Cuii0.png" height="150%" width="150%" alt="Copy rule"/>
</p>

<h2>Post-Lab lessons learnt</h2>

First ever lab (I have ever shared) DONE. I think learning how to navigate Github, creating a repository as well as learning how to use markdown text was probably the most challenging bit. Windows Anti-virus is definitely a great option to ensure your computer data is safe asssuming its configured properly. Learnt how to update threat definitions and perform a custom scan on a specific folder.

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
