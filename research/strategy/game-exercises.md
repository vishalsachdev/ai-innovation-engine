# Game-Based Teaching Exercises (gstack + Paperclip)

Exercises designed around: games/competitions/leaderboards, low floor/high ceiling, real-world impact, real-time feedback, constraints (budgets, tokens), and meta-learning about AI while using AI.

---

## 1. "The $10 Startup" (Budget Constraint Game)
- **Format:** 2-hour sprint, teams of 3-4
- **Setup:** Each team gets a Paperclip company with $10 real-token budget
- **Task:** Build a landing page for a product solving a UIUC student problem
- **Leaderboard:** Output quality (peer-voted) / dollars spent / speed
- **Mental models:** Resource allocation, burn rate, unit economics, prompt engineering as cost lever

## 2. "Org Chart Wars" (Structural Design A/B Test)
- **Format:** 1 week, individual/pairs, half flat org, half hierarchical
- **Setup:** Same budget, same mission, different org structures
- **Leaderboard:** Goal completion rate / cost per ticket / governance incidents
- **Mental models:** Span of control, coordination cost, principal-agent problem

## 3. "Office Hours Gauntlet" (Idea Validation Tournament)
- **Format:** Single-elimination bracket, 30 min/round
- **Setup:** Students run gstack `/office-hours` on business ideas
- **Rounds:** Validation → adversarial review (`/plan-ceo-review REDUCTION`) → full `/autoplan`
- **Leaderboard:** Demand reality score / specificity / peer vote
- **Mental models:** "Interest is not demand," narrowest wedge, Socratic AI partnership

## 4. "The Audit" (Security & Governance Red/Blue Team)
- **Format:** 90 min, pairs, swap roles at halftime
- **Blue:** Build Paperclip company + run gstack `/cso`
- **Red:** Review audit trail, find governance failures
- **Leaderboard:** Vulnerabilities found / governance failures found / cost efficiency
- **Mental models:** Attacker vs defender mindset, governance tradeoffs, audit trails

## 5. "Ship It" (Speed-to-Market Race)
- **Format:** 3-hour race, teams of 2-3
- **Phases:** `/office-hours` (20m) → `/autoplan` (30m) → Paperclip setup (20m) → Build (60m) → `/qa` (20m) → `/ship` (10m)
- **Constraints:** $15 budget, must pass `/qa` Standard tier, deploy to public URL
- **Leaderboard:** Time to ship / QA score / budget remaining / peer UX rating
- **Mental models:** Shipping > perfecting, parallelization, QA not optional

## 6. "The Retro" (Weekly Reflection Game)
- **Format:** 15 min weekly recurring
- **Setup:** Run gstack `/retro 7d`, submit 3-sentence reflection
- **Leaderboard (cumulative):** Shipping streak / insight score (peer-rated) / improvement trajectory
- **Mental models:** Data-driven self-assessment, kaizen, leading vs lagging indicators

## 7. "Model Marketplace" (Token Economics Simulation)
- **Format:** Trading game, full class, 5 rounds
- **Setup:** Fixed budget, 3 talent tiers (Haiku/Sonnet/Opus pricing), real tasks
- **Rounds:** Hire → Sprint → Review ROI → Pivot → Final
- **Leaderboard:** Quality/spend ratio / best deliverable / learning rate (R3→R5 improvement)
- **Mental models:** Token economics, 80/20 rule for AI spend, prompt engineering as force multiplier

---

## Design Principles (from Vishal's pedagogy preferences)

| Criterion | How Every Exercise Satisfies It |
|---|---|
| Leaderboard | 3+ measurable dimensions, displayed live |
| Low floor | Entry = dashboard click or slash command, zero code |
| High ceiling | Mastery = custom org design, prompt engineering, budget optimization |
| Constraints | Budget caps, time boxes, run limits, approval gates |
| Real-world impact | Ship real apps, deploy to real URLs, create reusable templates |
| Real-time feedback | Paperclip dashboard, gstack reports, live cost tracking |
| Meta-learning | Every constraint teaches an AI mental model |
