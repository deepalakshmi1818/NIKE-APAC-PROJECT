# NIKE-APAC-PROJECT
Data analytics project simulating Nike’s APAC YouTube ad strategy — SQL, Python (Pandas, Seaborn, SciPy) &amp; Power BI analysis of 39,199 trending videos across India, Japan &amp; South Korea for brand-safety and media-spend insights.
# Nike APAC — YouTube Ad Placement & Brand-Safety Analytics

A data analytics project simulating Nike's APAC digital ad strategy, analyzing **39,199 trending YouTube videos** across **India, Japan, and South Korea** to guide media spend, campaign timing, and brand-safety decisions.

---

## 📌 Project Overview

Brands running YouTube ad campaigns across APAC need to know **where**, **when**, and **how safely** their ads can appear. This project analyzes regional trending-video behavior — engagement, controversy risk, genre mix, and publishing rhythm — to answer three questions a media planning team would ask:

1. Which content genres and regions are safe to standardize creative across?
2. Where is brand-safety risk (dislike ratio / "friction") elevated, and does it differ by market?
3. When should campaign assets and influencer drops go live to maximize organic visibility at the lowest bid cost?

---

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| Data extraction & querying | SQL |
| Data cleaning & transformation | Python (Pandas) |
| Statistical testing | SciPy (Kruskal-Wallis H-test) |
| Visualization | Seaborn, Matplotlib |
| Dashboarding | Power BI |

---

## 📊 Dataset

- **39,199** trending videos across 3 regions: India, Japan, South Korea
- Fields: views, likes, dislikes, publish time, trending time, genre/category, region
- Power BI dashboard layer covers **35,000+** videos for the interactive engagement/friction view

---

## 🔍 Key Findings

### 1. Viral Velocity (Days to Trending)
India spikes sharply within Day 1–2 then decays fast. Japan is a slow-burn, peaking Day 3–5. South Korea holds a steady, moderate rise across Day 2–4.
→ **India needs front-loaded, closely-monitored spend; Japan supports sustained exposure.**

### 2. Top Genres by Region
Entertainment dominates all three markets (India 16,712 · South Korea 8,955 · Japan 6,259 trending videos). India's #2 genre is News & Politics; Japan's #2 is People & Blogs.
→ **Genre mix should guide creative placement per market.**

### 3. Engagement Rate (Likes / Views)
Median engagement: India 0.94%, Japan 1.16%, South Korea 1.10%. Kruskal-Wallis test: H = 0.81, p = 0.667 — **not statistically significant**.
→ **Core audience engagement behavior is uniform across borders — safe to standardize creative.**

### 4. Dislike Ratio (Brand-Safety Friction)
Average dislike ratio: India 7.91% (highest friction), Japan 6.19%, South Korea 5.33% (safest). Kruskal-Wallis test: H = 4886.88, p < 0.001 — **highly significant**.
→ **Brand-safety risk is culturally/regionally driven, not universal — India requires tighter moderation.**

### 5. Peak Publishing Hours
Japan and South Korea show a sharp mid-morning spike (peak share 9.7% Japan, 9.3% South Korea at 9–10 AM). India's curve is flatter, peaking around 12–2 PM. The **08:00–12:00 local window** is consistently the densest across all three markets; overnight hours (18:00–06:00) are consistently weakest.
→ **08:00–12:00 local time is the optimal window to launch campaign assets and influencer drops at the lowest initial bid cost.**

---

## 💡 Business Recommendation

| Market | Strategy |
|---|---|
| **India** | Front-loaded, closely-monitored ad spend; extra brand-safety moderation given higher friction |
| **Japan** | Steadier, narrative-driven placements; sustained exposure over several days |
| **South Korea** | Safest market for standardized creative; steady moderate rollout |
| **All markets** | Concentrate launch timing inside the shared 08:00–12:00 local window |

---

## 📁 Repository Structure

```
├── data/                     # Raw and cleaned trending-video datasets
├── sql/                      # Extraction & aggregation queries
├── notebooks/                # Python analysis (Pandas, Seaborn, SciPy)
├── dashboard/                # Power BI (.pbix) file
├── charts/                   # Exported chart gallery (viral velocity, genre mix, engagement, friction, publishing hours)
└── README.md
```

---

## 👤 Author

**Deepa Lakshmi**
Data Analyst | SQL · Python · Power BI · Tableau
[LinkedIn](https://linkedin.com/in/deepalakshmi) · Deepalakshmi0718@gmail.com
.
