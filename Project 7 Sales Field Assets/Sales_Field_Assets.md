# Nebius AI Cloud — Sales Field Assets
### Prepared for the Nebius Sales Team | April 2026

---

## Table of Contents
1. [Battle Cards](#battle-cards)
2. [Discovery Guides](#discovery-guides)
3. [Qualification Frameworks](#qualification-frameworks)
4. [Demo Narratives](#demo-narratives)
5. [Use-Case Playbooks](#use-case-playbooks)
6. [Objection-Handling Guides](#objection-handling-guides)
7. [Competitive Positioning](#competitive-positioning)
8. [Manager Coaching Tools](#manager-coaching-tools)

---

## 1. Battle Cards

### Battle Card A: Nebius vs. CoreWeave

**Positioning Summary:** CoreWeave is the scale-first, enterprise-only training powerhouse. Nebius is the full-stack, developer-friendly AI cloud with lower costs, faster onboarding, and a richer software layer — backed by the same NVIDIA relationship.

| Dimension | Nebius | CoreWeave |
|---|---|---|
| **H100 Hourly Rate** | ~$2.10–$2.95/hr | ~$4.76/hr |
| **Onboarding** | Self-serve + free credits | Enterprise intake form required |
| **Software Stack** | Full-stack: K8s, Slurm, PostgreSQL, MLOps, AI Studio | Raw compute-first; limited managed services |
| **Compliance** | HIPAA, SOC 2, GDPR, ISO 27001 | SOC 2; limited GDPR coverage |
| **EU Data Residency** | ✅ Finland (operational), expanding | ❌ Primarily US-based |
| **Spot Market Flexibility** | High — on-demand + shorter contracts | >98% locked long-term contracts |
| **Balance Sheet** | Cash-rich, low debt | Highly leveraged |
| **NVIDIA Relationship** | Reference Platform Cloud Partner; $2B NVIDIA investment | NVIDIA investor; tight integration |
| **Customer Concentration** | Diversified: startups, enterprises, AI labs | Concentrated: Microsoft = 62% of 2024 revenue |
| **Inference Tooling** | Nebius AI Studio (managed inference API) | Limited; relies on customers' own tooling |
| **TCO Study** | Lowest TCO across training, RL, and inference (SemiAnalysis) | Higher per-GPU cost |

**When Nebius Wins:**
- Customer needs managed services on top of GPU compute
- European data residency or GDPR compliance required
- Customer wants self-serve access, free trial credits, faster start
- Regulated industry (healthcare, finance) needing HIPAA/SOC 2
- Mid-market / startup needing full-stack without enterprise procurement complexity
- Inference workloads needing API-level access (AI Studio)

**When CoreWeave Might Win:**
- Frontier AI lab needing maximum bare-metal cluster scale (>10,000 GPUs immediately)
- Customer already has long-term committed contracts in place

**Winning Statements Against CoreWeave:**
- *"CoreWeave locks you into multi-year contracts at nearly 2x our H100 price. With Nebius, you get the same NVIDIA hardware, at a lower TCO validated by SemiAnalysis, with the flexibility to scale up or down."*
- *"CoreWeave requires enterprise sales engagement just to get access. You can launch on Nebius today, with free credits, in hours — not weeks."*
- *"We're the only AI cloud with full GDPR and HIPAA coverage AND a live EU data center. If your data can't leave Europe, CoreWeave isn't an option."*

---

### Battle Card B: Nebius vs. AWS / Azure / GCP (Hyperscalers)

**Positioning Summary:** Hyperscalers are built for general-purpose compute with GPU tacked on. Nebius is built from the ground up for AI — faster, cheaper, and without the DevOps overhead of adapting a general cloud to AI workloads.

| Dimension | Nebius | AWS / Azure / GCP |
|---|---|---|
| **GPU Pricing** | H100 from $2.10/hr | $12–$20+/hr for comparable GPU instances |
| **Provisioning Time** | Hours | Days to weeks (quota approvals, wait lists) |
| **AI-Specialization** | Purpose-built for AI training + inference | General cloud with AI added on |
| **Managed AI Orchestration** | Kubernetes + Slurm pre-configured | DIY setup required; add-on tools extra cost |
| **Inference API** | Nebius AI Studio (open-source LLMs, image models) | Proprietary APIs; closed models |
| **Storage for AI** | 1 TB/s read throughput, 2 GB/s per GPU | Standard cloud storage (not AI-optimized) |
| **MFU (Model FLOPS Utilization)** | Maximized; minimal virtualization overhead | Shared infrastructure; lower effective MFU |
| **Vendor Lock-in** | Open-source stack; standard APIs | Strong proprietary lock-in |
| **Compliance** | HIPAA, SOC 2, GDPR, ISO 27001 | Compliant but complex procurement |

**Winning Statements Against Hyperscalers:**
- *"AWS GPU instances cost 5–8x more per hour than Nebius. For the same $1M budget, you get dramatically more compute time — which means faster model iteration."*
- *"Hyperscalers make you wait weeks for GPU quota approvals. Nebius provisions thousands of GPUs within hours."*
- *"AWS infrastructure wasn't built for AI. You're paying the 'general purpose tax.' Nebius is engineered from rack design to software layer specifically for AI workloads — which is why we deliver maximum Model FLOPS Utilization."*

---

### Battle Card C: Nebius vs. Lambda Labs

**Positioning Summary:** Lambda is a lean, developer-friendly GPU renter. Nebius offers everything Lambda does, plus a full managed services stack, enterprise compliance, EU presence, and a production-ready inference layer.

| Dimension | Nebius | Lambda Labs |
|---|---|---|
| **H100 Pricing** | ~$2.10–$2.95/hr | Competitive (~$2/hr spot) |
| **Managed Services** | Full: K8s, Slurm, PostgreSQL, MLOps | Minimal; primarily raw compute |
| **Inference Layer** | Nebius AI Studio (managed API) | No managed inference product |
| **EU Data Centers** | ✅ Finland, expanding | ❌ Primarily US |
| **Compliance** | HIPAA, SOC 2, GDPR, ISO 27001 | Limited |
| **Hardware Availability** | Blackwell, Hopper, Vera Rubin access | Hopper-focused |
| **Enterprise SLAs** | Full enterprise SLAs | Limited |
| **Custom Hardware** | Proprietary racks + servers | Standard OEM |

**Winning Statement:**
- *"Lambda is great for prototyping. Nebius is built for production. When you're ready for enterprise SLAs, GDPR compliance, managed Kubernetes, and an inference API — that's when you move to Nebius."*

---

## 2. Discovery Guides

### Pre-Call Research Checklist
- [ ] What AI models is the prospect training/deploying? (LLM, image, audio, RL?)
- [ ] What cloud are they on today? (AWS, GCP, CoreWeave, Lambda, on-prem?)
- [ ] What GPU hardware do they currently use?
- [ ] What is their team size (ML engineers, DevOps)?
- [ ] Are they in a regulated industry? (healthcare, finance, legal)
- [ ] EU or multi-region requirements?
- [ ] Public AI products / recently launched models?

---

### Discovery Call Framework: The TRAIN Model

**T — Training & Inference Workloads**
- "Walk me through your current AI infrastructure setup. What types of workloads are you running — foundation model pre-training, fine-tuning, or production inference?"
- "How large are your largest training runs? Are you hitting GPU count or compute budget ceilings?"
- "What's your current average GPU utilization? Are you seeing Model FLOPS Utilization (MFU) below expectations?"
- "Do you serve models in production today? What does your inference stack look like?"

**R — Resources & Costs**
- "What's your current monthly cloud infrastructure spend?"
- "How are you currently provisioning GPUs — on-demand, reserved, or spot?"
- "Have you done any TCO analysis comparing providers? What did you find?"
- "How much engineering time does your team spend on infrastructure management vs. model development?"

**A — Access & Agility**
- "How long does it take you to provision a new GPU cluster today? Is that acceptable?"
- "Have you ever had training jobs fail due to infrastructure issues? How did that impact your timeline?"
- "Do you need the ability to scale up on short notice — say, for a large batch training run?"
- "How quickly do you need to be able to onboard new team members to the infrastructure?"

**I — Infrastructure Constraints & Compliance**
- "Do you have data residency requirements? European, US, or specific country?"
- "Are you subject to any compliance frameworks — HIPAA, SOC 2, GDPR, ISO 27001?"
- "Do you have a vendor approval process or security review requirements for cloud providers?"
- "Are there any open-source model licensing requirements that affect your infrastructure choices?"

**N — Needs, Timeline & Next Steps**
- "What's driving this evaluation now? Is there a specific project, product launch, or budget cycle?"
- "If you could change one thing about your current infrastructure setup, what would it be?"
- "Who else is involved in this decision — procurement, security, engineering leadership?"
- "What would a successful outcome look like at the end of a 90-day trial?"

---

### Pain Discovery Probes (Deep Dives)

**If on Hyperscalers:**
- "How long did it take to get your last GPU quota approved?"
- "Have you ever had a critical training run delayed because capacity wasn't available?"
- "What percentage premium are you paying vs. specialized AI cloud providers? Have you modeled that delta?"

**If on CoreWeave:**
- "Are you locked into long-term take-or-pay contracts? Does that flexibility match your business needs?"
- "Do you have GDPR or EU data residency requirements? How are you solving for that today?"
- "What additional services do you need that aren't covered by compute alone — orchestration, inference APIs, databases?"

**If on Lambda / Runpod:**
- "As you move from experimentation to production, what gaps are you running into?"
- "Do you have enterprise SLA requirements that your current provider can't meet?"
- "Are you handling Kubernetes and cluster management yourself? How much time does that take?"

---

## 3. Qualification Frameworks

### Nebius MEDDPICC Qualification Scorecard

**Score each dimension 0–3. Deals scoring 18+ are high-priority. Below 10 require re-qualification.**

---

**M — Metrics**
- *Key Question:* "What specific business or technical outcomes are you measuring?"
- 3 = Quantified TCO savings target, MFU improvement, provisioning time reduction, or inference throughput goal
- 2 = General cost reduction or performance improvement desired
- 1 = Vague "better AI infrastructure" stated
- 0 = No metrics defined
- *Nebius-Specific Proof Points:* Brave Search (100% GPU utilization, 11M+ daily AI answers); SemiAnalysis study (lowest TCO); provisioning in hours vs. weeks

**E — Economic Buyer**
- *Key Question:* "Who controls the infrastructure budget? Who signs the contract?"
- 3 = VP Engineering, CTO, or Head of AI identified and engaged
- 2 = IT or ML engineering champion identified; budget holder not yet accessed
- 1 = Working with individual contributors only
- 0 = Unknown

**D — Decision Criteria**
- *Key Question:* "What are your must-haves and nice-to-haves for a new GPU cloud?"
- 3 = Criteria documented; Nebius meets all must-haves (NVIDIA hardware, compliance, cost)
- 2 = Criteria partially known; Nebius competitive
- 1 = Criteria unclear
- 0 = No criteria defined
- *Watch For:* Compliance requirements (HIPAA/GDPR/SOC 2), EU data residency, Kubernetes managed services, AI Studio inference API

**D — Decision Process**
- *Key Question:* "Walk me through how a decision like this gets made — who's involved and what are the steps?"
- 3 = Clear process with timeline; Nebius included in formal evaluation
- 2 = Process partly known; some ambiguity in approvers
- 1 = "We'll figure it out" — informal process
- 0 = Unknown

**P — Paper Process**
- *Key Question:* "What does your procurement and legal review process look like for a new cloud vendor?"
- 3 = Security review and vendor approval timeline known; SOC 2 / ISO 27001 already accepted
- 2 = Process known; some steps unclear
- 1 = Procurement involved but timeline unknown
- 0 = Not yet started; unknown

**I — Identify Pain**
- *Key Question:* "What's broken or costing you right now with your current infrastructure?"
- 3 = Explicit, quantified pain: GPU cost, wait times, failed training runs, compliance gaps, DevOps burden
- 2 = General dissatisfaction stated
- 1 = Passive interest, no clear pain
- 0 = No pain identified — re-qualification needed

**C — Champion**
- *Key Question:* "Who internally is our advocate and will fight for this decision?"
- 3 = ML Engineering Lead or Head of AI actively championing; has access to economic buyer
- 2 = Champion identified but not yet tested under pressure
- 1 = Potential champion; not yet confirmed
- 0 = No champion

**C — Competition**
- *Key Question:* "Who else are you evaluating? What's your current provider?"
- 3 = Competitive situation known; Nebius differentiation clear and accepted by champion
- 2 = Competition known; Nebius positioning not fully established
- 1 = Competition suspected but not confirmed
- 0 = Unknown — critical risk

---

### ICP (Ideal Customer Profile) Quick-Check

**Tier 1 (Immediate Priority):**
- AI company training models >1B parameters
- Current GPU cloud spend >$50K/month
- European HQ or GDPR data residency requirements
- Regulated industry (healthcare, finance, pharma) needing HIPAA + SOC 2
- Team of 5+ ML engineers

**Tier 2 (Strong Fit):**
- AI-first product company (inference in production)
- Using hyperscalers for GPU and frustrated with cost/availability
- Startup with Series B+ funding and AI as core product
- Using open-source LLMs requiring managed inference (AI Studio fit)

**Tier 3 (Nurture):**
- Experimenting with AI but no production workloads
- Single GPU use cases (no distributed training)
- IT-led evaluation without ML engineering involvement

---

## 4. Demo Narratives

### Standard Demo Flow: "From Zero to Training in Minutes"
*Duration: 30–45 minutes | Audience: ML Engineers, Head of AI, CTO*

---

**Opening Hook (2 min)**
> "Today I want to show you what it looks like to go from signing up on Nebius to running your first distributed training job — and we'll do it without a single DevOps ticket. But first, let me ask — how long does it take you to provision a GPU cluster today on [current provider]?"

*[Let them answer. Use their answer as the contrast throughout.]*

---

**Act 1: Infrastructure in Minutes (8 min)**

*Story:* "Your ML engineers should spend their time on models, not infrastructure."

- **Show:** Nebius AI Cloud console → spin up an H100 cluster
- **Highlight:** Pre-configured NVIDIA drivers, CUDA libraries, InfiniBand networking — zero manual setup
- **Show:** Topology-aware scheduling — the system understands your GPU cluster geometry
- **Transition:** *"Notice we're already ready to train. On AWS, you'd still be waiting for quota approval."*

**Key talking points:**
- Thousand-GPU clusters available today in EU and US
- Node health monitoring and auto-repair — training jobs survive hardware failures
- Latest NVIDIA Blackwell (B200, GB200 NVL72) available now
- NVIDIA Reference Platform Cloud Partner — same hardware, optimized configuration

---

**Act 2: Maximum Performance (8 min)**

*Story:* "Not all GPU clouds are equal — and the difference shows up in your model quality and training speed."

- **Show:** MFU benchmarks — Nebius minimizes virtualization overhead
- **Show:** Storage performance: 1 TB/s read throughput for shared filesystems; 2 GB/s per GPU for object storage
- **Show:** Non-blocking InfiniBand fabric — AllReduce operations run at wire speed
- **Transition:** *"The SemiAnalysis study ran real production workloads — LLM pre-training, multimodal RL, and inference — and Nebius delivered the lowest TCO in every scenario."*

---

**Act 3: Full Stack — Not Just Compute (8 min)**

*Story:* "Nebius is the only AI cloud where compute, orchestration, storage, and inference live in one place."

- **Show:** Managed Kubernetes — zero configuration, production-ready
- **Show:** Managed Slurm — for HPC and research team workflows
- **Show:** Built-in observability — job monitoring, GPU utilization dashboards, alerting
- **Show:** Managed PostgreSQL for experiment tracking metadata
- **Transition:** *"This is why customers like Brave Search run 11 million AI-powered queries a day on Nebius — it's not just a GPU rental, it's a production platform."*

---

**Act 4: Nebius AI Studio — Inference Made Simple (8 min)**

*Story:* "When you're ready to serve your model — or access best-in-class open-source models via API — AI Studio is your inference layer."

- **Show:** AI Studio playground — compare models side by side
- **Show:** Single API for LLMs + image generation (Flux Schnell, Flux Dev, SDXL)
- **Show:** 100M+ tokens/minute standard capacity; auto-scaling
- **Show:** Per-token / per-image pricing — no idle capacity cost
- **Transition:** *"If you're building an AI product, you can train on Nebius AI Cloud and serve via AI Studio — one platform, one vendor, one bill."*

---

**Act 5: Security & Compliance (5 min)**

*Story:* "Enterprise AI needs enterprise trust."

- **Show:** Compliance certifications: HIPAA, SOC 2 Type II, GDPR, ISO 27001
- **Show:** Tenant-level isolation — your workloads are never shared
- **Show:** EU data centers (Finland) — data never leaves Europe for GDPR-sensitive workloads
- **Show:** IAM capabilities — granular access controls

---

**Closing & Call to Action (5 min)**
> "What we've shown you today is a complete AI cloud — not just GPU boxes. You get the compute, the orchestration, the inference layer, and the compliance — all at a TCO that's been independently validated as the lowest in the market. What would it mean for your team to ship your next model 30% faster, at half the infrastructure cost?"

*Next Step Offer:* Free trial credits + dedicated onboarding engineer for first 30 days.

---

## 5. Use-Case Playbooks

### Playbook 1: Foundation Model Pre-Training

**Target Buyer:** AI Labs, well-funded AI startups, research organizations
**Champion:** Head of AI Infrastructure / ML Platform Lead
**Economic Buyer:** CTO, VP Engineering

**The Situation:**
Company is training a large language model (7B–70B+ parameters) and faces: (a) massive compute costs on hyperscalers, (b) slow cluster provisioning, or (c) training instability due to hardware failures.

**Nebius Solution:**
- NVIDIA HGX H100 / H200 / Blackwell B200 clusters, 1,000+ GPU available
- Non-blocking InfiniBand fabric (NVIDIA Quantum-2) for minimum AllReduce overhead
- Managed Slurm or Kubernetes for job orchestration
- Fault-tolerant infrastructure with node health monitoring + auto-repair
- 1 TB/s shared filesystem throughput for dataset streaming

**ROI Metrics to Quantify:**
- Cost per training run: H100 at $2.10/hr vs. AWS p4d.24xlarge ~$32/hr (8x H100s = $4/GPU/hr)
- Faster provisioning: hours vs. 2–3 weeks on hyperscalers
- Training job continuity: auto-repair prevents costly restarts
- Engineering time saved: no cluster configuration required → 20–40 hrs saved per cluster

**Reference Customer:**
Recraft trained their first generative AI model for designers from scratch on Nebius using PyTorch + Kubeflow on Nebius AI Cloud, without provisioning delays or infrastructure failures.

**Qualification Signal:**
- Training budget >$100K/month
- Training runs lasting days to weeks
- Team frustrated with GPU availability on current provider

---

### Playbook 2: Production AI Inference at Scale

**Target Buyer:** AI product companies, SaaS platforms with AI features
**Champion:** Head of AI Product / ML Engineer
**Economic Buyer:** VP Product, CTO

**The Situation:**
Company has a trained model and needs to serve it to end users reliably, at low latency, high throughput, and acceptable cost — without managing complex infrastructure.

**Nebius Solution:**
- **Nebius AI Studio:** Managed inference API for open-source LLMs + image models
- Single API endpoint, 100M+ tokens/minute capacity
- Auto-scaling — no idle GPU cost
- Per-token / per-image pricing for predictable unit economics
- NVIDIA NIM™ microservices for enterprise-grade inference

**ROI Metrics:**
- Inference cost reduction vs. OpenAI API: 40–70% for equivalent open-source models
- Nearly 100% GPU utilization (Brave Search benchmark)
- Latency: low time-to-first-token for real-time applications
- 11M+ AI answers/day proven at scale (Brave Search)

**Reference Customer:**
Brave Search uses Nebius AI Cloud to deliver AI-powered search summaries for 11 million daily queries at nearly 100% GPU utilization, with low latency and high throughput — while maintaining strict privacy standards.

**Qualification Signal:**
- Serving AI features to end users at volume (>1M API calls/day)
- Looking to migrate from OpenAI API to open-source models (cost reduction)
- Need managed inference without dedicated ML ops team

---

### Playbook 3: MLOps & AI Platform for Enterprise Teams

**Target Buyer:** Enterprise companies building internal AI platforms
**Champion:** ML Platform Engineer, AI Center of Excellence Lead
**Economic Buyer:** VP Engineering, CDO/CAIO

**The Situation:**
Enterprise is building an internal AI platform to enable multiple data science teams. Needs managed orchestration, storage, experiment tracking, and compute — all in one place with enterprise-grade security and compliance.

**Nebius Solution:**
- Managed Kubernetes — production-ready, zero configuration
- Managed PostgreSQL — experiment metadata, model registry
- Container registry — internal model artifact management
- Integrated observability — GPU utilization, job health, alerting
- SOC 2 Type II + HIPAA + ISO 27001 compliance
- Tenant-level isolation + IAM for team access control

**ROI Metrics:**
- Reduce DevOps FTE allocation from 2–3 engineers to <0.5 FTE
- Centralize AI compute spend (eliminate shadow IT GPU purchases)
- Accelerate model experimentation cycles by 30–50%

**Reference Customer:**
JetBrains leverages Nebius AI Cloud infrastructure to power AI capabilities across developer tools for millions of developers globally.

**Qualification Signal:**
- Multiple data science teams needing shared infrastructure
- Struggling with Kubernetes management overhead
- Security/compliance review required (HIPAA or SOC 2 needed)

---

### Playbook 4: Healthcare / Regulated Industry AI

**Target Buyer:** Healthcare providers, pharma, biotech, financial services
**Champion:** Head of Data Science / AI
**Economic Buyer:** CTO, CIO, Compliance Officer

**The Situation:**
Organization wants to build AI models on sensitive data (patient records, clinical trials, financial data) and must ensure data never leaves compliant infrastructure.

**Nebius Solution:**
- HIPAA BAA available
- SOC 2 Type II + ISO 27001 certification
- GDPR compliance (EU data residency in Finland)
- Tenant-level isolation — no shared compute for sensitive data
- Privacy-focused architecture by default
- EU AI Act compliance for European healthcare customers

**ROI Metrics:**
- Avoid compliance breaches that carry $100K–$1.9M HIPAA penalties per violation
- Accelerate time-to-AI-production in regulated environments by months (vs. building private cloud)
- Reduce compliance overhead vs. managing own on-prem GPU cluster

**Qualification Signal:**
- HIPAA Business Associate Agreement required
- EU data residency non-negotiable
- Healthcare, pharma, financial services, legal verticals

---

### Playbook 5: AI Startup Scaling from Prototype to Production

**Target Buyer:** Series A–C AI startups
**Champion:** CTO / Co-Founder / Lead ML Engineer
**Economic Buyer:** CTO, CEO

**The Situation:**
Startup has proven their AI concept, is ready to scale training and inference, needs enterprise-grade infrastructure without enterprise procurement delays — and is cost-sensitive with investor scrutiny on burn rate.

**Nebius Solution:**
- Self-serve signup with free trial credits → zero procurement friction
- Pay-as-you-go (1-second billing increments) — no long-term commitment required
- Full-stack platform (no need to hire dedicated DevOps team)
- Scale from 1 GPU to 1,000+ GPUs as needed
- Nebius AI Studio for inference without dedicated inference infrastructure

**ROI Metrics:**
- Save 50–70% vs. AWS/GCP on GPU compute costs → extend runway
- Avoid 1–2 DevOps engineer hires with managed platform → $200K–$400K/year saved
- Launch production AI feature in days vs. weeks

**Reference Customer:**
Wubble (AI music platform) leveraged Nebius infrastructure and Kubernetes to build a scalable AI system for high-capacity inference, QLoRA adaptation, and faster audio analysis pipelines — reducing time-to-first-token and ensuring reliable performance.

**Qualification Signal:**
- Series A–C funding, active hiring of ML engineers
- AI is core product (not internal tooling)
- Budget-conscious: $10K–$200K/month cloud spend range

---

## 6. Objection-Handling Guides

### Objection 1: "We're already on AWS/Azure/GCP and it's too hard to switch."

**Acknowledge:** "Switching cloud providers is a real concern — migration risk, retraining teams, and re-architecting can be significant."

**Reframe:** "But consider what you're paying for that inertia. AWS GPU instances run 5–8x more per hour than Nebius for equivalent compute. For a team spending $500K/month on AWS GPU, that's $3–4M per year in avoidable costs. And we're not asking you to migrate everything at once."

**Bridge:** "Most customers start with new AI projects on Nebius while their existing workloads stay where they are. There's no rip-and-replace required. Our infrastructure uses standard Kubernetes and Slurm — your engineers don't need to learn new tools."

**Close:** "Would it make sense to run a parallel pilot on one upcoming training run and compare the cost and performance yourself?"

---

### Objection 2: "We've never heard of Nebius — how do I know you'll be around in 3 years?"

**Acknowledge:** "Brand trust is absolutely a fair consideration when choosing infrastructure that your AI products will depend on."

**Proof:** "Nebius has NVIDIA's $2 billion direct equity investment — the company that makes the GPUs we run on has bet $2 billion on us. We also have nearly $50 billion in contracted backlog from Meta and Microsoft. This isn't a startup hoping for customers — we're infrastructure that two of the world's largest AI companies depend on. And we have a $41 billion market cap with 27 analyst buy ratings."

**Human Angle:** "Our founding team built Yandex, one of Europe's largest internet companies. These are infrastructure engineers who have scaled systems to billions of users — they brought that expertise here."

**Close:** "Would a technical and financial due diligence session with our team give you the confidence to move to a pilot?"

---

### Objection 3: "CoreWeave is the established leader in AI cloud — why should I go with you?"

**Acknowledge:** "CoreWeave is a strong provider, especially for frontier AI labs doing massive training at scale."

**Differentiate:** "But CoreWeave is optimized for one thing: raw training scale. If you need managed Kubernetes, a production inference API, EU data residency, HIPAA compliance, or self-serve access without a lengthy enterprise sales process — Nebius has all of that. And our H100 rate is $2.10/hr vs. CoreWeave's $4.76/hr."

**Proof:** "CoreWeave's revenue is 62% dependent on one customer. Ours is diversified across thousands of customers, from Brave Search to JetBrains to enterprise healthcare companies. We're not optimized for one use case."

**Close:** "What's most important to you: maximum raw GPU scale for frontier training, or a full-stack platform with better economics and compliance support? That'll tell us which is the right fit."

---

### Objection 4: "Your pricing seems too cheap — what's the catch?"

**Acknowledge:** "That's a smart instinct. Cheap infrastructure with poor reliability will cost you more in failed training runs and engineer time than you save on hourly rates."

**Explain:** "Nebius achieves lower pricing because of vertical integration — we design our own servers, racks, and data centers. Removing the layers of middlemen and general-purpose overhead means we pass the savings on. We commissioned SemiAnalysis to independently model TCO across training, RL, and inference scenarios — Nebius had the lowest TCO in every single case."

**Add Credibility:** "Brave Search runs 11 million AI-powered queries daily on us at nearly 100% GPU utilization. That's not the behavior of a customer worried about reliability."

**Close:** "The best way to prove it is a pilot run. We'll give you trial credits — run one of your real workloads and compare performance and cost yourself."

---

### Objection 5: "We need to stay in the US — we can't use European infrastructure."

**Address Directly:** "We have US infrastructure — us-central1 region is live today. And we're building 300MW in Birmingham, Alabama and a 1,200MW campus in Missouri. The US is a core part of our infrastructure roadmap."

**Flip It:** "And actually, for customers with EU customers or GDPR requirements, our Finland data center is a differentiator. But if you're US-only, we have you covered."

---

### Objection 6: "We don't have the internal expertise to manage a new cloud platform."

**Acknowledge:** "It's true that changing infrastructure vendors requires some onboarding — and that takes time your team may not have."

**Reframe:** "But Nebius is specifically designed to reduce infrastructure management burden. Our managed Kubernetes, managed Slurm, and integrated observability mean your engineers don't need to configure clusters — they just submit jobs. We also provide dedicated onboarding engineering support in the first 30 days."

**Proof:** "Customers like Wubble and CentML were able to launch production AI systems on Nebius without a dedicated DevOps team."

**Close:** "Would a dedicated onboarding engineer working alongside your team for the first month change the equation for you?"

---

### Objection 7: "We're under a long-term contract with our current provider."

**Acknowledge:** "That's a real constraint, and we're not going to ask you to break contracts."

**Bridge:** "But contracts end, and budgets get reviewed. The best time to evaluate alternatives is before the renewal pressure hits. Let's talk about what your current contract covers, when it expires, and whether starting a smaller pilot on Nebius today would give you the leverage and data you need for your next negotiation."

**Close:** "When does your current contract come up for renewal?"

---

## 7. Competitive Positioning

### Core Positioning Statement

> **Nebius is the full-stack AI cloud built for teams who are serious about production — combining the lowest independently validated TCO, NVIDIA's latest hardware, and a complete software layer that eliminates DevOps overhead. Backed by NVIDIA's $2B investment and trusted by Meta, Microsoft, and Brave Search.**

---

### Differentiation Pillars

**Pillar 1: Lowest Total Cost of Ownership**
- Independent SemiAnalysis study: Nebius delivers lowest TCO across LLM pre-training, multimodal RL, and production inference
- H100 from $2.10/hr (vs. CoreWeave $4.76/hr, AWS $12–20+/hr)
- 1-second billing increments — no wasted spend
- Vertical integration: proprietary hardware design drives cost efficiency

**Pillar 2: Full-Stack, Not Just Compute**
- Managed Kubernetes + Slurm (pre-configured, production-ready)
- Managed PostgreSQL + container registry
- Integrated observability and monitoring
- Nebius AI Studio: inference-as-a-service for LLMs and image models
- This is what AWS/GCP would look like if they built it for AI from scratch

**Pillar 3: NVIDIA-First Architecture**
- NVIDIA Reference Platform Cloud Partner (highest NPN tier)
- $2B direct NVIDIA equity investment validates platform
- First to deploy Vera Rubin (NVL72) at scale
- GB200, GB300, HGX B200, HGX B300 available now
- Non-blocking InfiniBand fabric for maximum AllReduce throughput
- Maximized MFU — performance on par with leading benchmarks

**Pillar 4: Enterprise-Ready Compliance**
- HIPAA Business Associate Agreement available
- SOC 2 Type II certified
- GDPR compliant (EU data centers in Finland)
- ISO 27001 certified
- EU AI Act compliant
- Tenant-level isolation as standard

**Pillar 5: Developer-First Experience**
- Self-serve sign-up with free trial credits
- No enterprise intake form required (unlike CoreWeave)
- Ready to run within hours of provisioning
- Standard open-source tooling (no proprietary lock-in)
- Integrated with popular ML frameworks: PyTorch, Kubeflow, Weights & Biases, NCCL

---

### Proof Points Matrix

| Claim | Proof Point |
|---|---|
| Lowest TCO | SemiAnalysis independent study across 3 workload types |
| Production reliability | Brave Search: 11M+ daily AI answers at ~100% GPU utilization |
| Scale for enterprise | Meta ($27B), Microsoft ($19B+) contracted infrastructure |
| Developer trust | JetBrains, Recraft, CentML, Wubble, Prisma Labs |
| NVIDIA endorsement | $2B direct equity investment + Reference Platform Cloud Partner |
| Compliance | HIPAA BAA, SOC 2 Type II, ISO 27001, GDPR, EU AI Act |
| Speed to deploy | Hours from signup to running workloads |
| Hardware recency | First Vera Rubin NVL72 deployments in H2 2026 |

---

### One-Page Positioning vs. Each Competitor

**vs. AWS/Azure/GCP:** "Hyperscalers are built for everything — which means they're optimized for nothing. Nebius is built exclusively for AI. That's why we're 5–8x cheaper per GPU and provision in hours, not weeks."

**vs. CoreWeave:** "CoreWeave is the training-at-all-costs provider for frontier labs. Nebius is the full-stack AI cloud for companies building AI products — with better economics, EU compliance, developer-friendly access, and a managed software layer."

**vs. Lambda Labs:** "Lambda is a great starting point. Nebius is where you come when you're ready for production — enterprise SLAs, managed orchestration, compliance coverage, and an inference API."

**vs. On-Premise GPUs:** "Owning GPUs made sense before cloud GPU pricing came down. Today, Nebius delivers bare-metal performance in a managed cloud — without the capital cost, maintenance burden, or obsolescence risk of owned hardware."

---

## 8. Manager Coaching Tools

### Weekly Deal Review Framework

Use this for every active deal in the pipeline during 1:1s or team review sessions.

**Deal Health Check (5 Questions)**

1. **"Who is the economic buyer, and when did your AE last speak with them directly?"**
   - Green: Spoken to within 2 weeks; relationship active
   - Yellow: Identified but not yet directly engaged
   - Red: Unknown or only champion-level access

2. **"What is the prospect's stated #1 pain, and how has it been quantified?"**
   - Green: Specific, quantified pain (e.g., "$400K/month on AWS GPUs, want to cut 50%")
   - Yellow: General pain stated; not yet quantified
   - Red: No clear pain; deal is interest-only

3. **"What does the competitive landscape look like, and where does Nebius stand?"**
   - Green: Competition mapped; Nebius differentiation accepted by champion
   - Yellow: Competition known; positioning work in progress
   - Red: Competitor not identified; or prospect leaning toward competitor without Nebius countering

4. **"What is the next mutually agreed-upon step, and when is it scheduled?"**
   - Green: Specific next step, date confirmed, both sides committed
   - Yellow: Next step proposed but not confirmed
   - Red: "They'll get back to us" — no commitment

5. **"What compliance or legal requirements has the prospect shared, and are we cleared?"**
   - Green: Requirements known; SOC 2, HIPAA, GDPR confirmed as met
   - Yellow: Requirements known; legal review in progress
   - Red: Unknown — major risk if compliance is a gating factor

---

### Stage Gate Criteria

**Stage 1 → Stage 2 (Discovery → Qualification)**
- [ ] ICP confirmed (GPU spend >$50K/month or AI workload in production/near-production)
- [ ] Primary pain identified (cost, availability, compliance, DevOps burden)
- [ ] Champion identified and has access to economic buyer
- [ ] Evaluation timeline established

**Stage 2 → Stage 3 (Qualification → Technical Validation)**
- [ ] Economic buyer identified and engaged at least once
- [ ] Decision criteria documented; Nebius meets all must-haves
- [ ] Competitive landscape mapped
- [ ] Technical deep dive or demo scheduled
- [ ] MEDDPICC score ≥ 15

**Stage 3 → Stage 4 (Technical Validation → Proposal)**
- [ ] Technical validation complete (POC, benchmarks, or trial)
- [ ] Champion has presented Nebius internally
- [ ] Procurement / legal process understood
- [ ] Commercial scope (GPU count, services, term) aligned
- [ ] No unresolved compliance objections

**Stage 4 → Stage 5 (Proposal → Closed Won)**
- [ ] Proposal sent; verbal commitment received
- [ ] Economic buyer approved
- [ ] Legal / security review complete (SOC 2 / HIPAA / ISO 27001 accepted)
- [ ] MSA and Order Form in final negotiation
- [ ] Signed contract received

---

### Coaching Questions by Scenario

**Scenario A: Deal Stuck in Discovery (>30 days)**
- "Has the prospect verbally confirmed this is a priority project? Or is this exploratory?"
- "Who was the last executive-level touchpoint — and was there urgency?"
- "Is there a real budget allocated, or is this a 'maybe someday' evaluation?"
- *Action: Consider multi-threading; have AE request introduction to VP/CTO.*

**Scenario B: Prospect Stalling Before Technical Validation**
- "What is the stated reason for not scheduling the deep dive or POC?"
- "Is this an internal bandwidth issue, or are they evaluating another provider in parallel?"
- "Have we offered trial credits to lower the barrier to a real test?"
- *Action: Send free credit activation link + onboarding engineer introduction to remove friction.*

**Scenario C: Losing to CoreWeave**
- "Has the AE positioned our EU compliance and full-stack vs. CoreWeave's compute-only message?"
- "Has TCO been modeled and presented? ($2.10/hr vs. $4.76/hr, with SemiAnalysis study referenced)"
- "Has the champion been armed with the competitive battle card?"
- *Action: Set up a competitive technical session with Solutions Engineering.*

**Scenario D: Losing to Hyperscaler (Status Quo)**
- "Has the prospect quantified what they're overpaying vs. Nebius?"
- "Have we offered to run a cost modeling exercise using their actual workloads?"
- "Is there an upcoming renewal or budget review that creates a natural change moment?"
- *Action: Commission joint TCO analysis; involve Solutions Engineering for data-driven comparison.*

---

### AE Skill Coaching Checklist

Rate each AE 1–5 on the following Nebius-specific sales competencies:

| Competency | 1 (Needs Work) | 3 (Developing) | 5 (Expert) |
|---|---|---|---|
| **AI Infrastructure Knowledge** | Can't explain MFU or InfiniBand | Explains training vs. inference | Can discuss NVIDIA hardware architecture, Blackwell vs. Hopper differences |
| **TCO Discovery** | Doesn't ask about current GPU spend | Asks spend; can't model savings | Proactively models TCO comparison using prospect's actual workload data |
| **Compliance Navigation** | Unaware of HIPAA/GDPR requirements | Knows which certs Nebius has | Proactively raises compliance in discovery; guides procurement |
| **Competitive Selling** | Generic responses to CoreWeave | Can articulate 2–3 differentiators | Can handle any CoreWeave/AWS objection with data; arms champion |
| **Champion Development** | Single-threaded at engineer level | Champion identified; not tested | Champion actively advocates internally; AE has coached their narrative |
| **Multi-Threading** | Only one contact in account | 2–3 contacts across functions | Economic buyer + champion + technical contact all engaged |

---

### Monthly Pipeline Health Dashboard (Manager Template)

Track these metrics for the team each month:

| Metric | Target | Status |
|---|---|---|
| Average MEDDPICC score (active deals) | ≥ 16 | |
| % of deals with confirmed economic buyer | ≥ 70% | |
| % of deals with active POC / trial credits activated | ≥ 50% of Stage 3+ | |
| Win rate vs. CoreWeave | ≥ 40% | |
| Win rate vs. hyperscalers | ≥ 55% | |
| Average deal cycle (days) | < 60 days for <$100K ACV | |
| Deals stalled >45 days with no next step | 0 | |
| % of ICP-qualified pipeline | ≥ 80% | |

---

*© Nebius Sales Enablement | Confidential — For Internal Use Only*
*Last Updated: April 2026*
