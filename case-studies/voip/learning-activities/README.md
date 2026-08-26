# VoIP Learning Activities

This directory contains the original laboratory activities used in the **VoIP Multi-Network Laboratory** case study.

The activities form a progressive instructional sequence. Students begin by creating an individual virtual PBX environment, then configure SIP endpoints and physical IP phones, establish SIP trunking and call routing, and finally implement common business-PBX services.

Each student works with an independently routed VoIP environment. This allows the laboratory sequence to integrate PBX configuration with practical networking concepts including IPv4 addressing, LAN/WAN separation, routing, NAT, and service reachability.

> **Note:** Each laboratory is provided in **PDF** for browser viewing and **DOCX** as the original editable instructional document. The [Learning Activities page](index.qmd) provides the web-oriented overview used by the case-study site.

## Laboratory Sequence

### Phase 1 — Build the Student PBX

1. [Laboratory 1 — Configuring VirtualBox](Laboratory%201%20Configuring%20virtual%20box.pdf)  
   [View PDF](Laboratory%201%20Configuring%20virtual%20box.pdf) · [Download editable DOCX](Laboratory%201%20Configuring%20virtual%20box.docx)  
   Prepare the virtualization environment used to host the student's PBX.

2. [Laboratory 2 — Elastix](Laboratory%202%20Elastix.pdf)  
   [View PDF](Laboratory%202%20Elastix.pdf) · [Download editable DOCX](Laboratory%202%20Elastix.docx)  
   Deploy and configure the virtual PBX environment.

3. [Laboratory 3 — Setup the PBX & Extensions](Laboratory%203%20Setup%20the%20PBX%20%26%20the%20extensions.pdf)  
   [View PDF](Laboratory%203%20Setup%20the%20PBX%20%26%20the%20extensions.pdf) · [Download editable DOCX](Laboratory%203%20Setup%20the%20PBX%20%26%20the%20extensions.docx)  
   Configure the PBX and create the initial telephone extensions.

### Phase 2 — Register Physical and Software Endpoints

4. [Laboratory 4 — Configuring Zoiper](Laboratory%204%20Configuring%20zoiper.pdf)  
   [View PDF](Laboratory%204%20Configuring%20zoiper.pdf) · [Download editable DOCX](Laboratory%204%20Configuring%20zoiper.docx)  
   Configure a SIP softphone and register it to the student's PBX.

5. [Laboratory 5 — Installing an IP Phone](Laboratory%205%20Installing%20IP%20Phone.pdf)  
   [View PDF](Laboratory%205%20Installing%20IP%20Phone.pdf) · [Download editable DOCX](Laboratory%205%20Installing%20IP%20Phone.docx)  
   Configure and register a physical SIP/IP telephone.

### Phase 3 — PBX Interconnection and Call Routing

6. [Laboratory 6 — Creating a Trunk](Laboratory%206%20Creating%20trunk.pdf)  
   [View PDF](Laboratory%206%20Creating%20trunk.pdf) · [Download editable DOCX](Laboratory%206%20Creating%20trunk.docx)  
   Establish SIP trunk connectivity between PBX environments.

7. [Laboratory 7 — Creating Outbound Routes](Laboratory%207%20Creating%20outbound%20routes.pdf)  
   [View PDF](Laboratory%207%20Creating%20outbound%20routes.pdf) · [Download editable DOCX](Laboratory%207%20Creating%20outbound%20routes.docx)  
   Configure outbound call routing through the appropriate trunk.

8. [Laboratory 8 — Creating an Inbound Route](Laboratory%208%20Create%20an%20inbound%20route.pdf)  
   [View PDF](Laboratory%208%20Create%20an%20inbound%20route.pdf) · [Download editable DOCX](Laboratory%208%20Create%20an%20inbound%20route.docx)  
   Configure inbound call routing to the required PBX destination.

### Phase 4 — Automated PBX Services

