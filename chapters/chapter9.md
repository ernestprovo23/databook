# Chapter 9: Case Studies by Sector



Every framework in this book rests on a claim: organizational design determines AI outcomes more than technology does. That claim is only worth something if it holds up in the real world, across industries with different constraints, different data, and different stakes. This chapter puts it to the test.



We have spent eight chapters building the case for why governance, quality, and operating model matter more than any algorithm or platform. We have discussed maturity models, team structures, data quality dimensions, regulatory frameworks, and the economics of private AI. All of that is necessary. But theory without evidence is just opinion with better formatting.



What follows are nine case studies drawn from manufacturing, retail, media, insurance, finance, and the graveyard of high-profile failures. Some of these organizations got it right. Others lost hundreds of millions of dollars. The difference was rarely the algorithm. It was almost always the foundation underneath it: data quality, governance, operating model, and the willingness to treat data as infrastructure rather than an afterthought.



Read these stories with a pattern in mind. In every success, you will find the same ingredients we have discussed throughout this book: clean data, clear ownership, domain expertise embedded in the process, and governance that enabled speed rather than blocking it. In every failure, you will find at least one of those ingredients missing. The sector changes. The lesson does not.



## 9.1 Manufacturing: Siemens and the Predictive Maintenance Revolution



There is a moment in every factory when a machine stops. Not gradually, not with warning, but suddenly, in the middle of a shift, with parts half-finished on the line and workers standing idle. Unplanned downtime is one of the most expensive problems in manufacturing. It does not just cost money in lost production. It cascades. Missed delivery windows. Expedited shipping to compensate. Overtime labor to catch up. Damaged relationships with customers who needed those parts yesterday.



Siemens understood this problem intimately, because they were both the manufacturer and the technology provider trying to solve it. Their approach was not to build a smarter machine. It was to build a smarter relationship with the data those machines already produced.



Working with Senseye, a predictive maintenance platform, Siemens deployed AI-driven monitoring across their manufacturing operations. The system ingested sensor data from equipment on the factory floor, processed it at the edge, and identified patterns that preceded failure. Not the obvious ones, like a motor running hot, but the subtle signatures that human operators could not detect: slight vibration shifts, micro-fluctuations in power draw, patterns that only emerged when you analyzed thousands of operating hours across dozens of machines simultaneously.



The result was a 50% reduction in unplanned downtime. [SRC-01] That number alone would justify the investment. But the deeper story is about what made it possible.



First, Siemens started with data quality at the sensor level. This sounds obvious, but most manufacturing AI projects skip this step. They install sensors, connect them to a cloud platform, and expect the model to sort out the noise. Siemens did the opposite. They invested in calibrating sensors, establishing baseline readings, and building data validation directly into the ingestion pipeline. Before the AI ever saw a data point, that data point had already passed a quality gate. This is Chapter 5's data quality mandate in action, applied at the edge.



Second, they bridged the IT/OT gap. In manufacturing, there is a persistent divide between information technology, the enterprise systems that run the business, and operational technology, the industrial controls that run the factory floor. These two worlds speak different languages, use different protocols, and are managed by different teams who rarely share a hallway, let alone a strategy. Siemens built an integration layer that translated between them, ensuring that sensor data from the factory floor could flow into enterprise analytics without losing context or fidelity.



Third, and this is the part most organizations overlook, they built explainable models that operators actually trusted. A predictive maintenance system is useless if the person on the factory floor ignores its recommendations. Siemens designed their system to show operators not just what it predicted, but why. When the system flagged a compressor for inspection, it could point to the specific sensor readings and the historical pattern that triggered the alert. The operators did not have to take the AI's word for it. They could verify the reasoning and make an informed decision.



The lesson from Siemens is not about predictive maintenance specifically. It is about the integration pattern. Manufacturing AI succeeds when it bridges the gap between operational technology and information technology, when it respects the domain expertise of the people closest to the process, and when it treats data quality as the foundation, not a feature. Strip away the industry context, and you are looking at the same principles from Chapter 3's operations maturity model. Siemens operated at Level 4: automated pipelines, continuous monitoring, and governance integrated into the workflow. Most of their competitors were still at Level 1 or 2, collecting data they never used.



