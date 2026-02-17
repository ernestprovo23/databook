# Post 5: What Does a Modern Data Team Actually Look Like?
**Publication date**: Wednesday, March 4, 2026
**Source**: Chapter 3
**URL slug**: /modern-data-team-structure

---

## HOOK

Most companies have data people. A few analysts in finance. A data engineer who maintains the warehouse. Maybe a data scientist who built a model once and now maintains dashboards. These are data people. They are not a data team.

The distinction matters enormously, and almost nobody makes it.

A collection of individuals who work with data, scattered across departments, reporting to different leaders, operating with different priorities and no shared standards, is not a team. It is a coincidence. And you cannot build an AI strategy on a coincidence.

I have spent years helping organizations figure out why their data capabilities plateau despite hiring more data people. The answer is always the same: they have staffed roles without designing a team. They have added headcount without building structure. And structure -- not headcount -- is what determines whether a data organization can operate at the level AI demands.

---

## CORE ARGUMENT

Let me give you a framework for thinking about this. I call it the 5-Level Operations Maturity Model. It is not about technology sophistication. It is about how an organization's data team is structured, how data flows, and what that structure enables or prevents.

**Level 1: Ad-Hoc Data Access.** This is where most small companies start and where a surprising number of large companies remain stuck. Data lives in spreadsheets, individual databases, and people's heads. Analysis is done by whoever knows SQL or is good at Excel. There is no shared infrastructure, no data catalog, no documentation. When someone leaves, their institutional knowledge leaves with them. AI at this level is impossible. You cannot train a model on data that exists in forty different spreadsheets with forty different schemas maintained by forty different people who each have their own naming conventions.

**Level 2: Centralized Storage, Decentralized Use.** The organization has invested in a data warehouse or data lake. Data gets consolidated. There is some engineering discipline around ingestion and storage. But the users of that data -- the analysts, the business teams, the would-be AI builders -- are still scattered across the organization. They access the same data but interpret it differently. There is no shared semantic layer, no agreed-upon definitions, no governance. This is where most mid-market and many enterprise companies live. They have the infrastructure for AI but not the organizational coherence. Two analysts in two departments can query the same table and produce contradictory reports, and there is no mechanism to resolve which one is correct.

**Level 3: Governed Data Operations.** This is the inflection point. At Level 3, the organization has not just centralized data but centralized the authority over what data means. There is a data team -- not data people, a team -- with shared standards, a data dictionary, defined ownership for every critical dataset, and quality metrics that someone is accountable for. The team may be centralized or federated (hub-and-spoke), but either way, there are shared norms. When a business stakeholder asks "what was our revenue last quarter?" there is one answer, and the data team can certify it.

Most AI success stories come from organizations operating at Level 3 or above. That is not a coincidence. AI needs certified, governed, consistently defined data as its foundation. Everything below Level 3 produces the "garbage in, garbage out" problem, but at Level 3, you have the organizational infrastructure to prevent garbage from entering the system in the first place.

**Level 4: Integrated Data and Decision Operations.** At Level 4, the data team is not just producing clean data -- it is embedded in decision-making processes. Data products are built and maintained like software products, with SLAs, versioning, and user feedback loops. Business decisions have explicit data dependencies, and those dependencies are managed. The data team does not just answer questions; it shapes which questions get asked. ML models are in production, monitored, and maintained by dedicated MLOps processes. This is where AI starts compounding -- where models improve because the organizational feedback loop between model output and data quality is deliberate and continuous.

**Level 5: AI-Native Operations.** The organization does not "use AI." AI is embedded in operational processes as a first-class participant. Decisions that can be automated are automated, with human oversight designed into the system. Data quality is measured continuously and automatically, with alerts when drift is detected. The data team's role shifts from producing analysis to designing and maintaining intelligent systems. New business processes are designed with AI integration from the start, not bolted on after. Very few organizations operate here today. But this is the direction of travel, and the organizations that reach Level 3 and 4 deliberately will get here first.

Here is the hard truth: you cannot skip levels. I have watched organizations try to jump from Level 1 to Level 4 by buying a sophisticated ML platform. It does not work. Each level builds the organizational muscle for the next. You cannot maintain ML models in production (Level 4) if you cannot certify the quality of the data feeding them (Level 3). You cannot certify quality if you have not centralized and governed your data (Level 2 to 3 transition). The maturity model is sequential because each level's capabilities are prerequisites for the next.

---

## FRAMEWORK

**The 5-Level Operations Maturity Model**

