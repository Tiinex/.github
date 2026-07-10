# Tiinex Context v1

This file is a self-contained orientation pack for a human handoff or an LLM that does not follow links.

## Short Answer

Tiinex saves the context of AI-assisted work as readable Markdown files you own.
Each file can record where it came from, what it follows from, what changed, what it depends on, and how someone can continue later.
The goal is to keep work inspectable, recoverable, portable, and honest about its limits instead of leaving the real context trapped inside one tool or chat history.

The grounded public layer today is mostly plain provenance and readable artifacts.
LLM tooling may help later where useful, but a working general-purpose Tiinex AI runtime should not be assumed.

## What Tiinex Is

Tiinex is a filesystem-native way to preserve AI-assisted work as inspectable artifacts.

An artifact can be a note, trace, decision, evidence record, schema note, handoff pack, or another readable Markdown file that carries bounded work forward.

Tiinex cares about whether a later reader can answer practical questions:

- What is this artifact for?
- What did it come from?
- What does it follow from?
- What changed here?
- What are its limits?
- What would another person or model need to continue from here?

## What Tiinex Is Not

Tiinex is not only a public viewer.
Tiinex is not only schema documentation.
Tiinex is not an AI agent.
Tiinex is not a replacement for human judgment.
Tiinex is not a hidden memory service that asks readers to trust invisible state.

## Core Semantics

- Artifact: a readable Markdown record of some work, claim, decision, context, evidence, or continuation.
- Root: the starting authority or boundary for a lineage.
- Parent: the declared continuity edge that says what this artifact follows from.
- Origin: where the material came from or what grounds it.
- Transition: how one artifact became the next.
- Workspace: a view over artifacts and sources, not the whole project.
- Handoff: enough context for another human or model to continue without guessing.

These terms are separate because they describe separate responsibilities.
Tiinex should not flatten them into one generic relation.

## Why Tiinex Exists

AI-assisted work is often hard to inspect later.
Important context can disappear into chat history, private tool state, or one platform's memory of what happened.

That creates practical problems:

- work becomes hard to recover
- claims become hard to ground
- continuation depends on guessing
- handoffs become lossy
- platform changes can break continuity

Tiinex tries to preserve enough visible context that continuation does not depend on blind trust.

## Current Public Grounding

Treat these as the current public grounding surfaces:

- `docs` for schemas, examples, policies, and semantics
- `site` for the current public viewer and reference implementation, and the strongest public proof that the format works in practice
- `ai-provenance` only for the validator and linting surface that is still current, and only after verifying the specific part

Treat other repositories as historical, experimental, or stale unless they have been explicitly revalidated.

## Practical Outcome

When Tiinex is working well, a later reader should be able to inspect an artifact and understand:

- the scope of the work
- the declared parent context
- the material origin
- what was changed or concluded
- what is still uncertain
- what should happen next

## Ecosystem Shape

The Tiinex ecosystem spans multiple repositories and surfaces.
Historically or experimentally, different repos have explored different parts of the problem.

Examples include:

- docs and schema material
- provenance tooling
- lineage traversal logic
- VS Code workflow tooling
- viewer or receiver-facing presentation

Current grounding is listed separately above.
No single repo should be mistaken for the entire project.

## Bounded Answer To "What Is Tiinex?"

Tiinex is a way to preserve AI-assisted work as readable Markdown artifacts that explain where the work came from, what it follows from, what changed, what it depends on, and how another human or model can continue later.

## Handoff Guidance

If you are continuing Tiinex-related work, prefer these assumptions:

- the artifact is part of the product, not just a side log
- visible boundaries matter more than polished abstraction
- portability matters more than hiding complexity in one tool
- status and release notes are transient and should not redefine project identity
- first-contact explanations should stay concrete before using internal terms