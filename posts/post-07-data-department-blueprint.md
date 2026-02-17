# Post 7: The Data Department Blueprint
**Publication date**: Monday, March 9, 2026
**Source**: Chapter 4
**URL slug**: /data-department-blueprint

---

I want you to do something for me. Pull up your company's org chart. Find the word "data" somewhere on it. Now trace the reporting lines. How many different VPs do your data people report to?

If the answer is more than one, you do not have a data department. You have data people. That is not the same thing.

I have walked into organizations with sixty analysts, a dozen data engineers, and a handful of scientists scattered across marketing, finance, operations, and product. Each one reports to a business leader who treats them as a personal resource. Each one builds pipelines that duplicate work being done three floors away. Nobody owns data quality. Nobody owns the catalog. Nobody owns the strategy. And then the CEO stands up at an all-hands and asks, "Why aren't we an AI company yet?"

You are not an AI company because you never built the department that makes AI possible.

## The Real Problem With "Embedded" Data Teams

The distributed model -- analysts embedded in business units with dotted-line reporting to some central figure -- became popular for a reason. It sounded good. Business proximity. Domain expertise. Fast iteration.

Here is what actually happened.

Marketing's analyst built a customer segmentation model using a definition of "active customer" that finance had never seen. Finance's analyst built a revenue forecast on data that operations knew was three weeks stale. Product's data engineer built an event pipeline that captured 40% of actual user behavior because nobody told them about the mobile app's separate tracking system.

Each person did reasonable work in isolation. The organization got chaos.

This is the structural problem I keep coming back to throughout this book: organizational design determines outcomes. Not talent. Not tools. Not budget. Structure. If you scatter data people across the org chart with no shared standards, no common infrastructure, and no unified leadership, you will get exactly what that structure produces -- fragmented, contradictory, unreliable data.

And you cannot build AI on unreliable data. Full stop.

## What a Data Department Actually Looks Like

A properly chartered data department owns five functions. Not three. Not seven. Five. Each one requires a named owner, a clear reporting line, and a measurable deliverable. If any one of these functions is missing or orphaned in another department, your data capability has a structural hole that no amount of hiring will fix.

Here is the charter template I use with every client.

| Function | Owner Role | Reporting Line | Key Deliverable | Success Metric |
|---|---|---|---|---|
| Data Engineering | Head of Data Engineering | Reports to CDO/VP Data | Production pipelines, data platform | Pipeline uptime > 99.5%, data freshness SLAs met |
| Data Governance | Head of Data Governance | Reports to CDO/VP Data | Data catalog, quality standards, access policies | % of critical data assets cataloged and quality-scored |
| Analytics & BI | Head of Analytics | Reports to CDO/VP Data | Dashboards, ad hoc analysis, business metrics | Stakeholder satisfaction score, decision-support coverage |
| Data Science & ML | Head of Data Science | Reports to CDO/VP Data | Models, experiments, AI products | Model accuracy in production, experiment velocity |
| Data Strategy & Operations | Chief Data Officer / VP Data | Reports to CEO or COO | Roadmap, budget, cross-functional alignment | Data maturity score improvement, ROI on data initiatives |

Notice what is not on this chart: "Data Analyst reporting to VP of Marketing." That person might sit with marketing. They might attend marketing standups. But their standards, their tooling, their quality expectations, and their career path run through the data department.

This is the difference between embedding and scattering. Embedding means a data professional works closely with a business unit while maintaining membership in a data organization that sets standards. Scattering means that person belongs to marketing and nobody checks whether their definition of "conversion" matches anyone else's.

## The Charter Nobody Writes

Most data departments do not have a charter. They have a Confluence page from 2021 that lists team members and maybe some OKRs that stopped being relevant two quarters ago.

A charter is not a team page. A charter is a contract between the data organization and the rest of the company. It answers four questions:

**What do we own?** List every function, every system, every standard. If the data department does not own the data catalog, say so -- and name who does.

**What authority do we have?** Can the data team block a product launch if data quality standards are not met? Can they reject a dashboard request that uses undefined metrics? If the answer is no, your data department is a service desk, not a strategic function.

**What do we owe the business?** SLAs. Response times. Deliverable cadences. A charter without commitments is a wish list.

**How do we measure ourselves?** Not vanity metrics. Not "number of dashboards created." Real measures: data freshness, pipeline reliability, model performance in production, time from question to answer.

## Career Paths That Keep People

The fastest way to lose your best data engineer is to give them no path forward except "become a manager." The fastest way to lose your best analyst is to cap them at Senior Analyst with nowhere to go.

A real data department builds two tracks: an individual contributor track and a management track. They run in parallel, with equivalent compensation bands. A Staff Data Engineer and a Data Engineering Manager should be peers, not a subordinate and a boss.

This is not generosity. This is retention economics. Replacing a senior data engineer costs six to nine months of salary when you factor in recruiting, onboarding, and lost productivity. Building a career ladder costs a few hours of thoughtful organizational design.

## What to Do Monday Morning

1. **Audit your org chart.** Count every person with "data" in their title. Map who they report to. If they report to more than two different leaders with no shared data authority above them, you have a scattering problem. Name it.

2. **Draft a one-page charter.** Answer the four questions: What do we own? What authority do we have? What do we owe the business? How do we measure ourselves? Do not aim for perfection. Aim for a document you can put in front of your CEO and say, "This is what the data organization is accountable for."

3. **Publish your career ladder.** If your data professionals cannot see the next two roles ahead of them -- both as ICs and as managers -- build that document this week. Share it with your team. The ones who were quietly interviewing elsewhere might stop.

---

Book drops Q3 2026. Subscribe for early access and exclusive chapters not in the published version. Every Monday and Thursday, I am serializing "Data Is The New Oil" right here -- frameworks you can use before the book even ships.

---

## X Post (publish same day)

**Post:**
"You don't have a data department. You have data people scattered across the org chart reporting to VPs who treat them as personal resources. That structure guarantees failure."

**Reply:**
New post from the Data Is The New Oil series -- the blueprint for a data department that actually works. Charter template included. Read it here: [Substack link]

---

## YouTube Short Script

**[HOOK -- 0:00-0:15]**
Pull up your company's org chart right now. Find the word "data." Now trace the reporting lines. If your data people report to three different VPs with no shared authority above them -- you do not have a data department. You have scattered analysts. And that structure is why your AI initiatives keep failing.

**[BODY -- 0:15-0:50]**
I have seen this in companies with 60 analysts and a dozen data engineers. Marketing builds one definition of "active customer." Finance uses another. Product's pipeline captures half the user behavior because nobody told them about the mobile app. Everyone does reasonable work in isolation. The organization gets chaos. A real data department owns five functions under one leader: engineering, governance, analytics, data science, and strategy. And it has a charter -- a contract with the business that defines what it owns, what authority it has, and how it measures itself.

**[CTA -- 0:50-1:05]**
I break down the full charter template and career path framework in this week's post on Substack. Link in bio. The book drops Q3 2026 -- subscribe so you do not miss it.
