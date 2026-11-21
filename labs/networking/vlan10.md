# Cisco Packet Tracer — VLAN 10 access ports

**Practice recorded:** 11 October 2026.  
**Goal:** Create VLAN 10 and assign switch ports FastEthernet 0/6 and 0/7 as access ports.

## Command sequence used in the learning walkthrough

```text
enable
configure terminal
vlan 10
exit
interface range fastEthernet 0/6 - 7
switchport mode access
switchport access vlan 10
end
show vlan brief
```

## What to verify

The `show vlan brief` output should list VLAN 10 and ports Fa0/6 and Fa0/7. A switch-port assignment alone does not prove end-to-end connectivity or traffic isolation.

## Evidence status

The task and CLI walkthrough are documented. An original Packet Tracer topology, screenshot and actual switch output are not included, so no passed connectivity test is claimed.

**Learning focus:** VLAN membership, access-port configuration, interface ranges and CLI verification.

[Labs index](../README.md)
