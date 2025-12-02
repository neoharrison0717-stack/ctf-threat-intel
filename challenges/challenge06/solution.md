\# Solution — Challenge 06: Ransomware Precursor Activity



\## What You Were Supposed to Find

The adversary used PsExec-style lateral movement before deploying ransomware.



\## How to Solve

1\. In `eventlogs.evtxt\_export.txt`, search for service creation events (Event 7045).

2\. Spot suspicious service:

psexecsvc\_temp

3\. `netlogon.txt` shows failed and successful logins from host `ENG-SRV-12`.

4\. `timeline.csv` reveals the sequence:

Recon → Credential access → Lateral tool deployment.



\## Reasoning

These behaviors are classic ransomware staging.



\## Expected Flag

flag{psexec\_lateral\_move\_chain}

