# Post 9: Build, Buy, or Partner? The Framework That Changes the Decision
**Publication date**: Saturday, March 14, 2026
**Source**: Chapter 7
**URL slug**: /build-buy-partner-framework

---

In 2023, I watched a financial services company spend fourteen months and $2.3 million building a custom data quality platform. They had a team of nine engineers on it. They wrote 80,000 lines of code. They were proud of it.

The platform did roughly what Atlan, Monte Carlo, or any of a dozen commercial tools did out of the box. Except theirs had no community, no update roadmap beyond what their nine engineers could manage, and it took six months to onboard a new team member because the documentation was four Slack threads and a README that had not been updated since sprint three.

When I asked the VP of Engineering why they built instead of bought, the answer was: "We wanted full control."

Full control of what? Of a commodity capability that had nothing to do with why their customers chose them over the competition? They spent fourteen months building a monitoring dashboard while their competitors spent fourteen months building proprietary trading models on clean data.

That is the build-buy-partner decision gone wrong. And almost every enterprise I work with has a version of this story.

## The Decision Is Not About Cost

The first mistake most organizations make is framing build-vs-buy as a cost comparison. They pull up a spreadsheet: cost of engineering hours to build versus annual license fee to buy. The build option usually looks cheaper on paper because nobody accounts for maintenance, documentation, onboarding, opportunity cost, or the inevitable moment eighteen months later when the engineer who built the thing leaves and nobody understands the codebase.

The real question is not "what does it cost?" The real question is "where does our competitive advantage live?"

This is the principle that should govern every build-buy-partner decision in your data organization. If a capability is core to your differentiation -- if it is the reason customers choose you over competitors -- build it. Own it. Invest in it. Make it yours.

If a capability is commodity infrastructure -- something every company in your industry needs but nobody wins because of -- buy it. Get the best commercial tool, implement it quickly, and move on.

If a capability requires ecosystem access, specialized expertise, or market relationships that you do not have and cannot reasonably build -- partner. Find someone who has what you need and structure a relationship that gives you access without requiring you to become something you are not.

That is the entire framework. Three questions, three paths.

## The Decision Matrix

Here is how I walk clients through this. For every data capability or tool decision on the table, fill in this matrix.

| Capability Type | Core Differentiator? | Time to Market Need | Internal Capability | Recommended Path | Warning Sign |
|---|---|---|---|---|---|
| Proprietary ML models trained on your data | Yes -- this is your product edge | Medium (3-6 months) | Have data scientists, need infrastructure | BUILD -- own the IP, own the models, own the training pipeline | Outsourcing model training to a vendor who retains the weights |
| Data pipeline orchestration (Airflow, Dagster, etc.) | No -- every company needs pipelines | High (need it now) | Engineers could build it but should not | BUY -- use a managed service, ship in weeks not months | Engineers "prefer" to build a custom orchestrator |
| Cloud data warehouse (Snowflake, BigQuery, etc.) | No -- commodity storage and compute | High (foundational) | No reason to build this | BUY -- pick one, commit, optimize | Building a custom query engine when Snowflake exists |
| Real-time fraud detection models | Yes -- directly protects revenue | High (regulatory + business) | Have the data, need specialized ML expertise | BUILD with selective PARTNER -- own the model, partner for initial expertise | Buying an off-the-shelf fraud model that cannot learn from your data |
| Data catalog and metadata management | No -- table stakes for governance | Medium | Governance team exists, tool does not | BUY -- Atlan, Alation, or similar | Spending a year building a custom catalog nobody adopts |
| Industry-specific data feeds (market data, health records) | No -- you need access, not ownership | Low (ongoing relationship) | You do not produce this data | PARTNER -- license the data, integrate it cleanly | Trying to scrape or replicate data a partner already provides |
| Customer behavior analytics on your platform | Yes -- understanding your users is your edge | Medium | Have the data, have analysts | BUILD -- own the analysis, own the insights, own the definitions | Handing your clickstream data to a third-party analytics vendor who learns from it |

