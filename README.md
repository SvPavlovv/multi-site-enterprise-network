
# Corporate Network Design and Configuration

### Cisco Packet Tracer Project

## About the Project

I created this network in Cisco Packet Tracer to improve my practical networking skills and get more experience working with Cisco devices.

The project includes a main office in Sofia and two branch offices in Plovdiv and Varna. Each office has its own local network, and the routers use OSPF to communicate between the different locations.

In the Sofia office, I separated the departments into VLANs and configured DHCP, inter-VLAN routing, and some basic security features.

## Network Configuration

The main technologies I worked with were:

- **VLANs** – to separate the departments in the Sofia office.
- **Router-on-a-Stick** – to allow communication between VLANs.
- **DHCP** – to assign IP addresses automatically from a central server.
- **OSPF** – to exchange routing information between the three offices.
- **ACLs** – to restrict guest access to internal networks.
- **Port Security** – to control MAC addresses on selected switch ports.
- **SSH** – to manage the Sofia router remotely.

## IP Addressing

| Location / Department | Network |
|---|---|
| Sofia - Management | 192.168.10.0/24 |
| Sofia - IT | 192.168.11.0/24 |
| Sofia - Sales | 192.168.12.0/24 |
| Sofia - HR | 192.168.13.0/24 |
| Sofia - Servers | 192.168.14.0/24 |
| Sofia - Guest | 192.168.15.0/24 |
| Plovdiv | 192.168.20.0/24 |
| Varna | 192.168.30.0/24 |

## Testing and Troubleshooting

After configuring the network, I tested DHCP, OSPF, connectivity between the offices, and the security settings.

Some things didn't work correctly on the first attempt, especially DHCP and SSH. I used Cisco IOS commands to check the interfaces, routing tables, VLANs, and access lists.

I successfully tested communication between Sofia and both branch offices. The guest network was also unable to reach the internal hosts I tested.

SSH access from the Management VLAN worked, although I still need to fully verify the ACL restriction for connections from branch routers.

## What I Learned

This project helped me understand how different networking technologies work together.

I became more comfortable using the Cisco CLI, checking configurations, and troubleshooting connectivity problems.

I also learned that getting devices connected is only part of the work. Testing the configuration and understanding why something doesn't work are just as important.

## Project Files

- [Cisco Packet Tracer Project](MultiSiteEnterpriseNetwork.pkt)
- [Technical Documentation (Bulgarian)](Техническа%20Документация.docx)
