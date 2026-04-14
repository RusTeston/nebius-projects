# Nebius — Partner Enablement Framework
## Design Spec & Project Documentation

**Portfolio Artifact #5 of 5**
**Created by:** Rus Teston
**Role target:** Senior Manager, Revenue Enablement / Head of Revenue Enablement
**Company:** Nebius (nebius.com)
**File:** `nebius-partner-framework.html`

---

## 1. Purpose & Strategic Intent

This artifact demonstrates the highest-order thinking in the portfolio — the ability to design a partner enablement *system*, not just partner training content. The distinction matters enormously in a hiring context. Anyone can build a training module. A strategic enablement leader builds a framework that defines how partners progress, what they're capable of at each stage, and how their development connects directly to GTM revenue outcomes.

**Job description requirements this directly addresses:**
- *"Build and scale technical enablement programs for partners to improve their competency and independence"*
- *"Align partner enablement with go-to-market priorities and partner lifecycle stages"*
- *"Develop role-based learning paths, certifications, and technical training programs across audiences"*
- *"Own the end-to-end execution of technical enablement programs, including planning, delivery, and iteration"*
- *"Define and track key metrics such as ramp time, program adoption, and technical competency improvements"*

---

## 2. The Three Strategic Signals This Artifact Must Send

These three things must be immediately visible to a hiring manager — not buried in text, but communicated through the visual structure itself:

### Signal 1: You Think in Tiers and Maturity Stages
The lifecycle bar is the dominant visual element of the page — it appears before anything else. It shows four named stages (Onboarded → Competent → GTM-Ready → Expert), each with three things a generic framework never includes:
- What a partner **can do** at that stage (capability, not knowledge)
- What **unlocks** them to move forward (observable criterion, not completion)
- What **GTM outcome** is attached to each stage (pipeline, deals, campaigns)

A hiring manager reading this immediately understands: this person knows that partner development is a progression, not a one-time event, and that every stage should produce a business result.

### Signal 2: You Design Differently for Each Partner Type
The partner type matrix is the most information-dense section of the framework. It shows three columns — VAR, ISV/MSP, Alliance — with meaningfully different content, formats, and certifications at each maturity stage. The differences are real:
- A VAR's Foundation enablement is about commercial positioning and the deal registration process
- An ISV's Foundation enablement is about the Token Factory API quickstart and Terraform-based deployment
- An Alliance partner's Foundation enablement is about the joint value narrative and integration quickstart

These are not the same program with different names on them. The matrix makes that unmistakably clear.

### Signal 3: You Align Enablement to GTM Outcomes
Every stage in the lifecycle has a "GTM Unlock" — the specific go-to-market action that a partner should be able to take as a direct result of completing that stage's enablement. The Four Pillars section makes this explicit: "GTM Alignment" is one of four pillars, and it's defined as "enablement always connected to a go-to-market outcome." The Independence Metrics section tracks pipeline-level outcomes, not just training completion rates.

---

## 3. Content Design Rationale

### Why the Lifecycle Bar Comes First
Most partner enablement frameworks start with content — here are the modules, here are the formats, here is the calendar. This framework starts with the lifecycle because the lifecycle is the architecture. Every content decision is downstream of it. Starting with lifecycle signals that the designer understands the *why* before the *what*.

### Why the Matrix Has Three Partner Types With Real Differences
The three Nebius partner types (VAR, ISV/MSP, Alliance) have fundamentally different revenue motions, skill gaps, and customer relationships. Treating them the same would produce a program that serves none of them well. The matrix forces every enablement decision to be made three times — once per partner type — which produces better content and demonstrates deeper program thinking.

### Why GTM Outcomes Are Attached to Every Stage
Enablement without a GTM outcome is training for its own sake. Each stage's GTM Unlock is written as a specific, observable action — "first deal registered," "joint demand generation campaign launched," "published joint case study." These are things a Partner Manager can verify. They connect the enablement program to the commercial engine.

