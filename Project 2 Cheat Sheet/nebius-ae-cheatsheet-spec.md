# Nebius AI Cloud — AE Technical Cheat Sheet
## Design Spec & Project Documentation

**Portfolio Artifact #2 of 5**
**Created by:** Rus Teston
**Role target:** Senior Manager, Revenue Enablement / Head of Revenue Enablement
**Company:** Nebius (nebius.com)
**File:** `nebius-ae-cheatsheet.html`

---

## 1. Purpose & Strategic Intent

This artifact demonstrates the ability to translate complex technical content into a practical, role-appropriate sales enablement tool — one of the hardest things to do well in technical enablement. An AE who walks into a customer call without this kind of reference either over-engineers the conversation (trying to be an SA) or under-prepares (unable to qualify the workload). This cheat sheet threads that needle.

**Job description requirements this directly addresses:**
- *"Develop and deliver technical enablement for Account Executives to improve their ability to position and sell complex solutions"*
- *"Create scalable programs that increase technical fluency while remaining practical and relevant to the sales motion"*
- *"Partner with Product Marketing and technical subject matter experts to translate complex product capabilities into effective enablement assets"*
- *"Ensure consistency and quality of technical messaging across enablement programs"*

---

## 2. Content Design Rationale

### The Core Design Problem
AEs need to be technically credible without being technically deep. The failure mode on the left is an AE who gets lost trying to explain InfiniBand topology when they should be qualifying the deal. The failure mode on the right is an AE who says "I'll have to get back to you on that" to every technical question. This cheat sheet is designed to solve the right-side failure while preventing the left.

Every section answers a specific question an AE faces in a real deal moment:

| Section | Deal Moment It Solves |
|---|---|
| One-sentence pitch | "What does Nebius do?" (first 60 seconds) |
| Product portfolio | "Which product do I pitch?" (pre-call planning) |
| GPU tier reference | "What GPU should they use?" (discovery call) |
| Workload decoder | "What are they actually building?" (discovery call) |
| Discovery questions | "What do I ask to qualify this?" (discovery call) |
| Objection responses | "How do I handle pushback?" (any stage) |
| Competitive one-liners | "How do I differentiate?" (competitive deal) |
| Proof points | "What evidence do I have?" (any stage) |
| SA escalation guide | "When do I bring in technical help?" (always) |

### Content Selection Principles
- Every GPU tier name is the actual Nebius/NVIDIA product name — not a generic category
- Every proof point is sourced from a real Nebius customer (Brave Search, Recraft, CentML, Simulacra AI, Wubble) with real numbers
- Objection responses are written in first person, conversational language — not corporate bullet points
- The SA escalation guide uses green/yellow signals so AEs can make a judgment call without a flowchart

---

## 3. Design Decisions

