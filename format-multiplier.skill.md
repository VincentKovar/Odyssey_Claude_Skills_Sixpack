---
name: format-multiplier
description: >
  Multiplies a winning ad concept brief into new variants by pivoting the
  format â€” the visual execution, content structure, and hook style â€” while
  holding the strategic core (motivator, benefit, angle) fixed. Use this skill
  whenever the user wants to: run a format multiplier, change the format of an
  existing concept, execute the same angle in a different content structure,
  expand reach by adapting a validated strategy to new formats, or see what a
  brief looks like as a different ad type. Trigger on phrases like "run a
  format multiplier", "what would this look like as a [format]", "same angle
  different format", "turn this into a podcast ad", "turn this into a UGC",
  "adapt this to a different format", "what formats would work for this angle",
  or any request to vary the format of an existing brief while keeping the
  strategy intact. Always use this skill when a concept brief is in context
  and the user wants to reformat it without changing the strategic DNA.
---

# Format Multiplier Skill

## What This Skill Does

Takes an existing 8-field concept brief and multiplies it into new variants by
swapping the format â€” the visual execution, hook style, and content structure â€”
while keeping the strategic core locked. The core belief: a validated angle can
travel across formats. Format variations can reuse nearly all strategic DNA.

**The formula:**
`1 angle Ã— N formats = expanded reach without strategic drift`

---

## What Gets Locked vs. Swapped

**LOCKED (do not change):**
- Motivator
- Benefit
- Angle

**SWAPPED (must change):**
- Concept Name
- Concept Summary
- Format
- Why It Will Work
- Rationale

---

## How to Run a Format Multiplier

### Step 1 â€” Read the source brief
Identify the Motivator, Benefit, and Angle. These do not change.

### Step 2 â€” Suggest new formats (then let the user confirm)
Pull from the Odyssey Approved Format Library below. Suggest 3â€“5 formats that
would work well for the strategic angle, ranked by likely performance. Use this
format:

> Here are the formats I'd recommend multiplying this concept into, ranked by
> fit:
> 1. [Format name] â€” [One sentence on why this format suits this angle]
> 2. [Format name] â€” [One sentence]
> 3. [Format name] â€” [One sentence]

Wait for confirmation before writing any briefs.

### Step 3 â€” Write the multiplied brief
Output a complete 8-field brief. The Rationale must explicitly name:
- What strategic DNA was preserved (Motivator, Benefit, Angle)
- What changed (Format, hook style, visual execution)
- Why this specific format expresses the angle effectively

---

## The 8-Field Brief Format

Every output must use this exact structure:

```
Concept Name: [2-5 words, punchy]
Concept Summary: [One sentence â€” who speaks, what they say, setting, CTA]
Format: [Visual format label from approved list below]
Motivator: [One sentence, first-person â€” unchanged from source brief]
Benefit: [One sentence, concrete â€” unchanged from source brief]
Angle: [2-4 words â€” unchanged from source brief]
Why It Will Work: [One sentence â€” specific to this format, not generic]
Rationale:
- [What strategic DNA was locked and why it travels across formats]
- [What changed in the format and why]
- [Why this specific format works for this angle and client]
```

---

## Odyssey Approved Format Library

Use these exact labels. Do not invent new formats without flagging.

**Native**
- Trend Hook + Explainer
- Undeniable Proof Product Demo
- Founder Sale Announcement
- POV Comedic
- Trendy Edit Background VO
- Credible Figure Overlay
- Trending Music Text Explainer
- In-Store Explainer
- Native Comedy

**Scripted / Structured**
- Talking Head UGC
- Staged Organic Moment
- Staged Organic Moment / Street Interview Hybrid
- Street Interview
- Podcast Ad
- Listicle
- Word Wall Overlay
- Before/After
- Faceless UGC
- Green Screen

**Elevated / Static**
- Cinematic Brand Spot
- Slideshow
- Static Ad
- News Format
- Testimonial Card

---

## Format Guidance for Suggestions

Use this when recommending which formats to multiply into:

- **Staged Organic Moment**: Two people in a real-world setting. One discovers
  the product through the other. Feels TikTok-native. Perfect for
  problem-solution narratives.
- **Street Interview**: Interviewer asks strangers about a pain point. Organic
  social proof. Multiplies well by length â€” longer for TOF, shorter and direct
  for BOF.
- **Podcast Ad**: 9-step structure: Hook â†’ problem â†’ failed solutions â†’
  introduce solution â†’ re-introduce product â†’ reasons to believe â†’ desired
  outcome â†’ CTA. Multiplies across the 5 angles.
- **Word Wall Overlay**: Existing footage + long copy overlaid as text. Easiest
  to multiply â€” change one sentence, new ad. Great for complex messaging and
  educational content.
- **Faceless UGC**: Product demo without showing face. Authentic,
  product-forward. Can be created by anyone regardless of location or identity.
- **Listicle**: "N reasons why..." structure. Skimmable. Good for MOF feature
  education. Easy to produce with existing assets.
- **Trending Sound**: No VO. Visual storytelling + summary captions + trending
  audio. 88% of TikTok users say sound is essential. Multiplies with angles and
  funnel stages.
- **News Format**: Dark background. Subject photo. Red "NEWS" banner. All-caps
  bold headline. Yellow highlight on key word. High scroll-stop for cold
  traffic. Best for awareness stage.
- **Testimonial Card**: User quote dominates frame. Premium editorial feel. Best
  for warm audiences and retargeting.

---

## The Andromeda Rule

Before outputting any multiplied brief, check: does this new variant have the
same Format + Angle + Funnel Stage as any other brief already in context?

If yes: "This combination already exists as [Concept Name]. To avoid creative
decay, I'd suggest varying [dimension] instead. Here are alternatives: ..."

Never output two briefs that would look like the same ad in different clothes.

---

## Quality Rules

1. **Never output a variant where only the Concept Name changed.** The format
   shift must produce genuinely different creative execution.
2. **Rationale bullets must be specific.** "This works because it's engaging"
   is not acceptable. Name the mechanism â€” the format behavior, the proven
   TikTok structure, the platform-specific pattern.
3. **Why It Will Work must be specific to the format**, not a generic statement
   about the angle. Explain why this particular format unlocks this angle.
4. **The Motivator and Benefit fields must be copied verbatim from the source
   brief.** Do not rephrase, soften, or reframe them.
5. **The Andromeda Rule applies always.** Diversity across formats is
   non-negotiable â€” never output two formats that produce the same viewing
   experience.
