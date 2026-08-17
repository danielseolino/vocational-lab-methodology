# Architecture

This directory contains technical and educational architecture diagrams for the Analog Telephony Laboratory case study.

The diagrams document both the representation of the telecommunications service path used for student learning activities and the supporting laboratory infrastructure used to provide analog telephone service in a controlled vocational education environment.

---

## Figure 1 — Analog Telephony Laboratory: Service Path and Learning Environment

![Analog Telephony Laboratory Service Path](analog-telephony-service-path.png)

**Figure 1.** Analog Telephony Laboratory service path and learning environment, illustrating the relationship between outside-plant infrastructure, student-installed telecommunications infrastructure, and the supporting laboratory system.

The diagram represents the progression from outside-plant infrastructure through the NID, MDF, IDF, customer-premises cabling, and analog telephone installation.

It also illustrates how the laboratory PBX and a preconfigured VoIP endpoint provide functional service verification after the student completes the analog installation.

The general learning sequence represented by the environment is:

**Build → Terminate → Cross-connect → Test → Use**

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
