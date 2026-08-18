# Hardware

This section documents the hardware used to implement the Analog Telephony Laboratory.

The laboratory was developed primarily by reusing equipment already available in the vocational school. The specific models listed below represent the actual implementation and should not be interpreted as mandatory requirements for replication.

The objective is to demonstrate that an operational telecommunications training environment can be developed using existing, donated, repurposed, or low-cost equipment.

---

## Hardware Overview

| Component | Equipment Used | Function in the Laboratory | Required for Replication? |
|---|---|---|---|
| PBX Server | Dell Precision T3600 | Hosts the Linux-based PBX environment | No — any compatible computer may be used |
| Analog Telephony Interface | Digium AEX2400 | Provides the interface between the PBX server and analog telephone circuits | Equivalent analog interface required |
| FXS Modules | Digium S400M modules | Provide FXS interfaces for analog telephone extensions | Equivalent FXS capability required |
| Ethernet / PoE Switch | EnGenius EGS7228FP PoE+ | Provides network connectivity and PoE support for IP phones | Any suitable Ethernet/PoE switch |
| Wireless Network | ASUS RT-N10 Wireless N Router | Provides wireless access for mobile devices and softphones | Optional |
| Telephone Distribution | 25-pair telecommunications cable and distribution blocks | Connects the PBX analog interfaces to the laboratory distribution infrastructure | Functionally required |
| Analog Telephones | Standard analog telephones | Student-installed endpoints used for service testing | Yes |
| SIP / VoIP Phones | Preconfigured SIP phones | Provide functional verification of student-installed analog circuits | Optional but educationally valuable |

---

## PBX Server

The laboratory PBX is hosted on a repurposed **Dell Precision T3600 workstation**.

Rather than purchasing a dedicated telecommunications server, an existing computer was reused to provide the processing platform for the laboratory.

The server hosts the Linux-based PBX environment and supports both the analog telephony interface and the IP network used by the laboratory.

This reuse of existing computer hardware is an important element of the laboratory design because it reduces implementation cost while maintaining a functional telecommunications environment.

The Dell Precision T3600 is the equipment used in this implementation; however, the laboratory methodology does not depend on this specific computer model.

---

## Analog Telephony Interface

Analog telephone service is generated through a **Digium AEX2400 PCIe telephony interface card** installed in the PBX server.

The card is populated with **Digium S400M FXS modules**, providing analog subscriber interfaces for the laboratory.

The FXS interfaces reproduce the basic electrical and signaling conditions expected by standard analog telephones, allowing students to work with functional telephone circuits rather than simulated connections.

In the current implementation, the analog interface can support multiple student telephone lines simultaneously.

The specific Digium hardware represents the equipment available for this implementation. Other compatible analog telephony interfaces could be used to reproduce the same educational architecture.

---

## 25-Pair Distribution Interface

A 25-pair telecommunications cable connects the analog telephony interface to the laboratory distribution system.

An important design decision was made to avoid exposing the PBX interface cabling directly to repeated student handling.

Instead, an intermediate distribution and cross-connect point is used between the PBX hardware and the student-accessible telecommunications infrastructure.

This creates a replaceable interface between the relatively expensive telephony hardware and the cabling manipulated during laboratory activities.

### Why this matters

Vocational laboratories involve repeated termination, connection, disconnection, testing, and troubleshooting activities.

Components handled frequently by students can eventually become damaged.

Replacing a short section of telecommunications cable or rebuilding a cross-connect is inexpensive compared with replacing a specialized telephony interface, connector, or PBX component.

The distribution interface therefore serves two purposes:

1. **Telecommunications function** — providing an organized transition between the PBX and the laboratory cabling infrastructure.
2. **Equipment protection** — isolating expensive PBX hardware from components subjected to repeated student manipulation.

This approach contributes directly to the low-cost and maintainable design philosophy of the laboratory.

---

## Ethernet and PoE Infrastructure

An **EnGenius EGS7228FP PoE+ switch** provides Ethernet connectivity for the IP portion of the laboratory.

The switch supports the SIP/VoIP telephones used as functional endpoints and provides Power over Ethernet where required.

The IP network is not the primary learning objective of the analog telephony activities.

Instead, it acts as supporting infrastructure that allows students to verify their analog installations through actual telephone calls.

This separation is pedagogically intentional: students can experience the complete operation of the telecommunications service without requiring detailed VoIP configuration knowledge during the analog telephony module.

---

## Wireless Access

An **ASUS RT-N10 Wireless N Router** is included in the mobile laboratory setup.

Its primary purpose is to provide wireless network access when mobile devices or software-based SIP clients are used.

Wireless connectivity is not required for the analog telephone laboratory itself and should therefore be considered an optional supporting component.

This also illustrates the modular nature of the laboratory architecture: additional technologies can be incorporated without changing the underlying analog telecommunications exercises.

---

## Analog Telephone Endpoints

Standard analog telephones are used as student endpoints.

Students install the telecommunications pathway and eventually connect an analog telephone to the circuit they have constructed.

This allows verification to extend beyond continuity testing.

The student can observe dial tone, place or receive calls, and verify that the installed telecommunications pathway operates as part of a complete service.

---

## VoIP Endpoint for Functional Verification

A preconfigured SIP/VoIP telephone is connected to the same PBX environment.

During the analog telephony module, students are not required to configure or study the VoIP system in detail.

Instead, the VoIP telephone functions as a known working endpoint that can communicate with the analog extensions.

This provides an immediate and visible method of validating the student's work:

**Build → Terminate → Cross-connect → Test → Use**

After completing the analog installation, students can make or receive an actual telephone call.

The objective is to move the laboratory experience beyond isolated cable testing and allow students to observe the result of their work as a functioning telecommunications service.

Detailed VoIP concepts and configuration can subsequently be introduced in dedicated IP telephony activities.

---

## Mobile Laboratory Configuration

The telecommunications system was designed so that portions of the infrastructure can be installed on mobile equipment carts.

A typical mobile setup includes:

- PBX server
- analog telephony interface
- 25-pair distribution interface
- Ethernet/PoE switch
- wireless router/access point
- analog telephone
- SIP/VoIP telephone
- associated telecommunications cabling

This configuration allows the same infrastructure to support activities in different classrooms or laboratory areas.

Multiple setups can therefore share the same general architecture while being deployed according to instructional needs.

---

## Replication Principle

The hardware models documented here should be considered examples rather than a fixed bill of materials.

The laboratory architecture can be represented functionally as:

**Computer / PBX Server**

↓

**Analog Telephony Interface**

↓

**FXS Interfaces**

↓

**Protected Distribution / Cross-Connect**

↓

**Student Telecommunications Infrastructure**

↓

**Analog Telephone**

with a parallel IP infrastructure:

**PBX Server → Ethernet/PoE Network → SIP/VoIP Endpoint**

The important requirement is preservation of these functions, not duplication of the exact hardware models.

This allows vocational programs to adapt the laboratory to equipment they already own, equipment available through donations, or affordable components available locally.

---

## Design Philosophy

The hardware architecture follows four practical principles:

**Reuse available equipment → Protect expensive components → Provide functional service → Keep the system adaptable**

The resulting environment allows students to construct and test telecommunications infrastructure while interacting with an operational telephone system rather than an isolated training board.

This approach supports the broader objective of developing accessible, industry-based hands-on learning environments using existing or low-cost resources.
