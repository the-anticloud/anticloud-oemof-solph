# Educators — OEMOF_SOLPH

**Project:** OEMOF_SOLPH  
**Category:** SOLAR  
**Upstream:** https://github.com/oemof/oemof-solph  
**Pinned commit:** `943c057da7445e971750e95130c2e9b0158ce20d`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `4dce41338ccd5ee69d93d65142dfd87c0d219a6e548241e5b99b781d3970dc70`  
**Date:** October 2026

## Teaching with OEMOF_SOLPH

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `4dce41338ccd5ee69d93d65142dfd87c0d219a6e548241e5b99b781d3970dc70` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
