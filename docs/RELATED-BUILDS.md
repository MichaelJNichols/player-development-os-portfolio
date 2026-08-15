# Related Builds and Experiments

**Public snapshot: August 14, 2026**

Player Development OS is the primary case study in this repository. The work below is included because it shows adjacent product, integration, data, and operating-system capabilities without pretending that every project is part of PDOS.

## Rogue Baseball Intelligence

Rogue Baseball Intelligence is the broader product umbrella around the baseball work.

Recent public-site work includes:

- a product-led landing-page redesign;
- desktop, tablet, and mobile layout passes;
- real-device mobile corrections after visual review;
- accessibility, navigation, and metadata cleanup;
- a voluntary support/funding section using Stripe-hosted payment flows;
- documentation that keeps support separate from product entitlement and athlete access.

The active application repository remains private.

## Scouting Notebook

The Scouting Notebook is an active baseball research/scouting product being developed inside the private Rogue Baseball Intelligence repository.

### Product direction

The goal is to create a research surface that can bring multiple baseball-data perspectives together while preserving source context and exposing disagreement instead of hiding it.

### Current development evidence

- Static and refreshable data pipelines for multiple public baseball-data sources.
- FanGraphs-derived rate and value context.
- Baseball-Reference WAR/value component indexing.
- Savant defense, athleticism, and bat-tracking enrichment.
- Statcast-style outcome context and coverage notes.
- Career and season-window support.
- Source diagnostics and missing-data handling.
- Discrepancy methodology notes where sources define or calculate concepts differently.
- Sharded static indexes to stay within hosting/deployment constraints as datasets grow.

This is an active build, not a finished scouting platform, and no claim is made that unlike source metrics are directly interchangeable.

## Cozi Calendar for ChatGPT

[Public repository](https://github.com/MichaelJNichols/cozi-calendar-chatgpt)

This is a separate, non-baseball integration experiment built to make a read-only family calendar useful inside ChatGPT.

### What it demonstrates

- Converting an existing calendar feed into a narrow AI-facing tool.
- Cloudflare deployment and redirect handling.
- Deterministic availability calculations rather than relying on free-form model arithmetic.
- MCP-facing tool design.
- Evaluation prompts and regression tests.
- Private live validation without publishing a family's calendar data.

The project is deliberately small. Its value in the portfolio is evidence that the same product approach—identify a repetitive workflow, define a safe boundary, expose structured capability to AI, test it, and document it—works outside the baseball domain.

## Shared operating pattern

Across these projects, the recurring approach is:

1. Start with a concrete user or operating problem.
2. Define the smallest useful product loop.
3. Keep sensitive/private source data out of public evidence.
4. Separate deterministic business logic from model interpretation where correctness matters.
5. Use external services and data sources through explicit boundaries.
6. Retain tests, decisions, release evidence, and known limitations.
7. Expand only after the previous layer is understandable and supportable.

That operating pattern is the common portfolio story; the products themselves remain distinct.
