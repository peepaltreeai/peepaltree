# Peepal Tree Advisory — Project Bible
**Last updated:** May 2026 — v1.3  
**Purpose:** Single source of truth for all Claude sessions. Paste this at the start of any new session before requesting edits or additions.

### Changelog
- v1.0: Initial bible created
- v1.1: CNAME file removed. Next.js deferred. Netlify dropped in favour of Vercel. GitHub username confirmed: `parshantstack`. Repo: `peepal-tree`.
- v1.2: Site live at `https://peepal-tree.vercel.app`. Web3Forms contact form activated. Primary email `parshant.aiops@gmail.com`, CC `el.shankaro@googlemail.com`. PowerShell note added (use `;` not `&&`).
- v1.3: Full "Indian Precision" redesign applied. Key changes: hero rebuilt with single bold H1 ("Intelligent capital. Exceptional outcomes."), stats moved to bottom row (HRT style). Pure white + pure forest green backgrounds only — bg2 (#F2F4F0) removed. Service card grid lines removed, white space only. Nav letter-spacing increased, CTA shortened to "Connect". Gold replaced with cooler amber (#C8A96E). Logo rebuilt with correct peepal leaf geometry. Overclaiming subheading removed from Why Us. Contact section left column (placeholder details) removed — form is full width. Geographic anchoring removed from hero copy. "Schedule a Call" changed to "Get in Touch".

---

## 1. Company Overview

| Field | Detail |
|---|---|
| **Legal Name** | Peepal Tree Advisory Pvt. Ltd. |
| **Type** | Full-stack Indian financial services firm |
| **Positioning** | AI-native, multi-license wealth and credit platform |
| **Tagline** | *Intelligent capital. Exceptional outcomes.* |
| **Stage** | Operational — MVP website live, domain pending |
| **Location** | Mumbai, India |
| **Founded** | Active as of May 2026 |

---

## 2. Licenses & Regulatory Status

All five licenses are live and SEBI/RBI registered:

| License | Regulator | Notes |
|---|---|---|
| Research Analyst (RA) | SEBI | Powers advisory and research products |
| Portfolio Manager (PMS) | SEBI | Discretionary PMS, min ₹50L |
| Stock Broker | SEBI | Equity + F&O execution |
| Depository Participant (DP) | SEBI | Custody of client assets |
| NBFC | RBI | Lending — Loan Against Securities |

**Key credibility stat:** ₹1,300 Cr assets in custody, 1,000+ HNI clients.

---

## 3. Current Products (Live / MVP)

These four are the only services on the MVP website. Do not add future products to the site without explicit instruction.

### 01 — Research & Advisory (RA license)
- AI-powered equity research, institutional rigour at HNI-accessible pricing
- Sector deep-dives, model portfolios, live alerts
- Tags: Equity Research, Model Portfolios, Sector Coverage, AI Screening

### 02 — Portfolio Management (PMS license)
- Discretionary PMS for HNIs
- Quant-driven factor strategies + fundamental conviction
- Minimum investment: ₹50L
- Tags: Discretionary PMS, Quant Strategies, Min ₹50L, Real-time Reporting

### 03 — Loan Against Securities (NBFC license)
- Liquidity against equity, MF units, bonds held in DP account
- Digital drawdown, no prepayment fee
- Tags: LAS, Equity & MF Collateral, Digital Drawdown, No Prepayment Fee

### 04 — Broking & Execution (Broker + DP license)
- Full-service broking with dealer support
- Equity, F&O, IPO access
- Tags: Equity & F&O, IPO Access, Dealer Support, DP Custody

---

## 4. Future Products (NOT on website yet — roadmap only)

Do not surface these on the website until instructed:

| Product | License Required | Timeline |
|---|---|---|
| Algo Strategy Marketplace | RA + Broker | Year 2 |
| Fixed Income + Alt Assets | Broker + DP | Year 2 |
| NRI PMS (GIFT City) | PMS | Year 2–3 |
| IPO Financing | NBFC | Q2 Year 1 |
| Educational Content Hub | Brand | Q2 Year 1 |

---

## 5. Target Client Segments

| Segment | Description |
|---|---|
| **Retail Investors** | 120M+ demat accounts in India, Tier 2/3 fastest-growing. Active investors wanting regulated research + smart execution. |
| **HNIs & Families** | ₹50L+ investable assets. Want discretionary PMS, dedicated RM, and LAS facility. Existing base: 1,000+ clients. |
| **NRIs & Diaspora** | Indians in UK, US, UAE, Singapore. Want FEMA-compliant India equity access with premium service. |

---

## 6. Brand & Design System

### Colour Palette
```
--forest:      #0D3322   (primary dark green — dominant brand colour)
--forest-mid:  #1A5C3E   (hover states, secondary dark)
--leaf:        #3DAA6F   (section tags, license badges)
--leaf-pale:   #E8F5EE   (service tag backgrounds)
--amber:       #C8A96E   (cooler accent — replaces old gold, used throughout)
--amber-bright:#E5AE4A   (hero numbers, nav CTA, links on dark only)
--ink:         #111827   (body text)
--slate:       #4B5563   (secondary text, descriptions)
--muted:       #9CA3AF   (labels, placeholders)
--bg:          #FFFFFF   (pure white — only light background used)
NOTE: --bg2 (#F2F4F0) removed entirely. Only pure white and pure forest green.
```

### Typography
```
--serif:  'Cormorant Garamond' — headings, hero, section H2s, numbers
--sans:   'Outfit'             — body text, descriptions, UI copy
--mono:   'DM Mono'            — labels, tags, nav links, badges, form labels
```

### Type Scale
- Hero H1: clamp(2.8rem, 5vw, 4.8rem), serif, weight 700
- Section H2: clamp(1.9rem, 3.5vw, 3rem), serif, weight 700
- Section tag: 0.62rem, mono, uppercase, letter-spacing 0.2em, colour: var(--leaf)
- Body: 0.92–1rem, sans, weight 300
- Labels/tags: 0.58–0.68rem, mono, uppercase

### Logo
SVG peepal leaf with trunk and roots. Leaf fill: #2E8B57. Gold accent dot at drip-tip: #E5AE4A. Trunk/roots: #5D8A72. Used in nav (26×26px) and favicon (to be created).

### Design Principles
- Flat, no gradients or drop shadows
- Sharp corners (no border-radius on cards and buttons — brand choice)
- Thin borders: 1px or 1.5px, never thick
- Generous whitespace
- Professional, not flashy — trust over excitement

---

## 7. Section Structure & Rhythm (Important)

The page alternates dark/light with *intentional meaning*, not decoration:

| # | Section | Background | Semantic purpose |
|---|---|---|---|
| 1 | Hero | Dark (forest) | Identity — bold declarative statement, stats row at bottom |
| — | License Strip | White | Trust signal — regulatory proof |
| 2 | Services | White | Functional — what we offer, no grid lines, white space only |
| 3 | Why Us | Dark (forest) | Edge — three differentiators, no subheading claim |
| 4 | Who We Serve | White | Functional — self-qualification |
| 5 | Contact | Dark (forest) | Action — full-width form only, no placeholder details |
| — | Footer + Disclaimer | Dark (forest) | Continuous with contact |

**Rules:**
- Dark sections = identity/philosophy/action
- White sections = functional/informational
- No mid-grey backgrounds ever
- No visible grid lines between cards — white space only
- Contact section: form is full width, no contact details until domain/phone are real

---

## 8. Navigation

```
Logo (left) | Services · Our Edge · Who We Serve · Contact (centre) | Connect With Us CTA (right)
```

- Nav background: rgba(13,51,34,0.97) with backdrop-filter blur
- Active link: gold-mid colour
- CTA button: gold-mid text, gold-mid border, hover fills with subtle gold tint
- Mobile: nav links hidden, only logo + CTA shown

---

## 9. Tech Stack

### Current (MVP) — confirmed stack
| Layer | Choice | Notes |
|---|---|---|
| Site | Single `index.html` | Pure HTML/CSS/JS, no framework needed yet |
| Hosting | **Vercel** | Free tier, auto-deploy from GitHub. Netlify considered and dropped. |
| Forms | Web3Forms or Formspree | Replace `YOUR_FORMSPREE_ID` in form action before going live |
| Version control | **GitHub** | Username: `parshantstack` · Repo: `peepal-tree` |
| Domain | Pending | `peepaltree.in` — to be purchased (Namecheap or BigRock) |
| Email | Pending | `connect@peepaltree.in` via Cloudflare Email Routing → forwards to existing inbox |
| CNAME file | **Not needed** | Vercel handles domain via dashboard UI — no file required in repo |
| Next.js | **Deferred** | Not needed until: client login, 100+ pages, or live database required |

### When to upgrade to Next.js (triggers)
| Trigger | What to add |
|---|---|
| Client login / portal | Next.js + Clerk auth |
| Research library (100+ pages) | Next.js with static generation |
| Live portfolio data | Next.js + Supabase |
| Transactional emails / CRM | Resend API |

---

## 10. Deployment Setup

### GitHub → Vercel pipeline
```
Edit index.html in VS Code
    ↓
git add .
git commit -m "describe what changed"
git push
    ↓
Vercel auto-deploys in ~30 seconds
    ↓
Live at: https://peepal-tree.vercel.app
         (later: https://peepaltree.in)
```

### PowerShell note (important)
VS Code terminal runs PowerShell on Windows. Use `;` not `&&` to chain commands:
```powershell
git add . ; git commit -m "your message" ; git push
```
`&&` throws a parser error in PowerShell — use `;` or run commands one per line.

### GitHub repo (confirmed)
```
https://github.com/parshantstack/peepal-tree
```

### Live URL (confirmed)
```
https://peepal-tree.vercel.app
```

### Future URL (when domain ready)
```
https://peepaltree.in
```

### Domain setup (when ready)
1. Buy `peepaltree.in` from Namecheap or BigRock
2. In Vercel → Project → Settings → Domains → add `peepaltree.in`
3. Set nameservers to: `ns1.vercel-dns.com` / `ns2.vercel-dns.com`
4. Vercel auto-provisions SSL certificate
5. Add `www.peepaltree.in` → Vercel redirects to root automatically
6. Set up `connect@peepaltree.in` email via Cloudflare Email Routing (free)

---

## 11. Form Setup — ACTIVE ✓

Contact form is live via Web3Forms.

| Field | Value |
|---|---|
| Provider | Web3Forms (free, 250 submissions/month) |
| Access key | `d07bf69b-2863-4fb3-ab31-f9bc475f73e7` |
| Primary email | `parshant.aiops@gmail.com` (registered account) |
| CC email | `el.shankaro@googlemail.com` (Uma) |
| Subject line | "New enquiry — Peepal Tree Advisory" |
| From name | "Peepal Tree Website" |

No changes needed unless switching provider or adding more recipients.

---

## 12. Content Rules (for Claude sessions)

### What to include on the website
- Current 4 services only
- SEBI/RBI license references on every service card
- Trust numbers: 1,000+ HNI clients, ₹1,300 Cr custody, 5 licenses
- Regulatory disclaimer in footer (mandatory for SEBI-registered entities)
- Contact form + email + phone + location

### What NOT to include
- Revenue projections (₹226 Cr, ₹86 Cr EBITDA) — investor deck only
- IPO / valuation roadmap — premature, confidential
- Year 2–3 products — not live yet
- CAC tables, market sizing data — internal strategy
- Any claim that cannot be substantiated publicly

### Tone of voice
- Professional, not salesy
- Confident, not boastful
- Specific over vague ("₹1,300 Cr in custody" not "significant assets")
- Plain English — no jargon the client doesn't already know
- Serif headings carry authority; mono labels carry precision

---

## 13. Legal / Compliance Notes

- Regulatory disclaimer must appear on every page (currently in footer)
- All service descriptions must not constitute investment advice
- "SEBI Registered" must appear alongside RA and PMS references
- NRI content must reference FEMA compliance
- No performance claims or return guarantees anywhere on the site
- Standard disclaimer text (do not modify without legal review):
  > *"Peepal Tree Advisory Pvt. Ltd. is registered with SEBI as a Research Analyst and Portfolio Manager, and with RBI as an NBFC. Investments are subject to market risk. Past performance is not indicative of future results. This website is for informational purposes only and does not constitute an offer, solicitation, or investment advice. Please read all scheme-related documents carefully before investing."*

---

## 14. Pending Actions Checklist

- [x] MVP `index.html` built
- [x] Project bible created
- [x] GitHub repo → `github.com/parshantstack/peepal-tree`
- [x] Vercel connected → `https://peepal-tree.vercel.app`
- [x] Web3Forms contact form activated
- [x] CC email added (el.shankaro@googlemail.com)
- [x] Indian Precision redesign applied (v1.3)
- [x] Logo rebuilt with correct peepal leaf geometry
- [x] Hero copy finalised — no geographic anchoring
- [x] Contact section cleaned — form full width, no placeholders
- [ ] Add real phone number (update contact section when ready)
- [ ] Buy domain `peepaltree.in` (Namecheap or BigRock)
- [ ] Connect domain to Vercel via nameservers
- [ ] Set up `connect@peepaltree.in` via Cloudflare Email Routing
- [ ] Add favicon (peepal leaf — 32×32)
- [ ] Legal review of disclaimer text
- [ ] Push bible v1.3 to GitHub repo

---

## 15. How to Use This Bible in Future Claude Sessions

Paste this entire document at the start of your message, then describe what you want changed. Example prompts:

> *"[paste bible] Add a FAQ section after Who We Serve. Keep the light background. Questions should be about PMS minimum investment, LAS eligibility, and how research is delivered."*

> *"[paste bible] The hero tagline feels too abstract. Give me 3 alternative options that are more specific to the multi-license angle."*

> *"[paste bible] We're ready to add a fifth service — IPO Financing. Add it as service card 05 with the NBFC license tag. Timeline: Q2 Year 1."*

> *"[paste bible] Create a second page — about.html — for the team section. Same design system. Three founding team members, placeholder bios."*

