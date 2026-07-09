# Progress Log

A running record of completed work — courses, modules, labs, and milestones.
For deep-dive problem-solving writeups, see the [writeups](writeups/) folder.

---

### 2026-07-08 TryHackMe — Pre-Security path (COMPLETE) 

Finished the full Pre-Security path. Earlier modules are logged individually
above; this entry covers the remaining four and marks the path complete.

**Operating Systems Basics** — OS fundamentals across platforms, with hands-on
command line work in both Linux and Windows CLIs, plus an introduction to
operating system security concepts.

**Software Basics** — how computers represent and encode data, plus first
exposure to Python and JavaScript through simple demos, and the basics of
querying databases with SQL.

**How The Web Works** — DNS resolution in depth, the HTTP protocol and its
request/response structure, how websites are built and served, and tying it
together end-to-end.

**Attacks and Defenses** — the CIA triad (confidentiality, integrity,
availability) as the foundational security model, core cryptography concepts,
and an introduction to both the attacker's and defender's perspectives.

**Takeaway:** The path deliberately alternates offense and defense, and that
framing stuck with me — the same event looks completely different depending on
which side of it you're standing on. Coming out of it, the web and networking
material connected most directly to where I'm headed.

---

### 2026-02-08 - Study — ongoing
- **Moving onto Cyber Security 101 THM**
- **Linux Basics for Hackers by OTW** — resumed, through Chapter 4.
- **CompTIA A+ Core 2** — Section 1 complete (Operating Systems, Installing
  Operating Systems, Microsoft Windows, The Windows OS, The Windows Command Line,
  Windows Settings, Windows Networking, macOS, Linux, Installing Application,
  Cloud Producitivity).

---

### TryHackMe — Computer Fundamentals module (complete)

Completed the Computer Fundamentals module. Much of the hardware and OS
material was reinforcement of my A+ studies, but the virtualization and
cloud rooms connected directly to my cloud security goal.

**Rooms covered:** Inside a Computer, Computer Types, Client-Server,
Virtualization Basics, Cloud Computing Fundamentals.

**Key concepts:**
- **Boot process** — what happens at power-on: firmware → POST → select boot
  device → bootloader; UEFI holds the boot order.
- **Computer types** — desktops, laptops, workstations, servers, plus IoT and
  embedded devices, and what each is purpose-built for.
- **Client-server model** — how a client request travels (DNS, ports,
  protocols) to reach a server and return a response.
- **HTTP methods & inspection** — intro to request commands (focused on GET).
  In a VM, used browser inspection to break down a page's components — scheme,
  host, filename, full address, and response status — and monitored its live
  GET requests.
- **Virtualization** — hypervisors (Type 1 vs Type 2), containers, and why
  virtualization exists.
- **Cloud service models** — IaaS, PaaS, SaaS, and deployment models
  (public, private, hybrid). Used a VM to deploy a cloud instance.

**Takeaway:** The cloud and virtualization rooms were the most valuable here —
they're the foundation of where I'm headed with cloud security, so seeing the
service models and hypervisor types hands-on was a useful first exposure.

---

### TryHackMe — Network Fundamentals module (complete)

Completed the full Network Fundamentals module — a foundational deep-dive
that reinforced and extended my A+ networking knowledge.

**Rooms covered:** What is Networking?, Intro to LAN, OSI Model,
Packets & Frames, Extending Your Network.

**Key concepts:**
- **OSI model** — the 7 layers and what lives at each; using it to reason
  about where a problem or device belongs (switch = L2, router = L3).
- **Packets vs frames** — a packet (L3, IP addressing) gets wrapped inside
  a frame (L2, MAC addressing) as data moves down the stack.
- **ARP** — resolving a known IP to its MAC address, and why its lack of
  authentication makes ARP spoofing possible.
- **TCP three-way handshake** — SYN → SYN-ACK → ACK to establish a connection.
- **Firewalls** — stateful (tracks the whole connection) vs stateless
  (evaluates individual packets); operate at OSI layers 3 and 4.
- **VPN technologies** — PPP, PPTP, IPSec; port forwarding; LAN/VLAN basics.

**Takeaway:** The OSI model tied the whole module together — packets/frames,
firewalls, and ARP all made more sense once I could place them at a layer.

---

### TryHackMe — Introduction to Cyber Security module (complete)

Completed the 3-room intro module:

- **Offensive Security Intro** — hands-on with a basic web attack: found
  unlinked "hidden" pages via directory enumeration, then exploited weak
  access control to modify data I shouldn't have had access to.
- **Defensive Security Intro** — the blue-team mirror: used a SOC analyst
  dashboard to detect that same kind of directory enumeration attack,
  identified the malicious source IP, and blocked it.
- **Careers in Cyber** — surveyed four core roles: SOC analyst, penetration
  tester, forensic analyst, and security engineer.

**Takeaway:** Seeing the same attack (directory enumeration) from both the
attacker's and defender's side back-to-back made the concept stick — offense
and defense are two views of the same event.

---
