# Solution — Challenge 07: AtlasBeak Certificate Reuse

## What You Were Supposed to Find
The earliest campaign associated with the reused certificate.

## How to Solve
1. Compare `certificate_fingerprint.txt` with `historical_campaigns.csv`.
2. Cross-reference dates in `atlasbeak_timeline.json`.
3. Confirm with `tls_scan_results.txt` which campaigns used the fingerprint first.

## Expected Flag
flag{winter_storm}