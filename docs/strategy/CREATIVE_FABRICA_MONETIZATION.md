# PIN Monetization Strategy — Creative Fabrica First

**Status:** ACTIVE STRATEGY DECISION  
**Date:** 2026-09-18  
**Scope:** PIN Test / Commercial Readiness R0–R3

## Decision

For the first real PIN commercial loop, **Creative Fabrica is the primary monetization channel**.

**Admitad is not required for the initial R0/R1 path** and is retained as a reserve / diversification channel.

This replaces the previous CC0.company strategy, which was based on a misunderstanding of the intended provider.

## Intended first loop

```
Creative Fabrica product/opportunity
→ Hypothesis Agent
→ Content Agent
→ unique Pinterest creative
→ Publisher
→ Guardian authorization
→ Pinterest official API
→ real Pin publication
→ read-back / reality verification
→ affiliate click / conversion measurement
→ Creative Fabrica commission
→ payout evidence
→ Calyx provenance
```

## Commercial readiness mapping

### R0 — Reality Gate
One real Pinterest task is executed end-to-end and independently verified against reality.

Minimum evidence:
- selected Creative Fabrica target;
- intended Pin specification;
- actual Pinterest API result;
- returned Pin identifier / URL;
- independent read-back;
- destination-link verification;
- timestamps;
- hashes / provenance where applicable;
- final PASS only when observed reality matches intended state.

### R1 — Repeatability Gate
The same publication loop can be repeated reliably without false PASS.

### R2 — Value Gate
The loop produces measurable external value such as:
- impressions;
- saves;
- outbound clicks;
- affiliate clicks;
- conversions.

### R3 — Payment Gate
A real external monetary event is independently evidenced.

R3 is not satisfied by clicks, estimated commission, dashboard projections or pending balances alone. A settled/withdrawable commission or actual payout must be observed and preserved as evidence.

## Creative Fabrica verification rule

Creative Fabrica is treated as the **primary monetization provider**, but its commercial mechanics must still be verified against current official terms and the actual account.

Before relying on the channel commercially, preserve evidence for:
1. affiliate account approval;
2. current commission structure;
3. cookie / attribution rules;
4. permitted traffic sources, including Pinterest/social;
5. affiliate-link format;
6. payout thresholds and methods;
7. country / KYC / payment restrictions relevant to the operator;
8. one real successful commission and payout.

No historical commission percentage or third-party description is automatically treated as current VERIFIED truth.

## Content / rights rule

The PIN loop must only use creatives and product media in ways permitted by:
- Creative Fabrica affiliate terms;
- Creative Fabrica content/licensing terms;
- Pinterest policies;
- applicable copyright law.

Where original promotional creatives are created, source assets and transformations should be recorded in Calyx provenance.

## Admitad

Admitad remains available as:
- fallback if Creative Fabrica proves unsuitable;
- later diversification;
- comparison channel for R2/R3 economics.

It should not be added to the initial path unless there is a clear experimental reason.

## Architecture rule

This strategy does not weaken existing PIN capability controls:

- ACTION only through Guardian;
- Publisher requests CREATE_PIN capability rather than holding unrestricted authority;
- secrets remain outside agent-readable business logic;
- Calyx stores evidence/provenance;
- false-pass and repeat gates remain cumulative;
- production logic is not changed merely to manufacture a portfolio result.

## Why this decision

Creative Fabrica is a closer fit to Pinterest than a generic affiliate aggregator because its catalog is heavily visual and naturally aligned with Pinterest discovery behavior.

Removing Admitad from the first loop reduces:
- account / approval dependencies;
- integration surface;
- attribution ambiguity;
- debugging complexity;
- time to first end-to-end commercial test.

At the same time, Creative Fabrica preserves direct monetization potential from the beginning.

---

**Next gate:** create/approve the Creative Fabrica affiliate account, verify current affiliate mechanics from the live account and official terms, then define the exact R0 task contract.
