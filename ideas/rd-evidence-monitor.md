# R&D Conversation and Engineering Evidence

## Status

Strategic backlog. Do not allow this larger product to displace the quick-build roadmap.

## Proposition

Capture the engineering journey—not just the final code.

The capability captures contemporaneous software-development evidence from AI conversations and correlates it with repositories, commits, experiments and tests. It identifies material potentially relevant to UK R&D tax-claim preparation without deciding that work qualifies.

## Candidate evidence

- technological baseline;
- advance sought;
- technological uncertainty;
- why a solution was not readily deducible;
- alternatives;
- experiments and prototypes;
- failures and learning;
- measurements/tests;
- resolution or remaining uncertainty;
- routine/commercial work that should be excluded.

## Free Devmanic entry tools

A constrained free product could include:

- single-conversation import;
- secret/redaction review;
- candidate-evidence extraction;
- missing-context questions;
- R&D project canvas;
- evidence-readiness report;
- Markdown/JSON export;
- explicit non-eligibility disclaimer.

## Paid CRANIS2 capability

- continuous multi-agent capture;
- repository, branch, commit, PR, issue, test and release correlation;
- active, low-interruption evidence questions;
- competent-professional review/sign-off;
- immutable originals and versioned annotations;
- claim-period workspace;
- adviser access;
- activity-allocation support;
- evidence-pack export.

## Safeguards

The product must never:

- claim HMRC approval;
- guarantee eligibility or maximise claims;
- classify all difficult development as R&D;
- equate AI-session duration automatically with qualifying time;
- rewrite original evidence;
- transmit source/conversations without explicit consent;
- hide routine or non-qualifying work.

## Architecture

Capture a general `DevelopmentEvidenceEvent` once, then apply independent lenses:

- R&D tax;
- CRA/security;
- architecture decisions;
- AI governance;
- product documentation.

Each lens retains separate classifications, reviewers and decisions.

## Key risk

Conversations may contain source code, secrets, personal/customer data, vulnerabilities and commercial strategy. The production design must be local-first, encrypted, redactable, auditable and explicit about retention.
