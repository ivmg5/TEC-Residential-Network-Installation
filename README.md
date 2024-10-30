# **TEC Residential Network Installation**
> *Robust network infrastructure for residential connectivity at Tecnológico de Monterrey.*

## **Introduction**
The TEC Residential Network Installation project addresses the need for a secure and efficient network infrastructure in a new residential building at Tecnológico de Monterrey. The project focuses on designing and configuring a scalable network to support the digital needs of students, faculty, and staff, ensuring optimal connectivity across the building's physical and logical layouts.

## **Project Description**
- **Main functionality:** Design and implementation of a reliable network infrastructure to support multiple user groups with varied access needs.
- **Technologies used:** Cisco switches (C9300L series), Cisco routers (MX105), VLAN configurations, DHCP, and Cisco Packet Tracer for simulation.
- **Challenges faced:** Managing VLAN distribution to ensure effective network segmentation and integrating various devices into a seamless infrastructure.
- **Future improvements:** Potential IPv6 integration, automation for configuration management, and enhanced monitoring capabilities.

## **Table of Contents**
1. [Introduction](#introduction)
2. [Project Description](#project-description)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Additional Documentation](#additional-documentation)
6. [Testing](#testing)
7. [License](#license)

## **Installation**
1. **Prerequisites**:
   - **Cisco Packet Tracer** - [Download here](https://www.netacad.com/courses/packet-tracer).
   - **Cisco Network Equipment** - Necessary if replicating on actual hardware.

2. **Clone the repository:**
   ```bash
   git clone https://github.com/ivmg5/TEC-Residential-Network-Installation.git
   cd TEC-Residential-Network-Installation
   ```

3. **View configurations in Packet Tracer:**
   - Load `Design.pkt` in Cisco Packet Tracer to visualize the network topology.

### **Configuration Options**
- **Environment variables** for IP addresses and VLANs are included within each `.txt` configuration file.

## **Usage**
1. **Packet Tracer Simulation**:
   - Open `Design.pkt` in Cisco Packet Tracer to explore the network layout, including device placement and logical connections.
   
2. **Applying Configuration Files**:
   - Each `.txt` file contains device-specific configurations:
     - **Switch Core**: `switchcore_configuration.txt`
     - **TR1 Switch**: `TR1_switch_configuration.txt`
     - **TR2 Switch**: `TR2_switch_configuration.txt`
     - **Router**: `router_configuration.txt`

3. **Configuration Application Example**:
   ```bash
   copy tftp://<tftp-server-ip>/switchcore_configuration.txt running-config
   ```

## **Additional Documentation**
Refer to `Documentation.pdf` in the repository for detailed insights into the project’s design phases, network requirements, and implementation approach.

## **Testing**
Run tests in Packet Tracer by simulating network connectivity and monitoring device performance:
```bash
ping 172.24.45.254
```
- Use `show run` and `show ip route` commands on devices to verify configurations.

## **License**
This project is licensed under the MIT License.

[![Build Status](https://img.shields.io/badge/status-active-brightgreen)](#)
[![Network Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen)](#)