## 9.2 Retail: Walmart's Supply Chain Transformation



Walmart moves more physical goods than almost any company on Earth. Their supply chain is a machine of staggering complexity: thousands of suppliers, millions of products, 4,700 stores in the United States alone, and an e-commerce operation that has grown from afterthought to strategic pillar. Managing that system with spreadsheets and intuition stopped being viable a long time ago. What Walmart did with data and AI is one of the most consequential supply chain transformations in retail history.



The headline number is a 20% reduction in unit costs through AI-optimized supply chain and supplier negotiations. [SRC-02] That sounds clean and simple. It was neither.



Walmart's challenge was fragmentation. Their data lived in silos. Store-level inventory systems did not talk fluently to e-commerce fulfillment platforms. Supplier data came in dozens of formats. Customer behavior looked different depending on whether you measured it in a parking lot in Arkansas or on a smartphone in Brooklyn. Before Walmart could optimize anything with AI, they had to solve a data integration problem that would have been familiar to any reader of Chapter 5.



The breakthrough came with Walmart Luminate, their data and analytics platform that opened Walmart's behavioral and transactional data to suppliers. Luminate did not just provide dashboards. It created a closed-loop system where suppliers could see how their products performed at the shelf level, understand why certain items moved and others did not, and adjust their strategies in near real time. The results were dramatic: 75% e-commerce revenue growth and 50% supplier network growth for the platform. [SRC-03]



What made Luminate work was not the technology. It was the strategic decision to treat data as a shared asset across the entire supply chain, rather than hoarding it as a competitive weapon. Walmart recognized that when their suppliers made better decisions, Walmart's shelves were stocked more efficiently, waste went down, and customers found what they wanted more often. Data sharing created a flywheel: better supplier decisions led to better inventory, which led to better customer experience, which generated more behavioral data, which fed back into the system.



But the transformation was not without friction. Integrating e-commerce data with brick-and-mortar data required reconciling fundamentally different measurement systems. An online click and an in-store purchase tell you different things about the same customer. Walmart invested heavily in identity resolution and behavioral modeling to stitch those signals together into a coherent picture. They also had to navigate the tension between personalization and privacy. The more you know about a customer, the better you can serve them, but also the more you owe them in terms of transparency and consent. Walmart's governance framework, built before the personalization engine, not after, gave them the guardrails to move fast without stumbling into the privacy failures that have damaged other retailers.



The lesson from Walmart is about connectivity. Retail wins when data connects the entire chain, from supplier to shelf to customer and back again. An isolated optimization, improving warehouse routing without understanding demand signals, or personalizing the website without connecting to store inventory, delivers incremental gains at best. The compounding value comes from closing the loop. This is the data flywheel from Chapter 8 made tangible: proprietary data, fed into models that serve the business, generating more proprietary data, creating an advantage that compounds over time.



## 9.3 Media: Netflix and the $1 Billion Algorithm



Netflix saves approximately $1 billion per year through its recommendation system. [SRC-04] That figure is worth pausing on. Not because it is large, though it is, but because of what it reveals about what happens when data becomes the product experience itself.



Roughly 80% of what Netflix subscribers watch comes from algorithmic recommendations, not from browsing or searching. [SRC-05] The majority of the time, the viewer does not choose what to watch. The model chooses for them, and they agree. That is not a feature bolted onto a streaming service. That is the streaming service. Without that recommendation engine, Netflix estimated that subscribers would lose interest and cancel at a rate that would cost the company over a billion dollars annually in lost revenue.



The key driver behind this outcome is quality behavioral data at massive scale. Every interaction on the platform generates signal: what you watched, when you paused, when you skipped the intro, when you abandoned a show after seven minutes, when you rewatched a scene. Netflix does not just track what you chose. They track the context of the choice, the time of day, the device, what you watched before, how long you deliberated on the browse screen. This behavioral data, billions of signals per day, feeds models that learn not just what you like, but what you are likely to want right now, in this moment, on this evening, in this mood.



