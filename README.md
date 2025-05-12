# VLSM Subnetting and Network Design: 4 Routers in 4 Cities

## Project Overview
This project demonstrates the design and implementation of a network for a multinational company with four branch offices located in San Francisco, Chicago, Miami, and New York. The goal is to efficiently assign subnets using **Variable Length Subnet Masking (VLSM)** to meet the unique host requirements for each office.

The network uses the **IP address space 172.30.0.0/16**, and the specific host requirements for each city are as follows:

- **San Francisco**: 5996 hosts
- **Chicago**: 210 hosts
- **Miami**: 1080 hosts
- **New York**: 75 hosts

The project also includes inter-router connections, switch IP assignments, and the configuration of gateways.

## Technologies Used
- Cisco Packet Tracer (for simulation and configuration)
- VLSM (Variable Length Subnet Masking)
- IP Addressing and Subnetting
- Routing Protocols (Static Routing / Dynamic Routing, if implemented)

## Project Objectives
- Use VLSM to calculate and allocate the most efficient subnets for each router.
- Assign IP addresses to routers, switches, and PCs.
- Configure inter-router links with appropriate subnets for communication.
- Ensure connectivity across routers and between the routers and PCs.
- Provide documentation and detailed network addressing information.

## Project Structure
This repository contains the following:

- **/PacketTracer_Files**: Cisco Packet Tracer files for the network design.
- **README.md**: This file, containing project details and instructions.
- **Network_Diagram**: Visual representation of the network layout.
- **IP_Addressing_Documentation**: A detailed table listing the network address, subnet mask, usable IP range, and broadcast address for each subnet.
- **Router Configuration**: Sample configurations for the routers and network devices.


## Setup and Configuration
To get this project up and running, follow these steps:

1. Download the **PacketTracer_Files** folder.
2. Open the Packet Tracer file for each router configuration.
3. Check the **Router Configuration** files for IP addressing and routing setup.
4. Load the **IP Addressing Documentation** to understand the address range for each subnet.

## Questions and Tasks
The project includes the following tasks:

1. **Assign IP addresses**:
   - Assign the second IP to each connected switch.
   - Assign the last IP to each connected PC.
   - Configure router interfaces and inter-router links.

2. **Routing Configuration**:
   - Implement routing protocols (if applicable) to enable communication between routers and devices.

3. **Testing**:
   - Ping devices across different routers to verify network connectivity.

4. **Network Diagram**:
   - Provide a visual representation of the network layout.

## Future Enhancements
- **Dynamic Routing**: Implement a dynamic routing protocol like OSPF or EIGRP to replace static routing.
- **Security Measures**: Configure basic access control lists (ACLs) to secure the network.

## Conclusion
This project serves as a hands-on demonstration of VLSM subnetting, IP address allocation, and router configuration. It also highlights how to efficiently use IP address space in large networks while ensuring optimal connectivity.

---


