# HomeLAB - OFFENSE & DEFENSE

During the course of my project ill be taking you through a Cybersecurity HomeLab.That dives into the world of attack and defense.This home lab composes of a windows server2025 with Active Directory,ubuntu desktop ,Postifx Mail Transfer Agent ,Security onion ,wazuh and linux.This project does require one to have 8GB or ram and 100GB of storage in my case i am using an external drive for this and aswell a 4cpu cores.

**Part 1** - Here we looking at setting up active directory. 

Active Directory (AD) is a system developed by Microsoft that helps organizations manage and organize their computers, users, and other resources in a network. Think of it like a digital phone book that stores important information and makes sure only the right people can access the right things. It's used to log in, control permissions, and keep everything secure and organized—making it a key part of most Windows-based business environments.Essentaily,AD is what we will utalize for enterprise network .so in our lab we are going to have all the users and servers under our active directory they all will be connected to our AD.

![image alt](https://github.com/sbuTech101/cybersecurity/blob/073a31c7ac03026dc6cf4a6dcf34397a2502c272/windows%20server%20enterprise/ChatGPT%20Image%20Sep%2022%2C%202025%2C%2012_16_30%20PM.png)

**Part 2 - SettingUp vulnerable Enviroment**

Next, we’ll be setting up intentional vulnerabilities in our enterprise lab environment. While not standard in real-world systems, this is done for learning and testing purposes—to better understand how attacks work and how to defend against them.
We’ll then deploy Wazuh, an open-source SIEM tool used for detecting, preventing, and responding to threats across on-prem, cloud, and containerized environments.

**Part 3 - Provisioning and setting Ubuntu Desktop**

This will be another workstation in our enterprise network, running Ubuntu—a popular Linux distribution based on Debian. Ubuntu is known for its stability, security, and ease of use, making it suitable for a wide range of environments, including cloud computing, servers, desktops, and IoT devices. It’s commonly used in both development and production settings across the tech industry.

PART 4 
SETTING UP UBUNTU DESKTOP.
What is Linux & Ubuntu?
Linux: Linux is an open-source operating system kernel that serves as the foundation for various.distributions (distros) like Ubuntu, Debian, Fedora, and CentOS. It is known for its flexibility, stability, and security, making it a popular choice for servers, desktops, and embedded systems.
Ubuntu: Ubuntu is a Linux distribution based on Debian, developed and maintained by Canonical. It is designed to be user-friendly, making it a go-to choice for beginners while remaining robust enough for advanced users and enterprise environments. Ubuntu is available in various editions: Desktop, Server, and Core (for IoT).


Connect Ubuntu Desktop to Active Directory
Since Ubuntu (and Linux-native operating systems) are not native to the Microsoft ecosystem. Connecting Ubuntu (and Debian-based systems) to Active Directory can be accomplished in a couple ways. The easiest way is to connect Ubuntu to Active Directory is with Samba Winbind can also be used to join Linux systems which we will be using as the are other methods but i chose this one specifically as it is more understandable for me and it is mostly supported to date.
why are connecting to it.
so we can have our user of the ubuntu destro part of work enterprise and under AD.

to connnect to active direcotry we are gonna be using About samba winbind.what is it ?
• Samba Winbind: A component of the Samba suite that allows Linux systems to authenticate users against Windows Active Directory (AD) and integrate with Windows network environments. Is a more direct integration, especially useful for legacy systems and environments where tight compatibility with Windows protocols is necessary. It’s often preferred when working in older Windows Server environments or where native Samba compatibility is crucial.


Part 5.
for our part 5 of the project we are going to be setting up windows 11 enterprise which will serve as our sec-client and we are connecting this client to our AD as part of our enterprise network users.Exciting stuff!
And while we at it will configure a network adapter for this client using IPV 4 .this will intail IP address allocation and subnetting.

Part 6 
On this part of the project we will be setting up an ubuntu server, which we will clone the ubuntu machine destro since it serves as the ubuntu user desktop now in this part we will be using the same image to create an Ubuntu server. 
This ubuntu server will be the heart of the business enterprise the first and last line of security.This server is also the email server 
We will also dive into why a dedicated security server is so important in business enterprise architecture and why the server is so important.
its we will also connect this server to our active directory domain,

part 7 
We setupp a security onion vm.This is our secure workstation.
Security Onion is a free, open-source platform for network security monitoring (NSM), log management, and intrusion detection. 
It provides a comprehensive suite of tools designed to help analysts detect, investigate, and respond to cyber threats in real time.

Part 8
Setup Postfix Mail Transfer Agent (MTA)
Postfix is a widely used open-source mail transfer agent (MTA) that routes and delivers email messages. 
Postfix is commonly used on Unix-like systems, including Linux distributions, as a server-side solution for managing emails.

Part 9
As we move deeper into the tactil side of things now we dive into SIEMS and here we wil be setting up Wazuh Open Source SIEM
so here as will be shown from the network desighn we will be working from our security server.
Wazuh is an open-source platform that provides extended detection response (XDR) and System Information and Event Management (SIEM) to protect cloud, container, and server workloads.
Wazuh comes with an array of capabilities including log data analytics, intrusion and malware detection, file integrity monitoring, configuration assessment, vulnerability detection, and support for regulatory compliance.

Part 10
On this part of the project we get our hands dirty.We are going to be Setting up The Attacker Machine
we will utalise kali linux.
Kali Linux is a specialized Linux distribution tailored for cybersecurity professionals and ethical hackers. Developed by Offensive Security, it is a Debian-based operating system preloaded with tools designed for penetration testing, ethical hacking, and digital forensics. Kali Linux is widely used for assessing system vulnerabilities, testing network security, and investigating cyber incidents.
Kali comes with a suite of security tools to assist.

Part 11 
in this part of the lab we will be configuring a vulnerable enviroment.
we are going to perform configuration changes to make our environment ‘vulnerable’.
Depending on the size, scale, and complexity of a business network, attackers will often leverage insecure and default configurations to their advantage.

Part 12 The initial Access we perform the attack.
