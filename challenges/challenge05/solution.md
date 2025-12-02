\# Solution — Challenge 05: Insider Data Exfiltration



\## What You Were Supposed to Find

A user uploaded confidential files to an unapproved cloud storage provider.



\## How to Solve

1\. `proxy\_logs.txt` — search for large POST requests.

2\. Identify uploads to:

drive-share-sync\[.]io/upload

3\. `access\_times.csv` shows late-night access.

4\. `audit\_result.json` lists the user `m.teller` with classification violations.



\## Reasoning

Pattern matches insider exfil via cloud storage.



\## Expected Flag

flag{insider\_cloud\_exfil\_m\_teller}

