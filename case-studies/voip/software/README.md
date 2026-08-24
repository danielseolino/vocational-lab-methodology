# Software

The VoIP Multi-Network Laboratory combines open-source PBX software, virtualization, and SIP softphones to allow each student to build and operate an independent VoIP environment.

Unlike the central instructor-managed infrastructure, each student deploys and configures their own PBX within a virtual machine. This makes PBX installation, configuration, endpoint registration, routing, and troubleshooting part of the learning process.

## Software Environment

The laboratory uses the following main software components:

### Linux

Linux provides the operating system environment for the PBX platforms.

The central instructor-managed server and the student virtual PBX environments use Linux-based systems to host the telephony services.

### Asterisk / FreePBX

Asterisk provides the underlying telephony engine, while FreePBX provides the web-based administration interface used throughout the laboratory activities.

Students use the PBX environment to configure and explore functions including:

- SIP extensions;
- endpoint registration;
- SIP trunks;
- inbound and outbound routes;
- recordings and announcements;
- ring groups;
- queues;
- time conditions;
- IVR;
- and other PBX services introduced through the learning activities.

### VirtualBox

VirtualBox allows each student to operate an independent PBX on their assigned laptop.

The virtual machine is connected to the student's private `192.168.1.0/24` network, allowing the PBX to communicate with the physical IP phone and software endpoints while remaining behind the student's router.

This approach allows multiple complete PBX environments to operate simultaneously in the same laboratory.

### Zoiper

Zoiper is used as a SIP softphone endpoint on student devices.

Students can use Zoiper on:

- the laptop;
- a mobile device;
- and, during advanced activities, from another student's network.

This provides a flexible endpoint for testing extension registration, internal calling, external connectivity, NAT, and port forwarding.

## Central and Student PBX Roles

The laboratory deliberately uses two different PBX roles.

### Central PBX

The instructor-managed FreePBX server operates on the laboratory/provider network (`172.16.0.0/16`).

Its primary functions include:

- providing shared VoIP services;
- hosting laboratory/provider extensions;
- supporting SIP trunk interconnection;
- providing external calling targets for student systems;
- and supporting integration with other laboratory environments.

### Student PBX

Each student operates an independent FreePBX instance within their private `192.168.1.0/24` network.

Students are responsible for configuring their own PBX services, endpoints, trunks, and routing.

This separation creates a provider/customer relationship within the laboratory and allows students to troubleshoot both local and inter-network VoIP communication.

## SIP Interconnection

SIP trunks provide the logical connection between independently managed PBX systems.

Within the laboratory, trunking can be used to connect:

- student PBXs to the central VoIP infrastructure;
- independent student systems;
- the VoIP laboratory to the Analog Telephony Laboratory;
- and, in future development, additional telecommunications environments.

The use of SIP trunking therefore provides both a technical learning activity and an integration mechanism between laboratory systems.

## Software-Based Functional Verification

The software environment allows students to verify the operation of the network through actual telecommunications services.

Rather than validating configuration only through status screens or command output, students can register endpoints, establish calls, test routing, and observe whether the complete system operates as intended.

This provides immediate functional feedback between configuration decisions and observable system behavior.
