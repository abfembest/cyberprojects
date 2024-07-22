## Configuring IPv4 Static and Default Routes
# Topology
![image](https://github.com/user-attachments/assets/23b97df1-c44b-4201-96e9-24195638a2c6)
# Addressing Table
![image](https://github.com/user-attachments/assets/426d7a35-8a2f-4f28-b65f-e270ba82dcdb)
# The following steps were taken to configure the devices:

The IPs were configured on all the devices and the router with interface s0/0/0 for basic device settings, setting the IP address to 10.1.1.2 255.255.255.252, clock rate to 128000, and interface activation with R3(config-if)#no shutdown command.
For static route configurations, a recursive static route was set on R1 to 192.168.1.0/24 via 10.1.1.2, and a directly connected static route was set on R3 to 192.168.0.0/24 via s0/0/0. Static routes were removed from R1 using no ip route.
Finally, a default route was configured on R1 to 0.0.0.0/0 via s0/0/1.
