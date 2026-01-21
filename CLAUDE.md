# CLAUDE.md - Trends Radar Operations

Operational guide for adding and managing trend reports. For methodology (prompts, bias framework, interpretation template), see **[methodology.md](methodology.md)**.

---

## Quick Reference

### Adding a New Report

1. **Create folder:** `tech-[year]/[publisher-slug]/`
2. **Download PDF** (if available): `[year]-[publisher]-[short-name].pdf`
3. **Create README.md** with metadata (see template below)
4. **Create interpretation** using [methodology.md](methodology.md) template
5. **Add to Notion** (Trend Radar database)
6. **Update synthesis** (`tech-[year]/README.md`)
7. **Commit to GitHub**

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

## Folder Structure

```
tech-2026/
├── README.md                    # Synthesis (cross-report analysis)
├── google-cloud/
│   ├── README.md                # Report metadata
│   ├── 2026-google-cloud-5-ai-trends.pdf
│   └── 2026-google-cloud-5-ai-trends-interpretation.md
├── deloitte/
│   ├── README.md
│   ├── 2026-deloitte-tech-trends.pdf
│   └── 2026-deloitte-tech-trends-interpretation.md
└── ...
```

---

## README.md Template (Per Report)

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

- `README.md` — This file (metadata)
- `[year]-[publisher]-[short-name].pdf` — Original report
- `[year]-[publisher]-[short-name]-interpretation.md` — Our analysis

## Quick Summary

[2-3 bullet points]

**Bias Level:** [Low | Medium | Medium-High | High]
```

---

## Notion Integration

**Database:** Trend Radar
**ID:** `2ef643de-2988-44f1-a50e-7a9515185506`

### Required Fields

| Field | Format |
|-------|--------|
| **Name** | `[Publisher]: [Short Title]` |
| **Collection** | Tech Trends \| WEF Davos \| AI State of Play \| Other |
| **Year** | 2026 \| 2025 \| 2024 |
| **Publisher** | Select from list |
| **Type** | Report \| Article \| Video \| Podcast |
| **URL** | Link to original |
| **Summary** | 2-3 sentences |
| **Interpretation** | One-liner + bias rating |
| **NotebookLM** | Not Added \| Added \| Pending |

---

## Commands

| Command | Action |
|---------|--------|
| `Add [URL] to tech trends` | Create folder, README, interpretation, Notion entry |
| `Update synthesis` | Regenerate `tech-[year]/README.md` with all reports |
| `Search for [topic] reports` | Find additional sources via web search |
| `Show collection status` | List all reports with completion status |

---

## Quality Checklist

Before committing a new report:

- [ ] README.md has correct metadata and links
- [ ] PDF downloaded with correct filename (or noted as unavailable)
- [ ] Interpretation follows [methodology.md](methodology.md) template
- [ ] Interpretation starts with essence (fair summary first)
- [ ] Source URL and PDF link included in interpretation
- [ ] Cross-references to other reports included
- [ ] Notion entry created with all fields
- [ ] Synthesis README updated with new report
- [ ] Committed to GitHub

---

## Resources

- **Methodology:** [methodology.md](methodology.md) — Prompts, bias framework, interpretation template
- **Notion:** [Trend Radar Database](https://www.notion.so/2ef643de298844f1a50e7a9515185506)
- **NotebookLM:** [Tech Trends 2026](https://notebooklm.google.com/notebook/9b7b5a66-807e-4ba9-92e4-0e8536eddeb9) (not public)
