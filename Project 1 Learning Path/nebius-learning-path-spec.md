# Nebius AI Cloud — Role-Based Enablement Learning Paths
## Design Spec & Project Documentation

**Portfolio Artifact #1 of 5**
**Created by:** Rus Teston
**Role target:** Senior Manager, Revenue Enablement / Head of Revenue Enablement
**Company:** Nebius (nebius.com)
**File:** `nebius-learning-path.html`

---

## 1. Purpose & Strategic Intent

This artifact demonstrates the ability to design a **programmatic, multi-audience enablement system** from scratch — one of the core expectations of the role. Rather than showing a single training module or a slide deck, this learning path dashboard proves systems thinking: how do you ramp three entirely different audiences (SAs, AEs, Partners) on the same platform simultaneously, with role-appropriate depth, measurable milestones, and a clear progression from novice to certified expert?

**Job description requirements this directly addresses:**
- *"Design and deliver structured onboarding programs to accelerate ramp for Solutions Architects"*
- *"Develop and deliver technical enablement for Account Executives"*
- *"Build and scale technical enablement programs for partners"*
- *"Develop role-based learning paths, certifications, and technical training programs across audiences"*
- *"Partner with Product Marketing and technical subject matter experts to translate complex product capabilities into effective enablement assets"*

---

## 2. Audience Design Rationale

### Solutions Architect Track — "Technical Mastery"
- **Ramp target:** 12 weeks / ~52 hours seat time
- **Philosophy:** SAs need genuine technical depth, not awareness-level summaries. Every module includes hands-on labs and requires the SA to *demonstrate* capability, not just describe it.
- **Phase logic:** Foundation (platform + GPU literacy) → Practitioner (orchestration, networking, MLOps) → Expert (inference architecture, TCO modeling, capstone design)
- **Certification gates:** Technical assessment → Live architecture demo → Solution design presentation

### Account Executive Track — "Sales Fluency"
- **Ramp target:** 8 weeks / ~34 hours seat time
- **Philosophy:** AEs don't need to be engineers — they need enough technical fluency to lead discovery, qualify workloads, handle objections, and bring in the SA at the right moment. Every module is grounded in what an AE *does* in a deal, not what they need to *know* abstractly.
- **Phase logic:** Foundation (narrative + workload literacy + pricing) → Practitioner (competitive displacement + verticals + co-sell) → Expert (expansion selling + executive selling + deal simulation)
- **Certification gates:** Mock discovery + pitch → Full discovery role-play → Closed deal retrospective

### Partner Track — "Partner Competency"
- **Ramp target:** 10 weeks / ~38 hours seat time
- **Philosophy:** Partner enablement must build *independence* — the goal is partners who can win and deliver without leaning on Nebius resources constantly. Modules are sequenced to mirror the actual partner lifecycle: onboard → build → go-to-market → scale.
- **Phase logic:** Foundation (program onboarding + Token Factory API + cloud fundamentals) → Practitioner (solution building + GTM alignment + support model) → Expert (advanced solutions + thought leadership + first win review)
- **Certification gates:** Knowledge assessment + API demo → GTM plan review → First customer win presentation

---

## 3. Nebius Product Coverage

Every module is mapped to real Nebius products and capabilities. The following product areas are explicitly covered:

| Product / Capability | Tracks Covered |
|---|---|
| Nebius AI Cloud (platform overview) | SA, AE, Partner |
| NVIDIA GPU portfolio: H100, H200, B200, GB200 NVL72, GB300 NVL72 | SA, AE |
| Managed Kubernetes (Managed K8s) | SA, Partner |
| Slurm / Soperator | SA |
| NVIDIA InfiniBand / Quantum-X800 fabric | SA |
| High-Performance Storage (in-house, WEKA, VAST Data) | SA |
| Managed MLflow, Apache Spark, PostgreSQL | SA |
| Token Factory API | SA, AE, Partner |
| Nebius Partner Program (VAR, ISV/MSP, Alliance) | AE, Partner |
| Nebius Solution Library (GitHub / Terraform) | Partner |
| RAG, Agentic Search solutions | Partner |
| Compliance: SOC 2, HIPAA, GDPR, ISO 27001 | SA, AE |
| TCO / SemiAnalysis framework | SA, AE |
| Customer success stories: Brave, Recraft, CRISPR-GPT, Wubble, Simulacra AI | AE |

---

## 4. Design Decisions

### Visual Language
- **Theme:** Dark, technical, premium — deliberately mirroring Nebius's own brand aesthetic
- **Background:** `#080B0D` near-black with a subtle 48px grid overlay at 35% opacity. Creates a technical "graph paper" feel without being distracting.
- **Accent color:** `#00C853` — Nebius's own brand green, used consistently for certification gates, the creator byline, stat values, and interactive elements
- **Radial glow:** A large, low-opacity green radial gradient fixed behind the page header reinforces the Nebius brand identity without competing with content
- **Track colors:**
  - SA: `#3B9EFF` (blue) — signals technical depth and engineering precision
  - AE: `#FF7B3B` (orange) — signals energy, commercial momentum
  - Partner: `#B47FFF` (purple) — signals ecosystem and collaboration

