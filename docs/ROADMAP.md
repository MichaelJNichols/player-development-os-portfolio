# Product Roadmap

**Public snapshot: August 14, 2026**

This roadmap is directional and intentionally omits private implementation details, real athlete data, confidential pilot information, and exact production identifiers.

## Completed foundation

- Working single-athlete product loop
- Calendar-aware daily planning
- Athlete readiness, pain, and workload controls
- Coach planning, overrides, corrections, and retained history
- Progress and age-appropriate engagement views
- Mobile-first installable experience
- Synthetic public demonstration
- Product, architecture, safety, privacy, and release documentation
- Isolated multi-athlete staging foundation
- Identity, guardian, coach, invitation, onboarding, and plan-generation gates
- Deterministic rolling plan reconciliation
- Shared assignment/logging prescriptions
- Athlete-profile and assigned-coach presentation work
- Release-control and pilot-gate enforcement in source

## Current stage: integrated P2 pilot readiness

P2 has moved well beyond the initial architecture phase, but external activation remains intentionally gated.

The August 14 weekly close retained approximately 49% integrated-pilot readiness. That percentage is an internal readiness indicator, not a launch forecast. Source-level controls and rendered-role infrastructure exist, while hosted Cloudflare acceptance, exact runtime/data-state evidence, cleanup evidence, support UAT, and remaining pilot gates still control activation.

No real Player 2 data or family contact is authorized from this public snapshot.

### Active gate sequence

1. Complete hosted P2 release-control acceptance on the intended Cloudflare runtime.
2. Capture exact Worker, database, identity, and data-state evidence for the supported journey.
3. Complete synthetic/disposable record cleanup evidence.
4. Finish adult-facing support/funding desktop, mobile, and fallback UAT where applicable.
5. Close remaining athlete identity/profile integration and owner acceptance gates.
6. Retain legal, consent, pilot-protocol, migration, entitlement, audit, and support evidence required for external activation.
7. Activate only when every blocking gate passes; dates do not override evidence.

## Recent product-development work

### Athlete and coach experience

- Athlete-profile and assigned-coach context moved through a hosted synthetic mobile review cycle.
- Real-device presentation defects were corrected and disposable review fixtures were removed after acceptance.
- Multi-role rendered journeys and release-prevention controls were added to the P2 source line.

### Support / funding

A canonical voluntary-support experience now exists across approved adult-facing surfaces.

Principles:

- Stripe-hosted payment pages handle payment collection.
- Support remains voluntary and separate from athlete entitlement or coaching access.
- The same support model can be reused across Rogue Baseball Intelligence and approved PDOS surfaces.
- Support must not bypass pilot, legal, identity, or authorization gates.

### Public brand / product surface

The Rogue Baseball Intelligence landing page has been rebuilt around the product story and tested across desktop, tablet, and real mobile devices. It now serves as the public umbrella for Player Development OS, research/scouting work, and future baseball product experiments.

### Scouting Notebook

A separate scouting/research product is now under active development inside the private Rogue Baseball Intelligence repository. Current work includes multi-source baseball data ingestion, refresh workflows, source diagnostics, discrepancy methodology, defense/athleticism and bat-tracking enrichment, value/WAR context, and deployment-aware static-data sharding.

This work is adjacent to PDOS rather than part of the athlete-development pilot critical path.

## Near-term PDOS work

### Pilot readiness

- Hosted P2 journey acceptance
- Complete athlete identity/profile integration
- Owner acceptance
- Entitlement and audit evidence
- Migration and rollback evidence
- Legal and consent closeout
- Pilot protocol and support readiness

### Pilot learning after activation

- Onboarding completion and abandonment
- Daily assignment usefulness
- Athlete completion and honest-logging behavior
- Coach review and intervention frequency
- Guardian clarity and trust
- Support burden, failure points, and recovery time

## Post-pilot commercialization hypotheses

### Pricing and access

- Pricing and packaging validation
- Manual-paid and complimentary entitlements
- Payment integration after access behavior is proven
- Cancellation, expiration, grace-period, refund, and revocation workflows

### Equipment recommendation infrastructure — MON-003

This initiative remains explicitly post-pilot and must not delay onboarding, entitlement, migration, legal, or pilot readiness.

Product principles:

- Recommendations remain coaching-driven, not sales-driven.
- Products must be personally used, tested, or publicly endorsable.
- Every recommendation explains why it is appropriate.
- The application remains fully functional without affiliate links.
- Provider-independent product records retain a normal purchase-link fallback.

### Governed drill-video workflow

The internal drill-video inventory and governance workflow remains documented. Public use is contingent on rights, attribution, stable hosting, and permission-safe presentation.

## Separate portfolio experiment

[Cozi Calendar for ChatGPT](https://github.com/MichaelJNichols/cozi-calendar-chatgpt) is intentionally outside the PDOS roadmap. It demonstrates a reusable integration pattern: read-only external data, deterministic availability logic, an AI-facing tool boundary, Cloudflare deployment, evaluations, and regression testing.

## Later hypotheses

These are not committed PDOS features:

- Team-level products
- Instructor or facility accounts
- Additional sports
- Native mobile applications
- Advanced performance analytics
- Automated recommendations across larger datasets
- External wearable or training-system integrations

## Prioritization rule

PDOS work is prioritized in this order:

1. Youth safety and privacy
2. Correct access and identity boundaries
3. Data integrity and reproducible plan behavior
4. Daily athlete usefulness
5. Coach operating efficiency
6. Pilot learning
7. Monetization
8. Broader feature expansion

Adjacent Rogue Baseball Intelligence experiments may proceed only when they do not weaken the evidence gates or operating discipline of the PDOS pilot path.
