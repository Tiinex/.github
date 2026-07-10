# Tiinex

Tiinex saves the context of AI-assisted work as readable Markdown files you own.
Each file can say where it came from, what changed, what it depends on, and how someone can continue from there later.
The goal is to keep work inspectable, recoverable, portable, and honest about its limits instead of trapping it inside one app, model, chat history, or platform.

Today the grounded parts are plain provenance, readable artifacts, and continuity structure.
LLM tooling may support that later where it is useful, but it should not be assumed as the current runtime.

---

![Tiinex System](../assets/tiinex-roadmap-progress.png)

Vision map, not a status dashboard. Current working surfaces are listed below.

---

## What Tiinex Does

Tiinex is a way to preserve AI-assisted work as readable artifacts.
Right now the strongest grounded part is plain provenance in readable files.

An artifact can be a note, decision, trace, handoff, evidence record, schema note, or other Markdown file that explains some bounded piece of work.

The important part is not only storing the file. The file should also help a later reader answer practical questions such as:

- What is this?
- Where did it come from?
- What does it follow from?
- What changed here?
- What can I trust?
- What would I need to continue this work without guessing?

## What Tiinex Is Not

Tiinex is not only the viewer.
Tiinex is not only the schema docs.
Tiinex is not an AI agent.
Tiinex is not a replacement for human judgment.
Tiinex is not a hidden memory service that keeps the real state somewhere else.

The files are meant to stay readable on their own.

## Plain Terms

- Artifact: a readable Markdown record of some work, claim, decision, context, evidence, or continuation.
- Root: the starting authority or boundary for a lineage.
- Parent: the declared continuity edge that says what this artifact follows from.
- Origin: where the material came from or what grounds it.
- Transition: how one artifact became the next.
- Workspace: a view over artifacts and sources, not the whole project.
- Handoff: enough context for another human or model to continue without guessing.

These are different jobs. Tiinex does not collapse them into one generic link type.

## Why Someone Would Use It

AI-assisted work often disappears into tools that are hard to inspect later.
You may have a result but not a readable path back to the source, the decision boundary, the parent context, or the limits of the answer.

Tiinex tries to preserve that path in ordinary files.

That makes it easier to:

- inspect what happened
- recover after tool or platform failure
- move work across editors, providers, or runtimes
- hand work to another person or model
- keep claims tied to visible sources and limits

## What Exists Today

Current public grounding surfaces:

- `docs` for schemas, artifact examples, policy material, topics, and Tiinex semantics
- `site` for the current public viewer and reference implementation; it is also the strongest public proof that the format works in practice
- `ai-provenance` for the validator and linting surface that is still current; verify the specific part before treating anything else there as authoritative

Other Tiinex repositories may be historical, experimental, or stale. Do not treat them as current product state unless they have been explicitly revalidated.

Do not assume there is already a general-purpose Tiinex AI runtime behind these surfaces.
The grounded public surface today is mainly readable artifacts, provenance, policies, schemas, and a viewer that can inspect them.

## Start Here

- Public docs, schemas, policies, and artifacts: https://github.com/Tiinex/docs
- Current public viewer / reference implementation, and the strongest public proof that the format works: https://github.com/Tiinex/site
- Validator and linting surface that is still current in ai-provenance: https://github.com/Tiinex/ai-provenance
- Stable identity file for Tiinex itself: ../tiinex.orientation.v1.md
- Self-contained context pack for LLM or handoff use: ../tiinex.context.v1.md

Do not infer current Tiinex direction from older repos without revalidation.

## Longer View

Tiinex is trying to make AI-assisted work less fragile and less opaque.

That means:

- readable artifacts instead of hidden state
- explicit boundaries instead of implied memory
- recoverable continuation instead of one-shot chat history
- portable context instead of platform lock-in
- honest limits instead of polished but untraceable output

This is why terms like continuity, provenance, lineage, and handoff exist in the project. They are not the first thing a reader needs to learn, but they matter once the basic job is clear.

## Status And Releases

Stable identity and definitions live in the orientation files at the repo root.
Transient status, release notes, and implementation snapshots should live under `releases/`.

## Support

If you find the work valuable and want to support continued development:
https://ko-fi.com/Tiinusen