What Netflix got right was treating recommendation as core infrastructure rather than a product feature. Most media companies build a content library and then add a recommendation layer on top, like frosting on a cake. Netflix designed the cake around the recommendation engine. Their content acquisition strategy, their thumbnail design, their user interface, even their decision about which original shows to produce, all feed from and feed into the same behavioral data system. The recommendation engine is not a department at Netflix. It is the architecture.



This approach created a defensible competitive advantage that competitors have struggled to replicate. Disney, HBO, Amazon, and Apple have all entered the streaming market with massive content budgets and technical talent. They can license the same movies and shows. They can build a similar streaming interface. They can hire the same engineers. But they cannot replicate fifteen years of behavioral data from 200 million subscribers. That data is proprietary, compounding, and irreplaceable. Every day Netflix operates, the advantage grows. It is the definition of the data flywheel from Chapter 8, and it is the clearest illustration in this book of what happens when data becomes a moat rather than a byproduct.



But the Netflix story also carries a warning. Engagement models optimized without guardrails can create perverse outcomes. When the algorithm's only objective is maximizing watch time, it can push viewers toward content that is addictive rather than satisfying, sensational rather than substantive. Netflix has faced criticism for optimizing engagement metrics at the expense of content diversity, and the broader industry has grappled with similar questions about what happens when algorithms shape culture without accountability.



The lesson from Netflix is twofold. First, when data is the product experience, quality becomes existential. A 2% improvement in recommendation accuracy translates directly into retention, revenue, and competitive position. Second, scale without governance creates its own risks. The same system that saves a billion dollars can erode trust if it operates without transparency about how and why it makes recommendations. Chapter 6's governance imperative applies just as forcefully to a recommendation engine as it does to a medical device.



## 9.4 Healthcare: Data, Governance, and Life-or-Death Stakes



Healthcare is where data quality and governance collide with real human outcomes. The cost of a bad model is not just financial. It is clinical.



Mount Sinai’s readmission work shows what happens when data is brought together at scale. Researchers built EMR‑wide heart‑failure readmission models using thousands of variables across diagnoses, medications, labs, and procedures. [SRC-12] The point is not the model alone. It is that clinical, operational, and administrative data were reconciled into a usable system, which is a data quality victory before it is an AI victory.



Another example is HCA Healthcare and Google Cloud’s National Response Portal, built to manage hospital capacity and supplies during COVID-19. The platform pulled data from thousands of facilities into a single, operational view for governments and healthcare systems. [SRC-13] It was a data‑sharing and governance achievement disguised as a technology sprint.



Hackensack Meridian Health took a similar approach, working to unify data across the organization to improve clinical and operational decision‑making. [SRC-14] The case illustrates a recurring pattern: healthcare AI performs best when the data platform is treated as clinical infrastructure, not just IT infrastructure.



These examples reinforce the same principle: in healthcare, the data platform is as critical as the care model. If you cannot trust the data, you cannot trust the decisions.



## 9.5 Insurance and Finance: Progressive, JPMorgan, and Mastercard



### Progressive Snapshot: Turning Driving Data into a Business



In 2008, Progressive Insurance introduced Snapshot, a small device that plugged into a car's diagnostic port and recorded driving behavior: speed, braking patterns, time of day, miles driven. The premise was simple. Instead of pricing auto insurance based on demographics and credit scores, which are proxies for risk, why not price it based on actual driving behavior, which is risk itself?



The device generated a stream of operational data that Progressive had never had access to before. And what they discovered was that the data was worth far more than just better pricing. Safe drivers, validated by Snapshot data, could receive discounts. That was the initial value proposition. But the aggregate data, millions of driving profiles across different geographies, vehicle types, and conditions, became a product in its own right. Progressive could identify risk patterns that no actuarial table had ever captured. They could model accident likelihood with a granularity that transformed their underwriting. [SRC-16]



