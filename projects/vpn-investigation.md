# VPN Log Investigation

## Objective
Investigate suspicious VPN login activity using Elastic Stack.

## Tools Used
- Kibana
- Elastic Stack
- KQL

## Investigation

Query used:
event.dataset : "vpn"


Findings:
- Multiple failed login attempts detected
- Source IP repeated across several accounts
- Pattern consistent with brute force behaviour

## Conclusion

Activity suggests credential brute force attempts against the VPN service.
