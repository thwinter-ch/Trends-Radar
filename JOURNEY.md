# Journey: Building Trends Radar

*A development log of how this system came to be.*

---

## The Problem

Every January, the same dance:
- Deloitte publishes their Tech Trends
- Gartner drops their Top 10 Strategic Technologies
- McKinsey weighs in
- VCs like a16z publish "Big Ideas"
- Google, Microsoft, everyone has a take

These reports are useful. They're also product pitches. The challenge: collect them systematically, read them critically, and build a synthesized view that cuts through the noise.

## The Insight

**Treat bias detection as methodology, not opinion.**

Every consultancy report exists to serve the consultancy. That's not cynical — it's structural. The report is a lead generation tool. Understanding the commercial angle helps extract actual signal from noise.

So we built a framework:
- Rate commercial bias explicitly (Low/Medium/High)
- Ask "What are they selling?" for every trend
- Document what's genuinely useful alongside the critique
- Synthesize across reports to find real consensus

## Design Decisions

### Repository Structure

```
trends-radar/
├── README.md
├── JOURNEY.md
├── methodology.md
├── tech-2026/
│   ├── README.md           # Integrated synthesis
│   ├── google-cloud/       # Per-source analysis
│   │   ├── ai-agent-trends.md
│   │   └── ai-agent-trends.pdf
│   ├── deloitte/
│   └── ...
├── wef-2026/
└── ...
```

**Why this structure:**
- One repo for all trend collections (tech, WEF, etc.)
- Each collection/year combo gets a directory
- Per-source folders contain interpretation + original artifact
- Top-level README.md is the integrated synthesis

### The Interpretation Template

Every source gets the same treatment:
1. List the trends they claim
2. Map each trend to what they're selling
3. Analyze the commercial bias
4. Extract what's genuinely useful
5. Note what's missing
6. Rate on four dimensions

This makes analysis comparable across sources.

## The First Report

Google Cloud's "5 AI Trends for 2026: Agents take center stage" was the test case.

**What we found:**
- 5 trends, each mapping 1:1 to Google Cloud products
- "Grounded agents" is their technical differentiator push
- "Democratization" means "more customers on metered services"
- High commercial bias, but useful taxonomy of agent types

The framework worked. We could articulate both the bias and the value.

## Evolution of the Name

Started as "Tech Trends Collector" in the Second Brain project. But the scope expanded:
- Not just tech trends — WEF, industry reports, etc.
- Not just collecting — analyzing, synthesizing
- Not just a directory — a methodology

**Trends Radar** captures it better:
- Active scanning/monitoring
- Detection (signal vs. noise)
- Ongoing vigilance
- Multiple radar scans (tech, WEF, etc.)

## What's Next

### Immediate
- Complete the 2026 tech trends sweep
- Build out the WEF 2026 collection (Davos is Jan 20-24)
- Test the synthesis approach with multiple sources

### Future
- Year-over-year tracking (did predictions land?)
- Publisher credibility scoring over time
- Community contributions

---

## The Meta-Observation

Building this system was itself an exercise in the thing we're analyzing: synthesizing perspectives, detecting bias (our own included), and documenting decisions transparently.

The difference: we publish our methodology alongside our conclusions. When we say a report has "High commercial bias," you can see how we got there.

---

*Started: January 2026*
*Last updated: January 21, 2026*
