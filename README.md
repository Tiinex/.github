# Tiinex Organization Profile Repo

This repository carries the source for the public Tiinex organization profile and shared profile assets.

The public profile lives in [`profile/README.md`](profile/README.md).

## Current Purpose

This repo is the organization-level identity surface. It should explain Tiinex before any individual repo, viewer, schema bundle, experiment, or old tool claims authority.

The current public identity is provenance-first:

> Tiinex keeps provenance readable in Markdown artifacts you own.

Provenance means the visible trail around a piece of material: where it came from, what changed, what it depends on, what limits apply, and what should not be inferred from it.

## Current Public Grounding

Current public grounding surfaces are:

- `docs` — schemas, artifact examples, policy material, topics, and Tiinex semantics
- `site` — the current public viewer and reference implementation
- `ai-provenance` — partially current; only the validator, linting, and provenance pieces that are still actively used should be treated as current without fresh validation

Other Tiinex repositories may be historical, experimental, private-in-practice, or stale. Do not present them as current without revalidation.

## AI / LLM Boundary

AI and LLM workflows are important pressure tests and possible use cases for Tiinex, but they are not the identity boundary of the project.

Do not describe Tiinex as an AI runtime, agent system, or LLM handoff product unless a specific repo or artifact explicitly implements that behavior and is current.

## What Lives Here

- the public organization profile source
- shared profile assets used by that profile
- stable orientation and context files for first-contact readers
- repo-level context for the `.github` surface

## Stable Files

- [`profile/README.md`](profile/README.md) — public GitHub organization profile
- [`tiinex.orientation.v1.md`](tiinex.orientation.v1.md) — stable project identity
- [`tiinex.context.v1.md`](tiinex.context.v1.md) — self-contained context for readers and LLMs
- [`tiinex.orientation.manifest.v1.json`](tiinex.orientation.manifest.v1.json) — machine-readable map of entrypoints and authority

## Status And Releases

Transient status, release notes, and implementation snapshots should live under `releases/`.

Do not let release notes replace the stable identity files.
