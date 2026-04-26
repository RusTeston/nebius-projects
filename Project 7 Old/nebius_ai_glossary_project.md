# Nebius AI Infrastructure Glossary — Web Conversion Project

## Project Overview

This project involved converting a structured Word document (`.docx`) containing a comprehensive AI infrastructure glossary into a production-grade, enterprise-ready HTML web page. The deliverable is a single, self-contained HTML file with no external build dependencies — ready to deploy as a static page on any web host.

---

## Source Document

**File:** `Nebius_AI_Infrastructure_Glossary.docx`  
**Content:** A multi-table glossary covering 50+ AI infrastructure terms across 7 domain categories, with definitions, real-world analogies, business impact summaries, and authoritative "Learn More" links for each entry.

---

## What Was Built

### `nebius_ai_glossary.html`

A fully interactive, enterprise-grade reference page featuring:

- **50+ defined terms** across 7 domain sections
- **Live search** — filters all rows in real time as the user types
- **Category filtering** — one-click filters for each domain area (Hardware, ML Core, Distributed, Networking, Infrastructure, Data, DevOps)
- **Search term highlighting** — matched text is visually highlighted in yellow across all visible cells
- **Results counter** — live count of matching terms displayed in the control bar
- **"Learn More" links** — every term links directly to the authoritative external source cited in the original document
- **Responsive layout** — table columns collapse gracefully on tablet and mobile viewports
- **Sticky header + controls bar** — always accessible while scrolling through the glossary

---

## Technical Stack

| Layer | Choice | Rationale |
|---|---|---|
| Markup | Semantic HTML5 | Accessibility, SEO, maintainability |
| Styling | Vanilla CSS with custom properties | Zero dependencies, fast load, full control |
| Typography | DM Serif Display + DM Mono + Inter (Google Fonts) | Professional, distinctive, non-generic |
| Interactivity | Vanilla JavaScript (ES6+) | No framework overhead for a static reference page |
| Hosting | Static file — any CDN or web server | Maximum portability |

---

## Design System

### Color Palette

| Token | Hex | Usage |
|---|---|---|
| `--ink` | `#0d0f14` | Primary text, header, footer |
| `--bg` | `#f7f6f2` | Page background (warm off-white) |
| `--bg-warm` | `#eeeae0` | Controls bar, table headers |
| `--accent` | `#1a3cff` | Links, focus rings, search highlights |
| `--accent-2` | `#ff4d1c` | Logo dot, hero eyebrow text |

### Category Color Coding

Each of the 7 domain areas has a dedicated accent color applied to its section badge, row badge, and active filter button:

| Domain | Color |
|---|---|
| Hardware & Compute | `#1a3cff` (Electric Blue) |
| AI & ML Core | `#7c3aed` (Violet) |
| Distributed Training | `#0891b2` (Cyan) |
| Networking | `#dc2626` (Red) |
| Infrastructure & Cloud | `#d97706` (Amber) |
| Data & Storage | `#059669` (Emerald) |
| DevOps & Operations | `#4338ca` (Indigo) |

### Typography

- **Display / Headings:** DM Serif Display — elegant serif with italic variant for contrast
- **Monospace:** DM Mono — used for term names, badges, counters, and the logo wordmark
- **Body:** Inter (300–600 weights) — highly readable at small sizes

---

## Content Integrity

All content from the source Word document has been faithfully preserved, including:

- Every term name and full definition
- Every analogy (displayed in italics with a labeled callout)
- Every "Why It Matters" paragraph
- Every "Learn More" hyperlink, linked to the exact URL from the original document
- All 7 section headings and their groupings

No terms were added, removed, or summarized beyond what appeared in the source document.

---

## Sections Covered

1. **Hardware & Compute** — GPU, CPU, GPU Cluster, Node, GPU Instance *(5 terms)*
2. **AI & Machine Learning Core** — Inference, Training, Fine-Tuning, LLM, Transformer, Token, RAG, Epoch, Batch, Gradient, Optimizer, Hyperparameters, Checkpoint, Quantization, KV Cache, Tokenization, Dataset, Benchmark *(18 terms)*
3. **Distributed Training & Frameworks** — Distributed Training, PyTorch, TensorFlow, JAX, MLflow, JupyterLab *(6 terms)*
4. **Networking & Performance** — InfiniBand, Latency, Throughput, Bandwidth *(4 terms)*
5. **Infrastructure & Cloud** — Kubernetes, Container, Serverless, Terraform, IAM, Autoscaling, Cold Start, Provisioning *(8 terms)*
6. **Data & Storage** — Object Storage, S3, PostgreSQL, Apache Spark, Data Pipeline, Storage Throughput *(6 terms)*
7. **DevOps & Operations** — Slurm, API, CLI, Orchestration, Scheduling, GPU Utilization, Observability, Logging, Benchmark *(9 terms)*

---

## Skills Demonstrated

This project showcases competency in:

- **Technical content design** — transforming dense structured content into a scannable, navigable reference
- **Enterprise UI/UX** — sticky navigation, live search, visual hierarchy, and responsive design without a framework
- **Design systems thinking** — consistent tokens, color semantics, typographic scale
- **Information architecture** — multi-axis filtering (category + free text) with live feedback
- **Attention to data fidelity** — 100% content preservation across a complex, multi-table source document
- **Static web performance** — single self-contained file, no build step, fast cold load

---

## How to Use

1. Open `nebius_ai_glossary.html` in any modern browser
2. Use the **search bar** to filter by keyword across all terms, definitions, and analogies
3. Use the **category buttons** to narrow by domain area
4. Click any **↗ Learn More** link to open the authoritative external reference
5. Deploy as a static file to any web host, CDN, or GitHub Pages — no server required

---

*Project by: [Your Name] · Converted from Word document · Designed for enterprise portfolio presentation*
