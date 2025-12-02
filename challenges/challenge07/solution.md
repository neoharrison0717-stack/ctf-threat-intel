\# Solution — Challenge 07: Threat Actor TTP Classification



\## What You Were Supposed to Find

The actor’s TTPs map to MITRE ATT\&CK techniques associated with APT29-style intrusion chains.



\## How to Solve

1\. `log\_summary.txt` shows:

&nbsp;  - Credential dumping via LSASS access  

&nbsp;  - WMI remote execution  

&nbsp;  - Encrypted C2 with custom certificate  



2\. `ttp\_matrix.csv` maps:

T1003, T1047, T1573



3\. `actor\_notes.txt` mentions "stealthy ops" and "government targets".



4\. `ioc\_list.json` shows use of domains typically reported in APT29-like campaigns.



\## Reasoning

Technique overlap strongly matches known threat actor behaviors.



\## Expected Flag

flag{apt29\_style\_ttp\_cluster}

