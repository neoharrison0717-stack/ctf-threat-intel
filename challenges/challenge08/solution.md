# Solution — Challenge 08: Supply Chain Dependency Graph

## What You Were Supposed to Find
The central malicious NPM package.

## How to Solve
1. Analyze `dependency_graph.json` for package relationships.
2. Use `package_hashes.csv` to find duplicate hashes.
3. Check `npm_user_profiles.txt` and `ci_workflow_samples.yml` for patterns.
4. Identify the central node feeding the entire chain.

## Expected Flag
flag{evil-pkg-core}