# Perplexity Search Prompt: Weekly Tech Trend Reports

**Purpose:** Weekly search to discover new tech trend reports for the current year cycle.

**Schedule:** Run every Monday (or first working day of the week)

---

## The Search Prompt

```
Find technology trend predictions and reports published in the last 10 days from the following categories:

TECH VENDORS (examples):
- Google Cloud, Microsoft, AWS, IBM, Oracle, Salesforce, SAP, Adobe, ServiceNow
- But include ANY major tech vendor publishing trend reports

BIG CONSULTANCIES (examples):
- Deloitte, McKinsey, BCG, Accenture, Bain, KPMG, PwC, EY, Capgemini
- But include ANY major consultancy publishing trend reports

ANALYST FIRMS:
- Gartner, Forrester, IDC, CB Insights, 451 Research

VC FIRMS & INVESTORS:
- a16z (Andreessen Horowitz), Sequoia Capital, Bessemer Venture Partners, Greylock, Kleiner Perkins, First Round Capital, Insight Partners, General Catalyst

INDEPENDENT VOICES:
- Mary Meeker (Bond Capital)
- Scott Galloway (Prof G)
- Benedict Evans
- Ben Thompson (Stratechery)

ACADEMIC & INSTITUTIONS:
- MIT Technology Review
- Stanford HAI (Human-Centered AI)
- World Economic Forum

OTHER SOURCES:
- ARK Invest
- Visual Capitalist
- Harvard Business Review
- Any other major tech trend reports

Focus on:
- Annual "Tech Trends [YEAR]" reports
- "Top Technologies" or "Predictions for [YEAR]" reports
- Published in the LAST 10 DAYS
- Include exact publication dates and direct URLs
- Note if PDF is available or if content is web-only

Exclude:
- Product announcements (unless part of broader trends report)
- Individual blog posts (unless from known independent analysts)
- Conference presentations without published reports
```

---

## Usage Instructions

1. **Update the year:** Replace `[YEAR]` with current year (e.g., 2026) where it appears
2. **Run in Perplexity:** Paste the entire prompt into Perplexity search
3. **Review results:** Compare against existing collection in `tech-[year]/`
4. **Filter for new reports:** Check publication dates and sources
5. **Add to collection:** Follow [CLAUDE.md](CLAUDE.md) operations guide

**Note:** The prompt searches for reports from the last 10 days, making it ideal for weekly execution. The vendor/consultancy lists are examples—Perplexity will surface reports from any major source in those categories.

---

## What to Look For

**Must have:**
- Clear publication date
- Direct URL to report (not just landing page)
- PDF availability or web-accessible content
- Substantive content (not just a press release)

**Consider adding if:**
- Major publisher we haven't covered
- Unique perspective or framework
- Data-driven analysis (not just opinion)
- Covers blind spots in existing collection

**Skip if:**
- Paywalled with no preview (unless exceptionally important)
- Duplicate of existing coverage (same publisher, same year)
- Pure product announcement disguised as trends report
- No clear publication date

---

## Post-Search Actions

After discovering new reports:

1. **Triage:** Rank by priority (major publisher > niche player)
2. **Add:** Create folder, download PDF, write README
3. **Analyze:** Run interpretation using METHODOLOGY.md template
4. **Synthesize:** Update `tech-[year]/README.md` with new findings
5. **Commit:** Push to GitHub

---

## Search Variations

If the main prompt returns limited results, try these variations:

**Focus on specific sectors:**
```
Find AI/ML trend reports for [YEAR] from research firms, tech companies, and VCs
```

**Geographic variations:**
```
Find European technology trend reports for [YEAR] from Capgemini, SAP, or EU institutions
```

**Late cycle search:**
```
Find Q1 [YEAR] technology trend reports or predictions published after January [YEAR]
```

---

*Keep this prompt updated as we discover new relevant publishers.*
