## VLSM Subnetting and Network Design: 4 Routers in 4 Cities

### Project Overview

This project demonstrates the design and implementation of a network for a multinational company with four branch offices located in San Francisco, Chicago, Miami, and New York. The goal is to efficiently assign subnets using Variable Length Subnet Masking (VLSM) to meet the unique host requirements for each office.

The network uses the IP address space `172.30.0.0/16`, and the specific host requirements for each city are as follows:

* **San Francisco**: 5996 hosts
* **Chicago**: 210 hosts
* **Miami**: 1080 hosts
* **New York**: 75 hosts

The project also includes inter-router connections, switch IP assignments, and the configuration of gateways.

**Note**: The project was implemented on real networking devices. Cisco Packet Tracer was used solely to replicate the environment for documentation purposes and to generate a shareable file for GitHub reference.

### Technologies Used

* Real Cisco Devices (for actual implementation)
* Cisco Packet Tracer (replica only for documentation)
* VLSM (Variable Length Subnet Masking)
* IP Addressing and Subnetting
* Routing Protocol: **OSPF only**
* Remote Access: **SSH and Telnet**

### Project Objectives

* Use VLSM to calculate and allocate the most efficient subnets for each router.
* Assign IP addresses to routers, switches, and PCs.
* Configure inter-router links with appropriate subnets for communication.
* Ensure connectivity across routers and between the routers and PCs.
* Configure SSH and Telnet for router remote management.
* Provide documentation and detailed network addressing information.

### Project Structure

This repository contains the following:

* `/PacketTracer_Files`: Cisco Packet Tracer files for the replicated environment.
* `README.md`: This file, containing project details and instructions.
* `Network_Diagram`: Visual representation of the network layout.
* `IP_Addressing_Documentation`: A detailed listing of the network address, subnet mask, usable IP range, and broadcast address for each subnet.
* `Router and Switch Configuration`: Sample configurations for the routers and network devices.

### Setup and Configuration

To get this project up and running, follow these steps:

1. Download the `PacketTracer_Files` folder.
2. Open the Packet Tracer file for the replicated configuration.
3. Check the `Router Configuration` files for IP addressing and routing setup.
4. Load the `IP Addressing Documentation` to understand the address range for each subnet.


### Questions and Tasks

**Assign IP addresses:**

* Assign the second IP to each connected switch.
* Assign the last IP to each connected PC.
* Configure router interfaces and inter-router links.

**Routing Configuration:**

* Implement **OSPF only** to enable communication between routers and devices.

**Testing:**

* Ping devices across different routers to verify network connectivity.

**Network Diagram:**

* Provide a visual representation of the network layout.


### Conclusion

This project serves as a hands-on demonstration of VLSM subnetting, IP address allocation, and router configuration. It also highlights how to efficiently use IP address space in large networks while ensuring optimal connectivity and manageability using remote access methods like SSH and Telnet. The real-device implementation reflects practical deployment scenarios, while the Cisco Packet Tracer environment is maintained solely for documentation and archival purposes.
