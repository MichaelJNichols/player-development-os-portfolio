# Major Product Decisions

This document summarizes the decisions that most clearly demonstrate product judgment. It is not a complete technical decision log.

## 1. Start with one athlete before designing a platform

**Decision:** Build and operate the core workflow for one athlete before expanding to multi-athlete use.

**Why:** A narrow production case allowed rapid iteration on daily usefulness, coaching logic, workload handling, and engagement without prematurely building account administration and billing.

**Tradeoff:** The original product architecture could not simply be presented as a finished multi-tenant system. Expansion required deliberate identity, permission, onboarding, and data-boundary work.

## 2. Treat team schedules as product inputs

**Decision:** Make practices, games, travel, and calendar changes part of the daily planning logic.

**Why:** A development plan that ignores the athlete's actual schedule creates conflicts and unsafe workload recommendations.

**Tradeoff:** Calendar ingestion and reconciliation introduce unreliable external data, duplicates, changed events, and exception handling.

## 3. Put pain and readiness ahead of assignment completion

**Decision:** Pain, readiness, and workload gates can modify or stop planned work.

**Why:** Completion metrics are not valuable if the product encourages inappropriate activity.

**Tradeoff:** The system must sometimes produce a less satisfying answer—rest, modify, or consult a qualified professional—rather than always generating a workout.

## 4. Make safety generate the final actionable plan

**Decision:** Workload and safety evaluation occurs before the final daily assignment is presented. A restriction cannot merely appear beside a conflicting workout.

**Why:** Parallel status and assignment systems can produce contradictory guidance. The athlete needs one authoritative action for today.

**Tradeoff:** The original phased assignment may be temporarily replaced by a recovery prescription while remaining visible as context. Safe strength or mobility work may remain, but throwing tools and logging fields are removed.

## 5. Preserve program intent through deterministic reconciliation

**Decision:** Actual workload, readiness restrictions, changed team events, missed work, and displaced sessions are reconciled through explicit rules rather than casual date shifting.

**Why:** Moving a session without preserving its intent, stress category, recovery relationship, and return bridge can distort the larger program.

**Tradeoff:** The reconciler requires more formal state, tests, and coach-review boundaries than a simple editable calendar.

## 6. Generate assignment and logging from one prescription

**Decision:** The visible assignment and completed-work logger use the same strength definition, exercise list, set count, and effort rule.

**Why:** Asking an athlete to perform one thing and log another undermines data integrity and trust.

**Tradeoff:** Shared definitions reduce local screen flexibility, but they eliminate contradictory prescriptions and make later reporting defensible.

## 7. Preserve coach authority

**Decision:** Use automation to recommend and organize work while preserving coach overrides and traceable decisions.

**Why:** Athlete development involves context and judgment that cannot be safely reduced to a fully automated rule set.

**Tradeoff:** The product needs clear role boundaries and must explain when a recommendation was generated versus directly assigned.

## 8. Separate public demonstration from private production use

**Decision:** Maintain a synthetic public demonstration rather than sanitizing private production data at display time.

**Why:** Structural separation is safer than relying on every future screen, query, export, or screenshot to remove youth information correctly.

**Tradeoff:** Two environments create additional release, verification, and documentation work.

## 9. Design guardian and invitation controls before broad pilots

**Decision:** Introduce guardian policy acceptance, recipient-bound invitations, expiration, single use, and wrong-recipient rejection before scaling athlete onboarding.

**Why:** Youth identity and access cannot be treated as a minor account-management feature added after growth.

**Tradeoff:** This delayed more visible coach-dashboard and monetization features.

## 10. Use synthetic evidence publicly

**Decision:** Public screenshots, demonstrations, case studies, and portfolio materials use synthetic identities and records.

**Why:** A portfolio should prove product capability without turning a minor athlete's private development history into marketing content.

**Tradeoff:** Synthetic demonstrations may feel less emotionally compelling than a real player story, but the privacy boundary is more important.

## 11. Document AI-assisted development as an operating system

**Decision:** Maintain requirements, roadmap, tests, decisions, handoffs, releases, and operational controls alongside the build.

**Why:** AI can accelerate implementation, but speed without durable context creates fragile systems and unclear ownership.

**Tradeoff:** Documentation requires discipline and can appear slower in the moment, but it reduces rework and makes technical collaboration more credible.

## 12. Delay payment integration until product and legal gates are clearer

**Decision:** Prepare pricing and payment architecture without making monetization the first priority.

**Why:** Identity, consent, pilot terms, privacy, product value, and support obligations need enough definition before paid access is automated.

**Tradeoff:** Revenue validation occurs later, but the pilot is less likely to create avoidable operational or trust problems.

## 13. Keep equipment recommendations provider-independent

**Decision:** Model recommended equipment as coaching content first, with multiple affiliate providers and a normal purchase-link fallback as optional distribution fields.

**Why:** Product recommendations should remain useful when an affiliate program changes, a provider removes inventory, or monetization links are unavailable.

**Tradeoff:** The equipment library requires structured metadata, editorial standards, disclosure, and link maintenance rather than embedding one retailer's links directly into drills.

## 14. Keep affiliate work behind pilot readiness

**Decision:** Equipment and affiliate infrastructure is a post-pilot initiative and cannot consume a critical onboarding, entitlement, migration, legal, or pilot-readiness slot.

**Why:** Monetization ideas can easily distract from proving the core daily loop, access model, and buyer value.

**Tradeoff:** A plausible revenue stream is deliberately delayed in favor of stronger product evidence.

## 15. Govern drill video use through rights and attribution

**Decision:** Maintain an internal drill-video inventory and workflow, but publish or embed content only when rights, attribution, hosting stability, and youth-safe presentation are clear.

**Why:** Technical ability to link or embed a video does not establish permission or long-term product suitability.

**Tradeoff:** Some useful instructional content remains internal or experimental until the rights path is resolved.
