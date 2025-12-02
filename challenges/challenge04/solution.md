# Solution — Challenge 04: Frost Lantern Beacon Analysis

## What You Were Supposed to Find
The baseline beacon interval (short, long) in seconds.

## How to Solve
1. Use `frostlantern_beacons.pcap` to extract beacon timings.
2. Correlate with `beacon_intervals.csv`.
3. Use `suricata_alerts.json` to confirm which beacons are malicious.
4. Check `reverse_notes.txt` for obfuscation patterns.

## Expected Flag
flag{10_45}