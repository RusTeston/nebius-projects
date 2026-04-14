# Nebius — Enablement Metrics Dashboard
## Design Spec & Project Documentation

**Portfolio Artifact #4 of 5**
**Created by:** Rus Teston
**Role target:** Senior Manager, Revenue Enablement / Head of Revenue Enablement
**Company:** Nebius (nebius.com)
**File:** `nebius-metrics-dashboard.html`

---

## 1. Purpose & Strategic Intent

This artifact makes the single most important argument in the entire portfolio: that enablement is measurable, and that its measurements connect to revenue. Most enablement leaders can describe what they built. Far fewer can show how it performed — and fewer still can connect program completion to business outcomes like win rate, deal velocity, and partner pipeline. This dashboard does all three.

**Job description requirements this directly addresses:**
- *"Define and track key metrics such as ramp time, program adoption, and technical competency improvements"*
- *"Gather feedback from the field and use data to continuously improve enablement programs"*
- *"Report on enablement effectiveness and business impact"*
- *"Drive adoption and engagement across global teams"*

---

## 2. Measurement Philosophy

The dashboard is built around two distinct time horizons — a deliberate design choice that most enablement reporting collapses into one:

### Leading Indicators (In-Program)
These are signals visible *during* the enablement program that predict whether it's working before the business results arrive:
- **Ramp time trend** — are learners moving through phases faster quarter over quarter?
- **Competency scores** — are assessment scores meeting or exceeding the threshold at each gate?
- **Adoption funnel** — where are learners dropping off, and why?
- **Module NPS** — which content is landing and which needs to be rebuilt?

### Lagging Indicators (60–90 Days Post-Ramp)
These are business results that arrive after the program is complete — the proof that enablement changed behavior and drove revenue:
- **Technical win rate** — do SA-involved deals win more often when the SA completed the program?
- **Discovery-to-validation speed** — do enablement-complete AEs move to technical validation faster?
- **Partner deal velocity** — do certified partners close their first deal faster?
- **Cohort comparison** — head-to-head table of complete vs incomplete cohort performance across six metrics

The discipline of separating these two categories — and being explicit about which is which — is one of the clearest signals of measurement maturity.

---

## 3. Dashboard Section Rationale

### KPI Cards (Top Row)
Four headline numbers chosen because they answer the four questions a VP of Sales or CRO asks first:
1. "How fast are people ramping?" → Avg Ramp Time (7.4 weeks, down 2.1 from Q4)
2. "Are people finishing the program?" → Completion Rate (88%)
3. "Are people actually passing the assessments?" → Cert Gate Pass Rate (83%)
4. "Is this producing revenue?" → Partner-Sourced Pipeline ($2.4M, +38%)

Each card shows the metric, the delta vs prior quarter, and a one-line context note explaining what the number means and what the target is.

### Ramp Time Trend (Bar Chart)
Four quarters of data for each of the three tracks — showing consistent improvement. This is intentionally not a single number: the trend line is what matters, not the snapshot. An enablement leader who only reports "current ramp time" doesn't understand why it is what it is. Showing the trend demonstrates that the program is being actively managed and improved.

### Competency Scores (Phase-Level)
Three tracks × three phases = nine data points, showing that competency scores decrease slightly at each phase (Foundation → Practitioner → Expert). This is *expected and correct* — Expert gates should be harder than Foundation gates. A dashboard that shows flat scores across all phases would suggest the assessments aren't calibrated correctly.

### Adoption Funnel
The most actionable section for a program manager. It shows exactly where learners drop off, includes a "watch item" callout for the Phase 2 drop-off with a root cause hypothesis and the intervention already underway. This demonstrates that the dashboard is actively used to manage the program, not just to report on it.

### Module NPS (Field Feedback)
Twelve module scores across all three tracks. Two are flagged below 7.0 with a content review notice. The callout box includes the common feedback theme ("too theoretical, needs more real deal examples") and the specific revision plan. This is the most important thing a hiring manager can see in this section: not that all scores are high, but that low scores have been identified, diagnosed, and have a fix in motion.

### Revenue Correlation Panel
The executive money slide. Three metrics showing the business impact of enablement completion vs non-completion, followed by a six-row cohort comparison table. Every number in this section is framed as a comparison — complete vs incomplete — because absolute numbers don't tell a story. The gap tells the story.

### Content Iteration Log
Eight entries showing what changed, why, and what triggered the change. Five different trigger types are represented: NPS below threshold, product launch, funnel data, support ticket volume, win/loss analysis, and QA review. This demonstrates that the content is managed like a living program, not published once and forgotten.

---

## 4. Design Decisions

### Visual Language
- **Theme:** Dark operational dashboard — same base palette as the rest of the portfolio, but tighter information density and more data-forward visual elements
- **"Live Dashboard" pill** with a pulsing green dot — creates the sense of a real-time operations tool rather than a static document
- **Q1 2025 cohort label** — grounds the data in a specific reporting period, making it feel like an actual business report

