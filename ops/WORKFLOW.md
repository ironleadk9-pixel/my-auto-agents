# Product research workflow (default)

**Standing process for every new product lane.** Approved by Joseph 2026-09-20.
Does not rewrite in-flight work (e.g. HARNESS-001 continues on its existing path).

Crew: Pike researches → Harbor scores → Joseph decides → Reed designs later → Joseph publishes in YNS.

---

## Five beats

### 1. Intake
- Name the product lane (e.g. tactical harness, matching leash, collar).
- Pull the Amazon cluster and the race-bottom price range.
- Define **where we will not play** (race-to-bottom SKUs, banned brand clones, claim risks).

### 2. Supplier sweep with reviews from day one
- Scout real suppliers with real `source_url`s (never invent).
- From day one: ratings, buyer feedback, return / 1-star complaint themes.
- **Cut anything that fails the review bar before it reaches Joseph.**

### 3. Landed estimate on survivors only
- For candidates that survive the review bar only: build a **door-to-door landed proxy** (not FOB-only).
- Include freight / duty / calendar ship days as far as verifiable; mark UNSET honestly when missing.
- Score math uses landed reality:  
  `spread = sell − landed − Stripe − 6 − (0.10 × sell)`  
  KEEP only if `spread >= 10`. Sell band $34–$49 unless Joseph sets another band for that lane.

### 4. Score and open the packet
- Harbor scores **KEEP / KILL / WAIT** against the full picture (intake + reviews + landed).
- Open the packet under `products/` (and PR).  
- **Goal:** hand Joseph a clean verdict — not a list of open questions caused by missing first-pass data.
- UNSET on true landed, ship_days, or source_url still blocks KEEP (treat as KILL / WAIT per ops rules).

### 5. Joseph’s two decisions
1. **Sample yes / no**
2. Type **APPROVED** or **KILL** in `approvals/QUEUE.md`

After APPROVED + sample path, Reed may design listing copy for that SKU only. Joseph adds the product in YNS and runs `publish:store`. Agents never spend, never `publish:store`, never POST `/products`.

---

## Defaults this file owns

| Rule | Default |
|---|---|
| Process for new lanes | This five-beat flow |
| Brand clones | No ICEFANG / OneTigris / rabbitgoo / AUROTH |
| Service-dog claims | Never |
| Fake stock / scarcity | Never |
| Harbor asks Joseph | At most 3 decisions; prefer the two in beat 5 |
