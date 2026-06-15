# Tiinex

Infrastructure for owned continuity.

---

![Tiinex System](../assets/tiinex-roadmap-progress.png)

---

## What Tiinex Is

Tiinex builds continuity and provenance infrastructure around operational reality.

The goal is not AGI, replacement of humans, or hidden orchestration magic.

The goal is making AI-assisted work:

- explicit
- recoverable
- inspectable
- portable
- lineage-aware
- runtime-agnostic

Every interaction can become a trace.  
Every trace can participate in lineage.  
Continuity should survive runtimes, tools, providers, and platforms.

---

## What Works Now

The current Tiinex stack is no longer only a theory or schema exercise.

Working surfaces now include:

- markdown-first provenance artifacts with explicit parent, origin, schema, and integrity boundaries
- bounded lineage traversal that can walk a trace chain backward and preserve origin-recovery candidates
- provenance-first tooling that can read and inspect `.trace.md` artifacts and prove the PoC v1 format in practice
- a simple client-side public-provenance viewer direction whose newer schema surface is pushing toward a v2 receiver experience

The core proof is that provenance can stay portable, legible, and traversable without requiring one opaque runtime to hold the whole story.

---

## Current Public State

The strongest public grounding surfaces today are:

- **docs** for schemas, topics, and readable trace artifacts
- **ai-provenance** for the current PoC v1 provenance/tooling surface
- **lineage-bridge** for bounded lineage traversal and origin-aware reconstruction logic
- **ai-vscode-tools** for local VS Code workflow tooling around adjacent inspection and observability needs

The current `site` repo should not be read as the latest product state.

The newer web-app viewer/schema direction is ahead of the currently proven ai-provenance v1 tooling surface, and the polished public web surface has not yet replaced the older site repo.

---

## Start Here

- **Public docs and trace artifacts** → https://github.com/Tiinex/docs
- **Core provenance tooling** → https://github.com/Tiinex/ai-provenance
- **Lineage traversal engine** → https://github.com/Tiinex/lineage-bridge
- **VS Code workflow tooling** → https://github.com/Tiinex/ai-vscode-tools
- **Experimental feedback and topic tooling** → https://github.com/Tiinex/feedback

Choose the repository that matches the work surface instead of defaulting to `.github`.

---

## Core Principles

### Explicit
No hidden state required.

### Recoverable
Reconstruct what happened and continue forward.

### Observable
Inspect traces, lineage, continuity, and artifacts.

### Adaptable
Move across runtimes, providers, workflows, and environments.

### Yours
Your data. Your rules. Your continuity.

---

## Workflow Philosophy

Tiinex is built around continuity that should be:

- inspectable instead of hidden
- recoverable instead of fragile
- portable instead of platform-locked
- explicit instead of magical

The system intentionally embraces imperfect operational reality:

- degraded states
- partial success
- unresolved outputs
- reconstruction
- continuation under uncertainty

---

## Filesystem-Native by Design

The ecosystem explores:

- markdown-first workflows
- `.trace.md` lineage artifacts
- portable `.trace.zip` exports
- integrity verification
- explicit provenance
- recoverable carry-forward state

The goal is not proprietary containers.

The goal is continuity that survives platforms.

---

## Current Direction

The current direction is to keep pushing toward receiver-safe proof surfaces:

- read-only provenance viewing for external readers
- clearer trust signals around verified, linked, missing, and broken lineage
- continuity that remains understandable outside one editor or provider
- public proof flows that stay truthful even when receiver capability, packaging, and UX are still evolving

The ecosystem remains intentionally modular and runtime-agnostic.

---

## Current State

This is still active work, but the status has changed from pure exploration to early working infrastructure with an important split between proven v1 and emerging v2 surfaces.

Documentation, semantics, workflows, packaging, and UX will continue to evolve.

Current read:

- the provenance/tooling proof is real at PoC v1
- the richer public viewer/schema direction is further ahead conceptually than the currently proven tooling layer
- receiver effectiveness still depends on the receiver and the tooling available on that side

The project is being developed in public and intentionally favors:

- explicit iteration
- inspectability
- recoverability
- operational grounding

over polished illusion.

---

## Philosophy

Foundation first.

A stable continuity layer enables everything that comes next.

---

## Support

If you find the work valuable and want to support continued development:
https://ko-fi.com/Tiinusen
