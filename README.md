# Installation of Network Systems in the New Residential Building at Tecnológico de Monterrey

## Project Overview

This repository contains the complete files and configurations related to the installation of a network system in a new residential building at Tecnológico de Monterrey, Campus Guadalajara. The project aims to provide a robust, secure, and efficient infrastructure to meet the digital needs of students, faculty, and administrative staff. The initiative involves designing both the physical and logical aspects of the network, integrating devices like access points, cameras, fire detectors, and administrative computers, all to ensure comprehensive and seamless connectivity.

### Contents

- **Packet Tracer File**: The main `.pkt` file includes the complete network design and configuration, showcasing the physical and logical layouts.
- **Configuration Files**: Individual `.txt` files containing the configurations for each of the network devices:
  - `switchcore.txt`: Configuration of the core switch.
  - `TR1switch.txt`: Configuration for the TR1 switch.
  - `TR2switch.txt`: Configuration for the TR2 switch.
  - `router.txt`: Configuration of the router handling the network.
- **Documentation (PDF)**: The full project report details the network requirements, implementation plan, and design rationale.

### Key Features of the Network Design

1. **Robust Physical and Logical Network Layout**:
   - Physical designs that show where switches, access points, sensors, and other terminal equipment are located.
   - Logical designs employing VLANs and subnetting to efficiently distribute IP addresses and manage different segments of the network.

2. **Detailed Project Scope**:
   - The project includes multiple phases: Analysis, Design, Implementation, and Proposal Delivery.
   - Key components include detailed analysis of the physical spaces, network configuration, and the selection of suitable equipment for a high-traffic, high-reliability network.

3. **Hardware and Addressing**:
   - **Switches**: Different types of switches (Cisco C9300L-48UXG-4X-M and others) are used for core, access, and distribution layers.
   - **Routers**: A router (Cisco MX105) configured to manage dynamic IP allocation using DHCP and route traffic between VLANs.
   - **Access Points**: Multiple AP models (CW9164, CW9162, MR78) were selected to ensure optimal coverage for rooms, common areas, and outdoor environments.

4. **Security and Configuration Settings**:
   - Configuration includes VLAN segmentation, spanning-tree protocol (PVST) for network reliability, and DHCP configurations for device IP management.
   - Access control via passwords and encrypted secrets to secure the network against unauthorized changes.

### Configuration Files Breakdown

- **Switch Core Configuration** (`switchcore.txt`): Includes trunk configuration, PVST mode for loop prevention, and GigabitEthernet interface settings to connect to various network components.
- **TR1 Switch Configuration** (`TR1switch.txt`): This switch manages VLAN connections for the administration, entertainment, and infrastructure systems. It includes trunk and access configurations for different VLANs (VLAN 2, VLAN 5, etc.).
- **TR2 Switch Configuration** (`TR2switch.txt`): This switch handles the configuration for VLANs related to infrastructure (lighting, fire detection, etc.) and resident services. It also contains trunk and access port configurations.
- **Router Configuration** (`router.txt`): The router is responsible for providing DHCP services, managing inter-VLAN routing, and connecting the internal network to external internet services.

### Usage

1. **Packet Tracer File**:
   - Load the provided `.pkt` file in Cisco Packet Tracer to view the entire network simulation.
   - It shows the complete setup, including the physical locations of each network device and the logical connections.

2. **Configuration Files**:
   - These configuration files can be used to replicate the setup on actual Cisco hardware.
   - Apply each configuration to its respective device, ensuring the network matches the design laid out in the Packet Tracer file.

3. **Documentation**:
   - The PDF document contains an in-depth explanation of the project phases, equipment selection, design choices, and economic analysis. It's recommended to refer to this document for understanding the rationale behind each design decision.

### Network Design Goals

- **Scalability**: Designed to accommodate up to 1,000 users, including residents, visitors, and other devices like cameras and sensors.
- **Security**: All configurations are secured with encrypted passwords and limited access via VTY lines for remote management.
- **Reliability and Redundancy**: Redundant switches and spanning-tree protocols ensure the network remains operational even in case of device failures.

### Economic Proposal

The equipment costs are carefully detailed in the documentation to justify the choice of high-performance devices that meet both current needs and potential future scalability requirements. The selected devices provide high bandwidth, reliability, and compatibility with existing campus infrastructure.

### Future Improvements

This project lays the foundation for an easily expandable network infrastructure. Future improvements might include:

- **Upgrading to IPv6**: Currently, the network uses IPv4 with VLSM. Expanding to IPv6 will future-proof the system.
- **Network Automation**: Implementing network automation tools for configuration management to reduce the administrative overhead.
- **Advanced Monitoring**: Integration with network monitoring tools to continuously observe network health and optimize performance.

### License

This project is open-sourced under the [MIT License](LICENSE).
