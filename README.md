# azure-network-protocols

<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

1- Determine which protocol you need to use: First, determine which protocol you need to use based on the requirements of your application or service. For example, if you need to transfer files between two virtual machines, you may choose to use TCP.

2- Create the necessary resources: Depending on the protocol you choose, you may need to create additional resources, such as virtual machines, virtual networks, or load balancers. You will need to configure these resources appropriately based on your protocol requirements.

3- Configure the protocol: Once you have the necessary resources in place, you will need to configure the protocol itself. This may involve setting up firewall rules, network security groups, or other security-related settings.

4- Test the protocol: After you have configured the protocol, you should test it to make sure it is functioning as expected. You can do this by using tools such as telnet or netcat to connect to the appropriate port and verify that the connection is successful.

5- Monitor and optimize: Finally, you should monitor your network traffic to ensure that the protocol is working efficiently and optimize it as needed. This may involve tweaking settings such as buffer sizes, timeout thresholds, or other performance-related parameters.

<h2>Actions and Observations</h2>

Actions:

1- Enable or disable a protocol: You can enable or disable a specific protocol on a virtual machine or virtual network interface. This can be done using Azure Portal, Azure CLI, or Azure PowerShell.

2- Configure firewall rules: Firewall rules are used to control incoming and outgoing traffic for specific protocols. You can configure firewall rules to allow or block traffic based on IP addresses, ports, and protocols.

3- Set up network security groups (NSGs): NSGs provide another layer of security for your virtual machines and virtual networks by filtering network traffic based on rules you define. You can create and manage NSGs using Azure Portal, Azure CLI, or Azure PowerShell.

4- Implement load balancing: Load balancing can help distribute network traffic across multiple virtual machines, providing higher availability and better performance. Azure Load Balancer and Application Gateway are two services that provide load balancing functionality.

5- Use Azure ExpressRoute: Azure ExpressRoute provides a dedicated, private connection between your on-premises infrastructure and Azure datacenters. This can help improve network performance and security for mission-critical workloads.

6- Monitor network traffic: Azure provides several monitoring tools, including Azure Network Watcher, that allow you to monitor and diagnose issues with your network traffic. You can use these tools to monitor network performance, detect and diagnose issues, and optimize your network for better performance.


Observations:

1- Transmission Control Protocol/Internet Protocol (TCP/IP): This is the most common network protocol used for communication over the internet. It is a reliable, connection-oriented protocol that provides error detection and correction.

2- User Datagram Protocol (UDP): UDP is a connectionless protocol that does not provide error detection or correction. It is often used for real-time applications that require low latency, such as voice and video streaming.

3- Hypertext Transfer Protocol (HTTP): HTTP is a protocol used for communication between web servers and web clients. Azure supports HTTP and HTTPS, which is a secure version of HTTP that uses SSL/TLS encryption.

4- File Transfer Protocol (FTP): FTP is a protocol used for transferring files over a network. Azure supports FTP and FTPS, which is a secure version of FTP that uses SSL/TLS encryption.

5- Server Message Block (SMB): SMB is a protocol used for file sharing and printer sharing over a network. Azure supports SMB and SMB over VPN or ExpressRoute for secure access to Azure File Shares.

6- Internet Control Message Protocol (ICMP): ICMP is a protocol used for network troubleshooting and diagnostics. Azure supports ICMP for ping and traceroute operations.

