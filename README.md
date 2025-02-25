# Enterprise-DMVPN-Secure-Networking
This project implements a scalable, secure, and redundant DMVPN architecture for enterprise networks. It includes multipoint GRE tunnels, NHRP, EIGRP routing, redundancy, and IPSec encryption for secure communication. The draft documentation provides a step-by-step deployment guide, making it ideal for real-world networking environments. 
## Overview
This repository provides a comprehensive Dynamic Multipoint VPN (DMVPN) deployment designed for scalable, secure, and resilient enterprise networks. It includes configurations for multipoint GRE tunnels, NHRP, EIGRP routing, redundancy, and IPSec encryption for secure data transmission over public networks.

DMVPN enables seamless site-to-site and remote access VPN connectivity, reducing the complexity of traditional VPN architectures while maintaining security and performance.

## Project Scope
This deployment is designed for enterprises, ISPs, and cloud providers requiring secure, dynamic, and scalable VPN connectivity between multiple locations. The implementation ensures:
✅ Dynamic Tunnels – No need for static peer-to-peer VPNs
✅ Scalability – Supports large-scale remote sites without complex configurations
✅ Redundancy – Secondary hub for high availability and failover support
✅ Security – End-to-end encryption using IPSec and ISAKMP policies
✅ Optimized Routing – Using EIGRP with split-horizon adjustments

## Architecture Overview
The DMVPN deployment follows a Hub-and-Spoke model with:

Hub Router – Central node managing tunnels dynamically
Spoke Routers – Remote sites that establish tunnels as needed
Routing Protocol – EIGRP for dynamic route propagation
Encryption – IPSec for secure communication

# Configuration Highlights
🔹 Phase 1: Initial Setup
Basic IP addressing for WAN and LAN
Static routing for connectivity testing
🔹 Phase 2: DMVPN Tunnel Setup
Multipoint GRE (mGRE) tunnel interfaces
Next Hop Resolution Protocol (NHRP) for dynamic spoke registration
🔹 Phase 3: Dynamic Routing with EIGRP
Enable EIGRP over DMVPN tunnels
Adjust split-horizon to allow spoke-to-spoke communication
🔹 Phase 4: High Availability & Redundancy
Secondary Hub Router for failover
Redundant static mappings to ensure continuous operations
🔹 Phase 5: Security & Encryption
ISAKMP & IPSec policy implementation
DMVPN tunnel protected with IPSec profile
## Documentation & Implementation
The complete step-by-step implementation guide is available in the draft documentation included in this repository.

## Technology Stack
Cisco IOS Routers
GRE Tunneling & NHRP
EIGRP Routing Protocol
IPSec for Encryption

## Use Cases
✔ Enterprise WAN VPN – Secure branch office connectivity
✔ Cloud VPN Gateway – Connecting remote users to data centers
✔ ISP VPN Services – Scalable VPN solutions for clients

## Future Enhancements
🔹 Implement BGP over DMVPN for multi-cloud environments
🔹 Enable QoS policies for traffic prioritization
🔹 Integrate with SD-WAN solutions

### GNS3 Project Files  
Due to GitHub file size limits, the full **GNS3 portable project** is available for download here:  
📂 [Download GNS3 Project]([https://drive.google.com/your-link-here](https://drive.google.com/drive/folders/1Yqp0fCCcENL1_hVhUf3ERTgkVTS6Sarj?usp=drive_link)) 
⚠️ The file is **view-only**—please make a copy before making any modifications
