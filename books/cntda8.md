---
title: "Computer Networking: a Top Down Approach(8ed)"
layout: home
parent: Books
aliases:
  - "Computer Networking: a Top Down Approach"
  - 计算机网络：自顶向下方法
  - 计算机网络：自顶向下方法：原书第8版
ISBN(s):
  - "9787111712367"
publisher(s):
  - "[[机工社]]"
丛书: "[[计算机科学丛书]]"
w3: http://gaia.cs.umass.edu/kurose_ross
tags:
  - communications
---

# Computer Networking: a Top Down Approach(8ed)

<div>
	<a href="https://www.pearson.com/en-us/subject-catalog/p/computer-networking/P200000003334/9780136681557">
		<img src="https://www.pearson.com/store//pmccommercewebservices/v2/medias/size-W370-bigcovers-0136681557.jpg?context=bWFzdGVyfGltYWdlc3w4NTQ3N3xpbWFnZS9qcGVnfHN5cy1tYXN0ZXIvaW1hZ2VzL2hlZS9oMjMvMTI5NDkyOTIyMjA0NDYvc2l6ZV9XMzcwXy9iaWdjb3ZlcnMvMDEzNjY4MTU1Ny5qcGd8ZDk4ZGQwYmU3MzdhMzZjZTVhNmYyYjViZTk2OWJjZmI2MjM5ODlmNTk0NzEwMWY3NDVjNzkwY2UzNTQxNTY2NQ" style="height: 200px;" border="1">
	</a>
	<a href="https://course.cmpreading.com/web/teachRes/detail/5410/216">
		<img src="https://course.cmpreading.com/resource/access/L29wZW5yZXNvdXJjZXMvdGVhY2hfZWJvb2svaW1hZ2UvMjAyMi8wOS96aXAvMmMyN2ViNGY3MTM4Nzc5YTQ2YzUyMWI5YmE2NzJiZmJfMjU2LmpwZWck6K6h566X5py6572R57ucIEExLmpwZw==" style="height: 200px;" border="1">
	</a>
</div>

## TOC

### Chapter 1: Computer Networks and the Internet

- 1.1 What Is the Internet?
    - 1.1.1 A Nuts-and-Bolts Description
    - 1.1.2 A Services Description
    - 1.1.3 What Is a Protocol?
- 1.2 The Network Edge
    - 1.2.1 Access Networks
    - 1.2.2 Physical Media
- 1.3 The Network Core
    - 1.3.1 Packet Switching
    - 1.3.2 Circuit Switching
    - 1.3.3 A Network of Networks
- 1.4 Delay, Loss, and Throughput in Packet-Switched Networks
    - 1.4.1 Overview of Delay in Packet-Switched Networks
    - 1.4.2 Queuing Delay and Packet Loss
    - 1.4.3 End-to-End Delay
    - 1.4.4 Throughput in Computer Networks
- 1.5 Protocol Layers and Their Service Models
    - 1.5.1 Layered Architecture
    - 1.5.2 Encapsulation
- 1.6 Networks Under Attack
- 1.7 History of Computer Networking and the Internet
    - 1.7.1 The Development of Packet Switching: 1961—1972
    - 1.7.2 Proprietary Networks and Internetworking: 1972—1980
    - 1.7.3 A Proliferation of Networks: 1980—1990
    - 1.7.4 The Internet Explosion: The 1990s
    - 1.7.5 The New Millennium
- 1.8 Summary

- Homework Problems and Questions
- Wireshark Lab

### Chapter 2: Application Layer

- 2.1 Principles of Network Applications
    - 2.1.1 Network Application Architectures
    - 2.1.2 Processes Communicating
    - 2.1.3 Transport Services Available to Applications
    - 2.1.4 Transport Services Provided by the Internet
    - 2.1.5 Application-Layer Protocols
    - 2.1.6 Network Applications Covered in This Book
- 2.2 The Web and HTTP
    - 2.2.1 Overview of HTTP
    - 2.2.2 Non-Persistent and Persistent Connections
    - 2.2.3 HTTP Message Format
    - 2.2.4 User-Server Interaction: Cookies
    - 2.2.5 Web Caching
    - 2.2.6 HTTP/2
- 2.3 Electronic Mail in the Internet
    - 2.3.1 SMTP
    - 2.3.2 Mail Message Formats
    - 2.3.3 Mail Access Protocols
- 2.4 DNS–The Internet’s Directory Service
    - 2.4.1 Services Provided by DNS
    - 2.4.2 Overview of How DNS Works
    - 2.4.3 DNS Records and Messages
- 2.5 Peer-to-Peer Applications
    - 2.5.1 P2P File Distribution