### Why "Independence Building" Is One of the Four Pillars
The goal of partner enablement is not to create dependency — it's to eliminate it. A partner who needs a Nebius SA on every customer call is not a mature partner; they are an extension of Nebius's own field team. The independence pillar — and the metric that tracks decreasing SA escalation rate over time — signals that the program designer understands what partner scale actually looks like.

---

## 4. Design Decisions

### Visual Language
- **Theme:** Dark, technical, premium — consistent with Artifacts #1 and #2 for portfolio cohesion
- **Background:** `#060909` deepest black with 44px grid at 28% — slightly less intense than the cheat sheet, appropriate for a strategic document vs a quick reference
- **Gradient top bar:** The lifecycle section uses a four-color linear gradient (blue → green → orange → purple) across its top border — visually communicating progression and the four stages simultaneously
- **Ambient glow:** Low-opacity green radial gradient behind the header — brand consistency

### Color System
- **Nebius green `#00C853`:** Primary accent, lifecycle bar gradient element 2, GTM-related elements, core branding
- **VAR blue `#3B9EFF`:** Consistent with SA blue from Artifact #1 — signals structured/commercial
- **ISV orange `#FF9F3B`:** Consistent with AE orange from Artifact #1 — signals judgment/technical build
- **Alliance purple `#B47FFF`:** Consistent with partner purple from Artifact #1 — signals ecosystem/collaboration
- **Stage colors:** Stage 1 = blue (discovery/onboarding), Stage 2 = green (competency/growth), Stage 3 = orange (GTM/commercial), Stage 4 = purple (expert/ecosystem)

### Typography
- **Syne** (display): Framework title, stage names, stat values, pillar names — authority and technical precision
- **JetBrains Mono** (metadata): Section labels, partner type badges, certification badges, resource URLs, metrics — signals technical reference material
- **Epilogue** (body): A refined geometric humanist sans — slightly more open than DM Sans for longer descriptive text in the matrix cells and stage descriptions

### Layout Architecture
The page has a deliberate top-to-bottom information hierarchy:
1. **Brand + context** (top bar) — who made this, for whom, what the three partner types are
2. **Hero** — what this is and why it matters, with four headline stats
3. **Lifecycle bar** — the architectural foundation (dominant, full width)
4. **Partner type matrix** — the operational detail (full width, dense)
5. **Three-column bottom row** — pillars + metrics + resources (supporting detail)
6. **Footer** — attribution and references

This hierarchy mirrors how a strategic document should be read: strategy first, then execution, then evidence.

### The Lifecycle Bar
- Full-width, visually dominant, separated from the matrix by section label
- Four-color gradient top bar communicates progression visually without requiring a legend
- Each stage card has three layers: stage header (what stage, what they can do), stage body (enablement focus + unlock criteria), GTM box (the business outcome)
- Color coding in the stage body is subtle — gradient backgrounds, not solid fills — so the stage boxes feel like a system, not four separate components

### The Partner Type Matrix
- Grid layout with a fixed left column (row labels) and three content columns (one per partner type)
- Partner type column headers include: badge, full name, brief description of revenue motion, and primary skill gap — so readers understand WHY the content is different before they read what's different
- Cell content uses colored dots (matching partner type color) instead of generic bullet points — maintains visual system consistency
- Certification badges at the bottom of each cell make it clear that stage completion is verified, not assumed

---

## 5. Nebius-Specific Content References

| Content / Reference | Source |
|---|---|
| Three partner types: VAR, ISV/MSP, Alliance | nebius.com/nebius-partner-program |
| Token Factory API quickstart | docs.tokenfactory.nebius.com/quickstart |
| Nebius Solution Library (GitHub Terraform recipes) | github.com/nebius/nebius-solution-library |
| Trust Center (SOC 2, HIPAA, GDPR, ISO 27001) | nebius.com/trust-center |
| Partner Program portal and deal registration | nebius.com/nebius-partner-program |
| Nebius Academy | academy.nebius.com |
| AI Cloud documentation | docs.nebius.com |
| QLoRA / RAG / Agentic Search solutions | nebius.com/solutions/ |
| SemiAnalysis TCO framework (referenced in Commercial Fluency pillar) | nebius.com/calculating-the-total-cost-of-gpu-cluster |
| Nebius co-marketing program | nebius.com/nebius-partner-program |
| Partner types and revenue motions (Sales, Implementation, Development) | nebius.com/nebius-partner-program |

