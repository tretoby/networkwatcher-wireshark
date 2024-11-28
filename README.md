**Network Packet Capture in Azure with Network Watcher and Wireshark**

Objective

This project demonstrates the implementation of network packet capture and analysis using Azure Network Watcher and Wireshark. The goal is to showcase the ability to:
Configure and utilize Azure Network Watcher for capturing traffic in an Azure Virtual Network.
Analyze network traffic using Wireshark to identify patterns, potential vulnerabilities, and anomalies.
Gain hands-on experience in networking, cloud infrastructure, and security monitoring.

Skills Learned

Azure Cloud Infrastructure Management: Setting up Virtual Machines and Virtual Networks.
Network Monitoring: Capturing traffic using Azure Network Watcher’s packet capture feature.
Packet Analysis: Using Wireshark to inspect TCP/IP, HTTP, DNS, and other protocol packets.
Security Awareness: Identifying unusual network traffic and understanding basic network attack patterns.


Steps:
create a windows virtual machine
![image](https://github.com/user-attachments/assets/43be03d9-07f0-4402-87d2-b05e6e268c9e)

connect to to virtual machine then navigate to server manager (select add roles)
![image](https://github.com/user-attachments/assets/738e534a-6dd5-451a-b6ed-15b4c2d420a8)

install web server (IIS)

![image](https://github.com/user-attachments/assets/4db7dd4e-7203-4c03-b6b2-0b8c34d5eb81)

create a blob storage account
![image](https://github.com/user-attachments/assets/6d1add42-9243-48bb-ac08-7243128c5491)


In Azure navigate to network watcher and select packet capture
![image](https://github.com/user-attachments/assets/f17a39d4-5ec2-4bdf-9aa1-c726afa5d14a)

add resource group, and storage account, then set the time limit to 300 seconds
![image](https://github.com/user-attachments/assets/0687cb06-9428-4361-bbb3-32baf02424da)

navigate to target VM and select extentions to see the networkwatcher extention added to the virtual machine
![image](https://github.com/user-attachments/assets/7fd011fa-6e68-4c91-a246-1c4b0c4b8660)

navigate back to network watcher packet capture. The status should say loading while it is capturing the packets
![image](https://github.com/user-attachments/assets/abbb4678-8f74-4b00-a870-f61a2d874367)

now open up the web page by using the public ip of virtual machine to drive traffic to the server
![image](https://github.com/user-attachments/assets/4354baa8-3135-434f-b84e-d470b6b6052d)

stop packet capture
![image](https://github.com/user-attachments/assets/d1114d41-eac3-42b4-8f6f-176bb7ef3ef2)

navigate to the storage created previously, and select storage browser, blob containers, network watcher logs
![image](https://github.com/user-attachments/assets/eca65832-9bd5-4754-8c07-4f537025617b)

download packet capture log
![image](https://github.com/user-attachments/assets/1a48309b-5653-4434-8c8e-a61b56a961e8)

open wireshark and add downloaded file
![image](https://github.com/user-attachments/assets/0543a81d-4104-4a78-819b-733ee6014b61)

now you can see the contents of the capture file
![image](https://github.com/user-attachments/assets/260bebea-7ff2-4074-80f9-94b1959600dd)

filter using the port 80 that was previously used to connect to the virtual machine. filter = (ip.addr eq **** and tcp.port eq 80)
![image](https://github.com/user-attachments/assets/07380a3b-0d28-4d42-9966-d00229377d61)




















