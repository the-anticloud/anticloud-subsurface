# Independent Insurance — SUBSURFACE

**Project:** SUBSURFACE  
**Category:** OIL_GAS  
**Upstream:** https://github.com/softwareunderground/subsurface  
**Pinned commit:** `816db75bad6f1eda71209a4635490d2969eadeb0`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `da2973e7a7eaefd297e95c2a08c335108dd2c1441d7139bcc66ac1ee91b3e445`  
**Date:** October 2026

## Why AI-specific cover matters

Deploying AI in a regulated sector creates liability surfaces that ordinary
technology cover does not reach: inference liability, audit-trail liability,
data-breach liability and IP-infringement liability.

## How this project's architecture reduces insurable risk

| Risk | Cloud AI | SUBSURFACE with AIOSS |
|---|---|---|
| Audit-trail loss | high — vendor-controlled logs | low — append-only chain, verifiable offline |
| Data breach in transit | high — data transits external servers | low — no external endpoint |
| Compliance violation | high — cannot satisfy air-gap requirements | low — structural |
| IP liability | moderate | low — pinned provenance chain |

## Evidence package for an insurer

- AIOSS chain verification for head `da2973e7a7eaefd297e95c2a08c335108dd2c1441d7139bcc66ac1ee91b3e445`
- The 16-check register with per-check evidence hashes
- Framework control mapping in `BENCH.json`

## Contact

lois@0-1.gg
