# CLAUDE.md - Trends Radar Cookbook

This document defines the methodology for collecting, analyzing, and synthesizing technology trend reports.

## Purpose

Cut through vendor marketing disguised as thought leadership. Extract signal from noise. Call out bias while acknowledging valuable insights.

## Report Collection Process

### Step 1: Add New Report

1. **Create folder:** `tech-[year]/[publisher-slug]/`
2. **Create README.md** with metadata:
   ```markdown
   # [Publisher]: [Report Title]

   ## Original Report

   | Field | Value |
   |-------|-------|
   | **Title** | [Full original title] |
   | **Publisher** | [Organization] |
   | **URL** | [Link to report] |
   | **PDF** | `[filename].pdf` or N/A |
   | **Date Published** | [Date] |

   ## Files
   - `README.md` — This file
   - `[year]-[publisher]-[short-name].pdf` — Original report
   - `[year]-[publisher]-[short-name]-interpretation.md` — Our analysis

   ## Quick Summary
   [2-3 bullet points]

   **Bias Level:** [Low | Medium | Medium-High | High]
   ```

3. **Download PDF** (if available) with naming: `[year]-[publisher]-[short-name].pdf`

4. **Write interpretation** following the template below

5. **Add to Notion** (Trend Radar database)

6. **Commit to GitHub**

---

## Interpretation Template

Every interpretation file MUST follow this structure:

```markdown
# [Publisher]: [Report Title] — Interpretation

> **Source:** [Full URL to original report]
> **PDF:** [Link or "N/A (web only)"]
> **Interpretation Prompt:** "Extract key predictions, assess commercial bias, identify unique insights vs. consensus views, and note what benefits the author gains from these specific predictions."

## Essence of the Report

[Start with WHAT the report actually says. No snark yet. Summarize the core thesis and key predictions/findings in 3-5 paragraphs. Be fair and accurate.]

## Key Findings

### [Finding 1]
...

### [Finding 2]
...

## Who Benefits?

[NOW assess bias. Ask: "Who benefits if readers believe this?"]

**Author type:** [Vendor | Consulting Firm | VC | Research Firm | Independent Commentator | Academic]

**What they're selling:**
- [Product/service/narrative that benefits from these predictions]

**Bias assessment:**
- [Specific examples of how predictions align with author's interests]

**IMPORTANT:** For independent voices (Mary Meeker, Scott Galloway, Benedict Evans, academics), note that they are NOT selling products. Their incentives are:
- Media attention / audience growth
- Reputation as accurate forecaster
- Speaking fees / book sales
- VC deal flow (for investors)

These are different from vendor bias but still worth noting.

## Bias Scorecard

| Dimension | Rating | Notes |
|-----------|--------|-------|
| **Commercial Bias** | LOW / MEDIUM / HIGH | [Why] |
| **Technical Depth** | 1-5 | [Why] |
| **Actionable Insights** | 1-5 | [Why] |
| **Novel Ideas** | 1-5 | [Why] |

## Cross-Reference

- **Aligns with:** [Other reports that agree]
- **Conflicts with:** [Other reports that disagree]
- **Unique angles:** [What this report covers that others don't]
```

---

## Synthesis Document

Maintain `tech-[year]/README.md` as the master synthesis:

1. **Collection status table** — All reports, bias levels, status
2. **Consensus themes** — Where 3+ reports agree (with sources)
3. **Disagreement watch** — Where reports conflict (with sources)
4. **Unique insights by source** — What each adds that others miss
5. **Bias summary** — Reports grouped by bias level

Update this after adding each new report.

---

## Bias Assessment Framework

### Commercial Bias Levels

| Level | Definition | Examples |
|-------|------------|----------|
| **LOW** | No product to sell, editorial independence | MIT Tech Review, academics |
| **LOW-MEDIUM** | Independent but has audience/reputation incentives | Galloway, Meeker, Evans |
| **MEDIUM** | Research firm with subscription model | Gartner, Forrester, CB Insights |
| **MEDIUM-HIGH** | Consulting firm positioning for engagements | Deloitte, KPMG, Capgemini |
| **HIGH** | Vendor with products matching predictions | Google Cloud, Microsoft, IBM |

### Red Flags

- Every trend maps to author's product
- "Unprecedented" used excessively
- No acknowledgment of risks/limitations
- Predictions conveniently match existing investments
- Aggressive timelines for author's specialty

### Green Flags

- Acknowledges uncertainty
- Includes contrarian data
- Cites independent sources
- Discusses failures/limitations
- Predictions sometimes against author's interest

---

## File Naming Convention

```
[year]-[publisher]-[short-name].pdf
[year]-[publisher]-[short-name]-interpretation.md
```

Examples:
- `2026-deloitte-tech-trends.pdf`
- `2026-deloitte-tech-trends-interpretation.md`
- `2026-gartner-top-10-tech-trends-interpretation.md`
- `2025-mary-meeker-ai-trends.pdf`

---

## Notion Integration

Database: `Trend Radar` (ID: `2ef643de-2988-44f1-a50e-7a9515185506`)

Required fields:
- **Name:** `[Publisher]: [Short Title]`
- **Collection:** Tech Trends | WEF Davos | AI State of Play | Other
- **Year:** 2026 | 2025 | 2024
- **Publisher:** Select from list
- **Type:** Report | Article | Video | Podcast | Presentation
- **URL:** Link to original
- **Summary:** 2-3 sentences
- **Interpretation:** Snarky one-liner + bias rating
- **NotebookLM:** Not Added | Added | Pending

---

## Commands

| Command | Action |
|---------|--------|
| "Add [URL] to tech trends" | Create folder, README, interpretation, Notion entry |
| "Update synthesis" | Regenerate tech-[year]/README.md with all reports |
| "Search for [topic] reports" | Find additional sources via web search |
| "Show collection status" | List all reports with completion status |

---

## Quality Checklist

Before committing a new report:

- [ ] README.md has correct metadata and links
- [ ] Interpretation starts with essence (fair summary)
- [ ] Interpretation includes source URL and PDF link
- [ ] Interpretation includes the prompt used
- [ ] "Who Benefits?" section is accurate to author type
- [ ] Cross-references to other reports included
- [ ] Notion entry created with all fields
- [ ] Synthesis README updated
