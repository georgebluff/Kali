# Kali - Android Reverse TCP Handler Exploit on Oculus Question 2
### Oculus Quest 2 &amp; Kali Linux Exploit

Prerequisite Setup:
Oculus Quest 2 Developer Mode Enabled

Steps:
Configure WebServer from Kali <br/>
sudo python3 -m http.server --bind 127.0.0.1 9000 <br/>
![This is an image](https://raw.githubusercontent.com/georgebluff/Kali/main/apache%20webserver.png)

Configure localtunnel for browser redirect (optional) <br/>
![This is an image](https://raw.githubusercontent.com/georgebluff/Kali/main/localtunnel.png)

Confirm access to webserver on custom port
Create msfvenom malicious android .apk & put on desktop<br/>
![This is an image](https://raw.githubusercontent.com/georgebluff/Kali/main/msfvenom.png)

Launch msfconsole and use exploit/multi/handler for android reverse_tcp payload & 
set LHOST<br/>
show options<br/>
exploit<br/>
![This is an image](https://raw.githubusercontent.com/georgebluff/Kali/main/TCP%20handler.png)

Download & Install androidApp.apk from WebServer<br/>
![This is an image](https://raw.githubusercontent.com/georgebluff/Kali/main/oculus%20browser.png)

Run MainActivity com.metasploit.stage<br/>
![This is an image](https://raw.githubusercontent.com/georgebluff/Kali/main/unsupported%20apps.png)

Sysinfo<br/>
![This is an image](https://raw.githubusercontent.com/georgebluff/Kali/main/sysinfo.png)

  
  
Links:<br/>
  Access Android with Metasploit Kali (Cybersecurity) - https://www.youtube.com/watch?v=YRm-St0bJhU <br/>
  How To Set Up Port Forwarding in Kali Linux Without Router Access | Kali Linux 2021.2 - https://www.youtube.com/watch?v=juu5PM0_NUI <br/>
  Kali http server setup - https://linuxconfig.org/kali-http-server-setup <br/>
  
Notes: This infomation is for training and security research purposes only.
