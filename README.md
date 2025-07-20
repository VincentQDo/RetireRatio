# 📘 RetireRatio: MVP Project Proposal

## 🧠 Concept Summary

**RetireRatio** is a data-driven financial dashboard that visualizes long-term macroeconomic trends — especially **retirement-related capital flows** and **demographic pressures** — to help investors understand structural market risk and opportunity.

The core focus is on:
- **401(k) and IRA contribution vs. withdrawal behavior**
- **Aging U.S. population and its impact on retirement liquidity**
- **Passive vs. active investing trends**
- **Macro insights backed by real public data**

This project is for long-term thinkers and data-driven investors, not real-time traders.

---

## 👤 Target Users (MVP Phase)

| Audience             | Description                                                  |
|----------------------|--------------------------------------------------------------|
| Long-term investors  | FIRE community, DIY retirement planners, value investors     |
| Analysts/researchers | Macro researchers seeking structural economic signals        |
| Content creators     | Seeking data-backed visuals for market commentary            |
| Myself (Quang)       | To guide long-term investment allocation and analysis        |

**Projected initial users**: 100–500 (via SEO, Reddit, HN, X)

---

## 🧱 Scope of MVP

### ✅ Core Features
- 401(k) & IRA **net flows**: contribution vs. withdrawal
- U.S. population: retiree (RMD-age) vs. working-age trend
- Passive vs. active fund AUM over time
- Simple composite indicator: *"Retirement Liquidity Pressure Index"*
- Interactive charts + basic written insights
- Citation/source per chart
- Responsive web app with self-hosted deployment

### ❌ Excluded from MVP
- SPY or stock price tracking
- Daily data updates
- Subscriber-only or premium content
- Real-time news/data feeds

---

## 🧠 Use Cases

- Personal investing signal dashboard
- Long-form evergreen macro blog posts
- Reddit/X engagement via original charts
- Monthly/quarterly insights digest (optional)

---

## 📊 Data Sources (MVP)

| Domain                    | Source         | Method              | Notes                                   |
|---------------------------|----------------|----------------------|-----------------------------------------|
| 401(k)/IRA flows          | ICI.org        | XLS/PDF scraping     | Manual or Python/pandas parsing         |
| Retirement asset growth   | FRED           | API                  | e.g. `IRATOTL`, `QFRNTIRPUSQ`           |
| Demographics              | Census API     | JSON API             | ACS and Decennial data, age brackets    |
| Passive vs. active flows  | ICI.org        | XLS parsing          | Quarterly fund flow and AUM data        |
| RMD age thresholds        | IRS/Treasury   | Static CSV           | Determine age-driven withdrawal pressure|

---

## 🧰 Technical Stack

| Layer     | Tech                          |
|-----------|-------------------------------|
| Frontend  | SvelteKit + Chart.js or D3.js |
| Backend   | Go (API + data scheduler)     |
| ETL       | Python (pandas, requests)     |
| Database  | SQLite                        |
| Hosting   | Docker on VPS (e.g. DO/Hetzner) |
| Analytics | Optional (Plausible or GoatCounter) |

---

## 💵 Projected Cost (MVP Phase)

| Item                  | Cost (USD)     |
|-----------------------|----------------|
| Domain + DNS          | $10–20         |
| VPS Hosting (6 months)| $30–60         |
| APIs / Data Access    | Free           |
| Development           | Time only      |

**Total**: ~$50–80

---

## ⚠️ Concerns & Limitations

| Concern                         | Mitigation                                      |
|----------------------------------|-------------------------------------------------|
| Data scraping friction          | Start small, build ETL pipelines iteratively   |
| Limited audience                | Focus on niche quality, not viral growth       |
| Not real-time / low engagement  | Embrace slow, long-form content model          |
| API rate limits or data gaps    | Use monthly aggregation + caching              |
| No monetization (yet)           | Fine — focus on utility, traction comes later  |

---

## 🗓️ MVP Roadmap (8 Weeks)

| Phase                      | Timeline    | Deliverables                                     |
|----------------------------|-------------|--------------------------------------------------|
| 1. Data Source Testing     | Week 1      | Test ICI, FRED, Census APIs                      |
| 2. ETL + Storage Layer     | Week 2–3    | Python scripts → SQLite schema                  |
| 3. Go API Backend          | Week 3–4    | REST endpoints + refresh scheduler              |
| 4. Frontend + Charts       | Week 4–6    | SvelteKit + D3.js or Chart.js UI                |
| 5. Insights + Copywriting  | Week 6–7    | Draft brief takeaways per chart                 |
| 6. Deployment + Polish     | Week 7–8    | Deploy live site, SEO basics, Reddit test post  |

---

## 📌 Success Criteria

- Charts render real 401(k)/IRA trend data
- Public page deployed and SEO-ready
- At least 3–5 insightful visualizations with writeups
- Initial organic feedback from Reddit/X/HN

---

## ✅ Final Notes

RetireRatio is a long-term, niche project with compounding value. The MVP will focus on:
- **Retirement system stress**
- **Demographic realities**
- **Data-backed investing perspective**

Monetization, expansion, and subscriptions are **not the goal** for now.

The goal is simple: **build something useful, insightful, and honest.**

---

