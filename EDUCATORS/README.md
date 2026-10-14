# Educators — SUBSURFACE

**Project:** SUBSURFACE  
**Category:** OIL_GAS  
**Upstream:** https://github.com/softwareunderground/subsurface  
**Pinned commit:** `816db75bad6f1eda71209a4635490d2969eadeb0`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `da2973e7a7eaefd297e95c2a08c335108dd2c1441d7139bcc66ac1ee91b3e445`  
**Date:** October 2026

## Teaching with SUBSURFACE

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `da2973e7a7eaefd297e95c2a08c335108dd2c1441d7139bcc66ac1ee91b3e445` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
