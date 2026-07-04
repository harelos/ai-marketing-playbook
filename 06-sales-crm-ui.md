# SALES / CRM / OUTREACH UI PATTERNS
Append to the master build prompt. Use for any pipeline, lead-list, CRM, or cold-outreach tool. Codified from the CURRENT, source-verified UIs of Linear, Attio, Superhuman, HubSpot, Pipedrive, Apollo, Folk, Clay, and AI-SDR tools (July 2026 research). Verified hex/font values are marked; unconfirmed ones are tagged (uncertain) — sample those from live screenshots before locking.

## WHAT THE BEST-IN-CLASS TOOLS ACTUALLY DO

### Linear — gold standard for dense product UI (high-confidence, multi-source)
- Dark-first "surface ladder": canvas `#010102` → panels `#0f1011` → `#141516` → `#18191a`. Elevation comes from each surface being a hair LIGHTER, NOT from drop shadows. No shadows, no gradients.
- Hairlines/borders: `#23252a` → `#34343a`. Text: ink `#f7f8f8`, muted `#d0d6e0`, subtle `#8a8f98`. Most text/icons sit at 40-60% opacity grey; full color is reserved.
- ONE accent — "Linear Lavender" `#5e6ad2` (hover `#828fff`) — used ONLY on brand mark, focus rings, primary CTAs. Never a decorative fill.
- Whole theme generated in LCH color space from 3 variables (base, accent, contrast) → perceptually consistent contrast. ~22 color tokens total.
- Type: custom "Linear Display" (Inter-derived) for headings at weight 600 with aggressively negative tracking (80px display at ~-3px), "Linear Text" (Inter) body at 400, buttons 500. Size scale 12/14/16/18/20/22/28/40/56/80.
- Everything on a strict 4px grid. List rows ~36-40px. Left sidebar nav (~220px), 56px top bar. Radii: 4px chips, 6px tags, 8px buttons/inputs, 12px cards, pill for status/toggles.
- Signature status system: small CIRCULAR PROGRESS-RING icons (Backlog dashed → Todo empty → In Progress partial-fill → Done full-fill+check), not colored word-blocks. Priority = small stacked signal-bar glyphs.
- Cmd+K command palette IS the interface; single-letter composable shortcuts, discoverable on hover; optimistic/instant transitions (~60-120ms).

### Attio — design-forward modern CRM (verified)
- "Hunter Black" `#1C1D1F` (near-black with a GREEN undertone) foundation; single primary "Attio Teal" `#3ABDAF` for focus/primary/data highlights. Cool neutrals, deliberately "alive" vs enterprise blue.
- Spreadsheet-dense editable-cell tables, hairline borders, clean modern grotesque. Expensive via restraint + precise type + tight grid.

### Superhuman — keyboard-first email (structure verified; hex/font uncertain)
- Light, warm-minimal, spacious; built from ~5 grays. NO pure black / NO pure white; body text at ~90% black opacity.
- Accent-on-dark rule worth stealing: LOWER brightness + RAISE saturation so an accent keeps identity without bleeding into adjacent text.
- Three-pane layout, "Split Inbox" streams with unread-count badges. Cmd+K natural-language command palette that ALWAYS shows the shortcut next to each action + trains muscle memory ("next time try [key]"). vim nav (J/K/H/L), optimistic UI rendering before server confirm with undo as safety net. Internal target ~50ms/interaction. Premium feel = perceived instant response + typographic restraint.

### Pipedrive — pipeline CRM (verified; most copyable pattern here)
- Single confident primary green `#08A742`. Light + dark themes.
- Vertical KANBAN: deal cards in stage columns; each stage header shows DEAL COUNT + TOTAL VALUE; stages collapse/expand; you can drag into a collapsed stage.
- COLOR = URGENCY, NOT DECORATION — the defining pattern: deal cards carry activity arrows that ALSO drive sort order. Red = overdue (floats to top), green = due today, yellow = nothing scheduled, grey = future. "Rotting deals rise." Steal this: encode meaning in color and let it sort.
- Toggleable CELEBRATORY ANIMATION on deal-won (Preferences → Interface). A deliberate, praised dopamine hook. HubSpot users are literally begging for the same in community threads → strong signal a tasteful close-won moment matters.

### HubSpot — pipeline CRM (verified brand)
- Primary "Coral" `#FF7A59` (their rationale: coral = success); text/structure "Charcoal" `#33475B` (a cool blue-grey, NOT pure black); secondary "Calypso" `#00A4BD`. Light UI, cool neutrals.
- Type: Lexend Deca (body) + Queens (serif headings) on brand; product historically Avenir Next. Deal board offers table ⇄ kanban toggle.

