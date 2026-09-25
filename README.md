# asir-virtual-network-lab-
A virtual network laboratory developed as part of my Higher Technician in Networked Computer Systems Administration (ASIR) studies.  
The laboratory was built using VirtualBox and includes a firewall, a DMZ, an internal network, a Linux server, Windows Server and a Windows client.

## Objectives

- Build a multi-network virtual infrastructure.
- Configure an external network, a DMZ and an internal network.
- Configure a Debian-based firewall.
- Practice IP addressing and routing.
- Configure NAT and traffic forwarding.
- Configure Linux and Windows systems.
- Configure SSH access.
- Test network connectivity and firewall rules.
- Document troubleshooting and configuration decisions.

## Technologies

- VirtualBox 7.2
- Debian Linux
- Windows Server
- Windows Client
- iptables
- SSH
- NAT
- TCP/IP

## Network Architecture

The laboratory consists of three separate network segments:

|  Network |        Type      |     Subnet       |
|  ------- |------------------|------------------|
| External |    NAT Network   | `203.0.113.0/24` |
|   DMZ    | Internal Network | `172.16.1.0/24`  |
| Internal | Internal Network | `192.168.60.0/24`|

## Virtual Machines

| Virtual Machine | Operating System |       Purpose       |
|-----------------|------------------|---------------------|
|   `cortafuegos` |     Debian       | Firewall and router |
|   `servidor`    |     Debian       |     DMZ server      |
| `windows-server`|   Windows Server |   Internal server   |
|`windows-cliente´|      Windows     |   Internal client   |

## Documentation

- [Network Topology](docs/01-topology.md)
- [External Network](docs/02-external-network.md)
- [DMZ](docs/03-dmz.md)
- [Internal Network](docs/04-internal-network.md)
- [Firewall](docs/05-firewall.md)
- [Connectivity Tests](docs/06-connectivity-tests.md)

## Evidence

Screenshots, configuration files and network diagrams are included
in the corresponding project directories.

## Troubleshooting

Problems encountered during the laboratory setup and their
resolution are documented in:

[Troubleshooting Notes](notes/troubleshooting.md)
