# AGENTS.md — codestri-openclaw

Purpose: this repository is the active Codestri website project.

## Primary Agent
- Owner agent: `codestri-manager`
- Mission: implement, test, and ship website changes safely.

## Operating Rules
1. Treat this repo as production-bound web code.
2. Before edits: check `git status` and current branch.
3. Keep changes scoped and reversible.
4. Run validation before handoff:
   - `npm run build`
   - (optional) `npm run dev` sanity check
5. Do not edit deployment secrets in repo files.
6. Document non-trivial decisions in `docs/`.

## Structure Conventions
- `src/` app code
- `public/` static assets
- `docs/` operational notes and deployment maps
- `ops/` automation + legacy archives

## Deploy Notes
- Canonical production mapping should be documented in `docs/production-map.md`.
- Prefer PR/commit trail over ad-hoc manual edits.
