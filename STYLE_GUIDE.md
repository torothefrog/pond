# Pond style guide

Shared conventions for all torothefrog projects. The pond repo is the index of
all projects; this guide keeps them looking and behaving like one family.
Check it before starting or restyling a project.

## Project shape

- Static HTML/CSS/JS only: no build step, no runtime dependencies.
- Hosted on GitHub Pages at `https://torothefrog.github.io/<project>/`.
- Every project gets a lily-pad card on the Pond index (`index.html`) with
  honest chips: readiness ("Ready to play" vs "Experimental prototype") and
  device fit ("Mobile friendly" vs "Best on desktop").
- Fonts and icons are bundled in the repo with their licenses; no runtime CDN.

## Color

The pond palette (as used by the Pond index and Wonnect):

| Role | Hex |
| --- | --- |
| Deep background | `#0b1d13` |
| Secondary background | `#123324` |
| Card / lily pad | `#1d5c38` |
| Lighter pad | `#2e8b57` |
| Frog accent | `#7ee081` |
| Secondary accent | `#7ee0c2` |
| Lily pink | `#f2b8c6` |
| Text | `#e8f5e9` |
| Muted text | `#9fc8aa` |
| Wrong / danger | `#e2543e` |
| Reward / highlight gold | `#ffb703` |

Pages set `<meta name="theme-color" content="#0b1d13">`.

## Typography

- Game UI: Nunito (variable, weights 200-1000), bundled locally as woff2 with
  its SIL Open Font License 1.1. Must keep proper Slovenian ČŠŽčšž glyphs.
- Documents, spreadsheets and the Pond hub page: Roboto Mono.
- Slightly playful, not excessive.

## Icons

- Flat, recolorable SVG icons, inline or bundled with their license (for
  example Google Material Icons, Apache License 2.0).
- Never emoji as UI icons.

## Kids' games

- Icon-first controls, as little text as possible.
- Any visible UI text in UPPERCASE for kids learning to read, preserving čšž.
- Big touch targets; playable with touch, mouse and keyboard.
- Clear right/wrong feedback; gentle error states.

## Behavior

- Mobile and tablet friendly; respect safe-area insets.
- Progress persists in localStorage. Visual-only updates must never rename or
  migrate existing save keys.
- Sound, if any, is generated with Web Audio (no audio assets) and can be muted.

---

Conventions codified from the existing projects (Pond hub, Wonnect, Find the
Frog, Vracker, Clock) and Toro's confirmed design direction of 2 November 2026
(flat icons instead of emoji, playful typography with čšž support) and
7 November 2026 (icon-first, minimal text for kids).
