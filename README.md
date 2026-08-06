# stillven

![Status](https://img.shields.io/badge/Status-Research_Prototype-purple)
![Stage](https://img.shields.io/badge/Stage-Private_Validation-blue)
![Method](https://img.shields.io/badge/Method-Validation--Governed-lightgrey)
![Instrumentation](https://img.shields.io/badge/Instrumentation-LIVE-blue)

**A research project asking one narrow question: can a system govern its own execution well enough to make a measurable, repeatable difference — and actually prove it?**

Stillven is in active validation. The implementation, datasets, and experimental modules live in private repositories while the architecture is tested against its own success criteria. This page is the only public surface, and it stays deliberately thin until the results earn more.

---

## The Question
Modern operating systems balance responsiveness, throughput, efficiency, and fairness across everything running at once. Under load, the application you actually care about quietly competes with everything you don't — and the cost tends to show up as *inconsistency*, not raw slowness.

Most "optimizers" answer this with static tweaks, blunt cleanups, and confident claims. Almost none of them measure whether any of it actually helped.

## The Principle
> Execution should be governed by validation, not guesswork.

Stillven doesn't "boost" or "clean." It treats every action as a hypothesis — predicted before it runs, measured after, and kept only when the outcome holds up under real use. The bar isn't whether an intervention *sounds* right; it's whether the evidence says it worked, repeatably — that it can be shown, per run, without overclaiming, and that it survives independent adversarial review before it's ever trusted to act on its own.

## What's Public, and What Isn't
The method is the project; the mechanisms aren't on display. Source, telemetry schemas, and results stay private during validation — partly to protect the work, mostly because unvalidated claims aren't worth publishing. Public documentation expands only as internal milestones clear their gates.

---

```text
// ARCHITECTURE LIFECYCLE

  Σ  PROTOTYPE LINEAGE ············· 220 iterations    [ARCHIVED FOUNDATION]
  Σ  NATIVE REBUILD ················ 1,000+ iterations [UNDER VALIDATION]

  v0.1.x   Static execution prototyping ............. [DEPRECATED]
  v0.2.x   Telemetry decoupling & sensor boundary ... [COMPLETE]
  v0.3.x   Governance-loop architecture ............. [COMPLETE]
  v0.4.x   Validation harness ....................... [BUILT]
  v0.4.x   Cross-hardware generalization ............ [EXPANDING]
  v0.5.x   Measurement-integrity overhaul ........... [COMPLETE]
  v0.5.x   Single-surface interface rebuild ......... [COMPLETE]
  v0.6.x   Adaptive trust boundary .................. [COMPLETE · SEALED]
  v0.6.x   Trust-boundary safety hardening .......... [COMPLETE · RED-TEAMED]
  v0.6.x   Measurement-instrument validation ........ [COMPLETE]
  v0.7.x   Pre-registered controlled study .......... [SEALED · IN EXECUTION]

  Research threads:   RQ-001 [deferred — instrument first] · RQ-002 · RQ-003   [under seal]
```

Before a result is trusted, the instrument that produced it has to survive the same scrutiny the result would.
That work turned out to be most of the project — on purpose, and it earned its keep: it retired the project's
original headline metric after measurement showed it was wrong-signed, and the replacement study now runs
under a pre-registered design instead.

**One artifact in this repository is not thin by accident:** `sv265_schedule_commitment.txt` is the SHA-256
commitment of the current study's sealed randomization schedule, published *before* the randomness it commits
to exists, so the design cannot be quietly changed after the results are in. The schedule itself stays in
offline custody until the study freezes. That's the standard the rest of the work is being held to.

---

*Null results count. A probe that misses its pre-registered bar is filed as a miss — not re-framed, not quietly dropped.*

*Not accepting issues or contributions yet. Watch the repo to be here when the seal comes off.*
