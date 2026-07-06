## Changes to `src/routes/index.tsx` and `src/styles.css`

### 1. New color palette (classic editorial)
Update theme tokens in `src/styles.css`:
- Background: soft ivory `#F7F3EC`
- Surface / card: warm off-white `#FBF8F2`
- Primary text / headings: deep forest green `#1F3A2E`
- Body text: warm charcoal `#2B2A26`
- Muted / rule lines: warm gray `#B8B0A2`
- Accent (CTAs, links, pull-quote bar): terracotta `#B5533C` with hover `#9A4330`

Applied to masthead, category tag, byline, section headings, pull-quote, links, and both CTAs. Keeps existing layout, typography sizes, and structure untouched.

### 2. Third-grade reading level rewrite
Rewrite every body section so a third grader can read it:
- Short sentences (mostly under 15 words).
- Everyday words (swap "capitulated", "instinct", "abrasive", "desensitization", "cortisol", etc. for plain equivalents).
- Break long paragraphs into 2–3 sentence chunks.
- Keep all 8 section headings, the italic pull-quote, Cody/Daniel W testimonial, and the FAQ block intact (FAQ answers also simplified).
- Keep headline, subheadline, byline, "Partner Content" label, category tag, and image positions exactly as-is.

### 3. Add a third, extra-clear CTA after the hook (~200 words in)
Insert a new CTA block right after the opening "Hook" section, before "The Ancient Secret" section. It will contain:
- One line of plain text: "This is the board that fixed it for us."
- A large button labeled **"See The Nail Board On Amazon →"** (styled same as the final CTA, linking to the product URL).

### 4. Make all CTA buttons bigger and clearer
- Increase padding (`py-5 px-10`), font-size (`text-xl`), font-weight (`font-bold`), full-width on mobile, auto width on desktop.
- Use terracotta accent background, ivory text, subtle shadow, clear hover state.
- Rename button labels for clarity:
  - Mid-hook CTA: **"See The Nail Board →"**
  - Existing soft link near end stays as text link: **"See the board we found →"**
  - Final CTA button: **"Check Price & Availability →"**
- All three CTAs point to:
  `https://thedogparlor.store/products/dog-nail-file-board-adjustable-wooden-scratching-board-for-nail-trimming-self-scratcher-toy-safe-pet-grooming-accessories`
  (already stored in the `OUTBOUND` constant — reused, `target="_blank"` + `rel="noopener noreferrer"`.)

### Out of scope
No changes to masthead text, image assets, route structure, or backend. Pure content + styling swap.
