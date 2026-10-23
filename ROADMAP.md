# Persona 5 Theme - Roadmap

Working branch for the 2.0.0 line: `2.0.0-beta` (every phase below merges into it).
Discipline for each phase: `feature/<phase>-<slug>` branch → commit(s) → merge into `2.0.0-beta` → tag when visually verified.

## Phase 1 - Design foundation (no visual change)

- Reorganize the CSS into clearly labeled sections
- Consolidate the palette into `:root` variables (`--p5-white`, `--p5-black`, accent variants)
- Define reusable patterns once (corner card, skewed button, red-accent highlight) so later phases consume them
- **Milestone:** structure only, no visual change. Tag `2.0.0-beta-1` on merge.

## Phase 2 - Buttons & inputs (2 commits, from the README's "Upcoming Features")

- Commit A: all `[class*="lookFilled"]` button variants (primary/green/danger/brand) - black card + 2px white border + alternating rotate/skew treatment
- Commit B: text inputs & sliders (settings fields, titlebar inputs, volume slider) - consistent focus states. Tag `2.0.0-beta-2`.

## Phase 3 - Context menus & tooltips (1 commit)

- Right-click menus, sub-menus, checkbox/radio rows, hover tooltips
- Black card treatment + P5 hover styling (currently all inherit Discord defaults)

## Phase 4 - Modals & settings (2 commits)

- Commit A: settings navigation + general modal - black background, page navigation, radio/checkbox/toggle rows
- Commit B: dedicated assets - nickname popup, reconnecting screen, welcome banner

## Phase 5 - Chat enhancements (2 commits)

- Commit A: reactions bar, emoji picker, attachment/download cards
- Commit B: threads, forum channels, voice channel tiles (the `itemCard` remap is best-effort until now)

## Phase 6 - Profile popouts (1 commit, replaces the guessed `popout_` remap)

- Requirements check first: inspect the actual user popout DOM structure in the Discord client, then style banner/avatar/name/body sections precisely

## Ongoing housekeeping (any time)

- Update the README to reflect real current features; add a fresh screenshot
- Changelog notes live in release tags (annotated)