The result was not just better pricing. It was a new revenue stream. Snapshot turned operational data, the kind of data most companies collect and ignore, into a strategic asset that generated direct business value. Progressive did not need a breakthrough in AI to make this work. They needed the organizational clarity to recognize that the data they were collecting for one purpose could serve another, and the governance framework to do it responsibly.



The lesson from Progressive is deceptively simple: data monetization works when it creates value for the customer too. Drivers who opted into Snapshot got lower premiums. Progressive got better risk models and a new product line. The exchange was transparent and mutually beneficial. When data monetization feels extractive, when the company captures all the value and the customer gets nothing, trust collapses. Progressive avoided that trap by designing the program around shared benefit from the start.



### JPMorgan COiN: Automation at Scale



JPMorgan Chase’s Contract Intelligence (COiN) program used machine learning to automate contract review, a task that had previously required large teams of lawyers and operations staff. Reports estimate it saved roughly 360,000 hours of manual work each year. [SRC-15] This is a finance case study with a simple lesson: clear ownership and governance make it possible to deploy automation where the stakes are high and the documents are sensitive.



### Mastercard Advisors: When Your Data Is Worth More to Others



Mastercard processes billions of transactions every year. For decades, the value of that data was internal: fraud detection, network optimization, risk management. Then someone at Mastercard asked a different question. What if the aggregate patterns in our transaction data were more valuable to other businesses than they are to us?



That question became Mastercard Advisors, a consulting arm that packages anonymized, aggregated transaction insights and sells them to retailers, governments, and financial institutions. A retailer could use Mastercard's data to understand foot traffic patterns, spending trends, and competitive dynamics in ways that their own point-of-sale data could never reveal. A city government could use it to measure economic recovery after a natural disaster. The data was the same. The packaging made it transformative. [SRC-07]



What Mastercard recognized was a principle that applies across industries: sometimes your data is worth more to others than to you, if you can package it. The raw transaction data was useful internally. But the patterns, the aggregated view of consumer behavior across millions of merchants and hundreds of countries, that was a product. Mastercard did not sell individual transactions. They sold the intelligence that emerged from the aggregate. The distinction is critical. It protected consumer privacy, satisfied regulatory requirements, and created a high-margin consulting business that complemented rather than cannibalized their core payment processing revenue.



The lesson from Mastercard connects directly to Chapter 1's profit center transformation. Data departments are not cost centers when the data they manage can be productized. But productization requires three things: the governance to handle data responsibly, the analytical capability to extract meaningful patterns, and the business development acumen to find buyers who will pay for those patterns. Most organizations have the data. Few have all three capabilities. That is the gap.



## 9.6 When It Goes Wrong: Four Cautionary Tales



Success gets the headlines, but failure teaches the lessons. The four cases that follow are not obscure footnotes. They are some of the most expensive, most public, and most preventable data failures in recent history. Each one connects directly to the frameworks we have built throughout this book. Each one could have been avoided with the foundations described in earlier chapters.



### NASA Mars Climate Orbiter: A $125 Million Unit Conversion Error



On September 23, 1999, the Mars Climate Orbiter entered the Martian atmosphere at the wrong angle and disintegrated. The spacecraft, which had traveled 416 million miles over nine months, was destroyed in seconds. The cost: $125 million. [SRC-08]



The root cause was almost absurdly simple. One engineering team, at Lockheed Martin, had written software that calculated thruster force in imperial units (pound-force seconds). Another team, at NASA's Jet Propulsion Laboratory, expected those values in metric units (newton-seconds). Nobody caught the discrepancy. For months, the spacecraft's trajectory was being adjusted based on numbers that were off by a factor of 4.45. Each correction pushed the orbiter slightly closer to disaster. By the time anyone noticed, it was too late.



This was not a failure of artificial intelligence. There was no machine learning involved. It was a failure of data quality in its most elementary form, the kind described in Chapter 5's Seven Dimensions. Specifically, it was a failure of Consistency, making sure the same measurement means the same thing across systems, and Validity, ensuring data conforms to expected formats and rules. A validation gate that checked unit conventions at the interface between the two teams would have caught this error. It would have cost almost nothing to implement. Its absence cost $125 million and years of scientific work.



