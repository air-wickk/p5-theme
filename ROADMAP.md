# Persona 5 Theme - Roadmap

Basis for the 2.0.0 line: the `2.0.0-beta` branch now carries the original author's
2.0.0-beta-2 file as the working base. New phases merge into it.

Discipline for each phase: `feature/<phase>-<slug>` branch -> commit(s) -> merge into
`2.0.0-beta` -> tag when visually verified.

## Phase 1 - Author beta as the base (done)

- Adopted the author's beta file wholesale as `P5.theme.css`
- All asset URLs remapped to our GitHub Pages hosting (new `p5-main-menu.png`)
- Meta, site and repo links updated; `-focus-primary` typo and empty rulesets cleaned up

## Phase 2 - Buttons & inputs

- Commit A: bring her dead button rules to life: `lookFilled` primary (red fill,
  invert hover), `colorGreen`, header toolbar hover, plus black-card treatment for the
  voice strip buttons (camera / screen share / activity / soundboard)
- Commit B: text inputs and sliders (replace dead `.slider-1PF9SW` rules with live
  `[class*="slider"]` variants), consistent focus states
- **Milestone:** tag `2.0.0-beta-2` when visually verified

## Phase 3 - Search, menus & overlays

- Port the dead search and filter block (`searchBar`, `queryContainer`, `resultsGroup`,
  search chips, hint values) to live classes, keeping her visuals
- Port the date picker wrappers and context menu rules to live classes
- Cover tooltips and keyboard shortcut cards if the hover styles need siblings

## Phase 4 - Guild rail & channel tree leftovers

- Live ports for the remaining guild rail rules (`tutorialContainer`, `lowerBadge`,
  folder wrappers) and the channel tree block so they stop relying on matches that no
  longer render

## Phase 5 - Chat, friends & voice cards

- Message area, friends list, voice and activity card sections: port their dead
  hashed classes to live ones (the 1.11.1 tag work documented most of these mappings)

## Phase 6 - Popouts & modals

- User popout, nickname popup, notification settings, upload modal, everyone popup:
  port or consciously retire each dead block after checking against the live DOM

## Phase 7 - New polish on a stable base

- Decide the author token system questions she left open (accent candidates,
  `--p5-main-font` usage) and new drop-in effects once everything dead is either
  ported or removed

## Ongoing housekeeping (any time)

- Update the README to reflect real current features; add a fresh screenshot
- Changelog notes live in release tags (annotated)
