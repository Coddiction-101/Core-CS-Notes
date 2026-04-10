# 🎯 02 — Computer Networks Interview & Internship Prep
### Only What Gets Asked | 2026 Edition | Job Ready

> **File:** `02_CN_Interview_Prep.md`
> **Part of:** Computer Networks Repository → [Back to README](https://github.com/Coddiction-101/Core-CS-Notes/tree/main/CN__Computer-Networking)
> **Previous:** [01_CN_Masterguide.md](https://github.com/Coddiction-101/Core-CS-Notes/tree/main/CN__Computer-Networking/CN--Masterguide) | **Next:** [03_CN_Practice_Repository.md](./03_CN_Practice_Repository.md)

---

## 🎯 What You Got (~80 Pages):

### ONLY What Actually Gets Asked in 2026:

✅ **What to Study vs Skip** — Saves 40% time by cutting dead-weight topics

✅ **OSI & TCP/IP Models (20%)** — Layer-by-layer with exact interview answers

✅ **IP Addressing & Subnetting (25%)** — The #1 practical skill tested in writing

✅ **Core Protocols — TCP & UDP (20%)** — Handshake, ports, differences

✅ **Application Protocols (10%)** — DNS, DHCP, HTTP, ARP, SSH — how they work

✅ **Routing & Switching (15%)** — How packets find their way, VLANs

✅ **Network Security (10%)** — Attacks, firewalls, TLS, VPN

✅ **50 Most Asked Questions** — With detailed, speakable answers

✅ **Real-World Scenarios** — "What happens when you type google.com?"

✅ **Commands Cheat Sheet** — Every networking command you need

✅ **2-Week Study Plan** — Day-by-day with daily goals

✅ **Readiness Checklist** — Know exactly when you're interview-ready

---

## 🔥 Key Features:

### 1. What to Skip (Save Time!):

❌ Manchester encoding and NRZ signal details (never asked)

❌ Token Ring and FDDI (completely obsolete — dead tech)

❌ BGP deep internals — AS path attributes, communities (unless ISP/network role)

❌ OSPF LSA types in detail (only concept level needed)
❌ ATM and Frame Relay (legacy protocols — extinct)
❌ Layer 6 Presentation Layer in depth (only asked conceptually)
❌ Detailed hardware specs of cables (Cat6 max speed is enough — no one asks pinout)
❌ IPv6 migration strategies in depth (only basics needed)
❌ STP port states and timers in detail (only concept needed)
❌ SNMP MIB structure in detail (concept only)

### 2. What to MASTER (Asked 80%+ times):
⭐⭐⭐⭐⭐ **OSI Model — All 7 Layers** (Asked in 95% of networking interviews!)
⭐⭐⭐⭐⭐ **TCP vs UDP** (Must know cold — asked in every single interview!)
⭐⭐⭐⭐⭐ **TCP Three-Way Handshake** (Draw it from memory every time!)
⭐⭐⭐⭐⭐ **What happens when you type a URL** (Most common scenario question!)
⭐⭐⭐⭐⭐ **IP Addressing + Subnetting** (Written test — tested in 80% of companies!)
⭐⭐⭐⭐⭐ **Switch vs Router vs Hub** (Asked everywhere — must explain with analogy!)
⭐⭐⭐⭐ **DNS Resolution** (End-to-end — resolver to authoritative)
⭐⭐⭐⭐ **HTTP vs HTTPS + Status Codes** (Asked in dev + networking roles both)
⭐⭐⭐⭐ **DHCP DORA Process** (Draw it, explain it)
⭐⭐⭐⭐ **NAT and Private IP Ranges** (Must memorize ranges)
⭐⭐⭐ **Firewalls, VPN, TLS** (Security basics)
⭐⭐⭐ **VLANs** (Enterprise networking + dev-ops roles)

---

## 📊 Coverage Breakdown:

### Section 1: OSI Model (20% of interviews)
### Section 2: TCP/IP Model + OSI vs TCP/IP Comparison
### Section 3: IP Addressing & Subnetting (25% — the biggest practical section)
### Section 4: TCP & UDP + Port Numbers (20%)
### Section 5: DNS, DHCP, ARP (10%)
### Section 6: HTTP, HTTPS, FTP, SSH, Email (10%)
### Section 7: Routing & Switching + VLANs (15%)
### Section 8: Network Security (10%)
### Section 9: 50 Most Asked Interview Questions
### Section 10: Real-World Scenarios
### Section 11: Commands Cheat Sheet
### Section 12: 2-Week Study Plan
### Section 13: Readiness Checklist + Last-Day Rapid Review

---
---

# Section 1: OSI Model 🧱

## The 7 Layers — Master Reference Table

```
┌────┬──────────────┬───────────┬──────────────────────────┬──────────────────┐
│  # │  Layer Name  │ Data Unit │ Key Protocols            │ Key Devices      │
├────┼──────────────┼───────────┼──────────────────────────┼──────────────────┤
│  7 │ Application  │ Message   │ HTTP, HTTPS, FTP, DNS    │ Gateway, Proxy   │
│    │              │           │ SMTP, SSH, Telnet, SNMP  │                  │
├────┼──────────────┼───────────┼──────────────────────────┼──────────────────┤
│  6 │ Presentation │ Data      │ SSL/TLS, JPEG, MPEG, GIF │ —                │
│    │              │           │ ASCII, EBCDIC encoding   │                  │
├────┼──────────────┼───────────┼──────────────────────────┼──────────────────┤
│  5 │ Session      │ Data      │ NetBIOS, RPC, PPTP       │ —                │
├────┼──────────────┼───────────┼──────────────────────────┼──────────────────┤
│  4 │ Transport    │ Segment / │ TCP, UDP                 │ Firewall,        │
│    │              │ Datagram  │ Port numbers             │ Load Balancer    │
├────┼──────────────┼───────────┼──────────────────────────┼──────────────────┤
│  3 │ Network      │ Packet    │ IP, ICMP, ARP, OSPF, BGP │ Router           │
├────┼──────────────┼───────────┼──────────────────────────┼──────────────────┤
│  2 │ Data Link    │ Frame     │ Ethernet (802.3)         │ Switch, Bridge   │
│    │              │           │ Wi-Fi (802.11), PPP      │ NIC              │
├────┼──────────────┼───────────┼──────────────────────────┼──────────────────┤
│  1 │ Physical     │ Bit       │ Cat5e/6/6A, Fiber, DSL   │ Hub, Repeater    │
│    │              │           │ Radio waves, Coaxial     │ NIC (hardware)   │
└────┴──────────────┴───────────┴──────────────────────────┴──────────────────┘
```

## Layer-by-Layer — Interview-Ready Descriptions

### Layer 7 — Application ⭐⭐⭐⭐⭐
**One-line:** The interface between network and applications — where HTTP, DNS, and FTP live.
**Key point:** This is NOT your browser app — it is the **protocol** your browser uses (HTTP/HTTPS).
**Protocols:** HTTP (80), HTTPS (443), FTP (21), SMTP (25), DNS (53), DHCP (67/68), SSH (22), Telnet (23), SNMP (161)

### Layer 6 — Presentation ⭐⭐
**One-line:** Translates, encrypts, and compresses data so both sides can understand each other.
**Key point:** SSL/TLS encryption sits here in OSI. Data format translation (ASCII ↔ EBCDIC).
**Key point for interviews:** When people say "SSL is at Application Layer," they mean in TCP/IP model — in OSI it is Layer 6.

### Layer 5 — Session ⭐⭐
**One-line:** Manages the "session" — who opens it, keeps it alive, and closes it.
**Analogy:** Like managing a phone call — dial (establish), talk (maintain), hang up (terminate).
**Protocols:** NetBIOS, RPC

### Layer 4 — Transport ⭐⭐⭐⭐⭐
**One-line:** End-to-end delivery between applications using port numbers.
**Key point:** TCP = reliable + ordered. UDP = fast + connectionless. Port numbers identify applications.
**Data units:** TCP → Segment | UDP → Datagram

### Layer 3 — Network ⭐⭐⭐⭐⭐
**One-line:** Logical addressing (IP) and routing — gets packets from ANY source to ANY destination.
**Key point:** IP addresses live here. Routers operate here. Packets can cross multiple networks.
**Data unit:** Packet

### Layer 2 — Data Link ⭐⭐⭐⭐⭐
**One-line:** Delivers frames between two adjacent nodes on the SAME network using MAC addresses.
**Key point:** MAC addresses live here. Switches operate here. Only local delivery.
**Data unit:** Frame

### Layer 1 — Physical ⭐⭐⭐
**One-line:** Converts bits to signals (electrical, light, radio) and transmits over physical medium.
**Key point:** No addressing — just raw bit transmission. Hubs repeat bits to all ports.
**Data unit:** Bit

---

## Encapsulation — The Process You Must Know ⭐⭐⭐⭐⭐

```
SENDER → data travels DOWN the layers:

App data  →  [Data]
             ↓ Transport adds TCP header (port numbers)
             [TCP][Data]  =  Segment
             ↓ Network adds IP header (IP addresses)
             [IP][TCP][Data]  =  Packet
             ↓ Data Link adds Ethernet header + FCS (MAC addresses)
             [ETH][IP][TCP][Data][FCS]  =  Frame
             ↓ Physical converts to bits
             01010101010...  =  Bits on the wire

RECEIVER → data travels UP the layers (each layer strips its header)
```

**The one rule that trips everyone up:**
- **MAC addresses (Layer 2) change at every router hop**
- **IP addresses (Layer 3) stay the same end-to-end**

---

## OSI Mnemonics ⭐⭐⭐⭐⭐

**Top → Bottom (7 to 1):** **A**ll **P**eople **S**eem **T**o **N**eed **D**ata **P**rocessing

**Bottom → Top (1 to 7):** **P**lease **D**o **N**ot **T**hrow **S**ausage **P**izza **A**way

---
---

# Section 2: TCP/IP Model 🔌

## 4-Layer Breakdown

```
┌──────────────────┬─────────────────────┬─────────────────────────────────┐
│ TCP/IP Layer     │ OSI Equivalent      │ Key Protocols                   │
├──────────────────┼─────────────────────┼─────────────────────────────────┤
│ Application      │ Layer 5 + 6 + 7     │ HTTP, HTTPS, FTP, DNS, SMTP     │
│                  │                     │ SSH, DHCP, SNMP, Telnet         │
├──────────────────┼─────────────────────┼─────────────────────────────────┤
│ Transport        │ Layer 4             │ TCP, UDP                        │
├──────────────────┼─────────────────────┼─────────────────────────────────┤
│ Internet         │ Layer 3             │ IP (v4/v6), ICMP, ARP, IGMP     │
├──────────────────┼─────────────────────┼─────────────────────────────────┤
│ Network Access   │ Layer 1 + 2         │ Ethernet, Wi-Fi, PPP            │
│ (Link Layer)     │                     │ Cables, NICs, Switches          │
└──────────────────┴─────────────────────┴─────────────────────────────────┘
```

## OSI vs TCP/IP — The Comparison Table ⭐⭐⭐⭐⭐

| Feature | OSI Model | TCP/IP Model |
|---------|-----------|--------------|
| Full Name | Open Systems Interconnection | Transmission Control Protocol/Internet Protocol |
| Layers | 7 | 4 |
| Developed By | ISO (1984) | DARPA (1970s) |
| Purpose | Conceptual reference — teaching + troubleshooting | Practical implementation — actual internet |
| Usage Today | Understanding + explaining | Real-world internet operation |
| Protocol Specific? | No — generic framework | Yes — TCP and IP are specific |
| Where Reliability? | Can be at multiple layers | Transport layer (TCP) |

## Interview One-Liner ⭐⭐⭐⭐⭐
*"OSI is the 7-layer theoretical model we use to understand and troubleshoot networks. TCP/IP is the 4-layer practical model the actual internet runs on. OSI gives us the language; TCP/IP is the implementation."*

---
---

# Section 3: IP Addressing & Subnetting 📍

## IPv4 — The Basics ⭐⭐⭐⭐⭐

A 32-bit address written as 4 decimal octets separated by dots.
```
192  .  168  .   1   .  100
 ↑       ↑        ↑       ↑
8 bits  8 bits  8 bits  8 bits  =  32 bits total
Range: 0-255  for each octet
Total: 2³² = 4,294,967,296 addresses (~4.3 billion) — ALL EXHAUSTED
```

---

## IP Address Classes ⭐⭐⭐⭐

| Class | First Octet | Default Mask | Max Hosts | Purpose |
|-------|------------|-------------|----------|---------|
| **A** | 1 – 126 | 255.0.0.0 (/8) | 16,777,214 | Large orgs, ISPs |
| **B** | 128 – 191 | 255.255.0.0 (/16) | 65,534 | Medium orgs |
| **C** | 192 – 223 | 255.255.255.0 (/24) | 254 | Small networks |
| **D** | 224 – 239 | N/A | — | Multicast |
| **E** | 240 – 255 | N/A | — | Experimental |

> ⚠️ **127.x.x.x = Loopback (localhost)** — Not in any class above. Testing your own TCP/IP stack.

---

## Private IP Ranges — Must Memorize ⭐⭐⭐⭐⭐

```
┌──────────────────────────────────────────────────────────────────────┐
│  Class A:  10.0.0.0  –  10.255.255.255      →  10.0.0.0/8           │
│  Class B:  172.16.0.0 – 172.31.255.255      →  172.16.0.0/12        │
│  Class C:  192.168.0.0 – 192.168.255.255    →  192.168.0.0/16       │
└──────────────────────────────────────────────────────────────────────┘
```

**Not routable on the internet.** Your home Wi-Fi (192.168.1.x) is private.
**NAT** allows these private IPs to access the internet through one public IP.

---

## Special Addresses — Must Know ⭐⭐⭐⭐⭐

| Address | Purpose | Seen When |
|---------|---------|----------|
| **127.0.0.1** | Loopback / localhost | Testing local TCP/IP stack |
| **0.0.0.0** | Default route / unspecified | Routing tables ("catch all") |
| **255.255.255.255** | Limited broadcast | DHCP Discover, all local devices |
| **169.254.x.x** | APIPA — DHCP failed! | Device couldn't find DHCP server ⚠️ |

**APIPA Tip for Interviews:** If you see 169.254.x.x on a Windows machine, DHCP has failed. Check cable, Wi-Fi connection, or DHCP server. The device has no gateway → no internet.

---

## Subnetting — The Formula ⭐⭐⭐⭐⭐

```
Given prefix /n:

Total addresses       = 2^(32 - n)
Usable host addresses = 2^(32 - n) - 2
Block size            = 256 - (value of subnet mask in interesting octet)

Network address       = first address in the block (all host bits = 0)
Broadcast address     = last address in the block (all host bits = 1)
First usable host     = Network address + 1
Last usable host      = Broadcast address - 1
```

---

## Subnetting Quick Reference Table ⭐⭐⭐⭐⭐

| Prefix | Subnet Mask | Addresses | Usable Hosts | Block Size |
|--------|-------------|-----------|-------------|------------|
| /24 | 255.255.255.0 | 256 | **254** | 256 |
| /25 | 255.255.255.128 | 128 | **126** | 128 |
| /26 | 255.255.255.192 | 64 | **62** | 64 |
| /27 | 255.255.255.224 | 32 | **30** | 32 |
| /28 | 255.255.255.240 | 16 | **14** | 16 |
| /29 | 255.255.255.248 | 8 | **6** | 8 |
| /30 | 255.255.255.252 | 4 | **2** | 4 |
| /32 | 255.255.255.255 | 1 | 1 host route | — |

> 💡 **Quick rule:** Usable hosts = Total addresses − 2 (network + broadcast)

---

## Solved Subnetting Example ⭐⭐⭐⭐⭐

**Q: Find network, broadcast, first host, last host for `192.168.10.200/26`**

**Step 1:** /26 → Mask = 255.255.255.192 → Block size = 256 − 192 = **64**

**Step 2:** Blocks in 4th octet: 0, 64, 128, **192**, 256
→ 200 falls in the block starting at **192**

**Step 3:**
```
Network Address   =  192.168.10.192
Broadcast         =  192.168.10.255   (192 + 64 − 1)
First Host        =  192.168.10.193
Last Host         =  192.168.10.254
Usable Hosts      =  62
```

---

## VLSM — Variable Length Subnet Masking ⭐⭐⭐

Assign different prefix lengths to different subnets based on actual need. Avoids wasting addresses.

**Example:** Company has `10.1.0.0/24`, needs:
- Dept A: 100 hosts → /25 (126 usable) → `10.1.0.0/25`
- Dept B: 50 hosts → /26 (62 usable) → `10.1.0.128/26`
- Dept C: 25 hosts → /27 (30 usable) → `10.1.0.192/27`
- Link: 2 hosts → /30 (2 usable) → `10.1.0.224/30`

**Rule:** Assign largest subnet first. Start from .0. Don't overlap ranges.

---

## IPv6 — Basics ⭐⭐⭐

**Why:** IPv4 exhausted in 2011. IPv6 = 128-bit = 3.4 × 10³⁸ addresses.

```
Full:       2001:0db8:85a3:0000:0000:8a2e:0370:7334
Short:      2001:db8:85a3::8a2e:370:7334
             ↑ Leading zeros dropped, consecutive zeros → ::
Loopback:   ::1   (equivalent to 127.0.0.1)
```

| Feature | IPv4 | IPv6 |
|---------|------|------|
| Size | 32 bits | 128 bits |
| Format | Decimal dotted | Hex with colons |
| Broadcast | Yes | No (Multicast instead) |
| Auto-config | DHCP | SLAAC (self-configuring) |
| IPSec | Optional | Built-in |
| Loopback | 127.0.0.1 | ::1 |
| Header | Variable (20+ bytes) | Fixed (40 bytes) |

---
---

# Section 4: TCP and UDP 🚀

## TCP — Transmission Control Protocol ⭐⭐⭐⭐⭐

| Property | Value |
|----------|-------|
| Connection | ✅ Connection-oriented (handshake required) |
| Reliability | ✅ Guaranteed delivery (ACKs + retransmit) |
| Ordering | ✅ Sequence numbers ensure order |
| Flow Control | ✅ Window size prevents overwhelming receiver |
| Congestion Control | ✅ Slow Start, Congestion Avoidance |
| Speed | ❌ Slower due to overhead |
| Header | 20 bytes minimum |

---

## TCP Three-Way Handshake ⭐⭐⭐⭐⭐

```
CLIENT                                    SERVER
  │                                          │
  │──── [SYN] Seq=1000 ────────────────────► │
  │     "Hello, my sequence starts at 1000"  │
  │                                          │
  │◄─── [SYN-ACK] Seq=5000, Ack=1001 ───────│
  │     "Got it. Mine starts at 5000"        │
  │                                          │
  │──── [ACK] Ack=5001 ────────────────────► │
  │     "Got yours. Connection established!" │
  │                                          │
  │══════════ DATA TRANSFER ════════════════ │
```

**Why 3 steps and not 2?**
Both sides must:
1. Send their own Initial Sequence Number (SYN)
2. Confirm they received the other's ISN (ACK)
A 2-way handshake cannot accomplish both independently — the SYN-ACK does two jobs at once.

---

## TCP Four-Way Connection Close ⭐⭐⭐⭐

```
CLIENT                      SERVER
  │──── [FIN] ─────────────► │   "I'm done sending"
  │◄─── [ACK] ───────────── │   "Noted"
  │◄─── [FIN] ───────────── │   "I'm done too"
  │──── [ACK] ─────────────► │   "Got it — connection closed"
```

Each direction closes independently. That's why it needs 4 messages, not 3.

---

## TCP Flags — Know These ⭐⭐⭐⭐

| Flag | Full Name | When Used |
|------|-----------|----------|
| **SYN** | Synchronize | Connection setup — sends sequence number |
| **ACK** | Acknowledge | Confirms receipt of data |
| **FIN** | Finish | Graceful connection close |
| **RST** | Reset | Abrupt connection abort (error condition) |
| **PSH** | Push | Deliver data to app immediately (don't buffer) |
| **URG** | Urgent | Urgent data needs priority processing |

---

## UDP — User Datagram Protocol ⭐⭐⭐⭐⭐

| Property | Value |
|----------|-------|
| Connection | ❌ Connectionless (no handshake) |
| Reliability | ❌ Best effort (no guarantee) |
| Ordering | ❌ Not guaranteed |
| Speed | ✅ Fast — minimal overhead |
| Header | 8 bytes fixed |

**When UDP wins over TCP:**
- Real-time audio/video (VoIP, Zoom, Teams) — a late packet is worse than a dropped one
- DNS queries — tiny request/response, retry if no reply
- Online gaming — stale position data is useless — send new, don't retransmit old
- Live streaming — a slightly degraded frame is better than buffering
- DHCP — client has no IP yet, cannot establish TCP connection

---

## TCP vs UDP — The Master Comparison ⭐⭐⭐⭐⭐

| Feature | TCP | UDP |
|---------|-----|-----|
| Type | Connection-oriented | Connectionless |
| Reliability | Guaranteed | Best effort |
| Ordering | Guaranteed | Not guaranteed |
| Speed | Slower | Faster |
| Header Size | 20 bytes (min) | 8 bytes |
| Flow Control | ✅ Yes | ❌ No |
| Congestion Control | ✅ Yes | ❌ No |
| Use Cases | HTTP, HTTPS, FTP, SSH, Email | DNS, DHCP, VoIP, Streaming, Gaming |

---

## Port Numbers — Must Memorize ⭐⭐⭐⭐⭐

| Port | Protocol | Service | TCP/UDP |
|------|----------|---------|---------|
| **20** | FTP | File Transfer — Data | TCP |
| **21** | FTP | File Transfer — Control | TCP |
| **22** | SSH | Secure Remote Access | TCP |
| **23** | Telnet | Insecure Remote Access ⚠️ | TCP |
| **25** | SMTP | Send Email (server-to-server) | TCP |
| **53** | DNS | Domain Name Resolution | **TCP + UDP** |
| **67** | DHCP | DHCP Server | UDP |
| **68** | DHCP | DHCP Client | UDP |
| **80** | HTTP | Web (unencrypted) | TCP |
| **110** | POP3 | Email Download (old) | TCP |
| **143** | IMAP | Email Sync (modern) | TCP |
| **161** | SNMP | Network Monitoring (query) | UDP |
| **162** | SNMP | Network Monitoring (trap) | UDP |
| **443** | HTTPS | Secure Web | TCP |
| **587** | SMTP | Email Submission (client→server) | TCP |
| **3389** | RDP | Remote Desktop (Windows) | TCP |

**Port Ranges:**
```
0  –  1023   →  Well-Known (system services — root required to open)
1024 – 49151  →  Registered (specific applications)
49152 – 65535 →  Ephemeral/Dynamic (temporary client connections)
```

---
---

# Section 5: DNS, DHCP, ARP 📡

## DNS — Domain Name System ⭐⭐⭐⭐⭐

**What it does:** Translates human-readable names (google.com) to IP addresses (142.250.195.78). The internet's phone book.

### DNS Resolution — Step by Step

```
You type: www.youtube.com

1. Browser DNS cache → Miss
2. OS checks hosts file → Not found
3. Query sent to Recursive Resolver (8.8.8.8 or ISP's resolver)
4. Resolver cache → Miss
5. Resolver → Root Server: "Who handles .com?"
6. Root Server → "Ask the .com TLD server at 192.5.6.30"
7. Resolver → .com TLD Server: "Who handles youtube.com?"
8. TLD Server → "Ask YouTube's NS: ns1.google.com"
9. Resolver → YouTube's Authoritative NS: "What is www.youtube.com?"
10. Auth NS → "142.250.x.x, TTL 300"
11. Resolver caches answer for 300 seconds
12. Returns IP to your browser
13. Browser connects to 142.250.x.x
```

### DNS Record Types ⭐⭐⭐⭐

| Record | Purpose | Example |
|--------|---------|---------|
| **A** | Domain → IPv4 | google.com → 142.250.195.78 |
| **AAAA** | Domain → IPv6 | google.com → 2404:6800::x |
| **CNAME** | Alias to another domain | www.example.com → example.com |
| **MX** | Email server | gmail.com → smtp.google.com (priority 5) |
| **NS** | Authoritative name servers | google.com → ns1.google.com |
| **PTR** | Reverse DNS (IP → domain) | 78.195.250.142... → google.com |
| **TXT** | Text info | SPF, DKIM, domain verification |

### DNS Transport: UDP or TCP?
- **UDP port 53** — Standard queries (fast, small request/response)
- **TCP port 53** — Large responses, Zone transfers (AXFR)

---

## DHCP — Dynamic Host Configuration Protocol ⭐⭐⭐⭐⭐

**What it does:** Automatically assigns IP address, subnet mask, gateway, and DNS to devices joining the network.

### DORA Process — The Four Messages

```
CLIENT                              DHCP SERVER
  │                                      │
  │──[D] DISCOVER ─────────────────────► │
  │   Broadcast: 255.255.255.255          │
  │   "Anyone there? I need an IP!"      │
  │                                      │
  │◄──[O] OFFER ─────────────────────── │
  │   "You can have 192.168.1.50         │
  │    Gateway: 192.168.1.1              │
  │    DNS: 8.8.8.8 | Lease: 24 hrs"    │
  │                                      │
  │──[R] REQUEST ───────────────────────► │
  │   Broadcast: "I accept 192.168.1.50  │
  │   from Server X"                     │
  │                                      │
  │◄──[A] ACKNOWLEDGE ─────────────────── │
  │   "Confirmed! 192.168.1.50 is yours" │
```

**D → O → R → A = Discover → Offer → Request → Acknowledge**

**What DHCP assigns:**
- IP Address
- Subnet Mask
- Default Gateway
- DNS Server(s)
- Lease Duration (typically 24 hours to 7 days)

**DHCP Reservation:** Map a MAC address to always receive the same IP. Used for servers, printers, network equipment.

---

## ARP — Address Resolution Protocol ⭐⭐⭐⭐

**Problem:** You have a destination IP. You need the MAC address to send the Ethernet frame on your local network.
**Solution:** Broadcast "Who has this IP?" and the device replies with its MAC.

```
Device A (192.168.1.10) wants to reach Device B (192.168.1.5):

Step 1 — ARP Request (BROADCAST):
  "Who has 192.168.1.5? Tell 192.168.1.10"
  Destination MAC: FF:FF:FF:FF:FF:FF  ← goes to everyone

Step 2 — ARP Reply (UNICAST from B):
  "192.168.1.5 is at AA:BB:CC:DD:EE:FF"
  Sent directly to Device A only

Step 3:
  Device A stores (192.168.1.5 → AA:BB:CC:DD:EE:FF) in ARP cache
  Now sends frame with correct destination MAC
```

**View ARP table:** `arp -a` (Windows/Linux)

**ARP Spoofing attack:** Attacker sends fake ARP replies → traffic redirected through attacker = Man-in-the-Middle. Defense: Dynamic ARP Inspection (DAI) on switches, HTTPS everywhere.

---
---

# Section 6: HTTP, HTTPS, FTP, SSH, Email 🌍

## HTTP & HTTPS ⭐⭐⭐⭐⭐

| Feature | HTTP | HTTPS |
|---------|------|-------|
| Port | 80 | 443 |
| Encryption | ❌ Plaintext | ✅ TLS encrypted |
| Security | Anyone can read traffic | Unreadable if intercepted |
| Auth | No server verification | Certificate verifies server identity |
| Use | Never for sensitive data | Always — default for all sites |

### HTTP Methods ⭐⭐⭐⭐

| Method | Purpose | Has Body? |
|--------|---------|-----------|
| GET | Retrieve resource | No |
| POST | Submit data / create | Yes |
| PUT | Replace resource entirely | Yes |
| PATCH | Partially update resource | Yes |
| DELETE | Remove resource | No |
| HEAD | Headers only (no body) | No |

### HTTP Status Codes ⭐⭐⭐⭐⭐

```
2xx SUCCESS:
  200 OK              — Request succeeded
  201 Created         — Resource created (POST success)
  204 No Content      — Success, no response body

3xx REDIRECTION:
  301 Moved Permanently  — URL changed forever (update bookmarks)
  302 Found              — Temporary redirect
  304 Not Modified       — Use cached version

4xx CLIENT ERRORS:
  400 Bad Request        — Malformed request
  401 Unauthorized       — Must authenticate first
  403 Forbidden          — Authenticated but no permission
  404 Not Found          — Resource doesn't exist
  429 Too Many Requests  — Rate limited

5xx SERVER ERRORS:
  500 Internal Server Error  — Generic server failure
  502 Bad Gateway            — Upstream server bad response
  503 Service Unavailable    — Server down or overloaded
  504 Gateway Timeout        — Upstream server timed out
```

### TLS — What HTTPS Adds ⭐⭐⭐⭐⭐

TLS provides three guarantees:
1. **Confidentiality** — data is encrypted, unreadable if intercepted
2. **Integrity** — data cannot be modified in transit without detection
3. **Authentication** — the server's certificate proves its identity (verified by CA)

```
TLS Handshake (simplified):
Client → "Hello, I support TLS 1.3, here are my cipher suites"
Server → "OK, I choose AES-256. Here's my certificate."
Client → Verifies certificate with trusted Certificate Authority
Client → Sends key material encrypted with server's public key
Server → Decrypts with private key
Both → Derive same symmetric session key
Data  → All traffic encrypted with symmetric key (fast!)
```

**HTTP versions at a glance:**
- **HTTP/1.1** — One request at a time per connection (sequential)
- **HTTP/2** — Multiple requests simultaneously (multiplexing) + header compression
- **HTTP/3** — Built on QUIC (UDP) — lower latency, no head-of-line blocking

---

## FTP vs SFTP ⭐⭐⭐

| Protocol | Port | Encryption | Use Today |
|----------|------|-----------|----------|
| FTP | 21 (control) + 20 (data) | ❌ None — plaintext | ❌ Never |
| FTPS | 990 | ✅ TLS | Rare |
| SFTP | 22 | ✅ SSH | ✅ Standard |

**One-line:** FTP sends passwords in plaintext. Always use SFTP (runs over SSH port 22).

---

## SSH vs Telnet ⭐⭐⭐⭐

| Feature | SSH | Telnet |
|---------|-----|--------|
| Port | 22 | 23 |
| Encryption | ✅ Full session encryption | ❌ Completely plaintext |
| Auth options | Password + Key pairs | Password only (sent in plaintext) |
| Use Today | ✅ Standard for all remote access | ❌ Dead — never use |

**Interview answer:** *"Telnet sends everything including passwords in plaintext — anyone on the network can capture it. SSH encrypts the entire session. Telnet should never be used in any modern environment."*

---

## Email Protocols ⭐⭐⭐

| Protocol | Port | Direction | Key Behavior |
|----------|------|-----------|-------------|
| **SMTP** | 25 / 587 | Sending | Client → Server, Server → Server |
| **POP3** | 110 | Receiving | Downloads email, usually deletes from server |
| **IMAP** | 143 | Receiving | Syncs email — stays on server across all devices |

**One-line:**
SMTP sends. POP3 downloads (one device). IMAP syncs (all devices — used by Gmail, Outlook).

---
---

# Section 7: Routing & Switching 🔀

## MAC vs IP Address ⭐⭐⭐⭐⭐

| Feature | MAC Address | IP Address |
|---------|------------|-----------|
| OSI Layer | Layer 2 (Data Link) | Layer 3 (Network) |
| Type | Physical / Hardware | Logical / Software |
| Assigned By | Manufacturer (burned in) | DHCP or manually configured |
| Scope | Local network only | Global internet |
| Format | 48-bit hex (AA:BB:CC:DD:EE:FF) | 32-bit decimal (192.168.1.1) |
| Changes? | Permanent (mostly) | Yes — changes per network |
| Purpose | Deliver within same network | Route across different networks |
| Changes at routers? | ✅ YES — new frame each hop | ❌ NO — same end-to-end |

**Analogy:** MAC is your name. IP is your current address. Your name doesn't change when you move — but your address does.

---

## Hub vs Switch vs Router ⭐⭐⭐⭐⭐

| Feature | Hub | Switch | Router |
|---------|-----|--------|--------|
| OSI Layer | Layer 1 | Layer 2 | Layer 3 |
| Forwards Based On | Nothing — broadcasts all | MAC Address | IP Address |
| Collision Domain | 1 (all devices share) | 1 per port (separate each) | 1 per interface |
| Broadcast Domain | 1 | 1 (per VLAN) | Separate per interface |
| Intelligence | ❌ None | ✅ MAC table | ✅ Routing table |
| Status | Obsolete | Used everywhere | Used everywhere |

**The analogy that works in interviews:**
> Hub = shouting in a room (everyone hears everything)
> Switch = a city's internal roads (knows which house is where)
> Router = a highway connecting cities (routes between different networks)

---

## How a Switch Builds Its MAC Table ⭐⭐⭐⭐

```
1. Frame arrives on Port 3 from AA:BB:CC:11:22:33
   Switch records: AA:BB:CC:11:22:33 → Port 3  (LEARNING)

2. Frame is destined for AA:BB:CC:44:55:66
   Switch checks table:
   → Found at Port 5: forward ONLY to Port 5  (UNICAST FORWARD)
   → Not found: flood to ALL ports except Port 3  (UNKNOWN UNICAST FLOOD)
   → Destination = FF:FF:FF:FF:FF:FF: flood to ALL ports  (BROADCAST FLOOD)

3. Entries expire after ~300 seconds if unused  (AGING)
```

---

## VLANs — Virtual Local Area Networks ⭐⭐⭐⭐

**Problem without VLANs:** All devices on a switch share one broadcast domain. Finance sees HR's traffic. ARP broadcasts slow down everyone. Security boundary is non-existent.

**Solution:** VLANs create logical isolation on the same physical switch.

```
┌────────────────────────────────────────┐
│          Single Physical Switch         │
│                                        │
│  VLAN 10 (Finance)  — Ports 1,2,3,4    │
│  VLAN 20 (HR)       — Ports 5,6,7,8    │
│  VLAN 30 (IT)       — Ports 9,10,11,12 │
│                                        │
│  Finance can NOT reach HR at Layer 2   │
│  A router is needed for inter-VLAN     │
└────────────────────────────────────────┘
```

**Access Port:** Single VLAN, connects to end devices (PCs, printers).
**Trunk Port:** Carries multiple VLANs between switches or to a router. Uses **802.1Q** tagging.

**Inter-VLAN Routing:** Traffic between VLANs MUST go through a router (or Layer 3 switch). A router-on-a-stick uses one physical interface with sub-interfaces per VLAN.

---

## Routing — Static vs Dynamic ⭐⭐⭐⭐

| Feature | Static Routing | Dynamic Routing (OSPF, RIP) |
|---------|---------------|----------------------------|
| Configured By | Admin manually | Routers automatically via protocol |
| Adapts to failures? | ❌ No | ✅ Yes |
| Overhead | None | Protocol traffic |
| Security | ✅ More secure | Risk of protocol exploitation |
| Use Case | Small/simple networks | Large/complex networks |

**Default Route:** `0.0.0.0/0` — "If I don't have a specific route, send it here." This is the "gateway of last resort" — points to the internet.

**Longest Prefix Match:** When multiple routes match a destination, the router picks the most specific (longest prefix length wins).

```
Routes: 10.0.0.0/8 and 10.5.0.0/16 and 10.5.10.0/24
Packet to 10.5.10.50:
→ All three match
→ /24 wins (most specific — longest prefix)
```

---

## Key Routing Protocols ⭐⭐⭐

| Protocol | Type | Metric | Max Hops | Use Case |
|----------|------|--------|----------|---------|
| **RIP** | Distance Vector | Hop count | 15 | Small, simple — mostly legacy |
| **OSPF** | Link State | Cost (bandwidth) | None | Enterprise standard |
| **BGP** | Path Vector | Policy-based | None | Internet between ISPs |

**Administrative Distance (AD):** When multiple protocols offer routes to the same destination, lower AD wins.
```
Connected = 0   (most trusted)
Static    = 1
EIGRP     = 90
OSPF      = 110
RIP       = 120  (least trusted of the common ones)
```

---
---

# Section 8: Network Security 🔒

## Common Attacks ⭐⭐⭐⭐⭐

### DoS vs DDoS
**DoS:** Single attacker overwhelms a target with traffic/requests, making it unavailable.
**DDoS:** Distributed — thousands of compromised machines (botnet) attack simultaneously.
**Defense:** Rate limiting, Cloudflare/CDN, ISP-level traffic scrubbing, AWS Shield.

### Man-in-the-Middle (MitM) ⭐⭐⭐⭐⭐
```
Normal: Client ──────────────────────────► Server
MitM:   Client ──► [Attacker intercepts] ──► Server
```
**Methods:** ARP Spoofing, DNS Spoofing, Rogue Wi-Fi hotspot ("Free Airport WiFi").
**Defense:** HTTPS/TLS everywhere, VPN, HSTS, certificate pinning.

### ARP Spoofing
Attacker sends fake ARP replies → their MAC linked to the gateway's IP → all traffic flows through attacker.
**Defense:** Dynamic ARP Inspection (DAI) on switches, use encrypted protocols.

### DNS Spoofing / Cache Poisoning
False DNS records injected into resolver cache → users redirected to fake/malicious sites.
**Defense:** DNSSEC (signed DNS records), DNS over HTTPS (DoH), DNS over TLS (DoT).

### Port Scanning
Using Nmap to probe for open ports and running services — reconnaissance before attack.
**Defense:** Firewall (close unused ports), IDS/IPS, network segmentation.

### Packet Sniffing
Capturing unencrypted traffic with Wireshark or tcpdump.
**Defense:** Encryption (HTTPS, SSH, VPN) — sniffing encrypted traffic reveals nothing useful.

---

## Security Mechanisms ⭐⭐⭐⭐

### Firewall Types

| Type | How it Works | Capability |
|------|-------------|-----------|
| Packet Filter | Checks IP/port headers per packet | Simple but no connection awareness |
| Stateful | Tracks connection state table | Knows if packet belongs to established connection |
| NGFW (Next-Gen) | Deep packet inspection + IPS + app awareness | Most powerful — inspects content |

### VPN ⭐⭐⭐⭐
```
Your Device ──[Encrypted Tunnel]──► VPN Server ──► Internet
All traffic encrypted between you and VPN server
Your real IP hidden from destination
```
**Protocols:** IPsec, OpenVPN, WireGuard, SSL VPN.
**Use cases:** Remote work (access corporate network), privacy on public Wi-Fi, geo-bypass.

### IDS vs IPS ⭐⭐⭐

| | IDS | IPS |
|-|-----|-----|
| Action | Detect + Alert only | Detect + Block automatically |
| Placement | Out-of-band (traffic mirror) | Inline (in the traffic path) |
| Risk | May miss attacks | May block legitimate traffic |

### Encryption Summary ⭐⭐⭐⭐

| Type | How | Example | Speed | Use |
|------|-----|---------|-------|-----|
| Symmetric | Same key encrypts + decrypts | AES-256 | Fast | Bulk data encryption |
| Asymmetric | Public key encrypts, private key decrypts | RSA | Slow | Key exchange, auth |
| Hybrid | Asymmetric for key exchange → Symmetric for data | TLS | Fast + Secure | HTTPS |

**Why hybrid?** Asymmetric is too slow for bulk data. TLS uses RSA/ECC to securely exchange an AES key, then uses AES for everything else.

---
---

# Section 9: 50 Most Asked Interview Questions ❓

## OSI & Network Models (Q1–Q7)

---

**Q1. What is the OSI model? Name all 7 layers.** ⭐⭐⭐⭐⭐

The OSI model is a 7-layer conceptual framework developed by ISO to standardize network communication:

| Layer | Name | Key Protocols |
|-------|------|--------------|
| 7 | Application | HTTP, DNS, FTP, SMTP, SSH |
| 6 | Presentation | SSL/TLS, JPEG, MPEG |
| 5 | Session | NetBIOS, RPC |
| 4 | Transport | TCP, UDP |
| 3 | Network | IP, ICMP, OSPF |
| 2 | Data Link | Ethernet, Wi-Fi |
| 1 | Physical | Cables, radio waves |

*Mnemonic (top→bottom): "All People Seem To Need Data Processing"*

---

**Q2. What is the difference between OSI and TCP/IP models?** ⭐⭐⭐⭐⭐

OSI is a 7-layer theoretical reference model used for understanding and troubleshooting networks — developed by ISO in 1984. TCP/IP is a 4-layer practical model that the actual internet runs on — developed by DARPA in the 1970s. OSI is protocol-independent; TCP/IP specifically implements TCP and IP. When troubleshooting or explaining where something operates, we use OSI terminology.

---

**Q3. At which OSI layer does a router operate? What about a switch?** ⭐⭐⭐⭐⭐

A router operates at **Layer 3 (Network)** — it makes forwarding decisions based on IP addresses and maintains a routing table. A switch operates at **Layer 2 (Data Link)** — it forwards frames based on MAC addresses and maintains a MAC address table. A hub operates at **Layer 1** — it simply repeats all signals to all ports with no intelligence.

---

**Q4. What is encapsulation in networking?** ⭐⭐⭐⭐

Encapsulation is the process of adding headers (and sometimes trailers) at each OSI layer as data travels down from Application to Physical on the sender's side. Transport adds port numbers → Network adds IP addresses → Data Link adds MAC addresses and CRC. At the receiver, each layer strips its header as data travels up (decapsulation). The data unit changes name: Data → Segment → Packet → Frame → Bits.

---

**Q5. What is the difference between a MAC address and an IP address?** ⭐⭐⭐⭐⭐

MAC address is a **48-bit hardware address** at Layer 2 — burned into the NIC by the manufacturer, permanent, used only for local network delivery, and changes at every router hop. IP address is a **32-bit logical address** at Layer 3 — assigned by DHCP or manually configured, can change, used for global routing, and remains the same from source to destination. MAC is "who you are on this floor of the building." IP is "your full mailing address."

---

**Q6. What is the purpose of the TTL field in an IP packet?** ⭐⭐⭐⭐

TTL (Time to Live) prevents packets from looping forever in the network. Each router decrements TTL by 1 when forwarding a packet. When TTL reaches 0, the router discards the packet and sends an ICMP "Time Exceeded" message back to the source. Default TTL values: Windows = 128, Linux/Mac = 64, Cisco = 255. Traceroute uses TTL by sending packets with incrementally increasing TTL to discover each hop.

---

**Q7. What is ICMP and what is it used for?** ⭐⭐⭐⭐

ICMP (Internet Control Message Protocol) is a Layer 3 protocol used for network diagnostics and error reporting. The `ping` command uses ICMP Echo Request (Type 8) and Echo Reply (Type 0) to test connectivity and measure round-trip time. `traceroute`/`tracert` uses ICMP TTL Exceeded messages (Type 11) to discover the path. ICMP carries no user data — it is a control and diagnostic protocol only.

---

## TCP, UDP, and Transport (Q8–Q17)

---

**Q8. What is the difference between TCP and UDP?** ⭐⭐⭐⭐⭐

TCP is connection-oriented, reliable, ordered, and has flow/congestion control — used for HTTP, HTTPS, FTP, SSH, and email where data integrity matters. UDP is connectionless, unreliable, fast, with minimal overhead — used for DNS, DHCP, VoIP, video streaming, and gaming where speed matters more than perfect delivery. TCP has a 3-way handshake; UDP simply sends datagrams.

---

**Q9. Explain the TCP Three-Way Handshake.** ⭐⭐⭐⭐⭐

Three steps:
1. **SYN** — Client sends SYN with its Initial Sequence Number (ISN). "I want to connect. My sequence starts at X."
2. **SYN-ACK** — Server acknowledges (ACK = X+1) and sends its own ISN. "Got X. My sequence starts at Y."
3. **ACK** — Client acknowledges (ACK = Y+1). "Got Y. Connection established."

Both sides agree on sequence numbers before data flows. This ensures reliable, ordered communication.

---

**Q10. Why does TCP use a 3-way handshake and not a 2-way?** ⭐⭐⭐⭐

Both sides need to exchange AND acknowledge their Initial Sequence Numbers independently. A 2-way exchange (SYN → SYN-ACK) would let the server acknowledge the client's ISN and send its own, but the client never confirms it received the server's ISN. The third message (ACK) completes the mutual acknowledgment. Without it, the server doesn't know if the client is ready to receive.

---

**Q11. What is TCP flow control? What is the window size?** ⭐⭐⭐

TCP flow control prevents a fast sender from overwhelming a slow receiver. The receiver advertises a "window size" — the maximum number of bytes it can buffer at a time. The sender cannot transmit more unacknowledged data than this window size. If the receiver's buffer fills up, it advertises a window of 0, and the sender must pause.

---

**Q12. What is TCP congestion control?** ⭐⭐⭐

TCP detects network congestion through packet loss (timeout or duplicate ACKs) and reduces its sending rate. Key mechanisms: **Slow Start** (begins with a small window, doubles each RTT), **Congestion Avoidance** (grows linearly once threshold is reached), **Fast Retransmit** (retransmit on 3 duplicate ACKs without waiting for timeout), **Fast Recovery** (resume from half of congestion window after loss).

---

**Q13. What are well-known port numbers for HTTP, HTTPS, SSH, DNS, DHCP?** ⭐⭐⭐⭐⭐

HTTP = 80, HTTPS = 443, SSH = 22, FTP = 21, SMTP = 25, DNS = 53, DHCP = 67/68, Telnet = 23, IMAP = 143, POP3 = 110, RDP = 3389, SNMP = 161/162. These are must-memorize for any technical interview.

---

**Q14. What is a socket in networking?** ⭐⭐⭐

A socket is the combination of an IP address and a port number that uniquely identifies a specific application on a specific host. Format: `IP:Port` → `192.168.1.5:443`. A TCP connection is identified by a 4-tuple: {source IP, source port, destination IP, destination port}. This is how the OS knows which application should receive each incoming packet.

---

**Q15. What happens during TCP connection termination?** ⭐⭐⭐⭐

TCP uses a 4-way close because each direction is closed independently:
1. FIN — initiating side signals "I'm done sending"
2. ACK — other side acknowledges
3. FIN — other side signals "I'm also done sending"
4. ACK — first side acknowledges, connection fully closed

After the final ACK, the initiating side enters TIME_WAIT state (2×MSL = ~4 minutes) to ensure the final ACK was received and no stale packets arrive for a new connection.

---

**Q16. What is a RST packet in TCP?** ⭐⭐⭐

A TCP RST (Reset) packet abruptly terminates a connection, unlike FIN which closes gracefully. RST is sent when: a packet arrives for a port with no listening process, a firewall forcibly closes a connection, or there is a protocol violation. If you receive "Connection reset by peer," a RST was sent. A FIN closes politely; RST slams the door.

---

**Q17. Why would you use UDP for video streaming instead of TCP?** ⭐⭐⭐⭐

In live video streaming, a packet received 500ms late is useless — the stream has moved on. TCP would detect the lost packet, retransmit it, and hold all subsequent packets until the retransmission arrives — causing buffering and stuttering. UDP simply drops the late packet and continues. A slightly degraded frame is far better than the entire stream freezing. Applications like YouTube Live and Zoom build their own lightweight reliability on top of UDP.

---

## IP Addressing & Subnetting (Q18–Q27)

---

**Q18. What is subnetting and why do we use it?** ⭐⭐⭐⭐⭐

Subnetting divides a large IP network into smaller sub-networks. We use it to: reduce broadcast traffic (broadcasts only reach devices in the same subnet), improve security (departments can be isolated — Finance can't directly communicate with Guest Wi-Fi), and use address space efficiently (assign only as many addresses as needed for each segment).

---

**Q19. What is CIDR notation?** ⭐⭐⭐⭐⭐

CIDR (Classless Inter-Domain Routing) expresses an IP address and subnet mask together using a slash and prefix length. The prefix length indicates how many bits are the network portion. Example: `192.168.1.0/24` means 24 network bits and 8 host bits — giving 254 usable hosts. `/26` means 26 network bits, 6 host bits — giving 62 usable hosts. CIDR replaced the old classful system which wasted enormous amounts of address space.

---

**Q20. How many usable hosts are in a /26 subnet?** ⭐⭐⭐⭐⭐

A /26 subnet has 2^(32-26) = 2^6 = 64 total addresses. Subtract 2 (network address + broadcast address) = **62 usable hosts**. The block size = 256 - 192 = 64. Subnets: .0, .64, .128, .192.

---

**Q21. What is the difference between network address and broadcast address?** ⭐⭐⭐⭐

The network address is the first address in a subnet — all host bits are 0. It identifies the subnet itself and cannot be assigned to a device. The broadcast address is the last address — all host bits are 1. Packets sent to the broadcast address are received by all devices in the subnet. Both are reserved and cannot be assigned to hosts. For `192.168.1.0/24`: network = 192.168.1.0, broadcast = 192.168.1.255, usable = .1 to .254.

---

**Q22. What are private IP addresses? Why do they exist?** ⭐⭐⭐⭐⭐

Private IP addresses (RFC 1918) are ranges reserved for internal networks — 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16. They are NOT routable on the public internet. They exist to conserve the limited IPv4 address space — millions of home and office networks all use 192.168.1.x internally without conflicting with each other. NAT at the router translates private → public when accessing the internet.

---

**Q23. What is NAT? How does it work?** ⭐⭐⭐⭐⭐

NAT (Network Address Translation) translates private IP addresses to a public IP for internet access. When your device (192.168.1.10) sends a packet to the internet, the router replaces the source IP with its public IP and records the mapping (192.168.1.10:54321 ↔ public_IP:54321) in a NAT table. When the response comes back to public_IP:54321, the router looks up its table and delivers it to 192.168.1.10:54321. PAT (Port Address Translation) extends this so multiple private IPs share one public IP using different port numbers.

---

**Q24. What is the loopback address?** ⭐⭐⭐⭐

127.0.0.1 (::1 in IPv6) is the loopback address — any traffic sent to it is delivered back to the same machine without going onto the network. Used to test if the local TCP/IP stack is working, test local server applications during development ("ping 127.0.0.1" should always succeed regardless of network status), and reference "this machine" in configuration files.

---

**Q25. What does 169.254.x.x mean on a Windows machine?** ⭐⭐⭐⭐

169.254.x.x is an APIPA (Automatic Private IP Addressing) address. Windows automatically assigns itself an address in this range when it cannot reach a DHCP server. It means: the device has no valid IP configuration, has no default gateway, and cannot access the internet. It is a diagnostic indicator — check the network cable, Wi-Fi connection, or DHCP server.

---

**Q26. What is the default gateway?** ⭐⭐⭐⭐⭐

The default gateway is the IP address of the router on your local network. When a device wants to send traffic to a destination NOT on its local subnet, it sends the packet to the default gateway, which routes it further toward the destination. Without a default gateway, a device can only communicate within its own subnet.

---

**Q27. What is the subnet mask for a Class C network?** ⭐⭐⭐⭐

255.255.255.0 (or /24). This means the first 24 bits are the network portion and the last 8 bits are the host portion — giving 256 addresses, 254 usable hosts per network. Class A default mask is 255.0.0.0 (/8). Class B is 255.255.0.0 (/16).

---

## Application Protocols (Q28–Q37)

---

**Q28. What is DNS? How does it resolve a domain name?** ⭐⭐⭐⭐⭐

DNS (Domain Name System) translates domain names to IP addresses. Resolution: Browser checks local cache → OS checks hosts file → query sent to Recursive Resolver (8.8.8.8) → resolver checks cache → if miss, asks Root Server → Root points to .com TLD server → TLD points to domain's authoritative nameserver → auth NS returns IP → resolver caches and returns to browser. Entire process takes ~50-100ms. Cached responses take < 1ms.

---

**Q29. What is the difference between an A record and a CNAME record?** ⭐⭐⭐⭐

An **A record** maps a domain directly to an IPv4 address (google.com → 142.250.195.78). A **CNAME (Canonical Name)** record maps a domain to another domain name — an alias (www.example.com → example.com). The resolver follows the CNAME and then resolves the target. CNAME cannot be used at the zone apex (root of a domain).

---

**Q30. What is DHCP? Explain the DORA process.** ⭐⭐⭐⭐⭐

DHCP automatically assigns IP configuration to devices. DORA: **Discover** (client broadcasts "I need an IP"), **Offer** (server proposes IP address + config), **Request** (client broadcasts acceptance of the offer), **Acknowledge** (server confirms the lease). DHCP also provides subnet mask, default gateway, DNS servers, and lease duration.

---

**Q31. What is ARP? What is ARP Spoofing?** ⭐⭐⭐⭐

ARP resolves IP addresses to MAC addresses. When a device needs to send a frame to an IP on the local network, it broadcasts "Who has IP X?" — the device with that IP replies with its MAC address. The result is cached in the ARP table. ARP Spoofing is an attack where a malicious device sends fake ARP replies, associating its MAC with a legitimate IP (like the gateway), causing all traffic to flow through the attacker — enabling Man-in-the-Middle attacks.

---

**Q32. What is the difference between HTTP and HTTPS?** ⭐⭐⭐⭐⭐

HTTP (port 80) transmits data in plaintext — anyone intercepting the traffic can read everything including credentials and form data. HTTPS (port 443) uses TLS to encrypt all communication, providing: Confidentiality (data is unreadable), Integrity (data cannot be modified in transit), and Authentication (certificate proves server identity). HTTPS should be used for all websites, especially those handling any sensitive data.

---

**Q33. What HTTP status code means "Not Found"? What about "Server Error"?** ⭐⭐⭐⭐⭐

**404 Not Found** — the requested resource doesn't exist on the server.
**500 Internal Server Error** — generic server-side error (something broke on the server).
Also commonly asked: 200 (OK), 201 (Created), 301 (Moved Permanently), 403 (Forbidden), 401 (Unauthorized), 429 (Too Many Requests), 503 (Service Unavailable).

---

**Q34. What is the difference between SMTP, POP3, and IMAP?** ⭐⭐⭐

SMTP (port 25/587) sends email — from client to server and between servers. POP3 (port 110) retrieves email by downloading it to the device and usually deleting it from the server — works for single-device access. IMAP (port 143) keeps email on the server and syncs across all devices — used by all modern email services. SMTP sends; POP3 downloads (old); IMAP syncs (current standard).

---

**Q35. Why should you use SSH instead of Telnet?** ⭐⭐⭐⭐

Telnet transmits everything — including usernames, passwords, and all commands — in plaintext. Anyone on the network can capture and read it using a simple packet sniffer like Wireshark. SSH encrypts the entire session using strong cryptography. There is no valid reason to use Telnet in any modern environment. Even for lab testing, SSH should be the default.

---

**Q36. What is the difference between FTP and SFTP?** ⭐⭐⭐

FTP (File Transfer Protocol, port 21) transmits data including credentials in plaintext — completely insecure. SFTP (SSH FTP, port 22) runs over SSH and encrypts everything. FTPS adds TLS to FTP (port 990). In practice, SFTP is the standard for secure file transfer. FTP should never be used for anything requiring any level of security.

---

**Q37. What is HTTP/2 and how is it different from HTTP/1.1?** ⭐⭐⭐

HTTP/1.1 sends one request at a time per connection (sequential) and uses text-based format. HTTP/2 uses **multiplexing** — multiple requests and responses simultaneously over one TCP connection — eliminating the head-of-line blocking problem of HTTP/1.1. HTTP/2 also uses **binary format** (faster parsing), **header compression** (HPACK), and allows **server push** (proactively send resources). HTTP/3 goes further by using QUIC (UDP-based) instead of TCP.

---

## Routing, Switching, Security (Q38–Q50)

---

**Q38. What is the difference between a switch and a router?** ⭐⭐⭐⭐⭐

A **switch** operates at Layer 2 and connects devices within the **same** IP network — it forwards frames based on MAC addresses. A **router** operates at Layer 3 and connects **different** IP networks — it forwards packets based on IP addresses using a routing table. You need a router to move traffic between 192.168.1.0/24 and 192.168.2.0/24. A switch alone cannot do this.

---

**Q39. What is a VLAN? Why is it used?** ⭐⭐⭐⭐

A VLAN (Virtual LAN) is a logical network segment created within a physical switch. It isolates devices into separate broadcast domains without requiring separate physical hardware. Benefits: security (Finance and HR traffic isolated), reduced broadcasts (smaller broadcast domains), and logical grouping by function rather than physical location. Communication between VLANs requires a router or Layer 3 switch.

---

**Q40. What is a routing table?** ⭐⭐⭐⭐

A routing table is a database in a router listing known networks and how to reach them — the destination network, the next-hop router address, the outgoing interface, the routing protocol that learned this route, and the metric. When a packet arrives, the router performs a **longest prefix match** — finds the most specific matching route and forwards accordingly. The default route (0.0.0.0/0) catches all packets with no more specific match.

---

**Q41. What is OSPF?** ⭐⭐⭐

OSPF (Open Shortest Path First) is a link-state interior routing protocol. Routers exchange LSAs (Link State Advertisements) to build a complete network topology map (LSDB). Each router runs Dijkstra's SPF algorithm on its map to calculate shortest paths. OSPF uses cost (based on bandwidth) as its metric, has no hop-count limit, converges in seconds, and supports VLSM. It is the standard IGP for enterprise networks.

---

**Q42. What is BGP and why is it called the routing protocol of the internet?** ⭐⭐⭐

BGP (Border Gateway Protocol) routes traffic between Autonomous Systems (ISPs, large companies). Every ISP runs BGP to exchange routing information — what prefixes they can reach — with neighboring ISPs. BGP makes routing decisions based on policy (AS path, communities, local preference) rather than metrics like hop count. The global BGP routing table contains 900,000+ IPv4 routes. Without BGP, cross-ISP internet routing would be impossible.

---

**Q43. What is a firewall? What types exist?** ⭐⭐⭐⭐

A firewall filters network traffic based on rules. Types: **Packet Filter** (stateless — checks IP/port headers), **Stateful Firewall** (tracks connection state — knows if a packet belongs to an established connection), **Application Layer / NGFW** (inspects actual content — can block specific apps, has integrated IPS). In general, you want a stateful firewall at minimum; NGFWs for enterprise environments.

---

**Q44. What is a VPN? How does it work?** ⭐⭐⭐⭐

A VPN creates an encrypted tunnel between a client and a VPN server. All traffic is encrypted before leaving the client's device, decrypted at the VPN server, then sent to the destination. The destination sees the VPN server's IP, not the client's. Uses: secure remote work (access corporate resources), privacy on public Wi-Fi, bypassing geographic restrictions. Common protocols: IPsec, OpenVPN, WireGuard.

---

**Q45. What is a DoS vs DDoS attack?** ⭐⭐⭐⭐

DoS (Denial of Service) uses a single attacker to flood a target with traffic or exploit a vulnerability, making it unavailable to legitimate users. DDoS (Distributed DoS) uses thousands or millions of compromised devices (a botnet) simultaneously — making it impossible to simply block one source. DDoS attacks can exhaust bandwidth, CPU, or connection-handling capacity. Defenses include CDNs, rate limiting, traffic scrubbing, and anycast routing.

---

**Q46. What is SSL/TLS? What does TLS provide?** ⭐⭐⭐⭐⭐

TLS (Transport Layer Security) is a cryptographic protocol securing communication over networks. It provides:
1. **Confidentiality** — AES encryption makes traffic unreadable
2. **Integrity** — HMAC ensures data wasn't modified in transit
3. **Authentication** — digital certificate (signed by CA) verifies server identity

HTTPS uses TLS. The TLS handshake uses asymmetric encryption (RSA/ECC) to securely exchange a symmetric session key, then uses that symmetric key (AES) for all data — fast and secure.

---

**Q47. What is a Man-in-the-Middle attack?** ⭐⭐⭐⭐⭐

A MitM attack occurs when an attacker intercepts communication between two parties without either knowing. The attacker can read, modify, or inject messages. Common methods: ARP Spoofing (associate attacker's MAC with gateway IP), DNS Spoofing (redirect domain to attacker's IP), rogue Wi-Fi hotspot (victim connects to attacker's AP). Defense: HTTPS/TLS (encryption makes interception useless), VPN, HSTS, DNSSEC.

---

**Q48. What is the difference between IDS and IPS?** ⭐⭐⭐

An IDS (Intrusion Detection System) monitors network traffic for suspicious patterns and generates alerts but takes no action. An IPS (Intrusion Prevention System) monitors traffic and automatically blocks detected threats inline. IDS is passive (out-of-band — monitors a copy of traffic); IPS is active (inline — sits in the traffic path). IPS carries risk of false positives blocking legitimate traffic; IDS only misses attacks silently.

---

**Q49. What is the difference between unicast, broadcast, and multicast?** ⭐⭐⭐⭐

**Unicast:** One sender → one specific receiver (most internet traffic — your request to Google).
**Broadcast:** One sender → ALL devices on the local network (ARP requests, DHCP Discover). Only at Layer 2 — routers block broadcasts.
**Multicast:** One sender → multiple specific receivers who "subscribed" to a group (OSPF routing updates, video streaming to multiple clients). More efficient than multiple unicasts or broadcast.
IPv6 eliminates broadcast entirely — uses multicast and anycast instead.

---

**Q50. What happens step by step when you type "www.google.com" in your browser?** ⭐⭐⭐⭐⭐

1. **DNS Resolution** — Browser cache → OS hosts file → Recursive Resolver → Root → .com TLD → Google's NS → returns 142.250.x.x
2. **ARP** — Needs MAC of default gateway → ARP broadcast → router replies → frame can now be sent
3. **TCP 3-way Handshake** — SYN → SYN-ACK → ACK on port 443
4. **TLS Handshake** — Certificate verified → session key exchanged → encrypted channel established
5. **HTTP GET Request** — `GET / HTTP/2` sent (encrypted via TLS)
6. **Routing** — Packet traverses your LAN → router (NAT: private → public IP) → ISP → backbone routers (BGP) → Google's network
7. **Response** — Google's server returns `200 OK` with HTML/CSS/JS (encrypted)
8. **Rendering** — Browser decrypts, parses, and renders the page
9. **Connection Close** — FIN → ACK → FIN → ACK

*"If you can explain this completely with the right terms, you will impress any interviewer."*

---
---

# Section 10: Real-World Scenarios 🌍

## "Why is my internet slow even though Wi-Fi shows full bars?" ⭐⭐⭐⭐

Full bars = strong signal at **Layer 1/2 (Physical/Wi-Fi)**. Slow internet could be anywhere above that:
- ISP is throttling your connection (Layer 3+)
- Router is overloaded (many devices, old hardware)
- 2.4 GHz is congested (too many neighbors on same channel)
- DNS server is slow (try 1.1.1.1 or 8.8.8.8)
- The server you're accessing is far away or slow
- High latency despite good bandwidth (a 1 Gbps link with 500ms RTT is worse for video calls than 10 Mbps with 10ms RTT)

**Key insight:** Bandwidth ≠ Latency. Full Wi-Fi bars only confirms Layer 1-2 are fine.

---

## "Why does DHCP fail and what are the symptoms?" ⭐⭐⭐⭐

**Symptoms:** Device shows 169.254.x.x (APIPA) → no default gateway → no internet → can only talk to other 169.254.x.x devices on the same segment.

**Causes:** DHCP server is down, cable unplugged between device and switch, VLAN misconfiguration (device in VLAN with no DHCP scope), DHCP pool exhausted (all IPs in use), firewall blocking UDP 67/68.

**Diagnostic steps:** `ipconfig /release` → `ipconfig /renew` → check if 169.254 or real IP. If 169.254, it's a DHCP failure.

---

## "Why do you need a router if you already have a switch?" ⭐⭐⭐⭐⭐

A switch connects all devices within the same IP network (e.g., 192.168.1.0/24). They can all talk to each other using their MAC addresses. But to reach ANY other network — the internet (8.8.8.8), another department (10.0.0.x), or another office — you need a device that understands IP addresses and knows how to route between networks. That is a router.

*"A switch is the roads inside your city. A router is the highway that connects cities."*

---

## "What is the difference between HTTP and HTTPS in practice?" ⭐⭐⭐⭐⭐

On HTTP, if you are connected to a coffee shop Wi-Fi and submit a login form, the attacker running a packet sniffer on the same network can read your username and password in plaintext from the captured traffic. On HTTPS, even if the attacker captures every packet, they see only encrypted garbage — the session key was never transmitted in the clear. This is why every website handling any credentials must use HTTPS.

---

## "A user says the internet is working but they can't access a specific website." ⭐⭐⭐⭐

Systematic troubleshooting:
1. Can you ping the website's IP directly? (`nslookup website.com` → get IP → `ping IP`)
   - If ping works but URL fails → likely a browser or HTTPS issue
2. Can other users access it? → If yes, may be local DNS or firewall issue
3. Is DNS resolving correctly? (`nslookup website.com`) → Different IP than expected → DNS spoofing or wrong DNS server
4. Is port 443 accessible? (`telnet website.com 443`) → Connection refused → firewall blocking
5. Is there a proxy configured that's blocking? Check browser/system proxy settings
6. Is the site down globally? Check downdetector.com

---

## "What happens when the DHCP server is down but devices are already connected?" ⭐⭐⭐

Devices already connected: they keep using their current IP address until the lease expires (typically 24 hours to 7 days). At 50% of lease time, they try to renew (unicast to DHCP server) — if server is still down, they try again at 87.5%. If the lease expires and DHCP is still down, they fall back to APIPA (169.254.x.x) and lose internet access.

New devices joining during the outage: they immediately get APIPA since DHCP is unavailable — no internet access from the moment they join.

---
---

# Section 11: Commands Cheat Sheet 💻

## Windows Commands

```cmd
:: ── Network Information ──────────────────────────────────────
ipconfig                    Basic: IP, mask, gateway per interface
ipconfig /all               Full info: MAC, DHCP server, DNS, lease dates
ipconfig /release           Release current DHCP lease (now has no IP)
ipconfig /renew             Request new DHCP lease (triggers DORA)
ipconfig /flushdns          Clear local DNS resolver cache
ipconfig /displaydns        Show current DNS cache contents

:: ── Connectivity Testing ──────────────────────────────────────
ping 8.8.8.8                Test connectivity to Google DNS by IP
ping -t 8.8.8.8             Continuous ping until Ctrl+C
ping google.com             Test connectivity + DNS resolution together
ping -n 10 8.8.8.8          Ping exactly 10 times
ping 127.0.0.1              Test local TCP/IP stack (always works)
ping <gateway>              Test if you can reach your router

:: ── Path Analysis ─────────────────────────────────────────────
tracert google.com          Trace route — show every hop with latency
tracert -d google.com       Same but no DNS resolution (faster)
pathping google.com         Combines ping + tracert — packet loss per hop

:: ── DNS ────────────────────────────────────────────────────────
nslookup google.com              Basic A record lookup
nslookup -type=MX gmail.com      Look up mail servers
nslookup -type=NS google.com     Look up name servers
nslookup -type=TXT google.com    Look up TXT records
nslookup google.com 1.1.1.1      Query using specific DNS server (1.1.1.1)

:: ── ARP ────────────────────────────────────────────────────────
arp -a                      Show ARP table (IP to MAC mappings)
arp -d *                    Clear all ARP entries (requires admin)

:: ── Connections ────────────────────────────────────────────────
netstat -an                 All active connections + listening ports
netstat -b                  Show which program owns each connection (admin)
netstat -r                  Show routing table (same as route print)
route print                 Show full Windows routing table
```

## Linux / Mac Commands

```bash
# ── Network Information ─────────────────────────────────────────
ip addr show                Interface info (modern — replaces ifconfig)
ifconfig                    Interface info (older systems/Mac)
ip addr show eth0           Specific interface info
ip link show                Link layer info + status

# ── Routing ─────────────────────────────────────────────────────
ip route show               Routing table
ip route show default       Just the default gateway
route -n                    Routing table (older systems)

# ── Connectivity Testing ─────────────────────────────────────────
ping -c 4 8.8.8.8           Ping 4 times (Linux)
ping 8.8.8.8                Continuous ping on Linux (Ctrl+C to stop)
ping -c 4 google.com        Test DNS + connectivity
ping -c 1 127.0.0.1         Test loopback

# ── Path Analysis ───────────────────────────────────────────────
traceroute google.com       Trace route (Linux)
traceroute -n google.com    Without DNS resolution (faster)
mtr google.com              Real-time traceroute + packet loss (best tool)

# ── DNS ──────────────────────────────────────────────────────────
dig google.com              Full A record lookup with details
dig google.com +short       Just the IP address
dig MX gmail.com            Mail server records
dig NS google.com           Name server records
dig google.com @1.1.1.1     Query specific DNS server
dig google.com +trace       Full resolution trace from root servers
nslookup google.com         Basic lookup (works on Linux/Mac too)

# ── ARP ──────────────────────────────────────────────────────────
arp -n                      Show ARP table
ip neigh show               ARP table (modern)
ip neigh flush all          Clear ARP table

# ── Active Connections ───────────────────────────────────────────
netstat -tuln               All listening TCP/UDP ports
ss -tuln                    Modern netstat (faster, more detail)
ss -tnp                     Connections with process names
ss -s                       Summary statistics

# ── Packet Capture ───────────────────────────────────────────────
tcpdump -i eth0             Capture all traffic on eth0
tcpdump -i eth0 port 80     Capture only HTTP traffic
tcpdump -i eth0 host 8.8.8.8  Capture traffic to/from 8.8.8.8
tcpdump -w capture.pcap     Save to file for Wireshark analysis

# ── Scanning (Nmap — install separately) ─────────────────────────
nmap -sn 192.168.1.0/24     Discover hosts on subnet (ping sweep)
nmap -sV 192.168.1.1        Scan open ports + service versions
nmap -p 80,443 192.168.1.1  Check specific ports only
```

## Useful One-Liners

```bash
# Find your public IP address
curl ifconfig.me
curl icanhazip.com

# Test if a specific port is open (Linux/Mac)
nc -zv google.com 443       # "Connection succeeded" or "refused"
telnet google.com 443        # Works on Windows too (if Telnet enabled)

# Check HTTP headers only (no body)
curl -I https://google.com

# Full verbose HTTPS connection (shows TLS details)
curl -v https://google.com 2>&1 | head -50

# Check DNS propagation with specific servers
dig google.com @8.8.8.8 +short
dig google.com @1.1.1.1 +short
dig google.com @208.67.222.222 +short  # OpenDNS

# Watch DNS lookups in real time
watch -n 2 "dig google.com +short"

# Continuous traceroute (Linux)
mtr --report google.com
```

## Wireshark Filters (Quick Reference)

```
dns                         Show only DNS traffic
tcp                         Show only TCP traffic
udp                         Show only UDP traffic
http                        Show only HTTP traffic
tcp.port == 443             Show only HTTPS traffic
ip.addr == 8.8.8.8          Traffic to/from 8.8.8.8
ip.src == 192.168.1.10      Traffic FROM this IP
ip.dst == 192.168.1.10      Traffic TO this IP
tcp.flags.syn == 1          Show all SYN packets (connection starts)
arp                         Show all ARP requests/replies
dhcp or bootp               Show DHCP traffic
icmp                        Show ping traffic
tcp.analysis.retransmission Show retransmitted packets (packet loss)
```

---
---

# Section 12: 2-Week Study Plan 📅

**Daily commitment: 2.5 hours**
→ Morning: 2 hours theory + practice
→ Evening: 30 min review + 5 subnetting problems

## Week 1 — Core Concepts

| Day | Topic | Goal by End of Day |
|-----|-------|--------------------|
| **Day 1** | OSI Model (Section 1) | Recite all 7 layers with protocols, data units, devices from memory |
| **Day 2** | TCP/IP Model + OSI vs TCP/IP (Section 2) | Draw both models and map OSI to TCP/IP without notes |
| **Day 3** | IP Addressing — classes, private ranges, special IPs (Section 3) | Name all 3 private ranges and 3 special addresses instantly |
| **Day 4** | Subnetting formula + quick reference table (Section 3) | Solve 10 subnetting problems correctly using the formula |
| **Day 5** | TCP — 3-way handshake, flags, flow control (Section 4) | Draw the TCP handshake from memory with sequence numbers |
| **Day 6** | UDP + Port numbers (Section 4) | Explain TCP vs UDP differences and recall 10 port numbers |
| **Day 7** | DNS + DHCP + ARP (Section 5) | Trace DNS resolution and DORA end-to-end without notes |

## Week 2 — Protocols, Security, Practice

| Day | Topic | Goal by End of Day |
|-----|-------|--------------------|
| **Day 8** | HTTP/HTTPS + Status Codes + TLS (Section 6) | State 8 status codes, explain what TLS provides (3 things) |
| **Day 9** | Routing + Switching + VLANs (Section 7) | Explain hub vs switch vs router with analogy |
| **Day 10** | Network Security — attacks + defenses (Section 8) | Name 5 attacks and their defenses |
| **Day 11** | Commands Cheat Sheet (Section 11) | Run every command in the sheet on your actual machine |
| **Day 12** | Interview Q&A 1–25 (Section 9) | Answer all 25 without looking at notes |
| **Day 13** | Interview Q&A 26–50 (Section 9) | Answer all 25 + practice Q50 (URL scenario) aloud |
| **Day 14** | Mock interview + full review | Answer Q50 in 2 minutes from memory — record yourself |

## Daily Practice (Every Day)
- ✅ Explain 2 concepts out loud without looking at notes
- ✅ Solve 5 subnetting problems (use Section 3 formula)
- ✅ Answer 5 interview questions cold
- ✅ Run at least 3 commands from the cheat sheet

---
---

# Section 13: Readiness Checklist ✅

## You Are Ready for Interviews When You Can:

### OSI Model
- [ ] Name all 7 layers with correct numbers, protocols, data units, and devices from memory
- [ ] Explain encapsulation: data → segment → packet → frame → bits
- [ ] State the ONE rule: MAC changes every hop, IP stays the same end-to-end
- [ ] Map OSI layers to TCP/IP model instantly

### IP Addressing
- [ ] Name all 3 private IP ranges from memory (10.x, 172.16-31.x, 192.168.x)
- [ ] Identify if an IP is private or public in under 5 seconds
- [ ] Convert /26 to 255.255.255.192 and back without help
- [ ] Given any IP + prefix, find network, broadcast, first/last host in under 60 seconds
- [ ] Subnet a /24 into 4 equal parts with correct ranges
- [ ] Know what 169.254.x.x means immediately (DHCP failed → APIPA)

### TCP & UDP
- [ ] Draw the TCP 3-way handshake with sequence numbers from memory
- [ ] Explain why TCP needs 3 steps (not 2)
- [ ] Recite TCP flags: SYN, ACK, FIN, RST, PSH, URG
- [ ] State 5 TCP use cases and 5 UDP use cases
- [ ] Recall port numbers for HTTP, HTTPS, SSH, FTP, DNS, DHCP, SMTP, IMAP, POP3

### Application Protocols
- [ ] Trace DNS resolution from browser → recursive resolver → root → TLD → authoritative → IP
- [ ] Explain DORA using the "client shouting, server responding" mental model
- [ ] State what HTTP status codes 200, 201, 301, 400, 401, 403, 404, 500, 503 mean
- [ ] Explain what HTTPS adds over HTTP (3 things: confidentiality, integrity, authentication)
- [ ] State why SSH replaced Telnet in one clear sentence

### Routing & Switching
- [ ] Explain hub vs switch vs router with a clear analogy
- [ ] Describe how a switch builds its MAC table (learning + forwarding + flooding)
- [ ] Explain what a VLAN does and why you need a router for inter-VLAN traffic
- [ ] Explain longest prefix match in routing

### Security
- [ ] Describe Man-in-the-Middle attack and 2 defenses
- [ ] Explain what TLS provides (3 properties)
- [ ] Describe how a VPN works in 3 sentences
- [ ] Name 3 network attacks and their defenses

### The Scenario Question
- [ ] Answer "What happens when you type google.com" covering: DNS, ARP, TCP, TLS, HTTP, routing, NAT — in under 2 minutes

---

## 🔥 Last-Day Rapid Review — Memorize This Block

```
OSI LAYERS (7→1):   Application | Presentation | Session | Transport | Network | DataLink | Physical
DATA UNITS:         Message     | Data         | Data    | Segment   | Packet  | Frame    | Bit
DEVICES:            Gateway     | —            | —       | Firewall  | Router  | Switch   | Hub

TCP/IP LAYERS (4→1): Application | Transport | Internet | Network Access

TCP = Reliable, Connection-Oriented, Ordered  |  UDP = Fast, Connectionless, No Guarantee
TCP handshake: SYN → SYN-ACK → ACK           |  TCP close: FIN → ACK → FIN → ACK

PORTS TO MEMORIZE:
HTTP=80   HTTPS=443   SSH=22    FTP=21    TELNET=23
SMTP=25   POP3=110    IMAP=143  DNS=53    DHCP=67/68
RDP=3389  SNMP=161    SMTP-submit=587

PRIVATE IPs:   10.x.x.x  |  172.16-31.x.x  |  192.168.x.x
SPECIAL:       127.0.0.1 = loopback  |  169.254.x.x = APIPA (DHCP failed!)

SUBNETTING:
/24 = 254 hosts  |  /25 = 126  |  /26 = 62  |  /27 = 30  |  /28 = 14  |  /29 = 6  |  /30 = 2
Block size = 256 − (mask value in interesting octet)

DHCP DORA:    Discover → Offer → Request → Acknowledge
DNS resolves: names → IPs  |  ARP resolves: IPs → MACs

Switch = MAC table (Layer 2)  |  Router = IP routing table (Layer 3)
MAC changes every hop         |  IP stays the same end-to-end

HTTP = port 80 plaintext  |  HTTPS = port 443 + TLS (encrypted)
TLS provides: Confidentiality + Integrity + Authentication

ATTACKS:       MitM | DDoS | ARP Spoofing | DNS Spoofing | Port Scan | Sniffing
DEFENSES:      HTTPS | VPN | DAI | DNSSEC | Firewall | Encryption

URL SCENARIO:  DNS → ARP → TCP handshake → TLS handshake → HTTP GET → route → response → render
```

---

## 📝 Next Steps

**Today:**
1. Read OSI Model section — recite all 7 layers by tonight without notes
2. Memorize the TCP 3-way handshake diagram
3. Memorize all 3 private IP ranges

**This Week:**
1. Complete Sections 1–8 (theory)
2. Run all commands in Section 11 on your actual machine
3. Answer first 25 interview questions out loud (not in your head — speak them)

**Every Day Until Interview:**
- Explain "What happens when you type google.com" — add more protocol detail each day
- Solve 5 subnetting problems with the formula — no calculator
- Review the Rapid Review block above

---

> **Navigation:** [← 01_CN_Masterguide.md](./01_CN_Masterguide.md) | [Back to README](./README.md) | [03_CN_Practice_Repository.md →](./03_CN_Practice_Repository.md)

---

*File: `02_CN_Interview_Prep.md` | Version 1.0 | 2026*
*Part of the Computer Networks Repository*
*Companion to the Operating Systems Interview Prep guide*
