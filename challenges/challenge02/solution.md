\# Solution — Challenge 02: Supply Chain DLL Tampering



\## What You Were Supposed to Find

One DLL was replaced with a trojanized version in the installation directory of a vendor software package.



\## How to Solve

1\. Review `file\_manifest.json` and compare hashes.

2\. Identify mismatch for:

telemetry\_core.dll

3\. Hash in `telemetry\_core.dll.hash` does NOT match the vendor-signed hash in manifest.

4\. Open `incident\_log.txt` — shows unauthorized write events during update window.

5\. `diff.txt` shows added suspicious export:

Export: InitShadowChannel



\## Reasoning

Hash mismatch + added exports are strong indicators of tampering.



\## Expected Flag

flag{dll\_supply\_chain\_tamper\_detected}

