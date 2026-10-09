# Students — OEMOF_SOLPH

**Project:** OEMOF_SOLPH  
**Category:** SOLAR  
**Upstream:** https://github.com/oemof/oemof-solph  
**Pinned commit:** `943c057da7445e971750e95130c2e9b0158ce20d`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `4dce41338ccd5ee69d93d65142dfd87c0d219a6e548241e5b99b781d3970dc70`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `943c057da7445e971750e95130c2e9b0158ce20d`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `4dce41338ccd5ee69d93d65142dfd87c0d219a6e548241e5b99b781d3970dc70`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
