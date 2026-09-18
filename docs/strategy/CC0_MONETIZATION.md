# PIN Monetization Strategy — CC0.company First Candidate

**Status:** ACTIVE STRATEGY DECISION  
**Date:** 2026-09-18  
**Scope:** PIN Test / Commercial Readiness R0–R3

## Decision

For the first real PIN commercial loop, **CC0.company is the primary monetization candidate**.

**Admitad is not required for the initial R0/R1 test** and is retained as a reserve / secondary monetization channel.

The goal is to reduce external dependencies while preserving the possibility of monetization from the beginning.

## Intended first loop

```
Opportunity / monetizable object
→ Hypothesis Agent
→ Content Agent
→ creative generation
→ Publisher
→ Guardian authorization
→ Pinterest official API
→ real Pin publication
→ read-back / reality verification
→ Calyx evidence + provenance
→ traffic / action measurement
→ payout / revenue evidence when available
```

## Commercial readiness mapping

### R0 — Reality Gate
One real Pin task is executed end-to-end and independently verified against reality.

Minimum evidence:
- intended action;
- actual Pinterest API result;
- returned Pin identifier / URL;
- independent read-back;
- content / board / link comparison against intent;
- timestamps;
- hashes / provenance where applicable;
- final PASS only when observed reality matches the intended state.

### R1 — Repeatability Gate
The same loop can be repeated reliably without false PASS.

### R2 — Value Gate
The loop produces measurable external value such as impressions, saves, outbound clicks, qualified actions or other defined business metrics.

### R3 — Payment Gate
A real external monetary event is independently evidenced.

R3 must not be inferred from clicks, dashboard estimates, expected rewards or self-reported values. A real payout / settled revenue event must be observed and preserved as evidence.

## CC0.company rule

CC0.company is treated as a **candidate monetization provider until its exact payout, attribution, API, eligibility and withdrawal mechanics are independently verified**.

No payout rate, affiliate percentage, token/reward mechanism, or eligibility condition is considered VERIFIED merely because it appeared in conversation or marketing material.

Required evidence before relying on it commercially:
1. official terms / documentation;
2. actual account eligibility;
3. attribution mechanism;
4. payout trigger;
5. withdrawal / settlement path;
6. jurisdiction / KYC constraints relevant to the operator;
7. one real successful payout.

## Admitad

Admitad remains available as a fallback or later diversification channel.

It should not be added to the R0 path unless CC0.company proves unsuitable or the experiment specifically requires affiliate-network attribution.

## Architecture rule

This strategy must not weaken existing PIN capability controls:

- ACTION only through Guardian;
- Publisher requests CREATE_PIN capability rather than holding unrestricted authority;
- secrets remain outside agent-readable business logic;
- Calyx stores evidence/provenance;
- false-pass and repeat gates remain cumulative;
- production logic is not changed solely to manufacture a portfolio result.

## Why this decision

The first PIN experiment should test the smallest commercially meaningful closed loop.

Removing Admitad from the initial path reduces:
- account / approval dependencies;
- attribution complexity;
- failure ambiguity;
- integration surface;
- time to first real end-to-end test.

At the same time, a monetization-capable provider keeps the experiment aligned with the later R2/R3 commercial gates.

---

**Next gate:** independently verify CC0.company mechanics, then define the exact R0 task contract.
