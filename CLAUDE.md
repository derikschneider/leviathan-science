# CLAUDE.md — Working Rules

General working rules for Derik's projects — kept identical across repos (`vite-lit-1`, `workshop`, this one, `toolkit`, and `derik-workspace`) so they travel to whichever machine/repo you're working from. If these get updated, update all copies together.

## What this repo is

`leviathan-science` (GitHub: `derikschneider/leviathan-science`) — a font foundry site placeholder. Lit + TypeScript + Vite, deployed via GitHub Pages, **must stay public** (GitHub Pages requires it on the free plan, same constraint as `vite-lit-1`). Currently a minimal scaffold: a Spline 3D viewer embed ("Ghost Leviathan" model) plus commented-out variable-font weight/width slider controls (`--ls-wght`/`--ls-wdth` CSS custom properties) — not yet a built-out site, more a working sketch of the foundry's visual identity direction.

## Working Rules
Kept identical across repos (`private`, `vite-lit-1`, `workshop`, `leviathanscience`, `toolkit`) so they travel to whichever machine/repo you're working from. If these get updated, update all copies together.

- Think through the problem first, and read the relevant files in the codebase before proposing or making changes.
- Check in before major changes — lay out the plan and wait for confirmation before executing anything large or hard to reverse.
- Along the way, give a high-level explanation of what changed at each step, not a line-by-line narration.
- Keep every change as small and targeted as possible. Touch as little code as necessary to do the job. No speculative refactors, no scope creep, no unrequested cleanup while in the area — exception: sweeping changes (e.g. deleting an entire project or folder) are fine when explicitly asked for, but scope them exactly to what was requested.
- Never speculate about code that hasn't been opened. If a specific file is referenced, read it before answering. Investigate before making claims about the codebase — no guessing.
- Each project should have a maintained doc describing its architecture end-to-end, kept current as the project changes.
- Verify actual output, not just absence-of-errors — a clean typecheck or a script exiting 0 is not proof of correctness. Check the real result (render it, view the image, spot-check the data) before calling something done, and prefer two independent signals over one when it matters (raw source vs. a summarized fetch, `curl` vs. a browser timeout, and so on).
- Fix real bugs and debt the moment they're found, not after finishing the current task — a fix is cheapest right when it's caught, and deferred debt compounds as fast as new code gets generated.
