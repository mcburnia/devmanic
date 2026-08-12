# RepoDocs

## Proposition

Turn a software repository into traceable, reviewable product documentation while distinguishing observed facts, derived facts, inferences and missing human knowledge.

This is not an “AI writes a README” product.

## Target outputs

- product overview and intended purpose;
- supported platforms and installation;
- architecture and repository structure;
- components, interfaces and integrations;
- configuration/environment variables;
- build, deployment and operation;
- data stores and flows;
- authentication, authorisation and security controls;
- testing and observability;
- dependencies/SBOM summary;
- known gaps and questions;
- Markdown, HTML and machine-readable evidence.

## Evidence classifications

| Classification | Meaning |
|---|---|
| Observed | Direct repository evidence |
| Derived | Mechanically calculated |
| Inferred | Interpretation requiring review |
| Declared | Supplied/confirmed by a human |
| Missing | Required information not found |
| Conflicting | Evidence disagrees |
| Not applicable | Reviewed exclusion |

Every material generated claim should retain its source evidence and confidence.

## Pipeline

1. Deterministic repository inspection.
2. Language/framework adapters.
3. Canonical evidence graph.
4. AI-assisted interpretation.
5. Targeted human questions.
6. Review and correction.
7. Documentation generation.

## Constrained MVP

Support public repositories or ZIPs for a narrow ecosystem set:

- Node.js/TypeScript;
- Python;
- Java/Maven or Gradle;
- CMake-based C/C++.

Generate a fixed pack:

1. product overview;
2. technology inventory;
3. repository map;
4. build/run guide;
5. configuration reference;
6. interface/API summary;
7. security-relevant observations;
8. dependency summary;
9. missing-information questions;
10. Markdown ZIP.

## Privacy evolution

Production use should support a local evidence collector so proprietary source need not be uploaded.

## Relationship to other products

- RepoDocs produces written documentation.
- Repo-to-TracMap presents reviewed journeys visually.
- SBOM adapters produce component inventories.
- CRANIS2 continuously maintains governed evidence across releases.

## Excluded MVP scope

- universal language understanding;
- automatic compliance claims;
- private-repository OAuth;
- continuous monitoring;
- document-management workflows;
- full Annex VII generation.
