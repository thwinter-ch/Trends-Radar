# Trends Radar

Tech trend reports decoded. Every January, everyone publishes predictions. Most are product pitches. We collect them, detect the bias, extract the signal, and synthesize what actually matters.

## Built By

- **Research:** [Perplexity](https://perplexity.ai) for discovery and fact-finding
- **Analysis:** [Claude](https://claude.ai) for interpretation and synthesis
- **Curation:** A human who's tired of reading vendor pitches disguised as thought leadership

## Current Scans

| Collection | Status | Synthesis |
|------------|--------|-----------|
| [Tech Trends 2026](tech-2026/) | 9 reports | [Integrated view](tech-2026/README.md) |
| [WEF Davos 2026](wef-2026/) | Day 1 | [Daily summaries](wef-2026/README.md) |

## How We Work

1. **Collect** — Sweep known publishers, use Perplexity to find what we missed
2. **Download** — Get the original PDFs/reports
3. **Analyze** — Read each report with explicit bias detection
4. **Interpret** — Per-source analysis with commercial angle
5. **Synthesize** — Cross-report integration, find consensus and disagreement

### File Structure

Each source folder contains:
```
[source]/
├── README.md           # Original report title, official URL, metadata
├── [original-name].pdf # The actual report (when available)
└── interpretation.md   # Our analysis with bias detection
```

## Documentation

- [JOURNEY.md](JOURNEY.md) — How we built this system
- [methodology.md](methodology.md) — Our analysis framework

## Notion Database

Browsable index of all collected reports:
**[Research Reports](https://www.notion.so/2ef643de298844f1a50e7a9515185506)**

## Philosophy

> "When a consultancy tells you what the future looks like, ask who's paying for the vision."

Most trend reports exist to position products, create consulting urgency, or establish thought leadership. That doesn't make them useless — the underlying research is often solid. But the framing serves commercial interests. We read them critically and note the bias explicitly.

---

*Built with [Claude Code](https://claude.ai/code)*
