---
icon: '1'
---

# Networking Foundations

### Introduction to Networks

* Nodes - Individual devices connected to a network
* Links - Communication pathways that connect nodes (wired or wireless)

### OSI Model

OSI (Open Systems Interconnection) model has 7 layers: Physical, Data Link, Network, Transport, Session, Presentation, Application

#### 1. Physical Layer (Layer 1)

* Transmits raw bitstreams over a physical medium

#### 2. Data Link Layer (Layer 2)

* Provides node-to-node data transfer (direct link between 2 physically connected nodes)
* Ensures that data frames are transmitted with proper sync, error detection and correction
* Devices: Switches, bridges use MAC (Media Access Control) addresses

#### 3. Network Layer (Layer 3)

* Handles packet forwarding and routing to reach destination network
* Responsible for logical addressing and path determination
* Devices: Routers use IP (Internet Protocol) addresses

#### 4. Transport Layer (Layer 4)

* Responsible for (un-)reliable delivery of data, segmentation, reassembly of messages, flow control, and error checking
* Protocols: TCP (Transmission Control Protocol) and UDP (User Datagram Protocol)
* TCP: Reliable and connection-oriented with error recovery
* UDP: Faster and connectionless without guaranteed delivery

#### 5. Session Layer (Layer 5)

* Manages sessions between apps by establishing, maintaining and terminating connections, allowing devices to hold ongoing communications (sessions)
* Essential for session checkpointing and recovery to ensure data transfer resumes after interruptions
* Protocols and APIs coordinate communications between systems and apps

#### 6. Presentation Layer (Layer 6)

* Translator between app layer and network format
* Handles data representation such as encryption, decryption, compression and format conversion

#### 7. Application Layer (Layer 7)

* Provides network services directly to end-user apps (interface between the network and app)
* Enables resource sharing, remote file access, and other network services
* Protocols: HTTP, FTP, SMTP, DNS

### TCP/IP Model

TCP/IP (Transmission Control Protocol/Internet Protocol) model is a condensed version of the OSI model

#### 1. Link Layer

* Handles physical aspects of network such as Ethernet and Wi-Fi
* OSI equivalent: Physical layer, Data link layer

#### 2. Internet Layer

* Manages logical addressing of devices and routing of packets across networks
* Protocols: IP, ICMP
* OSI equivalent: Network layer

#### 3. Transport Layer

* Provides end-to-end communication services
* Ensures data packets are delivered sequentially and error-free
* Protocols: TCP, UDP
* OSI equivalent: Transport layer

#### 4. Application Layer

* Provides interfaces and protocols needed for data exchange between systems
* Protocols: HTTP, FTP, SMTP
* OSI equivalent: Session layer, Presentation layer, Application layer

### Protocols

Standardized rules that determine the formatting and processing of data to facilitate communication between devices in a network. Common protocols are HTTP, HTTPS, FTP, etc.

### Transmission

#### 1. Transmission Types

* Analog: Continuous signals to represent information (radio broadcasts)
* Digital: Discrete signals (bits) to encode data (modern tech)

#### 2. Transmission Modes

* Defines how data is sent between 2 devices
* Simplex mode: One-way communication only
* Half-duplex mode: Two-way communication but not simultaneuos (must take turns)
* Full-duplex mode: Simultaneous two-way communication

#### 3. Transmission Media

* Physical means by which data is transmitted in a network
* Wired media:
  * Twisted pair cables (Ethernet networks and LAN connections)
  * Coaxial cables (cable TV and early Ethernet)
  * Fiber optic cables (transmit data as light pulses for high-speed internet)
* Wireless media:
  * Radio waves (Wi-Fi and cellular networks)
  * Microwaves (Satellite commmunications)
  * Infrared (Short-range communications)

### Components of a Network

#### 1. End Devices (Hosts)

* Devices that sends or receives data within a network

#### 2. Intermediary Devices

* Facilitates data flow between end devices within a LAN or different networks by packet forwarding and have security features incorporated
* Network Interface Cards (NICs):
  * Hardware component installed in device that enables network connection
  * Each NIC has a unique MAC address
  * Can be designed for wired or wireless connections
* Routers:
  * Forward data packets between multiple networks and direct internet traffic
  * Operate at OSI network layer (layer 3) and reads network address info in data packets to determine their destinations
  * Use routing tables and routing protocols such as OSPF (Open Shortest Path First) or BGP (Border Gateway Protocol) to find most efficient path for data travel
* Switches
  * Primarily connect multiple devices within same network
  * Operate at OSI data link layer (layer 2) and use MAC addresses to forward data only to the intended recipient
  * Reduce network congestion and improve overall performance
* Hubs
  * Connects multiple devices in a network segment and broadcasts incoming data to all connected ports, regardless of destination
  * Operate at OSI physical layer (layer 1) and does not manage traffic intelligently, which can lead to network inefficiencies and collisions

#### 3. Network Media and Software Components

* Cabling and Connectors
* Network Protocols
  * Set of rules and conventions that control how data is formatted, transmitted, received, and interpreted across a network
  * Protocols encompass a wide range of aspects like Data Segmentation, Addressing, Routing, Error Checking, Synchronisation
* Network Management Software
  * Tools and apps to monitor, control and maintain network components and operations
  * Have functionalities like performance monitoring, configuration management, fault analysis, security management
* Software Firewalls (Host-based Firewalls)
  * Security app installed on individual devices to monitor and control incoming and outgoing network traffic based on predetermined security rules

#### 4. Servers

* Provide services to other computers (clients) over a network
* Facilitate service provision, enable resource sharing, handle data management and manage authentication