---

## 6. Technical Build Notes

### Stack
- Pure HTML and CSS — zero JavaScript, zero dependencies beyond Google Fonts CDN
- Google Fonts: Syne, JetBrains Mono, Epilogue
- All layout achieved with CSS Grid — no flexbox hacks, no JavaScript layout tricks
- Fully responsive: 4-column stages → 2-column → 1-column at 1100px and 780px breakpoints

### Deployment on AWS
```bash
# Upload to S3
aws s3 cp nebius-partner-framework.html s3://your-bucket/portfolio/nebius-partner-framework.html

# CloudFront invalidation
aws cloudfront create-invalidation --distribution-id YOUR_ID --paths "/portfolio/*"
```

**Suggested URL:** `yourdomain.com/portfolio/nebius/partner-framework`

### Print Optimization
Opens cleanly in Chrome for print on A3/Tabloid landscape with Background graphics enabled. The lifecycle bar and matrix print particularly well at full width.

---

## 7. How to Present This in an Interview

**Opening frame (25 seconds):**
> "Partner enablement is where most enablement programs fall flat — they build one curriculum, label it three times, and call it done. This framework is built differently. It starts with the lifecycle — what a partner can *do* at each stage, not just what they've consumed. And it designs completely different programs for the three Nebius partner types, because a VAR selling infrastructure has almost nothing in common with an ISV building on it."

**Key points to walk through:**
1. **Point to the lifecycle bar first.** Walk through one stage — show the "can do," "unlock criteria," and "GTM unlock" structure. Explain why GTM outcomes are attached to every stage rather than being separate from the learning program.
2. **Show the matrix and highlight the differences between partner types.** Pick one row — Foundation Enablement — and walk across the three columns to show concretely how the content differs. Emphasize: "these are not the same program with different names."
3. **Point to the Independence Building pillar.** Explain why it's a named pillar: "the goal of partner enablement is to reduce dependency on Nebius resources over time, not create it. That's a design principle, not just a metric."
4. **Show the Independence Metrics section.** Point to the "SA escalations per partner deal ↓ over time" metric — explain that a decreasing escalation rate is one of the best signals that a partner program is actually working.
5. **Name two or three Nebius-specific resources.** Mention the Solution Library on GitHub, the Token Factory quickstart, and the Trust Center — showing that the framework is grounded in real Nebius infrastructure.

**When asked "how would you prioritize this if you had limited capacity?":**
> "Build the Foundation enablement for all three partner types first — that's what gets partners into their first deal. The GTM-Ready and Expert stages can be developed while the first cohort is progressing through Foundation and Competent. Never make a partner wait at a stage because the next stage's content doesn't exist yet."

**When asked "how does this connect to revenue?":**
> "Every stage has a GTM unlock attached to it — an observable business action that the partner takes when they're ready. Stage 1 = first deal registered. Stage 2 = first active pipeline deal with a close date. Stage 3 = first customer win presented. These aren't learning milestones — they're revenue milestones. Enablement that can't point to those is just training."

---

## 8. Future Iterations

- **Partner scorecard:** A per-partner dashboard showing current maturity stage, time-in-stage, GTM outcomes achieved, and next unlock criteria
- **Vertical-specific tracks:** Life Sciences partner track (HIPAA-first, drug discovery use cases), Media & Entertainment track (GenAI content, Wubble-style proof points)
- **Sub-partner enablement module:** Expert-stage partners who are building their own partner networks need a train-the-trainer track
- **Localization:** Finnish, French, and German versions for Nebius's EU data center regions where the partner ecosystem is growing
- **LMS integration:** Each stage maps to a learning path in Docebo or Cornerstone; certification gates are assignment submissions with assessor rubrics

---

*Document version: 1.0 | Artifact: nebius-partner-framework.html | Portfolio: Rus Teston*
