# Ethics — SUBSURFACE

**Project:** SUBSURFACE  
**Category:** OIL_GAS  
**Upstream:** https://github.com/softwareunderground/subsurface  
**Pinned commit:** `816db75bad6f1eda71209a4635490d2969eadeb0`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `da2973e7a7eaefd297e95c2a08c335108dd2c1441d7139bcc66ac1ee91b3e445`  
**Date:** October 2026

## Position

SUBSURFACE is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
