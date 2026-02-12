# Replicating Network Architecture for a Government-Owned Energy Company

## Project Overview

This project focuses on replicating the real-world enterprise network architecture of a government-owned energy company using EVE-NG (Emulated Virtual Environment – Next Generation).

The lab simulates a production-grade corporate infrastructure including ISP connectivity, firewall redundancy, core switching, distribution layers, and end-user networks.

The goal of this project is to:

- Understand enterprise network design
- Simulate high-availability firewall deployment
- Implement core and distribution switching
- Replicate ISP and MPLS connectivity
- Design segmented internal networks
- Practice large-scale topology management in EVE-NG

---

## Lab Platform

This project is built using:

- EVE-NG
- Cisco 7206VXR (Dynamips)
- Sophos XG Firewall (QEMU)
- Juniper vJunos Switch (vEX)
- VPCS for end devices

---

## Network Components

The topology includes:

- ISP Router (Cisco 7206VXR)
- Primary Firewall (Sophos XG)
- Secondary Firewall (Sophos XG)
- Mini Firewall
- Juniper ISP Switch
- Core Switch 1
- Core Switch 2
- Distribution Switches
- Wireless Distribution Switch
- Multiple VLAN-based access networks
- Meeting Room Network
- Global Network simulation
- BSNL and MPLS cloud connectivity

---

## Architecture Design Highlights

- Dual firewall architecture for redundancy
- Core-distribution-access layered model
- ISP uplink simulation
- MPLS and PowerGrid external connectivity
- VLAN segmentation across multiple departments
- Multiple VPC hosts for endpoint simulation
- Wireless and meeting room network segmentation

---

## Software Requirements

To run this lab, you must install:

1. EVE-NG Community or Pro edition
2. VMware Workstation / ESXi (if running EVE as VM)
3. Required images:
   - Cisco c7200 image
   - Sophos XG Firewall image
   - Juniper vJunos Switch image
   - VPCS image

---

## How to Run This Lab

### Step 1: Install EVE-NG

Download from:

https://www.eve-ng.net/

Install it either:

- On VMware Workstation
- On ESXi
- On bare metal (recommended for performance)

---

### Step 2: Upload Device Images

Upload required images into:

/opt/unetlab/addons/


Fix permissions:

```bash
/opt/unetlab/wrappers/unl_wrapper -a fixpermissions
```

##Step 3: Import the Lab File

Upload the provided .unl file to:

/opt/unetlab/labs/

Restart EVE-NG services if required.

##Step 4: Start the Lab

-Open EVE-NG web interface
-Launch the lab
-Power on devices
-Begin configuration
-Project Objectives
-Replicate enterprise-grade network topology
-Configure routing and switching
-Implement firewall policies
-Practice VLAN configuration
-Understand ISP connectivity design
-Simulate production-level infrastructure

##Skills Demonstrated

-Enterprise Network Design
-Firewall Deployment (Sophos XG)
-Juniper Switching
-Cisco Routing
-VLAN and Layer 3 Switching
-High Availability Architecture
-Network Segmentation
-MPLS Simulation
-EVE-NG Lab Deployment

##Disclaimer

This project is created strictly for educational and training purposes.

The replicated architecture represents an energy company network design structure for learning and simulation only.

No proprietary configuration or confidential company data is included.

