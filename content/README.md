# Content Strategy

Content pieces built from the analysis. Each folder contains the post, the prompt used to generate it, and any supporting assets.

This directory is intentionally not linked from the root README—it's here for transparency, not promotion.

---

## Content Calendar

| # | Title | Status | Target Date | Dependencies |
|---|-------|--------|-------------|--------------|
| 1 | [Tech Trends Launch](01-tech-trends-launch/) | Ready | Jan 25 | None |
| 2 | [WEF Synthesis](02-wef-synthesis/) | Ready | Jan 24 | WEF data collection ✓ |
| 3 | [Methodology & Journey](03-methodology-journey/) | Ready | Jan 26 | Post #1 published |
| 4 | [Integrated Gamma Deck](04-gamma-deck/) | Ready | Jan 27+ | Posts #1-3 |
| 5 | TBD | - | - | - |
| 6 | TBD | - | - | - |

---

## Action Plan (What To Do)

### Jan 24 — Post #2: WEF Synthesis
1. Open `02-wef-synthesis/post.md`
2. Copy text between the triple backticks under "## Post"
3. Paste into LinkedIn
4. Immediately post first comment (copy from "## First Comment")
5. Optional: attach screenshot of GitHub README

### Jan 25 — Post #1: Tech Trends Launch
1. Open `01-tech-trends-launch/post.md`
2. Copy text between the triple backticks under "## Post"
3. Paste into LinkedIn
4. Immediately post first comment with repo link

### Jan 26 — Post #3: Methodology & Journey
1. Open `03-methodology-journey/post.md`
2. Copy text between the triple backticks under "## Post"
3. Paste into LinkedIn
4. Post first comment with three links (repo, methodology, journey)

### Jan 27+ — Post #4: Gamma Carousel
1. Open `04-gamma-deck/prompt.md`
2. Copy the Gamma prompt (everything in the code block)
3. Go to [gamma.app](https://gamma.app) → Create → Paste prompt
4. Generate deck, review, tweak slides as needed
5. Export as PDF
6. On LinkedIn: Create post → Add document → Upload PDF
7. Copy post text from `04-gamma-deck/post.md` into the post body
8. Publish, then add first comment with repo link

---

## Folder Structure

Each content piece follows this pattern:

```
[number]-[slug]/
├── post.md          # Final LinkedIn post
├── prompt.md        # Prompt used to generate the post
└── assets/          # Images, exports, supporting files
```

---

## Principles

- **Show the work:** Prompts are transparent
- **Version-controlled:** Content strategy evolves like code
- **Not the headline:** This directory exists but isn't promoted
- **Forkable:** Anyone can clone the approach

---

*Content created using Claude Code + Perplexity*
