# skill-xray landing page: notes

Built with the landing-page skill (2026-10-14), unattended run: every fallback taken is listed here.

## Product card
| Q | Answer | Evidence |
|---|---|---|
| Q1 seen? | screen | it writes one interactive HTML viewer of a skill (file tree, hover cards, report) |
| Q2 known? | new | no "x-ray for skills" category exists; the closest kin are scored reviews |
| Q3 first step | instant | one shell line copies the folder from the public repo into `~/.claude/skills`; free, no account |
| Q4 proof | none | no public users or quotes; proof = a real x-ray of a real public skill (de-aification) plus a maker note |
| Q5 reader | developers | Claude Code skill authors |

Leaves: real viewer as the centered hero capture (wide product screen, L3); outcome headline, subhead opens with what it is, 3 step how it works before features (L5); primary = the install command with a copy button (L2); friction line free, no account (L6); no pricing; worked example + maker note + honest version label (L10); technical tone, secondary = the source (L11).

## Identity (five levers)
- Type: a mono headline, as if the page were the file being read; sans for body (the viewer's own pair: `ui-monospace` and `ui-sans-serif`). No web fonts, same as the viewer.
- Colour: the viewer's neutral ramp (#0a0a0a ground, #ededed / #9f9f9f / #707070 ink). Accent = the viewer's yellow outline (#fbbf24), the colour of a hovered section in the product. The six meaning colours appear only inside the "what the colours mean" example, as product content.
- Radius: 6px controls, 10px captures, like the viewer's 4 to 8px.
- Copy register: plain, technical, second person, short.
- Peer: the viewer itself; it should read as the same object, not as a marketing skin around it.

## Fallbacks and decisions
- Install source: the public repo `kriss-045/agent-skills` (skills/skill-xray). The published copy differs from the local one only in its description line. Install line tested by extracting into /tmp.
- Demo: a fresh x-ray of the public de-aification skill (demo/de-aification.html). The existing design-showcase x-ray was not used because its annotations name an employer.
- Secondary action: Read the source (GitHub folder).
- Type scale is 6 sizes (landing-page visual.md), above design-lint's 3 text variation warn; the landing-page skill names that exception.

## Checker and eye
- check_page.js: 0 FAIL, 0 WARN (2026-10-14).
- design-lint warns kept: `numbering` fires on the real line numbers inside the colour excerpt (they are the file's line numbers, content not decoration); `text-variations` fires on the 6 size landing-page scale.
- Eye round 1 fixes: the hover card sat below the desktop fold (recropped so the outlined section and card show in the first screen); the mobile hero was a shrunken desktop shot (replaced with the real 390px layout, tapped section with its inline card).

## Hosting
- Vercel CLI on this Mac has no login (device flow needs Kriss), so the site ships on GitHub Pages from this repo. Moving to Vercel later: import the repo in the Vercel dashboard, no build step, output = repo root.
