# Solution — Challenge 03: Git Compromise Forensics

## What You Were Supposed to Find
The attacker's local timezone.

## How to Solve
1. Analyze `git_reflog_extract.json` for timezone offsets in timestamps.
2. Compare with `commit_log.txt` and `refs_heads_master.bak`.
3. Use the metadata in `malicious_patch.diff` for confirmation.

## Expected Flag
flag{UTC+3}