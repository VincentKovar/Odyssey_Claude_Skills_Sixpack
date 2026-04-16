---
name: customer-review-analyzer
description: >
  Analyzes a CSV of customer reviews for any brand and produces a comprehensive
  research report covering benefits, pain points, personas, emotional drivers,
  trigger events, objections, testimonials, and ad-ready headlines. Use this
  skill whenever the user wants to: analyze customer reviews, run a review
  analysis, extract insights from reviews, build a customer research report, or
  understand what customers are saying about a brand. Trigger on phrases like
  "analyze these reviews", "run the customer review analyzer", "analyze reviews
  for [brand]", "what are customers saying about [brand]", "customer research
  for [brand]", or any time a CSV of reviews is provided and the user wants
  insights. Always use this skill when a CSV file of reviews is present in
  context and the user wants analysis â€” even if they don't use the exact phrase
  "customer review analyzer."
---

# Customer Review Analyzer Skill

## What This Skill Does

Takes a CSV of customer reviews and produces a structured research report with
13 sections of actionable insights for marketing, creative, and strategy work.
The output is designed to feed directly into ad concept creation, persona
development, and messaging strategy.

---

## How to Run This Skill

### Step 1 â€” Identify Inputs

You need two things:
1. **A CSV file** of customer reviews (uploaded by the user or referenced in context)
2. **The brand name** â€” ask if not obvious from context

If no CSV is present, ask: "Can you upload the reviews CSV so I can run the analysis?"

### Step 2 â€” Read the CSV

Use the `bash_tool` or `view` tool to read the uploaded CSV from `/mnt/user-data/uploads/`. Parse all available review content â€” look for columns named `body`, `content`, `review`, `text`, `title`, or similar. Combine title + body fields when both are present for richer signal.

**Important:** Process as many reviews as possible. The old project only sent 10 to the API â€” this skill reads all reviews and sends a representative sample of up to 50 (or the full set if under 50).

```bash
# Example: read the CSV to understand its structure
head -5 /mnt/user-data/uploads/reviews.csv
wc -l /mnt/user-data/uploads/reviews.csv
```

### Step 3 â€” Run the Analysis

Read the full analysis prompt from `references/analysis-prompt.md` and use it to analyze the reviews yourself directly â€” you ARE the AI doing the analysis. Do not call an external API. Simply read the reviews and produce the report following the exact output format specified in `references/output-format.md`.

Work through all 13 sections systematically. Be specific â€” pull actual phrases, themes, and patterns from the real review data. Do not use generic filler.

### Step 4 â€” Output the Report

Produce the full formatted report in the conversation. Then save it as a markdown file:

```
/mnt/user-data/outputs/[BrandName]_Customer_Analysis.md
```

Present the file using `present_files` so the user can download it.

---

## Output Structure (13 Sections)

See `references/output-format.md` for the exact format. At a high level:

1. âœ… **Benefits** â€” Most frequently mentioned benefits, ranked by frequency
2. âŒ **Prior Pain Points** â€” Problems customers had BEFORE using the product
3. â­ï¸ **Features** â€” Specific product features customers mention
4. ðŸ¤” **Prior Objections** â€” Hesitations customers had BEFORE buying
5. ðŸ™ **Failed Solutions** â€” Other products/approaches customers tried that didn't work
6. ðŸ’¬ **Other** â€” Customer service, shipping, packaging, misc feedback
7. ðŸ§  **Emotional Motivations** â€” Top 3 emotional drivers, ranked by power
8. ðŸ‘¥ **Customer Personas** â€” 5 detailed personas ranked by frequency
9. ðŸ“£ **Static Headlines** â€” First-person quotes pulled/adapted from real reviews
10. âš”ï¸ **Comparisons** â€” How customers contrast this brand vs failed solutions
11. âš¡ **Trigger Events** â€” Specific moments that pushed customers to search/buy
12. â“ **Common Objections** â€” Questions and concerns that came up pre-purchase
13. ðŸ’¬ **One-Liner Testimonials** â€” Punchy single-sentence testimonials for ads

---

## Reference Files

- `references/output-format.md` â€” Exact formatting template for each section
- `references/analysis-prompt.md` â€” Detailed instructions for what to extract and how to think about each section

---

## Quality Rules

1. **Every insight must be grounded in the actual review data.** No generic marketing speak.
2. **Personas must feel like real people**, not demographic buckets. Include a name, a frustration, a goal, and an awareness level.
3. **Headlines must sound like real humans wrote them** â€” use the voice from the reviews.
4. **Trigger events should be specific situations**, not vague states (e.g. "my doctor dismissed me again and I went home and started Googling", not "looking for solutions").
5. **One-liners should be punchy enough to drop directly into an ad.**
6. **If the reviews are thin**, call that out. Don't fabricate signal that isn't there.
