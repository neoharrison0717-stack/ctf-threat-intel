\# Challenge 03 – Internal Git Compromise Metadata Forensics



\## Backstory

An attacker briefly accessed an internal Git server and injected malicious changes. Although the commit was reverted, traces remain in reflogs and backup refs.



The attacker spoofed timestamps but forgot to hide the timezone offset embedded inside one reflog line.



\## Description

Analyze the recovered Git metadata:

\- orphaned refs  

\- reflog fragments  

\- commit logs  

\- the partial malicious diff  



Determine the attacker’s local timezone offset based on metadata leakage.



\## Attachments

\- `commit\_log.txt`

\- `refs\_heads\_master.bak`

\- `git\_reflog\_extract.json`

\- `malicious\_patch.diff`



\## Task

Recover the timezone offset (e.g., UTC+2).



\## Flag Format

flag{UTC±X}

