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
| 58 | 56 | 2 | 0 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| s1-brdr1 | 6 | 6 | 0 | 0 | - | - |
| s1-brdr2 | 6 | 6 | 0 | 0 | - | - |
| s1-leaf1 | 6 | 6 | 0 | 0 | - | - |
| s1-leaf2 | 6 | 6 | 0 | 0 | - | - |
| s1-leaf3 | 6 | 6 | 0 | 0 | - | - |
| s1-leaf4 | 6 | 6 | 0 | 0 | - | - |
| s1-spine1 | 11 | 10 | 1 | 0 | System | - |
| s1-spine2 | 11 | 10 | 1 | 0 | System | - |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| Connectivity | 36 | 36 | 0 | 0 |
| Logging | 16 | 16 | 0 | 0 |
| System | 6 | 4 | 2 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 47 | s1-spine1 | System | VerifyMemoryUtilization | Verifies whether the memory utilization is below 75%. | - | FAIL | Device has reported a high memory usage: 93.83% |
| 58 | s1-spine2 | System | VerifyMemoryUtilization | Verifies whether the memory utilization is below 75%. | - | FAIL | Device has reported a high memory usage: 93.85% |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-brdr2 Ethernet1 | PASS | - |
| 2 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet7 | PASS | - |
| 3 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet7 | PASS | - |
| 4 | s1-brdr1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-brdr2 Ethernet6 | PASS | - |
| 5 | s1-brdr1 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 6 | s1-brdr1 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 7 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-brdr1 Ethernet1 | PASS | - |
| 8 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet8 | PASS | - |
| 9 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet8 | PASS | - |
| 10 | s1-brdr2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-brdr1 Ethernet6 | PASS | - |
| 11 | s1-brdr2 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 12 | s1-brdr2 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 13 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-leaf2 Ethernet1 | PASS | - |
| 14 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet2 | PASS | - |
| 15 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet2 | PASS | - |
| 16 | s1-leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-leaf2 Ethernet6 | PASS | - |
| 17 | s1-leaf1 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 18 | s1-leaf1 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 19 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-leaf1 Ethernet1 | PASS | - |
| 20 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet3 | PASS | - |
| 21 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet3 | PASS | - |
| 22 | s1-leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-leaf1 Ethernet6 | PASS | - |
| 23 | s1-leaf2 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 24 | s1-leaf2 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 25 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-leaf4 Ethernet1 | PASS | - |
| 26 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet4 | PASS | - |
| 27 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet4 | PASS | - |
| 28 | s1-leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-leaf4 Ethernet6 | PASS | - |
| 29 | s1-leaf3 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 30 | s1-leaf3 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 31 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet1 - Remote: s1-leaf3 Ethernet1 | PASS | - |
| 32 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-spine1 Ethernet5 | PASS | - |
| 33 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-spine2 Ethernet5 | PASS | - |
| 34 | s1-leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet6 - Remote: s1-leaf3 Ethernet6 | PASS | - |
| 35 | s1-leaf4 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 36 | s1-leaf4 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 37 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-leaf1 Ethernet2 | PASS | - |
| 38 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-leaf2 Ethernet2 | PASS | - |
| 39 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet4 - Remote: s1-leaf3 Ethernet2 | PASS | - |
| 40 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet5 - Remote: s1-leaf4 Ethernet2 | PASS | - |
| 41 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet7 - Remote: s1-brdr1 Ethernet2 | PASS | - |
| 42 | s1-spine1 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet8 - Remote: s1-brdr2 Ethernet2 | PASS | - |
| 43 | s1-spine1 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 44 | s1-spine1 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 45 | s1-spine1 | System | VerifyCPUUtilization | Verifies whether the CPU utilization is below 75%. | - | PASS | - |
| 46 | s1-spine1 | System | VerifyFileSystemUtilization | Verifies that no partition is utilizing more than 75% of its disk space. | - | PASS | - |
| 47 | s1-spine1 | System | VerifyMemoryUtilization | Verifies whether the memory utilization is below 75%. | - | FAIL | Device has reported a high memory usage: 93.83% |
| 48 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet2 - Remote: s1-leaf1 Ethernet3 | PASS | - |
| 49 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet3 - Remote: s1-leaf2 Ethernet3 | PASS | - |
| 50 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet4 - Remote: s1-leaf3 Ethernet3 | PASS | - |
| 51 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet5 - Remote: s1-leaf4 Ethernet3 | PASS | - |
| 52 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet7 - Remote: s1-brdr1 Ethernet3 | PASS | - |
| 53 | s1-spine2 | Connectivity | VerifyLLDPNeighbors | Verifies that the provided LLDP neighbors are connected properly. | Local: Ethernet8 - Remote: s1-brdr2 Ethernet3 | PASS | - |
| 54 | s1-spine2 | Logging | VerifyLoggingHosts | Verifies logging hosts (syslog servers) for a specified VRF. | - | PASS | - |
| 55 | s1-spine2 | Logging | VerifyLoggingSourceIntf | Verifies logging source-interface for a specified VRF. | - | PASS | - |
| 56 | s1-spine2 | System | VerifyCPUUtilization | Verifies whether the CPU utilization is below 75%. | - | PASS | - |
| 57 | s1-spine2 | System | VerifyFileSystemUtilization | Verifies that no partition is utilizing more than 75% of its disk space. | - | PASS | - |
| 58 | s1-spine2 | System | VerifyMemoryUtilization | Verifies whether the memory utilization is below 75%. | - | FAIL | Device has reported a high memory usage: 93.85% |
