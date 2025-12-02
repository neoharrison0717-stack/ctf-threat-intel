# Challenge 01 – APT “Sable Hydra” Infrastructure Constellation Mapping

## Backstory
A threat actor known as *Sable Hydra* has targeted your organization’s semiconductor research division. Their phishing domains rotate through rapidly changing infrastructure supported by fast-flux DNS and misconfigured servers.

Investigators collected several types of data from passive DNS, WHOIS snapshots, and an exposed Apache directory.

## Description
You are given the domain:

hydra-research-support[.]com

Use the attachments to build an infrastructure map. Identify pivot points such as:
- reused TLS certificate serial numbers  
- shared hosting ranges  
- IPs reused across different malicious domains  
- SOA, registrar, and contact patterns

Your goal is to identify the **single IPv4 address** that links at least **five** malicious domains.

## Attachments
- `dns_logs.csv`
- `pdns_snapshot.json`
- `whois_diff.txt`
- `apache_listing.html`

## Task
Determine the IPv4 address shared by the actor’s cluster.

## Flag Format
flag{X.X.X.X}