9. [Laboratory 9 — Generate a Welcome Message](Laboratory%209%20Generate%20a%20welcome%20message.pdf)  
   [View PDF](Laboratory%209%20Generate%20a%20welcome%20message.pdf) · [Download editable DOCX](Laboratory%209%20Generate%20a%20welcome%20message.docx)  
   Prepare audio content for automated telephone services.

10. [Laboratory 10 — Upload the WAV Message into System Recordings](Laboratory%2010%20Upload%20the%20wav%20message%20into%20the%20system%20recording.pdf)  
   [View PDF](Laboratory%2010%20Upload%20the%20wav%20message%20into%20the%20system%20recording.pdf) · [Download editable DOCX](Laboratory%2010%20Upload%20the%20wav%20message%20into%20the%20system%20recording.docx)  
    Add the prepared audio message to the PBX system recordings.

11. [Laboratory 11 — Creating an Announcement](Laboratory%2011%20Creating%20announcement.pdf)  
   [View PDF](Laboratory%2011%20Creating%20announcement.pdf) · [Download editable DOCX](Laboratory%2011%20Creating%20announcement.docx)  
    Configure an automated PBX announcement using the system recording.

12. [Laboratory 12 — Create a Ring Group](Laboratory%2012%20Create%20a%20ring%20group.pdf)  
   [View PDF](Laboratory%2012%20Create%20a%20ring%20group.pdf) · [Download editable DOCX](Laboratory%2012%20Create%20a%20ring%20group.docx)  
    Configure multiple extensions to respond as a functional group.

13. [Laboratory 13 — Create a Queue Group](Laboratory%2013%20Create%20a%20Queue%20group.pdf)  
   [View PDF](Laboratory%2013%20Create%20a%20Queue%20group.pdf) · [Download editable DOCX](Laboratory%2013%20Create%20a%20Queue%20group.docx)  
    Configure a call queue and its participating endpoints.

14. [Laboratory 14 — Create a Time Group](Laboratory%2014%20Create%20a%20time%20group.pdf)  
   [View PDF](Laboratory%2014%20Create%20a%20time%20group.pdf) · [Download editable DOCX](Laboratory%2014%20Create%20a%20time%20group.docx)  
    Define the schedule used by time-dependent PBX behavior.

15. [Laboratory 15 — Create a Time Condition](Laboratory%2015%20Create%20a%20time%20condition.pdf)  
   [View PDF](Laboratory%2015%20Create%20a%20time%20condition.pdf) · [Download editable DOCX](Laboratory%2015%20Create%20a%20time%20condition.docx)  
    Route calls according to the configured time group.

16. [Laboratory 16 — Create an IVR in the PBX](Laboratory%2016%20Create%20an%20ivr%20in%20the%20PBX.pdf)  
   [View PDF](Laboratory%2016%20Create%20an%20ivr%20in%20the%20PBX.pdf) · [Download editable DOCX](Laboratory%2016%20Create%20an%20ivr%20in%20the%20PBX.docx)  
    Integrate recordings, routing destinations, and telephone keypad input into an interactive voice response service.

## Advanced Learning Activities

After the formal laboratory sequence is operational, the environment can support additional activities that connect PBX configuration with networking and telecommunications interoperability.

### NAT and Port Forwarding

A student can create an extension on their PBX for use by a classmate located behind a different router. Because the hosting PBX is located inside a private LAN, the student must configure the required port forwarding and verify external SIP registration and connectivity.

This activity reinforces the relationship between **LAN/WAN separation, NAT, port forwarding, SIP registration, and service reachability**.

### Analog–VoIP Interconnection

When the same cohort completes both the Analog Telephony and VoIP modules, the central VoIP/FreePBX system can be connected to the analog telephony environment through a SIP trunk.

This intentionally reverses the role of the technologies across the two modules: the Analog Telephony laboratory uses VoIP endpoints to verify analog infrastructure, while the VoIP laboratory uses the analog environment as an external telecommunications destination.

## Related Documentation

- [VoIP Case Study](../index.qmd)
- [Architecture](../architecture/index.qmd)
- [Hardware](../hardware/index.qmd)
- [Software](../software/index.qmd)
- [Learning Activities — Web Overview](index.qmd)
