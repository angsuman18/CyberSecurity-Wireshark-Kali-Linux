# CyberSecurity-Wireshark-Kali-Linux

Wireshark is a network protocol analyzer that allows you to capture and interactively browse the traffic running on a computer network. It is widely used for network troubleshooting, analysis, software and protocol development, and education.

Here are some key features and uses of Wireshark:

1. **Live Capture and Offline Analysis**: Wireshark can capture data packets from a live network or read packets from a previously saved capture file.
2. **Deep Inspection**: It provides deep inspection of hundreds of protocols, with more being added all the time.
3. **Rich VoIP Analysis**: Wireshark can analyze Voice over IP (VoIP) calls in depth.
4. **Display Filters**: Powerful display filters allow you to focus on the packets you are interested in.
5. **Multi-Platform**: Wireshark runs on multiple operating systems, including Windows, Linux, macOS, Solaris, and others.
6. **Decryption Support**: Wireshark supports decrypting many protocols, including SSL/TLS, WEP, and WPA/WPA2.
7. **Extensive Capabilities**: It provides capabilities to create custom reports and statistics.
8. **Open Source**: Wireshark is released under the GNU General Public License (GPL).

### Basic Steps to Use Wireshark:

1. **Install Wireshark**: Download and install Wireshark from the official website [wireshark.org](https://www.wireshark.org/).
2. **Capture Packets**: Select the network interface to capture packets from and start the capture.
3. **Analyze Packets**: Use the provided filters and tools to analyze the captured data.
4. **Save and Export Data**: Save your captures and export them in various formats for further analysis.

### Common Use Cases:

- **Network Troubleshooting**: Identifying network issues by examining packet-level details.
- **Security Analysis**: Detecting security vulnerabilities and attacks.
- **Protocol Development**: Developing and testing network protocols.
- **Educational Purposes**: Learning about network protocols and how data travels across networks.


### Packets and Protocols in Networks

**Network Packets:**

A network packet is a formatted unit of data carried by a packet-switched network. It consists of control information and user data, which is also known as the payload. Packets are the basic units of data transfer in a network.

#### Components of a Network Packet:
1. **Header**: Contains metadata about the packet, such as source and destination addresses, packet sequencing information, and protocol details.
2. **Payload**: The actual data being transferred.
3. **Trailer**: Optional part used for error checking and control.

**Network Protocols:**

Network protocols are formal standards and policies comprised of rules, procedures, and formats that define communication between two or more devices over a network. They determine how data is transmitted, received, and processed across networks.

#### Types of Network Protocols:

1. **Application Layer Protocols**:
   - **HTTP/HTTPS**: Hypertext Transfer Protocol, used for transferring web pages.
   - **FTP**: File Transfer Protocol, used for transferring files.
   - **SMTP/POP3/IMAP**: Protocols for sending and receiving emails.

2. **Transport Layer Protocols**:
   - **TCP**: Transmission Control Protocol, provides reliable, ordered, and error-checked delivery of data.
   - **UDP**: User Datagram Protocol, provides a faster, connectionless service with no guarantee of delivery.

3. **Internet Layer Protocols**:
   - **IP**: Internet Protocol, responsible for addressing and routing packets.
   - **ICMP**: Internet Control Message Protocol, used for diagnostic and control purposes.
   - **ARP**: Address Resolution Protocol, maps IP addresses to physical MAC addresses.

4. **Link Layer Protocols**:
   - **Ethernet**: A protocol for wired local area networks.
   - **Wi-Fi**: A protocol for wireless local area networks.
   - **PPP**: Point-to-Point Protocol, used for direct communication between two network nodes.

#### Commonly Used Network Protocols:
- **HTTP/HTTPS**: For web browsing.
- **FTP/SFTP**: For file transfers.
- **SMTP/POP3/IMAP**: For email services.
- **DNS**: Domain Name System, translates domain names to IP addresses.
- **DHCP**: Dynamic Host Configuration Protocol, assigns IP addresses to devices on a network.
- **SNMP**: Simple Network Management Protocol, for managing devices on a network.

### Analyzing Packets with Wireshark:

Wireshark can capture and analyze packets from a variety of network protocols. Here are some basic steps to analyze packets:

1. **Capture Packets**:
   - Start Wireshark.
   - Select the network interface to capture packets from.
   - Click "Start" to begin capturing.

2. **Apply Filters**:
   - Use display filters to focus on specific packets (e.g., `http` to filter HTTP packets, `ip.addr == 192.168.1.1` to filter packets from/to a specific IP address).

3. **Inspect Packets**:
   - Click on a packet to view its detailed breakdown.
   - Examine the packet's header, payload, and trailer information.

4. **Analyze Protocols**:
   - Identify protocols used in the captured traffic.
   - Follow protocol streams (e.g., follow TCP stream) to analyze complete conversations.

Understanding packets and protocols is crucial for effective network analysis, troubleshooting, and security monitoring. 


Installing Wireshark on Kali Linux
Wireshark is typically pre-installed on Kali Linux, but if it’s not available or you need to update it, you can install it using the following steps:

Update the Package List:
Open a terminal and update the package list to ensure you have the latest versions:

sh
Copy code
sudo apt update
Install Wireshark:
Install Wireshark using the package manager:

sh
Copy code
sudo apt install wireshark
Configure Wireshark:
During the installation, you might be prompted to allow non-root users to capture packets. Select "Yes" to configure this setting.
