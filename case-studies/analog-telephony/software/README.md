# Software

This section documents the software environment used to implement the Analog Telephony Laboratory.

The laboratory uses a Linux-based PBX platform to generate and manage the analog telephone service used by students during practical activities. The same platform also supports SIP/VoIP endpoints used for functional verification of student-installed analog circuits.

The software components described here represent the actual laboratory implementation. Equivalent platforms may be used when replicating the environment.

---

## Software Overview

| Component | Software Used | Function in the Laboratory |
|---|---|---|
| Operating System | Linux | Hosts the telecommunications server environment |
| PBX Platform | FreePBX | Provides web-based PBX configuration and management |
| Telephony Engine | Asterisk | Handles call processing, extensions, and telephony services |
| Analog Hardware Support | DAHDI | Provides the interface between Asterisk and the analog telephony hardware |
| SIP/VoIP Support | Asterisk / FreePBX | Provides SIP extensions used for functional verification |
| Web Administration | FreePBX Web Interface | Allows configuration and management of the laboratory PBX |

---

## PBX Software Architecture

The core of the laboratory is a Linux-based PBX server running Asterisk and FreePBX.

Asterisk provides the underlying telephony services, while FreePBX provides a graphical management interface for configuring extensions, trunks, routing, and other PBX functions.

The server interfaces with the analog telephone infrastructure through the Digium telephony hardware and its associated DAHDI drivers.

The resulting architecture allows the laboratory server to generate analog telephone service internally without requiring a connection to the public switched telephone network (PSTN).

---

## Analog Telephony Support

Analog telephone extensions are provided through FXS interfaces installed in the PBX server.

DAHDI provides the software interface between the Linux operating system, the Digium hardware, and Asterisk.

This allows standard analog telephones connected through the laboratory distribution infrastructure to operate as extensions of the PBX.

---

## SIP / VoIP Integration

The same PBX server also supports SIP/VoIP extensions.

In the Analog Telephony Laboratory, VoIP is not introduced as the primary learning objective. Instead, preconfigured SIP phones are used as functional verification endpoints.

After students complete the analog installation, they can place calls between the student-installed analog telephone and a VoIP telephone connected to the laboratory network.

This provides immediate functional feedback while keeping the instructional focus on analog telecommunications infrastructure.

---

## Network Services

The PBX server is connected to the laboratory Ethernet network.

The network provides connectivity between the PBX server and SIP/VoIP endpoints and supports the additional network outlet installed by students as part of the laboratory activity.

The analog and Ethernet infrastructures therefore coexist within the same learning environment while remaining technically distinct.

---

## Replication Considerations

The specific software versions used in the original laboratory are not fundamental to the methodology.

A replicated environment requires:

- a Linux-compatible operating system;
- a PBX platform capable of supporting analog interfaces;
- appropriate drivers for the selected analog telephony hardware;
- support for FXS extensions;
- and, optionally, SIP/VoIP support for functional verification.

The objective is not to reproduce a specific software configuration, but to reproduce the functional learning environment.