### Apollo / Folk / Clay (style verified, exact hex uncertain)
- Apollo: 2024-25 rebrand to "warm, energetic, a bit bolder than SaaS" + depth/elevation + dark mode + a token system (13k tokens); dense VIRTUALIZED spreadsheet grid for enrichment (inline edit, per-source columns, Sent/Scheduled/Booked status labels).
- Folk: warm cream/off-white, rounded cards, avatar chips, pastel tag colors, approachable — proof warm can still be pro.
- Clay: cream/beige canvas + terracotta/clay-orange accent, playful brand over a serious spreadsheet grid.

### Cold-email dashboards — Instantly / Smartlead / Lemlist (brand hex verified; in-app tokens inferred)
- LIGHT theme is the category default in-app (Instantly is light-only with an upvoted dark-mode request; Smartlead light; Lemlist light+dark). A clean white/light-gray workspace + one saturated BLUE accent is the safe, trustworthy baseline; dark mode is a differentiator, not the default.
- BLUE is the category trust color: Instantly `#0081FF` (+ periwinkle secondary `#927FF2`, near-black `#141414`), Lemlist `#316BFF` (+ navy `#213756`). Keep palette tiny: one blue accent + cool neutrals + semantic green/red. Instantly uses purple only as a subtle SECONDARY — avoid the generic AI indigo-purple gradient as primary.
- Campaign data lives in DENSE ROWS (sent/opened/replied/bounced/positive as inline columns), KPI tiles reserved for the analytics overview. Master/Unified inbox mimics a real email client (left sidebar: Inbox/Sent/Important/Snoozed…) with saveable filtered "Views" + intent tags (interested/OOO/unsubscribe/bounce).
- Lemlist's GRANULAR LEAD-STATUS TAXONOMY is the best model to copy for CRM stages: enriching → to launch (ready for review) → waiting → in progress → sent → replied, plus skipped/paused — each a colored pill. Rich, human, first-class.
- Lesson in cheap vs premium: Smartlead is powerful but reviewers call it "outdated / designed by engineers not UX" — density alone isn't premium. Lemlist feels most premium via restraint + cohesion + real theming + human status language, not loud color.

## DO — concrete rules (with verified specifics)
1. ONE accent, guarded. Reserve it for primary CTA, focus ring, active nav, key data highlight only (Linear `#5e6ad2`, Attio `#3ABDAF`, HubSpot `#FF7A59`). Never spray it.
2. SURFACE LADDER, not shadows. Build depth from a 3-4 step lightness ramp + 1px hairline (Linear: `#010102`→`#0f1011`→`#141516`→`#18191a`). Reserve drop shadows for truly floating layers (popovers) if at all.
3. NEVER pure #000 / #FFF. Darkest ~`#0A0B0D`, lightest text ~`#F5F6F7` at ~90% opacity. Tint neutrals slightly (Attio green-tint, Folk warm-cream) — pick one temperature.
4. COLOR = MEANING. Define ~4 semantic hues (success/warn/error/info) and make color encode STATE or URGENCY. Steal Pipedrive: color that also drives sort (overdue floats up). Never decorative color.
5. On dark, tune accents perceptually: lower brightness + raise saturation so they don't bleed (Superhuman rule).
6. DENSITY IS A FEATURE. Rows 36-40px, hairline dividers (`rgba(255,255,255,.06)` dark), left-align text, right-align numbers, tabular figures. Scan 15+ leads per screen.
7. DEAL VALUE ALWAYS VISIBLE. Money in mono numerals on every row + a running TOTAL per stage/column header (deal count + summed value). It's the point of the tool.
8. PIPELINE = ORDERED STAGES. Kanban columns OR a fixed-order status field, cold→won left-to-right. Advancing a lead = one click/drag. Offer a table ⇄ kanban toggle.
9. STATUS as a small dot / ring-icon / low-chroma pill (≤ text size). Linear's progress-ring is the classiest; a 6-8px dot or a 12-16%-opacity tinted pill also works. Never full-saturation blocks.
10. TWO TYPEFACES MAX: a UI/body sans (Inter/Geist/General Sans) + optional tight display cut. Ship variable fonts. Hierarchy from size+weight+color, never underlines/text-shadow.
11. STRICT 4px GRID + consistent radii (6px inputs, 8-10px cards, 12px modals). Off-grid spacing (7/11/13px) is the #1 amateur tell.
12. LEFT SIDEBAR nav ~220-240px, collapsible; thin top bar. Active nav = accent text + subtle accent-tinted pill, not a heavy fill.
13. Cmd+K COMMAND PALETTE + single-letter shortcuts shown inline. Keyboard-first is a core trust signal in this category (Linear, Superhuman). Even a lightweight version reads as "fast/serious."
14. OPTIMISTIC UI: render the action before the server confirms, undo as the net. Perceived instant response = the premium feel. Motion 80-160ms ease-out; no bouncy easing on routine hovers.
15. ONE earned CELEBRATION: close-won only, ~1.5s, toggleable (Pipedrive pattern). One reward moment, tasteful, never confetti on minor actions. See 05-gamified-adhd-without-tells.md.
16. Ship empty/loading/dead states. "No leads match — loosen filters." Skeleton rows not spinners. A bounced email stays visible struck-through + faded.

