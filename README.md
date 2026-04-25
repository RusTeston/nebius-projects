# Nebius Technical Sales Enablement Projects

**Technical Sales Enablement Portfolio for Nebius AI Cloud**  
**Project Start**: April 13, 2026  
**Latest Updates**: April 20, 2026  
**Status**: ✅ LIVE - 10 PROJECTS OPERATIONAL - CI/CD ENABLED - TOKEN FACTORY INTEGRATED

---

## 🎯 Project Overview

A comprehensive portfolio of technical sales enablement tools built for Nebius AI Cloud, demonstrating expertise in revenue enablement program design, competitive intelligence, partner enablement frameworks, and AI infrastructure knowledge. All content is MVP sample ideas created for demonstration purposes using publicly available information.

**Live Site**: https://nebius.rus-teston.com

---

## 📁 Project Structure

### **Landing & Navigation**
- `index.html` — Disclaimer/splash gate page (entry point)
- `projects.html` — Main project landing page with all 10 cards
- `nebius_logo.png` — Nebius brand logo

### **Project 01 — Learning Path Dashboard**
- Role-based enablement learning paths for SA, AE, and Partner audiences
- 3 tracks, 27 modules, 12-week ramp target, 3 certification gates
- Interactive filter bar, expandable module cards

### **Project 02 — AE Technical Cheat Sheet**
- GPU tiers, workload decoder, discovery questions, objection responses
- Click-to-expand modal for readable detail view
- Color-coded sections by deal moment

### **Project 03 — SA 90-Day Onboarding Blueprint**
- Week-by-week program with 12 expandable week cards
- Interactive timeline with clickable week bubbles
- Manager coaching strips, certification gates, stakeholder map
- Sidebar: milestones, deliverables checklist, environment setup

### **Project 04 — Enablement Metrics Dashboard**
- KPI cards, ramp time trends, competency scores
- Adoption funnel with watch items, module NPS scores
- Revenue correlation panel with cohort comparison
- Content iteration log with trigger types

### **Project 05 — Partner Enablement Framework**
- 4-stage partner maturity lifecycle (Onboarded → Expert)
- Partner type matrix (VAR, ISV/MSP, Alliance)
- Four core pillars, independence metrics, key resources

### **Project 06 — Solutions Architect Battle Card**
- 4 competitor tabs: CoreWeave, Lambda Labs, Crusoe Cloud, RunPod
- Each tab: Tech Spec Gaps, Implementation Risk, Architectural Traps, Technical Rebuttals, Integration Playbook, Discovery Questions
- Color-coded risk levels, FUD/Rebuttal pairs, migration playbooks

### **Project 07 — AI Infrastructure Glossary**
- 50+ terms across 7 domain categories
- Live search with text highlighting, category filtering
- Color-coded sections, Learn More links

### **Project 08 — Enablement Key Performance Indicators (KPIs)**
- 25 KPIs across 5 categories
- Expandable cards with formula, data source, thresholds, accountability
- Business purpose banners, action plans for red metrics
- Sticky navigation, implementation phasing guide

### **Project 09 — Quick Competitive Positioning**
- 9 differentiators compared across 6 competitors
- Color-coded Strong/Partial/Weak indicators
- Positioning takeaway summary

### **Project 10 — Token Factory**
- A-Z AI & infrastructure glossary with 134+ terms
- Live search, A-Z letter navigation, red letter badges
- **Live Token Factory Integration**: DeepSeek V3.2 inference via Nebius Token Factory API
- Architecture: Browser → AWS Lambda → Nebius Token Factory API

---

## 🏗️ Infrastructure

**AWS Services:**
- **S3 Bucket**: `nebius-projects`
- **Region**: `us-east-1`
- **CloudFront Distribution**: `E3K7BNEXGNYAIR` (`d1e4e48fwamqee.cloudfront.net`)
- **Custom Domain**: `https://nebius.rus-teston.com`
- **ACM Certificate**: Covering `nebius.rus-teston.com` (TLS 1.2+, SNI)
- **DNS**: Route 53 alias record in `rus-teston.com` hosted zone
- **Lambda**: `nebius-token-factory-proxy` (Token Factory API proxy)
- **CloudFront Logging**: `rus-teston-cloudfront-logs` S3 bucket

**Nebius Integration:**
- **Token Factory API**: DeepSeek V3.2 model inference
- **Lambda Function URL**: Proxies browser requests to Token Factory
- **CORS**: Locked to `https://nebius.rus-teston.com`

**CI/CD Pipeline:**
- **GitHub Repo**: `github.com/RusTeston/nebius-projects` (public)
- **GitHub Actions**: Auto-deploy on push to main branch
- **OIDC Federation**: Secure AWS authentication (no stored credentials)
- **IAM Role**: `GitHubActions-Deploy` with least-privilege permissions
- **CloudFront Invalidation**: Automatic cache invalidation after each deploy

**Design System:**
- Navy gradient background (`#0C1A3A` → `#0A3050` → `#0E3558`)
- Inter font family throughout
- Nebius Canary brand color (`#E0FF4F`) for logo/branding
- Nebius green (`#00C853`) for accents
- Hover scale + glow effects on interactive elements
- Click-to-expand modals for detailed content
- Disclaimer splash gate with 7-day cookie

---

## 🚀 Deployment

**Manual Deploy:**
```bash
# Upload all files to S3
aws s3 sync . s3://nebius-projects --exclude ".git/*" --exclude ".github/*" --exclude ".gitignore" --exclude "*.md" --exclude "*.docx" --exclude "*.pdf"

# Invalidate CloudFront
aws cloudfront create-invalidation --distribution-id E3K7BNEXGNYAIR --paths "/*"
```

**CI/CD Deploy:**
Push to `main` branch → GitHub Actions automatically syncs to S3 and invalidates CloudFront.

---

## 📋 Technical Details

**Technology Stack:**
- Pure HTML/CSS/JavaScript (no frameworks)
- Self-contained single-file pages
- AWS S3 static hosting + CloudFront CDN
- Lambda (Python 3.12) for Token Factory proxy
- Nebius Token Factory API (DeepSeek V3.2)

**Monthly Cost:** ~$1-2 (S3 + CloudFront + Route 53 + Lambda)

---

## 🎊 Project Status

**ALL 10 PROJECTS LIVE** ✅  
**Website**: https://nebius.rus-teston.com  
**Splash Gate**: Disclaimer acknowledgment with 7-day cookie  
**Token Factory**: Live inference via DeepSeek V3.2  
**CI/CD**: GitHub Actions auto-deploy on push  
**Visitor Tracking**: CloudFront access logging enabled  

**Integration with rus-teston.com:**
- Nebius badge added to certification grid on homepage
- Links to `nebius.rus-teston.com` splash gate

---

*This project demonstrates comprehensive expertise in technical sales enablement, competitive intelligence, AI infrastructure knowledge, and hands-on integration with Nebius AI Cloud services.*
