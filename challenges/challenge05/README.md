\# Challenge 04 – Operation “Frost Lantern” Beacon Timing Reconstruction



\## Backstory

A malware family tied to the \*Frost Lantern\* group uses jittered short-long beacon intervals for C2 communication. The pattern is obfuscated, but PCAP captures and reverse-engineering notes give clues.



\## Description

Using captured beacon intervals, IDS alerts, and a timing-function summary from reverse analysis:

\- remove jitter  

\- identify repeated patterns  

\- correlate timing with malware logic  



Determine the intended (short,long) beacon pattern.



\## Attachments

\- `frostlantern\_beacons.pcap`

\- `suricata\_alerts.json`

\- `beacon\_intervals.csv`

\- `reverse\_notes.txt`



\## Task

Identify the intended baseline interval pair (in seconds).



\## Flag Format

flag{short\_long}

