# Appendix C: Financial Models



These models are simplified templates to support executive decision‑making. Replace placeholder values with your own.



## C1. AI Project ROI Template



**ROI (%) = (Net Benefit ÷ Total Cost) × 100**



**Total Cost:** Data engineering + model development + infrastructure + change management

**Net Benefit:** Revenue uplift + cost savings + risk reduction



**Example inputs:**

Revenue uplift: $1,200,000

Cost savings: $500,000

Risk reduction: $300,000

Total cost: $1,500,000



**Net Benefit = $2,000,000**

**ROI = (2,000,000 ÷ 1,500,000) × 100 = 133%**



## C2. Cost of Poor Data Calculator



**Annual Cost = (Error Rate × Volume × Cost per Error) + (Rework Hours × Hourly Cost)**



**Error Rate:** % of records with critical errors

**Volume:** Total records processed annually

**Cost per Error:** Financial impact per error (claims, refunds, lost time)

**Rework Hours:** Staff time spent fixing data issues



**Example inputs:**

Error rate: 3%

Volume: 2,000,000 records

Cost per error: $15

Rework hours: 4,000

Hourly cost: $60



**Annual Cost = (0.03 × 2,000,000 × 15) + (4,000 × 60)

= $900,000 + $240,000 = $1,140,000**



## C3. Build vs. Buy Cost Comparison



**Build Cost (Year 1) = Dev + Infra + Hiring + Governance**

**Buy Cost (Year 1) = Licenses + Integration + Vendor Support**



Include a **3‑year view**:

Build costs typically drop after Year 1

Buy costs often rise with usage and seat counts



**Decision rule:** If Year‑2+ recurring costs exceed the one‑time build premium, build becomes cheaper over the horizon.



## C4. AI Run‑Cost Model (Per‑Query)



**Per‑Query Cost = (Infra Cost ÷ Total Queries) + Monitoring + Retraining**



Use this to estimate when private infrastructure becomes cheaper than API pricing. The crossover point often occurs when usage stabilizes and volume rises.



## Sources (Draft)

Format: [SRC-##] Claim. Source. Status.

[SRC-01] Financial model templates derived from book content and standard ROI practice. Internal.