### Typography
- **Syne** (display/headings): A geometric, high-weight display font with strong personality — modern without being generic. Used for the main headline, track titles, and stat values.
- **JetBrains Mono** (labels/badges/tags): A developer-grade monospace font for all metadata labels, role badges, phase numbers, and competency tags. Signals technical credibility.
- **Inter** (body): Clean, readable body text for descriptions, module objectives, and filter controls.

### Layout Architecture
- Three-column grid (one per track) that collapses to single-column on mobile
- Filter bar allows the hiring manager to focus on one track at a time — a deliberate UX decision that demonstrates you think about how people will *consume* enablement content, not just produce it
- Expanding module cards avoid overwhelming the viewer with information density — everything is discoverable but not all visible at once
- Certification gates are visually distinct (green glowing bars) to reinforce the concept of measurable milestones

### Module Card Design
- Each card shows: icon, module name, format tag, duration tag, and product tag at a glance
- Expanding a card reveals: learning objectives (specific, measurable, behavioral) and a competency badge
- The left-border accent on expanded cards (colored by track) reinforces which audience you're looking at

---

## 5. Curriculum Design Philosophy

### Learning Objectives Format
All objectives follow a **behavioral, measurable format** — not vague awareness statements. Each objective starts with a verb that maps to an observable action:
- *Articulate, Deliver, Navigate* → communication/sales skills
- *Architect, Configure, Deploy, Implement* → technical/hands-on skills
- *Identify, Map, Compare* → analytical/discovery skills
- *Build, Produce, Demonstrate* → output/capstone skills

### Phase Progression Logic
Each phase builds on the previous. Foundation modules are prerequisites for Practitioner modules. Certification gates require *demonstration*, not just completion — a deliberate design choice that mirrors how strong enablement programs measure competency vs mere content consumption.

### Seat Time Estimates
- SA: ~52 hours (weighted toward labs and hands-on work; highest technical depth)
- AE: ~34 hours (balanced across sessions and self-paced; faster ramp needed for quota-carrying roles)
- Partner: ~38 hours (includes collaborative project work with Nebius teams)

---

## 6. Technical Build Notes

### Stack
- Pure HTML, CSS, JavaScript — no frameworks, no dependencies, no build step
- Google Fonts loaded via CDN: Syne, JetBrains Mono, Inter
- All interactivity (module expand/collapse, track filtering) implemented in vanilla JS (~40 lines)
- Fully responsive: 3-column grid → 2-column → 1-column via CSS Grid breakpoints

### Deployment on AWS
This file can be deployed in multiple ways on your AWS-hosted personal site:

**Option A — Static S3 + CloudFront (recommended):**
```bash
# Upload to S3 bucket
aws s3 cp nebius-learning-path.html s3://your-bucket-name/portfolio/nebius-learning-path.html

# Invalidate CloudFront cache if applicable
aws cloudfront create-invalidation --distribution-id YOUR_DIST_ID --paths "/portfolio/*"
```

**Option B — Direct EC2 / Nginx:**
Copy the file to your web root: `/var/www/html/portfolio/nebius-learning-path.html`

**Suggested URL:** `yourdomain.com/portfolio/nebius-ai-enablement/learning-path`

### Browser Support
Tested against: Chrome 120+, Safari 17+, Firefox 121+, Edge 120+
CSS features used: Grid, Custom Properties, `clamp()`, `backdrop-filter` (not used), `@keyframes`

---

## 7. How to Present This in an Interview

**Opening frame (30 seconds):**
> "One of the first things I'd do at Nebius is map out who needs to know what — and to what depth — before I ever build a single piece of content. This learning path dashboard is how I'd visualize that design work. It covers three audiences simultaneously, it's anchored to real Nebius products and customer use cases, and it has built-in competency gates that separate *completion* from *capability*."

**Key points to walk through:**
1. Show the three tracks and explain the philosophy difference between them (depth vs fluency vs independence)
2. Click into 2–3 module cards to show the behavioral objective format
3. Point out the certification gates and explain why they require *demonstration*, not just consumption
4. Call out specific Nebius content: Token Factory, vLLM/DeepSeek R1, the SemiAnalysis TCO framework, real customer examples
5. Mention that the design mirrors Nebius's own brand language — showing you do your homework

**When asked "how did you build this?":**
> "I researched Nebius's product portfolio, partner program structure, and customer success stories directly from the website before writing a single line. The curriculum design came first — I mapped objectives to roles and phases on paper — and the visual execution followed the Nebius brand direction deliberately. The whole thing is a single HTML file, deployable anywhere."

---

## 8. Future Iterations (Shows Program Thinking)

If asked how you'd evolve this, mention:
- **LMS integration:** Export each module as a SCORM object for delivery in Docebo, Cornerstone, or Seismic Learning
- **Completion tracking:** Add a lightweight localStorage-based progress tracker (or connect to an LMS API)
- **Versioning:** Tie modules to Nebius product release cycles — new GPU tier released = Foundation module updated within 2 weeks of launch
- **Localization:** Module content available in EN + target partner markets (DE, FR, FI given Nebius's European data center presence)
- **Feedback loop:** Add a post-module feedback widget (NPS + open comment) to feed the continuous improvement cycle

---

*Document version: 1.0 | Artifact: nebius-learning-path.html | Portfolio: Rus Teston*
