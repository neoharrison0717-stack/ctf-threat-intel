# Solution — Challenge 05: Orchid Ledger PDF Analysis

## What You Were Supposed to Find
The malware builder family used to create the embedded payload.

## How to Solve
1. Check `pdf_metadata.json` for unusual creator/editor fields.
2. Analyze `pdf_strings.txt` for patterns matching known builders.
3. Examine `embedded_js_obf.js` for obfuscation style.
4. Refer to `heuristic_report.txt` for confirmation.

## Expected Flag
flag{orchidbuilder}