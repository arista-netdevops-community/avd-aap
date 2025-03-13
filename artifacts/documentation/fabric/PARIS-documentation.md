# PARIS

## Table of Contents

- [Fabric Switches and Management IP](#fabric-switches-and-management-ip)
  - [Fabric Switches with inband Management IP](#fabric-switches-with-inband-management-ip)
- [Fabric Topology](#fabric-topology)
- [Fabric IP Allocation](#fabric-ip-allocation)
  - [Fabric Point-To-Point Links](#fabric-point-to-point-links)
  - [Point-To-Point Links Node Allocation](#point-to-point-links-node-allocation)
  - [Loopback Interfaces (BGP EVPN Peering)](#loopback-interfaces-bgp-evpn-peering)
  - [Loopback0 Interfaces Node Allocation](#loopback0-interfaces-node-allocation)
  - [VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)](#vtep-loopback-vxlan-tunnel-source-interfaces-vteps-only)
  - [VTEP Loopback Node allocation](#vtep-loopback-node-allocation)

## Fabric Switches and Management IP

| POD | Type | Node | Management IP | Platform | Provisioned in CloudVision | Serial Number |
| --- | ---- | ---- | ------------- | -------- | -------------------------- | ------------- |
| PARIS | l3leaf | dc1-leaf1a | 172.20.1.3/16 | cEOSLab | Provisioned | MTACHEDATACENTER003 |
| PARIS | l3leaf | dc1-leaf1b | 172.20.1.4/16 | cEOSLab | Provisioned | MTACHEDATACENTER004 |
| PARIS | l3leaf | dc1-leaf2a | 172.20.1.5/16 | cEOSLab | Provisioned | MTACHEDATACENTER005 |
| PARIS | l3leaf | dc1-leaf2b | 172.20.1.6/16 | cEOSLab | Provisioned | MTACHEDATACENTER006 |
| PARIS | spine | dc1-spine1 | 172.20.1.1/16 | cEOSLab | Provisioned | MTACHEDATACENTER001 |
| PARIS | spine | dc1-spine2 | 172.20.1.2/16 | cEOSLab | Provisioned | MTACHEDATACENTER002 |

> Provision status is based on Ansible inventory declaration and do not represent real status from CloudVision.

### Fabric Switches with inband Management IP

| POD | Type | Node | Management IP | Inband Interface |
| --- | ---- | ---- | ------------- | ---------------- |

## Fabric Topology

| Type | Node | Node Interface | Peer Type | Peer Node | Peer Interface |
| ---- | ---- | -------------- | --------- | ----------| -------------- |
| l3leaf | dc1-leaf1a | Ethernet49/1 | spine | dc1-spine1 | Ethernet1/1 |
| l3leaf | dc1-leaf1a | Ethernet50/1 | spine | dc1-spine2 | Ethernet1/1 |
| l3leaf | dc1-leaf1a | Ethernet55/1 | mlag_peer | dc1-leaf1b | Ethernet55/1 |
| l3leaf | dc1-leaf1a | Ethernet56/1 | mlag_peer | dc1-leaf1b | Ethernet56/1 |
| l3leaf | dc1-leaf1b | Ethernet49/1 | spine | dc1-spine1 | Ethernet2/1 |
| l3leaf | dc1-leaf1b | Ethernet50/1 | spine | dc1-spine2 | Ethernet2/1 |
| l3leaf | dc1-leaf2a | Ethernet49/1 | spine | dc1-spine1 | Ethernet3/1 |
| l3leaf | dc1-leaf2a | Ethernet50/1 | spine | dc1-spine2 | Ethernet3/1 |
| l3leaf | dc1-leaf2a | Ethernet55/1 | mlag_peer | dc1-leaf2b | Ethernet55/1 |
| l3leaf | dc1-leaf2a | Ethernet56/1 | mlag_peer | dc1-leaf2b | Ethernet56/1 |
| l3leaf | dc1-leaf2b | Ethernet49/1 | spine | dc1-spine1 | Ethernet4/1 |
| l3leaf | dc1-leaf2b | Ethernet50/1 | spine | dc1-spine2 | Ethernet4/1 |

## Fabric IP Allocation

### Fabric Point-To-Point Links

| Uplink IPv4 Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ---------------- | ------------------- | ------------------ | ------------------ |
| 10.255.255.0/26 | 64 | 16 | 25.0 % |

### Point-To-Point Links Node Allocation

| Node | Node Interface | Node IP Address | Peer Node | Peer Interface | Peer IP Address |
| ---- | -------------- | --------------- | --------- | -------------- | --------------- |
| dc1-leaf1a | Ethernet49/1 | 10.255.255.1/31 | dc1-spine1 | Ethernet1/1 | 10.255.255.0/31 |
| dc1-leaf1a | Ethernet50/1 | 10.255.255.3/31 | dc1-spine2 | Ethernet1/1 | 10.255.255.2/31 |
| dc1-leaf1b | Ethernet49/1 | 10.255.255.5/31 | dc1-spine1 | Ethernet2/1 | 10.255.255.4/31 |
| dc1-leaf1b | Ethernet50/1 | 10.255.255.7/31 | dc1-spine2 | Ethernet2/1 | 10.255.255.6/31 |
| dc1-leaf2a | Ethernet49/1 | 10.255.255.9/31 | dc1-spine1 | Ethernet3/1 | 10.255.255.8/31 |
| dc1-leaf2a | Ethernet50/1 | 10.255.255.11/31 | dc1-spine2 | Ethernet3/1 | 10.255.255.10/31 |
| dc1-leaf2b | Ethernet49/1 | 10.255.255.13/31 | dc1-spine1 | Ethernet4/1 | 10.255.255.12/31 |
| dc1-leaf2b | Ethernet50/1 | 10.255.255.15/31 | dc1-spine2 | Ethernet4/1 | 10.255.255.14/31 |

### Loopback Interfaces (BGP EVPN Peering)

| Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------- | ------------------- | ------------------ | ------------------ |
| 10.255.0.0/27 | 32 | 6 | 18.75 % |

### Loopback0 Interfaces Node Allocation

| POD | Node | Loopback0 |
| --- | ---- | --------- |
| PARIS | dc1-leaf1a | 10.255.0.3/32 |
| PARIS | dc1-leaf1b | 10.255.0.4/32 |
| PARIS | dc1-leaf2a | 10.255.0.5/32 |
| PARIS | dc1-leaf2b | 10.255.0.6/32 |
| PARIS | dc1-spine1 | 10.255.0.1/32 |
| PARIS | dc1-spine2 | 10.255.0.2/32 |

### VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)

| VTEP Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------------ | ------------------- | ------------------ | ------------------ |
| 10.255.1.0/27 | 32 | 4 | 12.5 % |

### VTEP Loopback Node allocation

| POD | Node | Loopback1 |
| --- | ---- | --------- |
| PARIS | dc1-leaf1a | 10.255.1.3/32 |
| PARIS | dc1-leaf1b | 10.255.1.3/32 |
| PARIS | dc1-leaf2a | 10.255.1.5/32 |
| PARIS | dc1-leaf2b | 10.255.1.5/32 |
