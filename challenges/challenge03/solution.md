\# Solution — Challenge 03: OSINT Infrastructure Mapping



\## What You Were Supposed to Find

Threat actor infrastructure pivoting from a GitHub account to VPS hosting and staging domains.



\## How to Solve

1\. Use `profile\_screenshot.png` to note the GitHub username: `ZeroPointResearch`.

2\. Look at `forks.json` — one repository contains a domain listed in comments:

logrelay-sync\[.]net

3\. `whois.txt` shows the domain registered using ProtonMail alias seen on the GitHub profile.

4\. `notes.txt` provides a leaked handle “zpr\_ops”.



\## Reasoning

Pivoting through social connections + reused aliases performs attribution.



\## Expected Flag

flag{osint\_linked\_zpr\_ops\_infra}

