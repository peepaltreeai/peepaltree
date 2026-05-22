# Peepal Tree Advisory — Project Bible
**Last updated:** May 2026 — v1.1  
**Purpose:** Single source of truth for all Claude sessions. Paste this at the start of any new session before requesting edits or additions.

### Changelog
- v1.1: CNAME file removed (not needed on Vercel). Next.js deferred — not needed for MVP. Netlify dropped in favour of Vercel. GitHub username confirmed: `parshantstack`. Repo: `peepal-tree`.

---

## 1. Company Overview

| Field | Detail |
|---|---|
| **Legal Name** | Peepal Tree Advisory Pvt. Ltd. |
| **Type** | Full-stack Indian financial services firm |
| **Positioning** | India's AI-native, multi-license wealth and credit platform |
| **Tagline** | *Where deep roots meet intelligent capital.* |
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
--forest:       #0D3322   (primary dark green — dominant brand colour)
--forest-mid:   #1A5C3E   (hover states, secondary dark)
--forest-light: #2E8B57   (accents)
--leaf:         #3DAA6F   (section tags, highlights)
--leaf-pale:    #E8F5EE   (light tints, hover backgrounds)
--gold:         #C9922A   (CTA buttons, accents)
--gold-mid:     #E5AE4A   (hero numbers, nav CTA, links on dark)
--ink:          #111827   (body text)
--slate:        #4B5563   (secondary text)
--muted:        #9CA3AF   (labels, placeholders)
--bg:           #F9FAF8   (light section background)
--bg2:          #F2F4F0   (alternate light background)
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
| 1 | Hero | Dark (forest) | Identity — who we are |
| — | License Strip | White | Trust signal — regulatory proof |
| 2 | Services | Light (bg) | Functional — what we offer |
| 3 | Why Us | Dark (forest) | Philosophy — why we're different |
| 4 | Who We Serve | Light (bg2) | Functional — self-qualification |
| 5 | Contact | Dark (forest) | Personal, committed — close on identity |
| — | Footer + Disclaimer | Dark (forest) | Continuous with contact |

**Rule:** Dark sections = identity/philosophy. Light sections = functional/informational. Do not break this rhythm without good reason.

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

### GitHub → Vercel Pipeline
```
Edit code locally
    ↓
git add . && git commit -m "description of change"
    ↓
git push origin main
    ↓
Vercel auto-deploys in ~30 seconds
    ↓
Live at: https://peepal-tree.vercel.app
         (later: https://peepaltree.in)
```

### GitHub repo (confirmed)
```
https://github.com/parshantstack/peepal-tree
```

### Git add tip
Use `git add .` to stage all files at once — no need to list filenames individually.
Only be careful if the folder has unrelated files. Best practice: keep all site files in a dedicated folder `C:\Users\sheor\Projects\peepal-tree\`.

### Current live URL
```
https://peepal-tree.vercel.app   (update once Vercel deployment confirmed)
```

### Domain setup (when ready)
1. Buy `peepaltree.in` from Namecheap or BigRock
2. In Vercel → Project → Settings → Domains → add `peepaltree.in`
3. Set nameservers to: `ns1.vercel-dns.com` / `ns2.vercel-dns.com`
4. Vercel auto-provisions SSL certificate
5. Add `www.peepaltree.in` → Vercel redirects to root automatically
6. Set up `connect@peepaltree.in` email via Cloudflare Email Routing (free)

---

## 11. Form Setup (Action Required)

The contact form currently has a placeholder ID. To activate:

**Option A — Formspree (current code)**
1. Sign up at formspree.io (free, 50 submissions/month)
2. Create new form → copy endpoint ID
3. In `index.html`, replace `YOUR_FORMSPREE_ID` with actual ID
4. Form submissions email to your inbox

**Option B — Web3Forms (recommended upgrade)**
1. Sign up at web3forms.com (free, 250 submissions/month)
2. Get access key
3. Change form action to `https://api.web3forms.com/submit`
4. Add `<input type="hidden" name="access_key" value="YOUR_KEY">`
5. No JS needed — works as plain HTML POST

**Option C — Netlify Forms (if switching to Netlify)**
1. Add `data-netlify="true"` to `<form>` tag
2. Add `<input type="hidden" name="form-name" value="contact">`
3. Remove Formspree action and JS fetch entirely

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

- [x] MVP `index.html` built and downloaded
- [x] Project bible created
- [x] GitHub repo created → `github.com/parshantstack/peepal-tree`
- [x] Hosting decision made → Vercel (not Netlify)
- [x] Next.js deferred — not needed for MVP
- [x] CNAME file dropped — not needed on Vercel
- [ ] Move files to dedicated folder `C:\Users\sheor\Projects\peepal-tree\`
- [ ] Run git commands to push `index.html` and bible to GitHub
- [ ] Connect GitHub repo to Vercel → get `.vercel.app` live URL
- [ ] Activate contact form — replace `YOUR_FORMSPREE_ID` (or switch to Web3Forms)
- [ ] Buy domain `peepaltree.in` (Namecheap or BigRock)
- [ ] Connect domain to Vercel via nameservers
- [ ] Set up `connect@peepaltree.in` via Cloudflare Email Routing
- [ ] Add real phone number to contact section in `index.html`
- [ ] Add favicon (peepal leaf — 32×32 SVG/PNG)
- [ ] Legal review of disclaimer text

---

## 15. How to Use This Bible in Future Claude Sessions

Paste this entire document at the start of your message, then describe what you want changed. Example prompts:

> *"[paste bible] Add a FAQ section after Who We Serve. Keep the light background. Questions should be about PMS minimum investment, LAS eligibility, and how research is delivered."*

> *"[paste bible] The hero tagline feels too abstract. Give me 3 alternative options that are more specific to the multi-license angle."*

> *"[paste bible] We're ready to add a fifth service — IPO Financing. Add it as service card 05 with the NBFC license tag. Timeline: Q2 Year 1."*

> *"[paste bible] Create a second page — about.html — for the team section. Same design system. Three founding team members, placeholder bios."*

