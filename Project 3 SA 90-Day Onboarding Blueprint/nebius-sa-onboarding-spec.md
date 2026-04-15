# Nebius — SA 90-Day Onboarding Blueprint
## Design Spec & Project Documentation

**Portfolio Artifact #3 of 5**
**Created by:** Rus Teston
**Role target:** Senior Manager, Revenue Enablement / Head of Revenue Enablement
**Company:** Nebius (nebius.com)
**File:** `nebius-sa-onboarding.html`

---

## 1. Purpose & Strategic Intent

This artifact is the most operationally complete piece in the portfolio. It answers the question that every VP of Sales eventually asks an enablement leader: *"How do we get new SAs to their first customer-ready demo as fast as possible — and how do we know when they're ready?"* The blueprint provides a complete, operational answer: a week-by-week program document that a new SA can follow from Day 1, a manager coaching guide embedded in every week, a stakeholder map, a deliverables checklist, and a technical environment setup guide.

**Job description requirements this directly addresses:**
- *"Design and deliver structured onboarding programs to accelerate ramp for Solutions Architects"*
- *"Build ongoing, programmatic enablement to continuously develop SA technical and sales capabilities"*
- *"Partner with SA leadership to identify skill gaps and translate them into targeted enablement programs"*
- *"Own the end-to-end execution of technical enablement programs, including planning, delivery, and iteration"*

---

## 2. Program Structure

### Three Phases

**Phase 1 — Foundation (Weeks 1–2, ~12 hours)**
Platform orientation, product portfolio, people and systems access. The goal is not deep technical fluency — it is enough platform understanding to pass Gate 1 (architecture walkthrough) and enter Phase 2 without being a bottleneck on the SA team.

**Phase 2 — Practitioner (Weeks 3–6, ~24 hours)**
Deep technical build. Every week has a hands-on lab tied to a real Nebius product: GPU provisioning (Week 3), multi-node Kubernetes cluster deployment (Week 4), MLOps stack deployment (Week 5), and TCO modeling/solution design (Week 6). By end of Phase 2, the SA can architect and defend a Nebius solution independently.

**Phase 3 — Expert (Weeks 7–12, ~16 hours)**
Customer-facing ramp. Token Factory inference architecture (Week 7), first live customer calls (Week 8), demo mastery (Week 9), advanced solution design for complex scenarios (Week 10), capstone build (Week 11), and Expert certification (Week 12). By end of Phase 3, the SA is independently customer-ready with a first solo account assigned.

### Three Certification Gates

Every gate requires a live, observable demonstration — not a quiz or a completion checkbox:

| Gate | Week | Format | What It Tests |
|---|---|---|---|
| Gate 1 | End of Week 2 | 30-min architecture walkthrough with SA Manager | Platform understanding, product portfolio, data center footprint |
| Gate 2 | End of Week 6 | 45-min live architecture demo to mock customer panel | Solution design, TCO modeling, Q&A under pressure |
| Gate 3 | End of Week 12 | 30-min capstone presentation to SA Manager + VP Sales + Senior SA | Full solution design, live demo, competitive defense |

---

## 3. Design Decisions

### The Manager Coaching Strip
Every week card contains a "Manager Action" strip — a specific, observable coaching action the SA's manager should take that week. This is the piece that most distinguishes this blueprint from a self-paced curriculum. Most onboarding programs give the manager a checkbox list at the end of each phase. This program gives the manager a weekly action with a specific evaluation focus.

The coaching strip is visually distinct — a dark background with a green left border and a "Manager Action" label in Nebius green — so a manager scanning the document can find their responsibility without reading the full week card.

### The "By end of this week, the SA can..." Box
Every week card ends with a plain-language capability statement. Not a learning objective ("the SA will understand X") — a behavioral statement ("the SA can do Y without Z"). This forces every week to have a measurable output, not just a content list.

### Three-View Architecture
The artifact has three distinct views in one document:
1. **Timeline view** (the dominant visual) — week bubbles with phase color coding, milestone stars at gate weeks, clickable to jump to week cards
2. **Week detail view** — expandable week cards with activities, people, deliverables, manager coaching, and end-of-week capability
3. **Sidebar panels** — milestone tracker, stakeholder map, deliverables checklist, and technical environment setup

This three-view structure means a new SA, their manager, and an enablement leader can each find what they need from the same document.

### Interactive Timeline
The timeline bubbles are clickable — clicking week 6 expands the Week 6 card and scrolls to it. The phase filter bar (All Weeks / Phase 1 / Phase 2 / Phase 3) shows and hides week cards dynamically, allowing a hiring manager to focus on any phase independently.

### Visual Language
- **Theme:** Dark, technical, premium — consistent with the full portfolio
- **Phase 1 (Foundation):** Blue (`#3B9EFF`) — signals structure, orientation, informational
- **Phase 2 (Practitioner):** Orange (`#FF9F3B`) — signals energy, judgment, hands-on work
- **Phase 3 (Expert):** Purple (`#B47FFF`) — signals mastery, ecosystem, expert-level engagement
- **Green (`#00C853`):** Certification gates, milestone stars, manager coaching elements — all GTM/outcome-connected elements
- **Timeline gradient:** The three-color linear gradient across the top of the timeline bar communicates all three phases in a single visual

