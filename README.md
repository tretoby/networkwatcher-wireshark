# Network Packet Capture and Analysis in Azure: Comprehensive Network Forensics Lab

## 🌐 Project Overview

This advanced cybersecurity laboratory demonstrates sophisticated network traffic capture and analysis techniques utilizing Microsoft Azure Network Watcher and Wireshark. The project provides a hands-on approach to understanding network infrastructure, traffic monitoring, and security analysis in cloud environments.

## 🎯 Objective

The primary goals of this network forensics project are to:
- Implement advanced network monitoring techniques in cloud infrastructure
- Leverage Azure Network Watcher for precise packet capture
- Perform comprehensive network traffic analysis using Wireshark
- Develop practical skills in cloud security and network investigation

## 🛠 Skills Developed

- **Cloud Infrastructure Management**
  - Azure Virtual Machine provisioning
  - Virtual network configuration
  - Cloud networking principles

- **Network Monitoring Techniques**
  - Azure Network Watcher configuration
  - Network traffic capture strategies
  - Traffic pattern identification

- **Advanced Packet Analysis**
  - Wireshark packet inspection
  - Protocol-level traffic analysis
  - Network communication pattern recognition

- **Cybersecurity Awareness**
  - Vulnerability detection
  - Traffic flow analysis
  - Network forensics fundamentals

## 📋 Prerequisites

- Microsoft Azure Account
- Active Azure Subscription
- Windows machine with:
  - Wireshark installed
  - Remote Desktop client

## 🚀 Step-by-Step Laboratory Procedure

### Step 1: Create Windows Virtual Machine
![Create Windows VM](https://github.com/user-attachments/assets/43be03d9-07f0-4402-87d2-b05e6e268c9e)

### Step 2: Configure Server Manager
![Server Manager Configuration](https://github.com/user-attachments/assets/738e534a-6dd5-451a-b6ed-15b4c2d420a8)

### Step 3: Install Web Server (IIS)
![Install IIS](https://github.com/user-attachments/assets/4db7dd4e-7203-4c03-b6b2-0b8c34d5eb81)

### Step 4: Create Blob Storage Account
![Create Storage Account](https://github.com/user-attachments/assets/6d1add42-9243-48bb-ac08-7243128c5491)

### Step 5: Access Network Watcher
![Network Watcher](https://github.com/user-attachments/assets/f17a39d4-7ec2-4bdf-9aa1-c726afa5d14a)


### Step 6: Configure Packet Capture
![Packet Capture Configuration](https://github.com/user-attachments/assets/0687cb06-9428-4361-bbb3-32baf02424da)

### Step 7: Verify Network Watcher Extension
![Network Watcher Extension](https://github.com/user-attachments/assets/7fd011fa-6e68-4c91-a246-1c4b0c4b8660)

### Step 8: Start Packet Capture
![Start Packet Capture](https://github.com/user-attachments/assets/abbb4678-8f74-4b00-a870-f61a2d874367)

### Step 9: Generate Web Traffic
![Generate Web Traffic](https://github.com/user-attachments/assets/4354baa8-3135-434f-b84e-d470b6b6052d)

### Step 10: Stop Packet Capture
![Stop Packet Capture](https://github.com/user-attachments/assets/4db7dd4e-7203-4c03-b6b2-0b8c34d5eb81)

### Step 11: Access Storage Browser
![Storage Browser](https://github.com/user-attachments/assets/eca65832-9bd5-4754-8c07-4f537025617b)

### Step 12: Download Packet Capture Log
![Download Capture Log](https://github.com/user-attachments/assets/1a48309b-5653-4434-8c8e-a61b56a961e8)

### Step 13: Open Capture in Wireshark
![Open in Wireshark](https://github.com/user-attachments/assets/0543a81d-4104-4a78-819b-733ee6014b61)

### Step 14: Analyze Packet Contents
![Packet Analysis](https://github.com/user-attachments/assets/260bebea-7ff2-4074-80f9-94b1959600dd)

### Step 15: Apply Advanced Filtering
![Apply Filters](https://github.com/user-attachments/assets/07380a3b-0d28-4d42-9966-d00229377d61)

## 🔍 Recommended Wireshark Filters

- `http`: HTTP traffic analysis
- `dns`: DNS query investigation
- `tcp.port == 80`: Web traffic examination
- `tcp.port == 443`: Secure web traffic analysis
- `ip.addr == <YOUR_VM_IP> and tcp.port == 80`: Targeted VM traffic

## 🛡️ Security Considerations

- Implement multi-factor authentication
- Use principle of least privilege
- Regularly update cloud resources
- Monitor and log network activities

