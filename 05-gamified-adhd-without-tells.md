# GAMIFIED / ADHD-FRIENDLY WITHOUT THE AI-TELLS
Append to the master build prompt. Read AFTER 02-anti-ai-look.md — this resolves the tension between "make it fun, dopamine, money-coming, ADHD" and "don't look AI-generated."

## THE TRAP (why Harel's first Sales Machine looked cheap)
Chasing "gamified + ADHD + exciting" pushed the design straight into the banned list: AI-purple + cyan + lime rainbow, glassmorphism cards, neon glow shadows, emoji as section headers (💰🎉🔥), everything pill-shaped and centered. Result: it read as a crypto/casino demo, not a tool you trust with a $5k/mo deal. Excitement was faked with COLOR and GLOW instead of earned with TYPE, MOTION, and REWARD TIMING.
Rule: dopamine comes from the MOMENT (a number ticking up, a win landing), not from the palette being loud all the time. A calm surface makes the reward moment pop; a loud surface drowns it.

## CORE PRINCIPLE — "calm canvas, loud moments"
Keep 95% of the UI quiet, dense, and confident (Linear/Attio calm). Spend all the energy on the few reward moments that map to real progress. If everything is exciting, nothing is.

## THE ENGINE — map every mechanic to Hooked (Trigger → Action → Variable Reward → Investment)
Ref: Nir Eyal, "Hooked". This is the honest version of "gamification" — it's just a well-built habit loop.
- TRIGGER: the money meter at the top is the first thing seen. Open app → see "$X/mo on the table" → itch to work a lead.
- ACTION: the lowest-friction next step is one click (change a status, copy an email). Never make the core action a form.
- VARIABLE REWARD: closing a lead fires an unpredictable-feeling celebration (count-up + burst + toast). Variability is what makes it addictive — same as a slot machine, but the reward is REAL progress, not random.
- INVESTMENT: every status saved, every verified email, every touched lead makes the board more valuable next session (stored value → loss aversion → return).

## THE 6 MECHANICS THAT WORK (and how to build each without a tell)
1. THE MONEY ODOMETER. One oversized tabular number (the signature element). Animate it counting up on every change (ease-out cubic, ~500ms, `font-variant-numeric:tabular-nums` so digits don't jump). This is the single biggest dopamine driver — real, honest, and looks premium because it's just great typography, not neon.
2. PROGRESS BAR / % WORKED. Loss-aversion engine: a half-full bar nags to be filled. Solid single-accent fill, not a rainbow gradient. Milestone copy ("12 booked") beats a raw number.
3. STREAK / COUNTER. "12 wins · 40 touched" in mono. Quiet by default; it's the ambient scoreboard, not a flashing badge.
4. WIN CELEBRATION. On a real close only: a SHORT burst (~18-20 particles, 1s, brand colors ONLY — 2-3 hues max, never 6-color rainbow) + a toast with specific copy ("Closed — $5,000/mo. On a roll."). Tasteful confetti = few pieces, brand palette, fast, gone. Casino confetti = many pieces, rainbow, slow, looping.
5. STATE COLOR, SPARINGLY. Won/verified = the ONE positive accent (a confident green). Everything else stays neutral. Color means something; it's not decoration.
6. INSTANT FEEDBACK ON EVERYTHING (ADHD需求). Every click confirms in <100ms: "copied" flips on the button, row lifts 1px on hover, status change instantly re-animates the meter. Latency kills the loop for an ADHD brain; responsiveness IS the reward.

## ADHD-SPECIFIC DESIGN RULES
- REDUCE CHOICE PARALYSIS: collapse everything by default (folded accordion). One open lead at a time = one decision at a time. Never show 147 open cards.
- ONE OBVIOUS NEXT ACTION per view. The primary button is visually loudest; secondary actions are quiet outlines. Don't present 5 equal-weight buttons.
- CHUNK + LABEL: short mono section labels (uppercase, letter-spaced) so the eye can scan and jump. Dense but scannable beats sparse-and-endless-scroll.
- MOMENTUM OVER PERFECTION: make starting trivial (status dropdown, copy button) so the first action costs nothing. The loop, once entered, self-propels.
- PROTECT FOCUS: no autoplaying motion, no looping animation, no things that move while reading. Motion only fires on user action. (Also respect `prefers-reduced-motion` — kill all animation for users who ask.)
- COLOR CAN BE WARM AND ENERGETIC — just DISCIPLINED. Warm charcoal + one confident gold + one green reads as energetic AND expensive. "ADHD colors" does NOT mean neon rainbow; it means high-contrast, warm, and a clear accent that guides the eye.

## PALETTE RECIPE FOR "EXCITING BUT TRUSTED"
- Base: a WARM near-black (e.g. #141210), never pure #000, never AI-purple gradient.
- Surfaces: SOLID layered warm grays (#1D1A15 / #242019), real borders (#2E2A22). No translucent glassmorphism, no backdrop-blur.
- ONE brand/energy accent: a warm gold/amber (#E8A33D) for momentum, money, primary CTA, active state.
- ONE positive accent: a confident green (#4FB477) for won/verified/money-in.
- Semantics only otherwise (muted rose for dead/error). That's it — 2 real colors + neutrals + semantics. The energy is in the number ticking, not the number of colors.
- Depth from subtle dark shadows (`0 10px 26px -14px rgba(0,0,0,.7)`), never colored neon glow.

## TYPE DOES THE EXCITEMENT
- A geometric display face with personality for the big number + headings (e.g. Space Grotesk, Clash, General Sans — NOT Inter/Roboto).
- A clean body face (e.g. Instrument Sans) and a real mono (Space Mono) for data/emails/counters. Mono on numbers reads as "instrument/dashboard" = credible.
- Oversized number + tiny label is the whole trick. Big confident numerals feel like money moving.

## SELF-AUDIT (before calling a "fun" UI done)
1. Screenshot it with all celebrations OFF. Does the resting state look calm, warm, expensive — like a tool a founder would trust? If it looks like a casino at rest, the energy is in the wrong place. Fix.
2. Are there exactly ONE or TWO real accent colors, or a rainbow? Cut to two.
3. Is every animation triggered by a user action, or is something looping/moving on its own? Kill ambient motion.
4. Does the biggest dopamine hit map to a REAL milestone (a close, a booked call), or is it just decoration firing? Tie reward to truth.
5. Run the 02-anti-ai-look banned list. Gamified is NOT an excuse for purple, glow, glass, or emoji headers.
Score fun /10 AND trust /10. Both must be >=9. A fun-10/trust-4 UI loses the deal.