## DON'T (what these premium tools avoid)
- No Bootstrap-blue `#007BFF`, no default Material purple, no purple-pink "AI-SDR" gradient as primary surface language.
- No pure #000/#FFF; no flat zero-hue grays.
- No drop-shadow-everything for elevation in dense UI — use the lightness ladder.
- No >2 typefaces; no Inter-nobody-chose with 4 fighting weights and no system.
- No saturated full-row/full-card status fills (turns a pipeline into a traffic jam). Dots/pills/rings carry state.
- No burying the money or hiding the primary action in a "…" menu.
- No animating everything; no 400ms+ transitions; no confetti on routine actions.
- No decorative color, and don't crowd the one accent across nav+buttons+links+badges+charts at once (dilution kills the "one confident brand" signal).
- No emoji as functional status in a pro tool (Folk-style warmth in tags is fine; deal stage is not).
- No color-only status — pair every color with a shape/label (accessibility).

## 3 ART DIRECTIONS (pick one, state it before coding)
A. "DENSE OPERATOR" (Linear + Attio). Dark: canvas `#0B0C0E`, panel `#131417`, card `#1A1C20`, hairline `rgba(255,255,255,.07)`, text `#F5F6F7`/muted `#8A8F98`; ONE accent Teal `#3ABDAF` or Lavender `#5e6ad2`; semantics `#3FB950/#D29922/#F85149`. Inter/Linear-Display type, 4px grid, 38px rows, ring/dot status, Cmd+K. For a power-user SDR who lives in the tool. Expensive via speed + restraint.
B. "WARM HUMAN CRM" (Folk + Clay). Light: canvas cream `#FAF8F4`, card `#FFFFFF`, hairline `rgba(0,0,0,.06)`, ink `#1C1D1F`; accent terracotta/clay `#E4744C` (uncertain — sample live); pastel segment tags. Rounded geometric sans, 10px cards, soft one-step elevation, avatar chips, one deal-won celebration. For founder-led/relationship selling. Expensive via warmth + precision.
C. "WARM MOMENTUM DESK" (Harel's Agent Sales Machine — HubSpot energy, honestly gamified). Warm charcoal `#141210`, gold `#E8A33D` energy accent + green `#4FB477` money-in; oversized tabular money odometer as the signature; dense folded accordion, mono data, tasteful close-won burst (2-3 brand hues only). For a solo operator who needs visible-progress dopamine. Expensive via type + reward timing, not neon. Pairs with 05-gamified-adhd-without-tells.md.

## SELF-AUDIT
- Total pipeline value + every lead's value visible without clicking? If no, fix.
- One consistent semantic color system, or a rainbow? Cut to ~4, make each mean something.
- Depth from a lightness ladder + hairlines, or shadow-everything? Rebuild as a ladder.
- Rows dense enough to scan 15+ leads? If giant cards, tighten to ~38px.
- One clear primary action per view; accent not diluted across everything?
- Does it look like Attio/Linear (trusted) or a crypto/AI-SDR gradient demo (not)? If the latter, re-run the direction step.

## CONFIDENCE / SOURCES
Verified: Linear (`#010102`/`#0f1011`/`#141516`/`#f7f8f8`/`#5e6ad2`, LCH themes, 4px grid, ring status, no shadows), Attio (`#1C1D1F`, `#3ABDAF`), Superhuman (5-gray, no pure b/w, 90% text, brightness-down/sat-up, Cmd+K, vim nav, optimistic UI), HubSpot (`#FF7A59`/`#33475B`/`#00A4BD`, Lexend Deca + Queens), Pipedrive (`#08A742`, activity-arrow urgency-color+sort, per-stage count+total, toggleable won animation), Apollo (token system, dark mode, virtualized grid, Sent/Scheduled/Booked labels).
Uncertain — sample live before locking: exact hex for Folk, Clay, Apollo, Instantly, Smartlead, Lemlist, Salesforge, Persana; Pipedrive's secondary purple/yellow + dark hexes; in-app product fonts (differ from brand-site fonts).
Refs: linear.app/brand · linear.app/now/how-we-redesigned-the-linear-ui · mobbin.com/colors/brand/linear · attio.com · blakecrosley.com/guides/design/superhuman · help.superhuman.com · brandpalettes.com/hubspot-logo-colors · brandfetch.com/pipedrive.com · pipedrive.com/en/blog/dark-theme · marksgroup.net (Pipedrive won-animation) · apollo.io/tech-blog (visual identity + spreadsheet UI).
