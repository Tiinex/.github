# Tiinex

Tiinex keeps provenance readable in Markdown artifacts you own.

Provenance means the visible trail around a piece of material: where it came from, what changed, what it depends on, what limits apply, and what should not be inferred from it.

The goal is to make work inspectable, recoverable, portable, and honest about its boundaries instead of hiding the important context inside one app, platform, chat history, private runtime, or later explanation.

---

![Tiinex System](../assets/tiinex-roadmap-progress.png)

Vision map, not a status dashboard. Some parts are implemented, some are active direction, and some are ambition. Current public grounding surfaces are listed below.

---

## What Tiinex Does

Tiinex is a way to preserve provenance as readable artifacts.

An artifact can be a note, decision, trace, evidence record, schema note, policy note, source boundary, workspace entrypoint, or other Markdown file that explains a bounded piece of material.

The important part is not only storing the file. The artifact should help a later reader answer practical questions such as:

- What is this?
- Where did it come from?
- What does it depend on?
- What does it follow from?
- What changed?
- What can I trust?
- What are the limits?
- What should not be inferred from it?

## Why Markdown Artifacts

Markdown is readable, portable, diffable, and works across many tools.

Tiinex uses Markdown because the important context should not require a private database, a single app, a hidden model memory, or a vendor dashboard before a person can inspect it.

The artifact should carry enough meaning that another reader can see the boundary of the material before trusting or continuing from it.

## What Tiinex Is Not

Tiinex is not only the viewer.
Tiinex is not only the schema docs.
Tiinex is not an AI agent.
Tiinex is not a general-purpose AI runtime.
Tiinex is not a replacement for human judgment.
Tiinex is not a hidden memory service that keeps the real state somewhere else.

AI and LLM workflows are important use cases and pressure tests. They are not the identity boundary of the project.

## Plain Terms

- Artifact: a readable Markdown record of some work, claim, decision, source boundary, evidence, policy, or continuation state.
- Provenance: the visible trail around material: where it came from, what changed, what supports it, and what limits apply.
- Root: the starting authority or boundary for a lineage.
- Parent: the declared continuity edge that says what this artifact follows from.
- Origin: where the material came from or what grounds it.
- Transition: how one artifact became the next.
- Policy: explicit boundaries around use, consent, attribution, interpretation, or continuation.
- Workspace: a view over artifacts and sources, not the whole project.

These are different jobs. Tiinex does not collapse them into one generic link type.

## Why Someone Would Use It

Work often loses its provenance.

A useful result might survive while the path back to its source, limits, decision boundary, or evidence disappears. That makes it hard to review, recover, reuse, or explain what happened.

Tiinex tries to preserve that path in ordinary files.

That makes it easier to:

- inspect what happened
- keep claims tied to visible sources and limits
- recover after tool or platform failure
- move material across tools or repositories
- review boundaries before trusting a result
- continue from explicit context instead of guessing

## What Exists Today

Current public grounding surfaces:

- `docs` for schemas, artifact examples, policy material, topics, and Tiinex semantics
- `site` for the current public viewer and reference implementation
- `ai-provenance` for the validator, linting, and provenance pieces that are still current; verify the specific part before treating anything else there as authoritative

Other Tiinex repositories may be historical, experimental, private-in-practice, or stale. Do not treat them as current product state unless they have been explicitly revalidated.

Do not assume there is a general-purpose Tiinex AI runtime behind these surfaces.

The grounded public surface today is mainly readable artifacts, provenance, policies, schemas, and a viewer that can inspect them.

## Start Here

- Public docs, schemas, policies, and artifacts: https://github.com/Tiinex/docs
- Current public viewer / reference implementation: https://github.com/Tiinex/site
- Partially current provenance validation/linting surface: https://github.com/Tiinex/ai-provenance
- Stable identity file for Tiinex itself: ../tiinex.orientation.v1.md
- Self-contained context pack for reader or LLM use: ../tiinex.context.v1.md

Do not infer current Tiinex direction from older repos without revalidation.

## Longer View

Tiinex is trying to make provenance less fragile and less opaque.

That means:

- readable artifacts instead of hidden state
- explicit boundaries instead of implied memory
- visible source and change context instead of polished but untraceable output
- portable context instead of platform lock-in
- honest limits instead of claims detached from evidence

This is why terms like provenance, lineage, root, parent, origin, transition, policy, and workspace exist in the project. They are not the first thing a reader needs to master, but they matter once the basic job is clear.

## Status And Releases

Stable identity and definitions live in the orientation files at the repo root.
Transient status, release notes, and implementation snapshots should live under `releases/`.

## Support

If you find the work valuable and want to support continued development:
https://ko-fi.com/Tiinusen
