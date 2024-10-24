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
| 356 | 356 | 0 |

### Summary Totals Devices Under Tests

| DUT | Total Tests | Tests Passed | Tests Failed | Categories Failed |
| --- | ----------- | ------------ | ------------ | ----------------- |
| s2-brdr1 |  49 | 49 | 0 | - |
| s2-brdr2 |  49 | 49 | 0 | - |
| s2-leaf1 |  48 | 48 | 0 | - |
| s2-leaf2 |  48 | 48 | 0 | - |
| s2-leaf3 |  48 | 48 | 0 | - |
| s2-leaf4 |  48 | 48 | 0 | - |
| s2-spine1 |  33 | 33 | 0 | - |
| s2-spine2 |  33 | 33 | 0 | - |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed |
| ------------- | ----------- | ------------ | ------------ |
| NTP |  8 | 8 | 0 |
| Interface State |  102 | 102 | 0 |
| LLDP Topology |  36 | 36 | 0 |
| MLAG |  6 | 6 | 0 |
| IP Reachability |  24 | 24 | 0 |
| BGP |  66 | 66 | 0 |
| Routing Table |  66 | 66 | 0 |
| Loopback0 Reachability |  48 | 48 | 0 |

## Failed Test Results Summary

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |

## All Test Results

| Test ID | Node | Test Category | Test Description | Test | Test Result | Failure Reason |
| ------- | ---- | ------------- | ---------------- | ---- | ----------- | -------------- |
| 1 | s2-brdr1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 2 | s2-brdr2 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 3 | s2-leaf1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 4 | s2-leaf2 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 5 | s2-leaf3 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 6 | s2-leaf4 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 7 | s2-spine1 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 8 | s2-spine2 | NTP | Synchronised with NTP server | NTP | PASS | - |
| 9 | s2-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s2-brdr2_Ethernet1 | PASS | - |
| 10 | s2-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s2-brdr2_Ethernet6 | PASS | - |
| 11 | s2-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S2-SPINE1_Ethernet7 | PASS | - |
| 12 | s2-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S2-SPINE2_Ethernet7 | PASS | - |
| 13 | s2-brdr1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_s1-brdr1_Ethernet4 | PASS | - |
| 14 | s2-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s2-brdr1_Ethernet1 | PASS | - |
| 15 | s2-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s2-brdr1_Ethernet6 | PASS | - |
| 16 | s2-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S2-SPINE1_Ethernet8 | PASS | - |
| 17 | s2-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S2-SPINE2_Ethernet8 | PASS | - |
| 18 | s2-brdr2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_s1-brdr2_Ethernet5 | PASS | - |
| 19 | s2-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s2-leaf2_Ethernet1 | PASS | - |
| 20 | s2-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s2-leaf2_Ethernet6 | PASS | - |
| 21 | s2-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S2-SPINE1_Ethernet2 | PASS | - |
| 22 | s2-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S2-SPINE2_Ethernet2 | PASS | - |
| 23 | s2-leaf1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - s2-host1_eth1 | PASS | - |
| 24 | s2-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s2-leaf1_Ethernet1 | PASS | - |
| 25 | s2-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s2-leaf1_Ethernet6 | PASS | - |
| 26 | s2-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S2-SPINE1_Ethernet3 | PASS | - |
| 27 | s2-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S2-SPINE2_Ethernet3 | PASS | - |
| 28 | s2-leaf2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - s2-host1_eth2 | PASS | - |
| 29 | s2-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s2-leaf4_Ethernet1 | PASS | - |
| 30 | s2-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s2-leaf4_Ethernet6 | PASS | - |
| 31 | s2-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S2-SPINE1_Ethernet4 | PASS | - |
| 32 | s2-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S2-SPINE2_Ethernet4 | PASS | - |
| 33 | s2-leaf3 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - s2-host2_eth1 | PASS | - |
| 34 | s2-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet1 - MLAG_PEER_s2-leaf3_Ethernet1 | PASS | - |
| 35 | s2-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet6 - MLAG_PEER_s2-leaf3_Ethernet6 | PASS | - |
| 36 | s2-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S2-SPINE1_Ethernet5 | PASS | - |
| 37 | s2-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S2-SPINE2_Ethernet5 | PASS | - |
| 38 | s2-leaf4 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - s2-host2_eth2 | PASS | - |
| 39 | s2-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S2-LEAF1_Ethernet2 | PASS | - |
| 40 | s2-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S2-LEAF2_Ethernet2 | PASS | - |
| 41 | s2-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_S2-LEAF3_Ethernet2 | PASS | - |
| 42 | s2-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_S2-LEAF4_Ethernet2 | PASS | - |
| 43 | s2-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet7 - P2P_LINK_TO_S2-BRDR1_Ethernet2 | PASS | - |
| 44 | s2-spine1 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet8 - P2P_LINK_TO_S2-BRDR2_Ethernet2 | PASS | - |
| 45 | s2-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet2 - P2P_LINK_TO_S2-LEAF1_Ethernet3 | PASS | - |
| 46 | s2-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet3 - P2P_LINK_TO_S2-LEAF2_Ethernet3 | PASS | - |
| 47 | s2-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet4 - P2P_LINK_TO_S2-LEAF3_Ethernet3 | PASS | - |
| 48 | s2-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet5 - P2P_LINK_TO_S2-LEAF4_Ethernet3 | PASS | - |
| 49 | s2-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet7 - P2P_LINK_TO_S2-BRDR1_Ethernet3 | PASS | - |
| 50 | s2-spine2 | Interface State | Ethernet Interface & Line Protocol == "up" | Ethernet8 - P2P_LINK_TO_S2-BRDR2_Ethernet3 | PASS | - |
| 51 | s2-brdr1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s2-brdr2_Po1 | PASS | - |
| 52 | s2-brdr2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s2-brdr1_Po1 | PASS | - |
| 53 | s2-leaf1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s2-leaf2_Po1 | PASS | - |
| 54 | s2-leaf1 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - s2-host1 | PASS | - |
| 55 | s2-leaf2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s2-leaf1_Po1 | PASS | - |
| 56 | s2-leaf2 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - s2-host1 | PASS | - |
| 57 | s2-leaf3 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s2-leaf4_Po1 | PASS | - |
| 58 | s2-leaf3 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - s2-host2 | PASS | - |
| 59 | s2-leaf4 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel1 - MLAG_PEER_s2-leaf3_Po1 | PASS | - |
| 60 | s2-leaf4 | Interface State | Port-Channel Interface & Line Protocol == "up" | Port-Channel4 - s2-host2 | PASS | - |
| 61 | s2-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 62 | s2-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 63 | s2-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 64 | s2-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 65 | s2-brdr1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 66 | s2-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 67 | s2-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 68 | s2-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 69 | s2-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 70 | s2-brdr2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 71 | s2-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 72 | s2-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 73 | s2-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 74 | s2-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 75 | s2-leaf1 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 76 | s2-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 77 | s2-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 78 | s2-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 79 | s2-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 80 | s2-leaf2 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 81 | s2-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 82 | s2-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 83 | s2-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 84 | s2-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 85 | s2-leaf3 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 86 | s2-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4093 - MLAG_PEER_L3_PEERING | PASS | - |
| 87 | s2-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan4094 - MLAG_PEER | PASS | - |
| 88 | s2-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan10 - Ten | PASS | - |
| 89 | s2-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan20 - Twenty | PASS | - |
| 90 | s2-leaf4 | Interface State | Vlan Interface & Line Protocol == "up" | Vlan3009 - MLAG_PEER_L3_iBGP: vrf OVERLAY | PASS | - |
| 91 | s2-brdr1 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 92 | s2-brdr2 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 93 | s2-leaf1 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 94 | s2-leaf2 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 95 | s2-leaf3 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 96 | s2-leaf4 | Interface State | Vxlan Interface Status & Line Protocol == "up" | Vxlan1 | PASS | - |
| 97 | s2-brdr1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 98 | s2-brdr1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 99 | s2-brdr2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 100 | s2-brdr2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 101 | s2-leaf1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 102 | s2-leaf1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 103 | s2-leaf2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 104 | s2-leaf2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 105 | s2-leaf3 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 106 | s2-leaf3 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 107 | s2-leaf4 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 108 | s2-leaf4 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback1 - VTEP_VXLAN_Tunnel_Source | PASS | - |
| 109 | s2-spine1 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 110 | s2-spine2 | Interface State | Loopback Interface Status & Line Protocol == "up" | Loopback0 - EVPN_Overlay_Peering | PASS | - |
| 111 | s2-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s2-brdr2_Ethernet1 | PASS | - |
| 112 | s2-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s2-brdr2_Ethernet6 | PASS | - |
| 113 | s2-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s2-spine1_Ethernet7 | PASS | - |
| 114 | s2-brdr1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s2-spine2_Ethernet7 | PASS | - |
| 115 | s2-brdr2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s2-brdr1_Ethernet1 | PASS | - |
| 116 | s2-brdr2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s2-brdr1_Ethernet6 | PASS | - |
| 117 | s2-brdr2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s2-spine1_Ethernet8 | PASS | - |
| 118 | s2-brdr2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s2-spine2_Ethernet8 | PASS | - |
| 119 | s2-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s2-leaf2_Ethernet1 | PASS | - |
| 120 | s2-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s2-leaf2_Ethernet6 | PASS | - |
| 121 | s2-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s2-spine1_Ethernet2 | PASS | - |
| 122 | s2-leaf1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s2-spine2_Ethernet2 | PASS | - |
| 123 | s2-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s2-leaf1_Ethernet1 | PASS | - |
| 124 | s2-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s2-leaf1_Ethernet6 | PASS | - |
| 125 | s2-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s2-spine1_Ethernet3 | PASS | - |
| 126 | s2-leaf2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s2-spine2_Ethernet3 | PASS | - |
| 127 | s2-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s2-leaf4_Ethernet1 | PASS | - |
| 128 | s2-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s2-leaf4_Ethernet6 | PASS | - |
| 129 | s2-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s2-spine1_Ethernet4 | PASS | - |
| 130 | s2-leaf3 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s2-spine2_Ethernet4 | PASS | - |
| 131 | s2-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet1 - remote: s2-leaf3_Ethernet1 | PASS | - |
| 132 | s2-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet6 - remote: s2-leaf3_Ethernet6 | PASS | - |
| 133 | s2-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s2-spine1_Ethernet5 | PASS | - |
| 134 | s2-leaf4 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s2-spine2_Ethernet5 | PASS | - |
| 135 | s2-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s2-leaf1_Ethernet2 | PASS | - |
| 136 | s2-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s2-leaf2_Ethernet2 | PASS | - |
| 137 | s2-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: s2-leaf3_Ethernet2 | PASS | - |
| 138 | s2-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: s2-leaf4_Ethernet2 | PASS | - |
| 139 | s2-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet7 - remote: s2-brdr1_Ethernet2 | PASS | - |
| 140 | s2-spine1 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet8 - remote: s2-brdr2_Ethernet2 | PASS | - |
| 141 | s2-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet2 - remote: s2-leaf1_Ethernet3 | PASS | - |
| 142 | s2-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet3 - remote: s2-leaf2_Ethernet3 | PASS | - |
| 143 | s2-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet4 - remote: s2-leaf3_Ethernet3 | PASS | - |
| 144 | s2-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet5 - remote: s2-leaf4_Ethernet3 | PASS | - |
| 145 | s2-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet7 - remote: s2-brdr1_Ethernet3 | PASS | - |
| 146 | s2-spine2 | LLDP Topology | LLDP topology - validate peer and interface | local: Ethernet8 - remote: s2-brdr2_Ethernet3 | PASS | - |
| 147 | s2-brdr1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 148 | s2-brdr2 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 149 | s2-leaf1 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 150 | s2-leaf2 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 151 | s2-leaf3 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 152 | s2-leaf4 | MLAG | MLAG State active & Status connected | MLAG | PASS | - |
| 153 | s2-brdr1 | IP Reachability | ip reachability test p2p links | Source: s2-brdr1_Ethernet2 - Destination: s2-spine1_Ethernet7 | PASS | - |
| 154 | s2-brdr1 | IP Reachability | ip reachability test p2p links | Source: s2-brdr1_Ethernet3 - Destination: s2-spine2_Ethernet7 | PASS | - |
| 155 | s2-brdr2 | IP Reachability | ip reachability test p2p links | Source: s2-brdr2_Ethernet2 - Destination: s2-spine1_Ethernet8 | PASS | - |
| 156 | s2-brdr2 | IP Reachability | ip reachability test p2p links | Source: s2-brdr2_Ethernet3 - Destination: s2-spine2_Ethernet8 | PASS | - |
| 157 | s2-leaf1 | IP Reachability | ip reachability test p2p links | Source: s2-leaf1_Ethernet2 - Destination: s2-spine1_Ethernet2 | PASS | - |
| 158 | s2-leaf1 | IP Reachability | ip reachability test p2p links | Source: s2-leaf1_Ethernet3 - Destination: s2-spine2_Ethernet2 | PASS | - |
| 159 | s2-leaf2 | IP Reachability | ip reachability test p2p links | Source: s2-leaf2_Ethernet2 - Destination: s2-spine1_Ethernet3 | PASS | - |
| 160 | s2-leaf2 | IP Reachability | ip reachability test p2p links | Source: s2-leaf2_Ethernet3 - Destination: s2-spine2_Ethernet3 | PASS | - |
| 161 | s2-leaf3 | IP Reachability | ip reachability test p2p links | Source: s2-leaf3_Ethernet2 - Destination: s2-spine1_Ethernet4 | PASS | - |
| 162 | s2-leaf3 | IP Reachability | ip reachability test p2p links | Source: s2-leaf3_Ethernet3 - Destination: s2-spine2_Ethernet4 | PASS | - |
| 163 | s2-leaf4 | IP Reachability | ip reachability test p2p links | Source: s2-leaf4_Ethernet2 - Destination: s2-spine1_Ethernet5 | PASS | - |
| 164 | s2-leaf4 | IP Reachability | ip reachability test p2p links | Source: s2-leaf4_Ethernet3 - Destination: s2-spine2_Ethernet5 | PASS | - |
| 165 | s2-spine1 | IP Reachability | ip reachability test p2p links | Source: s2-spine1_Ethernet2 - Destination: s2-leaf1_Ethernet2 | PASS | - |
| 166 | s2-spine1 | IP Reachability | ip reachability test p2p links | Source: s2-spine1_Ethernet3 - Destination: s2-leaf2_Ethernet2 | PASS | - |
| 167 | s2-spine1 | IP Reachability | ip reachability test p2p links | Source: s2-spine1_Ethernet4 - Destination: s2-leaf3_Ethernet2 | PASS | - |
| 168 | s2-spine1 | IP Reachability | ip reachability test p2p links | Source: s2-spine1_Ethernet5 - Destination: s2-leaf4_Ethernet2 | PASS | - |
| 169 | s2-spine1 | IP Reachability | ip reachability test p2p links | Source: s2-spine1_Ethernet7 - Destination: s2-brdr1_Ethernet2 | PASS | - |
| 170 | s2-spine1 | IP Reachability | ip reachability test p2p links | Source: s2-spine1_Ethernet8 - Destination: s2-brdr2_Ethernet2 | PASS | - |
| 171 | s2-spine2 | IP Reachability | ip reachability test p2p links | Source: s2-spine2_Ethernet2 - Destination: s2-leaf1_Ethernet3 | PASS | - |
| 172 | s2-spine2 | IP Reachability | ip reachability test p2p links | Source: s2-spine2_Ethernet3 - Destination: s2-leaf2_Ethernet3 | PASS | - |
| 173 | s2-spine2 | IP Reachability | ip reachability test p2p links | Source: s2-spine2_Ethernet4 - Destination: s2-leaf3_Ethernet3 | PASS | - |
| 174 | s2-spine2 | IP Reachability | ip reachability test p2p links | Source: s2-spine2_Ethernet5 - Destination: s2-leaf4_Ethernet3 | PASS | - |
| 175 | s2-spine2 | IP Reachability | ip reachability test p2p links | Source: s2-spine2_Ethernet7 - Destination: s2-brdr1_Ethernet3 | PASS | - |
| 176 | s2-spine2 | IP Reachability | ip reachability test p2p links | Source: s2-spine2_Ethernet8 - Destination: s2-brdr2_Ethernet3 | PASS | - |
| 177 | s2-brdr1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 178 | s2-brdr2 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 179 | s2-leaf1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 180 | s2-leaf2 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 181 | s2-leaf3 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 182 | s2-leaf4 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 183 | s2-spine1 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 184 | s2-spine2 | BGP | ArBGP is configured and operating | ArBGP | PASS | - |
| 185 | s2-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.2.9 | PASS | - |
| 186 | s2-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.16 | PASS | - |
| 187 | s2-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.18 | PASS | - |
| 188 | s2-brdr1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.255.0 | PASS | - |
| 189 | s2-brdr2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.2.8 | PASS | - |
| 190 | s2-brdr2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.20 | PASS | - |
| 191 | s2-brdr2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.22 | PASS | - |
| 192 | s2-brdr2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.255.2 | PASS | - |
| 193 | s2-leaf1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.2.1 | PASS | - |
| 194 | s2-leaf1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.0 | PASS | - |
| 195 | s2-leaf1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.2 | PASS | - |
| 196 | s2-leaf2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.2.0 | PASS | - |
| 197 | s2-leaf2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.4 | PASS | - |
| 198 | s2-leaf2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.6 | PASS | - |
| 199 | s2-leaf3 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.2.5 | PASS | - |
| 200 | s2-leaf3 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.8 | PASS | - |
| 201 | s2-leaf3 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.10 | PASS | - |
| 202 | s2-leaf4 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 10.252.2.4 | PASS | - |
| 203 | s2-leaf4 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.12 | PASS | - |
| 204 | s2-leaf4 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.14 | PASS | - |
| 205 | s2-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.1 | PASS | - |
| 206 | s2-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.5 | PASS | - |
| 207 | s2-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.9 | PASS | - |
| 208 | s2-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.13 | PASS | - |
| 209 | s2-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.17 | PASS | - |
| 210 | s2-spine1 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.21 | PASS | - |
| 211 | s2-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.3 | PASS | - |
| 212 | s2-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.7 | PASS | - |
| 213 | s2-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.11 | PASS | - |
| 214 | s2-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.15 | PASS | - |
| 215 | s2-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.19 | PASS | - |
| 216 | s2-spine2 | BGP | ip bgp peer state established (ipv4) | bgp_neighbor: 172.16.2.23 | PASS | - |
| 217 | s2-brdr1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.1 | PASS | - |
| 218 | s2-brdr1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.2 | PASS | - |
| 219 | s2-brdr1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.7 | PASS | - |
| 220 | s2-brdr2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.1 | PASS | - |
| 221 | s2-brdr2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.2 | PASS | - |
| 222 | s2-brdr2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.1.8 | PASS | - |
| 223 | s2-leaf1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.1 | PASS | - |
| 224 | s2-leaf1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.2 | PASS | - |
| 225 | s2-leaf2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.1 | PASS | - |
| 226 | s2-leaf2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.2 | PASS | - |
| 227 | s2-leaf3 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.1 | PASS | - |
| 228 | s2-leaf3 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.2 | PASS | - |
| 229 | s2-leaf4 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.1 | PASS | - |
| 230 | s2-leaf4 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.2 | PASS | - |
| 231 | s2-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.7 | PASS | - |
| 232 | s2-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.8 | PASS | - |
| 233 | s2-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.3 | PASS | - |
| 234 | s2-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.4 | PASS | - |
| 235 | s2-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.5 | PASS | - |
| 236 | s2-spine1 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.6 | PASS | - |
| 237 | s2-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.7 | PASS | - |
| 238 | s2-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.8 | PASS | - |
| 239 | s2-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.3 | PASS | - |
| 240 | s2-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.4 | PASS | - |
| 241 | s2-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.5 | PASS | - |
| 242 | s2-spine2 | BGP | bgp evpn peer state established (evpn) | bgp_neighbor: 10.250.2.6 | PASS | - |
| 243 | s2-brdr1 | Routing Table | Remote VTEP address | 10.255.2.7 | PASS | - |
| 244 | s2-brdr1 | Routing Table | Remote VTEP address | 10.255.2.3 | PASS | - |
| 245 | s2-brdr1 | Routing Table | Remote VTEP address | 10.255.2.5 | PASS | - |
| 246 | s2-brdr2 | Routing Table | Remote VTEP address | 10.255.2.7 | PASS | - |
| 247 | s2-brdr2 | Routing Table | Remote VTEP address | 10.255.2.3 | PASS | - |
| 248 | s2-brdr2 | Routing Table | Remote VTEP address | 10.255.2.5 | PASS | - |
| 249 | s2-leaf1 | Routing Table | Remote VTEP address | 10.255.2.7 | PASS | - |
| 250 | s2-leaf1 | Routing Table | Remote VTEP address | 10.255.2.3 | PASS | - |
| 251 | s2-leaf1 | Routing Table | Remote VTEP address | 10.255.2.5 | PASS | - |
| 252 | s2-leaf2 | Routing Table | Remote VTEP address | 10.255.2.7 | PASS | - |
| 253 | s2-leaf2 | Routing Table | Remote VTEP address | 10.255.2.3 | PASS | - |
| 254 | s2-leaf2 | Routing Table | Remote VTEP address | 10.255.2.5 | PASS | - |
| 255 | s2-leaf3 | Routing Table | Remote VTEP address | 10.255.2.7 | PASS | - |
| 256 | s2-leaf3 | Routing Table | Remote VTEP address | 10.255.2.3 | PASS | - |
| 257 | s2-leaf3 | Routing Table | Remote VTEP address | 10.255.2.5 | PASS | - |
| 258 | s2-leaf4 | Routing Table | Remote VTEP address | 10.255.2.7 | PASS | - |
| 259 | s2-leaf4 | Routing Table | Remote VTEP address | 10.255.2.3 | PASS | - |
| 260 | s2-leaf4 | Routing Table | Remote VTEP address | 10.255.2.5 | PASS | - |
| 261 | s2-brdr1 | Routing Table | Remote Lo0 address | 10.250.2.7 | PASS | - |
| 262 | s2-brdr1 | Routing Table | Remote Lo0 address | 10.250.2.8 | PASS | - |
| 263 | s2-brdr1 | Routing Table | Remote Lo0 address | 10.250.2.3 | PASS | - |
| 264 | s2-brdr1 | Routing Table | Remote Lo0 address | 10.250.2.4 | PASS | - |
| 265 | s2-brdr1 | Routing Table | Remote Lo0 address | 10.250.2.5 | PASS | - |
| 266 | s2-brdr1 | Routing Table | Remote Lo0 address | 10.250.2.6 | PASS | - |
| 267 | s2-brdr1 | Routing Table | Remote Lo0 address | 10.250.2.1 | PASS | - |
| 268 | s2-brdr1 | Routing Table | Remote Lo0 address | 10.250.2.2 | PASS | - |
| 269 | s2-brdr2 | Routing Table | Remote Lo0 address | 10.250.2.7 | PASS | - |
| 270 | s2-brdr2 | Routing Table | Remote Lo0 address | 10.250.2.8 | PASS | - |
| 271 | s2-brdr2 | Routing Table | Remote Lo0 address | 10.250.2.3 | PASS | - |
| 272 | s2-brdr2 | Routing Table | Remote Lo0 address | 10.250.2.4 | PASS | - |
| 273 | s2-brdr2 | Routing Table | Remote Lo0 address | 10.250.2.5 | PASS | - |
| 274 | s2-brdr2 | Routing Table | Remote Lo0 address | 10.250.2.6 | PASS | - |
| 275 | s2-brdr2 | Routing Table | Remote Lo0 address | 10.250.2.1 | PASS | - |
| 276 | s2-brdr2 | Routing Table | Remote Lo0 address | 10.250.2.2 | PASS | - |
| 277 | s2-leaf1 | Routing Table | Remote Lo0 address | 10.250.2.7 | PASS | - |
| 278 | s2-leaf1 | Routing Table | Remote Lo0 address | 10.250.2.8 | PASS | - |
| 279 | s2-leaf1 | Routing Table | Remote Lo0 address | 10.250.2.3 | PASS | - |
| 280 | s2-leaf1 | Routing Table | Remote Lo0 address | 10.250.2.4 | PASS | - |
| 281 | s2-leaf1 | Routing Table | Remote Lo0 address | 10.250.2.5 | PASS | - |
| 282 | s2-leaf1 | Routing Table | Remote Lo0 address | 10.250.2.6 | PASS | - |
| 283 | s2-leaf1 | Routing Table | Remote Lo0 address | 10.250.2.1 | PASS | - |
| 284 | s2-leaf1 | Routing Table | Remote Lo0 address | 10.250.2.2 | PASS | - |
| 285 | s2-leaf2 | Routing Table | Remote Lo0 address | 10.250.2.7 | PASS | - |
| 286 | s2-leaf2 | Routing Table | Remote Lo0 address | 10.250.2.8 | PASS | - |
| 287 | s2-leaf2 | Routing Table | Remote Lo0 address | 10.250.2.3 | PASS | - |
| 288 | s2-leaf2 | Routing Table | Remote Lo0 address | 10.250.2.4 | PASS | - |
| 289 | s2-leaf2 | Routing Table | Remote Lo0 address | 10.250.2.5 | PASS | - |
| 290 | s2-leaf2 | Routing Table | Remote Lo0 address | 10.250.2.6 | PASS | - |
| 291 | s2-leaf2 | Routing Table | Remote Lo0 address | 10.250.2.1 | PASS | - |
| 292 | s2-leaf2 | Routing Table | Remote Lo0 address | 10.250.2.2 | PASS | - |
| 293 | s2-leaf3 | Routing Table | Remote Lo0 address | 10.250.2.7 | PASS | - |
| 294 | s2-leaf3 | Routing Table | Remote Lo0 address | 10.250.2.8 | PASS | - |
| 295 | s2-leaf3 | Routing Table | Remote Lo0 address | 10.250.2.3 | PASS | - |
| 296 | s2-leaf3 | Routing Table | Remote Lo0 address | 10.250.2.4 | PASS | - |
| 297 | s2-leaf3 | Routing Table | Remote Lo0 address | 10.250.2.5 | PASS | - |
| 298 | s2-leaf3 | Routing Table | Remote Lo0 address | 10.250.2.6 | PASS | - |
| 299 | s2-leaf3 | Routing Table | Remote Lo0 address | 10.250.2.1 | PASS | - |
| 300 | s2-leaf3 | Routing Table | Remote Lo0 address | 10.250.2.2 | PASS | - |
| 301 | s2-leaf4 | Routing Table | Remote Lo0 address | 10.250.2.7 | PASS | - |
| 302 | s2-leaf4 | Routing Table | Remote Lo0 address | 10.250.2.8 | PASS | - |
| 303 | s2-leaf4 | Routing Table | Remote Lo0 address | 10.250.2.3 | PASS | - |
| 304 | s2-leaf4 | Routing Table | Remote Lo0 address | 10.250.2.4 | PASS | - |
| 305 | s2-leaf4 | Routing Table | Remote Lo0 address | 10.250.2.5 | PASS | - |
| 306 | s2-leaf4 | Routing Table | Remote Lo0 address | 10.250.2.6 | PASS | - |
| 307 | s2-leaf4 | Routing Table | Remote Lo0 address | 10.250.2.1 | PASS | - |
| 308 | s2-leaf4 | Routing Table | Remote Lo0 address | 10.250.2.2 | PASS | - |
| 309 | s2-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr1 - 10.250.2.7 Destination: 10.250.2.7 | PASS | - |
| 310 | s2-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr1 - 10.250.2.7 Destination: 10.250.2.8 | PASS | - |
| 311 | s2-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr1 - 10.250.2.7 Destination: 10.250.2.3 | PASS | - |
| 312 | s2-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr1 - 10.250.2.7 Destination: 10.250.2.4 | PASS | - |
| 313 | s2-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr1 - 10.250.2.7 Destination: 10.250.2.5 | PASS | - |
| 314 | s2-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr1 - 10.250.2.7 Destination: 10.250.2.6 | PASS | - |
| 315 | s2-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr1 - 10.250.2.7 Destination: 10.250.2.1 | PASS | - |
| 316 | s2-brdr1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr1 - 10.250.2.7 Destination: 10.250.2.2 | PASS | - |
| 317 | s2-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr2 - 10.250.2.8 Destination: 10.250.2.7 | PASS | - |
| 318 | s2-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr2 - 10.250.2.8 Destination: 10.250.2.8 | PASS | - |
| 319 | s2-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr2 - 10.250.2.8 Destination: 10.250.2.3 | PASS | - |
| 320 | s2-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr2 - 10.250.2.8 Destination: 10.250.2.4 | PASS | - |
| 321 | s2-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr2 - 10.250.2.8 Destination: 10.250.2.5 | PASS | - |
| 322 | s2-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr2 - 10.250.2.8 Destination: 10.250.2.6 | PASS | - |
| 323 | s2-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr2 - 10.250.2.8 Destination: 10.250.2.1 | PASS | - |
| 324 | s2-brdr2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-brdr2 - 10.250.2.8 Destination: 10.250.2.2 | PASS | - |
| 325 | s2-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf1 - 10.250.2.3 Destination: 10.250.2.7 | PASS | - |
| 326 | s2-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf1 - 10.250.2.3 Destination: 10.250.2.8 | PASS | - |
| 327 | s2-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf1 - 10.250.2.3 Destination: 10.250.2.3 | PASS | - |
| 328 | s2-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf1 - 10.250.2.3 Destination: 10.250.2.4 | PASS | - |
| 329 | s2-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf1 - 10.250.2.3 Destination: 10.250.2.5 | PASS | - |
| 330 | s2-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf1 - 10.250.2.3 Destination: 10.250.2.6 | PASS | - |
| 331 | s2-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf1 - 10.250.2.3 Destination: 10.250.2.1 | PASS | - |
| 332 | s2-leaf1 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf1 - 10.250.2.3 Destination: 10.250.2.2 | PASS | - |
| 333 | s2-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf2 - 10.250.2.4 Destination: 10.250.2.7 | PASS | - |
| 334 | s2-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf2 - 10.250.2.4 Destination: 10.250.2.8 | PASS | - |
| 335 | s2-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf2 - 10.250.2.4 Destination: 10.250.2.3 | PASS | - |
| 336 | s2-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf2 - 10.250.2.4 Destination: 10.250.2.4 | PASS | - |
| 337 | s2-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf2 - 10.250.2.4 Destination: 10.250.2.5 | PASS | - |
| 338 | s2-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf2 - 10.250.2.4 Destination: 10.250.2.6 | PASS | - |
| 339 | s2-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf2 - 10.250.2.4 Destination: 10.250.2.1 | PASS | - |
| 340 | s2-leaf2 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf2 - 10.250.2.4 Destination: 10.250.2.2 | PASS | - |
| 341 | s2-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf3 - 10.250.2.5 Destination: 10.250.2.7 | PASS | - |
| 342 | s2-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf3 - 10.250.2.5 Destination: 10.250.2.8 | PASS | - |
| 343 | s2-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf3 - 10.250.2.5 Destination: 10.250.2.3 | PASS | - |
| 344 | s2-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf3 - 10.250.2.5 Destination: 10.250.2.4 | PASS | - |
| 345 | s2-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf3 - 10.250.2.5 Destination: 10.250.2.5 | PASS | - |
| 346 | s2-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf3 - 10.250.2.5 Destination: 10.250.2.6 | PASS | - |
| 347 | s2-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf3 - 10.250.2.5 Destination: 10.250.2.1 | PASS | - |
| 348 | s2-leaf3 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf3 - 10.250.2.5 Destination: 10.250.2.2 | PASS | - |
| 349 | s2-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf4 - 10.250.2.6 Destination: 10.250.2.7 | PASS | - |
| 350 | s2-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf4 - 10.250.2.6 Destination: 10.250.2.8 | PASS | - |
| 351 | s2-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf4 - 10.250.2.6 Destination: 10.250.2.3 | PASS | - |
| 352 | s2-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf4 - 10.250.2.6 Destination: 10.250.2.4 | PASS | - |
| 353 | s2-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf4 - 10.250.2.6 Destination: 10.250.2.5 | PASS | - |
| 354 | s2-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf4 - 10.250.2.6 Destination: 10.250.2.6 | PASS | - |
| 355 | s2-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf4 - 10.250.2.6 Destination: 10.250.2.1 | PASS | - |
| 356 | s2-leaf4 | Loopback0 Reachability | Loopback0 Reachability | Source: s2-leaf4 - 10.250.2.6 Destination: 10.250.2.2 | PASS | - |
