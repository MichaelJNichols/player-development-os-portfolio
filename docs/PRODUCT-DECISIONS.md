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

## 4. Preserve coach authority

**Decision:** Use automation to recommend and organize work while preserving coach overrides and traceable decisions.

**Why:** Athlete development involves context and judgment that cannot be safely reduced to a fully automated rule set.

**Tradeoff:** The product needs clear role boundaries and must explain when a recommendation was generated versus directly assigned.

## 5. Separate public demonstration from private production use

**Decision:** Maintain a synthetic public demonstration rather than sanitizing private production data at display time.

**Why:** Structural separation is safer than relying on every future screen, query, export, or screenshot to remove youth information correctly.

**Tradeoff:** Two environments create additional release, verification, and documentation work.

## 6. Design guardian and invitation controls before broad pilots

**Decision:** Introduce guardian policy acceptance, recipient-bound invitations, expiration, single use, and wrong-recipient rejection before scaling athlete onboarding.

**Why:** Youth identity and access cannot be treated as a minor account-management feature added after growth.

**Tradeoff:** This delayed more visible coach-dashboard and monetization features.

## 7. Use synthetic evidence publicly

**Decision:** Public screenshots, demonstrations, case studies, and portfolio materials use synthetic identities and records.

**Why:** A portfolio should prove product capability without turning a minor athlete's private development history into marketing content.

**Tradeoff:** Synthetic demonstrations may feel less emotionally compelling than a real player story, but the privacy boundary is more important.

## 8. Document AI-assisted development as an operating system

**Decision:** Maintain requirements, roadmap, tests, decisions, handoffs, releases, and operational controls alongside the build.

**Why:** AI can accelerate implementation, but speed without durable context creates fragile systems and unclear ownership.

**Tradeoff:** Documentation requires discipline and can appear slower in the moment, but it reduces rework and makes technical collaboration more credible.

## 9. Delay payment integration until product and legal gates are clearer

**Decision:** Prepare pricing and payment architecture without making monetization the first priority.

**Why:** Identity, consent, pilot terms, privacy, product value, and support obligations need enough definition before paid access is automated.

**Tradeoff:** Revenue validation occurs later, but the pilot is less likely to create avoidable operational or trust problems.
