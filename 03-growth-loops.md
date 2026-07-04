# GROWTH LOOPS (make it COMPOUND) — replaces "network effects" section
Core idea (Reforge / Brian Balfour, "Growth Loops are the New Funnels"):
A funnel is one-way and leaky — growth stops when spend stops. A LOOP feeds its output back as the next input, so it compounds exponentially. Every durable company runs on >=1 compounding loop, not a bigger funnel.
Ref: https://www.reforge.com/blog/growth-loops

## BEFORE BUILDING, DESIGN THE LOOP EXPLICITLY
Write it as a closed circle with 4 stages, and name each for THIS product:
  NEW USER -> ACTION they take -> OUTPUT that action creates -> that OUTPUT exposes/creates the NEXT new user -> repeat.
If you can't draw a closed loop, you only have a funnel. Fix that first.
State the loop's k-factor lever and its CYCLE TIME (shorter time = faster compounding — optimize to shorten it).

## PICK A PRIMARY LOOP (at least one; the best products stack two)

1) VIRAL LOOPS — pick the sub-type that fits the product:
   a. COLLABORATIVE (highest k-factor): core value REQUIRES other people, so using it = inviting them. The product is pointless alone. Models: Figma (share link pulls in collaborators), Slack (team adoption inside out), Notion (shared workspaces). Build invite INTO the core workflow, not a settings page.
   b. EMBEDDED: every external touchpoint the product creates exposes it to a non-user. Models: Calendly (every scheduling link → a prospect; 20M users mostly from this), Typeform. Make the artifact the user sends carry the product.
   c. OUTPUT / WATERMARK: the product creates shareable output that carries the brand. Models: Loom (video links), Canva & "Made with Typeform" watermarks. Every share is a branded acquisition surface (allow removing it on paid).
   d. REFERRAL (two-sided): reward BOTH sides. Model: Dropbox free-space referral = 35% of daily signups early on. Use when the product isn't inherently multi-user.

2) CONTENT LOOP (compounds via SEO/social, scales without ad spend):
   USER creates content -> it gets indexed/shared -> new users discover it -> they sign up -> they create more content. Models: Pinterest (UGC indexed by Google), Notion (30k+ public templates driving SEO), TikTok (watermarked UGC). If users produce anything shareable (a funnel, a workout, a result, a template), make it public-by-default-friendly, SEO-indexable, and easy to share.

3) PAID LOOP (only if unit economics allow it):
   spend on ads -> acquire user -> RETAIN long enough to recover CAC + margin -> reinvest profit into more ads. Powered by RETENTION and LTV, not by budget. Weak retention = this loop leaks and dies.

## RULES FOR EVERY LOOP
- Bake the loop into the CORE product so using it well IS spreading it. Never a bolt-on "refer a friend" page nobody visits.
- Instrument it: track invites sent, invite->activation %, k-factor, and loop cycle time. Optimize the weakest stage and shorten the cycle.
- Loops depend on RETENTION: a leaky bucket can't compound. The habit/daily-return layer is a prerequisite, not optional.
- Reference open-source referral/waitlist mechanics to model on:
    Viral waitlist + referrals .. https://github.com/balazsotakomaiya/waitlist
    schemeBeam (referral tool) .. https://github.com/eemebarbe/schemeBeam
    viral-waitlist (fullstack) .. https://github.com/s-xync/viral-waitlist

## SELF-AUDIT
- Draw the loop. Does each user's action produce >=1 new user's action? If the circle doesn't close, it's still a funnel — redesign until it loops.
- Is the loop inside the core flow or bolted on the side? Move it into the core.
- What's the cycle time, and what's the single fastest way to halve it?
