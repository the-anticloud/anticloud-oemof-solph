# Independent Insurance — OEMOF_SOLPH

**Project:** OEMOF_SOLPH  
**Category:** SOLAR  
**Upstream:** https://github.com/oemof/oemof-solph  
**Pinned commit:** `943c057da7445e971750e95130c2e9b0158ce20d`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `4dce41338ccd5ee69d93d65142dfd87c0d219a6e548241e5b99b781d3970dc70`  
**Date:** October 2026

## Why AI-specific cover matters

Deploying AI in a regulated sector creates liability surfaces that ordinary
technology cover does not reach: inference liability, audit-trail liability,
data-breach liability and IP-infringement liability.

## How this project's architecture reduces insurable risk

| Risk | Cloud AI | OEMOF_SOLPH with AIOSS |
|---|---|---|
| Audit-trail loss | high — vendor-controlled logs | low — append-only chain, verifiable offline |
| Data breach in transit | high — data transits external servers | low — no external endpoint |
| Compliance violation | high — cannot satisfy air-gap requirements | low — structural |
| IP liability | moderate | low — pinned provenance chain |

## Evidence package for an insurer

- AIOSS chain verification for head `4dce41338ccd5ee69d93d65142dfd87c0d219a6e548241e5b99b781d3970dc70`
- The 16-check register with per-check evidence hashes
- Framework control mapping in `BENCH.json`

## Contact

lois@0-1.gg