- 2.6 Video Streaming and Content Distribution Networks
    - 2.6.1 Internet Video
    - 2.6.2 HTTP Streaming and DASH
    - 2.6.3 Content Distribution Networks
    - 2.6.4 Case Studies: Netflix and YouTube
- 2.7 Socket Programming: Creating Network Applications
    - 2.7.1 Socket Programming with UDP
    - 2.7.2 Socket Programming with TCP
- 2.8 Summary

- Homework Problems and Questions
- Socket Programming Assignments
- Wireshark Labs: HTTP, DNS

### Chapter 3: Transport Layer

- 3.1 Introduction and Transport-Layer Services
    - 3.1.1 Relationship Between Transport and Network Layers
    - 3.1.2 Overview of the Transport Layer in the Internet
- 3.2 Multiplexing and Demultiplexing
- 3.3 Connectionless Transport: UDP
    - 3.3.1 UDP Segment Structure
    - 3.3.2 UDP Checksum
- 3.4 Principles of Reliable Data Transfer
    - 3.4.1 Building a Reliable Data Transfer Protocol
    - 3.4.2 Pipelined Reliable Data Transfer Protocols
    - 3.4.3 Go-Back-N (GBN)
    - 3.4.4 Selective Repeat (SR)
- 3.5 Connection-Oriented Transport: TCP
    - 3.5.1 The TCP Connection
    - 3.5.2 TCP Segment Structure
    - 3.5.3 Round-Trip Time Estimation and Timeout
    - 3.5.4 Reliable Data Transfer
    - 3.5.5 Flow Control
    - 3.5.6 TCP Connection Management
- 3.6 Principles of Congestion Control
    - 3.6.1 The Causes and the Costs of Congestion
    - 3.6.2 Approaches to Congestion Control
- 3.7 TCP Congestion Control
    - 3.7.1 Classic TCP congestion Control
    - 3.7.2 Network-Assisted Explicit Congestion Notification and Delay-based Congestion Control
    - 3.7.3 Fairness
- 3.8 Evolution of transport-layer functionality
- 3.9 Summary

- Homework Problems and Questions
- Programming Assignments
- Wireshark Labs: Exploring TCP, UDP

### Chapter 4: The Network Layer: Data Plane

- 4.1 Overview of Network Layer
    - 4.1.1 Forwarding and Routing: The Network Data and Control Planes
    - 4.1.2 Network Service Models
- 4.2 What’s Inside a Router?
    - 4.2.1 Input Port Processing and Destination-Based Forwarding
    - 4.2.2 Switching
    - 4.2.3 Output Port Processing
    - 4.2.4 Where Does Queuing Occur?
    - 4.2.5 Packet Scheduling
- 4.3 The Internet Protocol (IP): IPv4, Addressing, IPv6, and More
    - 4.3.1 IPv4 Datagram Format
    - 4.3.2 IPv4 Addressing
    - 4.3.3 Network Address Translation (NAT)
    - 4.3.4 IPv6
- 4.4 Generalized Forwarding and SDN
    - 4.4.1 Match
    - 4.4.2 Action
    - 4.4.3 OpenFlow Examples of Match-plus-action in Action
- 4.5 Middleboxes
- 4.6 Summary

- Homework Problems and Questions
- Wireshark Lab: IP

### Chapter 5: The Network Layer: Control Plane

- 5.1 Introduction
- 5.2 Routing Algorithms
    - 5.2.1 The Link-State (LS) Routing Algorithm
    - 5.2.2 The Distance-Vector (DV) Routing Algorithm
- 5.3 Intra-AS Routing in the Internet: OSPF
- 5.4 Routing Among the ISPs: BGP
    - 5.4.1 The Role of BGP
    - 5.4.2 Advertising BGP Route Information
    - 5.4.3 Determining the Best Routes
    - 5.4.4 IP-Anycast
    - 5.4.5 Routing Policy
    - 5.4.6 Putting the Pieces Together: Obtaining Internet Presence
- 5.5 The SDN Control Plane
    - 5.5.1 The SDN Control Plane: SDN Controller and SDN Control Applications
    - 5.5.2 OpenFlow Protocol
    - 5.5.3 Data and Control Plane Interaction: An Example
    - 5.5.4 SDN: Past and Future
- 5.6 ICMP: The Internet Control Message Protocol
- 5.7 Network Management, SNMP, and NETCONF/YANG
    - 5.7.1 The Network Management Framework
    - 5.7.2 The Simple Network Management Protocol (SNMP)
    - 5.7.3 NETCONF and YANG
- 5.8 Summary

- Homework Problems and Questions
- Socket Programming Assignment
- Programming Assignment
- Wireshark Lab: ICMP

### Chapter 6: The Link Layer and LANs

- 6.1 Introduction to the Link Layer
    - 6.1.1 The Services Provided by the Link Layer
    - 6.1.2 Where Is the Link Layer Implemented?
