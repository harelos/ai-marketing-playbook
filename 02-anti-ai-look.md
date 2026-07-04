# ANTI-AI-LOOK ADDENDUM — "STOP MAKING IT LOOK AI-GENERATED"
Append to the master build prompt. This OVERRIDES defaults.
Root cause: LLMs converge on the statistical average of their training data (distributional convergence). Your job is to actively escape the average.
Tell reference: https://github.com/JCarterJohnson/vibecoded-design-tells

## BANNED BY DEFAULT (negative constraints — the "AI tells")
Do NOT use any of these unless explicitly asked:
- Purple / indigo / violet, and purple→blue gradients ("AI purple").
- Inter, Roboto, or Open Sans as the primary font.
- Generic aspirational headlines: "Build the future", "Elevate your X", "Supercharge your workflow", "Unleash", "Seamless", "Effortless".
- Emoji as section headers or feature-list bullets.
- Everything centered; identical padding + identical border-radius on every element.
- Glassmorphism, neon glows, and default shadcn look shipped untouched.
- Three identical feature cards in a row with a generic icon on top.
- Stock-photo hero of people pointing at laptops; generic AI blob illustrations.
- Vague filler copy. Every word must be specific to THIS product and user.

## PROCESS — do not collapse taste, exploration, and spec into one step
1. DIRECTION FIRST: before any code, write a 3-line art direction — the vibe (name a real brand/app it should feel like), the emotion, and what it must NOT feel like. No "clean and modern" — be specific (e.g. "editorial like Linear, warm like Notion, confident not cute").
2. EXPLORE 3 OPTIONS: propose three genuinely DIFFERENT visual directions (different font pairing, palette, layout personality). Let me pick one. Do not converge on the first idea — the first idea is usually the average.
3. PIN THE SPEC: lock the winner into an explicit design spec (font stack, exact hex palette, spacing scale, radius, motion rules) and build to it.

## MAKE EVERY CHOICE HAVE A REASON (design intent)
State why: this button is large because it's the primary action; this is split into steps because the form is long; only 3 metrics show because those drive the decision. If a choice has no reason, it's a default — replace it.

## CONCRETE WAYS TO LOOK CUSTOM, NOT TEMPLATED
- TYPE: pick a real typeface with personality (Google Fonts / Fontshare https://fontshare.com). Pair a distinctive display font with a clean body font. Use a real type scale; vary weight boldly. Type IS the design.
- COLOR: generate a real palette first, then hand the AI the hex codes as hard constraints. Tools: https://coolors.co , https://www.realtimecolors.com , https://huemint.com . One confident brand color + a warm/cool neutral ramp (not gray-500). Near-black text, off-white surfaces, never #000/#fff.
- LAYOUT: break the grid on purpose somewhere — an asymmetric hero, an oversized number, an off-center headline. Sameness comes from perfect symmetry.
- DETAIL: give it ONE signature element (a custom cursor, a distinctive card treatment, a branded empty state, a hand-tuned chart). Craft lives in specifics.

## MICROINTERACTIONS — the premium tell, used with RESTRAINT
- Motion carries the brand: playful vs. understated to match the product voice.
- Restraint is the point: if everything animates, nothing stands out. Keep most of the UI quiet; spend motion on the few moments that deserve weight (primary CTA, success, state change). 150–250ms, eased, respects reduced-motion.
- "Slightly off" motion reads as cheap. Tune timing and easing deliberately.

## SELF-AUDIT BEFORE DONE
Ask: "Would someone look at this and instantly say 'an AI made this'?" Check against the BANNED list and the vibecoded-design-tells repo. If any tell is present, remove it and re-run. Score distinctiveness /10; if under 9, redo the DIRECTION step — do not just tweak colors.
