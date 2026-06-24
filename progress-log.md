# Progress Log

A running record of completed work — courses, modules, labs, and milestones.
For deep-dive problem-solving writeups, see the [writeups](writeups/) folder.

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
