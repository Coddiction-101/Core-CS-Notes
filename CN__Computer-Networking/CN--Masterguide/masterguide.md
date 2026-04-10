# 📖 01 — Computer Networks Masterguide
### Deep Theory | Complete Concepts | From Zero to Advanced

> **File:** `01_CN_Masterguide.md`
> **Part of:** Computer Networks Repository → [Back to README](./README.md)
> **Audience:** Complete beginners building a strong foundation
> **Pair with:** `03_CN_Practice_Repository.md` for hands-on labs

---

## 📌 Table of Contents

| # | Section |
|---|---------|
| 1 | [What Is a Computer Network — Really?](#1-what-is-a-computer-network--really) |
| 2 | [History and Evolution of Networking](#2-history-and-evolution-of-networking) |
| 3 | [Types of Networks](#3-types-of-networks) |
| 4 | [Network Topologies](#4-network-topologies) |
| 5 | [The OSI Model — All 7 Layers](#5-the-osi-model--all-7-layers) |
| 6 | [The TCP/IP Model](#6-the-tcpip-model) |
| 7 | [OSI vs TCP/IP — Complete Comparison](#7-osi-vs-tcpip--complete-comparison) |
| 8 | [Physical Layer — How Data Travels](#8-physical-layer--how-data-travels) |
| 9 | [Data Link Layer — Frame by Frame](#9-data-link-layer--frame-by-frame) |
| 10 | [Network Layer — IP and Routing](#10-network-layer--ip-and-routing) |
| 11 | [IP Addressing — IPv4 Deep Dive](#11-ip-addressing--ipv4-deep-dive) |
| 12 | [Subnetting — Complete Guide](#12-subnetting--complete-guide) |
| 13 | [IPv6 — The Future of Addressing](#13-ipv6--the-future-of-addressing) |
| 14 | [Transport Layer — TCP and UDP](#14-transport-layer--tcp-and-udp) |
| 15 | [Application Layer Protocols](#15-application-layer-protocols) |
| 16 | [DNS — The Internet's Phone Book](#16-dns--the-internets-phone-book) |
| 17 | [DHCP — Automatic IP Assignment](#17-dhcp--automatic-ip-assignment) |
| 18 | [Routing — How Packets Find Their Way](#18-routing--how-packets-find-their-way) |
| 19 | [Switching and VLANs](#19-switching-and-vlans) |
| 20 | [Wireless Networking — Wi-Fi](#20-wireless-networking--wi-fi) |
| 21 | [Network Security](#21-network-security) |
| 22 | [Network Devices — Complete Reference](#22-network-devices--complete-reference) |
| 23 | [Real-World Scenarios](#23-real-world-scenarios) |
| 24 | [Key Facts and Statistics](#24-key-facts-and-statistics) |
| 25 | [Learning Roadmap](#25-learning-roadmap) |
| 26 | [Common Mistakes to Avoid](#26-common-mistakes-to-avoid) |
| 27 | [What to Do While and After Learning](#27-what-to-do-while-and-after-learning) |
| 28 | [Career Paths and Certifications](#28-career-paths-and-certifications) |
| 29 | [Glossary](#29-glossary) |

---

---

# 1. What Is a Computer Network — Really?

## The Textbook Definition
A computer network is a collection of two or more computing devices connected together to **share resources**, **exchange data**, and **communicate** with each other.

## The Real Definition
That definition is technically correct but tells you nothing about why it matters or how deeply networking affects every moment of modern life. Here is the real picture.

Every time you send a WhatsApp message, watch a YouTube video, make a UPI payment, or open an email — a staggering amount of engineering happens in the background. Your message gets broken into pieces. Each piece gets labeled with addresses. Those pieces travel through wires, routers, undersea cables, and wireless signals across potentially thousands of kilometers. They get reassembled in the correct order at the destination and presented to your friend in under a second.

That entire journey — the rules that govern how data is broken, addressed, routed, reassembled, and verified — is what computer networking is about.

## Why Computer Networks Exist — Four Core Purposes

**1. Resource Sharing**
Before networks, if ten employees needed to print something, you needed ten printers. With a network, one printer serves all ten. The same applies to storage — one file server can be accessed by the entire office.

**2. Communication**
Email, video calls, messaging, collaboration tools — all of it is possible only because computers can communicate over networks. This transformed how businesses operate and how people connect globally.

**3. Centralized Management**
A network administrator can manage, update, monitor, and secure thousands of devices from a single location. Without a network, each device would need individual attention.

**4. Reliability Through Redundancy**
Networks can be designed so that if one path fails, data automatically finds another route. This redundancy makes critical systems — hospitals, banks, airports — resistant to failure.

## Scale: From Two Computers to the Entire Internet

A network can be as small as two laptops connected by a cable, or as large as the entire internet — a global network of billions of devices connected through millions of routers, thousands of ISPs, and hundreds of undersea cables. The same fundamental principles govern both.

---

---

# 2. History and Evolution of Networking

Understanding history explains why networks are designed the way they are. Every design decision has a reason rooted in a problem that needed solving.

## 1960s — The Seed Is Planted

The United States Department of Defense funded **ARPANET** (Advanced Research Projects Agency Network) — the direct ancestor of today's internet. The driving idea was extraordinary: design a communication network that could survive a nuclear attack. If any part of the network was destroyed, data would automatically route around the damage through surviving paths.

This decentralized, fault-tolerant design philosophy is embedded in the internet's architecture to this day. In 1969, ARPANET connected its first four nodes: UCLA, Stanford Research Institute, UC Santa Barbara, and the University of Utah. The first message sent was "LO" — the system crashed before completing "LOGIN."

## 1970s — Protocols Are Born

**Vint Cerf** and **Bob Kahn** developed **TCP/IP** — the Transmission Control Protocol / Internet Protocol. This was revolutionary: it gave all computers a common language, regardless of manufacturer or operating system. Any device that speaks TCP/IP can communicate with any other device that speaks TCP/IP. Cerf and Kahn are rightly called the **"Fathers of the Internet."**

## 1980s — Standards and Growth

**DNS (Domain Name System)** was created in 1983, replacing the cumbersome practice of maintaining a single shared text file that mapped hostnames to IP addresses. As the network grew, a single file could not scale.

**Ethernet**, developed by Bob Metcalfe at Xerox PARC, became the dominant local area network standard — and still is today, though dramatically evolved.

In 1983, ARPANET formally adopted TCP/IP. This is considered the official birthday of the internet.

## 1989–1991 — The Web Changes Everything

**Tim Berners-Lee** at CERN invented the **World Wide Web** — HTTP, HTML, and URLs. It is critical to understand: the web is NOT the internet. The web is an application that runs ON TOP of the internet, the same way email or DNS is an application. But the web democratized access to information and transformed the internet from a tool for researchers into a tool for everyone.

## 1990s — Commercial Internet Arrives

Internet Service Providers (ISPs) proliferated. Dial-up modems connected homes over telephone lines at 56 Kbps. Browsers like Netscape made the web visual and accessible. Email became the primary business communication tool. The dot-com era began — and eventually crashed in 2000-2001.

## 2000s — Broadband and the Mobile Revolution

DSL and cable broadband replaced dial-up. Wi-Fi (IEEE 802.11) became ubiquitous in homes, offices, and coffee shops. The iPhone launched in 2007 and changed the internet forever — a computer in everyone's pocket, connected always.

## 2010s–Present — Cloud, IoT, and 5G

Cloud computing moved applications off individual devices onto networked servers. The Internet of Things connected billions of non-computer devices (sensors, cameras, vehicles, appliances). 5G networks began delivering multi-gigabit wireless speeds. Video calling became routine. Software-Defined Networking (SDN) began separating network control intelligence from physical hardware.

The network is now the foundation of every industry — healthcare, finance, manufacturing, agriculture, education, and government all depend on it.

---

---

# 3. Types of Networks

Networks are classified by their **geographic scope**, **ownership**, and **purpose**. Understanding these types helps you understand which technologies apply where.

## PAN — Personal Area Network

**Scale:** ~10 meters — the space around a single person
**Purpose:** Connect personal devices around one individual
**Technologies:** Bluetooth, NFC (Near Field Communication), Infrared, Zigbee

Examples:
- Bluetooth connecting your phone to wireless earbuds
- NFC enabling a contactless payment at a store
- A smartwatch syncing data with your phone

PANs are the smallest networks. They require no infrastructure — devices connect directly to each other.

## LAN — Local Area Network

**Scale:** Single building or campus (up to ~1 km)
**Purpose:** Connect devices within a home, office, school, or small campus
**Technologies:** Ethernet (IEEE 802.3), Wi-Fi (IEEE 802.11)
**Ownership:** Privately owned and managed

Examples:
- Your home Wi-Fi network connecting your phone, laptop, and smart TV
- A company's office network connecting all workstations, printers, and servers
- A school computer lab

LANs offer **high speed** (100 Mbps to 10 Gbps) and **low latency** because devices are physically close. They are the most common type of network that most people work with directly.

## MAN — Metropolitan Area Network

**Scale:** A city or metropolitan area (5–50 km)
**Purpose:** Connect multiple LANs across a city
**Technologies:** Fiber optic, WiMAX (IEEE 802.16)
**Ownership:** ISPs, telecommunications companies, city governments

Examples:
- A cable television network serving a city
- A city-wide Wi-Fi network in a smart city initiative
- A university with multiple campuses connected across a city

## WAN — Wide Area Network

**Scale:** Countries, continents, or globally
**Purpose:** Connect networks across large geographic distances
**Technologies:** Fiber optic cables (terrestrial and submarine), satellite, MPLS, leased lines
**Ownership:** Multiple organizations — ISPs own different segments

Examples:
- **The internet is the largest WAN in existence**
- A multinational company connecting its offices across India, the US, and Europe
- An ATM network connecting banks across a country

WANs are typically slower than LANs (due to distance) and have higher latency. They are usually leased from telecommunications providers rather than owned outright.

## CAN — Campus Area Network

**Scale:** Multiple buildings on a connected campus (larger than LAN, smaller than MAN)
**Purpose:** Connect buildings on a university, hospital, or corporate campus

Example: IIT Bombay's network connecting all academic buildings, hostels, and admin offices.

## SAN — Storage Area Network

**Scale:** Within a data center
**Purpose:** High-speed network dedicated to connecting servers to storage devices
**Technologies:** Fiber Channel, iSCSI

SANs are specialized networks — not general-purpose. They exist to give servers fast, reliable access to shared storage arrays in data centers.

## Key Comparison Table

| Type | Scale | Speed | Example | Owned By |
|------|-------|-------|---------|---------|
| PAN | ~10m | Low | Bluetooth earbuds | Individual |
| LAN | Building | Very High | Home/office Wi-Fi | Individual/Company |
| MAN | City | High | City Wi-Fi | ISP/Government |
| WAN | Country/Globe | Medium | Internet | Multiple ISPs |
| CAN | Campus | Very High | University network | University |
| SAN | Data center | Extremely High | Server storage | Company |

---

---

# 4. Network Topologies

Topology is the arrangement of nodes (devices) and links (connections) in a network. There are two types:

- **Physical topology:** How cables actually run and devices are physically placed
- **Logical topology:** How data actually flows, regardless of physical layout

## Bus Topology

```
PC1 --- PC2 --- PC3 --- PC4 --- PC5
|_________________________________|
              BUS / BACKBONE
       [Terminator]       [Terminator]
```

**How it works:** All devices connect to a single shared cable — the bus. Data travels in both directions along the cable. Every device sees all traffic and checks if data is addressed to it.

**Terminators** at each end absorb signals to prevent them from bouncing back and causing interference.

| Advantages | Disadvantages |
|-----------|--------------|
| Simple and inexpensive to install | Single point of failure — bus breaks = entire network fails |
| Easy to add new devices | Performance degrades with more devices (more collisions) |
| Less cable than star topology | Difficult to troubleshoot |
| | Limited cable length |

**Status:** Obsolete. Used in very early Ethernet (10BASE2, 10BASE5). No longer deployed.

---

## Ring Topology

```
    PC1
   /    \
PC4      PC2
   \    /
    PC3
```

**How it works:** Each device connects to exactly two others, forming a ring. Data travels in one direction (unidirectional ring) or both directions (bidirectional/dual ring). A **token** (special control frame) passes around the ring — a device can only transmit when it holds the token.

| Advantages | Disadvantages |
|-----------|--------------|
| Predictable, orderly data flow | One broken device or cable breaks the entire ring |
| No data collisions (token controls access) | Adding/removing devices disrupts the network |
| Each device acts as a repeater | Slower than star topology |

**Examples:** Token Ring (IBM), FDDI (Fiber Distributed Data Interface)
**Status:** Largely obsolete. Dual-ring designs still used in some fiber backbone networks for redundancy.

---

## Star Topology

```
        PC1
         |
PC4 --- Switch --- PC2
         |
        PC3
```

**How it works:** All devices connect to a central device — typically a **switch** (or hub in old networks). All data goes through this central point. The central device manages forwarding.

| Advantages | Disadvantages |
|-----------|--------------|
| Failure of one device does not affect others | Central device is a single point of failure |
| Easy to add or remove devices | More cabling required than bus |
| Easy to troubleshoot — isolate central device or individual connection | More expensive (needs a switch) |
| High performance with modern switches | |

**Status:** The **dominant topology in modern networks**. Every home Wi-Fi network is a star topology — all devices connect to the router/access point.

---

## Mesh Topology

```
PC1 ——— PC2
|  \  / |
|   \/  |
|   /\  |
|  /  \ |
PC4 ——— PC3
```

**Full Mesh:** Every device connects to every other device directly.
**Number of connections** in a full mesh with n nodes = **n(n-1)/2**

**Partial Mesh:** Only some devices have multiple connections — a compromise between cost and redundancy.

| Advantages | Disadvantages |
|-----------|--------------|
| Extremely high redundancy | Very expensive — huge amount of cabling |
| Multiple paths — failure of any single link doesn't disrupt communication | Complex to manage and configure |
| High overall bandwidth | Impractical for large numbers of devices |

**Use:** The internet's backbone uses partial mesh. Military networks, financial institutions, and critical infrastructure use full mesh for critical nodes.

---

## Tree (Hierarchical) Topology

```
                [Root Switch]
               /             \
        [Switch A]         [Switch B]
        /       \           /       \
    [PC1]     [PC2]     [PC3]     [PC4]
```

**How it works:** A hierarchy of star networks. Root node at top, branches below. Used in large enterprise and campus networks where departments connect to a distribution switch, which connects to a core switch.

| Advantages | Disadvantages |
|-----------|--------------|
| Scalable — easy to add branches | Root node failure affects everything below |
| Organized — logical hierarchy maps to organizational structure | More complex than a flat star |
| Easy to manage segments independently | |

---

## Hybrid Topology

Most real-world networks combine multiple topologies. For example:
- Each department uses a **star topology** (devices connect to a switch)
- Departments connect to each other using a **partial mesh** (for redundancy)
- The entire organization connects to the internet via a **tree hierarchy**

This combination is called a **hybrid topology**.

---

---

# 5. The OSI Model — All 7 Layers

## Why the OSI Model Exists

Before the OSI model, different vendors created incompatible networking systems. An IBM computer could not communicate with a DEC computer. Cisco routers could not interoperate with 3Com switches. Every vendor had their own proprietary protocols.

The **International Organization for Standardization (ISO)** developed the OSI (Open Systems Interconnection) model in **1984** as a universal reference framework. It divides the enormous problem of network communication into **seven distinct, manageable layers**, each with a specific, well-defined responsibility.

The genius of the layered model:
- Each layer only communicates with the layers directly above and below it
- Each layer provides services to the layer above it
- Each layer uses services from the layer below it
- Changing the implementation of one layer does not affect others

Think of it like building construction. The plumbing team, electrical team, and structural team each do their specific job. They interact at defined points (water pipes go through walls made by structural team) but each team works independently on their domain.

## The 7 Layers — Master Reference

```
┌─────────────────────────────────────────────────────────────────────────┐
│ #  │   Layer Name   │ Data Unit │  Key Protocols        │ Key Devices    │
├─────────────────────────────────────────────────────────────────────────┤
│ 7  │  Application   │  Message  │ HTTP,FTP,DNS,SMTP,SSH │ Gateway, Proxy │
│ 6  │  Presentation  │  Data     │ SSL/TLS, JPEG, MPEG   │ —              │
│ 5  │  Session       │  Data     │ NetBIOS, RPC, PPTP    │ —              │
│ 4  │  Transport     │  Segment  │ TCP, UDP              │ Firewall, LB   │
│ 3  │  Network       │  Packet   │ IP, ICMP, ARP, OSPF   │ Router         │
│ 2  │  Data Link     │  Frame    │ Ethernet, Wi-Fi, PPP  │ Switch, Bridge │
│ 1  │  Physical      │  Bit      │ Ethernet cables, DSL  │ Hub, Repeater  │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## Layer 7 — Application Layer

**What it is:** The topmost layer. The interface between the network and the software applications that use it.

**Critical clarification:** This layer does NOT refer to applications like Chrome, WhatsApp, or Gmail. It refers to the **network protocols** those applications use. Chrome uses HTTP/HTTPS. Gmail uses SMTP (to send) and IMAP (to receive).

**Responsibilities:**
- Provides network services directly to end-user applications
- Handles high-level protocols for email, file transfer, web browsing
- Identifies communication partners and checks resource availability

**Protocols:** HTTP (web browsing), HTTPS (secure web), FTP (file transfer), SMTP (send email), POP3/IMAP (receive email), DNS (name resolution), DHCP (IP assignment), SSH (secure remote access), Telnet (remote access), SNMP (network management)

**Data Unit:** Message / Data

---

## Layer 6 — Presentation Layer

**What it is:** The translator of the OSI model. Ensures that data sent by one system can be read and understood by another, even if they use different formats.

**Responsibilities:**
- **Data translation:** Converts between different character encoding formats (e.g., EBCDIC used by IBM mainframes vs ASCII used by most systems)
- **Encryption/Decryption:** SSL/TLS encryption operates here — data is encrypted before being passed down to the Transport layer
- **Compression:** Reduces data size for efficient transmission — JPEG (images), MPEG (video), GIF (animations)

**Key insight for interviews:** When people say "SSL/TLS operates at the Application layer," they are referring to the TCP/IP model (which combines layers 5–7 into "Application"). In the OSI model, TLS is in the Presentation layer.

**Data Unit:** Data

---

## Layer 5 — Session Layer

**What it is:** Manages the communication sessions between two applications.

**Responsibilities:**
- **Session establishment:** Setting up a communication session between two applications
- **Session maintenance:** Keeping the session alive, handling breaks
- **Session termination:** Properly closing the session when done
- **Dialog control:** Determining who speaks at a given time (half-duplex vs full-duplex)
- **Synchronization:** Adding checkpoints to long transfers so they can resume after a failure rather than starting over

**Analogy:** Think of a phone call. Someone initiates it (establishment), both parties talk (maintenance), and someone says "goodbye" and hangs up (termination). The Session layer manages exactly this for application-to-application communication.

**Protocols:** NetBIOS, RPC (Remote Procedure Call), PPTP

**Data Unit:** Data

---

## Layer 4 — Transport Layer

**What it is:** The layer responsible for **end-to-end communication** between applications on different hosts. This is one of the most critical layers.

**Responsibilities:**
- **Segmentation:** Breaks large data from the Application layer into smaller **segments**. If a file is 10MB and the maximum segment size is 1460 bytes, Transport breaks it into thousands of segments.
- **Reassembly:** At the receiver, reassembles segments back into the original data in the correct order
- **Port numbers:** Identifies which application each segment belongs to. Port 80 = HTTP, Port 443 = HTTPS, Port 22 = SSH. Multiple applications can use the network simultaneously because each has a different port number.
- **Flow control:** Receiver tells sender how much data it can handle — prevents the sender from overwhelming the receiver's buffer
- **Error control:** Detects lost or corrupted segments and requests retransmission
- **Multiplexing:** Multiple applications sending data simultaneously, all sharing the same network connection

**Protocols:**
- **TCP** (Transmission Control Protocol) — reliable, ordered, connection-oriented
- **UDP** (User Datagram Protocol) — fast, connectionless, unreliable

**Data Unit:**
- TCP produces **Segments**
- UDP produces **Datagrams**

**Key devices:** Load balancers, firewalls (when filtering by port)

---

## Layer 3 — Network Layer

**What it is:** Responsible for **logical addressing** and **routing** — determining the best path for data to travel from source to destination, potentially across many different networks.

**The critical distinction from Layer 2:** Layer 2 handles delivery within the same network (your home network). Layer 3 handles delivery across different networks (your home → your ISP → internet → YouTube's servers).

**Responsibilities:**
- **Logical addressing:** Assigns IP addresses to packets. Unlike MAC addresses (Layer 2) which are hardware-assigned, IP addresses are logical — they can be configured, changed, and encode location information.
- **Routing:** When a packet arrives at a router, the router examines the destination IP address and consults its routing table to determine which direction to forward the packet. This happens at every router along the path.
- **Fragmentation:** If a packet is too large for a link it must traverse, the Network layer can break it into smaller fragments (IPv4 only; IPv6 routers do not fragment).

**Protocols:** IP (IPv4, IPv6), ICMP, OSPF, BGP, RIP

**Key device: Router**

**Data Unit:** Packet

---

## Layer 2 — Data Link Layer

**What it is:** Responsible for **node-to-node delivery** of data on the same network segment. While the Network layer handles global addressing, the Data Link layer handles local delivery.

**Sub-layers:**
- **LLC (Logical Link Control):** Interfaces with the Network layer, provides error detection
- **MAC (Media Access Control):** Controls how devices access the shared medium, handles MAC addressing

**Responsibilities:**
- **Framing:** Encapsulates packets from the Network layer into **frames** by adding a header (containing source and destination MAC addresses) and a trailer (containing error-checking information)
- **Physical addressing:** MAC addresses identify devices on the local network segment
- **Error detection:** CRC (Cyclic Redundancy Check) in the frame trailer detects transmission errors
- **Medium access control:** Determines when a device can transmit to avoid collisions (CSMA/CD for wired Ethernet, CSMA/CA for Wi-Fi)
- **Flow control:** Basic flow control at the frame level

**Protocols:** Ethernet (IEEE 802.3), Wi-Fi (IEEE 802.11), PPP, ARP

**Key devices: Switch**, Bridge, NIC (Network Interface Card)

**Data Unit:** Frame

---

## Layer 1 — Physical Layer

**What it is:** The lowest layer. Concerned entirely with the actual transmission of raw **bits** (0s and 1s) over a physical medium.

**Responsibilities:**
- Defines the electrical/optical/radio signals that represent bits
- Specifies cable types, connector shapes, pin layouts
- Defines transmission rates (bits per second)
- Manages bit synchronization — ensures sender and receiver agree on exactly when each bit starts and ends

**Key point:** There is NO addressing at this layer. It simply moves bits. The Physical layer has no idea what those bits mean — it just ensures 1s arrive as 1s and 0s arrive as 0s.

**Technologies:** Cat5e, Cat6, Cat6A cables; Fiber optic cables; Coaxial cable; Radio waves (Wi-Fi signals); DSL over telephone lines; USB

**Key devices:** Hubs, Repeaters, Network cables themselves, NIC (physical components)

**Data Unit:** Bit

---

## Encapsulation — The Most Important Process in Networking

Every time data travels down through the OSI layers on the sender's side, each layer **adds its own header** (and sometimes a trailer) to the data. This process is called **encapsulation**.

At the receiver, each layer **strips its header** as data travels up. This is called **decapsulation**.

```
SENDER SIDE (Data traveling DOWN through layers):

Application  │ [  USER DATA  ]
             │
Transport    │ [TCP HEADER][  USER DATA  ]         ← Segment
             │
Network      │ [IP HEADER][TCP HEADER][  DATA  ]   ← Packet
             │
Data Link    │ [ETH HDR][IP HDR][TCP HDR][DATA][FCS] ← Frame
             │
Physical     │ 0101010110100101...                  ← Bits on wire


RECEIVER SIDE (Data traveling UP through layers):

Physical     │ 0101010110100101... received
             │
Data Link    │ [ETH HDR][IP HDR][TCP HDR][DATA][FCS]
             │  Strip Ethernet header + check FCS
Network      │ [IP HDR][TCP HDR][DATA]
             │  Strip IP header
Transport    │ [TCP HDR][DATA]
             │  Strip TCP header, reassemble
Application  │ [  USER DATA  ]  ← Original data delivered
```

**The most important rule in all of networking:**
- **Layer 2 (MAC addresses) changes at every hop** — each router creates a new frame with new MAC addresses
- **Layer 3 (IP addresses) stays the same end-to-end** — source and destination IP never change in transit

---

## Peer Communication — The Illusion of Direct Layer-to-Layer Talk

Even though data physically passes through many layers and devices, each layer on the sender communicates **logically** with the same layer on the receiver. The Transport layer on your laptop appears to talk directly to the Transport layer on Google's server, even though the data passes through 15 routers in between. Each layer uses its protocol headers to achieve this.

```
Your Laptop                         Google's Server
────────────                        ──────────────
[Application] ◄──── HTTP ──────────► [Application]
[Transport  ] ◄──── TCP  ──────────► [Transport  ]
[Network    ] ◄──── IP   ──────────► [Network    ]
[Data Link  ] ◄─ Ethernet ─────────► [Data Link  ]
[Physical   ] ◄─── Bits  ──────────► [Physical   ]
              (through many routers)
```

---

## OSI Mnemonics

**Layers 7 to 1 (Top to Bottom):**
**A**ll **P**eople **S**eem **T**o **N**eed **D**ata **P**rocessing
Application → Presentation → Session → Transport → Network → Data Link → Physical

**Layers 1 to 7 (Bottom to Top):**
**P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way
Physical → Data Link → Network → Transport → Session → Presentation → Application

---

---

# 6. The TCP/IP Model

## What Is the TCP/IP Model?

The TCP/IP model (also called the **Internet Model** or **DoD Model**) is the practical model that the actual internet runs on. While the OSI model is the reference framework used for understanding and teaching, TCP/IP is what is actually implemented in every device connected to the internet.

TCP/IP was developed in the 1970s — before the OSI model — and has 4 layers:

```
┌──────────────────────────────────────────────────────────────┐
│  Layer 4  │  Application   │ HTTP, HTTPS, FTP, DNS, SMTP     │
│           │                │ SSH, Telnet, DHCP, SNMP          │
├──────────────────────────────────────────────────────────────┤
│  Layer 3  │  Transport     │ TCP, UDP                         │
├──────────────────────────────────────────────────────────────┤
│  Layer 2  │  Internet      │ IP (v4/v6), ICMP, ARP, IGMP     │
├──────────────────────────────────────────────────────────────┤
│  Layer 1  │  Network Access│ Ethernet, Wi-Fi, PPP             │
│           │  (Link Layer)  │ Physical cables + Data Link      │
└──────────────────────────────────────────────────────────────┘
```

## TCP/IP Layer Details

### Layer 4 — Application Layer
Combines OSI Layers 5 (Session), 6 (Presentation), and 7 (Application) into one.
All application-level protocols live here — HTTP, HTTPS, FTP, SMTP, DNS, DHCP, SSH, SNMP.
The application itself handles any session management or data formatting it needs.

### Layer 3 — Transport Layer
Identical to OSI Layer 4.
TCP and UDP operate here.
Port numbers identify applications.
TCP provides reliable, ordered delivery. UDP provides fast, connectionless delivery.

### Layer 2 — Internet Layer
Corresponds to OSI Layer 3 (Network).
IP addressing and routing are the core functions.
Key protocols: IP (v4 and v6), ICMP (ping, error reporting), ARP (IP to MAC resolution), IGMP (multicast management).

### Layer 1 — Network Access Layer (Link Layer)
Combines OSI Layers 1 (Physical) and 2 (Data Link).
Handles the actual transmission of data on the physical medium.
Includes Ethernet framing, Wi-Fi transmission, physical cables, and all hardware-level functions.

---

---

# 7. OSI vs TCP/IP — Complete Comparison

## Side-by-Side Layer Mapping

```
OSI Model                  TCP/IP Model
─────────────────          ─────────────────
7. Application   ─┐
6. Presentation  ─┤──────► Application Layer
5. Session       ─┘
                 
4. Transport     ──────────► Transport Layer

3. Network       ──────────► Internet Layer

2. Data Link     ─┐
1. Physical      ─┴──────►  Network Access Layer
```

## Comparison Table

| Feature | OSI Model | TCP/IP Model |
|---------|-----------|--------------|
| Full Name | Open Systems Interconnection | Transmission Control Protocol/Internet Protocol |
| Developed By | ISO | DARPA |
| Year | 1984 | 1970s |
| Number of Layers | 7 | 4 |
| Primary Purpose | Conceptual reference/teaching | Practical implementation |
| Usage Today | Troubleshooting and education | Actual internet operation |
| Protocol Specific? | Protocol-independent (generic) | Protocol-specific (TCP, IP) |
| Transport Layer | Any transport protocol | TCP and UDP specifically |
| Reliability Handling | Can be at multiple layers | Primarily at Transport (TCP) |
| Approach | Top-down (theory first) | Bottom-up (practical first) |
| Flexibility | More granular (7 layers) | Simpler (4 layers) |

## The Key Insight

**OSI** = The map. Use it to understand, explain, and troubleshoot networking. When an interviewer asks "at which layer does X operate?" — they want the OSI answer.

**TCP/IP** = The road. Use it to describe what actually happens on the internet. Real implementation uses TCP/IP.

Both models describe the same reality — just organized differently. Knowing how to map between them fluently is a sign of genuine understanding.

---

---

# 8. Physical Layer — How Data Travels

The Physical layer is where all the abstraction ends and raw physics begins. This is where software becomes electricity, light, or radio waves.

## Transmission Media

### Wired Media — Guided

**Twisted Pair Cable**
The most common network cabling in the world. Two copper wires twisted around each other inside a plastic jacket. The twist is crucial — it dramatically reduces **electromagnetic interference (EMI)** because adjacent twists cancel each other's interference signals.

```
Cross-section of UTP Cable:
┌─────────────────────────┐
│  ○─ ─○  ○─ ─○  ○─ ─○  │
│  pair1  pair2  pair3   │
│  twisted, twisted       │
└─────────────────────────┘
```

**UTP (Unshielded Twisted Pair)** — The standard.

| Standard | Max Speed | Max Distance | Use |
|----------|----------|-------------|-----|
| Cat 5e | 1 Gbps | 100m | Older office networks |
| Cat 6 | 10 Gbps | 55m (10G) / 100m (1G) | Modern offices |
| Cat 6A | 10 Gbps | 100m | Data centers, modern offices |
| Cat 7 | 10 Gbps | 100m | High-interference environments |
| Cat 8 | 40 Gbps | 30m | Data center switches |

**STP (Shielded Twisted Pair)** — Has additional metallic shielding around each pair or the entire cable. Used in high-interference environments (near heavy machinery, radio equipment).

---

**Fiber Optic Cable**
Transmits data as **pulses of light** rather than electrical signals. The core is ultra-pure glass or plastic. Light undergoes **total internal reflection** — it bounces off the inner walls of the glass core and travels forward, staying contained even around gentle bends.

```
Fiber Optic Cross-Section:
┌────────────────────────┐
│  ╔══════╗             │  ← Outer jacket
│  ║ Core ║             │  ← Cladding (lower refractive index)
│  ╚══════╝             │  ← Core (higher refractive index)
└────────────────────────┘
Light bounces via total internal reflection →→→→→→→→
```

**Single-Mode Fiber (SMF):**
- Very thin core (~9 micrometers)
- Uses laser as light source
- Supports very long distances (tens to hundreds of kilometers)
- Used for intercity connections, ISP backbones, undersea cables

**Multi-Mode Fiber (MMF):**
- Wider core (~50–62.5 micrometers)
- Uses LED as light source
- Shorter distances (up to ~2km)
- Used within buildings and campuses

**Advantages over copper:**
- Completely immune to electromagnetic interference
- Supports enormous bandwidth
- Very low signal loss over distance
- Cannot be easily tapped (more secure)
- Lighter and thinner

---

**Coaxial Cable**
A central conductor surrounded by insulation, a braided metal shield, and an outer jacket. Better noise resistance than twisted pair. Used in cable television (CATV) and old Ethernet (10BASE2). Still used for the "last mile" of cable internet connections.

---

### Wireless Media — Unguided

**Radio Waves**
Travel in all directions from the antenna. Used for: Wi-Fi (2.4 GHz, 5 GHz, 6 GHz), cellular networks (4G/5G), Bluetooth, AM/FM radio, satellite. Different frequencies have fundamentally different behaviors:

```
Frequency vs Behavior:
Low frequency (AM radio, 0.5-1.7 MHz)  → Travels thousands of km, low data rate
Medium (FM radio, 88-108 MHz)          → Travels hundreds of km
High (Wi-Fi 2.4 GHz)                   → Good range, penetrates walls
Very High (Wi-Fi 5 GHz)                → High speed, short range, less wall penetration
Extremely High (mmWave 5G, 24-100 GHz) → Very high speed, very short range, blocked by obstacles
```

**Microwaves**
High-frequency radio (above 1 GHz). Used for point-to-point terrestrial links and satellite communication. Require **line-of-sight** — cannot go around obstacles. Used for TV broadcasting relay towers and long-distance telephone backbones in areas without fiber.

**Infrared**
Very short range, requires direct line-of-sight, cannot penetrate walls. Used for TV remotes, some short-range device communication. Not practical for networks.

---

## Key Physical Layer Concepts

### Bandwidth
The **maximum data transfer capacity** of a link, measured in bits per second (bps). Common units: Kbps, Mbps, Gbps.

Bandwidth is the width of the pipe — how much data CAN flow simultaneously. A 100 Mbps Ethernet link can carry up to 100 megabits per second.

### Throughput
The **actual** amount of data successfully transmitted per unit of time. Always **≤ bandwidth** due to overhead, errors, protocol headers, and congestion. If you have a 100 Mbps link but experience 10% packet loss, your effective throughput might be 60 Mbps.

### Latency
The **time delay** for data to travel from source to destination. Measured in milliseconds (ms). Composed of:

| Component | What It Is | Example |
|-----------|-----------|---------|
| Propagation Delay | Time for signal to physically travel | Light takes ~5ms per 1000km in fiber |
| Transmission Delay | Time to put bits on the wire | 1000 bytes ÷ 100Mbps = 0.08ms |
| Processing Delay | Time at each router/switch | Usually microseconds |
| Queuing Delay | Waiting in router buffers | Varies — can dominate under congestion |

**Bandwidth vs Latency — The Crucial Distinction:**
High bandwidth ≠ Low latency. You can have a 1 Gbps satellite link with 600ms latency (useless for video calls) or a 10 Mbps fiber link with 1ms latency (excellent for video calls). Bandwidth is the pipe width. Latency is the pipe length.

### Attenuation
The reduction in signal strength as it travels through a medium. All signals weaken with distance. This is why Ethernet cables have a 100m maximum — beyond that, the signal is too weak to reliably detect. Repeaters amplify the signal to extend distance.

### Noise
Unwanted signals that interfere with the transmitted signal.
- **Thermal noise:** Random electron movement in copper wires
- **Crosstalk:** Signal from one wire coupling into adjacent wire
- **EMI (Electromagnetic Interference):** From motors, fluorescent lights, other cables

**SNR (Signal-to-Noise Ratio):** The ratio of the desired signal to background noise, in decibels (dB). Higher SNR = cleaner signal = higher possible data rate.

---

---

# 9. Data Link Layer — Frame by Frame

The Data Link layer takes raw bits from the Physical layer and organizes them into **frames** — structured packages with addressing, sequencing, and error-detection information.

## MAC Addresses

Every **NIC (Network Interface Card)** has a globally unique **48-bit** (6-byte) MAC (Media Access Control) address burned in by the manufacturer during production.

**Format:** Written as 6 pairs of hexadecimal digits:
```
A4:C3:F0:85:AC:2D
│─────────│ │────│
   OUI      Device
(Manufacturer)
```

**OUI (Organizationally Unique Identifier):** First 3 bytes (24 bits) — assigned to the manufacturer by IEEE. You can look up any OUI to find who made the device. A4:C3:F0 = Wistron, 00:1A:2B = Cisco, etc.

**Device portion:** Last 3 bytes (24 bits) — assigned by the manufacturer to uniquely identify the specific device.

**Total unique MAC addresses possible:** 2⁴⁸ = ~281 trillion — more than enough for every device ever made.

**Key distinction from IP addresses:**
- MAC = Layer 2, hardware, local network only, permanent
- IP = Layer 3, logical, global internet, can change

**Special MAC addresses:**
- `FF:FF:FF:FF:FF:FF` = Broadcast — all devices on the local network receive this frame

---

## The Ethernet Frame Structure

When the Network layer passes a packet down to the Data Link layer, it gets encapsulated into a frame:

```
┌─────────┬─────┬──────────┬──────────┬──────────┬─────────────────┬─────┐
│Preamble │ SFD │ Dest MAC │ Src MAC  │  Type/   │   Data (Payload)│ FCS │
│ 7 bytes │ 1B  │  6 bytes │  6 bytes │  Length  │   46–1500 bytes │ 4B  │
│         │     │          │          │  2 bytes │                 │     │
└─────────┴─────┴──────────┴──────────┴──────────┴─────────────────┴─────┘
```

**Preamble (7 bytes):** Alternating 1s and 0s (10101010...) — used to synchronize the clocks of sender and receiver before the actual data arrives.

**SFD — Start Frame Delimiter (1 byte):** 10101011 — the final byte of the preamble, marking the exact start of the frame.

**Destination MAC (6 bytes):** The MAC address of the intended recipient. If `FF:FF:FF:FF:FF:FF`, the frame goes to all devices on the network (broadcast).

**Source MAC (6 bytes):** The MAC address of the sender. Switches use this to learn which MAC address is on which port.

**EtherType/Length (2 bytes):** If value > 1500, it identifies the Layer 3 protocol carried:
- `0x0800` = IPv4
- `0x0806` = ARP
- `0x86DD` = IPv6
- `0x8100` = 802.1Q VLAN tagged frame

**Data / Payload (46–1500 bytes):** The IP packet from the Network layer. Minimum 46 bytes — if the actual data is shorter, padding is added. Maximum 1500 bytes = the **MTU (Maximum Transmission Unit)** of Ethernet. If an IP packet is larger than 1500 bytes, it must be fragmented.

**FCS — Frame Check Sequence (4 bytes):** A **CRC (Cyclic Redundancy Check)** value. The sender calculates a mathematical checksum over the entire frame and places it here. The receiver calculates its own checksum and compares. If they match, the frame arrived without errors. If they don't match, the frame is silently discarded (upper layers handle retransmission if needed).

---

## Error Detection — CRC

CRC is the error detection mechanism in Ethernet frames. Here is how it works conceptually:

1. Sender treats the entire frame data as a large binary number
2. Divides it by a predetermined polynomial (divisor)
3. The remainder of this division = the CRC value = placed in FCS field
4. Receiver performs the same division on received data
5. If receiver's remainder = sender's CRC → no error
6. If they differ → error detected → frame discarded

CRC detects all single-bit errors, all burst errors up to the CRC length, and most larger burst errors. It does **NOT** correct errors — just detects them. Error correction is handled by upper layers (TCP requests retransmission).

---

## Medium Access Control — Who Transmits When?

When multiple devices share the same physical medium, they need rules to prevent chaos. Two devices transmitting simultaneously creates a **collision** — both signals merge, garbling both.

### CSMA/CD — For Wired Ethernet

**Carrier Sense Multiple Access / Collision Detection**

```
Device wants to transmit:
  ↓
CARRIER SENSE: Is the medium idle? 
  If busy → wait → try again
  If idle → transmit
  ↓
During transmission: COLLISION DETECTION — am I hearing my own signal cleanly?
  If clean → continue transmitting
  If garbled (collision detected!) → stop immediately
  ↓
Send JAM SIGNAL → tells all devices a collision occurred
  ↓
RANDOM BACKOFF: wait a random amount of time (Binary Exponential Backoff)
  ↓
Try transmitting again
```

**Important note:** CSMA/CD is essentially **obsolete** in modern networks. Modern switches create a separate collision domain for each port and operate in full-duplex mode — there is only one device per collision domain, so collisions are impossible.

### CSMA/CA — For Wireless (Wi-Fi)

**Carrier Sense Multiple Access / Collision Avoidance**

Wireless devices cannot detect collisions (a transmitting device's own signal drowns out incoming signals). So instead of detecting and recovering from collisions, Wi-Fi tries to **avoid them**:

1. Listen to see if medium is busy
2. If busy, wait
3. If idle, wait an additional random backoff period (DIFS + random slot time)
4. If still idle after backoff → transmit
5. Receiver sends an ACK frame confirming receipt
6. If no ACK received → assume collision → retry with larger random backoff

The randomized backoff means devices are unlikely to start transmitting at the exact same moment even if they all detect the medium is free simultaneously.

---

## ARP — Address Resolution Protocol

**The Problem:** The Network layer gives you a destination IP address. To send a frame on the local network, you need the destination's **MAC address**. How do you find it?

**The Solution:** ARP broadcasts a question to everyone on the network: "Who has this IP address? Please tell me your MAC."

```
ARP Process:

Device A (192.168.1.10, AA:AA:AA:AA:AA:AA) wants to send to 192.168.1.5
but doesn't know its MAC address.

Step 1 — ARP Request (broadcast):
┌────────────────────────────────────────────────────────────┐
│ "Who has 192.168.1.5? Tell 192.168.1.10"                  │
│ Source MAC: AA:AA:AA:AA:AA:AA                               │
│ Destination MAC: FF:FF:FF:FF:FF:FF (broadcast — everyone!) │
└────────────────────────────────────────────────────────────┘
                    ↓ sent to all devices on network

Step 2 — ARP Reply (unicast from the device with 192.168.1.5):
┌────────────────────────────────────────────────────────────┐
│ "192.168.1.5 is at BB:BB:BB:BB:BB:BB"                      │
│ Source MAC: BB:BB:BB:BB:BB:BB                               │
│ Destination MAC: AA:AA:AA:AA:AA:AA (directly to requester) │
└────────────────────────────────────────────────────────────┘

Step 3 — Device A:
  Stores (192.168.1.5 → BB:BB:BB:BB:BB:BB) in its ARP cache
  Now sends the frame with destination MAC = BB:BB:BB:BB:BB:BB
```

**ARP Cache:** Each device maintains a local ARP table mapping IP addresses to MAC addresses. Entries expire after a period (typically 20 minutes for dynamic entries) to handle IP address changes.

**Command to view ARP table:**
- Windows: `arp -a`
- Linux: `arp -n` or `ip neigh show`

---

## How a Switch Learns and Forwards

A switch is the most common Layer 2 device. It maintains a **MAC Address Table** (also called a CAM table — Content Addressable Memory table).

```
MAC Address Table:
┌────────┬───────────────────┬──────┐
│  Port  │    MAC Address    │ VLAN │
├────────┼───────────────────┼──────┤
│   1    │ AA:BB:CC:11:22:33 │   1  │
│   2    │ AA:BB:CC:44:55:66 │   1  │
│   3    │ AA:BB:CC:77:88:99 │   1  │
└────────┴───────────────────┴──────┘
```

**Learning:** When a frame arrives on Port 1, the switch records "AA:BB:CC:11:22:33 is on Port 1" in its table. Now it knows where to send future frames destined for this MAC.

**Forwarding Decision:**
```
Frame arrives at switch:
  ↓
Read destination MAC address
  ↓
Look up in MAC table:
  Found → forward ONLY to that port (unicast)
  Not found → flood to ALL ports except incoming (unknown unicast flood)
  FF:FF:FF:FF:FF:FF → flood to ALL ports except incoming (broadcast)
```

**Why switches are better than hubs:**
- Hub = repeater at Layer 1 → copies all bits to all ports → everyone sees all traffic → collisions → insecure
- Switch = intelligent Layer 2 device → sends frames only to the correct port → no collisions → private

---

---

# 10. Network Layer — IP and Routing

## What the Network Layer Does

The Data Link layer delivers frames between adjacent nodes on the same network. The Network layer delivers packets from **any source to any destination anywhere in the world**, potentially crossing hundreds of different networks operated by different organizations.

The two key functions:
1. **Logical Addressing (IP Addresses)** — assigns global addresses that encode location
2. **Routing** — determines the best path from source to destination

## The Router's Job

When a packet arrives at a router, the router:
1. Strips the Layer 2 frame header (it served its purpose — getting the packet to this router)
2. Reads the **destination IP address** from the Layer 3 packet header
3. Looks up the destination in its **routing table**
4. Determines the outgoing interface and next-hop router
5. Creates a **new** Layer 2 frame with new source and destination MAC addresses
6. Forwards the packet

This process repeats at every router along the path. The IP addresses in the packet NEVER change. The MAC addresses change at every hop.

## ICMP — Internet Control Message Protocol

ICMP operates at Layer 3 and is used for:
- **Network diagnostics:** The `ping` command uses ICMP Echo Request (Type 8) and Echo Reply (Type 0)
- **Error reporting:** When a router cannot forward a packet, it sends an ICMP error back to the source
- **Path discovery:** `traceroute` uses ICMP TTL Exceeded messages (Type 11)

ICMP is not used to carry user data — it is purely a control and diagnostics protocol.

## IPv4 Packet Header

The IPv4 header is minimum 20 bytes:

```
 0                   1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
├─┬─────┬──────────────┬───────────────────────────────────────────┤
│ Version │ IHL │ DSCP+ECN │           Total Length                │
├─────────┴──────────────┴───────────────────────────────────────┤
│         Identification          │ Flags │  Fragment Offset       │
├────────────────┬────────────────┴────────────────────────────────┤
│      TTL       │    Protocol    │         Header Checksum        │
├────────────────┴────────────────────────────────────────────────┤
│                       Source IP Address                          │
├──────────────────────────────────────────────────────────────────┤
│                    Destination IP Address                         │
├──────────────────────────────────────────────────────────────────┤
│                    Options (if IHL > 5)                           │
└──────────────────────────────────────────────────────────────────┘
```

**Key fields:**

**Version (4 bits):** IP version. `0100` = IPv4, `0110` = IPv6.

**IHL — Internet Header Length (4 bits):** Length of the header in 32-bit words. Minimum 5 (= 20 bytes). Maximum 15 (= 60 bytes with options).

**Total Length (16 bits):** Size of the entire packet (header + data) in bytes. Maximum 65,535 bytes.

**TTL — Time to Live (8 bits):** Number of router hops a packet can make before being discarded.
- Each router decrements TTL by 1
- When TTL = 0, the router discards the packet and sends an ICMP "Time Exceeded" message back
- **Purpose:** Prevents packets from circulating forever in routing loops
- **Default values:** Windows = 128, Linux/Mac = 64, Cisco routers = 255

**Protocol (8 bits):** Identifies the Layer 4 protocol in the payload:
- `6` = TCP
- `17` = UDP
- `1` = ICMP
- `89` = OSPF

**Source IP (32 bits):** IP address of the original sender. Never changes in transit.

**Destination IP (32 bits):** IP address of the intended recipient. Never changes in transit.

**Fragmentation fields (Identification, Flags, Fragment Offset):** If a packet is larger than the MTU of a link it must traverse, the router (IPv4 only) fragments it. The receiving end reassembles fragments using these fields. IPv6 routers do not fragment — hosts must determine the path MTU and fragment before sending.

---

---

# 11. IP Addressing — IPv4 Deep Dive

## The Basics

An IPv4 address is a **32-bit number** written as four 8-bit groups (octets) in decimal, separated by dots.

```
     192    .    168    .     1     .    100
  11000000  . 10101000  . 00000001  . 01100100
  (8 bits)    (8 bits)    (8 bits)    (8 bits)
  ────────────────────────────────────────────
                    32 bits total
```

Each octet ranges from 0 to 255 (2⁸ = 256 possible values per octet).

Total possible IPv4 addresses: 2³² = **4,294,967,296** (~4.3 billion).

## Network vs Host Portions

An IP address has two parts:
- **Network portion:** Identifies which network the device is on (like a city name)
- **Host portion:** Identifies the specific device on that network (like a house number)

The **subnet mask** defines where the boundary is between network and host portions.

```
IP Address:   192.168.1.100
Subnet Mask:  255.255.255.0
              ─────────────
Binary:
IP:     11000000.10101000.00000001.01100100
Mask:   11111111.11111111.11111111.00000000
        ─────────────────────────────────
        ← Network Portion (24 bits)  → ← Host (8 bits) →
```

The **1 bits** in the mask mark the network portion.
The **0 bits** mark the host portion.

## Classful Addressing

Originally, IP addresses were divided into classes based on the leading bits:

| Class | Leading Bits | First Octet | Default Mask | Network Bits | Host Bits | Max Hosts |
|-------|-------------|-------------|-------------|-------------|----------|----------|
| A | 0 | 1–126 | 255.0.0.0 /8 | 8 | 24 | 16,777,214 |
| B | 10 | 128–191 | 255.255.0.0 /16 | 16 | 16 | 65,534 |
| C | 110 | 192–223 | 255.255.255.0 /24 | 24 | 8 | 254 |
| D | 1110 | 224–239 | — | Multicast | — | — |
| E | 1111 | 240–255 | — | Experimental | — | — |

**Note:** 127.x.x.x is reserved for loopback (localhost). Not assigned to any class for network use.

**The problem with classful addressing:** A company needing 500 hosts would get a Class B address (65,534 hosts), wasting 65,034 addresses. This inefficiency led to IP address exhaustion and the development of CIDR.

## CIDR — Classless Inter-Domain Routing

CIDR (introduced 1993) allows the subnet mask to be **any length** — not just 8, 16, or 24 bits. The mask length is written after a slash: `/n` where n is the number of network bits.

```
192.168.1.0/24  → 24 network bits, 8 host bits = 254 usable hosts
192.168.1.0/25  → 25 network bits, 7 host bits = 126 usable hosts
192.168.1.0/26  → 26 network bits, 6 host bits = 62 usable hosts
10.0.0.0/8      → 8 network bits, 24 host bits = 16,777,214 usable hosts
```

## Private IP Ranges (RFC 1918)

These addresses are reserved for private networks and are **NOT routable on the public internet**:

```
┌─────────────────────────────────────────────────────────────┐
│ Class A: 10.0.0.0 – 10.255.255.255      (10.0.0.0/8)       │
│          16,777,216 addresses                                │
├─────────────────────────────────────────────────────────────┤
│ Class B: 172.16.0.0 – 172.31.255.255   (172.16.0.0/12)     │
│          1,048,576 addresses                                 │
├─────────────────────────────────────────────────────────────┤
│ Class C: 192.168.0.0 – 192.168.255.255 (192.168.0.0/16)    │
│          65,536 addresses                                    │
└─────────────────────────────────────────────────────────────┘
```

**Your home network** is almost certainly `192.168.1.x` or `192.168.0.x`.
**Corporate networks** often use `10.x.x.x` for their large address space.
**NAT** (Network Address Translation) allows devices with private IPs to access the internet through a single public IP.

## Special IP Addresses — Must Know

| Address/Range | Purpose | Notes |
|--------------|---------|-------|
| 127.0.0.1 | Loopback / localhost | Traffic loops back to same device — tests TCP/IP stack |
| 127.0.0.0/8 | Entire loopback range | All 127.x.x.x addresses loop back |
| 0.0.0.0 | "This network" or unspecified | Used in routing as "default route" |
| 255.255.255.255 | Limited broadcast | All devices on local network |
| 169.254.0.0/16 | APIPA (link-local) | Windows auto-assigns when DHCP fails ⚠️ |
| 224.0.0.0/4 | Multicast | Class D — send to multiple specific receivers |

**APIPA (Automatic Private IP Addressing):** If a Windows device cannot find a DHCP server, it automatically assigns itself an address in the 169.254.x.x range. This allows communication with other devices also using APIPA on the same network, but **provides no internet access**. Seeing a 169.254.x.x address is a diagnostic indicator that DHCP is failing.

## NAT — Network Address Translation

Since private IPs cannot be routed on the internet, NAT (typically performed by a home router or corporate firewall) translates private addresses to public ones for outbound traffic, and reverses the translation for responses.

```
HOME NETWORK                     INTERNET
─────────────                    ────────
192.168.1.10 ─┐                  google.com
192.168.1.11 ─┤─► [ROUTER] ──►  203.0.113.1 (public IP)
192.168.1.12 ─┘  NAT Table:      ▲
              192.168.1.10:54321 ↔ 203.0.113.1:54321
              192.168.1.11:45678 ↔ 203.0.113.1:45678
```

**PAT (Port Address Translation)** — the most common form, also called "NAT overload." Uses port numbers to differentiate between multiple private hosts sharing one public IP. This is what your home router does.

---

---

# 12. Subnetting — Complete Guide

## Why Subnet?

Subnetting divides one large network into smaller **sub-networks** (subnets). Reasons:

**Reduce broadcasts:** In a /24 network with 254 hosts, one ARP broadcast reaches 253 other devices. In an office with 1000 devices on one flat network, ARP storms can cause significant congestion. Subnetting into four /26 networks means broadcasts only reach 62 devices.

**Improve security:** Different subnets can have different access policies. Finance in VLAN 10 / 192.168.10.0/24, HR in VLAN 20 / 192.168.20.0/24 — a firewall rule can prevent HR from accessing Finance systems.

**Efficient address use:** Assign only the addresses needed for each segment.

**Organizational clarity:** Network topology maps to business structure.

## The Subnetting Formula — Memorize This

```
Given prefix /n:

Total addresses      = 2^(32 - n)
Usable host addresses = 2^(32 - n) - 2
                        (subtract: network address + broadcast address)

Network address      = IP AND subnet mask (all host bits = 0)
Broadcast address    = Network address with all host bits = 1
First usable host    = Network address + 1
Last usable host     = Broadcast address - 1

Block size           = 256 - (value of subnet mask in interesting octet)
Subnets increment    = by block size
```

## Step-by-Step Method

### Step 1: Identify the "Interesting Octet"
The interesting octet is the one where the subnet boundary falls — where the mask is neither 255 (full) nor 0 (empty).

```
/24 = 255.255.255.0   → Interesting octet = 4th (value = 0, but boundary is here)
/26 = 255.255.255.192 → Interesting octet = 4th (value = 192)
/20 = 255.255.240.0   → Interesting octet = 3rd (value = 240)
```

### Step 2: Calculate Block Size
Block size = 256 – (mask value in interesting octet)
```
/26 → mask = 192 → block size = 256 - 192 = 64
/27 → mask = 224 → block size = 256 - 224 = 32
/28 → mask = 240 → block size = 256 - 240 = 16
/20 → mask = 240 → block size = 256 - 240 = 16 (in the 3rd octet)
```

### Step 3: List Subnets
Subnets start at 0 and increment by the block size:
```
/26 (block size 64): 0, 64, 128, 192
/27 (block size 32): 0, 32, 64, 96, 128, 160, 192, 224
```

### Step 4: Find Network, Broadcast, Hosts for Any IP

Given IP + prefix → find which block it falls in → that block start = network address, block end = broadcast.

---

## Solved Example 1 — Basic

**Problem:** Find network address, broadcast, first host, last host, and number of usable hosts for `172.16.45.200/26`

**Step 1:** Prefix /26 → Mask = 255.255.255.192 → Block size = 256 – 192 = **64**

**Step 2:** List blocks in 4th octet: 0, 64, 128, **192**, 256
- 200 falls in the block starting at **192** (192 to 255)

**Step 3:** Results:
```
Network Address   = 172.16.45.192
Broadcast Address = 172.16.45.255  (192 + 64 - 1 = 255)
First Host        = 172.16.45.193
Last Host         = 172.16.45.254
Usable Hosts      = 2^(32-26) - 2 = 64 - 2 = 62
```

---

## Solved Example 2 — Design Subnets

**Problem:** Divide `192.168.20.0/24` into 8 equal subnets.

**Step 1:** Need 8 subnets → need 2³ = 8 → borrow **3 bits** → New prefix = 24 + 3 = **/27**

**Step 2:** New mask = 255.255.255.224 → Block size = 256 – 224 = **32**

**Step 3:** All 8 subnets:

| Subnet | Network Address | First Host | Last Host | Broadcast | Hosts |
|--------|----------------|-----------|----------|-----------|-------|
| 1 | 192.168.20.0 | .1 | .30 | .31 | 30 |
| 2 | 192.168.20.32 | .33 | .62 | .63 | 30 |
| 3 | 192.168.20.64 | .65 | .94 | .95 | 30 |
| 4 | 192.168.20.96 | .97 | .126 | .127 | 30 |
| 5 | 192.168.20.128 | .129 | .158 | .159 | 30 |
| 6 | 192.168.20.160 | .161 | .190 | .191 | 30 |
| 7 | 192.168.20.192 | .193 | .222 | .223 | 30 |
| 8 | 192.168.20.224 | .225 | .254 | .255 | 30 |

---

## Solved Example 3 — VLSM (Variable Length Subnet Masking)

**Problem:** A company has `10.1.0.0/24`. They need:
- Department A: 100 hosts
- Department B: 50 hosts
- Department C: 25 hosts
- Router link: 2 hosts

**Approach:** Assign largest first. Use the smallest subnet that fits.

```
Dept A: needs 100 hosts → need 128 addresses → /25 (126 usable hosts ✓)
  Subnet: 10.1.0.0/25   → Range: 10.1.0.1 – 10.1.0.126

Dept B: needs 50 hosts → need 64 addresses → /26 (62 usable hosts ✓)
  Subnet: 10.1.0.128/26 → Range: 10.1.0.129 – 10.1.0.190

Dept C: needs 25 hosts → need 32 addresses → /27 (30 usable hosts ✓)
  Subnet: 10.1.0.192/27 → Range: 10.1.0.193 – 10.1.0.222

Router link: needs 2 hosts → /30 (2 usable hosts ✓)
  Subnet: 10.1.0.224/30 → Range: 10.1.0.225 – 10.1.0.226

Remaining: 10.1.0.228 – 10.1.0.255 (available for future use)
```

---

## Quick Reference Table — Common Prefix Lengths

| Prefix | Subnet Mask | Total IPs | Usable Hosts | Block Size |
|--------|------------|-----------|-------------|-----------|
| /24 | 255.255.255.0 | 256 | 254 | 256 |
| /25 | 255.255.255.128 | 128 | 126 | 128 |
| /26 | 255.255.255.192 | 64 | 62 | 64 |
| /27 | 255.255.255.224 | 32 | 30 | 32 |
| /28 | 255.255.255.240 | 16 | 14 | 16 |
| /29 | 255.255.255.248 | 8 | 6 | 8 |
| /30 | 255.255.255.252 | 4 | 2 | 4 |
| /31 | 255.255.255.254 | 2 | 0* | 2 |
| /32 | 255.255.255.255 | 1 | 1** | 1 |

**/31:** No broadcast/network concept — used for point-to-point links (RFC 3021).
**/32:** Single host route — refers to exactly one device.

---

---

# 13. IPv6 — The Future of Addressing

## Why IPv6?

IPv4's 4.3 billion addresses were exhausted. IANA allocated the last blocks in 2011. While NAT extended IPv4's life, it breaks end-to-end connectivity and adds complexity. IPv6 is the permanent solution.

## IPv6 Address Format

IPv6 addresses are **128 bits**, written as **8 groups of 4 hexadecimal digits** separated by colons:

```
Full:     2001:0db8:85a3:0000:0000:8a2e:0370:7334
```

### Simplification Rules

**Rule 1:** Leading zeros within any group can be omitted:
```
0db8 → db8       0000 → 0       0370 → 370
```

**Rule 2:** One consecutive sequence of all-zero groups can be replaced with `::` (only once per address):
```
2001:0db8:0000:0000:0000:0000:0000:0001
→ 2001:db8::1
```

**Examples:**
```
Full:       fe80:0000:0000:0000:0202:b3ff:fe1e:8329
Simplified: fe80::202:b3ff:fe1e:8329

Full:       0000:0000:0000:0000:0000:0000:0000:0001
Simplified: ::1  (loopback)
```

## IPv6 Address Space

Total IPv6 addresses: **2¹²⁸ ≈ 3.4 × 10³⁸**

To put this in perspective: if the entire surface of the Earth were divided into 1 mm² squares, each square could have approximately 655 billion unique IPv6 addresses. We will never run out.

## IPv6 Address Types

| Type | Prefix | Description |
|------|--------|-------------|
| Global Unicast | 2000::/3 | Routable on internet — "public" IPv6 |
| Link-Local | fe80::/10 | Auto-configured, valid only on local link |
| Loopback | ::1/128 | Like IPv4's 127.0.0.1 |
| Unique Local | fc00::/7 | Like IPv4 private addresses |
| Multicast | ff00::/8 | Replaces IPv4 broadcast |
| Anycast | Same as unicast | Delivered to nearest of multiple destinations |

**Link-Local addresses** are automatically configured on every IPv6 interface from the MAC address using the EUI-64 process. They always start with `fe80`. They are used for neighbor discovery and router discovery on the local network segment.

## IPv4 vs IPv6 — Key Differences

| Feature | IPv4 | IPv6 |
|---------|------|------|
| Address Size | 32 bits | 128 bits |
| Notation | Dotted decimal | Colon hexadecimal |
| Total Addresses | ~4.3 billion | ~3.4 × 10³⁸ |
| Header Size | 20 bytes (variable) | 40 bytes (fixed) |
| Header Complexity | 12 fields | 8 fields (simpler) |
| Broadcast | Yes | No — uses multicast |
| Auto-config | DHCP required | SLAAC (self-configuring) |
| Fragmentation | By routers | By source hosts only |
| IPSec | Optional | Built-in support |
| NAT | Required (address scarcity) | Designed to not need NAT |
| Loopback | 127.0.0.1 | ::1 |
| ARP | Uses ARP (broadcast) | Uses NDP (Neighbor Discovery Protocol, multicast) |

---

---

# 14. Transport Layer — TCP and UDP

## The Transport Layer's Role

The Transport layer provides **end-to-end communication services** for applications. It is the layer that determines:
- Is delivery guaranteed or best-effort?
- Are segments delivered in order?
- How do we prevent the sender from overwhelming the receiver?
- How do multiple applications use the network simultaneously?

The answers come from the two transport protocols: **TCP** and **UDP**.

## Port Numbers

Port numbers are 16-bit numbers (0–65535) that identify **which application** on a host should receive a segment.

**Without ports:** Your computer receives a segment. Is it for Chrome? WhatsApp? A background update service? Impossible to tell.

**With ports:** Each segment has a destination port number. Port 443 → deliver to the HTTPS process. Port 22 → deliver to the SSH process.

```
Source Address: 192.168.1.10
Destination Address: 172.217.160.174
Source Port: 54321  ← random ephemeral port assigned by OS to this browser session
Destination Port: 443  ← HTTPS — tell the receiving OS to deliver to its HTTPS server
```

**Port Ranges:**
```
Well-Known Ports:    0 – 1023      System services, requires admin to open
Registered Ports:    1024 – 49151  Application-specific
Dynamic/Ephemeral:   49152 – 65535 Temporarily assigned to client connections
```

---

## TCP — Transmission Control Protocol

TCP provides a **reliable, ordered, connection-oriented byte stream** service.

### TCP's Guarantees

**Connection-oriented:** A TCP connection must be explicitly established (3-way handshake) before data flows, and explicitly closed afterward.

**Reliable delivery:** Every segment sent is acknowledged. If no acknowledgment arrives within a timeout period, the segment is retransmitted.

**Ordered delivery:** Segments are numbered with **Sequence Numbers**. If they arrive out of order (different paths through the internet), the receiver holds them and reorders before delivering to the application.

**No duplicates:** If a duplicate segment arrives (sender retransmitted because it thought the first was lost), the receiver discards it.

**Flow control:** The receiver advertises a **Window Size** — the maximum number of bytes it can buffer. The sender cannot send more than one window's worth of unacknowledged data. This prevents a fast sender from overwhelming a slow receiver.

**Congestion control:** TCP detects network congestion by observing packet loss (retransmissions) or explicit congestion signals. It automatically reduces its sending rate. Key algorithms: Slow Start, Congestion Avoidance, Fast Retransmit, Fast Recovery.

### TCP Three-Way Handshake (Connection Establishment)

```
CLIENT                              SERVER
  │                                    │
  │──── SYN (Seq=1000) ──────────────► │
  │     "I want to connect.             │
  │      My sequence starts at 1000"   │
  │                                    │
  │◄─── SYN-ACK (Seq=5000, Ack=1001) ──│
  │     "OK. I acknowledge 1000+1=1001. │
  │      My sequence starts at 5000"   │
  │                                    │
  │──── ACK (Ack=5001) ──────────────► │
  │     "I acknowledge 5000+1=5001.     │
  │      Connection established!"      │
  │                                    │
  │════════ DATA TRANSFER ═════════════│
```

**Why three steps, not two?**
Both sides need to:
1. Send their Initial Sequence Number (ISN)
2. Have their ISN acknowledged

You cannot combine these four events into fewer than three messages. The SYN-ACK message does two things simultaneously — it acknowledges the client's SYN AND sends the server's own SYN.

### TCP Four-Way Connection Termination

Either side can initiate termination. Each direction is closed independently:

```
CLIENT                              SERVER
  │──── FIN ─────────────────────► │  "I'm done sending data"
  │◄─── ACK ──────────────────────  │  "Acknowledged — noted"
  │                                    │  (Server may still be sending)
  │◄─── FIN ──────────────────────  │  "I'm also done sending"
  │──── ACK ─────────────────────► │  "Acknowledged"
                                        (Connection fully closed)
```

**TIME_WAIT state:** After sending the final ACK, the client waits for a period (typically 2× Maximum Segment Lifetime = 2–4 minutes) before fully closing. This ensures the final ACK was received and no delayed segments from the old connection interfere with a new connection on the same port.

### TCP Header Structure

```
┌────────────────────┬────────────────────┐
│   Source Port      │ Destination Port   │  (16+16 = 32 bits)
├────────────────────┴────────────────────┤
│            Sequence Number              │  (32 bits)
├─────────────────────────────────────────┤
│          Acknowledgment Number          │  (32 bits)
├──────┬──────┬───────────────────────────┤
│ HLEN │ Rsvd │ Control Flags  │ Window   │  (32 bits)
├──────┴──────┴────────────────┴──────────┤
│    Checksum          │  Urgent Pointer  │  (32 bits)
├──────────────────────┴──────────────────┤
│            Options (if any)             │
└─────────────────────────────────────────┘
```

**Control Flags (6 bits):**
- **SYN:** Synchronize sequence numbers (connection setup)
- **ACK:** Acknowledgment number is valid
- **FIN:** Finish — no more data from sender (connection teardown)
- **RST:** Reset — abort the connection (error condition)
- **PSH:** Push — deliver data to application immediately without buffering
- **URG:** Urgent — urgent pointer field is valid

---

## UDP — User Datagram Protocol

UDP provides a **fast, connectionless, unreliable** service. It simply sends datagrams and does not verify receipt.

### UDP Header — 8 bytes only

```
┌────────────────────┬────────────────────┐
│   Source Port      │ Destination Port   │  (16+16 = 32 bits)
├────────────────────┼────────────────────┤
│      Length        │     Checksum       │  (16+16 = 32 bits)
├────────────────────┴────────────────────┤
│                Data                     │
└─────────────────────────────────────────┘
```

The entire UDP header is just 8 bytes. Compare to TCP's minimum 20 bytes — UDP has 60% less overhead.

### Why Use UDP at All?

UDP's apparent unreliability is actually its strength for specific use cases:

**Real-time audio/video (VoIP, video conferencing, live streaming):**
If a voice packet arrives 500ms late, it is useless — the conversation has moved on. A retransmission makes things worse. It is better to play silence or a glitch and move on. UDP's "best effort" behavior is exactly what these applications need.

**DNS queries:**
A DNS query is tiny. If the response doesn't arrive in ~100ms, the application simply retries. The overhead of TCP's handshake would more than double the time for a simple lookup.

**Online gaming:**
A player's position update 50ms ago is irrelevant if a newer update has arrived. Retransmitting old position data would cause the game to stutter. Games use UDP and implement their own lightweight reliability only for critical events (player death, score updates).

**DHCP:**
A client has no IP address yet — it cannot establish a TCP connection. UDP broadcasts work perfectly.

**QUIC (HTTP/3):**
Google invented QUIC — a protocol built on top of UDP that implements its own reliability, multiplexing, and connection management. It gets the benefits of reliability while avoiding TCP's specific limitations (particularly head-of-line blocking).

---

## TCP vs UDP — Complete Comparison

| Feature | TCP | UDP |
|---------|-----|-----|
| Connection | Connection-oriented (handshake required) | Connectionless (just send) |
| Reliability | Guaranteed delivery (ACKs + retransmit) | Best effort (no guarantee) |
| Ordering | Guaranteed order (sequence numbers) | Not guaranteed |
| Speed | Slower (overhead of reliability) | Faster (minimal overhead) |
| Header Size | 20 bytes minimum | 8 bytes (fixed) |
| Flow Control | Yes (window size) | No |
| Congestion Control | Yes (Slow Start, etc.) | No |
| Error Checking | Checksum + ACK-based | Checksum only |
| Use Cases | HTTP, HTTPS, FTP, SSH, Email | DNS, DHCP, VoIP, Streaming, Gaming |

---

---

# 15. Application Layer Protocols

## HTTP — HyperText Transfer Protocol

HTTP is the foundation of the World Wide Web. It is a **request-response protocol** using a client-server model. The browser is the client. The web server is the server.

**Port:** 80 | **Transport:** TCP | **Stateless:** each request is independent

### HTTP Request Structure
```
GET /index.html HTTP/1.1
Host: www.example.com
User-Agent: Mozilla/5.0 (Chrome/120.0)
Accept: text/html,application/xhtml+xml
Accept-Language: en-US,en
Connection: keep-alive
[blank line]
[body — empty for GET, data for POST]
```

### HTTP Response Structure
```
HTTP/1.1 200 OK
Date: Mon, 01 Jan 2026 12:00:00 GMT
Server: Apache/2.4.41
Content-Type: text/html; charset=UTF-8
Content-Length: 1234
[blank line]
[body — the HTML content]
```

### HTTP Methods

| Method | Purpose | Has Body? | Idempotent? |
|--------|---------|----------|------------|
| GET | Retrieve a resource | No | Yes |
| POST | Submit data, create resource | Yes | No |
| PUT | Replace a resource entirely | Yes | Yes |
| PATCH | Partially update a resource | Yes | No |
| DELETE | Remove a resource | No | Yes |
| HEAD | Get headers only (no body) | No | Yes |
| OPTIONS | Get allowed methods for a resource | No | Yes |

**Idempotent:** Making the same request multiple times has the same effect as making it once. GET is idempotent (reading data doesn't change it). POST is not (submitting a form twice creates two records).

### HTTP Status Codes

```
1xx — Informational:
  100 Continue    — Client can continue with its request

2xx — Success:
  200 OK          — Request succeeded
  201 Created     — Resource was created (typically POST)
  204 No Content  — Success but no response body

3xx — Redirection:
  301 Moved Permanently  — Resource moved forever (update your links)
  302 Found              — Temporary redirect
  304 Not Modified       — Cached version is still valid

4xx — Client Errors:
  400 Bad Request        — Malformed request syntax
  401 Unauthorized       — Authentication required
  403 Forbidden          — Authenticated but not allowed
  404 Not Found          — Resource doesn't exist
  405 Method Not Allowed — HTTP method not supported
  429 Too Many Requests  — Rate limited

5xx — Server Errors:
  500 Internal Server Error — Generic server failure
  502 Bad Gateway           — Invalid response from upstream server
  503 Service Unavailable   — Server down or overloaded
  504 Gateway Timeout       — Upstream server timed out
```

### HTTP Versions

**HTTP/1.0:** New TCP connection for every request. Slow.

**HTTP/1.1 (1997):** Persistent connections (keep-alive) — multiple requests over one TCP connection. Still sequential — must wait for response before next request.

**HTTP/2 (2015):** Multiplexing — multiple requests and responses simultaneously over one TCP connection. Binary format (not text). Header compression (HPACK). Server push (server can proactively send resources the client will need). Major performance improvement.

**HTTP/3 (2022):** Runs over **QUIC** instead of TCP. QUIC is built on UDP and implements its own reliability. Eliminates TCP's head-of-line blocking problem (where one lost packet stalls all subsequent packets). Faster connection establishment (0-RTT in some cases). The future of web communication.

---

## HTTPS — HTTP Secure

HTTPS = HTTP + TLS (Transport Layer Security). Everything that travels between your browser and the server is encrypted.

**Port:** 443 | **Transport:** TCP

### What TLS Provides
1. **Confidentiality:** All data is encrypted — even if intercepted, it's unreadable
2. **Integrity:** Data cannot be modified in transit without detection (HMAC)
3. **Authentication:** The server's identity is verified via a **digital certificate** issued by a trusted Certificate Authority (CA)

### TLS Handshake (Simplified)
```
Client ──► "ClientHello: I support TLS 1.3, here are my cipher suites"
Server ──► "ServerHello: I choose AES-256-GCM-SHA384. Here's my certificate."
Client     [Verifies certificate with CA's public key — is this really the real server?]
Client ──► [Generates and sends key material encrypted with server's public key]
Server     [Decrypts key material with private key]
Both sides  derive the same symmetric session key
Client ──► "Finished" [first encrypted message]
Server ──► "Finished" [confirms encryption working]
Data flows  fully encrypted with symmetric key (AES is fast)
```

The certificate contains the server's public key and is signed by a Certificate Authority (like DigiCert, Let's Encrypt). Your browser trusts a built-in list of CAs. If the CA signed the certificate, you can trust the public key belongs to the real server.

---

## FTP — File Transfer Protocol

FTP uses **two separate TCP connections**:
- **Control connection (port 21):** Commands (login, list directory, download command)
- **Data connection (port 20):** Actual file transfer

**Active vs Passive mode:**
- **Active FTP:** Server initiates the data connection back to the client. Problematic with firewalls.
- **Passive FTP:** Client initiates both connections. Works better with firewalls. Most clients use passive.

**Critical security issue:** FTP transmits usernames, passwords, and data in **plaintext**. Anyone on the network can see everything. Never use plain FTP for anything sensitive.

**Secure alternatives:**
- **SFTP (SSH FTP):** FTP over SSH tunnel. Port 22. Fully encrypted. Most common secure alternative.
- **FTPS (FTP over TLS):** Adds TLS encryption to FTP. Port 990 (implicit) or 21 (explicit). Less common than SFTP.

---

## SSH — Secure Shell

SSH provides encrypted remote command-line access to devices and servers.

**Port:** 22 | **Transport:** TCP | **Encryption:** Full session encryption

**What SSH replaced:** Telnet (port 23) — which transmitted everything in plaintext, including passwords. Telnet should never be used in any modern environment.

**SSH Key Authentication (more secure than passwords):**
```
Step 1: Generate key pair
  ssh-keygen → creates private key (keep secret!) + public key (share freely)

Step 2: Copy public key to server
  ssh-copy-id user@server → appends public key to ~/.ssh/authorized_keys on server

Step 3: Connect
  ssh user@server → SSH uses private key to prove identity without sending password
```

**SSH uses:**
- Remote server management
- Secure file transfer (SFTP, SCP)
- SSH tunneling (port forwarding) — tunnel other protocols through SSH
- Git over SSH (GitHub, GitLab)

---

## SMTP, POP3, IMAP — Email Protocols

### The Email Flow
```
Sender's Email Client
    │ SMTP (port 587 — submission)
    ▼
Sender's Mail Server (MTA — Mail Transfer Agent)
    │ SMTP (port 25 — server to server)
    ▼
Recipient's Mail Server
    │
    ▼
Recipient's Email Client
    │ POP3 (port 110) or IMAP (port 143) — retrieval
```

### SMTP — Simple Mail Transfer Protocol
- **Purpose:** Send email (from client to server, and between mail servers)
- **Port 25:** Server-to-server email relay
- **Port 587:** Client to server (with authentication) — what your email app uses to send
- **Port 465:** SMTPS (SMTP over TLS — older)
- **Push protocol:** The server accepts mail pushed to it

### POP3 — Post Office Protocol v3
- **Purpose:** Download email from server to local device
- **Port:** 110 (995 for POP3S — encrypted)
- **Behavior:** Downloads messages and typically **deletes them from the server**
- **Best for:** Single device access — all email lives on your computer
- **Problem:** Email is not accessible from other devices after download

### IMAP — Internet Message Access Protocol
- **Purpose:** Access email on the server, with a synchronized copy on the client
- **Port:** 143 (993 for IMAPS — encrypted)
- **Behavior:** Email stays on the server. Changes sync across all devices.
- **Best for:** Multiple device access — same inbox on phone, tablet, laptop
- **Used by:** Gmail, Outlook, Yahoo Mail — all modern email services

---

## Telnet vs SSH — Security Comparison

| Feature | Telnet | SSH |
|---------|--------|-----|
| Port | 23 | 22 |
| Encryption | ❌ None — all plaintext | ✅ Full encryption |
| Authentication | Password (sent in plaintext) | Password or public key |
| Security | ❌ Completely insecure | ✅ Secure |
| Status in 2026 | Obsolete — never use | Standard for all remote access |

**Real-world analogy:** Using Telnet is like shouting your password in a crowded room. Using SSH is like speaking in a private, soundproof booth. The choice is obvious.

---

## SNMP — Simple Network Management Protocol

SNMP monitors and manages network devices — routers, switches, servers, printers — from a central location.

**Port:** UDP 161 (queries), UDP 162 (traps)

**Components:**
- **NMS (Network Management System):** The monitoring software (Nagios, PRTG, SolarWinds, Zabbix)
- **Agent:** Software running on each managed device that responds to SNMP queries
- **MIB (Management Information Base):** A database of variables the agent can report on (CPU load, interface bandwidth, error counts)

**Operations:**
- **GET:** NMS queries a device for a specific value
- **GETNEXT/GETBULK:** Get multiple values efficiently
- **SET:** NMS changes a configuration value on a device
- **TRAP:** Device proactively sends an alert to NMS (interface went down, CPU spiked, temperature high)

**Versions:**
- SNMPv1/v2c: Community string for authentication (essentially just a password in plaintext) — not secure
- SNMPv3: Adds proper authentication (MD5/SHA) and privacy (DES/AES encryption) — use this

---

---

# 16. DNS — The Internet's Phone Book

## The Problem DNS Solves

Computers route to IP addresses. Humans remember names. Before DNS, every computer on the internet needed to keep a single shared file (`HOSTS.TXT`) listing every hostname and its IP address. As the internet grew from dozens to thousands of machines, maintaining this single file became impossible. DNS was created in 1983 to replace it with a scalable, distributed, automatic system.

## The DNS Hierarchy

DNS is organized as an **inverted tree** — the root at the top, branches below:

```
                         [.]  ← Root (unnamed, often written as ".")
                          │
         ┌────────────────┼─────────────────┐
        .com             .in              .org    ← TLD (Top-Level Domain)
         │                │                │
    ┌────┘             ┌──┘                └──────┐
  google            flipkart             wikipedia
     │                 │
  ┌──┘              ┌──┘
 www             www
```

**Root Level (.):** 13 sets of root servers (a-root through m-root) distributed globally using **anycast routing** — there are actually over 1,300 physical servers, but they share 13 IP addresses. They know the IP addresses of all TLD name servers.

**TLD (Top-Level Domain):** `.com`, `.org`, `.net`, `.in`, `.uk`, `.edu`, `.gov` etc. Each TLD has its own set of servers that know the authoritative servers for all domains within that TLD.

**Second-Level Domain:** `google.com`, `amazon.in`, `bbc.co.uk` — the domains you register with a registrar (GoDaddy, Namecheap, BigRock).

**Subdomain:** `www.google.com`, `mail.google.com`, `drive.google.com` — configured by the domain owner.

## Full DNS Resolution — Step by Step

When you type `www.google.com` in your browser for the first time:

```
Browser on your laptop
        │
        │ Step 1: Check browser DNS cache → Miss
        │
        ↓
Your Operating System
        │ Step 2: Check hosts file (/etc/hosts) → Not found
        │
        ↓
Recursive Resolver (your ISP's or 8.8.8.8 or 1.1.1.1)
        │ Step 3: Check resolver cache → Miss (first time)
        │
        │ Step 4: Query Root Server: "Where is .com?"
        ↓ Root Server: "Ask 192.5.6.30 (Verisign .com TLD server)"
        │
        │ Step 5: Query .com TLD Server: "Where is google.com?"
        ↓ TLD Server: "Ask 216.239.32.10 (Google's auth nameserver)"
        │
        │ Step 6: Query Google's Authoritative Nameserver: "What is www.google.com?"
        ↓ Google NS: "www.google.com is 142.250.195.78, TTL 300 seconds"
        │
        │ Step 7: Resolver caches result for 300 seconds
        │ Step 8: Returns 142.250.195.78 to your browser
        │
        ↓
Browser connects to 142.250.195.78 on port 443 (HTTPS)
```

**Total time:** 50–100ms for uncached. Subsequent lookups from cache: < 1ms.

## DNS Record Types

| Record | Full Name | Purpose | Example |
|--------|-----------|---------|---------|
| **A** | Address | Domain → IPv4 address | google.com → 142.250.195.78 |
| **AAAA** | IPv6 Address | Domain → IPv6 address | google.com → 2404:6800::x |
| **CNAME** | Canonical Name | Alias → another domain | www.example.com → example.com |
| **MX** | Mail Exchange | Email server for domain | gmail.com → smtp.google.com (priority 5) |
| **NS** | Name Server | Which servers are authoritative | google.com → ns1.google.com |
| **PTR** | Pointer | Reverse DNS (IP → domain) | 78.195.250.142.in-addr.arpa → google.com |
| **TXT** | Text | Arbitrary text (SPF, DKIM, verification) | google.com → v=spf1 include:... |
| **SOA** | Start of Authority | Zone parameters (TTL, admin email) | Zone primary server info |
| **SRV** | Service | Service location | _http._tcp.example.com → host + port |

## TTL — Time to Live in DNS

Every DNS record has a **TTL (Time to Live)** value in seconds. This tells resolvers how long they can cache the answer before querying again.

- Short TTL (60–300s): Used when IP might change soon (e.g., during a migration)
- Long TTL (3600–86400s): Used for stable records — reduces DNS query load
- Default is often 3600s (1 hour) to 86400s (24 hours)

**Practical impact:** If you change your DNS records, clients with the old value cached will use it until the TTL expires. Plan TTL carefully before migrations.

## DNS Uses UDP or TCP?

**UDP port 53:** Used for regular queries. Queries and typical responses fit in a single UDP datagram. Fast and efficient.

**TCP port 53:** Used when the response is larger than 512 bytes (UDP limit for DNS), and for **zone transfers** (AXFR/IXFR — copying entire DNS zones between primary and secondary authoritative servers).

---

---

# 17. DHCP — Automatic IP Assignment

## Why DHCP Exists

Without DHCP, every device joining a network would need manual configuration: IP address, subnet mask, default gateway, DNS servers. In a corporation with 10,000 devices — new employees, guests, devices moving between offices — manual configuration would be a full-time job and an endless source of errors (duplicate IPs, wrong gateway).

DHCP automates all of this. A device joins the network and within seconds has a valid IP configuration — no human intervention required.

## The DORA Process — Four-Message Exchange

```
CLIENT                              DHCP SERVER
  │                                      │
  │                                      │
  │──[1] DHCP DISCOVER ────────────────► │
  │   Broadcast (255.255.255.255)         │
  │   Src IP: 0.0.0.0 (has no IP yet)    │
  │   "I'm new here. Anyone have an IP?" │
  │                                      │
  │◄──[2] DHCP OFFER ─────────────────── │
  │   "I offer you 192.168.1.50          │
  │    Mask: 255.255.255.0               │
  │    Gateway: 192.168.1.1              │
  │    DNS: 8.8.8.8, 8.8.4.4            │
  │    Lease: 24 hours"                  │
  │                                      │
  │──[3] DHCP REQUEST ─────────────────► │
  │   Broadcast (other servers may       │
  │   have offered — decline them)       │
  │   "I'd like to accept your offer     │
  │    for 192.168.1.50, Server X"       │
  │                                      │
  │◄──[4] DHCP ACK ────────────────────── │
  │   "Confirmed! 192.168.1.50 is        │
  │    yours for 24 hours. Here's        │
  │    your full configuration."         │
  │                                      │
Client configures its interface:
  IP: 192.168.1.50
  Mask: 255.255.255.0
  Gateway: 192.168.1.1
  DNS: 8.8.8.8
```

**DORA = Discover → Offer → Request → Acknowledge**

Both Discover and Request are **broadcast** because the client has no IP address yet and must reach all potential servers.

## DHCP Components

**IP Address Pool:** The range of IPs the server can assign. Example: 192.168.1.10 – 192.168.1.200. The server tracks which are in use.

**Lease Duration:** How long a client can use an address. At 50% of lease time, the client attempts to renew with the same server. At 87.5% of lease time, it broadcasts for any DHCP server. If lease expires without renewal, the client releases the IP and starts DORA again.

**Exclusions:** Addresses within the pool that should never be assigned. Reserve these for devices with static IPs (printers, servers, network equipment).

**Reservations:** Map a specific MAC address to a specific IP address. The device always gets the same IP via DHCP — behaves like static but without manual device configuration. Used for servers, network printers, and IoT devices.

**Options:** Additional configuration sent to clients:
| Option | Number | Content |
|--------|--------|---------|
| Subnet Mask | 1 | 255.255.255.0 |
| Default Gateway | 3 | 192.168.1.1 |
| DNS Servers | 6 | 8.8.8.8, 8.8.4.4 |
| Domain Name | 15 | company.local |
| NTP Server | 42 | 192.168.1.5 |
| TFTP Server | 66 | 192.168.1.10 |

## DHCP Relay

In large networks, routers separate broadcast domains. A DHCP Discover broadcast cannot cross a router — it stays on the local subnet. But the DHCP server might be on a different subnet.

**DHCP Relay Agent** (also called IP Helper Address): Configured on the router, it intercepts DHCP broadcasts on the local subnet and **unicasts** them to the DHCP server on another network. The server responds to the relay agent, which forwards to the client. Allows one centralized DHCP server to serve multiple subnets.

---

---

# 18. Routing — How Packets Find Their Way

## The Core Problem

When your laptop sends a packet to a server in the US, it travels through your home router, your ISP's routers, multiple backbone routers across the internet, and finally arrives at the destination. Each router along the way makes an independent forwarding decision: "Based on the destination IP, which way should I send this packet?"

Collectively, these decisions route the packet to its destination. Routing is the process of making those decisions optimally.

## The Routing Table

Every router maintains a **routing table** — a database mapping destination networks to outgoing interfaces and next-hop router addresses.

```
Example Routing Table:
┌─────────────────┬─────────────┬───────────┬──────────┬────────┐
│ Destination     │ Gateway     │ Interface │ Protocol │ Metric │
├─────────────────┼─────────────┼───────────┼──────────┼────────┤
│ 192.168.1.0/24  │ directly    │ Fa0/0     │ Connected│ 0      │
│ 192.168.2.0/24  │ directly    │ Fa0/1     │ Connected│ 0      │
│ 10.0.0.0/8      │ 192.168.2.2 │ Fa0/1     │ Static   │ 1      │
│ 172.16.0.0/16   │ 192.168.2.3 │ Fa0/1     │ OSPF     │ 110    │
│ 0.0.0.0/0       │ 203.0.113.1 │ Fa0/2     │ Static   │ 1      │
└─────────────────┴─────────────┴───────────┴──────────┴────────┘
```

**Longest Prefix Match:** When multiple routes match a destination, the router uses the most specific one (longest prefix = most bits match).

Example: Packet for 172.16.5.50
- `172.16.0.0/16` matches — use this route
- `0.0.0.0/0` also matches — but /16 is more specific → use /16

## Route Sources

| Source | Code | Description | Admin Distance |
|--------|------|-------------|---------------|
| Connected | C | Directly attached network | 0 |
| Static | S | Manually configured by admin | 1 |
| EIGRP | D | Cisco's proprietary dynamic routing | 90 |
| OSPF | O | Open standard link-state protocol | 110 |
| RIP | R | Old distance-vector protocol | 120 |
| BGP | B | Internet border routing | 20 (eBGP) / 200 (iBGP) |

**Administrative Distance (AD):** When multiple routing protocols provide routes to the same destination, AD determines which is trusted more. Lower AD = more trusted = wins.

## Static Routing

Routes manually configured by the network administrator.

```
Cisco IOS example:
ip route 192.168.5.0 255.255.255.0 192.168.1.2
          [destination] [mask]      [next-hop]
"To reach 192.168.5.0/24, send packets to 192.168.1.2"

Default route (gateway of last resort — all unknown traffic):
ip route 0.0.0.0 0.0.0.0 203.0.113.1
"For anything I don't have a specific route for, send to 203.0.113.1"
```

**Advantages:** Simple, predictable, zero overhead, secure.
**Disadvantages:** Does not adapt to failures, must be manually updated, doesn't scale.
**Use:** Small networks, stub networks with one exit, specific routes that should never change.

## Dynamic Routing

Routers automatically discover routes using routing protocols. Routers exchange routing information and calculate optimal paths.

**Advantages:** Automatically adapts to failures, scales to large networks.
**Disadvantages:** Overhead (routing protocol traffic), complexity, potential for routing loops during convergence.

### RIP — Routing Information Protocol

- **Type:** Distance-Vector
- **Metric:** Hop count (number of routers)
- **Maximum hop count:** 15 (16 = unreachable — limits network size)
- **Updates:** Broadcasts entire routing table every 30 seconds
- **Convergence:** Slow (15–180 seconds)
- **Versions:** RIPv1 (classful, broadcast), RIPv2 (classless, multicast, supports VLSM)
- **Use today:** Rare. Too limited for modern networks.

### OSPF — Open Shortest Path First

- **Type:** Link-State
- **Metric:** Cost (reference bandwidth / interface bandwidth). Default: 100 Mbps / link speed.
- **Algorithm:** Dijkstra's Shortest Path First (SPF)
- **Updates:** Sends LSAs (Link State Advertisements) when topology changes, not periodically
- **Convergence:** Fast (seconds)
- **Areas:** Organized into areas to reduce LSA flooding. Area 0 = backbone. All other areas connect to Area 0.
- **Features:** Supports VLSM, CIDR, authentication, no hop count limit
- **Use today:** The standard IGP for enterprise networks

**How OSPF works:**
1. Routers discover neighbors by sending Hello packets
2. Neighbors exchange LSAs (information about connected links)
3. Each router builds an identical LSDB (Link State Database) — a complete map of the network
4. Each router runs Dijkstra's SPF algorithm on its LSDB to calculate shortest paths
5. Best paths are installed in the routing table

### BGP — Border Gateway Protocol

- **Type:** Path-Vector
- **Used for:** Routing between Autonomous Systems (ISPs, large companies)
- **Metric:** Policy-based (AS path length, communities, local preference)
- **Convergence:** Deliberately slow — stability > speed for internet routing
- **Scale:** Manages 900,000+ IPv4 routes in the global routing table
- **Sessions:** TCP port 179

**BGP is the routing protocol of the internet.** Every ISP runs BGP to exchange routing information with other ISPs. When you access a website, BGP is responsible for routing your packets between your ISP's network and the website's hosting provider's network.

---

---

# 19. Switching and VLANs

## How Switches Work — Deep Dive

A switch's fundamental behavior:

**1. Learning (Building the MAC table):**
Every time a frame arrives, the switch reads the **source MAC address** and records which port it arrived on. Over time, the switch builds a complete picture of which device is where.

**2. Forwarding:**
When a frame arrives, look up the **destination MAC** in the table:
- **Found:** Forward the frame ONLY out that specific port (unicast forwarding)
- **Not found:** Flood the frame out ALL ports except the incoming port (unknown unicast flood)
- **Broadcast (FF:FF:FF:FF:FF:FF):** Flood out ALL ports except incoming

**3. Filtering:**
If the source and destination MAC are on the same port (same collision domain), the switch discards the frame — no need to forward.

**4. Aging:**
MAC table entries expire after a period (typically 300 seconds / 5 minutes) of inactivity. If a device moves to a different port or is disconnected, its old entry eventually ages out.

## Full Duplex and Collision Domains

**Old hubs:** All devices share one collision domain. Devices must use CSMA/CD. Maximum utilization ~30-40% before performance degrades badly.

**Modern switches:** Each port is a **separate collision domain**. With only one device per collision domain, collisions cannot occur. Combined with **full-duplex** operation (simultaneous send and receive), switches effectively eliminate the need for CSMA/CD entirely.

## VLANs — Virtual Local Area Networks

### The Problem

Without VLANs, all devices on a switch are in the **same broadcast domain**. An ARP broadcast from one device goes to every other device. The Finance department's traffic is visible to the Sales department at Layer 2. Growing the network means growing the broadcast domain, degrading performance.

### The Solution

VLANs create **logical segments** within a physical switch. Devices in different VLANs are isolated — they cannot communicate at Layer 2, as if they were on entirely separate switches.

```
Physical reality:        Logical reality (with VLANs):
One switch               Three virtual switches
All ports connected      VLAN 10: Finance (ports 1-4)
                         VLAN 20: HR (ports 5-8)
                         VLAN 30: IT (ports 9-12)

Finance broadcasts only reach Finance ports.
HR broadcasts only reach HR ports.
Finance CANNOT talk to HR without going through a router.
```

### VLAN Configuration

**Access Port:** A port assigned to a single VLAN. Connected to end devices (PCs, printers). The device connected doesn't know it's in a VLAN — frames arrive and leave without VLAN tags.

**Trunk Port:** A port that carries **multiple VLANs** simultaneously. Connected between switches, or between a switch and a router. Frames are **tagged** with their VLAN ID using 802.1Q.

### 802.1Q VLAN Tagging

When a frame leaves an access port and enters a trunk link, the switch **inserts a 4-byte 802.1Q tag** into the Ethernet frame:

```
Normal Ethernet Frame:
[Preamble][SFD][Dst MAC][Src MAC][EtherType][Data][FCS]

802.1Q Tagged Frame:
[Preamble][SFD][Dst MAC][Src MAC][0x8100][TCI][EtherType][Data][FCS]
                                   ↑       ↑
                              TPID (marks 802.1Q)
                                         │
                                 TCI (Tag Control Info):
                                 - PCP: 3-bit priority (QoS)
                                 - DEI: 1-bit drop eligible
                                 - VID: 12-bit VLAN ID (1-4094)
```

The **Native VLAN** is the VLAN whose frames are sent untagged on trunk links. Default is VLAN 1. A best practice is to change the native VLAN from 1 to an unused VLAN.

### Inter-VLAN Routing

Devices in different VLANs cannot communicate directly — they are in different Layer 2 domains. To communicate, traffic must go through a **Layer 3 device** (router or Layer 3 switch).

**Router-on-a-Stick:** A single router interface carrying all VLANs via subinterfaces, connected to a switch trunk port.

```
                    Router
                   /  Fa0/0
        Subinterfaces:
        Fa0/0.10 → 192.168.10.1 (VLAN 10 gateway)
        Fa0/0.20 → 192.168.20.1 (VLAN 20 gateway)
        Fa0/0.30 → 192.168.30.1 (VLAN 30 gateway)
                    |
                  [Trunk]
                    |
                  Switch
              /    |    \
          VLAN10 VLAN20 VLAN30
```

**Layer 3 Switch (SVIs):** A switch with built-in routing capability. More efficient than router-on-a-stick for large environments.

### STP — Spanning Tree Protocol

**The Problem:** Redundant paths between switches are essential for reliability. But redundant paths create **Layer 2 loops**. A broadcast frame would circulate forever in a loop — each switch forwards it out all ports, the frame arrives at both ports and gets forwarded again — this is a **broadcast storm**. Within seconds, it consumes all available bandwidth and crashes the network.

**The Solution:** STP (IEEE 802.1D) detects loops and **blocks redundant ports**, keeping only a loop-free topology. If the active path fails, STP re-enables a blocked path.

**STP Process:**
1. All switches elect a **Root Bridge** (lowest Bridge ID wins)
2. Each non-root switch finds its **Root Port** (best path to Root Bridge)
3. Each network segment elects a **Designated Port** (best port on that segment toward Root)
4. All other ports are **Blocked** (no data forwarding — only listens for BPDUs)

**RSTP (Rapid Spanning Tree — IEEE 802.1w):** Converges in 1–6 seconds instead of STP's 30–50 seconds. Backward compatible. The modern standard.

---

---

# 20. Wireless Networking — Wi-Fi

## IEEE 802.11 Standards

Wi-Fi is governed by the IEEE 802.11 family of standards. Each generation improves speed, capacity, and efficiency:

| Standard | Wi-Fi Name | Year | Max Speed | Frequency | Key Feature |
|----------|-----------|------|----------|-----------|-------------|
| 802.11b | Wi-Fi 1 | 1999 | 11 Mbps | 2.4 GHz | First consumer Wi-Fi |
| 802.11a | Wi-Fi 2 | 1999 | 54 Mbps | 5 GHz | 5 GHz, less interference |
| 802.11g | Wi-Fi 3 | 2003 | 54 Mbps | 2.4 GHz | 54 Mbps on popular 2.4 GHz |
| 802.11n | Wi-Fi 4 | 2009 | 600 Mbps | 2.4/5 GHz | MIMO antennas |
| 802.11ac | Wi-Fi 5 | 2013 | 3.5 Gbps | 5 GHz | MU-MIMO, wide channels |
| 802.11ax | Wi-Fi 6 | 2019 | 9.6 Gbps | 2.4/5 GHz | OFDMA, high density |
| 802.11ax | Wi-Fi 6E | 2021 | 9.6 Gbps | 2.4/5/6 GHz | Opens 6 GHz band |
| 802.11be | Wi-Fi 7 | 2024 | 46 Gbps | 2.4/5/6 GHz | Multi-Link Operation |

## 2.4 GHz vs 5 GHz vs 6 GHz

| Feature | 2.4 GHz | 5 GHz | 6 GHz |
|---------|---------|-------|-------|
| Range | Longer | Shorter | Shortest |
| Wall Penetration | Better | Less | Least |
| Interference | High (crowded) | Less | Very low (new) |
| Non-overlapping channels | 3 (1, 6, 11) | 24 | Many |
| Max speed | Lower | Higher | Highest |
| Best for | Range, IoT devices | Streaming, gaming | Wi-Fi 6E/7 devices |

## Wireless Security Evolution

**WEP (Wired Equivalent Privacy) — 1999:**
The original Wi-Fi security. Uses RC4 cipher with static keys. Completely broken by 2001 — can be cracked in minutes with widely available tools. **Never use.** The name "Wired Equivalent Privacy" is deeply ironic — it provides far less security than a wired network.

**WPA (Wi-Fi Protected Access) — 2003:**
Created as an emergency fix while WPA2 was being developed. Uses TKIP (Temporal Key Integrity Protocol) — dynamic keys per packet. Better than WEP but still vulnerable. **Do not use.**

**WPA2 — 2004:**
The standard for most of the 2010s. Uses AES (Advanced Encryption Standard) — genuinely strong encryption. Two modes:
- **WPA2-Personal (WPA2-PSK):** Pre-shared key — one password for everyone (home/small office)
- **WPA2-Enterprise:** 802.1X authentication — each user has their own credentials (corporate environments)

**WPA3 — 2018:**
Current standard. Major improvements:
- **SAE (Simultaneous Authentication of Equals):** Replaces PSK — resistant to offline dictionary attacks (even if someone captures the 4-way handshake, they cannot brute-force the password offline)
- **Forward Secrecy:** Each session uses unique keys — compromising one session does not expose past sessions
- **OWE (Opportunistic Wireless Encryption):** Encrypts traffic even on "open" networks (coffee shop Wi-Fi) without a password
- **Required for Wi-Fi 6 certification**

## SSID, BSS, ESS

**SSID (Service Set Identifier):** The name of a Wi-Fi network. When you see "HomeNetwork" or "CafeWiFi" in your device's Wi-Fi list — those are SSIDs. An SSID can be broadcast (visible to all) or hidden (not broadcast, devices must know it to connect — provides minimal security benefit).

**BSS (Basic Service Set):** A single access point and all the client devices associated with it.

**ESS (Extended Service Set):** Multiple access points sharing the same SSID, allowing seamless client **roaming** across a large area — a university campus, an airport, a large office. When a client moves out of range of one AP and into range of another AP with the same SSID, it roams (re-associates) to the new AP without dropping the connection.

**Channel Planning:** In an ESS, adjacent access points should use non-overlapping channels to prevent interference. For 2.4 GHz: use channels 1, 6, and 11. For 5 GHz: many more channels available.

---

---

# 21. Network Security

## The Threat Landscape

Every connected network is potentially accessible to adversaries globally. Understanding attacks is the first step to defending against them.

## Common Network Attacks

### DoS and DDoS

**DoS (Denial of Service):** A single attacker sends enormous volumes of traffic or malformed packets to a target, exhausting its resources (CPU, bandwidth, memory) so it cannot serve legitimate users.

**DDoS (Distributed Denial of Service):** Thousands or millions of compromised machines (a **botnet**) simultaneously attack a target. The distributed nature makes it impossible to simply block one source IP.

**Types:**
- **Volumetric:** Flood the target with traffic (UDP flood, ICMP flood)
- **Protocol:** Exploit protocol weaknesses (SYN flood — creates half-open TCP connections, exhausting server memory)
- **Application:** Target web application vulnerabilities (HTTP flood with complex queries)

**Defenses:** Rate limiting, traffic scrubbing services (Cloudflare, AWS Shield), CDNs, anycast routing to distribute attack traffic, ISP-level filtering.

---

### Man-in-the-Middle (MitM)

An attacker positions themselves **between two communicating parties**, intercepting and potentially altering the communication without either party being aware.

```
Normal:   Client ─────────────────────────► Server
MitM:     Client ──► [Attacker] ──► Server
          Everything passes through attacker
```

**Enablers:**
- **ARP Spoofing:** Attacker sends fake ARP replies associating their MAC with the gateway's IP — all traffic goes through attacker
- **DNS Spoofing:** Corrupt DNS cache to point domain to attacker's IP
- **Rogue Wi-Fi AP:** Set up a fake "Free_WiFi" access point — all traffic passes through attacker's device
- **SSL Stripping:** Downgrade HTTPS to HTTP where possible

**Defenses:** HTTPS everywhere (TLS), HSTS (HTTP Strict Transport Security — browser remembers to always use HTTPS), VPN, certificate pinning, DNSSEC.

---

### ARP Spoofing / ARP Poisoning

```
Normal ARP:
  192.168.1.1 (gateway) → MAC: AA:AA:AA:AA:AA:AA

ARP Spoofing Attack:
  Attacker sends: "192.168.1.1 is at BB:BB:BB:BB:BB:BB" (fake, unsolicited)
  All devices update ARP cache with wrong mapping
  All traffic meant for gateway → actually goes to attacker
```

ARP has no authentication. Any device can send an ARP reply claiming any IP → MAC mapping.

**Defenses:**
- **Dynamic ARP Inspection (DAI):** Switch feature that validates ARP packets against a DHCP snooping binding table. Only allows ARP packets that match known IP-MAC-port bindings.
- Static ARP entries for critical devices
- VPN/TLS encryption (even if intercepted, attacker cannot read or modify encrypted content)

---

### DNS Spoofing / Cache Poisoning

Attacker injects false DNS records into a resolver's cache.

```
Normal: user → resolver → "google.com = 142.250.195.78" → goes to Google
Attack: resolver cache poisoned → "google.com = attacker's IP" → goes to phishing site
```

**Defenses:**
- **DNSSEC:** Cryptographically signs DNS records — resolvers can verify the signature
- **DoH (DNS over HTTPS):** Encrypts DNS queries over HTTPS (port 443) — prevents interception and spoofing
- **DoT (DNS over TLS):** Encrypts DNS queries over TLS (port 853)
- Use reputable resolvers (1.1.1.1, 8.8.8.8) rather than ISP defaults

---

### Port Scanning

Using tools like **Nmap** to probe a target system for open ports and identify running services.

```
nmap -sV 192.168.1.1
PORT     STATE SERVICE   VERSION
22/tcp   open  ssh       OpenSSH 8.4
80/tcp   open  http      Apache 2.4.51
443/tcp  open  https     Apache 2.4.51
3306/tcp open  mysql     MySQL 8.0.27
```

Not an attack itself — reconnaissance. But reveals what services are running, enabling targeted exploitation.

**Defenses:** Firewall rules (only open necessary ports), IDS/IPS (detect scanning patterns), network segmentation (attackers cannot scan internal networks from the outside).

---

### Packet Sniffing

Capturing and reading network traffic using tools like Wireshark.

On a **shared medium** (Wi-Fi), all traffic in the vicinity is transmitted in the air — any device can capture frames meant for others.

In a **switched network**, only traffic addressed to you, broadcast traffic, and traffic on a mirrored port is visible to your NIC. However, a compromised switch, ARP spoofing, or a rogue access point can expose traffic.

**Defenses:** Encryption (HTTPS, SSH, VPN) — if all traffic is encrypted, sniffing reveals nothing useful. TLS prevents sniffed traffic from being readable even if captured.

---

## Security Mechanisms

### Firewalls

A firewall inspects network traffic and allows or blocks it based on configured rules.

**Packet Filter (Stateless):**
- Examines each packet independently
- Rules based on source/destination IP, port, protocol
- Fast but no context — cannot distinguish between a legitimate response and an attack packet

**Stateful Firewall:**
- Tracks connection state
- Maintains a state table of established connections
- Can distinguish between legitimate responses (to connections you initiated) and unsolicited packets
- Much more effective than stateless

**Application Layer Firewall / NGFW (Next-Generation Firewall):**
- Deep packet inspection — reads actual application content
- Application awareness — can block specific apps (block BitTorrent but allow HTTP)
- Integrated IPS
- User identity awareness
- SSL inspection (decrypts TLS to inspect content)

### IDS and IPS

| Feature | IDS (Intrusion Detection System) | IPS (Intrusion Prevention System) |
|---------|----------------------------------|-----------------------------------|
| Action | Detect and alert | Detect and block automatically |
| Placement | Out-of-band (monitors copy of traffic) | Inline (sits in traffic path) |
| Performance impact | Minimal | Some latency |
| Risk | False negatives (missed attacks) | False positives (blocking legit traffic) |

### VPN — Virtual Private Network

Creates an **encrypted tunnel** over the public internet, making remote users appear to be on the internal network.

```
Remote Employee                    Corporate Office
192.168.50.10 ──[Encrypted Tunnel]──► 10.0.0.0/8
              ← VPN Server authenticates and assigns internal IP
              ← All traffic encrypted between user and VPN server
              ← Can access internal resources as if physically present
```

**VPN Protocols:**
| Protocol | Security | Speed | Use |
|----------|---------|-------|-----|
| IPsec | Strong | Fast | Site-to-site VPN, always-on |
| OpenVPN | Strong | Good | Cross-platform client VPN |
| WireGuard | Modern/Strong | Very fast | Modern client VPN |
| SSL/TLS VPN | Strong | Good | Clientless web VPN |

---

---

# 22. Network Devices — Complete Reference

| Device | OSI Layer | What It Does | How It Decides | Key Fact |
|--------|-----------|-------------|----------------|---------|
| **Hub** | Layer 1 | Repeats bits to all ports | Nothing — broadcasts everything | Obsolete. Creates one collision domain. Everyone sees all traffic. |
| **Switch** | Layer 2 | Forwards frames to correct port | MAC address table | Creates separate collision domains. Modern switches = full duplex = no collisions. |
| **Router** | Layer 3 | Routes packets between networks | IP routing table + routing protocol | Connects different IP networks. Creates separate broadcast domains. |
| **Layer 3 Switch** | L2 + L3 | Switches within VLANs, routes between VLANs | MAC table + routing table | High-speed inter-VLAN routing without separate router |
| **Access Point (AP)** | Layer 2 | Provides wireless access | 802.11 association | Bridges wireless clients to wired network |
| **Wireless Controller** | L2–L7 | Manages many APs centrally | Policy/configuration | Enterprise Wi-Fi management |
| **Firewall** | L3–L7 | Allows/blocks traffic by rule | ACL rules, state table | Security enforcement point |
| **IDS/IPS** | L3–L7 | Detects/prevents intrusions | Signature matching, anomaly | IDS alerts, IPS blocks |
| **Load Balancer** | L4 or L7 | Distributes traffic across servers | Round-robin, least-conn, hash | High availability and horizontal scaling |
| **Proxy Server** | Layer 7 | Intermediary for requests | Forward/reverse proxy rules | Caching, filtering, anonymity, SSL termination |
| **Modem** | Layer 1 | Connects to ISP | Modulates/demodulates signal | DSL, cable, fiber protocol conversion |
| **Repeater** | Layer 1 | Regenerates signal | Nothing | Extends cable distance |
| **Bridge** | Layer 2 | Connects two network segments | MAC address | Like a 2-port switch. Legacy device. |
| **NIC** | L1–L2 | Network interface in a device | — | Has MAC address. Hardware connecting device to network. |

---

---

# 23. Real-World Scenarios

## Scenario 1: Complete Journey of a Web Request

**"What happens when you type https://www.flipkart.com in your browser?"**

```
STEP 1 — DNS RESOLUTION
─────────────────────────────────────────────────────────────────
Browser: Check local DNS cache → miss
OS: Check hosts file → not found
OS: Query recursive resolver (e.g., 8.8.8.8)
Resolver: Root → .com TLD → Flipkart's NS → Answer: 23.x.x.x
Browser: Has IP for flipkart.com

STEP 2 — ARP FOR DEFAULT GATEWAY
─────────────────────────────────────────────────────────────────
Your laptop needs to send a packet to the internet.
First step: Find MAC address of default gateway (home router)
ARP: "Who has 192.168.1.1?" → Router replies: "AA:BB:CC:DD:EE:FF"
ARP cache updated.

STEP 3 — TCP THREE-WAY HANDSHAKE
─────────────────────────────────────────────────────────────────
Laptop → Router → ISP → Internet → Flipkart's servers
SYN → SYN-ACK → ACK (to port 443)
TCP connection established.

STEP 4 — TLS HANDSHAKE
─────────────────────────────────────────────────────────────────
ClientHello → ServerHello + Certificate
Browser verifies Flipkart's certificate with CA
Key exchange → Both derive symmetric session key
Encrypted channel established.

STEP 5 — HTTP REQUEST
─────────────────────────────────────────────────────────────────
Browser sends: GET / HTTP/2 (encrypted via TLS)
This traverses: Your LAN → Your router (NAT: private→public) →
ISP → Multiple backbone routers (BGP routing) → Flipkart CDN/servers

STEP 6 — ROUTING HOP BY HOP
─────────────────────────────────────────────────────────────────
Each router: Read dest IP → lookup routing table → forward to next hop
Layer 2 MAC addresses change at every hop
Layer 3 IP addresses stay the same throughout

STEP 7 — RESPONSE
─────────────────────────────────────────────────────────────────
Flipkart servers: 200 OK with HTML + CSS + JS (encrypted)
Response routes back (TCP ensures all segments arrive)
Browser decrypts + renders the page

STEP 8 — CONNECTION CLOSE
─────────────────────────────────────────────────────────────────
FIN → ACK → FIN → ACK
```

Total time for a typical page: **0.5 – 3 seconds**

---

## Scenario 2: Home Network Architecture

```
Internet (Public IP: 103.x.x.x)
           │
       [FTTH ONT] ← Fiber optic from ISP
           │ Ethernet
       [Wi-Fi Router]
       ┌───┴───────────────────────────────────┐
       │  Functions:                            │
       │  - Router (routes to internet)         │
       │  - Switch (connects wired devices)     │
       │  - Access Point (Wi-Fi)                │
       │  - DHCP server (assigns 192.168.1.x)   │
       │  - NAT (maps private → public IP)      │
       │  - Basic firewall (blocks unsolicited) │
       └───────────────────────────────────────┘
              │           │          │
         Wired PC    Laptop (Wi-Fi) Phone (Wi-Fi)
       192.168.1.10  192.168.1.11  192.168.1.12
```

**What happens when your phone accesses a website:**
1. Phone sends packet: Src 192.168.1.12, Dst 142.250.x.x
2. Router NAT: Translates Src to 103.x.x.x:54321, records in NAT table
3. Packet routes across internet to Google
4. Google responds to 103.x.x.x:54321
5. Router NAT table: 103.x.x.x:54321 → 192.168.1.12:54321
6. Packet delivered to your phone

---

## Scenario 3: Enterprise Network — Three-Tier Architecture

Large enterprise networks use a **three-tier hierarchical design**:

```
                    ┌─────────────────────────────────────┐
                    │     CORE LAYER (Layer 3 Switches)    │
                    │  High-speed backbone: 40Gbps links   │
                    │  Routing between distribution blocks │
                    │  Redundant, no user devices here     │
                    └──────────────┬──────────────────────┘
                                   │ Multiple redundant links
               ┌───────────────────┴───────────────────┐
               │          DISTRIBUTION LAYER             │
               │  Layer 3 Switches per building/floor    │
               │  Inter-VLAN routing                     │
               │  Security policies (ACLs)               │
               │  Redundant uplinks to core              │
               └───────────────┬───────────────────────┘
                                │ Multiple links
               ┌────────────────┴──────────────────────┐
               │          ACCESS LAYER                   │
               │  Layer 2 Switches per floor/department  │
               │  VLANs assigned per department          │
               │  PoE for phones and APs                 │
               │  End devices connect here               │
               └───────────────────────────────────────┘
```

This design provides **redundancy** (multiple paths), **security** (policies at distribution), and **scalability** (add access switches without redesigning core).

---

---

# 24. Key Facts and Statistics

The global cloud computing market relies on approximately **400 undersea cables** spanning over 1.3 million km — they carry about **95% of all international internet traffic**. Satellites (including Starlink) carry less than 5%.

Light travels through fiber optic cables at approximately **200,000 km/s** — about 2/3 the speed of light in vacuum. The theoretical minimum latency from Mumbai to London (approximately 7,200 km) is about 36ms just for propagation — practical latency is 100–150ms.

There are approximately **5.4 billion internet users** worldwide as of 2024 — about 67% of the global population.

The internet carries approximately **400 exabytes (400 billion GB) of data per month**.

**IPv4 addresses** were fully exhausted: IANA allocated the last blocks in 2011. APNIC (Asia-Pacific) exhausted its free pool in 2011, RIPE (Europe) in 2012, ARIN (North America) in 2015.

**BGP**, the internet's routing protocol, maintains a global routing table of over **900,000 IPv4 routes** and growing.

A single **Ethernet frame** can carry a maximum of **1,500 bytes** of data (the MTU). For a 100MB file, that requires approximately **66,667 frames** at the network layer.

The **TCP three-way handshake** adds at minimum **1.5 round trips** of latency before any data can flow. For a server 100ms away, this is 150ms of setup time before the first byte of content.

**Wi-Fi 6** (802.11ax) can theoretically deliver **9.6 Gbps** — fast enough to download a full 1080p HD movie in approximately 5 seconds.

The **Domain Name System (DNS)** handles over **3.5 trillion DNS queries per day** globally.

---

---

# 25. Learning Roadmap

## Phase 0 — Prerequisites (Week 1)

Before studying networking formally, ensure comfort with:

**Binary and Hexadecimal Arithmetic:**
Networking requires binary operations for IP addressing and subnetting.
Practice: Convert decimal ↔ binary ↔ hex until fluent.
```
Decimal 192 = Binary 11000000 = Hex C0
Decimal 168 = Binary 10101000 = Hex A8
Binary AND: 11000000 AND 11111111 = 11000000 (used in subnet calculations)
```

**Basic Command Line:**
Windows CMD or Linux terminal. File navigation, running commands, reading output. This matters because networking is diagnosed and configured from the command line.

**Conceptual Understanding:**
What is the internet? What is Wi-Fi? What does "connecting to a network" mean? You likely already know this from daily usage — now you will learn the engineering underneath.

---

## Phase 1 — Conceptual Foundation (Weeks 2–3)

**Master the OSI Model** until you can describe each layer without notes:
- What is its responsibility?
- What protocols operate there?
- What is the data unit?
- What devices operate there?
- What does "encapsulation" add at this layer?

**Study TCP/IP** and map it to OSI.

**Study network types** (LAN, WAN, MAN) and **topologies** (Star, Bus, Ring, Mesh).

**Milestone:** Draw the OSI model from memory with all layers, protocols, data units, and devices. Explain encapsulation end-to-end.

---

## Phase 2 — IP Addressing and Subnetting (Weeks 4–5)

IP addressing is the skill that separates people who understand networking from those who have just read about it.

Spend significant time here. Practice every day.

1. Master binary conversion — decimal ↔ binary without a calculator
2. Understand classful addressing and its limitations
3. Master CIDR notation
4. Learn private address ranges and special addresses by heart
5. Understand the subnet formula and practice until subnetting is intuitive
6. Practice VLSM (variable length subnet masking)

**Milestone:** Given any IP and prefix length, state network address, broadcast, first host, last host, and usable host count in under 60 seconds without a calculator.

---

## Phase 3 — Protocols Deep Dive (Weeks 6–8)

Study each protocol in this order:
1. TCP and UDP — understand every detail. Draw the handshake from memory.
2. DNS — trace a complete resolution
3. DHCP — walk through DORA
4. HTTP and HTTPS — methods, status codes, TLS
5. ARP — how it works and how it can be abused
6. Email protocols (SMTP, POP3, IMAP)
7. SSH vs Telnet — never use Telnet

**Milestone:** For any protocol, state its port number, transport (TCP/UDP), purpose, and key characteristics from memory.

---

## Phase 4 — Hands-On Practice (Weeks 9–12)

**This phase makes everything real.** Use the `03_CN_Practice_Repository.md` file for structured labs.

Install and use:
- **Cisco Packet Tracer** — build virtual networks
- **Wireshark** — capture and analyze real traffic
- **Command line tools** — ping, tracert, nslookup, arp, netstat on your own machine

Practice subnetting problems daily — target 50 problems from the Practice Repository.

**Milestone:** You have built a working VLAN network with inter-VLAN routing in Packet Tracer, AND you have captured and read a TCP handshake in Wireshark from your own computer.

---

## Phase 5 — Advanced Topics (Weeks 13–16)

1. **Routing:** Static routes, OSPF (areas, LSA, SPF algorithm), BGP concepts
2. **VLANs and trunking:** Configure trunk ports, 802.1Q tagging, STP
3. **Network security:** Attacks, firewalls, IDS/IPS, VPN, TLS
4. **Wireless:** 802.11 standards, WPA3, roaming, channel planning
5. **IPv6:** Addressing, NDP, migration strategies

**Milestone:** You can design a complete small-to-medium business network on paper — IP addressing scheme, VLSM subnetting, VLAN design, routing strategy, and security zones.

---

---

# 26. Common Mistakes to Avoid

**Mistake 1: Memorizing the OSI Model Without Understanding It**
Many students memorize "Layer 4 is Transport" without understanding WHY Transport exists or WHAT PROBLEM it solves. The OSI model is not a list to memorize — it is a framework for understanding. Ask "why" at every layer.

**Mistake 2: Skipping Binary Math**
Students try to memorize subnet masks instead of calculating them. This works for /24 and /26 but fails for /19 or /22. Understanding binary makes all subnet calculations logical. Spend the time.

**Mistake 3: Not Practicing Subnetting Enough**
Reading subnetting is not the same as doing subnetting. You need to practice 50–100 problems until it becomes reflexive. There is no shortcut.

**Mistake 4: Confusing MAC and IP Addresses**
These are fundamentally different. MAC = Layer 2, hardware, local, 48-bit hex, permanent. IP = Layer 3, logical, global, 32-bit decimal, changeable. Confusing them indicates a gap in understanding the layer model.

**Mistake 5: Not Using Wireshark or Packet Tracer**
A student who has seen a TCP handshake in Wireshark will never forget it. One who has only read about it might forget the details within a week. Hands-on tools make abstract concepts permanent.

**Mistake 6: Treating OSI and TCP/IP as Separate Topics**
They describe the same reality from different perspectives. Map every protocol to both models. Know that when an interview question asks about OSI layers, they want the 7-layer answer, not the 4-layer answer.

**Mistake 7: Not Understanding "Why" Behind Design Decisions**
Why does TCP have a three-way handshake and not two? Why does DNS use UDP instead of TCP for queries? Why does the Ethernet frame have a minimum size of 64 bytes? Understanding the reasoning makes the knowledge permanent and applicable to new situations.

**Mistake 8: Learning Only Theory Without Commands**
Knowing that `ping` uses ICMP is theory. Actually running `ping -t 8.8.8.8` and reading the output is practical. Both are necessary. Practice every command in the cheat sheet on your own machine.

---

---

# 27. What to Do While and After Learning

## While Learning

**Build alongside reading:** Do not read an entire chapter, then practice. Read one concept, immediately apply it. Learn about DHCP today, run `ipconfig /release` and `ipconfig /renew` today and capture the DORA packets in Wireshark today.

**Maintain a concepts notebook:** For each major concept, write: What is it? What problem does it solve? How does it work? What are the failure modes? This forces you to articulate understanding, not just recognition.

**Practice subnetting every single day:** 5 problems per day for 30 days = 150 problems = subnetting fluency. Make it a daily habit.

**Follow curiosity:** When you use the internet, ask: what is actually happening right now? When you connect to Wi-Fi — DHCP. When you open YouTube — DNS, TCP, QUIC, CDN. When you make a video call — UDP, RTP, codec. Every daily action is a networking scenario.

**Teach concepts to someone else:** Explaining networking to a non-technical person (family member, friend) forces you to truly understand it. If you cannot explain it simply, you do not understand it deeply.

## After Learning

**Pursue certification:**
- **CompTIA Network+** — vendor-neutral, good foundation certificate
- **Cisco CCNA** — industry gold standard for entry-level networking. Rigorous, respected, career-transforming.

**Build a home lab:**
- A managed switch (TP-Link, Cisco SG series) — practice VLANs and trunking on real hardware
- An old laptop or mini PC as a router (pfSense or Cisco IOS on GNS3)
- Even Cisco Packet Tracer with a realistic topology serves the purpose

**Learn adjacent skills:**
- **Linux networking:** `ip`, `ss`, `iptables`, `tcpdump` — essential for network engineers
- **Python for networking:** Netmiko, NAPALM, Scapy — automate network tasks
- **Cloud networking:** AWS VPC, Azure VNet, security groups — networking's future (covered in Cloud Computing repository)

**Contribute and connect:**
- Write about what you've learned — blog posts, GitHub documentation
- Join networking communities on Reddit (r/networking, r/ccna), LinkedIn
- Study real incident reports (Cloudflare, AWS, Fastly outage post-mortems — all networking)

---

---

# 28. Career Paths and Certifications

## Career Paths

**Network Administrator / Engineer**
Design, implement, and maintain an organization's network infrastructure. Configure routers, switches, firewalls, and wireless. Monitor performance. Troubleshoot outages.
Entry salary: ₹3–6 LPA | Experienced: ₹8–20 LPA

**Network Security Engineer**
Focus on protecting network infrastructure. Firewall management, IDS/IPS, VPN administration, security auditing, incident response.
Entry salary: ₹4–8 LPA | Experienced: ₹15–40 LPA

**Cloud Network Engineer**
Design and manage networking in cloud environments — AWS VPC, Azure Virtual Networks, Google Cloud VPC. One of the fastest-growing roles.
Entry salary: ₹5–10 LPA | Experienced: ₹15–50 LPA

**NOC Engineer (Network Operations Center)**
Monitor network health 24/7. Respond to alerts. Escalate incidents. Excellent entry-level role for building practical experience.
Entry salary: ₹2.5–5 LPA

**Site Reliability Engineer (SRE)**
Combines software engineering with networking/systems. Ensures large-scale internet services remain reliable. One of the highest-paid tech roles.
Entry salary: ₹8–15 LPA | Experienced: ₹30–80+ LPA

**ISP / Telecom Network Engineer**
Works for internet service providers. BGP routing, MPLS networks, peering agreements, large-scale infrastructure.
Entry salary: ₹3–6 LPA | Experienced: ₹10–25 LPA

## Certifications

| Certification | Level | Vendor | Focus | Value |
|--------------|-------|--------|-------|-------|
| CompTIA Network+ | Foundation | Vendor-neutral | General networking | Good starting point |
| Cisco CCNA | Associate | Cisco | Routing, switching, wireless, security | ⭐ Highly recommended |
| Cisco CCNP | Professional | Cisco | Advanced enterprise networking | Strong mid-career |
| Cisco CCIE | Expert | Cisco | Most prestigious networking cert | Career-defining |
| Juniper JNCIA | Associate | Juniper | Juniper networking | ISP environments |
| AWS Solutions Architect | Associate | AWS | Cloud networking + services | Essential for cloud path |
| CompTIA Security+ | Foundation | Vendor-neutral | Security fundamentals | Good for security path |
| Certified Ethical Hacker (CEH) | Intermediate | EC-Council | Offensive security | Penetration testing path |

**The recommended path for most beginners:**
CompTIA Network+ (3 months) → Cisco CCNA (6 months) → Specialization based on career direction

---

---

# 29. Glossary

**ACL (Access Control List):** Ordered list of permit/deny rules applied to network traffic, filtering based on source/destination IP, port, and protocol.

**ARP (Address Resolution Protocol):** Layer 3 protocol that resolves IPv4 addresses to MAC addresses via broadcast on local networks.

**AS (Autonomous System):** A network under single administrative control, identified by an ASN (Autonomous System Number). ISPs and large companies are each an AS.

**Attenuation:** Reduction in signal strength as it travels through a medium. All guided media attenuate with distance.

**Bandwidth:** Maximum data transfer capacity of a link (pipe width). Measured in bps.

**BGP (Border Gateway Protocol):** The routing protocol connecting autonomous systems across the internet. Handles 900,000+ routes in the global routing table.

**Broadcast Domain:** All devices that receive a Layer 2 broadcast frame. Routers and VLANs create separate broadcast domains.

**CIDR (Classless Inter-Domain Routing):** Variable-length subnet masking using prefix notation (/24, /26). Replaced classful addressing.

**Collision Domain:** All devices that can cause a collision if transmitting simultaneously. Modern switches create one collision domain per port.

**CRC (Cyclic Redundancy Check):** Error detection algorithm used in Ethernet FCS field.

**CSMA/CA:** Collision avoidance mechanism for wireless networks — wait for idle + random backoff before transmitting.

**CSMA/CD:** Collision detection mechanism for wired Ethernet — transmit when idle, detect and recover from collisions. Largely obsolete with modern switches.

**Default Gateway:** Router's IP address on a local network. Packets destined for other networks are sent here.

**DHCP (Dynamic Host Configuration Protocol):** Automatically assigns IP configuration (address, mask, gateway, DNS) to devices via the DORA process.

**DNS (Domain Name System):** Hierarchical distributed system translating domain names to IP addresses.

**Encapsulation:** Adding headers/trailers at each OSI layer as data moves down the stack on the sender.

**FCS (Frame Check Sequence):** 4-byte CRC value appended to Ethernet frames for error detection.

**Firewall:** Device filtering network traffic based on configured rules — packet filter, stateful, NGFW.

**Fragment:** A portion of an IP packet created when the original packet exceeds the MTU of a link.

**FTP (File Transfer Protocol):** Two-connection file transfer protocol. Insecure — use SFTP instead.

**Full Duplex:** Simultaneous bidirectional communication. Eliminates collisions on modern switched Ethernet.

**HTTP (HyperText Transfer Protocol):** Application protocol for web communication. Port 80, TCP.

**HTTPS:** HTTP + TLS encryption. Port 443, TCP. Provides confidentiality, integrity, authentication.

**Hub:** Layer 1 device repeating all incoming bits to all ports. Creates one collision domain. Completely obsolete.

**ICMP (Internet Control Message Protocol):** Layer 3 protocol for diagnostics (ping, traceroute) and error reporting.

**IDS/IPS (Intrusion Detection/Prevention System):** Monitors network traffic for malicious patterns. IDS alerts; IPS blocks.

**IMAP (Internet Message Access Protocol):** Email retrieval protocol keeping messages on server for multi-device sync. Port 143.

**IP (Internet Protocol):** Layer 3 protocol providing logical addressing and best-effort packet delivery.

**IPsec:** Suite of protocols for IP-level encryption and authentication. Used in VPNs.

**ISP (Internet Service Provider):** Company providing internet access to consumers and businesses.

**Latency:** Time delay for data to travel from source to destination. Components: propagation, transmission, processing, queuing delay.

**Link-Local Address:** IPv4 169.254.x.x (APIPA) or IPv6 fe80::/10 — auto-configured, valid only on local network segment.

**MAC Address:** 48-bit hardware address assigned to every NIC. Unique globally. Used for Layer 2 delivery.

**MTU (Maximum Transmission Unit):** Maximum frame/packet size on a medium. 1500 bytes for Ethernet.

**NAT (Network Address Translation):** Translates private IP addresses to public for internet access. PAT maps multiple private IPs to one public IP using port numbers.

**NIC (Network Interface Card):** Hardware connecting a device to a network. Has a MAC address.

**OSPF (Open Shortest Path First):** Link-state routing protocol using Dijkstra's algorithm. Standard enterprise IGP.

**Packet:** Layer 3 data unit containing IP header and payload.

**POP3 (Post Office Protocol v3):** Email retrieval protocol downloading messages to device. Port 110.

**Port:** 16-bit number identifying an application/service on a host.

**QoS (Quality of Service):** Mechanisms prioritizing certain traffic types (voice, video) over others.

**RIP (Routing Information Protocol):** Simple distance-vector routing protocol using hop count. Maximum 15 hops.

**Router:** Layer 3 device routing packets between different IP networks using IP routing table.

**Routing Table:** Database in router listing known destination networks, next-hop routers, and outgoing interfaces.

**SMTP (Simple Mail Transfer Protocol):** Email sending protocol. Port 25 (server-to-server), 587 (client submission).

**SNMP (Simple Network Management Protocol):** Network monitoring and management protocol. UDP ports 161/162.

**SSH (Secure Shell):** Encrypted remote access protocol. Port 22. Replaces insecure Telnet.

**STP (Spanning Tree Protocol):** Prevents Layer 2 loops in switched networks by blocking redundant paths.

**Subnet:** A logically divided portion of an IP network sharing the same network address prefix.

**Subnet Mask:** 32-bit number identifying network and host portions of an IP address.

**Switch:** Layer 2 device forwarding frames based on MAC addresses. Creates separate collision domains per port.

**TCP (Transmission Control Protocol):** Reliable, connection-oriented, ordered transport protocol. Used for HTTP, HTTPS, SSH, email.

**Telnet:** Unencrypted remote access. Port 23. Never use — replaced by SSH.

**TLS/SSL (Transport Layer Security):** Cryptographic protocol providing encrypted, authenticated communication. Used by HTTPS.

**TTL (Time to Live):** Decremented at each router hop. Prevents packets looping forever. Also used in DNS for cache duration.

**UDP (User Datagram Protocol):** Fast, connectionless, unreliable transport protocol. Used for DNS, VoIP, streaming, gaming.

**VLAN (Virtual LAN):** Logical network segmentation within a physical switch. Isolates broadcast domains.

**VPN (Virtual Private Network):** Encrypted tunnel over public network for secure remote access.

**WAN (Wide Area Network):** Network spanning large geographic distances. The internet is the largest WAN.

**Wireshark:** Free network protocol analyzer capturing and displaying real network traffic.

**802.11:** IEEE standard governing Wi-Fi wireless networking (b/g/n/ac/ax generations).

**802.1Q:** IEEE standard for VLAN tagging on Ethernet trunk links (4-byte tag added to frame).

---

> **Navigation:** [Back to Repository README](./README.md) | [Next: 02_CN_Interview_Prep.md →](./02_CN_Interview_Prep.md)

---

*File: `01_CN_Masterguide.md` | Version 1.0 | 2026*
*Part of the Computer Networks Repository*
*Pair with `03_CN_Practice_Repository.md` for hands-on labs*
