# FreePBX Configuration

This document describes the PBX configuration used to support the Analog Telephony Laboratory.

The objective of this configuration is to provide a self-contained telephone service that allows students to install, terminate, cross-connect, test, and use analog telephone circuits without requiring access to the public switched telephone network (PSTN).

The PBX server also supports SIP/VoIP endpoints. In the analog telephony activities, these endpoints are used primarily for functional verification of student-installed analog lines.

---

## System Architecture

The laboratory PBX is based on:

- Linux operating system
- Asterisk telephony engine
- FreePBX management interface
- DAHDI hardware interface
- Digium AEX2400 analog interface card
- Digium S400M FXS modules

The basic software and hardware relationship is:

```text
FreePBX
   │
Asterisk
   │
DAHDI
   │
Digium AEX2400
   │
S400M FXS Modules
   │
25-Pair Distribution Interface
   │
Laboratory Telecommunications Infrastructure
   │
Student-Installed Analog Telephone