| Level | Team Structure | Data Access | AI Capability | Typical Company Stage |
|---|---|---|---|---|
| **1: Ad-Hoc** | No formal data team; analysts embedded in departments with no coordination | Spreadsheets, local databases, tribal knowledge; no shared infrastructure | None; insufficient data consistency for any modeling | Startups, small businesses, or large companies with legacy neglect |
| **2: Centralized Storage** | Data engineers maintain infrastructure; analysts scattered across business units with no shared standards | Data warehouse or lake exists; access is available but interpretation is inconsistent | Experimental only; proofs of concept that do not reach production | Mid-market companies; enterprises early in "digital transformation" |
| **3: Governed Operations** | Defined data team (centralized or hub-and-spoke) with shared standards, data dictionary, quality metrics, and named dataset owners | Governed, documented, certified; one source of truth with clear definitions | Production-viable; models can be trained on certified data with validated definitions | Enterprises with dedicated data leadership (CDO or VP of Data) |
| **4: Integrated Decision Ops** | Data team embedded in business processes; data products managed like software with SLAs and feedback loops; dedicated MLOps function | Data products with versioning, SLAs, and quality monitoring; self-service with guardrails | Active production models with monitoring, retraining pipelines, and business feedback loops | Mature enterprises with data-informed culture and operational AI |
| **5: AI-Native** | Data and AI teams integrated into operational design; human oversight designed into automated decision systems; continuous improvement loops | Real-time, continuously monitored, automatically quality-checked; data as a living operational asset | AI embedded in operational processes; new processes designed AI-first; compounding intelligence | Industry leaders; data-native companies; organizations 3-5 years ahead of current enterprise norm |

---

## TAKEAWAY

**What to do Monday morning:**

- **Assess your level honestly.** Gather your data team leads and one business stakeholder. Read the maturity model descriptions aloud. Ask everyone to independently write down which level they think the organization operates at. If there is disagreement -- and there almost always is -- the discussion about why they disagree is more valuable than the number. The gap between how leadership perceives data maturity and how the data team experiences it is diagnostic.

- **Identify one Level 3 requirement you are missing and build it this quarter.** If you do not have a data dictionary, build one for your top ten datasets. If you do not have named data owners, assign them. If you do not have quality metrics, define accuracy and freshness scores for your three most critical data sources. You do not need to achieve Level 3 in a quarter. You need to make concrete, visible progress on one specific gap.

- **Stop hiring data scientists until you have Level 3 foundations.** This is controversial advice, and I stand by it. A data scientist without governed, certified, well-documented data spends eighty percent of their time doing data engineering and data governance work that should have been done before they were hired. Hire the governance and engineering roles first. Build the foundation. Then hire the scientists who will build on it. The ROI on data science talent increases dramatically when they can actually do data science instead of data janitorial work.

---

**Book drops Q3 2026. Subscribe for early access + exclusive chapters not in the published version.** If the maturity model sparked a debate on your team about what level you are actually at, good. That debate is the beginning of organizational clarity. Forward this to the people who need to be in that conversation.

---

## X Post (publish same day)

**Main post:**
"Most companies have data people. Almost none have a data team. The distinction is the difference between individuals who work with data and an organization that can build AI. You cannot build an AI strategy on a coincidence of headcount."

**Reply to own post:**
New Substack: The 5-Level Operations Maturity Model for data teams. Most enterprises are stuck between Level 2 and 3. I explain why, and what Level 3 actually looks like. Free read: [link] From "Data Is The New Oil" (Q3 2026).

---

## YouTube Short Script

**[HOOK - 0:00 to 0:15]**
Most companies have data people. Analysts in finance. An engineer maintaining the warehouse. Maybe a data scientist who built one model and now maintains dashboards. That is not a data team. That is a coincidence. And you cannot build AI on a coincidence.

**[BODY - 0:15 to 0:55]**
I use a 5-level maturity model. Level 1 is ad-hoc -- spreadsheets and tribal knowledge. Level 2 is centralized storage, but everyone interprets the data differently. Level 3 is where the magic starts -- governed operations, shared definitions, named data owners, quality metrics someone is accountable for. Almost all AI success stories come from Level 3 or above. And here is the thing you cannot skip levels. I have watched companies try to jump from Level 1 to Level 4 by buying an ML platform. It never works.

The question is not "how many data people do we have?" It is "what level is our data organization operating at, and what specific gap is preventing us from reaching the next one?"

**[CTA - 0:55 to 1:05]**
Full maturity model breakdown is on my Substack with the team structures and capabilities at each level. Link in bio. From my book "Data Is The New Oil" -- Q3 2026.