The rightmost column -- Warning Sign -- is the most important one. Every wrong decision has a tell. The tell for a bad build decision is usually someone saying "we want full control." The tell for a bad buy decision is usually "it was cheaper." The tell for a bad partner decision is usually "we did not have time."

## The Three Mistakes

**Mistake 1: Building commodity infrastructure.** This is the most common and the most expensive. Engineers love to build. That is what they were hired to do. And left to their own instincts, a talented engineering team will build beautiful, custom solutions to solved problems. Your job as a data leader is to redirect that energy toward problems that actually differentiate your business.

**Mistake 2: Buying your core differentiator.** This is the quieter mistake, and it is more dangerous. When you buy an off-the-shelf ML model for your core use case, you are renting someone else's intelligence. You do not own the training data pipeline. You do not own the model weights. You cannot customize the architecture. And worst of all, your competitor can buy the same model tomorrow and eliminate whatever advantage you thought you had.

**Mistake 3: Partnering out of impatience.** Partnerships work when you need access to something you structurally cannot build -- data feeds, market relationships, specialized domain expertise during a ramp-up. Partnerships fail when they are just a shortcut to avoid the work of building internal capability. If you partner because you are impatient, you will be dependent forever. If you partner because you need a bridge, you will eventually own the capability yourself.

## How to Pressure-Test the Decision

Before you commit to build, buy, or partner on any data capability, run it through three questions:

**"If our competitor had this exact same capability tomorrow, would it matter?"** If no, it is commodity -- buy it. If yes, it is a differentiator -- build it.

**"Can we maintain this in-house for the next three years?"** Building something you cannot maintain is worse than buying something you do not love. Be honest about your team's capacity, not just their capability.

**"What happens if this vendor or partner disappears?"** If the answer is "we are in serious trouble," you have a dependency problem. That does not mean you should not buy or partner -- it means you should negotiate accordingly and have a migration plan.

## What to Do Monday Morning

1. **List your last five data tool or platform decisions.** For each one, write down whether you built, bought, or partnered -- and whether that capability is a core differentiator, commodity infrastructure, or ecosystem access. If you built a commodity or bought a differentiator, you have found the problem. Flag it for re-evaluation.

2. **Apply the three-question test to your next pending decision.** Whatever data tool, platform, or capability your team is currently evaluating -- run it through the competitor test, the maintenance test, and the disappearance test. Write down the answers before the next vendor call.

3. **Protect your engineers' time.** Identify one custom-built internal tool that replicates a commercial product. Calculate the engineering hours spent on maintenance last quarter. Present the number to your leadership team with a recommendation to migrate and redeploy those engineers to differentiating work.

---

Book drops Q3 2026. Subscribe for early access and exclusive chapters not in the published version. Every Monday and Thursday, I am serializing "Data Is The New Oil" right here -- frameworks you can use before the book even ships.

---

## X Post (publish same day)

**Post:**
"A company spent 14 months and $2.3M building a custom data quality platform. It did what any commercial tool does out of the box. They wanted 'full control' -- of a commodity capability that had nothing to do with why customers chose them."

**Reply:**
Build what differentiates you. Buy what everyone needs. Partner for access you cannot create. The full decision matrix is in today's post: [Substack link]

---

## YouTube Short Script

**[HOOK -- 0:00-0:12]**
Fourteen months. Two point three million dollars. Nine engineers. Eighty thousand lines of code. To build a data quality platform that did exactly what a commercial tool does out of the box. I see this mistake everywhere.

**[BODY -- 0:12-0:50]**
The build-buy-partner decision is not about cost. It is about one question: where does your competitive advantage live? If the capability is core to your differentiation -- the reason customers choose you -- build it. Own the IP, own the models, own the pipeline. If it is commodity infrastructure that every company needs, buy it. Get the best tool, ship it in weeks, and move on. If it requires ecosystem access you do not have, partner. The mistake most companies make is building commodity infrastructure while buying their core differentiator. That is exactly backwards.

**[CTA -- 0:50-1:05]**
I published the full decision matrix on Substack today -- every capability type mapped to the right path. Link in bio. Book drops Q3 2026.