### Color Usage
- **Green** for positive metrics, above-target numbers, complete cohort values — Nebius brand color doubles as the success indicator
- **Blue/Orange/Purple** for track-specific data visualization (SA/AE/Partner) — consistent with the full portfolio color system
- **Orange** for warning states (⚠ watch items, content review flags) — signals attention needed without alarm
- **Red** for below-threshold indicators (NPS scores below 7.0, drop-off badges) — used sparingly so it carries weight

### Sparklines
Three small bar sparklines in the revenue correlation cards show trend direction (decreasing for time metrics, increasing for performance metrics) without requiring a full chart. They add visual rhythm to the data cards and communicate "this is tracked over time" without taking up space.

### Watch Items and Callout Boxes
Two orange callout boxes (Phase 2 drop-off, two modules below NPS threshold) and one iteration log are the most important elements for a hiring manager reading this. They prove that the dashboard owner is actively using the data to manage the program — not just collecting it.

### Cohort Comparison Table
Deliberately simple — six rows, two value columns (Complete vs Incomplete), clean borders. No charts, no gradients. The contrast between the numbers is the story: 68% vs 49% win rate, $148K vs $102K deal size, 24 days vs 42 days to first deal. Simplicity makes those gaps land harder.

---

## 5. Technical Build Notes

### Stack
- Pure HTML and CSS — single file, zero JavaScript (except the pulsing dot animation via CSS `@keyframes`)
- Google Fonts: Syne, JetBrains Mono, DM Sans
- All charts are CSS-only: bar widths set as inline `width` percentages on colored `div` elements
- Sparklines are CSS flexbox with `align-items: flex-end` and varying `height` percentages
- Fully responsive: 4-column KPI row collapses to 2×2; panels stack vertically at 720px

### Data Note
All data is illustrative — representative of what a real Q1 2025 cohort report would look like for a program of this scale. Cohort sizes (SA n=48, AE n=56, Partner n=38) and all metric values are designed to be realistic and internally consistent.

### Deployment on AWS
```bash
aws s3 cp nebius-metrics-dashboard.html s3://your-bucket/portfolio/nebius-metrics-dashboard.html
aws cloudfront create-invalidation --distribution-id YOUR_ID --paths "/portfolio/*"
```
**Suggested URL:** `yourdomain.com/portfolio/nebius/metrics-dashboard`

---

## 6. How to Present This in an Interview

**Opening frame (25 seconds):**
> "Every enablement leader can tell you what they built. The ones who last in the role can tell you how it performed — and connect it to revenue. This dashboard is how I'd report on the Nebius enablement program to a VP of Sales or a CRO. Leading indicators during the program, lagging indicators 60 to 90 days post-ramp, and a head-to-head cohort comparison that shows exactly what happens when people complete the program versus when they don't."

**Key points to walk through:**
1. Show the four KPI cards — explain why these four numbers are what a business leader asks first
2. Point to the adoption funnel's Phase 2 drop-off watch item — explain that the most important thing in this section isn't the completion rate, it's the intervention already underway
3. Show the two flagged module NPS scores — point out that the callout includes the feedback theme and the specific revision plan, not just the score
4. Open the revenue correlation section — walk through the cohort comparison table and let the numbers speak: 68% vs 49% win rate, $148K vs $102K deal size
5. Show the iteration log — point out the five different trigger types and explain that each one represents a different feedback loop connected to the program

**When asked "how do you actually get this data?":**
> "Three sources: LMS completion and assessment data (Docebo, Cornerstone, or a Notion tracker pre-LMS), post-module survey data collected via a simple Typeform or Google Form, and CRM data pulled from Salesforce — specifically pipeline created, close rates, and deal size segmented by whether the rep completed the enablement program. The cohort comparison is the hardest to get right because you need a clean way to tag enablement-complete reps in the CRM. That's a RevOps conversation, and it's worth having early."

**When asked "what would you do with the Phase 2 drop-off data?":**
> "Root cause first. The funnel shows it happens after Cert Gate 1 — so people are passing the assessment and then disengaging before Phase 2 starts. That pattern almost always means a manager release problem, not a content problem. The intervention is a manager briefing module at program kickoff — which is already logged in the iteration log. If that doesn't move the number within one cohort, the next step is a manager commitment form signed before their report enrolls."

---

## 7. Future Iterations

- **Real-time LMS connection** — if Nebius uses Docebo or Seismic Learning, this dashboard can be replaced with a live API-connected version
- **Individual learner drilldown** — clicking a track in the funnel expands to show individual completion status by module (for manager use, not reporting)
- **Regional segmentation** — separate views for North America vs Europe given Nebius's multi-region footprint
- **Quarterly executive summary export** — a one-page PDF auto-generated from this dashboard for CRO/VP reporting

---

*Document version: 1.0 | Artifact: nebius-metrics-dashboard.html | Portfolio: Rus Teston*
