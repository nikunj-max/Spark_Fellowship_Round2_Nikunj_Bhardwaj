# 🌉 FoodBridge India By Nikunj Bhardwaj
### Spark Fellowship Round 2 Submission — Build a Business Solution to Reduce Food Waste in Urban India

> **"Don't Let It Rot. Let It Reach."**  
> Surplus food, matched in minutes — not wasted in hours.

---

## 📁 Project Structure

```
FoodBridge_India_SparkR2/
│
├── FoodBridge_India_SparkR2.pdf    ← Main 4-Pages submission
├── Nikunj_Spark_Round2.pynb        ← ML models + visualization code
├── dashboard_full.png              ← Full ML dashboard (8-panel)
└── README.md                       ← This file
```

---

## 🧠 The Problem in One Line

**40% of food cooked in urban India never reaches a plate** — not because supply is short, but because coordination is broken.

| Reality | Numbers |
|---------|---------|
| Food waste generated in Delhi alone | 900 MT/day (MCD 2023) |
| Annual food value lost nationally | ₹92,000 Crore |
| Indians who are food-insecure | 200M+ |
| Average restaurant surplus per day | 15–20 kg |

The gap isn't charity. It's logistics, hygiene, trust, and timing. **FoodBridge India solves all four.**

---

## 💡 The Solution

**FoodBridge India** is a hyper-local, real-time food surplus matching platform for urban India.

### How It Works (4 Steps)
1. **Donor Posts** — Restaurant/cafe uploads surplus food via WhatsApp or app with photo + hygiene checklist
2. **AI Matches** — Algorithm instantly matches to the nearest verified NGO/receiver within 5km & 2-hour window
3. **Pick-Up Alert** — Volunteer receives GPS pin + food details; confirms pickup in <15 minutes
4. **Delivered** — Food reaches shelter/family; donor gets an impact card; both parties rate the exchange

### Safety & Trust System
- 🧼 Mandatory hygiene checklist per listing (FSSAI-aligned)
- ⏱ 2-hour pickup window (auto-expires after)
- 📍 GPS tracking for every delivery
- ⭐ Dual rating system (builds trust scores over time)

---

## 🤖 Machine Learning Components

### Models Built

| Model | Algorithm | Purpose | Performance |
|-------|-----------|---------|------------|
| A | Random Forest Classifier | Predict successful donor-receiver match | **98% accuracy** |
| B | Gradient Boosting Regressor | Predict kg of food waste prevented | **R² = 0.957** |
| C | K-Means Clustering | Donor segmentation (4 cohorts) | 4 distinct segments |
| D | Linear Regression | 24-month growth projection | Used for KPI forecasting |

### Features Used for Matching
- `surplus_kg` — quantity of food available
- `pickup_window_hr` — time window (1–4 hrs)
- `distance_km` — donor-to-receiver proximity
- `hygiene_score` — 0–10 hygiene rating
- `trust_score` — historical reliability score

### 4 Donor Segments (K-Means)
1. **High-Value Regulars** — High hygiene, high volume, repeat donors
2. **Small Occasional** — Low volume, infrequent, needs activation
3. **Bulk Seasonal** — Large batches but seasonal (caterers, events)
4. **Trust-Building** — New partners with lower initial trust scores

---

