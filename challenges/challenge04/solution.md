\# Solution — Challenge 04: Malicious Phishing Document



\## What You Were Supposed to Find

The phishing PDF contains a hyperlink redirecting to a credential harvesting portal.



\## How to Solve

1\. Open `doc\_metadata.json` — see the editor `PDFCreator 0.47 (modified)`.

2\. Inspect hyperlinks in `pdf\_links.txt`:

https://hr-benefits.example.com.login-check\[.]info

3\. `email\_headers.txt` shows spoofed internal address.

4\. `decoded\_payload.txt` contains Base64-decoded HTML referencing an O365 phishing kit.



\## Reasoning

Spoof + redirect domain + embedded malicious content = phishing lure.



\## Expected Flag

flag{o365\_phish\_redirect\_detected}

