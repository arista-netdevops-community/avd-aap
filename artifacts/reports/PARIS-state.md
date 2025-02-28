# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed | Total Tests Skipped |
| ----------- | ------------------ | ------------------ | ------------------- |
| 255 | 231 | 0 | 24 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| dc1-leaf1a | 50 | 46 | 0 | 4 | - | Hardware |
| dc1-leaf1b | 49 | 45 | 0 | 4 | - | Hardware |
| dc1-leaf2a | 51 | 47 | 0 | 4 | - | Hardware |
| dc1-leaf2b | 49 | 45 | 0 | 4 | - | Hardware |
| dc1-spine1 | 28 | 24 | 0 | 4 | - | Hardware |
| dc1-spine2 | 28 | 24 | 0 | 4 | - | Hardware |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| BGP | 36 | 36 | 0 | 0 |
| Connectivity | 64 | 64 | 0 | 0 |
| Hardware | 24 | 0 | 0 | 24 |
| Interfaces | 77 | 77 | 0 | 0 |
| MLAG | 4 | 4 | 0 | 0 |
| Routing | 38 | 38 | 0 | 0 |
| System | 12 | 12 | 0 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | dc1-leaf1a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-spine1 (IP: 10.255.0.1) | PASS | - |
| 2 | dc1-leaf1a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-spine2 (IP: 10.255.0.2) | PASS | - |
| 3 | dc1-leaf1a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf1b (IP: 10.255.1.97) | PASS | - |
| 4 | dc1-leaf1a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-spine1 (IP: 10.255.255.0) | PASS | - |
| 5 | dc1-leaf1a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-spine2 (IP: 10.255.255.2) | PASS | - |
| 6 | dc1-leaf1a | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet49/1 - Remote: dc1-spine1 Ethernet1/1 | PASS | - |
| 7 | dc1-leaf1a | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet50/1 - Remote: dc1-spine2 Ethernet1/1 | PASS | - |
| 8 | dc1-leaf1a | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet55/1 - Remote: dc1-leaf1b Ethernet55/1 | PASS | - |
| 9 | dc1-leaf1a | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet56/1 - Remote: dc1-leaf1b Ethernet56/1 | PASS | - |
| 10 | dc1-leaf1a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: dc1-leaf1a Loopback0 (IP: 10.255.0.3) | PASS | - |
| 11 | dc1-leaf1a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: dc1-leaf1b Loopback0 (IP: 10.255.0.4) | PASS | - |
| 12 | dc1-leaf1a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: dc1-leaf2a Loopback0 (IP: 10.255.0.5) | PASS | - |
| 13 | dc1-leaf1a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: dc1-leaf2b Loopback0 (IP: 10.255.0.6) | PASS | - |
| 14 | dc1-leaf1a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: dc1-spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 15 | dc1-leaf1a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: dc1-spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 16 | dc1-leaf1a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet49/1 (IP: 10.255.255.1) - Destination: dc1-spine1 Ethernet1/1 (IP: 10.255.255.0) | PASS | - |
| 17 | dc1-leaf1a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet50/1 (IP: 10.255.255.3) - Destination: dc1-spine2 Ethernet1/1 (IP: 10.255.255.2) | PASS | - |
| 18 | dc1-leaf1a | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 19 | dc1-leaf1a | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 20 | dc1-leaf1a | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 21 | dc1-leaf1a | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 22 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - SERVER_server1_eth1 = 'up' | PASS | - |
| 23 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - SERVER_ixia_eth1 = 'up' | PASS | - |
| 24 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet49/1 - P2P_dc1-spine1_Ethernet1/1 = 'up' | PASS | - |
| 25 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet50/1 - P2P_dc1-spine2_Ethernet1/1 = 'up' | PASS | - |
| 26 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet55/1 - MLAG_dc1-leaf1b_Ethernet55/1 = 'up' | PASS | - |
| 27 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet56/1 - MLAG_dc1-leaf1b_Ethernet56/1 = 'up' | PASS | - |
| 28 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 29 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 30 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback10 - DIAG_VRF_Production = 'up' | PASS | - |
| 31 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - SERVER_server1 = 'up' | PASS | - |
| 32 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel551 - MLAG_dc1-leaf1b_Port-Channel551 = 'up' | PASS | - |
| 33 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan11 - Web = 'up' | PASS | - |
| 34 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan12 - Database = 'up' | PASS | - |
| 35 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_Production = 'up' | PASS | - |
| 36 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 37 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 38 | dc1-leaf1a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 39 | dc1-leaf1a | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 40 | dc1-leaf1a | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 41 | dc1-leaf1a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: dc1-spine1 | PASS | - |
| 42 | dc1-leaf1a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: dc1-spine2 | PASS | - |
| 43 | dc1-leaf1a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: dc1-leaf1a | PASS | - |
| 44 | dc1-leaf1a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: dc1-leaf1b | PASS | - |
| 45 | dc1-leaf1a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: dc1-leaf2a | PASS | - |
| 46 | dc1-leaf1a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: dc1-leaf2b | PASS | - |
| 47 | dc1-leaf1a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: dc1-leaf1a | PASS | - |
| 48 | dc1-leaf1a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: dc1-leaf2a | PASS | - |
| 49 | dc1-leaf1a | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 50 | dc1-leaf1a | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 51 | dc1-leaf1b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-spine1 (IP: 10.255.0.1) | PASS | - |
| 52 | dc1-leaf1b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-spine2 (IP: 10.255.0.2) | PASS | - |
| 53 | dc1-leaf1b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf1a (IP: 10.255.1.96) | PASS | - |
| 54 | dc1-leaf1b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-spine1 (IP: 10.255.255.4) | PASS | - |
| 55 | dc1-leaf1b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-spine2 (IP: 10.255.255.6) | PASS | - |
| 56 | dc1-leaf1b | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet49/1 - Remote: dc1-spine1 Ethernet2/1 | PASS | - |
| 57 | dc1-leaf1b | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet50/1 - Remote: dc1-spine2 Ethernet2/1 | PASS | - |
| 58 | dc1-leaf1b | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet55/1 - Remote: dc1-leaf1a Ethernet55/1 | PASS | - |
| 59 | dc1-leaf1b | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet56/1 - Remote: dc1-leaf1a Ethernet56/1 | PASS | - |
| 60 | dc1-leaf1b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: dc1-leaf1a Loopback0 (IP: 10.255.0.3) | PASS | - |
| 61 | dc1-leaf1b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: dc1-leaf1b Loopback0 (IP: 10.255.0.4) | PASS | - |
| 62 | dc1-leaf1b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: dc1-leaf2a Loopback0 (IP: 10.255.0.5) | PASS | - |
| 63 | dc1-leaf1b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: dc1-leaf2b Loopback0 (IP: 10.255.0.6) | PASS | - |
| 64 | dc1-leaf1b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: dc1-spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 65 | dc1-leaf1b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: dc1-spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 66 | dc1-leaf1b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet49/1 (IP: 10.255.255.5) - Destination: dc1-spine1 Ethernet2/1 (IP: 10.255.255.4) | PASS | - |
| 67 | dc1-leaf1b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet50/1 (IP: 10.255.255.7) - Destination: dc1-spine2 Ethernet2/1 (IP: 10.255.255.6) | PASS | - |
| 68 | dc1-leaf1b | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 69 | dc1-leaf1b | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 70 | dc1-leaf1b | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 71 | dc1-leaf1b | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 72 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - SERVER_server1_eth2 = 'up' | PASS | - |
| 73 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet49/1 - P2P_dc1-spine1_Ethernet2/1 = 'up' | PASS | - |
| 74 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet50/1 - P2P_dc1-spine2_Ethernet2/1 = 'up' | PASS | - |
| 75 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet55/1 - MLAG_dc1-leaf1a_Ethernet55/1 = 'up' | PASS | - |
| 76 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet56/1 - MLAG_dc1-leaf1a_Ethernet56/1 = 'up' | PASS | - |
| 77 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 78 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 79 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback10 - DIAG_VRF_Production = 'up' | PASS | - |
| 80 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - SERVER_server1 = 'up' | PASS | - |
| 81 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel551 - MLAG_dc1-leaf1a_Port-Channel551 = 'up' | PASS | - |
| 82 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan11 - Web = 'up' | PASS | - |
| 83 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan12 - Database = 'up' | PASS | - |
| 84 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_Production = 'up' | PASS | - |
| 85 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 86 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 87 | dc1-leaf1b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 88 | dc1-leaf1b | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 89 | dc1-leaf1b | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 90 | dc1-leaf1b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: dc1-spine1 | PASS | - |
| 91 | dc1-leaf1b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: dc1-spine2 | PASS | - |
| 92 | dc1-leaf1b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: dc1-leaf1a | PASS | - |
| 93 | dc1-leaf1b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: dc1-leaf1b | PASS | - |
| 94 | dc1-leaf1b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: dc1-leaf2a | PASS | - |
| 95 | dc1-leaf1b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: dc1-leaf2b | PASS | - |
| 96 | dc1-leaf1b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: dc1-leaf1a | PASS | - |
| 97 | dc1-leaf1b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: dc1-leaf2a | PASS | - |
| 98 | dc1-leaf1b | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 99 | dc1-leaf1b | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 100 | dc1-leaf2a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-spine1 (IP: 10.255.0.1) | PASS | - |
| 101 | dc1-leaf2a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-spine2 (IP: 10.255.0.2) | PASS | - |
| 102 | dc1-leaf2a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf2b (IP: 10.255.1.101) | PASS | - |
| 103 | dc1-leaf2a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-spine1 (IP: 10.255.255.8) | PASS | - |
| 104 | dc1-leaf2a | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-spine2 (IP: 10.255.255.10) | PASS | - |
| 105 | dc1-leaf2a | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet49/1 - Remote: dc1-spine1 Ethernet3/1 | PASS | - |
| 106 | dc1-leaf2a | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet50/1 - Remote: dc1-spine2 Ethernet3/1 | PASS | - |
| 107 | dc1-leaf2a | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet55/1 - Remote: dc1-leaf2b Ethernet55/1 | PASS | - |
| 108 | dc1-leaf2a | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet56/1 - Remote: dc1-leaf2b Ethernet56/1 | PASS | - |
| 109 | dc1-leaf2a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: dc1-leaf1a Loopback0 (IP: 10.255.0.3) | PASS | - |
| 110 | dc1-leaf2a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: dc1-leaf1b Loopback0 (IP: 10.255.0.4) | PASS | - |
| 111 | dc1-leaf2a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: dc1-leaf2a Loopback0 (IP: 10.255.0.5) | PASS | - |
| 112 | dc1-leaf2a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: dc1-leaf2b Loopback0 (IP: 10.255.0.6) | PASS | - |
| 113 | dc1-leaf2a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: dc1-spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 114 | dc1-leaf2a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: dc1-spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 115 | dc1-leaf2a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet49/1 (IP: 10.255.255.9) - Destination: dc1-spine1 Ethernet3/1 (IP: 10.255.255.8) | PASS | - |
| 116 | dc1-leaf2a | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet50/1 (IP: 10.255.255.11) - Destination: dc1-spine2 Ethernet3/1 (IP: 10.255.255.10) | PASS | - |
| 117 | dc1-leaf2a | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 118 | dc1-leaf2a | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 119 | dc1-leaf2a | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 120 | dc1-leaf2a | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 121 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - SERVER_server2_eth1 = 'up' | PASS | - |
| 122 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - SERVER_ixia_eth2 = 'up' | PASS | - |
| 123 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - SERVER_server3_Ethernet1 = 'up' | PASS | - |
| 124 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet49/1 - P2P_dc1-spine1_Ethernet3/1 = 'up' | PASS | - |
| 125 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet50/1 - P2P_dc1-spine2_Ethernet3/1 = 'up' | PASS | - |
| 126 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet55/1 - MLAG_dc1-leaf2b_Ethernet55/1 = 'up' | PASS | - |
| 127 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet56/1 - MLAG_dc1-leaf2b_Ethernet56/1 = 'up' | PASS | - |
| 128 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 129 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 130 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback10 - DIAG_VRF_Production = 'up' | PASS | - |
| 131 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - SERVER_server2 = 'up' | PASS | - |
| 132 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel551 - MLAG_dc1-leaf2b_Port-Channel551 = 'up' | PASS | - |
| 133 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan11 - Web = 'up' | PASS | - |
| 134 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan12 - Database = 'up' | PASS | - |
| 135 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_Production = 'up' | PASS | - |
| 136 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 137 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 138 | dc1-leaf2a | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 139 | dc1-leaf2a | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 140 | dc1-leaf2a | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 141 | dc1-leaf2a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: dc1-spine1 | PASS | - |
| 142 | dc1-leaf2a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: dc1-spine2 | PASS | - |
| 143 | dc1-leaf2a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: dc1-leaf1a | PASS | - |
| 144 | dc1-leaf2a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: dc1-leaf1b | PASS | - |
| 145 | dc1-leaf2a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: dc1-leaf2a | PASS | - |
| 146 | dc1-leaf2a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: dc1-leaf2b | PASS | - |
| 147 | dc1-leaf2a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: dc1-leaf1a | PASS | - |
| 148 | dc1-leaf2a | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: dc1-leaf2a | PASS | - |
| 149 | dc1-leaf2a | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 150 | dc1-leaf2a | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 151 | dc1-leaf2b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-spine1 (IP: 10.255.0.1) | PASS | - |
| 152 | dc1-leaf2b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-spine2 (IP: 10.255.0.2) | PASS | - |
| 153 | dc1-leaf2b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf2a (IP: 10.255.1.100) | PASS | - |
| 154 | dc1-leaf2b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-spine1 (IP: 10.255.255.12) | PASS | - |
| 155 | dc1-leaf2b | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-spine2 (IP: 10.255.255.14) | PASS | - |
| 156 | dc1-leaf2b | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet49/1 - Remote: dc1-spine1 Ethernet4/1 | PASS | - |
| 157 | dc1-leaf2b | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet50/1 - Remote: dc1-spine2 Ethernet4/1 | PASS | - |
| 158 | dc1-leaf2b | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet55/1 - Remote: dc1-leaf2a Ethernet55/1 | PASS | - |
| 159 | dc1-leaf2b | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet56/1 - Remote: dc1-leaf2a Ethernet56/1 | PASS | - |
| 160 | dc1-leaf2b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: dc1-leaf1a Loopback0 (IP: 10.255.0.3) | PASS | - |
| 161 | dc1-leaf2b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: dc1-leaf1b Loopback0 (IP: 10.255.0.4) | PASS | - |
| 162 | dc1-leaf2b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: dc1-leaf2a Loopback0 (IP: 10.255.0.5) | PASS | - |
| 163 | dc1-leaf2b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: dc1-leaf2b Loopback0 (IP: 10.255.0.6) | PASS | - |
| 164 | dc1-leaf2b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: dc1-spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 165 | dc1-leaf2b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: dc1-spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 166 | dc1-leaf2b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet49/1 (IP: 10.255.255.13) - Destination: dc1-spine1 Ethernet4/1 (IP: 10.255.255.12) | PASS | - |
| 167 | dc1-leaf2b | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet50/1 (IP: 10.255.255.15) - Destination: dc1-spine2 Ethernet4/1 (IP: 10.255.255.14) | PASS | - |
| 168 | dc1-leaf2b | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 169 | dc1-leaf2b | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 170 | dc1-leaf2b | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 171 | dc1-leaf2b | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 172 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - SERVER_server2_eth2 = 'up' | PASS | - |
| 173 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet49/1 - P2P_dc1-spine1_Ethernet4/1 = 'up' | PASS | - |
| 174 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet50/1 - P2P_dc1-spine2_Ethernet4/1 = 'up' | PASS | - |
| 175 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet55/1 - MLAG_dc1-leaf2a_Ethernet55/1 = 'up' | PASS | - |
| 176 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet56/1 - MLAG_dc1-leaf2a_Ethernet56/1 = 'up' | PASS | - |
| 177 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 178 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 179 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback10 - DIAG_VRF_Production = 'up' | PASS | - |
| 180 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - SERVER_server2 = 'up' | PASS | - |
| 181 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel551 - MLAG_dc1-leaf2a_Port-Channel551 = 'up' | PASS | - |
| 182 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan11 - Web = 'up' | PASS | - |
| 183 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan12 - Database = 'up' | PASS | - |
| 184 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_Production = 'up' | PASS | - |
| 185 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 186 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 187 | dc1-leaf2b | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 188 | dc1-leaf2b | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 189 | dc1-leaf2b | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 190 | dc1-leaf2b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: dc1-spine1 | PASS | - |
| 191 | dc1-leaf2b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: dc1-spine2 | PASS | - |
| 192 | dc1-leaf2b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: dc1-leaf1a | PASS | - |
| 193 | dc1-leaf2b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: dc1-leaf1b | PASS | - |
| 194 | dc1-leaf2b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: dc1-leaf2a | PASS | - |
| 195 | dc1-leaf2b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: dc1-leaf2b | PASS | - |
| 196 | dc1-leaf2b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.3 - Peer: dc1-leaf1a | PASS | - |
| 197 | dc1-leaf2b | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.1.5 - Peer: dc1-leaf2a | PASS | - |
| 198 | dc1-leaf2b | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 199 | dc1-leaf2b | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 200 | dc1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-leaf1a (IP: 10.255.0.3) | PASS | - |
| 201 | dc1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-leaf1b (IP: 10.255.0.4) | PASS | - |
| 202 | dc1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-leaf2a (IP: 10.255.0.5) | PASS | - |
| 203 | dc1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-leaf2b (IP: 10.255.0.6) | PASS | - |
| 204 | dc1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf1a (IP: 10.255.255.1) | PASS | - |
| 205 | dc1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf1b (IP: 10.255.255.5) | PASS | - |
| 206 | dc1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf2a (IP: 10.255.255.9) | PASS | - |
| 207 | dc1-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf2b (IP: 10.255.255.13) | PASS | - |
| 208 | dc1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1/1 - Remote: dc1-leaf1a Ethernet49/1 | PASS | - |
| 209 | dc1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2/1 - Remote: dc1-leaf1b Ethernet49/1 | PASS | - |
| 210 | dc1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3/1 - Remote: dc1-leaf2a Ethernet49/1 | PASS | - |
| 211 | dc1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4/1 - Remote: dc1-leaf2b Ethernet49/1 | PASS | - |
| 212 | dc1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1/1 (IP: 10.255.255.0) - Destination: dc1-leaf1a Ethernet49/1 (IP: 10.255.255.1) | PASS | - |
| 213 | dc1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2/1 (IP: 10.255.255.4) - Destination: dc1-leaf1b Ethernet49/1 (IP: 10.255.255.5) | PASS | - |
| 214 | dc1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3/1 (IP: 10.255.255.8) - Destination: dc1-leaf2a Ethernet49/1 (IP: 10.255.255.9) | PASS | - |
| 215 | dc1-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4/1 (IP: 10.255.255.12) - Destination: dc1-leaf2b Ethernet49/1 (IP: 10.255.255.13) | PASS | - |
| 216 | dc1-spine1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 217 | dc1-spine1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 218 | dc1-spine1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 219 | dc1-spine1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 220 | dc1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1/1 - P2P_dc1-leaf1a_Ethernet49/1 = 'up' | PASS | - |
| 221 | dc1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2/1 - P2P_dc1-leaf1b_Ethernet49/1 = 'up' | PASS | - |
| 222 | dc1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3/1 - P2P_dc1-leaf2a_Ethernet49/1 = 'up' | PASS | - |
| 223 | dc1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4/1 - P2P_dc1-leaf2b_Ethernet49/1 = 'up' | PASS | - |
| 224 | dc1-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 225 | dc1-spine1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 226 | dc1-spine1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 227 | dc1-spine1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 228 | dc1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-leaf1a (IP: 10.255.0.3) | PASS | - |
| 229 | dc1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-leaf1b (IP: 10.255.0.4) | PASS | - |
| 230 | dc1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-leaf2a (IP: 10.255.0.5) | PASS | - |
| 231 | dc1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: dc1-leaf2b (IP: 10.255.0.6) | PASS | - |
| 232 | dc1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf1a (IP: 10.255.255.3) | PASS | - |
| 233 | dc1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf1b (IP: 10.255.255.7) | PASS | - |
| 234 | dc1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf2a (IP: 10.255.255.11) | PASS | - |
| 235 | dc1-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: dc1-leaf2b (IP: 10.255.255.15) | PASS | - |
| 236 | dc1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1/1 - Remote: dc1-leaf1a Ethernet50/1 | PASS | - |
| 237 | dc1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2/1 - Remote: dc1-leaf1b Ethernet50/1 | PASS | - |
| 238 | dc1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3/1 - Remote: dc1-leaf2a Ethernet50/1 | PASS | - |
| 239 | dc1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4/1 - Remote: dc1-leaf2b Ethernet50/1 | PASS | - |
| 240 | dc1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1/1 (IP: 10.255.255.2) - Destination: dc1-leaf1a Ethernet50/1 (IP: 10.255.255.3) | PASS | - |
| 241 | dc1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2/1 (IP: 10.255.255.6) - Destination: dc1-leaf1b Ethernet50/1 (IP: 10.255.255.7) | PASS | - |
| 242 | dc1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3/1 (IP: 10.255.255.10) - Destination: dc1-leaf2a Ethernet50/1 (IP: 10.255.255.11) | PASS | - |
| 243 | dc1-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4/1 (IP: 10.255.255.14) - Destination: dc1-leaf2b Ethernet50/1 (IP: 10.255.255.15) | PASS | - |
| 244 | dc1-spine2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 245 | dc1-spine2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 246 | dc1-spine2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 247 | dc1-spine2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 248 | dc1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1/1 - P2P_dc1-leaf1a_Ethernet50/1 = 'up' | PASS | - |
| 249 | dc1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2/1 - P2P_dc1-leaf1b_Ethernet50/1 = 'up' | PASS | - |
| 250 | dc1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3/1 - P2P_dc1-leaf2a_Ethernet50/1 = 'up' | PASS | - |
| 251 | dc1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4/1 - P2P_dc1-leaf2b_Ethernet50/1 = 'up' | PASS | - |
| 252 | dc1-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 253 | dc1-spine2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 254 | dc1-spine2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 255 | dc1-spine2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
