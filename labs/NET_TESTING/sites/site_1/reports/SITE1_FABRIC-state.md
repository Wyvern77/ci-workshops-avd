# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed |
| ----------- | ------------------ | ------------------ |
| 356 | 344 | 12 |

### Summary Totals Devices Under Tests

| DUT | Total Tests | Tests Passed | Tests Failed | Categories Failed |
| --- | ----------- | ------------ | ------------ | ----------------- |
| s1-brdr1 |  49 | 43 | 6 | LLDP Topology, IP Reachability, BGP |
| s1-brdr2 |  49 | 49 | 0 | - |
| s1-leaf1 |  48 | 48 | 0 | - |
| s1-leaf2 |  48 | 48 | 0 | - |
| s1-leaf3 |  48 | 48 | 0 | - |
| s1-leaf4 |  48 | 48 | 0 | - |
| s1-spine1 |  33 | 30 | 3 | LLDP Topology, IP Reachability, BGP |
| s1-spine2 |  33 | 30 | 3 | LLDP Topology, IP Reachability, BGP |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed |
| ------------- | ----------- | ------------ | ------------ |
| NTP |  8 | 8 | 0 |
| Interface State |  102 | 102 | 0 |
| LLDP Topology |  36 | 32 | 4 |
| MLAG |  6 | 6 | 0 |
| IP Reachability |  24 | 20 | 4 |
| BGP |  66 | 62 | 4 |
| Routing Table |  66 | 66 | 0 |
| Loopback0 Reachability |  48 | 48 | 0 |

## Failed Test Results Summary

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 113 | s1-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet6 | FAIL | s1-spine1.atd.lab - Ethernet7 |
| 114 | s1-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet6 | FAIL | s1-spine2.atd.lab - Ethernet7 |
| 139 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-brdr1_Ethernet2 | FAIL | s1-spine2.atd.lab - Ethernet6 |
| 145 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-brdr1_Ethernet3 | FAIL | s1-spine1.atd.lab - Ethernet6 |
| 153 | s1-brdr1 | IP Reachability | ip reachability test p2p links | Source: s1-brdr1_Ethernet2 - Destination: s1-spine1_Ethernet6 | FAIL | 100% packet loss |
| 154 | s1-brdr1 | IP Reachability | ip reachability test p2p links | Source: s1-brdr1_Ethernet3 - Destination: s1-spine2_Ethernet6 | FAIL | 100% packet loss |
| 169 | s1-spine1 | IP Reachability | ip reachability test p2p links | Source: s1-spine1_Ethernet6 - Destination: s1-brdr1_Ethernet2 | FAIL | 100% packet loss |
| 175 | s1-spine2 | IP Reachability | ip reachability test p2p links | Source: s1-spine2_Ethernet6 - Destination: s1-brdr1_Ethernet3 | FAIL | 100% packet loss |
| 186 | s1-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.16 | FAIL | Session state Active |
| 187 | s1-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.18 | FAIL | Session state Active |
| 209 | s1-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.17 | FAIL | Session state Active |
| 215 | s1-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.19 | FAIL | Session state Active |

