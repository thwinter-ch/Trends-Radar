# Methodology: Analyzing Trend Reports

## Core Premise

Every trend report serves an agenda. This isn't inherently bad — it's structural. Understanding the agenda helps extract signal from noise.

**Our job:** Read critically, document bias explicitly, extract genuine insights.

---

## The Prompts

### Interpretation Prompt (Single Report)

Use this when analyzing one report:

> "Summarize the essence of this report — what it actually says, fairly and accurately. Then assess: Who benefits if readers believe these predictions? What is the author selling (products, services, subscriptions, reputation)? Identify unique insights versus consensus views. Note cross-references to other reports in our collection."

### Synthesis Prompt (Cross-Report)

Use this when updating the collection README:

> "Compare all reports in this collection. Where do 3+ sources agree? Where do they disagree? What do independent voices (no product to sell) say that vendors won't? What's the meta-pattern — how should readers interpret vendor vs consultant vs independent reports differently?"

---

## The Analysis Framework

### Step 1: Identify the Publisher Type

| Publisher Type | Typical Agenda | Bias Pattern |
|----------------|----------------|--------------|
| **Tech Vendor** (Google, Microsoft, AWS, IBM) | Sell platform/products | Trends require their infrastructure |
| **Big Consultancy** (McKinsey, BCG, Deloitte, KPMG) | Sell transformation projects | Trends require consultants to implement |
| **Design Consultancy** (Accenture Song, Frog) | Sell design/innovation services | Trends require human-centered design |
| **Analyst Firm** (Gartner, Forrester, CB Insights) | Sell research subscriptions | Trends create FOMO requiring more research |
| **VC/Investor** (a16z, Sequoia) | Support portfolio positioning | Trends validate their investment thesis |
| **Institution** (WEF, MIT Tech Review) | Maintain relevance, editorial independence | Generally lower bias |
| **Independent Commentator** (Meeker, Galloway, Evans) | Audience growth, reputation, speaking fees | Different bias — see below |

### Independent Authors (Special Handling)

Authors like Mary Meeker, Scott Galloway, or Benedict Evans are NOT selling products. But they still have incentives:

| Incentive | How It Might Bias |
|-----------|-------------------|
| **Reputation** | Incentive to be right, but also to be quotable |
| **Media attention** | Provocative > accurate sometimes |
| **Speaking fees** | Bold predictions get invitations |
| **VC deal flow** | (For investors) Good analysis attracts founders |
| **Contrarian brand** | Some build identity on disagreeing with consensus |

**Key difference:** These biases are toward *attention* and *accuracy*, not toward *selling a specific product*. That makes them more trustworthy for "what might actually happen" vs vendors who are trustworthy for "what products are coming."

### Step 2: Ask "What Are They Selling?"

For every trend identified, ask:
- What product/service does this implicitly recommend?
- Who benefits if this trend is widely adopted?
- Does the publisher offer solutions for this trend?

**Example:** When Google Cloud says "grounded agents" are the future, they're selling their grounding APIs and Vertex AI. That's not dishonest — but it's not neutral either.

### Step 3: Evaluate on Four Dimensions

#### Commercial Bias
How much does the report serve the publisher's commercial interests?

| Level | Definition |
|-------|------------|
| **Low** | Trends don't clearly map to publisher's products/services |
| **Medium** | Some trends favor publisher's offerings, others don't |
| **High** | Most/all trends point toward publisher's solutions |

#### Technical Depth
How substantive is the technical content?

| Score | Definition |
|-------|------------|
| **1/5** | Buzzwords only, no technical detail |
| **2/5** | Surface-level, good for executives |
| **3/5** | Some technical detail, limited architecture |
| **4/5** | Solid technical content, implementable insights |
| **5/5** | Deep technical analysis with evidence |

#### Actionable Insights
Can you actually do something with this?

| Score | Definition |
|-------|------------|
| **1/5** | Pure vision, no practical guidance |
| **2/5** | General direction, no specifics |
| **3/5** | Some actionable recommendations |
| **4/5** | Clear action items with context |
| **5/5** | Detailed playbook with examples |

#### Novelty
Is this actually new, or repackaged consensus?

