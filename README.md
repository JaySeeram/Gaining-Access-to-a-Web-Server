# Gaining Access to a Web Server

## Description
This projects demonstrates how to gain access to a web server. The most important thing that we require, is the target's ip. Which, in most cases is usually going to be static, or will not change very much.
<br/>

## Tools Used
- <b>Zenmap</b> 
- <b>Metasploitable 2</b>

## OS Used
- <b>Kali Linux</b>

## Process
- **First launch metasploitable from your virtual box.**
- **Login with your credentials.**
- **The default credentials are:**
  - **Username:** msfadmin
  - **Password:** msfadmin

<p align="center">
<b>Enter Credentials:</b>
<br/>
<img src="https://imgur.com/6LgmPEV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- You won't be able to see the password while typing.
- Once done, press enter.

<p align="center">
<b>Logged in Screen:</b>
<br/>
<img src="https://imgur.com/8VK0S0Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- This screen will appear once you've successfully logged in.
- Make sure you've given the right credentials, if you fail to login.

<p align="center">
<b>Verify the IP address</b>
<br/>
<img src="https://imgur.com/lQUWqjB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- Type the `ifconfig` to check the ip address.
- No3 launch kali linux from virtual box and open the terminal.

<p align="center">
<b>Ping command</b>
<br/>
<img src="https://imgur.com/tpKfxup.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- Let's check if the server is active or not by typing `ping <ipaddress>`
- Once we start receiving packets, its evident that the server is active.
- You can also check by searching the ip address on your web browser

<p align="center">
<b>Metasploitable Web</b>
<br/>
<img src="https://imgur.com/JKJeq7q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
