<h1>SSH Apache Server File Transfer Home Lab</h1>

<h2>Description:</h2>

I set up an Apache server on an Ubuntu VM and used SSH to securely connect from a Windows machine. I created a simple webpage using Apache and successfully transferred a test file between the two operating systems, demonstrating secure file transfer and web hosting capabilities.

<br/>
<br/>
<br/>
<br/>
<br/>

<p align="center">  
I started by installing 'openssh-server' to enable SSH on my Ubuntu system. 

<img src="https://i.imgur.com/ZRE0w6c.png" style="height: auto; width: 600px;"/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">  
Following this, I used the 'systemctl' command several times to check the status, <br/> 
enable and start the SSH service in this case. 

<br/> 
<img src="https://i.imgur.com/Nqc43iG.png" style="height: auto; width: 600px;"/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">  
Next I needed to change the firewall settings to allow SSH to connect to my <br/>
Windows machine. Enabling 'UFW' makes changing the firewall settings very simple. 

<br/>
<img src="https://i.imgur.com/Bav5V7f.png" style="height: auto; width: 600px;"/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">  
In order to access the Apache server's webpage via the <br/>
IP address above, I had to enable HTTP and HTTPS.

<br/>
<img src="https://i.imgur.com/6U2tMTl.png" style="height: auto; width: 550px;"/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">  
I connected to my Ubuntu VM via SSH now, listing <br/>
the contents of the directory to verify the connection.
  
<br/>
<img src="https://i.imgur.com/USWWccN.png" style="height: auto; width: 550px;"/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">  
After that, I installed the Apache2 package - 

<br/>
<img src="https://i.imgur.com/0kP46ED.png" style="height: auto; width: 750px;"/>
<br/>
<p align="center">  
- enabled and started the Apache service.

<br/>
<img src="https://i.imgur.com/vaTSTe7.png" style="height: auto; width: 750px;"/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">  
I edited the index file, producing this absolute Mona Lisa here.

<br/>
<img src="https://i.imgur.com/WJdtmOK.png" style="height: auto; width: 500px;"/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">  
At this point, I was trying to transfer a file from the server to my Windows client. Connecting <br/>
via SFTP to my VM. Using the 'get' command, I coppied -

<br/>
<img src="https://i.imgur.com/6OdrYjt.png" style="height: auto; width: 600px;"/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">  
- This file from my VM -

<br/>
<img src="https://i.imgur.com/aKXWexY.png" style="height: auto; width: 600px;"/>
<br/>
<br/>
<br/>
<br/>
<br/>
<p align="center">  
- To the Windows machine.
  
<br/>
<img src="https://i.imgur.com/r5EswHF.png" style="height: auto; width: 600px;"/>













