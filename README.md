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

- Now launch the zenmap application.
- And enter the ip address of the metasploitable server to scan for vulnerabilities

<p align="center">
<b>Zenmap Scan</b>
<br/>
<img src="https://imgur.com/stB7X0o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- You can see how many ports are open.
- This is actually a gold mine for a hacker.
- Lets look at it in a more detailed manner by switching to the Ports/Hosts output

<p align="center">
<b>Zenmap Scan</b>
<br/>
<img src="https://imgur.com/FeE7OBO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- We can see that port 22 is open.
- And it is running the ssh service.
- Let us gain access through this.

<p align="center">
<b>Elevated privileges</b>
<br/>
<img src="https://imgur.com/sYSjoS9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- Wee need to be in the root user

<p align="center">
<b>Elevated privileges</b>
<br/>
<img src="https://imgur.com/ShtUi26.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- Now type the command `ssh msfadmin@<ipaddress>`
- We can easily gain access because we already know the password for metasploitable
- Just type the password and you will get access to it.

<p align="center">
<b>Elevated privileges</b>
<br/>
<img src="https://imgur.com/NWbYHNG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- Now we are in the web server
- You can perform `ls` or `pwd` or another command to navigate through the files
- We have successfully gained access to it.

<p align="center">
<b>Elevated privileges</b>
<br/>
<img src="https://imgur.com/n7muPBt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
</p>

- You can come out of it by typing the `logout` command

## Issues
- In some cases you might get the fllowing error message

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
