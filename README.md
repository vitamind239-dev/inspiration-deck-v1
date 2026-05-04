# Inspiration Deck v1

Lightweight browser-based weekly inspiration system with a stable production entry and rotating content.

## How it works

- `index.html` → production entry (always points to `w_cur`)
- `preview.html` → preview entry (bypasses time gating, can target any week)
- `w_cur/` → current live week
- `w_X/` → archived or staged weeks (e.g. `w_4`, `w_5`)

## Weekly flow

1. Prepare next week in a new folder (`w_6`, `w_7`, etc.)
2. Validate using `preview.html`
3. Promote by copying content into `w_cur`

No changes to `index.html` required.

## Purpose

Separate content from code. Keep production stable while allowing simple, repeatable weekly updates.