---

## 4. Nebius-Specific Content Coverage

Every week is anchored to real Nebius products, real customer examples, and real technical context:

| Week | Nebius Content Referenced |
|---|---|
| Week 1 | Nebius company narrative, $700M raise, Nasdaq listing, NVIDIA Reference Platform status |
| Week 2 | AI Cloud architecture, data center footprint (US, Finland, France, Iceland), Trust Center (SOC 2, HIPAA, GDPR, ISO 27001), SemiAnalysis TCO study |
| Week 3 | GPU tier portfolio (H100, H200, HGX B200, HGX B300, GB200 NVL72, GB300 NVL72), Hopper vs Blackwell, MFU |
| Week 4 | Managed Kubernetes, Soperator/Slurm, NVIDIA Quantum-X800 InfiniBand, storage (1 TB/s throughput, WEKA, VAST Data) |
| Week 5 | Managed MLflow, Apache Spark, PostgreSQL, competitive positioning (AWS, GCP, Azure, CoreWeave), Brave Search, Recraft, Wubble |
| Week 6 | SemiAnalysis TCO framework, solution design for 7B parameter training scenario |
| Week 7 | Token Factory API, vLLM-optimized throughput, DeepSeek R1 inference optimization, Brave Search architecture |
| Week 8 | RAG architecture, Agentic Search, QLoRA, LoRA, PEFT fine-tuning patterns |
| Week 9 | Nebius Solution Library (GitHub Terraform recipes), demo environment design |
| Week 10 | HIPAA-compliant EU AI training, stable diffusion inference (TheStage AI reference), agentic search (RAG) |
| Week 11 | Full-stack capstone: GPU selection, cluster config, storage, MLOps, TCO, compliance |
| Week 12 | Expert certification, solo account assignment, 30-60-90 growth plan |

---

## 5. Technical Build Notes

### Stack
- Pure HTML, CSS, JavaScript — single file, no build step, no external dependencies beyond Google Fonts CDN
- Google Fonts: Syne, JetBrains Mono, Epilogue
- JavaScript: ~50 lines — card expand/collapse, timeline bubble click-to-scroll, phase filter
- Fully responsive: phases stack vertically at 720px, sidebar moves to 2-column grid at 1100px

### Deployment on AWS
```bash
aws s3 cp nebius-sa-onboarding.html s3://your-bucket/portfolio/nebius-sa-onboarding.html
aws cloudfront create-invalidation --distribution-id YOUR_ID --paths "/portfolio/*"
```

**Suggested URL:** `yourdomain.com/portfolio/nebius/sa-onboarding`

---

## 6. How to Present This in an Interview

**Opening frame (30 seconds):**
> "A 90-day onboarding program is only as good as its answer to two questions: what can the SA do at the end of each week that they couldn't do at the start, and what is the manager doing to confirm it? This blueprint answers both questions, for every week. Let me walk you through the structure."

**Key points to walk through:**
1. Click a week bubble in the timeline to show the jump-to-week interactivity
2. Open Week 6 (Gate 2) — show the three components: activities, manager coaching action, and end-of-week capability statement. Point out that the gate requires a live demo, not a quiz.
3. Show the manager coaching strip — explain that giving a manager a weekly specific action is what separates a real onboarding program from a self-paced curriculum
4. Point to the stakeholder map — explain why knowing who to meet and when matters for an SA's credibility ramp
5. Show the technical environment setup panel — point out that everything is provisioned before Day 1, not discovered during Week 3 labs
6. Point out the Nebius-specific content anchoring — GPU tiers by name, real customer examples (Brave Search, Recraft, Wubble), actual product names (Soperator, Token Factory, SemiAnalysis TCO study)

**When asked "how would you compress this if you needed to ramp faster?":**
> "The first decision is which labs to keep and which to convert to guided walkthroughs. Labs 1 and 3 (GPU provisioning and Token Factory) are non-negotiable — an SA who hasn't provisioned a GPU or built an inference endpoint can't credibly support a customer doing either. Lab 2 (Kubernetes) could be converted to a guided walkthrough with a senior SA if the SA has prior Kubernetes experience, shaving 3–4 days off the Phase 2 timeline."

---

## 7. Future Iterations

- **Cohort tracking dashboard:** Connect to the Enablement Metrics Dashboard (Artifact #4) — SA ramp time tracked per cohort, Gate pass rates by week, manager coaching completion rates
- **Specialty tracks:** Life Sciences track (HIPAA-first, drug discovery workloads), Media track (stable diffusion, Wubble-style inference), Physical AI track (robotics simulation)
- **LMS integration:** Each week maps to an LMS module. Gate assessments are assignment submissions with manager scoring via rubric. Automatic progression unlock on gate pass.
- **Manager certification:** Before an SA Manager can run this program, they complete a 4-hour "How to Run the 90-Day Program" certification — covering gate assessment criteria, coaching strip expectations, and how to write structured gate feedback

---

*Document version: 1.0 | Artifact: nebius-sa-onboarding.html | Portfolio: Rus Teston*
