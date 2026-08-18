# Architecture

This directory contains technical and educational architecture diagrams for the Analog Telephony Laboratory case study.

The diagrams document both the representation of the telecommunications service path used for student learning activities and the supporting laboratory infrastructure used to provide analog telephone service in a controlled vocational education environment.

---
## Figure 1 — Analog Telephony Laboratory: End-to-End Service Path

![Analog Telephony Laboratory End-to-End Service Path](analog-telephony-service-path.png)

**Figure 1.** End-to-end architecture of the Analog Telephony Laboratory, showing how analog telephone service generated locally by the PBX is routed through a simulated outside-plant environment and into infrastructure installed by students.

The PBX provides FXS analog service through the Digium AEX2400 interface and S400M FXS modules. This service is routed through a 25-pair distribution system to a simulated outside plant consisting of a SLIC/distribution point, aerial drop cable, and NID.

From the NID, students build and terminate the customer-side infrastructure through the MDF and IDF. The learning activity includes both an analog telecommunications path (e.g., Cat 3 to an RJ-11 outlet) and a network path (Cat 6 to an RJ-45 outlet), reflecting the coexistence of legacy and IP-based telecommunications infrastructure.

After completing the installation, students connect an analog telephone to the line they installed. A preconfigured SIP/VoIP endpoint, operating through the laboratory network and PBX, is then used to place and receive calls with the student-installed analog extension. In this activity, VoIP is used as a functional verification tool rather than as the primary subject of instruction.

The complete learning sequence represented by the laboratory is:

**Service Generation → Simulated Outside Plant → Build → Terminate → Cross-Connect → Test → Functional Use**

---

## Figure 2 — PBX Analog Telephony Architecture

![PBX Analog Telephony Architecture](pbx-analog-telephony-architecture.png)

**Figure 2.** Technical architecture of the laboratory PBX infrastructure used to generate and distribute analog telephone extensions to student installations.

The PBX environment is based on a Linux server running Asterisk and FreePBX with a Digium AEX2400 PCI Express telephony interface.

The AEX2400 supports S400M quad-port FXS modules, providing up to 24 analog station interfaces. These interfaces supply the analog telephone service used throughout the laboratory without requiring connection to the Public Switched Telephone Network (PSTN).

A 25-pair distribution connection provides a protective and maintainable interface between the PBX hardware and the telecommunications infrastructure routinely handled during student activities.

This architecture allows individual analog extensions to be routed through the MDF and subsequently to student installations while protecting the primary PBX cabling from repeated handling and modification.

---

## Figure 3 — Mobile Analog/VoIP Training Platform

![Mobile Analog VoIP Training Platform](mobile-analog-voip-training-platform.png)

**Figure 3.** Physical implementation of one of the mobile Analog/VoIP training platforms used to support telecommunications laboratory activities.

The mobile platform consolidates the principal service and network components required for the laboratory into a transportable system. The implementation includes the PBX server, PoE Ethernet switch, wireless router/access point, preconfigured VoIP telephone, analog telephony interface hardware, and the 25-pair distribution/protection connection.

The 25-pair distribution connection provides an intermediate interface between the PBX hardware and the cabling routinely handled during laboratory activities. This allows frequently manipulated external cabling and terminations to be repaired or replaced without requiring modification or replacement of the primary PBX interface cabling.

The preconfigured VoIP telephone provides a functional endpoint that can be used during analog telephony activities to verify completed student installations without requiring students to configure the VoIP infrastructure at this stage of the curriculum.

Two mobile platforms are available for laboratory activities, while an additional fixed installation is maintained in the telecommunications laboratory. The mobile configuration allows the same infrastructure to support different classrooms, modules, and instructors without requiring complete duplication of the system.

## Architecture Design Considerations

The laboratory architecture was developed around several practical considerations:

- representation of relevant telecommunications service-path components;
- support for multiple simultaneous student installations;
- separation between student-handled infrastructure and core PBX equipment;
- low-cost repair and replacement of frequently manipulated cabling;
- reuse of the same PBX infrastructure across multiple laboratory activities;
- functional verification of completed installations;
- integration with subsequent VoIP learning activities;
- operation without recurring PSTN service requirements.

These design decisions support the broader objective of transforming authentic telecommunications work processes into accessible and maintainable hands-on learning environments for vocational education.

---

## Planned Documentation

Additional architecture documentation will include:


- relationship between mobile and fixed laboratory installations;
- hardware inventory and implementation considerations.