### Visual Language
- **Theme:** Dark, technical, premium — deliberately consistent with the Learning Path Dashboard (Artifact #1) and Nebius's own brand
- **Background:** `#070A0C` near-black with 40px grid overlay at 30% opacity — lighter grid density than Artifact #1 because this is a reference document, not a showcase
- **Accent color:** `#00C853` (Nebius green) for the primary card accent, discovery questions, GPU flagship tier, and proof chips
- **Section accent colors:**
  - Green: Strategic/positioning content (one-sentence pitch, GPU tiers, discovery questions)
  - Blue (`#3B9EFF`): Product portfolio + SA escalation — informational, structural
  - Orange (`#FF9F3B`): Workload decoder — signals "this requires a judgment call"
  - Red (`#FF4D4D`): Objections + competitive — signals urgency and competitive tension
  - Purple (`#B47FFF`): Proof points — signals credibility and external validation

### Typography
- **Syne** (display/headings): Used for section headlines, GPU names as flagship, proof stats — consistent with Artifact #1
- **JetBrains Mono** (labels/metadata): Used for card labels, GPU badges, workload keys, question numbers — signals technical reference material
- **DM Sans** (body): A refined humanist sans — slightly warmer and more readable than Inter for dense reference content at small sizes

### Layout Architecture
- **Density-optimized**: This is a cheat sheet, not a presentation — information density is intentional. Everything visible at a glance without scrolling on a 1440px display.
- **Row-based grid**: Each row groups semantically related sections — positioning + products go together; GPU tiers + workload decoder go together; competitive + proof + escalation go together
- **No card is the same height**: Heights are determined by content, not forced to match — avoids the "grid for the sake of grid" trap
- **Color-coded by section theme**: An AE scanning this quickly can find the competitive section (red top border) or the proof points (purple) without reading headers

### GPU Tier Design
- Flagship tiers (GB300, GB200) get a distinct treatment — green text, gradient background, left highlight — so AEs know immediately these are the top of the portfolio
- Each tier has a badge that communicates the primary use case orientation (Training / Balanced / Extended Mem / Cost-Effective) in the fewest possible characters
- The InfiniBand footnote at the bottom is a one-liner that gives AEs enough to sound credible without requiring them to understand the technology

### Workload Decoder Design
- Three-column layout mirrors the three workload types — AEs can scan across a row (Customer says → They need → Pitch → GPU → Proof) to get the complete picture for any workload type
- Each column has a real customer proof point at the bottom — discovery conversations should always end with a reference, not just a feature description

### Objection Handler Design
- Each objection has a flag (Competitive / Commercial / Trust / Technical) so AEs can find the right response by objection type, not by memory
- Responses start with a bold coaching cue in the first sentence — AEs read that first, then the full response
- Language is conversational and first-person — designed to be spoken, not read aloud from a script

### Proof Points Design
- Large stat number as the headline — AEs remember numbers, not prose
- Customer and workload type called out below in monospace — so AEs can name-drop accurately
- Six proof points chosen to cover different dimensions: scale (11M+ queries), cost (5x lower), quality (20B params / benchmark), speed (90% faster), credibility (#19 supercomputer), and third-party validation (SemiAnalysis Gold Medal)

---

## 4. Nebius Product & Content Coverage

| Content Area | Source / Nebius Reference |
|---|---|
| One-sentence positioning | nebius.com homepage — "ultimate cloud for AI innovators" |
| NVIDIA Reference Platform Partner status | nebius.com/about + partner program page |
| Nasdaq listing + $700M raise | nebius.com/investor-hub |
| GPU tier names and specs | nebius.com/ai-cloud — GB300 NVL72, GB200 NVL72, HGX B300/B200/H200/H100 |
| InfiniBand / Quantum-X800 | nebius.com/ai-cloud technical specs |
| Token Factory positioning | nebius.com/services/token-factory |
| Managed MLflow, Spark, PostgreSQL | nebius.com/ai-cloud — fully managed services |
| Soperator (Slurm) | nebius.com/services/soperator |
| Storage: 1 TB/s throughput, WEKA, VAST Data | nebius.com/services/storage |
| SemiAnalysis Gold Medal / TCO study | nebius.com/calculating-the-total-cost-of-gpu-cluster |
| Brave Search proof point (11M+ daily, ~100% util) | nebius.com customer case study |
| CentML proof point (5x lower costs) | nebius.com customer case study |
| Recraft proof point (20B params, DALL·E 3 benchmark) | nebius.com customer case study |
| Simulacra AI proof point (90% faster) | nebius.com customer case study |
| ISEG #19 supercomputer | nebius.com homepage |
| Compliance: SOC 2, HIPAA, GDPR, ISO 27001 | nebius.com/trust-center |
| EU data centers (Finland, France, Iceland) | nebius.com/nebius-partner-program |
| Terraform, Kubernetes, Slurm, open standards | nebius.com/ai-cloud + solution library |

---

## 5. Technical Build Notes

### Stack
- Pure HTML, CSS, JavaScript — single file, zero dependencies beyond Google Fonts CDN
- Google Fonts: Syne, JetBrains Mono, DM Sans
- No JavaScript required — this document is purely CSS-driven
- Fully responsive: multi-column → single column via CSS Grid breakpoints

### Print Optimization
This cheat sheet is designed to print well on A3/tabloid or 11×17" paper in landscape mode. To print cleanly:
- Open in Chrome
- File → Print → More settings
- Paper size: Tabloid (11×17) or A3, Landscape
- Scale: Fit to page
- Background graphics: Enable (required for the dark theme)

### Deployment on AWS
```bash
# Upload to S3
aws s3 cp nebius-ae-cheatsheet.html s3://your-bucket-name/portfolio/nebius-ae-cheatsheet.html

# CloudFront invalidation
aws cloudfront create-invalidation --distribution-id YOUR_DIST_ID --paths "/portfolio/*"
```

**Suggested URL:** `yourdomain.com/portfolio/nebius/ae-cheatsheet`

---

## 6. How to Present This in an Interview

**Opening frame (20 seconds):**
> "AE enablement lives or dies on one test: does the AE walk into a discovery call more prepared than they would have been without it? This cheat sheet is built to pass that test. Every section answers a specific question an AE faces in a real deal — not in a training room."

**Key points to walk through:**
1. Point out the workload decoder — explain why decoding what a customer *says* versus what they *need* is the core AE technical fluency skill
2. Show the objection handler — note that each response starts with a bold coaching cue, and the language is written to be spoken, not read
3. Point to the SA escalation guide — explain that a clear escalation framework is what separates an AE who burns SA time unnecessarily from one who brings them in at exactly the right moment
4. Name-drop the proof points — mention Brave Search (11M+ daily AI answers), CentML (5x cost reduction), and Recraft (20B params) as specific Nebius customers you referenced
5. Note the color coding — the four accent colors (green, orange, red, purple) map to four different deal moments so an AE can find what they need at a glance under pressure

**When asked "how would you validate this is working?":**
> "Two signals: manager observation on discovery calls within 30 days — are AEs asking the six questions on this sheet? And win/loss data at 90 days — specifically, are deals where an AE used this reference qualifying faster and losing less often to competitive displacement?"

---

## 7. Future Iterations

- **Vertical versions**: Life Sciences edition (HIPAA-first, CRISPR-GPT proof point), Media edition (Wubble, Recraft), Physical AI edition
- **Interactive web version**: Click a workload type → expands to show the full discovery question set for that workload
- **Seismic / Highspot card**: Package the objection handler section as a Seismic card so AEs can pull it up on mobile during a call
- **Quarterly refresh cycle**: GPU tier table updated with each new Nebius product launch; proof points updated as new customer case studies are published

---

*Document version: 1.0 | Artifact: nebius-ae-cheatsheet.html | Portfolio: Rus Teston*
