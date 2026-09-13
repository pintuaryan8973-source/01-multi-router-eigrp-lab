# Multi-Router EIGRP Routing Lab

## Project Overview

This project demonstrates the design and configuration of a multi-router network using Cisco Packet Tracer.

EIGRP dynamic routing was implemented to enable communication between multiple networks.

The lab focuses on practical routing configuration, EIGRP neighbor formation, dynamic route learning, connectivity testing and troubleshooting.

---

## Objective

The objective of this project is to:

- Design a multi-router network topology
- Configure IPv4 addressing
- Configure EIGRP dynamic routing
- Establish EIGRP neighbor relationships
- Verify dynamically learned routes
- Test end-to-end network connectivity
- Analyze packet paths using Traceroute
- Practice basic network troubleshooting

---

## Technologies / Tools Used

- Cisco Packet Tracer
- Cisco Routers
- Cisco IOS CLI
- IPv4 Addressing
- EIGRP
- Ping
- Traceroute
- Git
- GitHub

---

## Lab Environment

This project was performed in a controlled Cisco Packet Tracer lab environment for educational purposes.

The network contains multiple routers connected through different IPv4 networks.

### EIGRP Autonomous System

```text
100
```

---

## What I Did

In this project I:

- Designed a multi-router network topology
- Configured router interfaces
- Assigned IPv4 addresses
- Enabled router interfaces
- Configured EIGRP AS 100
- Advertised connected networks through EIGRP
- Established EIGRP neighbor relationships
- Verified dynamically learned EIGRP routes
- Checked router interface status
- Tested remote network connectivity using Ping
- Used Traceroute to analyze packet paths
- Verified routing using Cisco IOS commands

---

## EIGRP Configuration

EIGRP was configured using Autonomous System Number:

```text
100
```

EIGRP allows routers to exchange routing information dynamically.

The configuration was verified using Cisco IOS commands.

---

## EIGRP Neighbor Verification

Command used:

```text
show ip eigrp neighbors
```

The router successfully formed EIGRP neighbor relationships.

Observed neighbor addresses included:

```text
70.0.0.2
40.0.0.1
```

This confirmed that EIGRP adjacency between the routers was successfully established.

The neighbor table also showed stable EIGRP communication.

---

## Routing Table Verification

Command used:

```text
show ip route
```

The routing table displayed both directly connected networks and dynamically learned routes.

EIGRP-learned routes are identified by the letter:

```text
D
```

The appearance of `D` routes confirmed that the routers were successfully exchanging routing information through EIGRP.

---

## EIGRP Configuration Verification

Command used:

```text
show running-config | section router eigrp
```

This command was used to verify the EIGRP configuration running on the router.

It helped confirm:

- EIGRP process number
- Advertised networks
- Routing configuration

---

## Interface Verification

Command used:

```text
show ip interface brief
```

This command was used to verify:

- Interface names
- IPv4 addresses
- Interface status
- Protocol status

This helped confirm that the required router interfaces were active and correctly configured.

---

## Connectivity Test

Remote network connectivity was tested using Ping.

Command used:

```text
ping 100.0.0.1
```

The Ping test completed successfully.

This confirmed that packets were able to travel between different networks through the configured routers.

---

## Traceroute Test

Command used:

```text
traceroute 100.0.0.1
```

Observed route:

```text
1   40.0.0.2
2   70.0.0.2
```

The Traceroute test successfully displayed the path taken by packets toward the remote destination.

This helped verify the routing path selected by the network.

---

## Verification Commands

The following commands were used during the project:

```text
show ip eigrp neighbors
show ip route
show running-config | section router eigrp
show ip interface brief
ping 100.0.0.1
traceroute 100.0.0.1
```

---

## Results

The Multi-Router EIGRP Routing Lab was successfully configured and tested.

### Final Results

- Router interfaces were successfully configured
- EIGRP AS 100 was successfully configured
- EIGRP neighbor relationships were established
- Dynamic routes appeared in the routing table
- Routers successfully exchanged routing information
- Remote network Ping testing was successful
- Traceroute successfully displayed the packet path
- End-to-end network connectivity was verified

---

## Screenshots

The repository contains practical evidence from the lab.

Screenshots include:

1. Network Topology
2. EIGRP Neighbor Table
3. Routing Table
4. EIGRP Configuration
5. Interface Status
6. Ping Test
7. Traceroute Test

Screenshots are stored inside the:

```text
screenshots/
```

folder.

---

## Screenshot Structure

```text
screenshots/
│
├── 01-topology.png
├── 02-eigrp-neighbors.png
├── 03-routing-table.png
├── 04-eigrp-config.png
├── 05-interface-status.png
├── 06-ping-test.png
└── 07-traceroute.png
```

---

## Learning Outcomes

Through this project I learned:

- How dynamic routing works
- How EIGRP works in a multi-router environment
- How routers discover EIGRP neighbors
- How EIGRP exchanges routing information
- How to verify EIGRP neighbors
- How to understand a routing table
- How to identify EIGRP routes
- How to verify router interface status
- How to test network connectivity using Ping
- How to analyze routing paths using Traceroute
- How to perform basic network troubleshooting
- How to document a networking project on GitHub

---

## Troubleshooting

During network testing, the following commands can help identify problems:

```text
show ip interface brief
show ip route
show ip eigrp neighbors
ping <destination-ip>
traceroute <destination-ip>
```

These commands help verify interfaces, routing tables, EIGRP adjacency and network connectivity.

---

## Future Improvements

This project can be improved in the future by practically implementing:

- VLANs
- Inter-VLAN Routing
- DHCP
- DNS
- Access Control Lists (ACL)
- Network segmentation
- Additional routing scenarios
- Advanced troubleshooting
- Network redundancy

These features will only be added after practical implementation and testing.

---

## Security & Ethics

All networking and security experiments shown in this repository were performed in a controlled lab environment for educational purposes.

No unauthorized network, system, server, website, wireless network or device was tested.

---

## Project Status

```text
Status: Completed
Environment: Cisco Packet Tracer
Routing Protocol: EIGRP
EIGRP AS: 100
Connectivity Test: Successful
Traceroute Test: Successful
```

---

## Author

**Pintu Aryan**

Aspiring Cyber Security Analyst

Networking | Python | Security Operations

### GitHub

https://github.com/pintuaryan8973-source

---

## Repository

Project Repository:

https://github.com/pintuaryan8973-source/01-multi-router-eigrp-lab