| Score | Definition |
|-------|------------|
| **1/5** | Entirely derivative, nothing new |
| **2/5** | Familiar themes with new framing |
| **3/5** | Mix of consensus and fresh perspectives |
| **4/5** | Several genuinely new insights |
| **5/5** | Paradigm-shifting original research |

### Step 4: Extract Genuine Value

Despite bias, most reports contain useful content:
- **Data:** Original research, survey results, case studies
- **Frameworks:** Taxonomies, models, decision frameworks
- **Signals:** What big players are betting on (revealed preferences)
- **Synthesis:** Connections between trends others miss

Document what's genuinely useful alongside the bias analysis.

---

## The Interpretation Template

Each source interpretation follows this structure:

```markdown
# [Publisher]: [Report Title] — Interpretation

> **Source:** [Full URL to original report]
> **PDF:** `[filename].pdf` or "N/A (web only)" or "[link] (gated)"
> **Published:** [Month Year or Full Date]
> **Prompt:** "Summarize the essence of this report — what it actually says, fairly and accurately. Then assess: Who benefits if readers believe these predictions?"

## Essence of the Report

[START HERE. Summarize what the report actually says — fairly, accurately, without snark.
This section should be useful even to someone who likes the report.
3-5 paragraphs covering core thesis and key findings.]

## Key Findings

### [Finding 1]
[Detail]

### [Finding 2]
[Detail]

## Who Benefits?

**Author type:** [Vendor | Consultancy | Analyst Firm | VC | Independent | Institution]

**What they're selling:** [Products, services, subscriptions, or "nothing directly"]

**How predictions align with interests:**
- [Specific example 1]
- [Specific example 2]

**For independent authors, note actual incentives:**
- [Reputation, media attention, speaking fees, etc.]

## Bias Scorecard

| Dimension | Rating | Notes |
|-----------|--------|-------|
| **Commercial Bias** | LOW / MEDIUM / HIGH | [Why] |
| **Technical Depth** | X/5 | [Why] |
| **Actionable Insights** | X/5 | [Why] |
| **Novel Ideas** | X/5 | [Why] |

## Cross-Reference

- **Aligns with:** [Other reports that agree]
- **Conflicts with:** [Other reports that disagree]
- **Unique angles:** [What this report covers that others don't]

## Bottom Line

[One paragraph: Read it for X, skip it for Y, filter for Z]
```

### Template Rules

1. **Essence comes first** — Be fair before being critical
2. **Source URL is required** — Reader should be able to verify
3. **PDF link if available** — Note if gated or web-only
4. **Publication date is required** — Context matters: early reports vs late reports
5. **Prompt is shown** — Transparency about how we analyzed
6. **Cross-references required** — Connect to other reports in collection

---

## Cross-Report Synthesis

The integrated synthesis (each collection's README.md) covers:

### Agreement Patterns
What do multiple publishers agree on? Strong signal if:
- Competitors agree (Google and Microsoft both say X)
- Different publisher types agree (consultancy + VC + analyst)

### Disagreement Patterns
Where do publishers diverge? Often reveals:
- Genuine uncertainty in the market
- Conflicting commercial interests
- Different time horizons

### The Hype Check
For each major trend:
- Is this actually new or recycled from last year?
- What's the timeline claim? (Usually too aggressive)
- What needs to be true for this trend to materialize?

---

## Our Own Biases

We have them too:

1. **Skepticism bias:** We may underweight genuinely useful content due to commercial framing
2. **Recency bias:** Current reports feel more relevant than they might be
3. **Selection bias:** We collect from known publishers, might miss important voices
4. **Snark bias:** Snarky analysis is fun to write but can obscure nuance

We try to be aware of these. Call us out if you see them affecting conclusions.

---

## How to Use This Collection

**If you're an executive:** Read the integrated synthesis for each collection. Dive into individual sources for detail.

**If you're a practitioner:** Check the "Actionable Insights" scores. Skip low-scoring reports unless you need the data.

**If you're a strategist:** Look for disagreement patterns. That's where the interesting questions are.

**If you're skeptical:** Good. Read the methodology, check our work, file issues when we get it wrong.

---

*This methodology evolves. Suggestions welcome.*
