\# Solution — Challenge 01: Suspicious Beaconing



\## What You Were Supposed to Find

The beaconing pattern indicates a compromised workstation calling out to a known C2 infrastructure every 60 seconds.



\## How to Solve

1\. Open `traffic.pcap` in Wireshark.

2\. Filter using: `dns or http`.

3\. Identify repeated DNS requests to:

hxxp://pulse-sync\[.]com/update

4\. Cross-reference with `alert.png` — the EDR screenshot highlights the same domain as “High-Risk: Command \& Control”.



5\. Use `sysinfo.json` — the hostname `WS-FIN-07` matches the logs.



\## Reasoning

The repetitive timing + known malicious domain reveal a scheduled beacon.



\## Expected Flag

flag{beacon\_pulse\_sync\_c2}

