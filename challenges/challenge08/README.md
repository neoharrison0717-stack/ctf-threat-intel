\# Challenge 08 – NPM Supply Chain Dependency Graph Attack



\## Backstory

Attackers created a cluster of malicious npm packages designed to poison a CI/CD pipeline. Many share similar commit patterns, CI workflows, and hash similarities.



\## Description

Using the dependency graph, user profile notes, CI workflow samples, and hash clustering:

\- map package relationships  

\- identify dependency bottlenecks  

\- find the central pivot package feeding the entire attack chain



This “hub” package is the attacker’s true anchor.



\## Attachments

\- `dependency\_graph.json`

\- `npm\_user\_profiles.txt`

\- `ci\_workflow\_samples.yml`

\- `package\_hashes.csv`



\## Task

Identify the central malicious package.



\## Flag Format

flag{package\_name}

