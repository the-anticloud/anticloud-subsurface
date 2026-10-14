# Students — SUBSURFACE

**Project:** SUBSURFACE  
**Category:** OIL_GAS  
**Upstream:** https://github.com/softwareunderground/subsurface  
**Pinned commit:** `816db75bad6f1eda71209a4635490d2969eadeb0`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `da2973e7a7eaefd297e95c2a08c335108dd2c1441d7139bcc66ac1ee91b3e445`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `816db75bad6f1eda71209a4635490d2969eadeb0`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `da2973e7a7eaefd297e95c2a08c335108dd2c1441d7139bcc66ac1ee91b3e445`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
