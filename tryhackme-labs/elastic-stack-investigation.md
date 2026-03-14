# Elastic Stack Investigation – TryHackMe

## Objective
Investigate VPN connection logs to identify suspicious activity and potential unauthorized access.

## Tools Used
- Kibana
- Elastic Stack
- SIEM log analysis

## Investigation Steps
1. Opened Kibana Discover.
2. Filtered VPN logs for authentication events.
3. Investigated failed login attempts.
4. Checked activity after employee termination date.

## Example Query
event.category:authentication AND event.outcome:failure

## Findings
User **Johnny Brown** continued to authenticate after termination on 1 January 2022.

## MITRE ATT&CK Mapping
T1078 – Valid Accounts

## Conclusion
The account may have been misused after termination, indicating possible credential compromise.