The lesson is uncomfortable precisely because it is so basic. If a $125 million spacecraft can be destroyed by a unit conversion error, what is happening in your data pipelines right now? Most organizations do not have the validation gates to catch this kind of mismatch. They rely on convention, on the assumption that everyone is speaking the same language. The Mars Climate Orbiter is proof that assumption is not a quality strategy. Quality is not optional. It is the price of admission.



### Unity Audience Pinpoint: When Bad Data Meets Scale



In 2022, Unity Technologies disclosed a $110 million revenue impact tied to problems with its Audience Pinpoint tool, which used machine learning to target mobile advertising. [SRC-09] The tool was supposed to match ads to users based on behavioral data, optimizing ad spend for Unity's customers. Instead, it ingested bad training data, and the models trained on that data made poor targeting decisions at scale.



The mechanics were straightforward. Audience Pinpoint relied on signals from Apple's ecosystem, and when Apple tightened its privacy controls with iOS 14.5, the data flowing into Unity's models changed in ways the system was not prepared to handle. The training data no longer accurately represented user behavior. But the models kept running, kept targeting, kept spending advertisers' money, now based on degraded inputs that produced degraded outputs.



Unity did not lose $110 million because their algorithm was bad. They lost it because the data feeding that algorithm was bad, and they had no quality monitoring in place to catch the degradation before it compounded. This is Chapter 5's multiplication effect made painfully real: bad data multiplied by AI scale equals catastrophic outcomes at speed. A human media buyer making poor decisions might waste thousands of dollars before someone noticed. An automated system making the same poor decisions, millions of times per day, can burn through $110 million before the quarterly report lands.



The lesson is about monitoring as much as it is about quality. Even if your data is clean at launch, it will not stay clean. External changes, regulatory shifts, platform policy updates, changes in user behavior, can degrade your inputs without warning. If you do not have continuous monitoring in place, the kind described in Chapter 3's MLOps maturity framework, you will not know your model is failing until the financial damage is already done. The bigger the model, the more damage bad data does. Scale is an amplifier. It amplifies success, but it amplifies failure just as efficiently.



### United Healthcare AI Claims: Innovation Without Governance



In 2023, United Healthcare faced a lawsuit alleging that its AI-driven claims processing system was denying legitimate medical claims without adequate human review. [SRC-10] The system, designed to streamline the claims adjudication process, was making coverage decisions that directly affected patients' access to care. When those decisions were wrong, and they were wrong often enough to trigger legal action, the consequences were not abstract. Real people were denied coverage for medical procedures they needed.



The root cause was not a malfunctioning algorithm. The algorithm was doing exactly what it was designed to do: process claims faster and more consistently than human reviewers. The problem was that the system was deployed without the governance infrastructure to ensure its decisions were fair, explainable, and subject to meaningful human oversight. There was no adequate appeals process for AI-generated denials. There was no transparency about how the system weighed different factors. There was no governance framework that asked the fundamental question: should an algorithm be making this decision at all without a human in the loop?



This failure connects directly to two of this book's core frameworks. Chapter 6's governance imperative argues that regulation is not a brake on innovation but a competitive advantage when done right. United Healthcare skipped that step. They deployed a system that touched people's health and money without building the audit trails, the explainability requirements, or the human oversight mechanisms that healthcare AI demands. Chapter 2's ownership vacuum is visible here too. When no single leader owns the governance of an AI system, the system operates in the gap between what technology can do and what the organization should allow it to do.



The lesson is stark. When AI touches people's health and money, governance is not optional. It is the difference between innovation and litigation. The technology worked. The organization around it did not. And in healthcare, where the stakes are literally life and death, that organizational failure is not just expensive. It is unconscionable.



### Google Flu Trends: The Model That Could Not Explain Itself



In 2008, Google launched Flu Trends, a system that used search query data to predict flu outbreaks faster than the CDC's traditional surveillance methods. For a few years, it seemed to work. The press was enthusiastic. Public health officials were intrigued. Google had demonstrated, apparently, that the right data and the right model could outpace traditional epidemiology.



