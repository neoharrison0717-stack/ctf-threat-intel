\# Solution — Challenge 08: Reverse-Engineering a Fake Malware Sample



\## What You Were Supposed to Find

The binary is a benign mock sample, but contains an embedded string revealing the command keyword.



\## How to Solve

1\. Open `strings\_output.txt`.

2\. Search for structured keywords — find:

CMD\_TRIGGER\_ALPHA

3\. In `analysis\_notes.txt`, see reference to unused function `parseAlphaTrigger()`.

4\. `manifest.yaml` shows the compiled time intentionally randomized.



\## Reasoning

Hidden string indicators are often used in beginner-friendly RE challenges.



\## Expected Flag

flag{cmd\_trigger\_alpha}

