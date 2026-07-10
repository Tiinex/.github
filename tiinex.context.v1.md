# Tiinex Context v1

This file is a self-contained orientation pack for a human reader or an LLM that does not follow links.

## Short Answer

Tiinex keeps provenance readable in Markdown artifacts you own.

Provenance means the visible trail around material: where it came from, what changed, what it depends on, what limits apply, and what should not be inferred from it.

The goal is to keep work inspectable, recoverable, portable, and honest about its boundaries instead of leaving important context trapped inside one tool, platform, chat history, private runtime, or later explanation.

## What Tiinex Is

Tiinex is a filesystem-native way to preserve provenance as inspectable artifacts.

An artifact can be a note, trace, decision, evidence record, schema note, policy note, source boundary, workspace entrypoint, or another readable Markdown file that carries bounded material forward.

Tiinex cares about whether a later reader can answer practical questions:

- What is this artifact for?
- Where did the material come from?
- What does it depend on?
- What does it follow from?
- What changed here?
- What are its limits?
- What should not be inferred from it?

## What Tiinex Is Not

Tiinex is not only a public viewer.
Tiinex is not only schema documentation.
Tiinex is not an AI agent.
Tiinex is not a general-purpose AI runtime.
Tiinex is not a replacement for human judgment.
Tiinex is not a hidden memory service that asks readers to trust invisible state.

## AI / LLM Boundary

AI and LLM workflows are important use cases and pressure tests.

They are not the identity boundary of Tiinex.

Do not summarize Tiinex as an AI runtime, agent framework, or LLM handoff product unless a specific current repo or artifact explicitly implements that behavior.

## Core Semantics

- Artifact: a readable Markdown record of some work, claim, decision, source boundary, evidence, policy, or continuation state.
- Provenance: the visible trail around material: where it came from, what changed, what supports it, and what limits apply.
- Root: the starting authority or boundary for a lineage.
- Parent: the declared continuity edge that says what this artifact follows from.
- Origin: where the material came from or what grounds it.
- Transition: how one artifact became the next.
- Policy: explicit boundaries around use, consent, attribution, interpretation, or continuation.
- Workspace: a view over artifacts and sources, not the whole project.

These terms are separate because they describe separate responsibilities.
Tiinex should not flatten them into one generic relation.

## Why Tiinex Exists

Work often loses its provenance.

The result may survive while the source, limits, decision boundary, evidence, or transformation path disappears.

That creates practical problems:

- work becomes hard to inspect
- claims become hard to ground
- trust depends on guessing
- reuse becomes risky
- platform changes can break continuity
- polished output can hide missing evidence

Tiinex tries to preserve enough visible context that interpretation does not depend on blind trust.

## Current Public Grounding

Treat these as the current public grounding surfaces:

- `docs` for schemas, examples, policies, topics, and semantics
- `site` for the current public viewer and reference implementation
- `ai-provenance` only for validator, linting, and provenance pieces that are still current, and only after verifying the specific part

Treat other repositories as historical, experimental, private-in-practice, or stale unless they have been explicitly revalidated.

## Practical Outcome

When Tiinex is working well, a later reader should be able to inspect an artifact and understand:

- the scope of the material
- the declared parent context
- the material origin
- what was changed or concluded
- what is still uncertain
- what limits or policies apply
- what should not be inferred

## Ecosystem Shape

The Tiinex ecosystem spans multiple repositories and surfaces.
Historically or experimentally, different repos have explored different parts of the problem.

Examples include:

- docs and schema material
- provenance tooling
- lineage traversal logic
- VS Code workflow tooling
- viewer or receiver-facing presentation
- AI and LLM workflow experiments

Current grounding is listed separately above.
No single repo should be mistaken for the entire project.

## Bounded Answer To "What Is Tiinex?"

Tiinex keeps provenance readable in Markdown artifacts you own: where material came from, what changed, what it depends on, what limits apply, and what should not be inferred from it.

## Guidance For Continuation

If you are continuing Tiinex-related work, prefer these assumptions:

- artifacts are part of the product, not just side logs
- visible boundaries matter more than polished abstraction
- provenance should remain inspectable near the material
- portability matters more than hiding complexity in one tool
- status and release notes are transient and should not redefine project identity
- first-contact explanations should stay concrete before using internal terms