Then it fell apart. By 2013, Google Flu Trends was consistently overestimating flu prevalence, sometimes by more than double the CDC's confirmed numbers. [SRC-11] The model, which had been lauded as a breakthrough, became a cautionary tale cited in statistics courses and AI ethics papers around the world.



What went wrong was a cascade of the problems this book has been describing. The model relied on search queries as a proxy for flu activity. But search behavior is noisy. People search for flu symptoms when they have a cold, when they are worried about someone else, when the news runs a story about a bad flu season, or when a flu-related topic trends on social media. The model could not distinguish between someone who was sick and someone who was scared. It treated all signals as equivalent, and as media coverage of flu season intensified, the model's predictions inflated with it.



Worse, the model was a black box. When its predictions diverged from reality, nobody could explain why. There was no mechanism to identify which signals were driving the overestimation, no way to isolate the bias, and no process for recalibrating the model against ground truth. The system could not explain itself, and when stakeholders lost confidence in its outputs, there was nothing to point to except the gap between prediction and reality.



This failure maps to Chapter 3's discussion of Explainable AI and Chapter 5's Relevance dimension. The data Google used was not relevant to the task in the way the model assumed. Search queries correlate with flu activity, but correlation is not causation, and when the correlation breaks down, an unexplainable model cannot tell you why. The absence of explainability did not just cause a technical failure. It caused a trust failure. Public health officials who had begun to rely on Flu Trends had to abandon it, and the broader credibility of AI in public health took a hit that lasted years.



The lesson is about humility and transparency. When you cannot explain why your model is wrong, you cannot fix it. And when stakeholders, whether they are public health officials, executives, or customers, lose trust in your model's outputs, rebuilding that trust is far more expensive than building explainability in from the start. Google eventually shut down Flu Trends in 2015. The data was still there. The compute was still there. But the trust was gone, and without trust, the system had no value.



Confidence without transparency is not intelligence. It is guessing with expensive hardware.



## 9.7 The Pattern Across Sectors



Nine case studies. Five sectors. Five successes and four failures. The surface details are wildly different. Sensor data on a factory floor has nothing in common with search queries about flu symptoms. A recommendation algorithm at Netflix solves a different problem than a claims adjudication system at a health insurer. The regulatory environment for insurance has little overlap with the regulatory environment for mobile advertising.



And yet, the pattern underneath is remarkably consistent.



Every success story in this chapter shares the same foundation. Siemens invested in data quality before deploying models. Walmart connected data across organizational silos to create a closed-loop system. Netflix treated data as core infrastructure, not a feature. Progressive and Mastercard recognized that operational data could become a product. In each case, the technology was necessary but not sufficient. What made it work was the organizational design around the technology: clear ownership, quality gates, governance frameworks, and a willingness to integrate data into the business model rather than running it as a side project.



Every failure story shares a different pattern, one defined by absence. NASA lacked validation gates between teams. Unity lacked continuous monitoring of input data quality. United Healthcare lacked governance and human oversight for a high-stakes AI system. Google lacked explainability in a model that stakeholders needed to trust. In each case, the technology performed as designed. It was the organizational infrastructure, the part that does not make the demo reel, that was missing.



The frameworks from earlier chapters map directly onto these outcomes:



| Framework | Success Pattern | Failure Pattern |

|-----------|----------------|-----------------|

| Data Quality (Ch 5) | Quality gates at ingestion; sensor-level calibration | No validation; degraded inputs undetected |

| Governance (Ch 6) | Governance built before deployment; audit trails | No oversight; autonomous decisions in high-stakes domains |

| Operations Maturity (Ch 3) | Continuous monitoring; human-in-the-loop | Frozen or unmonitored models; no feedback loops |

| Organizational Design (Ch 2) | Clear ownership; IT/OT integration; cross-functional teams | Siloed teams; ownership vacuums; no accountability |



The implication for your organization is not that you need to replicate Walmart's supply chain or Netflix's recommendation engine. It is that you need the same foundations they built before the AI ever mattered: clean data, clear ownership, continuous monitoring, and governance that keeps pace with the technology. The sector shapes the execution. It does not change the requirements.



