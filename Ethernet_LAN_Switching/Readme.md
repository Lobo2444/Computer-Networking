ARP and ICMP Flow Simulation in Cisco Packet Tracer



**Objective:**

* Understand ARP resolution before the ICMP Transmission
* Observe MAC Learning Behavior in a layer 2 switch
* Validating packet flow using simulation mode to understand Broadcast and Unicast Frame



**Topology**:

* 4PCs
* 2 switches
* Copper Straight through and Cross Over Cable



IP Configured in every PCs

Desktop ---> Ip config --> 192.168....







**What Happens in this Network**

1. In a Fresh Network the switches doesn't know the destination of the other device
2. So from PC 1 from source Mac address an ARP request will be sent to find the Unknown devices with know Ip address of the destination device **(the request is Broadcast)**
3. Then the PC which IP matches will receive it and send a ARP reply which is a **Unicast reply** then the switch will learn the MAC address of the destination device.
4. Here switch 1 will do broadcast if the request comes from its network and switch 2 will do unicast to reply because it knows the destination already when it got when the destination was source address
5. Then sending ping request(ICMP) from pc 1 and 2 to 3 and 4 all mac address will be learnt by switch
6. Then verifying it by accessing switch CLI in real time using remote access(ssh/Telnet)
7. Use "show mac address-table" in previlage mode in switch CLI