## All Test Results

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 1 | s1-brdr1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 2 | s1-brdr2 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 3 | s1-leaf1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 4 | s1-leaf2 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 5 | s1-leaf3 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 6 | s1-leaf4 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 7 | s1-spine1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 8 | s1-spine2 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 9 | s1-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-brdr2_Ethernet1 | PASS | - |
| 10 | s1-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-brdr2_Ethernet6 | PASS | - |
| 11 | s1-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S1-SPINE1_Ethernet6 | PASS | - |
| 12 | s1-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S1-SPINE2_Ethernet6 | PASS | - |
| 13 | s1-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_s2-brdr1_Ethernet4 | PASS | - |
| 14 | s1-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-brdr1_Ethernet1 | PASS | - |
| 15 | s1-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-brdr1_Ethernet6 | PASS | - |
| 16 | s1-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S1-SPINE1_Ethernet8 | PASS | - |
| 17 | s1-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S1-SPINE2_Ethernet8 | PASS | - |
| 18 | s1-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_s2-brdr2_Ethernet5 | PASS | - |
| 19 | s1-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-leaf2_Ethernet1 | PASS | - |
| 20 | s1-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-leaf2_Ethernet6 | PASS | - |
| 21 | s1-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S1-SPINE1_Ethernet2 | PASS | - |
| 22 | s1-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S1-SPINE2_Ethernet2 | PASS | - |
| 23 | s1-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - s1-host1_eth1 | PASS | - |
| 24 | s1-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-leaf1_Ethernet1 | PASS | - |
| 25 | s1-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-leaf1_Ethernet6 | PASS | - |
| 26 | s1-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S1-SPINE1_Ethernet3 | PASS | - |
| 27 | s1-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S1-SPINE2_Ethernet3 | PASS | - |
| 28 | s1-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - s1-host1_eth2 | PASS | - |
| 29 | s1-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-leaf4_Ethernet1 | PASS | - |
| 30 | s1-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-leaf4_Ethernet6 | PASS | - |
| 31 | s1-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S1-SPINE1_Ethernet4 | PASS | - |
| 32 | s1-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S1-SPINE2_Ethernet4 | PASS | - |
| 33 | s1-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - s1-host2_eth1 | PASS | - |
| 34 | s1-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s1-leaf3_Ethernet1 | PASS | - |
| 35 | s1-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s1-leaf3_Ethernet6 | PASS | - |
| 36 | s1-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S1-SPINE1_Ethernet5 | PASS | - |
| 37 | s1-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S1-SPINE2_Ethernet5 | PASS | - |
| 38 | s1-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - s1-host2_eth2 | PASS | - |
| 39 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S1-LEAF1_Ethernet2 | PASS | - |
| 40 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S1-LEAF2_Ethernet2 | PASS | - |
| 41 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_S1-LEAF3_Ethernet2 | PASS | - |
| 42 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_S1-LEAF4_Ethernet2 | PASS | - |
| 43 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - P2P_LINK_TO_S1-BRDR1_Ethernet2 | PASS | - |
| 44 | s1-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet8 - P2P_LINK_TO_S1-BRDR2_Ethernet2 | PASS | - |
| 45 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S1-LEAF1_Ethernet3 | PASS | - |
| 46 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S1-LEAF2_Ethernet3 | PASS | - |
| 47 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_S1-LEAF3_Ethernet3 | PASS | - |
| 48 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_S1-LEAF4_Ethernet3 | PASS | - |
| 49 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - P2P_LINK_TO_S1-BRDR1_Ethernet3 | PASS | - |
| 50 | s1-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet8 - P2P_LINK_TO_S1-BRDR2_Ethernet3 | PASS | - |
| 51 | s1-brdr1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-brdr2_Po1 | PASS | - |
| 52 | s1-brdr2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-brdr1_Po1 | PASS | - |
| 53 | s1-leaf1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-leaf2_Po1 | PASS | - |
| 54 | s1-leaf1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - s1-host1 | PASS | - |
| 55 | s1-leaf2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-leaf1_Po1 | PASS | - |
| 56 | s1-leaf2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - s1-host1 | PASS | - |
| 57 | s1-leaf3 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-leaf4_Po1 | PASS | - |
| 58 | s1-leaf3 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - s1-host2 | PASS | - |
| 59 | s1-leaf4 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s1-leaf3_Po1 | PASS | - |
| 60 | s1-leaf4 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - s1-host2 | PASS | - |
| 61 | s1-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 62 | s1-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 63 | s1-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 64 | s1-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 65 | s1-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 66 | s1-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 67 | s1-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 68 | s1-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 69 | s1-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 70 | s1-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 71 | s1-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 72 | s1-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 73 | s1-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 74 | s1-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 75 | s1-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 76 | s1-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 77 | s1-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 78 | s1-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 79 | s1-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 80 | s1-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 81 | s1-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 82 | s1-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 83 | s1-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 84 | s1-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 85 | s1-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 86 | s1-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 87 | s1-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 88 | s1-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 89 | s1-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 90 | s1-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 91 | s1-brdr1 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 92 | s1-brdr2 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 93 | s1-leaf1 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 94 | s1-leaf2 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 95 | s1-leaf3 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 96 | s1-leaf4 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 97 | s1-brdr1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 98 | s1-brdr1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 99 | s1-brdr2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 100 | s1-brdr2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 101 | s1-leaf1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 102 | s1-leaf1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 103 | s1-leaf2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 104 | s1-leaf2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 105 | s1-leaf3 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 106 | s1-leaf3 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 107 | s1-leaf4 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 108 | s1-leaf4 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 109 | s1-spine1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 110 | s1-spine2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 111 | s1-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-brdr2_Ethernet1 | PASS | - |
| 112 | s1-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-brdr2_Ethernet6 | PASS | - |
| 113 | s1-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet6 | FAIL | s1-spine1.atd.lab - Ethernet7 |
| 114 | s1-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet6 | FAIL | s1-spine2.atd.lab - Ethernet7 |
| 115 | s1-brdr2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-brdr1_Ethernet1 | PASS | - |
| 116 | s1-brdr2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-brdr1_Ethernet6 | PASS | - |
| 117 | s1-brdr2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet8 | PASS | - |
| 118 | s1-brdr2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet8 | PASS | - |
| 119 | s1-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-leaf2_Ethernet1 | PASS | - |
| 120 | s1-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-leaf2_Ethernet6 | PASS | - |
| 121 | s1-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet2 | PASS | - |
| 122 | s1-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet2 | PASS | - |
| 123 | s1-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-leaf1_Ethernet1 | PASS | - |
| 124 | s1-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-leaf1_Ethernet6 | PASS | - |
| 125 | s1-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet3 | PASS | - |
| 126 | s1-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet3 | PASS | - |
| 127 | s1-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-leaf4_Ethernet1 | PASS | - |
| 128 | s1-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-leaf4_Ethernet6 | PASS | - |
| 129 | s1-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet4 | PASS | - |
| 130 | s1-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet4 | PASS | - |
| 131 | s1-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s1-leaf3_Ethernet1 | PASS | - |
| 132 | s1-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-leaf3_Ethernet6 | PASS | - |
| 133 | s1-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-spine1_Ethernet5 | PASS | - |
| 134 | s1-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-spine2_Ethernet5 | PASS | - |
| 135 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-leaf1_Ethernet2 | PASS | - |
| 136 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-leaf2_Ethernet2 | PASS | - |
| 137 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: s1-leaf3_Ethernet2 | PASS | - |
| 138 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: s1-leaf4_Ethernet2 | PASS | - |
| 139 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-brdr1_Ethernet2 | FAIL | s1-spine2.atd.lab - Ethernet6 |
| 140 | s1-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet8 - remote: s1-brdr2_Ethernet2 | PASS | - |
| 141 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s1-leaf1_Ethernet3 | PASS | - |
| 142 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s1-leaf2_Ethernet3 | PASS | - |
| 143 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: s1-leaf3_Ethernet3 | PASS | - |
| 144 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: s1-leaf4_Ethernet3 | PASS | - |
| 145 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s1-brdr1_Ethernet3 | FAIL | s1-spine1.atd.lab - Ethernet6 |
| 146 | s1-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet8 - remote: s1-brdr2_Ethernet3 | PASS | - |
| 147 | s1-brdr1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 148 | s1-brdr2 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 149 | s1-leaf1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 150 | s1-leaf2 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 151 | s1-leaf3 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 152 | s1-leaf4 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 153 | s1-brdr1 | IP Reachability | ip reachability test p2p links | Source: s1-brdr1_Ethernet2 - Destination: s1-spine1_Ethernet6 | FAIL | 100% packet loss |
| 154 | s1-brdr1 | IP Reachability | ip reachability test p2p links | Source: s1-brdr1_Ethernet3 - Destination: s1-spine2_Ethernet6 | FAIL | 100% packet loss |
| 155 | s1-brdr2 | IP Reachability | ip reachability test p2p links | Source: s1-brdr2_Ethernet2 - Destination: s1-spine1_Ethernet8 | PASS | - |
| 156 | s1-brdr2 | IP Reachability | ip reachability test p2p links | Source: s1-brdr2_Ethernet3 - Destination: s1-spine2_Ethernet8 | PASS | - |
| 157 | s1-leaf1 | IP Reachability | ip reachability test p2p links | Source: s1-leaf1_Ethernet2 - Destination: s1-spine1_Ethernet2 | PASS | - |
| 158 | s1-leaf1 | IP Reachability | ip reachability test p2p links | Source: s1-leaf1_Ethernet3 - Destination: s1-spine2_Ethernet2 | PASS | - |
| 159 | s1-leaf2 | IP Reachability | ip reachability test p2p links | Source: s1-leaf2_Ethernet2 - Destination: s1-spine1_Ethernet3 | PASS | - |
| 160 | s1-leaf2 | IP Reachability | ip reachability test p2p links | Source: s1-leaf2_Ethernet3 - Destination: s1-spine2_Ethernet3 | PASS | - |
| 161 | s1-leaf3 | IP Reachability | ip reachability test p2p links | Source: s1-leaf3_Ethernet2 - Destination: s1-spine1_Ethernet4 | PASS | - |
| 162 | s1-leaf3 | IP Reachability | ip reachability test p2p links | Source: s1-leaf3_Ethernet3 - Destination: s1-spine2_Ethernet4 | PASS | - |
| 163 | s1-leaf4 | IP Reachability | ip reachability test p2p links | Source: s1-leaf4_Ethernet2 - Destination: s1-spine1_Ethernet5 | PASS | - |
| 164 | s1-leaf4 | IP Reachability | ip reachability test p2p links | Source: s1-leaf4_Ethernet3 - Destination: s1-spine2_Ethernet5 | PASS | - |
| 165 | s1-spine1 | IP Reachability | ip reachability test p2p links | Source: s1-spine1_Ethernet2 - Destination: s1-leaf1_Ethernet2 | PASS | - |
| 166 | s1-spine1 | IP Reachability | ip reachability test p2p links | Source: s1-spine1_Ethernet3 - Destination: s1-leaf2_Ethernet2 | PASS | - |
| 167 | s1-spine1 | IP Reachability | ip reachability test p2p links | Source: s1-spine1_Ethernet4 - Destination: s1-leaf3_Ethernet2 | PASS | - |
| 168 | s1-spine1 | IP Reachability | ip reachability test p2p links | Source: s1-spine1_Ethernet5 - Destination: s1-leaf4_Ethernet2 | PASS | - |
| 169 | s1-spine1 | IP Reachability | ip reachability test p2p links | Source: s1-spine1_Ethernet6 - Destination: s1-brdr1_Ethernet2 | FAIL | 100% packet loss |
| 170 | s1-spine1 | IP Reachability | ip reachability test p2p links | Source: s1-spine1_Ethernet8 - Destination: s1-brdr2_Ethernet2 | PASS | - |
| 171 | s1-spine2 | IP Reachability | ip reachability test p2p links | Source: s1-spine2_Ethernet2 - Destination: s1-leaf1_Ethernet3 | PASS | - |
| 172 | s1-spine2 | IP Reachability | ip reachability test p2p links | Source: s1-spine2_Ethernet3 - Destination: s1-leaf2_Ethernet3 | PASS | - |
| 173 | s1-spine2 | IP Reachability | ip reachability test p2p links | Source: s1-spine2_Ethernet4 - Destination: s1-leaf3_Ethernet3 | PASS | - |
| 174 | s1-spine2 | IP Reachability | ip reachability test p2p links | Source: s1-spine2_Ethernet5 - Destination: s1-leaf4_Ethernet3 | PASS | - |
| 175 | s1-spine2 | IP Reachability | ip reachability test p2p links | Source: s1-spine2_Ethernet6 - Destination: s1-brdr1_Ethernet3 | FAIL | 100% packet loss |
| 176 | s1-spine2 | IP Reachability | ip reachability test p2p links | Source: s1-spine2_Ethernet8 - Destination: s1-brdr2_Ethernet3 | PASS | - |
| 177 | s1-brdr1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 178 | s1-brdr2 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 179 | s1-leaf1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 180 | s1-leaf2 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 181 | s1-leaf3 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 182 | s1-leaf4 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 183 | s1-spine1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 184 | s1-spine2 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 185 | s1-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.1.9 | PASS | - |
| 186 | s1-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.16 | FAIL | Session state Active |
| 187 | s1-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.18 | FAIL | Session state Active |
| 188 | s1-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.255.1 | PASS | - |
| 189 | s1-brdr2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.1.8 | PASS | - |
| 190 | s1-brdr2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.20 | PASS | - |
| 191 | s1-brdr2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.22 | PASS | - |
| 192 | s1-brdr2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.255.3 | PASS | - |
| 193 | s1-leaf1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.1.1 | PASS | - |
| 194 | s1-leaf1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.0 | PASS | - |
| 195 | s1-leaf1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.2 | PASS | - |
| 196 | s1-leaf2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.1.0 | PASS | - |
| 197 | s1-leaf2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.4 | PASS | - |
| 198 | s1-leaf2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.6 | PASS | - |
| 199 | s1-leaf3 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.1.5 | PASS | - |
| 200 | s1-leaf3 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.8 | PASS | - |
| 201 | s1-leaf3 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.10 | PASS | - |
| 202 | s1-leaf4 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.1.4 | PASS | - |
| 203 | s1-leaf4 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.12 | PASS | - |
| 204 | s1-leaf4 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.14 | PASS | - |
| 205 | s1-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.1 | PASS | - |
| 206 | s1-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.5 | PASS | - |
| 207 | s1-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.9 | PASS | - |
| 208 | s1-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.13 | PASS | - |
| 209 | s1-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.17 | FAIL | Session state Active |
| 210 | s1-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.21 | PASS | - |
| 211 | s1-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.3 | PASS | - |
| 212 | s1-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.7 | PASS | - |
| 213 | s1-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.11 | PASS | - |
| 214 | s1-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.15 | PASS | - |
| 215 | s1-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.19 | FAIL | Session state Active |
| 216 | s1-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.1.23 | PASS | - |
| 217 | s1-brdr1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.1 | PASS | - |
| 218 | s1-brdr1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.2 | PASS | - |
| 219 | s1-brdr1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.7 | PASS | - |
| 220 | s1-brdr2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.1 | PASS | - |
| 221 | s1-brdr2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.2 | PASS | - |
| 222 | s1-brdr2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.8 | PASS | - |
| 223 | s1-leaf1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.1 | PASS | - |
| 224 | s1-leaf1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.2 | PASS | - |
| 225 | s1-leaf2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.1 | PASS | - |
| 226 | s1-leaf2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.2 | PASS | - |
| 227 | s1-leaf3 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.1 | PASS | - |
| 228 | s1-leaf3 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.2 | PASS | - |
| 229 | s1-leaf4 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.1 | PASS | - |
| 230 | s1-leaf4 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.2 | PASS | - |
| 231 | s1-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.7 | PASS | - |
| 232 | s1-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.8 | PASS | - |
| 233 | s1-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.3 | PASS | - |
| 234 | s1-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.4 | PASS | - |
| 235 | s1-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.5 | PASS | - |
| 236 | s1-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.6 | PASS | - |
| 237 | s1-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.7 | PASS | - |
| 238 | s1-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.8 | PASS | - |
| 239 | s1-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.3 | PASS | - |
| 240 | s1-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.4 | PASS | - |
| 241 | s1-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.5 | PASS | - |
| 242 | s1-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.6 | PASS | - |
| 243 | s1-brdr1 | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 244 | s1-brdr1 | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 245 | s1-brdr1 | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 246 | s1-brdr2 | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 247 | s1-brdr2 | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 248 | s1-brdr2 | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 249 | s1-leaf1 | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 250 | s1-leaf1 | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 251 | s1-leaf1 | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 252 | s1-leaf2 | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 253 | s1-leaf2 | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 254 | s1-leaf2 | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 255 | s1-leaf3 | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 256 | s1-leaf3 | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 257 | s1-leaf3 | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 258 | s1-leaf4 | Routing Table | Remote VTEP address | 10.255.1.7 | PASS | - |
| 259 | s1-leaf4 | Routing Table | Remote VTEP address | 10.255.1.3 | PASS | - |
| 260 | s1-leaf4 | Routing Table | Remote VTEP address | 10.255.1.5 | PASS | - |
| 261 | s1-brdr1 | Routing Table | Remote Lo0 address | 10.250.1.7 | PASS | - |
| 262 | s1-brdr1 | Routing Table | Remote Lo0 address | 10.250.1.8 | PASS | - |
| 263 | s1-brdr1 | Routing Table | Remote Lo0 address | 10.250.1.3 | PASS | - |
| 264 | s1-brdr1 | Routing Table | Remote Lo0 address | 10.250.1.4 | PASS | - |
| 265 | s1-brdr1 | Routing Table | Remote Lo0 address | 10.250.1.5 | PASS | - |
| 266 | s1-brdr1 | Routing Table | Remote Lo0 address | 10.250.1.6 | PASS | - |
| 267 | s1-brdr1 | Routing Table | Remote Lo0 address | 10.250.1.1 | PASS | - |
| 268 | s1-brdr1 | Routing Table | Remote Lo0 address | 10.250.1.2 | PASS | - |
| 269 | s1-brdr2 | Routing Table | Remote Lo0 address | 10.250.1.7 | PASS | - |
| 270 | s1-brdr2 | Routing Table | Remote Lo0 address | 10.250.1.8 | PASS | - |
| 271 | s1-brdr2 | Routing Table | Remote Lo0 address | 10.250.1.3 | PASS | - |
| 272 | s1-brdr2 | Routing Table | Remote Lo0 address | 10.250.1.4 | PASS | - |
| 273 | s1-brdr2 | Routing Table | Remote Lo0 address | 10.250.1.5 | PASS | - |
| 274 | s1-brdr2 | Routing Table | Remote Lo0 address | 10.250.1.6 | PASS | - |
| 275 | s1-brdr2 | Routing Table | Remote Lo0 address | 10.250.1.1 | PASS | - |
| 276 | s1-brdr2 | Routing Table | Remote Lo0 address | 10.250.1.2 | PASS | - |
| 277 | s1-leaf1 | Routing Table | Remote Lo0 address | 10.250.1.7 | PASS | - |
| 278 | s1-leaf1 | Routing Table | Remote Lo0 address | 10.250.1.8 | PASS | - |
| 279 | s1-leaf1 | Routing Table | Remote Lo0 address | 10.250.1.3 | PASS | - |
| 280 | s1-leaf1 | Routing Table | Remote Lo0 address | 10.250.1.4 | PASS | - |
| 281 | s1-leaf1 | Routing Table | Remote Lo0 address | 10.250.1.5 | PASS | - |
| 282 | s1-leaf1 | Routing Table | Remote Lo0 address | 10.250.1.6 | PASS | - |
| 283 | s1-leaf1 | Routing Table | Remote Lo0 address | 10.250.1.1 | PASS | - |
| 284 | s1-leaf1 | Routing Table | Remote Lo0 address | 10.250.1.2 | PASS | - |
| 285 | s1-leaf2 | Routing Table | Remote Lo0 address | 10.250.1.7 | PASS | - |
| 286 | s1-leaf2 | Routing Table | Remote Lo0 address | 10.250.1.8 | PASS | - |
| 287 | s1-leaf2 | Routing Table | Remote Lo0 address | 10.250.1.3 | PASS | - |
| 288 | s1-leaf2 | Routing Table | Remote Lo0 address | 10.250.1.4 | PASS | - |
| 289 | s1-leaf2 | Routing Table | Remote Lo0 address | 10.250.1.5 | PASS | - |
| 290 | s1-leaf2 | Routing Table | Remote Lo0 address | 10.250.1.6 | PASS | - |
| 291 | s1-leaf2 | Routing Table | Remote Lo0 address | 10.250.1.1 | PASS | - |
| 292 | s1-leaf2 | Routing Table | Remote Lo0 address | 10.250.1.2 | PASS | - |
| 293 | s1-leaf3 | Routing Table | Remote Lo0 address | 10.250.1.7 | PASS | - |
| 294 | s1-leaf3 | Routing Table | Remote Lo0 address | 10.250.1.8 | PASS | - |
| 295 | s1-leaf3 | Routing Table | Remote Lo0 address | 10.250.1.3 | PASS | - |
| 296 | s1-leaf3 | Routing Table | Remote Lo0 address | 10.250.1.4 | PASS | - |
| 297 | s1-leaf3 | Routing Table | Remote Lo0 address | 10.250.1.5 | PASS | - |
| 298 | s1-leaf3 | Routing Table | Remote Lo0 address | 10.250.1.6 | PASS | - |
| 299 | s1-leaf3 | Routing Table | Remote Lo0 address | 10.250.1.1 | PASS | - |
| 300 | s1-leaf3 | Routing Table | Remote Lo0 address | 10.250.1.2 | PASS | - |
| 301 | s1-leaf4 | Routing Table | Remote Lo0 address | 10.250.1.7 | PASS | - |
| 302 | s1-leaf4 | Routing Table | Remote Lo0 address | 10.250.1.8 | PASS | - |
| 303 | s1-leaf4 | Routing Table | Remote Lo0 address | 10.250.1.3 | PASS | - |
| 304 | s1-leaf4 | Routing Table | Remote Lo0 address | 10.250.1.4 | PASS | - |
| 305 | s1-leaf4 | Routing Table | Remote Lo0 address | 10.250.1.5 | PASS | - |
| 306 | s1-leaf4 | Routing Table | Remote Lo0 address | 10.250.1.6 | PASS | - |
| 307 | s1-leaf4 | Routing Table | Remote Lo0 address | 10.250.1.1 | PASS | - |
| 308 | s1-leaf4 | Routing Table | Remote Lo0 address | 10.250.1.2 | PASS | - |
| 309 | s1-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr1 - 10.250.1.7 Destination: 10.250.1.7 | PASS | - |
| 310 | s1-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr1 - 10.250.1.7 Destination: 10.250.1.8 | PASS | - |
| 311 | s1-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr1 - 10.250.1.7 Destination: 10.250.1.3 | PASS | - |
| 312 | s1-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr1 - 10.250.1.7 Destination: 10.250.1.4 | PASS | - |
| 313 | s1-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr1 - 10.250.1.7 Destination: 10.250.1.5 | PASS | - |
| 314 | s1-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr1 - 10.250.1.7 Destination: 10.250.1.6 | PASS | - |
| 315 | s1-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr1 - 10.250.1.7 Destination: 10.250.1.1 | PASS | - |
| 316 | s1-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr1 - 10.250.1.7 Destination: 10.250.1.2 | PASS | - |
| 317 | s1-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr2 - 10.250.1.8 Destination: 10.250.1.7 | PASS | - |
| 318 | s1-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr2 - 10.250.1.8 Destination: 10.250.1.8 | PASS | - |
| 319 | s1-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr2 - 10.250.1.8 Destination: 10.250.1.3 | PASS | - |
| 320 | s1-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr2 - 10.250.1.8 Destination: 10.250.1.4 | PASS | - |
| 321 | s1-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr2 - 10.250.1.8 Destination: 10.250.1.5 | PASS | - |
| 322 | s1-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr2 - 10.250.1.8 Destination: 10.250.1.6 | PASS | - |
| 323 | s1-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr2 - 10.250.1.8 Destination: 10.250.1.1 | PASS | - |
| 324 | s1-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-brdr2 - 10.250.1.8 Destination: 10.250.1.2 | PASS | - |
| 325 | s1-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf1 - 10.250.1.3 Destination: 10.250.1.7 | PASS | - |
| 326 | s1-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf1 - 10.250.1.3 Destination: 10.250.1.8 | PASS | - |
| 327 | s1-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf1 - 10.250.1.3 Destination: 10.250.1.3 | PASS | - |
| 328 | s1-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf1 - 10.250.1.3 Destination: 10.250.1.4 | PASS | - |
| 329 | s1-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf1 - 10.250.1.3 Destination: 10.250.1.5 | PASS | - |
| 330 | s1-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf1 - 10.250.1.3 Destination: 10.250.1.6 | PASS | - |
| 331 | s1-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf1 - 10.250.1.3 Destination: 10.250.1.1 | PASS | - |
| 332 | s1-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf1 - 10.250.1.3 Destination: 10.250.1.2 | PASS | - |
| 333 | s1-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf2 - 10.250.1.4 Destination: 10.250.1.7 | PASS | - |
| 334 | s1-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf2 - 10.250.1.4 Destination: 10.250.1.8 | PASS | - |
| 335 | s1-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf2 - 10.250.1.4 Destination: 10.250.1.3 | PASS | - |
| 336 | s1-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf2 - 10.250.1.4 Destination: 10.250.1.4 | PASS | - |
| 337 | s1-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf2 - 10.250.1.4 Destination: 10.250.1.5 | PASS | - |
| 338 | s1-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf2 - 10.250.1.4 Destination: 10.250.1.6 | PASS | - |
| 339 | s1-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf2 - 10.250.1.4 Destination: 10.250.1.1 | PASS | - |
| 340 | s1-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf2 - 10.250.1.4 Destination: 10.250.1.2 | PASS | - |
| 341 | s1-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf3 - 10.250.1.5 Destination: 10.250.1.7 | PASS | - |
| 342 | s1-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf3 - 10.250.1.5 Destination: 10.250.1.8 | PASS | - |
| 343 | s1-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf3 - 10.250.1.5 Destination: 10.250.1.3 | PASS | - |
| 344 | s1-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf3 - 10.250.1.5 Destination: 10.250.1.4 | PASS | - |
| 345 | s1-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf3 - 10.250.1.5 Destination: 10.250.1.5 | PASS | - |
| 346 | s1-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf3 - 10.250.1.5 Destination: 10.250.1.6 | PASS | - |
| 347 | s1-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf3 - 10.250.1.5 Destination: 10.250.1.1 | PASS | - |
| 348 | s1-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf3 - 10.250.1.5 Destination: 10.250.1.2 | PASS | - |
| 349 | s1-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf4 - 10.250.1.6 Destination: 10.250.1.7 | PASS | - |
| 350 | s1-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf4 - 10.250.1.6 Destination: 10.250.1.8 | PASS | - |
| 351 | s1-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf4 - 10.250.1.6 Destination: 10.250.1.3 | PASS | - |
| 352 | s1-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf4 - 10.250.1.6 Destination: 10.250.1.4 | PASS | - |
| 353 | s1-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf4 - 10.250.1.6 Destination: 10.250.1.5 | PASS | - |
| 354 | s1-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf4 - 10.250.1.6 Destination: 10.250.1.6 | PASS | - |
| 355 | s1-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf4 - 10.250.1.6 Destination: 10.250.1.1 | PASS | - |
| 356 | s1-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s1-leaf4 - 10.250.1.6 Destination: 10.250.1.2 | PASS | - |
