For my second project, I decided to explore different honeypots.
A honeypot is a cybersecurity mechanism and is used to open ports so we can attract malicious actors.
They also gather intelligence about our attacker, identity, and methods.
I chose Pentbox because of its GUI which makes it straightforward.

# Honeypot
Automatic and Manual Honeypot using Pentbox 

![image alt](https://github.com/fabianvagi91/Honeypot/blob/81a9cd8616c8ab3206f44f61d7f40f2186d27a46/Install.jpg) 

Installation from https://github.com/technicaldada/pentbox uncompressing and execution of Pentbox
For the Honeypot configuration, it is important to execute as root user.

![image alt](https://github.com/fabianvagi91/Honeypot/blob/81a9cd8616c8ab3206f44f61d7f40f2186d27a46/pentboxmenu.jpg) 

In the menu, we can see all the options available that we can do.
I choose option 2 Network tools and inside I choose 3 which is Honeypot
For the first time using this tool, I wanted the configuration not to have to be an issue so I chose the first option  Fast Auto Configuration.
Fast Auto Configuration opens the port 80 HTTP.

![image alt](https://github.com/fabianvagi91/Honeypot/blob/81a9cd8616c8ab3206f44f61d7f40f2186d27a46/testingport80.jpg) 

For testing purposes, i opened my Firefox and entered 127.0.0.1:80
And receive notifications from the honeypot that has been an intrusion.
Here are the logs and we have useful information about the attempt.
(which OS was used by the attacker, browser, and time)


![image alt](https://github.com/fabianvagi91/Honeypot/blob/81a9cd8616c8ab3206f44f61d7f40f2186d27a46/manualconfigport22.jpg) 

After realizing how this tool behaves I wanted to customize my honeypot configuration.
I selected the option Manual Configuration and chose to open port 22 SSH.
Also customized my message to the intruder, name, and location of the log file and alarms with sound.

![image alt](https://github.com/fabianvagi91/Honeypot/blob/81a9cd8616c8ab3206f44f61d7f40f2186d27a46/manualtesting.jpg) 

For testing the honeypot i needed to know the ip of the honeypot (the ip of the virtual machine)

![image alt](https://github.com/fabianvagi91/Honeypot/blob/81a9cd8616c8ab3206f44f61d7f40f2186d27a46/testingport22.jpg)

And i used nmap to see if the port 22 its open (means that my honeypot is running in this port)
After using the nmap tool we generate logs into our honeypot.

![image alt](https://github.com/fabianvagi91/Honeypot/blob/81a9cd8616c8ab3206f44f61d7f40f2186d27a46/logs.jpg) 

Inside the directory of pentbox we can see the logs of the honeypot that i made in port 22.
When i open the file i see the alerts made during the testing.

!IMPORTANT!

Pentbox only works when the terminal is runnning

# Conclusion

During the research i read a lot about different types of Honeypots and their capabilities.

Learned much more about well-known ports, reinforced my knowlage about firewalls rules and network protocols.

Practiced how to read logs and to extract usefull information form the logs


