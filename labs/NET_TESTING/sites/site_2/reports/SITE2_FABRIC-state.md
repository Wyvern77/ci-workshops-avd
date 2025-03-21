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
| 392 | 353 | 7 | 32 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| s2-brdr1 | 52 | 47 | 1 | 4 | System | Hardware |
| s2-brdr2 | 52 | 47 | 1 | 4 | System | Hardware |
| s2-leaf1 | 53 | 49 | 0 | 4 | - | Hardware |
| s2-leaf2 | 53 | 48 | 1 | 4 | System | Hardware |
| s2-leaf3 | 53 | 48 | 1 | 4 | System | Hardware |
| s2-leaf4 | 53 | 48 | 1 | 4 | System | Hardware |
| s2-spine1 | 38 | 33 | 1 | 4 | System | Hardware |
| s2-spine2 | 38 | 33 | 1 | 4 | System | Hardware |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| BGP | 54 | 54 | 0 | 0 |
| Connectivity | 108 | 108 | 0 | 0 |
| Hardware | 32 | 0 | 0 | 32 |
| Interfaces | 102 | 102 | 0 | 0 |
| MLAG | 6 | 6 | 0 | 0 |
| Routing | 74 | 74 | 0 | 0 |
| System | 16 | 9 | 7 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 52 | s2-brdr1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 104 | s2-brdr2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 210 | s2-leaf2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 263 | s2-leaf3 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 316 | s2-leaf4 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 354 | s2-spine1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 392 | s2-spine2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | s2-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine1 (IP: 10.250.2.1) | PASS | - |
| 2 | s2-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine2 (IP: 10.250.2.2) | PASS | - |
| 3 | s2-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-brdr2 (IP: 10.252.2.9) | PASS | - |
| 4 | s2-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine1 (IP: 172.16.2.16) | PASS | - |
| 5 | s2-brdr1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine2 (IP: 172.16.2.18) | PASS | - |
| 6 | s2-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s2-brdr2 Ethernet1 | PASS | - |
| 7 | s2-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s2-spine1 Ethernet7 | PASS | - |
| 8 | s2-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s2-spine2 Ethernet7 | PASS | - |
| 9 | s2-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s2-brdr2 Ethernet6 | PASS | - |
| 10 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.7) - Destination: s2-brdr1 Loopback0 (IP: 10.250.2.7) | PASS | - |
| 11 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.7) - Destination: s2-brdr2 Loopback0 (IP: 10.250.2.8) | PASS | - |
| 12 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.7) - Destination: s2-leaf1 Loopback0 (IP: 10.250.2.3) | PASS | - |
| 13 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.7) - Destination: s2-leaf2 Loopback0 (IP: 10.250.2.4) | PASS | - |
| 14 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.7) - Destination: s2-leaf3 Loopback0 (IP: 10.250.2.5) | PASS | - |
| 15 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.7) - Destination: s2-leaf4 Loopback0 (IP: 10.250.2.6) | PASS | - |
| 16 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.7) - Destination: s2-spine1 Loopback0 (IP: 10.250.2.1) | PASS | - |
| 17 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.7) - Destination: s2-spine2 Loopback0 (IP: 10.250.2.2) | PASS | - |
| 18 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.2.17) - Destination: s2-spine1 Ethernet7 (IP: 172.16.2.16) | PASS | - |
| 19 | s2-brdr1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.2.19) - Destination: s2-spine2 Ethernet7 (IP: 172.16.2.18) | PASS | - |
| 20 | s2-brdr1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 21 | s2-brdr1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 22 | s2-brdr1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 23 | s2-brdr1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 24 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s2-brdr2_Ethernet1 = 'up' | PASS | - |
| 25 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s2-spine1_Ethernet7 = 'up' | PASS | - |
| 26 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s2-spine2_Ethernet7 = 'up' | PASS | - |
| 27 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_s1-brdr1_Ethernet4 = 'up' | PASS | - |
| 28 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s2-brdr2_Ethernet6 = 'up' | PASS | - |
| 29 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 30 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 31 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s2-brdr2_Port-Channel1 = 'up' | PASS | - |
| 32 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 33 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 34 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 35 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 36 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 37 | s2-brdr1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 38 | s2-brdr1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 39 | s2-brdr1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 40 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.1 - Peer: s2-spine1 | PASS | - |
| 41 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.2 - Peer: s2-spine2 | PASS | - |
| 42 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.3 - Peer: s2-leaf1 | PASS | - |
| 43 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.4 - Peer: s2-leaf2 | PASS | - |
| 44 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.5 - Peer: s2-leaf3 | PASS | - |
| 45 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.6 - Peer: s2-leaf4 | PASS | - |
| 46 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.7 - Peer: s2-brdr1 | PASS | - |
| 47 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.8 - Peer: s2-brdr2 | PASS | - |
| 48 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.3 - Peer: s2-leaf1 | PASS | - |
| 49 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.5 - Peer: s2-leaf3 | PASS | - |
| 50 | s2-brdr1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.7 - Peer: s2-brdr1 | PASS | - |
| 51 | s2-brdr1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 52 | s2-brdr1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 53 | s2-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine1 (IP: 10.250.2.1) | PASS | - |
| 54 | s2-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine2 (IP: 10.250.2.2) | PASS | - |
| 55 | s2-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-brdr1 (IP: 10.252.2.8) | PASS | - |
| 56 | s2-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine1 (IP: 172.16.2.20) | PASS | - |
| 57 | s2-brdr2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine2 (IP: 172.16.2.22) | PASS | - |
| 58 | s2-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s2-brdr1 Ethernet1 | PASS | - |
| 59 | s2-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s2-spine1 Ethernet8 | PASS | - |
| 60 | s2-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s2-spine2 Ethernet8 | PASS | - |
| 61 | s2-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s2-brdr1 Ethernet6 | PASS | - |
| 62 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.8) - Destination: s2-brdr1 Loopback0 (IP: 10.250.2.7) | PASS | - |
| 63 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.8) - Destination: s2-brdr2 Loopback0 (IP: 10.250.2.8) | PASS | - |
| 64 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.8) - Destination: s2-leaf1 Loopback0 (IP: 10.250.2.3) | PASS | - |
| 65 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.8) - Destination: s2-leaf2 Loopback0 (IP: 10.250.2.4) | PASS | - |
| 66 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.8) - Destination: s2-leaf3 Loopback0 (IP: 10.250.2.5) | PASS | - |
| 67 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.8) - Destination: s2-leaf4 Loopback0 (IP: 10.250.2.6) | PASS | - |
| 68 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.8) - Destination: s2-spine1 Loopback0 (IP: 10.250.2.1) | PASS | - |
| 69 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.8) - Destination: s2-spine2 Loopback0 (IP: 10.250.2.2) | PASS | - |
| 70 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.2.21) - Destination: s2-spine1 Ethernet8 (IP: 172.16.2.20) | PASS | - |
| 71 | s2-brdr2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.2.23) - Destination: s2-spine2 Ethernet8 (IP: 172.16.2.22) | PASS | - |
| 72 | s2-brdr2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 73 | s2-brdr2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 74 | s2-brdr2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 75 | s2-brdr2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 76 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s2-brdr1_Ethernet1 = 'up' | PASS | - |
| 77 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s2-spine1_Ethernet8 = 'up' | PASS | - |
| 78 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s2-spine2_Ethernet8 = 'up' | PASS | - |
| 79 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_s1-brdr2_Ethernet5 = 'up' | PASS | - |
| 80 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s2-brdr1_Ethernet6 = 'up' | PASS | - |
| 81 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 82 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 83 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s2-brdr1_Port-Channel1 = 'up' | PASS | - |
| 84 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 85 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 86 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 87 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 88 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 89 | s2-brdr2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 90 | s2-brdr2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 91 | s2-brdr2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 92 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.1 - Peer: s2-spine1 | PASS | - |
| 93 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.2 - Peer: s2-spine2 | PASS | - |
| 94 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.3 - Peer: s2-leaf1 | PASS | - |
| 95 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.4 - Peer: s2-leaf2 | PASS | - |
| 96 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.5 - Peer: s2-leaf3 | PASS | - |
| 97 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.6 - Peer: s2-leaf4 | PASS | - |
| 98 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.7 - Peer: s2-brdr1 | PASS | - |
| 99 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.8 - Peer: s2-brdr2 | PASS | - |
| 100 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.3 - Peer: s2-leaf1 | PASS | - |
| 101 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.5 - Peer: s2-leaf3 | PASS | - |
| 102 | s2-brdr2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.7 - Peer: s2-brdr1 | PASS | - |
| 103 | s2-brdr2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 104 | s2-brdr2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 105 | s2-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine1 (IP: 10.250.2.1) | PASS | - |
| 106 | s2-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine2 (IP: 10.250.2.2) | PASS | - |
| 107 | s2-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf2 (IP: 10.252.2.1) | PASS | - |
| 108 | s2-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine1 (IP: 172.16.2.0) | PASS | - |
| 109 | s2-leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine2 (IP: 172.16.2.2) | PASS | - |
| 110 | s2-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s2-leaf2 Ethernet1 | PASS | - |
| 111 | s2-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s2-spine1 Ethernet2 | PASS | - |
| 112 | s2-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s2-spine2 Ethernet2 | PASS | - |
| 113 | s2-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s2-leaf2 Ethernet6 | PASS | - |
| 114 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.3) - Destination: s2-brdr1 Loopback0 (IP: 10.250.2.7) | PASS | - |
| 115 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.3) - Destination: s2-brdr2 Loopback0 (IP: 10.250.2.8) | PASS | - |
| 116 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.3) - Destination: s2-leaf1 Loopback0 (IP: 10.250.2.3) | PASS | - |
| 117 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.3) - Destination: s2-leaf2 Loopback0 (IP: 10.250.2.4) | PASS | - |
| 118 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.3) - Destination: s2-leaf3 Loopback0 (IP: 10.250.2.5) | PASS | - |
| 119 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.3) - Destination: s2-leaf4 Loopback0 (IP: 10.250.2.6) | PASS | - |
| 120 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.3) - Destination: s2-spine1 Loopback0 (IP: 10.250.2.1) | PASS | - |
| 121 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.3) - Destination: s2-spine2 Loopback0 (IP: 10.250.2.2) | PASS | - |
| 122 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.2.1) - Destination: s2-spine1 Ethernet2 (IP: 172.16.2.0) | PASS | - |
| 123 | s2-leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.2.3) - Destination: s2-spine2 Ethernet2 (IP: 172.16.2.2) | PASS | - |
| 124 | s2-leaf1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 125 | s2-leaf1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 126 | s2-leaf1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 127 | s2-leaf1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 128 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s2-leaf2_Ethernet1 = 'up' | PASS | - |
| 129 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s2-spine1_Ethernet2 = 'up' | PASS | - |
| 130 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s2-spine2_Ethernet2 = 'up' | PASS | - |
| 131 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s2-host1_eth1 = 'up' | PASS | - |
| 132 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s2-leaf2_Ethernet6 = 'up' | PASS | - |
| 133 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 134 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 135 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s2-leaf2_Port-Channel1 = 'up' | PASS | - |
| 136 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s2-host1 = 'up' | PASS | - |
| 137 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 138 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 139 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 140 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 141 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 142 | s2-leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 143 | s2-leaf1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 144 | s2-leaf1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 145 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.1 - Peer: s2-spine1 | PASS | - |
| 146 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.2 - Peer: s2-spine2 | PASS | - |
| 147 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.3 - Peer: s2-leaf1 | PASS | - |
| 148 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.4 - Peer: s2-leaf2 | PASS | - |
| 149 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.5 - Peer: s2-leaf3 | PASS | - |
| 150 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.6 - Peer: s2-leaf4 | PASS | - |
| 151 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.7 - Peer: s2-brdr1 | PASS | - |
| 152 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.8 - Peer: s2-brdr2 | PASS | - |
| 153 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.3 - Peer: s2-leaf1 | PASS | - |
| 154 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.5 - Peer: s2-leaf3 | PASS | - |
| 155 | s2-leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.7 - Peer: s2-brdr1 | PASS | - |
| 156 | s2-leaf1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 157 | s2-leaf1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 158 | s2-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine1 (IP: 10.250.2.1) | PASS | - |
| 159 | s2-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine2 (IP: 10.250.2.2) | PASS | - |
| 160 | s2-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf1 (IP: 10.252.2.0) | PASS | - |
| 161 | s2-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine1 (IP: 172.16.2.4) | PASS | - |
| 162 | s2-leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine2 (IP: 172.16.2.6) | PASS | - |
| 163 | s2-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s2-leaf1 Ethernet1 | PASS | - |
| 164 | s2-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s2-spine1 Ethernet3 | PASS | - |
| 165 | s2-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s2-spine2 Ethernet3 | PASS | - |
| 166 | s2-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s2-leaf1 Ethernet6 | PASS | - |
| 167 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.4) - Destination: s2-brdr1 Loopback0 (IP: 10.250.2.7) | PASS | - |
| 168 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.4) - Destination: s2-brdr2 Loopback0 (IP: 10.250.2.8) | PASS | - |
| 169 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.4) - Destination: s2-leaf1 Loopback0 (IP: 10.250.2.3) | PASS | - |
| 170 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.4) - Destination: s2-leaf2 Loopback0 (IP: 10.250.2.4) | PASS | - |
| 171 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.4) - Destination: s2-leaf3 Loopback0 (IP: 10.250.2.5) | PASS | - |
| 172 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.4) - Destination: s2-leaf4 Loopback0 (IP: 10.250.2.6) | PASS | - |
| 173 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.4) - Destination: s2-spine1 Loopback0 (IP: 10.250.2.1) | PASS | - |
| 174 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.4) - Destination: s2-spine2 Loopback0 (IP: 10.250.2.2) | PASS | - |
| 175 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.2.5) - Destination: s2-spine1 Ethernet3 (IP: 172.16.2.4) | PASS | - |
| 176 | s2-leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.2.7) - Destination: s2-spine2 Ethernet3 (IP: 172.16.2.6) | PASS | - |
| 177 | s2-leaf2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 178 | s2-leaf2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 179 | s2-leaf2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 180 | s2-leaf2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 181 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s2-leaf1_Ethernet1 = 'up' | PASS | - |
| 182 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s2-spine1_Ethernet3 = 'up' | PASS | - |
| 183 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s2-spine2_Ethernet3 = 'up' | PASS | - |
| 184 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s2-host1_eth2 = 'up' | PASS | - |
| 185 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s2-leaf1_Ethernet6 = 'up' | PASS | - |
| 186 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 187 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 188 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s2-leaf1_Port-Channel1 = 'up' | PASS | - |
| 189 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s2-host1 = 'up' | PASS | - |
| 190 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 191 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 192 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 193 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 194 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 195 | s2-leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 196 | s2-leaf2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 197 | s2-leaf2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 198 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.1 - Peer: s2-spine1 | PASS | - |
| 199 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.2 - Peer: s2-spine2 | PASS | - |
| 200 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.3 - Peer: s2-leaf1 | PASS | - |
| 201 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.4 - Peer: s2-leaf2 | PASS | - |
| 202 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.5 - Peer: s2-leaf3 | PASS | - |
| 203 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.6 - Peer: s2-leaf4 | PASS | - |
| 204 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.7 - Peer: s2-brdr1 | PASS | - |
| 205 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.8 - Peer: s2-brdr2 | PASS | - |
| 206 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.3 - Peer: s2-leaf1 | PASS | - |
| 207 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.5 - Peer: s2-leaf3 | PASS | - |
| 208 | s2-leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.7 - Peer: s2-brdr1 | PASS | - |
| 209 | s2-leaf2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 210 | s2-leaf2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 211 | s2-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine1 (IP: 10.250.2.1) | PASS | - |
| 212 | s2-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine2 (IP: 10.250.2.2) | PASS | - |
| 213 | s2-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf4 (IP: 10.252.2.5) | PASS | - |
| 214 | s2-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine1 (IP: 172.16.2.8) | PASS | - |
| 215 | s2-leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine2 (IP: 172.16.2.10) | PASS | - |
| 216 | s2-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s2-leaf4 Ethernet1 | PASS | - |
| 217 | s2-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s2-spine1 Ethernet4 | PASS | - |
| 218 | s2-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s2-spine2 Ethernet4 | PASS | - |
| 219 | s2-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s2-leaf4 Ethernet6 | PASS | - |
| 220 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.5) - Destination: s2-brdr1 Loopback0 (IP: 10.250.2.7) | PASS | - |
| 221 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.5) - Destination: s2-brdr2 Loopback0 (IP: 10.250.2.8) | PASS | - |
| 222 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.5) - Destination: s2-leaf1 Loopback0 (IP: 10.250.2.3) | PASS | - |
| 223 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.5) - Destination: s2-leaf2 Loopback0 (IP: 10.250.2.4) | PASS | - |
| 224 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.5) - Destination: s2-leaf3 Loopback0 (IP: 10.250.2.5) | PASS | - |
| 225 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.5) - Destination: s2-leaf4 Loopback0 (IP: 10.250.2.6) | PASS | - |
| 226 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.5) - Destination: s2-spine1 Loopback0 (IP: 10.250.2.1) | PASS | - |
| 227 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.5) - Destination: s2-spine2 Loopback0 (IP: 10.250.2.2) | PASS | - |
| 228 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.2.9) - Destination: s2-spine1 Ethernet4 (IP: 172.16.2.8) | PASS | - |
| 229 | s2-leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.2.11) - Destination: s2-spine2 Ethernet4 (IP: 172.16.2.10) | PASS | - |
| 230 | s2-leaf3 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 231 | s2-leaf3 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 232 | s2-leaf3 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 233 | s2-leaf3 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 234 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s2-leaf4_Ethernet1 = 'up' | PASS | - |
| 235 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s2-spine1_Ethernet4 = 'up' | PASS | - |
| 236 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s2-spine2_Ethernet4 = 'up' | PASS | - |
| 237 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s2-host2_eth1 = 'up' | PASS | - |
| 238 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s2-leaf4_Ethernet6 = 'up' | PASS | - |
| 239 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 240 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 241 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s2-leaf4_Port-Channel1 = 'up' | PASS | - |
| 242 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s2-host2 = 'up' | PASS | - |
| 243 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 244 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 245 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 246 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 247 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 248 | s2-leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 249 | s2-leaf3 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 250 | s2-leaf3 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 251 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.1 - Peer: s2-spine1 | PASS | - |
| 252 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.2 - Peer: s2-spine2 | PASS | - |
| 253 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.3 - Peer: s2-leaf1 | PASS | - |
| 254 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.4 - Peer: s2-leaf2 | PASS | - |
| 255 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.5 - Peer: s2-leaf3 | PASS | - |
| 256 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.6 - Peer: s2-leaf4 | PASS | - |
| 257 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.7 - Peer: s2-brdr1 | PASS | - |
| 258 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.8 - Peer: s2-brdr2 | PASS | - |
| 259 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.3 - Peer: s2-leaf1 | PASS | - |
| 260 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.5 - Peer: s2-leaf3 | PASS | - |
| 261 | s2-leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.7 - Peer: s2-brdr1 | PASS | - |
| 262 | s2-leaf3 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 263 | s2-leaf3 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 264 | s2-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine1 (IP: 10.250.2.1) | PASS | - |
| 265 | s2-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-spine2 (IP: 10.250.2.2) | PASS | - |
| 266 | s2-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf3 (IP: 10.252.2.4) | PASS | - |
| 267 | s2-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine1 (IP: 172.16.2.12) | PASS | - |
| 268 | s2-leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-spine2 (IP: 172.16.2.14) | PASS | - |
| 269 | s2-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: s2-leaf3 Ethernet1 | PASS | - |
| 270 | s2-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s2-spine1 Ethernet5 | PASS | - |
| 271 | s2-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s2-spine2 Ethernet5 | PASS | - |
| 272 | s2-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: s2-leaf3 Ethernet6 | PASS | - |
| 273 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.6) - Destination: s2-brdr1 Loopback0 (IP: 10.250.2.7) | PASS | - |
| 274 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.6) - Destination: s2-brdr2 Loopback0 (IP: 10.250.2.8) | PASS | - |
| 275 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.6) - Destination: s2-leaf1 Loopback0 (IP: 10.250.2.3) | PASS | - |
| 276 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.6) - Destination: s2-leaf2 Loopback0 (IP: 10.250.2.4) | PASS | - |
| 277 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.6) - Destination: s2-leaf3 Loopback0 (IP: 10.250.2.5) | PASS | - |
| 278 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.6) - Destination: s2-leaf4 Loopback0 (IP: 10.250.2.6) | PASS | - |
| 279 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.6) - Destination: s2-spine1 Loopback0 (IP: 10.250.2.1) | PASS | - |
| 280 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.250.2.6) - Destination: s2-spine2 Loopback0 (IP: 10.250.2.2) | PASS | - |
| 281 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.2.13) - Destination: s2-spine1 Ethernet5 (IP: 172.16.2.12) | PASS | - |
| 282 | s2-leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.2.15) - Destination: s2-spine2 Ethernet5 (IP: 172.16.2.14) | PASS | - |
| 283 | s2-leaf4 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 284 | s2-leaf4 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 285 | s2-leaf4 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 286 | s2-leaf4 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 287 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - MLAG_s2-leaf3_Ethernet1 = 'up' | PASS | - |
| 288 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s2-spine1_Ethernet5 = 'up' | PASS | - |
| 289 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s2-spine2_Ethernet5 = 'up' | PASS | - |
| 290 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - SERVER_s2-host2_eth2 = 'up' | PASS | - |
| 291 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - MLAG_s2-leaf3_Ethernet6 = 'up' | PASS | - |
| 292 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 293 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 294 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel1 - MLAG_s2-leaf3_Port-Channel1 = 'up' | PASS | - |
| 295 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel4 - SERVER_s2-host2 = 'up' | PASS | - |
| 296 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan10 - Ten = 'up' | PASS | - |
| 297 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan20 - Twenty = 'up' | PASS | - |
| 298 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_OVERLAY = 'up' | PASS | - |
| 299 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 300 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 301 | s2-leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 302 | s2-leaf4 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 303 | s2-leaf4 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 304 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.1 - Peer: s2-spine1 | PASS | - |
| 305 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.2 - Peer: s2-spine2 | PASS | - |
| 306 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.3 - Peer: s2-leaf1 | PASS | - |
| 307 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.4 - Peer: s2-leaf2 | PASS | - |
| 308 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.5 - Peer: s2-leaf3 | PASS | - |
| 309 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.6 - Peer: s2-leaf4 | PASS | - |
| 310 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.7 - Peer: s2-brdr1 | PASS | - |
| 311 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.250.2.8 - Peer: s2-brdr2 | PASS | - |
| 312 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.3 - Peer: s2-leaf1 | PASS | - |
| 313 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.5 - Peer: s2-leaf3 | PASS | - |
| 314 | s2-leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.2.7 - Peer: s2-brdr1 | PASS | - |
| 315 | s2-leaf4 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 316 | s2-leaf4 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 317 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-brdr1 (IP: 10.250.2.7) | PASS | - |
| 318 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-brdr2 (IP: 10.250.2.8) | PASS | - |
| 319 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-leaf1 (IP: 10.250.2.3) | PASS | - |
| 320 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-leaf2 (IP: 10.250.2.4) | PASS | - |
| 321 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-leaf3 (IP: 10.250.2.5) | PASS | - |
| 322 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-leaf4 (IP: 10.250.2.6) | PASS | - |
| 323 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-brdr1 (IP: 172.16.2.17) | PASS | - |
| 324 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-brdr2 (IP: 172.16.2.21) | PASS | - |
| 325 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf1 (IP: 172.16.2.1) | PASS | - |
| 326 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf2 (IP: 172.16.2.5) | PASS | - |
| 327 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf3 (IP: 172.16.2.9) | PASS | - |
| 328 | s2-spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf4 (IP: 172.16.2.13) | PASS | - |
| 329 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s2-leaf1 Ethernet2 | PASS | - |
| 330 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s2-leaf2 Ethernet2 | PASS | - |
| 331 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: s2-leaf3 Ethernet2 | PASS | - |
| 332 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: s2-leaf4 Ethernet2 | PASS | - |
| 333 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet7 - Remote: s2-brdr1 Ethernet2 | PASS | - |
| 334 | s2-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet8 - Remote: s2-brdr2 Ethernet2 | PASS | - |
| 335 | s2-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.2.0) - Destination: s2-leaf1 Ethernet2 (IP: 172.16.2.1) | PASS | - |
| 336 | s2-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.2.4) - Destination: s2-leaf2 Ethernet2 (IP: 172.16.2.5) | PASS | - |
| 337 | s2-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4 (IP: 172.16.2.8) - Destination: s2-leaf3 Ethernet2 (IP: 172.16.2.9) | PASS | - |
| 338 | s2-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet5 (IP: 172.16.2.12) - Destination: s2-leaf4 Ethernet2 (IP: 172.16.2.13) | PASS | - |
| 339 | s2-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet7 (IP: 172.16.2.16) - Destination: s2-brdr1 Ethernet2 (IP: 172.16.2.17) | PASS | - |
| 340 | s2-spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet8 (IP: 172.16.2.20) - Destination: s2-brdr2 Ethernet2 (IP: 172.16.2.21) | PASS | - |
| 341 | s2-spine1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 342 | s2-spine1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 343 | s2-spine1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 344 | s2-spine1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 345 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s2-leaf1_Ethernet2 = 'up' | PASS | - |
| 346 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s2-leaf2_Ethernet2 = 'up' | PASS | - |
| 347 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_s2-leaf3_Ethernet2 = 'up' | PASS | - |
| 348 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_s2-leaf4_Ethernet2 = 'up' | PASS | - |
| 349 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet7 - P2P_s2-brdr1_Ethernet2 = 'up' | PASS | - |
| 350 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet8 - P2P_s2-brdr2_Ethernet2 = 'up' | PASS | - |
| 351 | s2-spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 352 | s2-spine1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 353 | s2-spine1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 354 | s2-spine1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
| 355 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-brdr1 (IP: 10.250.2.7) | PASS | - |
| 356 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-brdr2 (IP: 10.250.2.8) | PASS | - |
| 357 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-leaf1 (IP: 10.250.2.3) | PASS | - |
| 358 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-leaf2 (IP: 10.250.2.4) | PASS | - |
| 359 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-leaf3 (IP: 10.250.2.5) | PASS | - |
| 360 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: s2-leaf4 (IP: 10.250.2.6) | PASS | - |
| 361 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-brdr1 (IP: 172.16.2.19) | PASS | - |
| 362 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-brdr2 (IP: 172.16.2.23) | PASS | - |
| 363 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf1 (IP: 172.16.2.3) | PASS | - |
| 364 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf2 (IP: 172.16.2.7) | PASS | - |
| 365 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf3 (IP: 172.16.2.11) | PASS | - |
| 366 | s2-spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: s2-leaf4 (IP: 172.16.2.15) | PASS | - |
| 367 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: s2-leaf1 Ethernet3 | PASS | - |
| 368 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: s2-leaf2 Ethernet3 | PASS | - |
| 369 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: s2-leaf3 Ethernet3 | PASS | - |
| 370 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: s2-leaf4 Ethernet3 | PASS | - |
| 371 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet7 - Remote: s2-brdr1 Ethernet3 | PASS | - |
| 372 | s2-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet8 - Remote: s2-brdr2 Ethernet3 | PASS | - |
| 373 | s2-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 172.16.2.2) - Destination: s2-leaf1 Ethernet3 (IP: 172.16.2.3) | PASS | - |
| 374 | s2-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 172.16.2.6) - Destination: s2-leaf2 Ethernet3 (IP: 172.16.2.7) | PASS | - |
| 375 | s2-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4 (IP: 172.16.2.10) - Destination: s2-leaf3 Ethernet3 (IP: 172.16.2.11) | PASS | - |
| 376 | s2-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet5 (IP: 172.16.2.14) - Destination: s2-leaf4 Ethernet3 (IP: 172.16.2.15) | PASS | - |
| 377 | s2-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet7 (IP: 172.16.2.18) - Destination: s2-brdr1 Ethernet3 (IP: 172.16.2.19) | PASS | - |
| 378 | s2-spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet8 (IP: 172.16.2.22) - Destination: s2-brdr2 Ethernet3 (IP: 172.16.2.23) | PASS | - |
| 379 | s2-spine2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab. |
| 380 | s2-spine2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab. |
| 381 | s2-spine2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab. |
| 382 | s2-spine2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab. |
| 383 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_s2-leaf1_Ethernet3 = 'up' | PASS | - |
| 384 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_s2-leaf2_Ethernet3 = 'up' | PASS | - |
| 385 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_s2-leaf3_Ethernet3 = 'up' | PASS | - |
| 386 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_s2-leaf4_Ethernet3 = 'up' | PASS | - |
| 387 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet7 - P2P_s2-brdr1_Ethernet3 = 'up' | PASS | - |
| 388 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet8 - P2P_s2-brdr2_Ethernet3 = 'up' | PASS | - |
| 389 | s2-spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 390 | s2-spine2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 391 | s2-spine2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | PASS | - |
| 392 | s2-spine2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | FAIL | Reload cause is: 'System reloaded due to Zero Touch Provisioning' |
