\# Challenge 07 – AtlasBeak C2 Certificate Reuse Lineage



\## Backstory

AtlasBeak routinely reuses self-signed TLS certificates across operations. You recovered a suspicious fingerprint from a recent scan and now must trace it through historical datasets.



\## Description

Compare the provided fingerprint against:

\- historical campaign records  

\- atlas timeline data  

\- recent TLS scans  



Find the earliest campaign where the certificate appeared.



\## Attachments

\- `certificate\_fingerprint.txt`

\- `historical\_campaigns.csv`

\- `atlasbeak\_timeline.json`

\- `tls\_scan\_results.txt`



\## Task

Submit the earliest campaign name associated with the certificate.



\## Flag Format

flag{campaign\_name}

