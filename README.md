# Network Packet Capture and Analysis in Azure

## Project Overview

This hands-on cybersecurity and networking project demonstrates advanced techniques for network traffic capture and analysis using Microsoft Azure Network Watcher and Wireshark. The comprehensive lab provides practical experience in cloud infrastructure, network monitoring, and security analysis.

## Objective

The primary objectives of this project are to:
- Demonstrate advanced network monitoring techniques in cloud environments
- Implement packet capture using Azure Network Watcher
- Perform in-depth network traffic analysis with Wireshark
- Develop practical skills in cloud security and network forensics

## Skills Developed

- **Cloud Infrastructure Management**
  - Provisioning and configuring Azure Virtual Machines
  - Managing Virtual Network resources
  - Understanding cloud networking configurations

- **Network Monitoring**
  - Configuring Azure Network Watcher
  - Implementing packet capture techniques
  - Analyzing network traffic patterns

- **Packet Analysis**
  - Wireshark packet inspection
  - Protocol-level traffic analysis (TCP/IP, HTTP, DNS)
  - Identifying network communication characteristics

- **Security Awareness**
  - Recognizing potential network vulnerabilities
  - Understanding traffic flow and communication patterns
  - Basic network forensics and investigation techniques

## Prerequisites

- Microsoft Azure Account
- Active Subscription
- Windows or Linux Machine with:
  - Wireshark Installed
  - Azure CLI or Azure PowerShell (optional)

## Step-by-Step Laboratory Procedure

### 1. Azure Virtual Machine Preparation

#### 1.1 Create Windows Virtual Machine
- Navigate to Azure Portal
- Select "Virtual Machines"
- Click "Create"
- Choose Windows Server image
- Configure network settings
- Ensure necessary inbound ports are open (80, 443)

#### 1.2 Configure Web Server
- Connect to Virtual Machine via Remote Desktop
- Open Server Manager
- Navigate to "Add Roles and Features"
- Select and install Internet Information Services (IIS)

### 2. Network Monitoring Setup

#### 2.1 Create Storage Account
- Navigate to Azure Portal Storage Accounts
- Create a new storage account
- Generate a blob container for storing network captures

#### 2.2 Configure Network Watcher
- Access Network Watcher in Azure Portal
- Select "Packet Capture" option
- Choose target Virtual Machine
- Configure capture parameters:
  - Select Storage Account
  - Set time limit (recommended: 300 seconds)
  - Define capture filters (optional)

### 3. Traffic Generation and Capture

#### 3.1 Generate Network Traffic
- Access Virtual Machine's public IP address
- Open web browser
- Load IIS default page
- Perform basic interactions to generate network traffic

#### 3.2 Capture Network Packets
- Return to Network Watcher
- Stop packet capture
- Verify capture status and size

### 4. Packet Analysis with Wireshark

#### 4.1 Download Capture File
- Navigate to configured Storage Account
- Access Storage Browser
- Locate Network Watcher logs container
- Download packet capture file

#### 4.2 Wireshark Analysis
- Open Wireshark
- Load downloaded capture file
- Apply filters for focused analysis
  - Example filter: `(ip.addr == <VM_IP> and tcp.port == 80)`

## Recommended Filters for Investigation

- `http`: Display HTTP traffic
- `dns`: Analyze DNS queries
- `tcp.port == 80`: Web traffic
- `tcp.port == 443`: HTTPS traffic

## Security Considerations

- Always use strong authentication
- Implement least privilege access
- Regularly update and patch systems
- Monitor and log network activities

🏁 Conclusion
This network packet capture and analysis project bridges theoretical knowledge with practical cybersecurity skills. By leveraging Azure Network Watcher and Wireshark.




















