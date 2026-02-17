# Post 2: Why Data Is The New Oil (And Why That Analogy Falls Short)
**Publication date**: Wednesday, February 25, 2026
**Source**: Chapter 1
**URL slug**: /data-is-the-new-oil-analogy

---

In 2006, Clive Humby said "data is the new oil." Twenty years later, that phrase shows up in every pitch deck, every boardroom slide, every LinkedIn post from someone who has never operated a refinery or a data pipeline. And here is what nobody wants to say out loud: the analogy is breaking your strategy.

Oil sits in the ground and waits. It does not change composition while you build the rig. It does not degrade the moment you pump it. It does not require a human being to decide, every single day, whether it still means what it meant yesterday.

Data does all of those things.

I have spent ten years watching organizations pour millions into "data infrastructure" modeled on oil extraction logic. Extract, transform, load, done. Pipe it in, refine it, ship it out. And then they wonder why the AI they built on top of it produces garbage.

The metaphor got you in the door. Now it is time to walk through it.

## What the Metaphor Gets Right

Let me be clear about what the oil analogy earned. Data, like oil, is a raw material. It has to be processed before it becomes useful. It powers economic engines. It creates competitive advantages for those who control it. Humby was not wrong. He was incomplete.

The incompleteness is where the danger lives.

When you treat data like oil, you build extraction infrastructure. You build pipelines. You measure success by volume -- how many terabytes did we ingest this quarter? How many sources are connected? How fast can we move data from point A to point B? These are engineering questions, and they have engineering answers. Organizations are very good at answering engineering questions. That is not where they fail.

They fail at the part the oil metaphor cannot account for: data requires continuous human judgment to remain valuable.

## Where the Metaphor Breaks Down

Oil does not decay semantically. A barrel of crude pulled from the Permian Basin in January means the same thing in March. But a customer record from January? A market signal from Q1? A regulatory classification from last fiscal year? These things change meaning. They change meaning because the world around them changes, and data is a reflection of the world, not a substance independent of it.

This distinction is not academic. It determines whether your AI investment produces value or produces confident nonsense at scale.

I watched a Fortune 500 retailer spend eighteen months building what they called a "data lake." They had every right to be proud of the engineering. The pipelines were fast, the storage was cheap, the architecture was clean. They had extracted and loaded data from forty-seven internal systems. Textbook oil-metaphor execution.

Then they tried to build a demand-forecasting model on top of it. The model pulled product category codes from three different systems that each defined categories differently. One system had been decommissioned but was still feeding data. Two of the customer segmentation fields had been redefined during a CRM migration eighteen months earlier, and nobody had updated the data dictionary.

The model trained fine. It produced outputs. The outputs were wrong in ways that looked right, which is the most dangerous kind of wrong there is.

No amount of pipeline engineering would have caught that. What was needed was organizational judgment infrastructure -- people with the authority and context to say "this field no longer means what the schema says it means." People whose job it is to maintain the relationship between data and reality.

Oil does not need that. Data does.

## The Extraction Trap

Here is the second failure of the oil metaphor: it implies that extraction is the hard part. With oil, that is arguably true. Finding it, drilling it, pulling it out of the ground -- that is where most of the capital goes. Once you have it, refining it is a known, repeatable, industrial process.

With data, extraction is the easy part. Your systems are already producing data constantly. The hard part -- the part that determines whether your AI strategy succeeds -- is governance, quality, context, and ownership. Who decides what this data means? Who is accountable when it changes? Who has the authority to say "this source is no longer trustworthy"?

These are not engineering questions. They are organizational design questions. And the oil metaphor gives you zero language for them.

## The Moat Is Not What You Think

The third failure is the moat assumption. Companies hoard data the way they would hoard oil reserves, assuming that more data equals more competitive advantage. But data without context is not an asset. It is a liability -- storage costs, compliance risk, attack surface, and technical debt, all growing while the data sits there losing relevance.

The competitive moat in data is not volume. It is the organizational capability to turn data into accurate, timely, contextual decisions. That capability lives in people, processes, and governance structures. Not in pipelines.

| Characteristic | Oil | Data |
|---|---|---|
| **Ownership** | Clear title, mineral rights, legal frameworks established over a century | Fragmented across departments, vendors, and jurisdictions; ownership often undefined |
| **Decay Rate** | Stable for millions of years; does not lose composition | Decays semantically in weeks or months; meaning shifts as business context changes |
| **Human Judgment Requirement** | Minimal once refining process is established | Continuous; requires human context to validate meaning, quality, and relevance |
| **Infrastructure Type** | Physical: rigs, pipelines, refineries (capital-intensive, build-once) | Organizational: governance, roles, accountability, data dictionaries (ongoing, never "done") |
| **Competitive Moat** | Volume of reserves and control of supply chain | Quality of judgment infrastructure and speed of context-aware decision-making |
| **Failure Mode** | Spill, shortage, price volatility | Confident wrong answers at scale, compliance violations, eroded trust |
| **Scaling Model** | More extraction = more value (generally) | More data without governance = more liability and noise |

## What to Do Monday Morning

1. **Audit your "data lake" for semantic decay.** Pick your three most critical data sources. For each one, ask: when was the last time a human verified that the field definitions in the schema match what the data actually represents today? If nobody can answer that question, you do not have a data asset. You have a storage bill.

2. **Assign data ownership to people, not systems.** Every critical dataset needs a named human being -- not a team, not a Slack channel, a person -- who is accountable for its accuracy, timeliness, and meaning. If your org chart does not have these roles, your AI strategy has no foundation.

3. **Stop measuring data success by volume.** Replace "how much data do we have?" with "how much of our data can we certify as accurate and contextually current right now?" That number is your real data asset. Everything else is overhead.

---

Book drops Q3 2026. Subscribe for early access and exclusive chapters not in the published version. Every Monday and Thursday, I am serializing "Data Is The New Oil" right here -- frameworks you can use before the book even ships.

---

## X Post (publish same day)

**Post:**
"Data decays. Oil doesn't. That single difference is why your AI strategy is failing and your data lake is becoming a data swamp. The oil metaphor got you in the door. Now it's time to walk through it."

**Reply:**
New on Substack: Why the "data is the new oil" analogy is actively breaking enterprise AI strategies -- and what to replace it with. Free read: [Substack link]

---

## YouTube Short Script

**[HOOK -- 0:00-0:15]**
"Data is the new oil." You have heard that a hundred times. Here is what nobody tells you: that metaphor is destroying your AI strategy. I have spent ten years watching it happen.

**[BODY -- 0:15-0:50]**
Oil sits in the ground. It does not change. A barrel of crude means the same thing today as it did last year. Data? Data decays. A customer record from six months ago might already be wrong. A product category code might have been redefined in a system migration nobody documented. And when you build AI on top of data that has silently changed meaning, you do not get bad outputs. You get confident bad outputs. That is worse.

The oil metaphor tells you to build pipelines. What you actually need is judgment infrastructure. People with the authority to say "this data no longer means what the schema says it means."

**[CTA -- 0:50-1:00]**
I break this down in my new Substack series from my upcoming book "Data Is The New Oil." Link in bio. Subscribe for early access to chapters before publication.