- 6.2 Error-Detection and -Correction Techniques
    - 6.2.1 Parity Checks
    - 6.2.2 Checksumming Methods
    - 6.2.3 Cyclic Redundancy Check (CRC)
- 6.3 Multiple Access Links and Protocols
    - 6.3.1 Channel Partitioning Protocols
    - 6.3.2 Random Access Protocols
    - 6.3.3 Taking-Turns Protocols
    - 6.3.4 DOCSIS: The Link-Layer Protocol for Cable Internet Access
- 6.4 Switched Local Area Networks
    - 6.4.1 Link-Layer Addressing and ARP
    - 6.4.2 Ethernet
    - 6.4.3 Link-Layer Switches
    - 6.4.4 Virtual Local Area Networks (VLANs)
- 6.5 Link Virtualization: A Network as a Link Layer
    - 6.5.1 Multiprotocol Label Switching (MPLS)
- 6.6 Data Center Networking
    - 6.6.1 Data Center Architectures
    - 6.6.2 Trends in Data Center Networking
- 6.7 Retrospective: A Day in the Life of a Web Page Request
    - 6.7.1 Getting Started: DHCP, UDP, IP, and Ethernet
    - 6.7.2 Still Getting Started: DNS and ARP
    - 6.7.3 Still Getting Started: Intra-Domain Routing to the DNS Server
    - 6.7.4 Web Client-Server Interaction: TCP and HTTP
- 6.8 Summary

- Homework Problems and Questions
- Wireshark Labs: Ethernet and Home Networking

### Chapter 7: Wireless and Mobile Networks

- 7.1 Introduction
- 7.2 Wireless Links and Network Characteristics
    - 7.2.1 CDMA
- 7.3 Wireless LANs
    - 7.3.1 The 802.11 Architecture
    - 7.3.2 The 802.11 MAC Protocol
    - 7.3.3 The IEEE 802.11 Frame
    - 7.3.4 Mobility in the Same IP Subnet
    - 7.3.5 Advanced Features in 802.11
    - 7.3.6 Bluetooth
- 7.4 Cellular Networks: 4G and 5G
    - 7.4.1 4G LTE Cellular Networks: Architecture and Elements
    - 7.4.2 LTE Protocol Stacks
    - 7.4.3 LTE Radio Access Network
    - 7.4.4 LTE Network Attachment and Power Management
    - 7.4.5 The Global Cellular Network: a Network of Networks
    - 7.4.6 5G Cellular Networks
- 7.5 Mobility Management: Principles
    - 7.5.1 Device Mobility: a Network-layer Perspective
    - 7.5.2 Home Networks and Roaming on Visited Networks
    - 7.5.3 Direct and Indirect Routing to/from a Mobile Device
- 7.6 Mobile Management in Practice
    - 7.6.1 Mobility Management in 4G/5G Networks
    - 7.6.2 Mobile IP
- 7.7 Wireless and Mobility: Impact on Higher-Layer Protocols
- 7.8 Summary

- Homework Problems and Questions
- Wireshark Lab: 802.11

### Chapter 8: Security in Computer Networks

- 8.1 What Is Network Security?
- 8.2 Principles of Cryptography
    - 8.2.1 Symmetric Key Cryptography
    - 8.2.2 Public Key Encryption
- 8.3 Message Integrity and Digital Signatures
    - 8.3.1 Cryptographic Hash Functions
    - 8.3.2 Message Authentication Code
    - 8.3.3 Digital Signatures
- 8.4 End-Point Authentication
    - 8.4.1 Building an Authentication Protocol
- 8.5 Securing E-Mail
    - 8.5.1 Secure E-Mail
    - 8.5.2 PGP
- 8.6 Securing TCP Connections: SSL
    - 8.6.1 The Big Picture
    - 8.6.2 A More Complete Picture
- 8.7 Network-Layer Security: IPsec and Virtual Private Networks
    - 8.7.1 IPsec and Virtual Private Networks (VPNs)
    - 8.7.2 The AH and ESP Protocols
    - 8.7.3 Security Associations
    - 8.7.4 The IPsec Datagram
    - 8.7.5 IKE: Key Management in IPsec
- 8.8 Securing Wireless LANs and 4G/5G Cellular Networks
    - 8.8.1 Authentication and Key Agreement in 802.11 Wireless LANs
    - 8.8.2 Authentication and Key Agreement in 4G/5G Cellular Networks
- 8.9 Operational Security: Firewalls and Intrusion Detection Systems
    - 8.9.1 Firewalls
    - 8.9.2 Intrusion Detection Systems
- 8.10 Summary

- Homework Problems and Questions
- Wireshark Lab: SSL
- IPsec Lab

---

Last Updated: Tue Oct  1 21:30:27 CST 2024
