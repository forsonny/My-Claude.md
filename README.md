# My CLAUDE.md

A curated `CLAUDE.md` you can install into your Claude configuration folder to steer Claude toward shipping distinctive, production-ready UI with strong information hierarchy, intentional minimalism, accessibility, and performance discipline.

This repo is intentionally small: the value is in the instruction file.

## What’s inside

- `CLAUDE.md`: User-level instructions that
  - Emphasize “do it now”, stay on-scope, and prioritize deliverables over narration
  - Default to a Senior Frontend Architect + avant-garde UI designer stance
  - Enforce a minimal, purposeful design philosophy
  - Set implementation standards (semantic HTML, WCAG-minded defaults, composable components)
  - Add a deep-reasoning mode via the `ULTRATHINK` trigger
  - Add an automatic multi-step execution pipeline (MAKER), with opt-out commands
  - Include a Windows-specific warning about backslashes in file paths when editing files

## Install

Copy `CLAUDE.md` into your Claude config directory:

```bash
mkdir -p ~/.claude
cp CLAUDE.md ~/.claude/CLAUDE.md
````

If your environment expects a different filename or location, keep the contents the same and adjust the path accordingly.

## How to use it day-to-day

### Normal mode (default)

Expect a tight format:

1. The Code
2. Rationale (brief)
3. Notes (few bullets)

### ULTRATHINK mode

If you write exactly:

```text
ULTRATHINK
```

Claude should switch to deeper, structured reasoning:

* UX psychology (cognitive load, attention flow, error prevention)
* Technical tradeoffs (rendering, state, SSR/hydration if relevant)
* Accessibility (target WCAG 2.2 AA)
* Scalability (boundaries, theming, maintainability)

### MAKER workflow

This instruction set includes an automatic multi-step pipeline for tasks that involve creating, building, implementing, etc.

To bypass MAKER for a one-off request, say:

* `skip MAKER`
  or
* `no MAKER`

## Customization tips

Keep `CLAUDE.md` human-readable and focused. Good additions:

* Common commands (build, test, lint)
* Repo conventions (naming, branching, commit expectations)
* Key directories and architectural boundaries
* “Gotchas” specific to your stack or deployment

## Repository layout

* `CLAUDE.md` - the instruction file
