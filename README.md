# Modern Hotel Network Design

## Project Description

As a part of the end-year networking project, the task is to design and implement the network for Vic Modern Hotel. The hotel comprises three floors, each housing different departments. The network design should ensure efficient communication between departments, secure access, and reliable connectivity.

## Requirements

1. **Floor Layout:**
   - First Floor: Reception, Store, Logistics
   - Second Floor: Finance, HR, Sales/Marketing
   - Third Floor: IT, Admin

2. **Networking Equipment:**
   - Three routers, one for each floor, placed in the server room on the third floor.
   - Routers connected to each other using serial DCE cables.
   - Inter-router network:
     - 10.10.10.0/30
     - 10.10.10.4/30
     - 10.10.10.8/30
   - One switch per floor.
   - WiFi networks for laptops and phones on each floor.
   - Printers in each department.

3. **VLAN Configuration:**
   - First Floor:
     - Reception: VLAN 80, Network 192.168.8.0/24
     - Store: VLAN 70, Network 192.168.7.0/24
     - Logistics: VLAN 60, Network 192.168.6.0/24
   - Second Floor:
     - Finance: VLAN 50, Network 192.168.5.0/24
     - HR: VLAN 40, Network 192.168.4.0/24
     - Sales/Marketing: VLAN 30, Network 192.168.3.0/24
   - Third Floor:
     - Admin: VLAN 20, Network 192.168.2.0/24
     - IT: VLAN 10, Network 192.168.1.0/24

4. **Routing Protocol:**
   - Use OSPF for route advertisement.

5. **DHCP Configuration:**
   - Configure routers as DHCP servers.
   - Dynamic IP address allocation for all devices.

6. **SSH Configuration:**
   - Enable SSH in all routers for remote login.

7. **Port Security:**
   - Configure port security on the switch in the IT department.
   - Only allow Test-PC (connected to port fa0/1) with the sticky method for MAC address acquisition.
   - Set violation mode to shutdown.

## Technologies Implemented

- Cisco Packet Tracer for network topology creation.
- Hierarchical Network Design for scalability and manageability.
- Correct cabling for connecting networking devices.
- VLAN creation and port assignment.
- Subnetting and IP addressing for efficient address allocation.
- Inter-VLAN routing using the router-on-a-stick method.
- DHCP server configuration on routers.
- SSH configuration for secure remote access.
- Port security (switchport security) for access control.
- WLAN configuration for wireless network access (using Cisco Access Points).
- Host device configurations for network connectivity.
- Testing and verifying network communication.

## Additional Notes

- Test-PC connected to port fa0/1 in the IT department is used for remote login testing purposes.

  ![scenraio](https://github.com/YuklidD/Cisco_pkt_project3/blob/main/HMS.jpg)