### Output
![Image Alt](https://github.com/nikunj-max/Spark_Fellowship_Round2_Nikunj_Bhardwaj/blob/main/dashboard_full.png)
The script will:
1. Generate a 500-record synthetic dataset modelling Delhi/NCR donor patterns
2. Train 4 ML models
3. Print model performance metrics to console
4. Save 4 visualization PNGs:
   - `dashboard_full.png` — Full 8-panel ML dashboard
   - `flow_diagram.png` — Platform flow with safety badges
   - `timeline_7day.png` — 7-day launch blitz circle timeline
   - `kpi_board.png` — Year 1 KPI projection board

### Sample Console Output
```
[ML] Random Forest Match Accuracy : 98.0%
[ML] GBM R² (waste prevented)     : 0.957  |  RMSE: 2.00 kg
[ML] KMeans segments identified   : 4
[ML] Projected waste prevented M24: 8,840 kg/month

============================================================
  MODEL SUMMARY
============================================================
  Random Forest  — Match Prediction Accuracy : 98.0%
  Gradient Boost — Waste Regression R²       : 0.957
  KMeans         — Donor Segments            : 4
============================================================
  MONTH 12 PROJECTIONS
============================================================
  Partners onboarded  : 18
  Waste prevented     : 5.0k kg/month
  Meals facilitated   : 14k meals/month
  CO₂ avoided         : 12 tonnes/month
  Revenue (est.)      : ₹12k/month
```

---

## 💰 Business Model

### Revenue Streams

| Phase | Model | Details |
|-------|-------|---------|
| 0–6 months | **Free** | Build GMV baseline, prove match rate |
| 6–12 months | **5% Commission** | ₹50/kg avg × 5% = ₹2.50/kg recurring |
| Ongoing | **CSR Sponsorship** | ₹50k–2L per corporate partner for branding + impact reporting |
| Ongoing | **NGO Subscription** | ₹999/month for priority alerts + analytics |

### Unit Economics (Month 12 Projection)
- Partners: ~18 active donors
- Food redistributed: ~5,000 kg/month
- Match rate: 65%+
- Monthly revenue: ~₹12,000
- CO₂ avoided: ~12 tonnes/month
- Meals served: ~14,000/month

---

## 🗓️ 7-Day Launch Plan

| Day | Action | Target |
|-----|--------|--------|
| 1 | Map 50 restaurants within 3km radius | Identify donor candidates |
| 2 | Launch WhatsApp broadcast + Instagram post | Go live publicly |
| 3 | First 3 donors sign the hygiene waiver | Early adopters |
| 4 | First pilot pickup day | Proof of concept |
| 5 | Collect feedback + refine checklist | Product-market fit |
| 6 | Onboard 7 partners total | Momentum |
| 7 | Hit 10 partners · publish impact report | Target achieved ✅ |

**Budget**: ₹10,000 (WhatsApp groups, Google Forms, Instagram, printouts, travel)  
**Team**: 3 people (1 ops, 1 tech, 1 outreach)  
**Tools**: WhatsApp Business, Google Forms, Google Sheets, Maps API (free tier)

---

## 📣 Marketing Strategy

### Tagline
> **"Don't Let It Rot. Let It Reach."**

### Campaign Hashtags
`#FoodBridgeIndia` · `#DontLetItRot` · `#WasteNotFeedMore`

### Gen-Z First Campaign Post (Sample)
> bro your restaurant is wasting food AGAIN? 😤  
> we matched 47 restaurants with shelters last week.  
> takes 2 mins to post. saves 20 meals. it's a vibe. 🌊  
> Join FoodBridge. Don't let it rot.

### Channel Strategy
- **Day 1–7**: WhatsApp broadcast to restaurant owners (warm network)
- **Week 2**: Instagram Reels with before/after impact stories
- **Month 2**: CSR pitch deck to Zomato Foundation, Reliance Foundation, local RWAs

---

## ✅ Success Metrics

| # | Metric | Target |
|---|--------|--------|
| 1 | Partners onboarded | 10 in 7 days → 50 by Month 3 |
| 2 | Food rescued | 500 kg+ in Month 1 |
| 3 | Match rate | ≥65% (ML model target) |
| 4 | Avg platform rating | 4.5/5 (donor + receiver) |
| 5 | CO₂ avoided | 50 tonnes by Year 1 |

---

## ⚠️ Risk Management

| Risk | Mitigation |
|------|------------|
| Food safety liability | FSSAI-aligned checklist + donor signs waiver |
| No-shows / cancellations | Auto-alerts + ₹500 penalty for repeat offenders |
| Low early adoption | Free phase + direct WhatsApp outreach on Day 1 |
| Tech barrier for donors | WhatsApp-first (no app download required) |

---

## 👤 About This Submission

This is a **genuine, ground-validated idea** — not a theoretical concept.

Before building this deck, I personally:
- Mapped restaurants near my college for surplus patterns
- Spoke with 3 local restaurants — all confirmed daily waste
- Identified 2 NGOs within 5km who actively need food donations

The ML models are built on realistic synthetic data that mirrors actual Delhi/NCR food ecosystem parameters (FSSAI reports, MCD data, NITI Aayog food waste studies).

---

## 🔗 Submission Details

- **Candidate**: NIKUNJ BHARDWAJ
- **College**: GGSIPU-USAR
- **File name**: `Nikunj_Bhardwaj_GGSIPU-USAR_SparkRound2.pdf`

---

*"You do not need a perfect idea. You need clear thinking, practical execution, and a builder mindset."*  
— Spark Fellowship Team

**FoodBridge India has all three.**
