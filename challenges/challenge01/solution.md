# Solution — Challenge 01: Sable Hydra Infrastructure Mapping

## What You Were Supposed to Find
The IPv4 address shared by at least 5 malicious domains.

## How to Solve
1. Examine `dns_logs.csv` and `pdns_snapshot.json` to list domains and IPs.
2. Compare entries in `whois_diff.txt` to find reused registrant info.
3. Check `apache_listing.html` for exposed directories and IPs.
4. Cross-reference all sources — identify the single IPv4 used by multiple domains.

## Expected Flag
flag{192.168.101.42}
