# Product Roadmap

**Public snapshot: August 1, 2026**

This roadmap is directional and intentionally omits private implementation details, real athlete data, confidential pilot information, and exact production identifiers.

## Completed foundation

- Problem definition and working single-athlete product loop
- Calendar-aware daily planning
- Athlete readiness, pain, and workload controls
- Coach planning, overrides, corrections, and retained history
- Progress and age-appropriate engagement views
- Mobile-first installable experience
- Synthetic public demonstration
- Product, architecture, safety, privacy, and release documentation
- Isolated multi-athlete staging foundation
- Identity, guardian, coach, invitation, onboarding, and plan-generation gates

## Product corrections completed August 1

The product was reviewed across the private working application, public demo, and isolated staging environment. The following shared behaviors were corrected and retained as parity evidence:

- **Safety now produces the final actionable assignment.** When required pitching rest is active, a throwing assignment resolves to a no-throw recovery day. Safe strength or mobility work can remain, while throwing tools and logging fields are removed.
- **Assignment and logging now share one strength prescription.** Exercise list, set count, and effort rules remain consistent between the daily assignment and completed-work logger.
- **Rolling plan reconciliation now preserves program intent.** Actual workload, readiness restrictions, team-calendar changes, displaced work, recovery sequences, and return bridges are handled through deterministic rules rather than ad hoc date shifting.
- **Responsive navigation parity was restored.** A mobile Progress-view overlap was corrected without changing athlete records or workload logic.

## Current stage: controlled multi-athlete pilot readiness

The technical foundation is ahead of the prior forecast, but external activation remains gated by owner-account, migration, pilot-protocol, and legal evidence.

### Active gate sequence

1. Verify permanent support and privacy contact paths.
2. Establish the real platform-owner account through normal authentication and retain role-boundary and audit evidence.
3. Complete a controlled migration rehearsal with parity, idempotency, and rollback checks.
4. Finalize the pilot protocol and pilot register without activating an external athlete.
5. Complete qualified legal review of guardian, minor-data, privacy, and pilot treatment.
6. Run the weekly readiness review and activate only when every blocking gate has retained evidence.

A target date never overrides a failed safety, privacy, authorization, migration, or legal gate.

## Near-term product work

### Coach operating experience

- Multi-athlete roster and exception dashboard
- Readiness and workload triage
- Plan assignment, review, publication, and override workflows
- Team-calendar management
- Athlete switching and relationship-scoped navigation
- Complete administrator audit coverage

### Pilot learning

- Onboarding completion and abandonment
- Daily assignment usefulness
- Athlete completion and honest-logging behavior
- Coach review and intervention frequency
- Guardian clarity and trust
- Support burden, failure points, and recovery time

### Legal and operating readiness

- Guardian and minor-response treatment
- Support and privacy contact validation
- Pilot consent and acknowledgment flow
- Data-flow and provider inventory
- Retention, deletion, incident, and escalation procedures

## Post-pilot commercialization hypotheses

### Pricing and access

- Pricing and packaging validation
- Manual-paid and complimentary entitlements
- Payment integration after access behavior is proven
- Cancellation, expiration, grace-period, refund, and revocation workflows

### Equipment recommendation infrastructure — MON-003

This initiative is explicitly **post-pilot** and must not delay onboarding, entitlement, migration, legal, or pilot readiness.

The planned equipment library will connect products to coaching context through structured metadata such as age or level, purpose, skills trained, related drills and plans, coach notes, budget and premium alternatives, and multiple provider links.

Product principles:

- Recommendations remain coaching-driven, not sales-driven.
- Products must be personally used, tested, or publicly endorsable.
- Every recommendation explains why it is appropriate.
- The application remains fully functional without affiliate links.
- Provider-independent product records retain a normal purchase-link fallback.

### Governed drill-video workflow

A complete internal drill-video inventory and governance workflow has been documented. Public use remains contingent on rights, attribution, stable hosting, and permission-safe presentation. A limited tooling experiment may proceed only when it does not consume a critical-path pilot slot.

## Later hypotheses

These are not committed features:

- Team-level products
- Instructor or facility accounts
- Additional sports
- Native mobile applications
- Advanced performance analytics
- Automated recommendations across larger datasets
- External wearable or training-system integrations

## Prioritization rule

Work is prioritized in this order:

1. Youth safety and privacy
2. Correct access and identity boundaries
3. Data integrity and reproducible plan behavior
4. Daily athlete usefulness
5. Coach operating efficiency
6. Pilot learning
7. Monetization
8. Broader feature expansion
