<h1>HONEYOPT IN KALI LINUX</h1>



<h2>Description</h2>
Project consists of a configured and deployed a honeypot on Kali Linux using Pentbox 1.8 to simulate a vulnerable HTTPS service and monitor intrusion attempts. The project included identifying the system’s IP address, configuring the honeypot on port 443 with custom intrusion messages, and enabling logging for attack activity. Functionality was validated by simulating unauthorized access through a browser, which triggered intrusion detection alerts and log entries. This project strengthened my skills in honeypot deployment, intrusion detection, and security monitoring.
<br />


<h2>🔧 Languages & Technologies Utilized</h2>

Ruby → Pentbox itself is written in Ruby (pentbox.rb is the script you executed).

Bash / Shell Commands → You used basic Linux terminal commands (ifconfig, cd, ./pentbox.rb, etc.) to configure and run the honeypot.

Networking Protocols →

TCP/HTTPS (port 443) → The honeypot simulated a service running over HTTPS.

IP (inet address) → Used for targeting the honeypot in the browser.

Kali Linux Environment → The OS where the honeypot was deployed and tested.

<h2>🌐Environments Used </h2>

- <b>🐧Kali Linux</b> (21H2)

<h2>🚶Program walk-through:</h2>

<p align="center">
Record eth0 IP address: <br/>
<img src="https://i.imgur.com/T4wQP62.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Change to Pentbox directory -1.8:  <br/>
<img src="https://i.imgur.com/s0iaqdq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
In the Terminal, navigate through the Pentbox menu by selecting Network Tools (2), then Honeypot (3), and finally choosing Manual Configuration (2) to access the advanced setup options.: <br/>
<img src="https://i.imgur.com/nk2Tk4I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure the honeypot by setting the open port to 443 and entering the custom intrusion message “Caught You!!” to display when an unauthorized connection was attempted.:  <br/>
<img src="https://i.imgur.com/KB7l6af.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enable logging for intrusion attempts by selecting ‘y’ and pressed Enter to save the logs, then accepted the default incremental log file name by pressing Enter again.(may take some time):  <br/>
<img src="https://i.imgur.com/NS2Ik1O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Minimize the Terminal, opened Firefox ESR from the sidebar, typed the new HTTPS URL in the address bar, and pressed Enter to navigate to the site.:  <br/>
<img src="https://i.imgur.com/5t727Tp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Closed the 'Problem loading page' window in Firefox.:  <br/>
<img src="https://i.imgur.com/YGn7TFI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Return to the Terminal window, 'INTRUSION ATTEMPT DETECTED!', and pressCtrl+C to stop it.":  <br/>
<img src="https://i.imgur.com/pRdpITw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
