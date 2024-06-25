<h1>Elastic Stack SIEM Home Lab using Kali Linux</h1>

<h2>Description</h2>
This project consists of setting up Kali Linux virtual machine, configuring agents to collect logs and forward them to the SIEM, generating and querying different types of security events, utilizing analysis and visualization tools, and creating and testing alerts in the SIEM. This provides hands-on experience with security monitoring and incident response. 
<br />


<h2>Tools and Environments Used</h2>

- <b>Kali Linux VM</b> 
- <b>VMWare Workstation</b>
- <b>Elastic SIEM</b>

<h2>Program walk-through:</h2>

<p align="center">
After setting up Kali VM, I install Elastic Defend agent on VM in order to forward logs to SIEM. I then run sudo command in order to verify agent was installed correctly.<br/>
<img src="https://i.imgur.com/2FgAvYj.png" height="80%" width="80%"/>
<br />
<br />
<img src="https://i.imgur.com/XHhH7Vo.png" height="80%" width="80%"/>
<br />
<br />
Next, I ran a couple Nmap scans, which  is a scanning tool that can perform a variety of tasks to help explore networks and perform security audits, in order to generate some security events. I also generated more logs by entering the wrong password and using ssh to connect to my local machine. <br/>
<img src="https://i.imgur.com/Wgs8dzL.png" height="80%" width="80%"/>
<br />
<br />
After the data was forwarded to the SIEM, I started to query the security logs so I could analyze them using Elastic's log feature. Here I analyze Nmap scans, ssh login, and other security events. <br/>
<img src="https://i.imgur.com/XNJQ4mF.png" height="80%" width="80%"/>
<br />
<br />
<img src="https://i.imgur.com/TqYKm5L.png" height="80%" width="80%"/>
<br />
<br />
<img src="https://i.imgur.com/ZL7Qv0n.png" height="80%" width="80%"/>
<br />
<br />
Next, I created a dashboard that displays count of agent IDs every 30 minutes. I also created an alert that sends me an Email every time an NMap scan is run. <br/>
<img src="https://i.imgur.com/Om0nutm.png" height="80%" width="80%"/>
<br />
<br />
<img src="https://i.imgur.com/EuoKd9k.png" height="80%" width="80%"/>
<br />
<br />
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
