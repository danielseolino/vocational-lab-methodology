# VoIP Multi-Network Laboratory

This case study documents a hands-on VoIP learning environment designed for vocational telecommunications education.

The laboratory is based on a multi-network architecture in which each student builds and manages an independent VoIP network while a central instructor-managed infrastructure provides a shared provider/interconnection network.

Each student works with a dedicated router, laptop, virtual PBX environment, physical IP telephone, and softphone endpoints. This allows students to configure and troubleshoot a complete VoIP system rather than interacting only with a preconfigured centralized PBX.

The laboratory integrates practical concepts including:

- IPv4 addressing and private network ranges;
- LAN and WAN segmentation;
- routing and Network Address Translation (NAT);
- virtualized PBX deployment;
- SIP extensions and endpoints;
- physical IP phones and softphones;
- SIP trunks;
- inbound and outbound call routing;
- PBX services such as recordings, announcements, ring groups, queues, time conditions, and IVR;
- port forwarding and external endpoint registration;
- and interconnection with analog telephony infrastructure.

## Layered Network Architecture

The laboratory uses three private IPv4 network layers:

**School / Enterprise Network**  
`10.0.0.0/8`

**VoIP Laboratory / Provider Network**  
`172.16.0.0/16`

**Student / Customer LAN**  
`192.168.1.0/24`

Each student router connects its WAN interface to the shared 172.16.0.0/16 laboratory network while providing an isolated 192.168.1.0/24 LAN for the student's PBX and VoIP endpoints.

This structure allows students to explore the relationship between IP addressing, LAN/WAN separation, routing, NAT, and VoIP services within a controlled laboratory environment.

## Student Laboratory Environment

Each student receives a dedicated equipment set including:

- laptop computer;
- router;
- physical SIP/IP telephone;
- VirtualBox environment running the student's PBX;
- Zoiper softphone on the laptop;
- and a mobile softphone endpoint.

The student therefore operates an independent routed network and is responsible for configuring and validating the services within that environment.

## Central VoIP Infrastructure

A separate instructor-managed mobile laboratory platform provides the shared VoIP provider/interconnection network.

The central infrastructure includes:

- Linux / FreePBX / Asterisk server;
- Ethernet switching;
- routing infrastructure;
- SIP endpoint for testing and demonstrations;
- and connectivity to the student WAN interfaces.

The central PBX provides external extensions and SIP interconnection services that allow students to place calls beyond their own private networks.

## Advanced Network Activity

After the individual student systems are operational, students explore NAT and port forwarding by allowing another student to register a VoIP endpoint to an extension hosted on their PBX.

This activity demonstrates why an internal service is not automatically reachable from an external network and introduces practical troubleshooting involving ports, NAT, routing, and SIP connectivity.

## Cross-Module Integration

When the same student group completes both the Analog Telephony and VoIP modules, the two laboratory environments can be interconnected through a SIP trunk.

The educational roles are intentionally reversed between the modules:

**Analog Telephony Module:**  
Students build analog infrastructure and use VoIP endpoints for functional verification.

**VoIP Module:**  
Students build VoIP infrastructure and use existing analog telephone lines and endpoints for functional verification.

This allows the same infrastructure to support different learning objectives while demonstrating interoperability between legacy and IP-based telecommunications systems.

## Documentation

This case study will include:

- system and network architecture;
- central infrastructure documentation;
- student hardware configuration;
- software and PBX configuration;
- learning activities;
- SIP trunk and routing examples;
- NAT and port-forwarding activities;
- cross-module analog/VoIP integration;
- and replication considerations.

Additional documentation will be added as the case study is developed.