There is one more thing these case studies reveal, and it is worth stating plainly. The successes in this chapter were not accidents. They were the result of deliberate organizational choices made before the AI was deployed, not after. Siemens chose to invest in sensor calibration. Walmart chose to share data with suppliers. Netflix chose to make recommendations the architecture. Progressive and Mastercard chose to treat data as a product. These were not technology decisions. They were business decisions, made by leaders who understood what data could do and built organizations capable of doing it.



The failures were also the result of choices, or more precisely, the absence of them. Nobody at NASA chose to skip the unit validation. Nobody at Unity chose to ignore data quality monitoring. Nobody at United Healthcare chose to deploy an ungoverned system. These gaps emerged because the organizational infrastructure to prevent them did not exist. When nobody owns the decision, the decision does not get made. And when the decision does not get made, the default is failure.



If this chapter has done its job, you should be able to look at your own organization and ask: which pattern are we following? The one that leads to Siemens, or the one that leads to NASA? The answer is not about your technology stack. It is about your organizational design. It always has been.



In the final chapter, we turn from diagnosis to action, building the roadmap that takes these lessons from case study to execution.



## Sources (Draft)

Format: [SRC-##] Claim. Source. Status. Use `2025_data_sources.md` where applicable; otherwise mark as external.

[SRC-01] Claim: Siemens achieved 50% downtime reduction through AI-driven predictive maintenance (Senseye). Source: `2025_data_sources.md` (Strategic Report, Case Study Compendium). Verify exact citation.

[SRC-02] Claim: Walmart achieved 20% unit cost cut through AI-optimized supply chain and supplier negotiations. Source: `2025_data_sources.md` (Strategic Report, Case Study Compendium). Verify exact citation.

[SRC-03] Claim: Walmart Luminate drove 75% e-commerce revenue growth and 50% supplier network growth. Source: `updated_book_outline_v2.md` (Section 1.4). Verify exact citation.

[SRC-04] Claim: Netflix saves approximately $1 billion annually from its recommendation system. Source: `2025_data_sources.md` (Strategic Report, Case Study Compendium). Verify exact citation.

[SRC-05] Claim: 80% of Netflix consumption is driven by algorithmic recommendations. Source: `2025_data_sources.md` (Strategic Report, Case Study Compendium). Verify exact citation.

[SRC-06] Claim: Progressive Snapshot created a new revenue stream from driving data monetization. Source: `updated_book_outline_v2.md` (Section 1.4). Verify exact citation.

[SRC-07] Claim: Mastercard Advisors turned transaction data into a consulting business. Source: `updated_book_outline_v2.md` (Section 1.4). Verify exact citation.

[SRC-08] Claim: NASA Mars Climate Orbiter loss cost $125 million due to imperial/metric unit mismatch. Source: `2025_data_sources.md` (Strategic Report, Case Study Compendium). Verify exact citation.

[SRC-09] Claim: Unity Technologies suffered $110 million loss from poor input data in Audience Pinpoint. Source: `2025_data_sources.md` (Strategic Report, Case Study Compendium). Verify exact citation.

[SRC-10] Claim: United Healthcare faced lawsuit over AI claims system deployed without adequate governance. Source: External (news coverage, 2023). Verify exact citation.

[SRC-11] Claim: Google Flu Trends consistently overestimated flu prevalence, sometimes by more than double CDC figures. Source: External (Lazer et al., "The Parable of Google Flu," Science, 2014). Verify exact citation.

[SRC-12] Mount Sinai EMR‑wide heart‑failure readmission modeling study. PubMed / PSB proceedings. External.

[SRC-13] HCA Healthcare + Google Cloud National Response Portal case study. Google Cloud case study. External.

[SRC-14] Hackensack Meridian Health data platform case study. Google Cloud case study. External.

[SRC-15] JPMorgan Chase COiN contract intelligence program saving ~360,000 hours annually. Independent / press reporting. External.

[SRC-16] Progressive Snapshot usage‑based insurance program overview. Progressive corporate site. External.
