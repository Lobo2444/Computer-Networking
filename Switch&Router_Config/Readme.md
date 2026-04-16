Demonstrating a basic multi-network topology built using Cisco Packet Tracer. The objective was to configure multiple LANs connected through a router while ensuring proper communication, interface configuration, and troubleshooting of common network issues such as duplex mismatches.



**Topology Overview**



The network consists of three separate LAN segments:



* **LAN 1 (Yellow zone):**Contains three PCs connected to a switch. This represents a small local network.
* **LAN 2 (Cyan zone):** Another group of PCs connected to a second switch, forming a separate subnet.
* **LAN 3 (Pink zone):** A third LAN with two PCs connected through a switch.



All three LANs are interconnected using a central router. Additionally, laptops are used for initial configuration and testing purposes.



**Key Configuration Tasks**

1. **Router Configuration**
* Assigned IP addresses to each router interface corresponding to different LANs
* Each interface acts as the default gateway for its respective subnet
* Ensured all interfaces are enabled (no shutdown)

**2. Switch Configuration**

* Verified interface status using show interfaces
* Adjusted speed and duplex settings where necessary
* Disabled unused ports for better network hygiene

**3. End Device Configuration**

* Assigned IP addresses manually to all PCs
* Configured subnet masks and default gateways
* Ensured each device points to the correct router interface
* Important Concepts Applied
* Duplex Mismatch Issue



A key part of this activity was identifying and preventing duplex mismatches



**Common problematic scenarios:**



* Auto vs Auto (generally works, but not always reliable)
* Manual vs Manual (must match exactly)
* Auto vs Manual (can cause mismatch issues)



**Resolution approach:**



1. Ensured consistent duplex settings across connected interfaces
2. Verified using switch and router interface status commands
3. Connectivity Verification
4. Used ping to test communication:
5. Within the same LAN
6. Across different LANs via the router
7. Confirmed end-to-end connectivity after configuration
8. Final Steps



**Saved configurations using:**



* copy running-config startup-config
* Rechecked all device configurations to ensure persistence after reload
* Outcome



**At the end of this activity:**



1. All three LANs successfully communicate through the router
2. Interface issues such as duplex mismatches were resolved
3. The network operates as expected with proper IP addressing and routing

