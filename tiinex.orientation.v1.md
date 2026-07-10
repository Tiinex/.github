# Tiinex Orientation v1

Tiinex preserves AI-assisted work as readable Markdown artifacts that people own.
Those artifacts are meant to stay useful after the original tool session is gone.
They should help a later reader see what happened, what the work depends on, where material came from, what changed, and what can be continued next.

Today the strongest grounded layer is plain provenance and continuity in readable files.
Future LLM tooling may support that work, but it should not be assumed as the current runtime baseline.

## Core Identity

Tiinex is a filesystem-native approach to preserving AI-assisted work.

It is not one app.
It is not one viewer.
It is not one schema repo.
It is not one model provider.

It is a way to keep work inspectable, recoverable, portable, and bounded through readable artifacts.

## What Tiinex Preserves

Tiinex artifacts can preserve:

- context
- claims
- decisions
- evidence
- traces of work
- continuation state
- handoff material
- policy and boundary notes

The exact file type can vary, but the artifact should remain readable without requiring hidden application state.

## Continuity Model

Tiinex uses several distinct concepts on purpose.

- Root: the starting authority or boundary for a lineage.
- Parent: what this artifact directly follows from.
- Origin: where the material came from or what grounds it.
- Transition: how one artifact became the next.
- Workspace: a view over artifacts and sources, not the whole project.
- Handoff: enough context for another human or model to continue without guessing.

These concepts must not be collapsed into one generic link idea, because they answer different questions.

## Non-Goals

Tiinex is not:

- an autonomous agent that should replace humans
- a hidden memory layer that keeps the real context somewhere opaque
- a claim that every artifact is complete or correct
- a promise that one repo or one UI represents the whole system

Tiinex should make limits easier to see, not easier to hide.

## Ecosystem Shape

Historically or experimentally, Tiinex has explored surfaces such as:

- schemas and examples
- provenance tooling
- lineage traversal
- VS Code workflows
- viewer and receiver surfaces

Current grounding is listed separately below.
None of those alone defines all of Tiinex.

## Current Public Grounding

The public surfaces that should currently be treated as grounded are:

- `docs` for schemas, artifacts, policy material, and semantics
- `site` for the current public viewer and reference implementation, and the strongest public proof that the format works in practice
- `ai-provenance` only for the validator and linting surface that is still current, and only with local verification of the specific part

Other repositories may be historical, experimental, or stale and should not be treated as current without revalidation.

## Stable Reading

If someone asks "What is Tiinex?", the bounded answer is:

Tiinex is a way to save AI-assisted work as readable Markdown files that explain where the work came from, what it follows from, what changed, and how it can be continued later.