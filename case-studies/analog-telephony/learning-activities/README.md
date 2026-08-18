# Learning Activities

This section documents the practical learning activities used in the Analog Telephony Laboratory case study.

The activities are designed as a progressive sequence in which students build, terminate, distribute, test, and operate telecommunications infrastructure. Rather than completing isolated technical exercises, students progressively construct portions of a functional telecommunications service environment.

The laboratory activities presented here are selected from the instructional activities used in Module 20 — Connection to the Telephone Network.

The original laboratory documents have been preserved as instructional evidence. File names used in this repository describe the technical purpose of each activity rather than the original classroom numbering.

---

## Learning Sequence

The core learning sequence follows the progression:

**Build → Terminate → Distribute → Test → Connect → Operate**

Students begin with customer-premises infrastructure and progressively work toward a complete telecommunications service path that includes internal distribution, analog telephone service, network connectivity, and outside-plant components.

Functional testing is an important part of the approach. Where appropriate, completed installations are connected to the laboratory telecommunications infrastructure so that students can verify that the circuits and services they installed actually operate.

---

## Activity 1 — Customer-Premises Infrastructure

**Document:** [customer-premises-infrastructure.pdf](customer-premises-infrastructure.pdf)

The first activity introduces the physical infrastructure required to support telecommunications services within the customer premises.

Students perform practical installation tasks including:

- installation of drywall and telecommunications mounting hardware;
- installation of telecommunications cabling between the student workspace and the IDF;
- installation of Cat 3 telephone cabling;
- termination of an RJ-11 telephone outlet;
- preparation of infrastructure that will be used in subsequent activities.

This activity establishes the physical foundation upon which the remaining telecommunications system is constructed.

---

## Activity 2 — Structured Cabling and Telephony Distribution

**Document:** [structured-cabling-and-telephony-distribution.pdf](structured-cabling-and-telephony-distribution.pdf)

The second activity expands the installation from basic customer-premises infrastructure to structured cabling, distribution, testing, and telephone connectivity.

Students perform tasks involving:

- T568A and T568B terminations;
- modular connector installation;
- telecommunications faceplates;
- patch-panel termination;
- GigaBIX termination;
- cabling between the IDF and telecommunications rack;
- cable qualification using professional test equipment;
- connection to the telephone distribution infrastructure;
- cross-connection through the MDF;
- connection of the student-installed analog telephone circuit.

The activity combines structured cabling practices with telephone distribution, allowing students to see how individual installation tasks become part of a larger telecommunications system.

### Functional Verification

After the analog telephone circuit has been completed, the installation can be connected to the laboratory PBX infrastructure.

A preconfigured VoIP telephone connected to the same PBX environment can then be used as a functional endpoint for call testing.

The VoIP configuration itself is not the instructional focus of this activity. Instead, the VoIP endpoint provides a practical way for students to verify that the analog infrastructure they installed is operational.

This creates an immediate and observable result: the student-installed telephone circuit becomes part of a functioning communications system.

---

## Activity 3 — Aerial Drop and Network Interface

**Document:** [aerial-drop-and-network-interface.pdf](aerial-drop-and-network-interface.pdf)

The third core activity extends the learning environment from the building distribution infrastructure toward a simulated outside-plant installation.

Students work with components representing the service path between the telecommunications distribution infrastructure and the customer premises.

Tasks include:

- installation of cabling between the MDF and the Network Interface Device (NID);
- termination and connection at the NID;
- installation of an aerial drop;
- connection between the SLIC/distribution point and the NID;
- cross-connection of the completed service path.

This activity allows students to work beyond the traditional laboratory bench and experience a physical service path representing the transition between outside-plant infrastructure and customer-premises telecommunications wiring.

---

## Functional Learning Environment

A central characteristic of the laboratory is that student work is integrated into a functioning telecommunications environment.

The supporting PBX infrastructure provides analog telephone service to the circuits constructed by students. Preconfigured VoIP endpoints may then be used to verify the completed analog installations.

The objective is not to teach VoIP configuration during these analog telephony activities. The VoIP endpoint functions as a verification tool that makes the result of the student's work immediately observable.

Students therefore experience the relationship between:

**physical installation → termination → distribution → cross-connection → service activation → functional communication**

This approach helps connect individual installation procedures to the operation of a complete telecommunications service.

---

## Optional Activities

Additional activities used within the instructional module are documented separately in the [`optional-activities`](optional-activities/) directory.

These activities extend the learning environment beyond the core analog service-path sequence and include:

- coaxial cable distribution and testing;
- analog PABX configuration and operation.

They are maintained separately because they represent complementary telecommunications competencies rather than required stages of the core service-path sequence documented above.

---

## Educational Purpose

The purpose of these activities is to provide students with hands-on experience that reflects the relationships between telecommunications components encountered in practical installation work.

The laboratory environment emphasizes:

- authentic installation tasks;
- progressive construction of infrastructure;
- use of telecommunications distribution systems;
- testing and verification;
- integration of multiple technologies;
- functional outcomes rather than isolated component exercises.

The equipment and infrastructure used in this implementation were largely existing, donated, repurposed, or already available within the vocational training environment.

The activities are therefore presented as an example of how existing resources can be organized into an integrated, industry-oriented learning environment rather than as a prescriptive laboratory design.

---

## Related Documentation

Additional technical information about the laboratory implementation is available in:

- [`../architecture/`](../architecture/) — system architecture and service-path diagrams
- [`../hardware/`](../hardware/) — hardware components and implementation
- [`../software/`](../software/) — PBX software environment and configuration

Together, these sections document the relationship between the instructional activities and the technical infrastructure supporting the Analog Telephony Laboratory.
