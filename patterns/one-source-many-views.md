# One source, many views

**The pattern:** Keep one authoritative, human-legible source of systems, interfaces, owners, and provenance. Render every map, impact assessment, and ownership chart from it on demand, instead of drawing each one by hand.

| The source holds | Views rendered from it |
|---|---|
| Systems: layer, owners, vendor, the platform underneath | Impact radius: what a change touches directly, and what it ripples to |
| Interfaces: one per pair of systems, with direction set field by field; kind, method, frequency, owner, criticality, compliance, failure mode | System of record by lifecycle stage, with conflicts and gaps flagged |
| Provenance on every claim: a fact source and a last-verified date | Drift: where the source and telemetry disagree |

**Why it matters:** A hand-drawn map is true on the day it is drawn. Facts trapped in a drawing can't answer the next question, such as what breaks if a vendor changes its API. Separating the facts from the rendering lets one source answer project planning, software assessments, onboarding, and audits.

**The weak point is drift.** Every inventory starts accurate and decays. Each interface names the fact source it can be checked against, which is the [fact source per control axis](fact-source-per-control-axis.md) pattern applied to architecture. The drift report is itself a view, and often the most useful one.

**Prior art:** The model/view split comes from the C4 model and Structurizr. One YAML file per entity, kept in git, comes from Backstage's software catalog. What higher ed adds is the lifecycle axes (prospect to alum, candidate to separated) and the system of record per data domain.

**Worked example:** [RCU Systems Atlas](https://rjoy28.github.io/higher-ed-ai-cookbook/demos/rcu-atlas/), built on the fictional Riverside Christian University fixture. Source: [`rcu-systems.yaml`](../test-kitchen/rcu-systems-atlas/rcu-systems.yaml).

*Status: draft, in the Test Kitchen.*
