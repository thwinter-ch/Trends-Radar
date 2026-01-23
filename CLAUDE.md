# CLAUDE.md - Trends Radar Operations

Operational guide for adding and managing trend reports. For methodology (prompts, bias framework, interpretation template), see **[methodology.md](methodology.md)**.

---

## Quick Reference

### Adding a New Report

1. **Create folder:** `tech-[year]/[publisher-slug]/`
2. **Download PDF** (if available): `[year]-[publisher]-[short-name].pdf`
3. **Create README.md** with metadata (see template below)
4. **Create interpretation** using [methodology.md](methodology.md) template
5. **Update synthesis** (`tech-[year]/README.md`)
6. **Commit to GitHub**

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

## Commands

| Command | Action |
|---------|--------|
| `Add [URL] to tech trends` | Create folder, README, interpretation |
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
- [ ] Synthesis README updated with new report
- [ ] Committed to GitHub

---

## Resources

- **Methodology:** [methodology.md](methodology.md) — Prompts, bias framework, interpretation template
