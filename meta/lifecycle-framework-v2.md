# AI-PM Craft Lifecycle Framework (v2)

## Overview

This framework organizes AI-augmented product management knowledge across six phases. Each phase maps intuitively (without a lookup table) to a common enterprise product development lifecycle, while drawing its vocabulary and conceptual grounding from widely-recognized PM thought leaders. The phase names are chosen to be **evocative synonyms** — close enough in meaning to map instantly, distinct enough to carry their own lineage and nuance.

| # | This Framework | Enterprise Analog | Core Question |
|---|---|---|---|
| 1 | **Discover** | Identify | *What problems are worth solving?* |
| 2 | **Frame** | Define | *What does success look like, and what's the bet?* |
| 3 | **Shape** | Design | *What solution takes form, and for whom?* |
| 4 | **Build** | Deliver | *How do we ship with clarity and conviction?* |
| 5 | **Release** | Launch | *How do we put this into the world deliberately?* |
| 6 | **Measure** | Learn | *Did it work, and what do we do next?* |

---

## Phase 1: DISCOVER

**Core question:** *What problems are worth solving?*

### Phase Lineage

This phase synthesizes two foundational traditions: **Teresa Torres' Continuous Discovery Habits** and **Marty Cagan's Discovery Track** (SVPG Dual-Track Agile).

Torres made the definitive case for continuous, structured problem discovery as a discipline unto itself. Her Opportunity Solution Tree (OST) starts with a desired business outcome and maps customer needs hierarchically beneath it, ensuring every problem the team pursues connects to a measurable goal. She defines the core unit of discovery as the **opportunity** — "an unmet customer need, pain point, or desire... an opportunity to positively impact our customers" ([producttalk.org](https://www.producttalk.org/opportunity-solution-trees/)). Her keystone habit is **weekly customer interviews**: "A weekly habit is easier to maintain and keeps you agile" (*Continuous Discovery Habits*, 2021). Her more recent work with Aakash Gupta ([news.aakashg.com](https://www.news.aakashg.com/p/teresa-torres-podcast)) demonstrates how AI accelerates synthesis — creating "interview snapshots" and opportunity clusters — while keeping human judgment at the center of prioritization.

Cagan's contribution is the **Opportunity Assessment**, a lightweight alternative to full PRDs that forces teams to answer ten questions before committing to a solution. The critical ones for this phase: *"Exactly what problem will this solve? For whom do we solve that problem? How big is the opportunity? How will we measure success?"* ([svpg.com](https://svpg.com/assessing-product-opportunities/)). Cagan also coined the term **"Opportunity Backlog"** (with Jeff Patton) as a replacement for the traditional product roadmap — a prioritized list of problems to explore, not features to build ([svpg.com](https://www.svpg.com/the-opportunity-backlog/)).

The first diamond of the **Double Diamond** (Design Council, 2005/2019) provides the structural shape: diverge broadly in research (Discover), then converge on the right problem to solve (Define). Our Discover phase corresponds to that first divergent move.

### Components

| Component | Description | Enterprise Analog |
|---|---|---|
| **Problem Signal Detection** | Detecting unmet needs, emerging pain points, and weak signals from usage data, support tickets, sales conversations, and direct customer contact. Torres' "weekly customer interviews" as a keystone habit; Cagan's emphasis on observing customer misbehavior as a discovery technique. | Customer problem statement identification |
| **Market & Competitive Intelligence** | Competitive analysis, market sizing, technology trend monitoring, and adjacent-market scanning. Cagan's Opportunity Assessment questions 3–6: *"How big is the opportunity? What alternatives are out there? Why are we best suited? Why now?"* ([svpg.com](https://svpg.com/assessing-product-opportunities/)) | Market/competitive research |
| **Opportunity Prioritization** | Managing and ranking the space of possible problems to solve. Torres' OST for hierarchical mapping; RICE or ICE scoring for backlog triage. Cagan and Patton's "Opportunity Backlog" reframes this as a prioritized list of *problems*, not features: "We want to make sure we solve the problem, even though we may have to try several different features or approaches" ([svpg.com](https://www.svpg.com/the-opportunity-backlog/)). | Manage/prioritize idea backlog |
| **Problem Brief** | A concise articulation of the problem worth solving, who it affects, and why now. Draws from Cagan's Opportunity Assessment (the ten questions) and Amazon's Working Backwards PR/FAQ. The output is a compelling "why" document — not yet a "what" or "how." | Product brief |

### AI-PM Emphasis

AI dramatically compresses **Problem Signal Detection** — automated review mining, support ticket clustering, usage anomaly detection, and sentiment analysis across channels. Torres describes AI as "a thought partner that extends your capacity" for synthesis, but stresses that pattern recognition in interviews still requires human presence ([news.aakashg.com](https://www.news.aakashg.com/p/teresa-torres-podcast)). **Market & Competitive Intelligence** benefits from AI-powered competitive monitoring and patent landscape analysis. The human premium is in **Opportunity Prioritization** — the judgment of which signals matter most given strategic context.

---

## Phase 2: FRAME

**Core question:** *What does success look like, and what's the bet?*

### Phase Lineage

This phase addresses the most significant structural gap in modern PM frameworks: **the formal commitment to success criteria before solution design begins.**

The strongest precedent is **Robert Cooper's Stage-Gate**, where Stage 2 is literally titled **"Build the Business Case"** — requiring "primary market research, VoC, technical feasibility studies, value proposition clarification, financial evaluation, and risk assessment" before a project can proceed to development. Cooper designed this as a formal gate: *"The key output is a robust business case, specifying the product definition, market positioning, financials, and a plan for the next Stage or Stages"* ([stage-gate.com](https://www.stage-gate.com/blog/the-stage-gate-model-an-overview/)). Stage-Gate has served as the dominant framework for managing new product development for over forty years.

**Melissa Perri's** *Escaping the Build Trap* (2018) provides the philosophical backbone for why this phase must exist. The "build trap" is *"when organizations become stuck measuring their success by outputs rather than outcomes"* — shipping features without knowing what success looks like. Her antidote is the **Product Kata** (adapted from Toyota Kata): understand the direction → analyze the current condition → **set the next target condition** → experiment. That "target condition" — a measurable future state — is exactly what Frame produces. Her litmus test: *"Raise your hand if you went back and iterated on the last thing you shipped... How do you know that what you shipped was successful?"* ([melissaperri.com](https://melissaperri.com/book))

**Reforge's Product Strategy Stack** (Ravi Mehta, Casey Winters, et al.) provides the vertical alignment model: Company Mission → Company Strategy → Product Strategy → Product Roadmap → Product Goals. Frame is where strategy gets translated into measurable product goals and sequenced roadmap commitments ([reforge.com](https://www.reforge.com/courses/mastering-product-management)).

**Pragmatic Institute's Framework** is the only major framework that treats both a "Business Case" activity *and* a "Performance and Analytics" activity as discrete, first-class responsibilities within the lifecycle — validating that this separation is both useful and widely taught ([pragmaticinstitute.com](https://www.pragmaticinstitute.com/product/framework/)).

### Components

| Component | Description | Enterprise Analog |
|---|---|---|
| **Stakeholder Intent Alignment** | Refining intent, securing sponsorship, and building shared understanding of the problem and its strategic importance. Cagan's emphasis on empowered teams requires explicit alignment on the *problem* before granting autonomy on the *solution*. Torres recommends using the OST itself as a stakeholder communication device: *"Your leader needs to trust that you can reach your outcome. You need to show you have a plan for how to get there"* ([producttalk.org](https://www.producttalk.org/getting-started-with-discovery/)). | Intent refinement with stakeholders |
| **Success Criteria & Business Case** | Defining the objective function: what KPIs will prove this worked? Financial modeling, PRED development, North Star metric selection, and guardrail metrics. This is Cooper's Stage-Gate "Build the Business Case" reimagined for continuous product development — lighter than a formal business case, but equally rigorous about defining measurable outcomes *before* committing resources. Perri's key principle: a feature isn't done when it ships — it's done when it achieves the desired outcome. | Business case documentation / PRED development |
| **Roadmap Definition** | Translating strategy into a time-aware plan. Outcome-based roadmapping (NOW/NEXT/LATER), strategic sequencing of bets, and explicit articulation of what is — and isn't — in scope. Reforge's Strategy Stack provides the vertical alignment; this is the horizontal expression. Singer's concept of **appetite** — *"start with a number, end with a design"* — is a useful input: how much time is this problem worth? ([basecamp.com/shapeup](https://basecamp.com/shapeup)) | Product roadmap definition |

### AI-PM Emphasis

**Success Criteria & Business Case** is where AI can generate financial models, forecast KPI trajectories from historical analogs, and stress-test assumptions. Lenny Rachitsky rates strategy and discovery as the PM skills *most* disrupted by AI (🤖🤖🤖🤖 on his 5-point scale), noting that *"high-level strategic skills will be most disrupted by AI, while soft skills become more valuable"* ([lennysnewsletter.com](https://www.lennysnewsletter.com/p/how-ai-will-impact-product-management)). **Roadmap Definition** benefits from AI-assisted dependency mapping and scenario planning. **Stakeholder Intent Alignment** remains deeply human — Lenny's "Sync the People" job is the PM function *least* disrupted by AI.

---

## Phase 3: SHAPE

**Core question:** *What solution takes form, and for whom?*

### Phase Lineage

This phase draws from three traditions: **Ryan Singer's Shape Up** methodology for scoping and de-risking, the **Double Diamond's second diamond** (Develop) for solution ideation, and **Cagan's solution-space discovery** for validation.

Singer's *Shape Up: Stop Running in Circles and Ship Work that Matters* (2019) introduced the concept of **shaping** — where senior practitioners define a solution's boundaries before handing it to a build team. Three properties define well-shaped work: *"It's rough. It's solved. It's bounded."* The key conceptual innovation is **appetite over estimation**: *"Estimates start with a design and end with a number. Appetite starts with a number and ends with a design"* ([basecamp.com/shapeup](https://basecamp.com/shapeup)). Shaping uses **fat-marker sketches** (deliberately low-fidelity so you can't add too much detail) and **breadboards** (flow diagrams using only words) to define a solution at the right level of abstraction. Singer: *"We can only judge what is a 'good' solution in the context of how much time we want to spend and how important it is"* ([basecamp.com/shapeup](https://basecamp.com/shapeup)). Lenny Rachitsky endorsed Shape Up as *"an incredible system that takes as input 'kludgy, clumsily scaled product org unsure about what to build and how' and delivers as output 'a focused clear thinking set of teams that has a rhythm, a method, and a purpose'"* ([x.com/lennysan](https://x.com/lennysan/status/1906750748689571927)).

Cagan's **four risks** provide the evaluation lens for this phase: *value risk* (will customers buy/use it?), *usability risk* (can they figure it out?), *feasibility risk* (can we build it?), and *viability risk* (does it work for the business?). The goal of Shape is to de-risk before committing to full Build ([svpg.com](https://www.svpg.com/product-discovery/)).

Torres emphasizes that solutions should always be plural — *"you start with a teeny tiny opportunity... and smaller opportunities lead to smaller solutions, which allow you to test quicker because you're working with smaller chunks of work"* ([chameleon.io](https://www.chameleon.io/blog/opportunity-solution-tree)). The OST's solution layer encourages generating **multiple solutions per opportunity**, then testing underlying assumptions rather than whole ideas.

### Components

| Component | Description | Enterprise Analog |
|---|---|---|
| **Persona & Journey Mapping** | Constructing or refining user models and mapping end-to-end customer journeys. Not just demographic profiles — behavioral archetypes grounded in real interview data (Torres' story-based interviewing) and jobs-to-be-done framing (Christensen/Moesta). | User persona creation + Customer journey maps |
| **Prototyping & Risk Reduction** | Wireframes, interactive prototypes, fat-marker sketches (Singer), and proof-of-concept builds. Cagan's four risks (value, usability, feasibility, viability) provide the evaluation lens. Torres: *"Break your ideas into their underlying assumptions. Often, you can test assumptions a lot faster than full ideas... Most assumption tests you can run in a day or two, while most idea tests take weeks"* ([chameleon.io](https://www.chameleon.io/blog/opportunity-solution-tree)). | Wireframes/prototypes |
| **Go-to-Market Planning** | Positioning, messaging architecture, channel strategy, and pricing model design. Deliberately placed in Shape (not Release) because GTM decisions constrain solution design — how you plan to reach customers should influence what you build. Pragmatic Institute treats GTM as a peer activity to product design, not a downstream afterthought ([pragmaticinstitute.com](https://www.pragmaticinstitute.com/product/framework/)). | GTM planning |

### AI-PM Emphasis

This is the phase **most visibly transformed by AI**. The Product-Led Alliance's AI-augmented lifecycle maps tools like Visily, Uizard, and Galileo AI to the prototyping stage, noting that *"AI is augmenting product designers to test their ideas faster, with less effort"* ([productledalliance.com](https://www.productledalliance.com/ai-augmented-product-development/)). Google AI PM Marily Nika demonstrates a workflow inversion: *skip the PRD first, go straight from idea to prototype, show engineers, then write the PRD* — collapsing what was a multi-week handoff into a single session using tools like v0.dev and Google AI Studio ([lennysnewsletter.com](https://www.lennysnewsletter.com/p/pms-who-use-ai-will-replace-those)). Claire Vo's ChatPRD (used by 10,000+ PMs) and her demonstration of going from idea to shipped product in 30 minutes using AI agents exemplify this compression ([creatoreconomy.so](https://creatoreconomy.so/p/from-idea-to-product-in-30min-using-ai-agents-claire-vo)). **Persona & Journey Mapping** benefits from AI-generated behavioral clusters from usage data. The human premium remains in judgment — deciding *which* prototype direction to pursue.

---

## Phase 4: BUILD

**Core question:** *How do we ship with clarity and conviction?*

### Phase Lineage

This phase covers the PM's role *during* engineering execution — not the engineering itself, but the continuous acts of specification, decomposition, negotiation, and communication that keep a build on track and aligned to intent.

**Cagan's Delivery Track** in Dual-Track Agile is the structural foundation: validated ideas flow from discovery into delivery, where engineering builds production-quality software. The PM's job during delivery is to maintain fidelity to the validated concept while enabling the team to make good micro-decisions. Cagan's key insight: *"The primary responsibility for product managers is discovery. The bulk of the PM's time needs to be focused on working with her product team, with her key stakeholders, and with her customers to discover solutions that her customers love and that work for the business"* — which means during Build, the PM is already running the next cycle of discovery in parallel ([svpg.com](https://www.svpg.com/product-discovery/)).

**Lenny Rachitsky** defined the PM's three jobs as *"shape the product, ship the product, and synchronize the people — and all of that in order to drive impact for the business"* ([lennysnewsletter.com](https://www.lennysnewsletter.com/p/what-is-product-management)). The Build phase maps primarily to "Ship the Product" and "Synchronize the People." In his AI impact analysis, he rates spec-writing and project management as moderately disrupted, but stakeholder synchronization as least disrupted — making the human coordination skills of Build *more* valuable as AI accelerates everything else ([lennysnewsletter.com](https://www.lennysnewsletter.com/p/how-ai-will-impact-product-management)).

**Singer's circuit breaker** from Shape Up provides an important Build discipline: *"If they don't finish, by default the project doesn't get an extension. We defined our appetite at the start... If the project was only worth six weeks, it would be foolish to spend two, three or ten times that"* ([basecamp.com/shapeup](https://basecamp.com/shapeup)). This reframes scope management from "preventing scope creep" to "empowering teams to cut scope themselves."

### Components

| Component | Description | Enterprise Analog |
|---|---|---|
| **Feature Specification Writing** | Writing and maintaining feature specifications, PRDs, and technical design documents. Claire Vo's ChatPRD demonstrates AI-assisted spec writing at scale. Lenny rates this as a 🤖🤖🤖 task: *"Describe what you want in human language, get an 80% complete draft, refine it, and then ship"* ([lennysnewsletter.com](https://www.lennysnewsletter.com/p/how-ai-will-impact-product-management)). The human premium is ensuring specs faithfully translate strategic intent into buildable scope. | Feature specification documents |
| **User Story & Acceptance Criteria** | Breaking features into user stories with clear acceptance criteria. Cagan recommends Jeff Patton's Story Mapping as *"the most generally useful technique I know"* for visualizing and decomposing work. The art is in decomposition that enables parallel work, incremental delivery, and testable increments. | User stories and acceptance criteria |
| **Stakeholder Communication** | Status communication, steering committee updates, cross-functional coordination, and expectation management. Lenny's "Sync the People" — the PM function *least* disrupted by AI and arguably *most* important as AI accelerates everything else. Rachitsky: *"PMs will continue to be the 'glue' or 'conductor' who tie everything together"* ([lennysnewsletter.com](https://www.lennysnewsletter.com/p/how-ai-will-impact-product-management)). | Manage stakeholders (e.g., status updates) |
| **Scope & Priority Tradeoffs** | Scope negotiations, priority shifts, and the ongoing tension between ambition and appetite. Singer's circuit breaker concept (killing what won't ship in time) is a useful mental model: *"Every part of a product doesn't need to be equally prominent, equally fast, and equally polished"* ([basecamp.com/shapeup](https://basecamp.com/shapeup)). Includes technical debt tradeoffs and quality/speed negotiations. | Tradeoff assessments/prioritizations |

### AI-PM Emphasis

**Feature Specification Writing** and **User Story & Acceptance Criteria** are prime targets for AI augmentation — ChatPRD, spec-writing copilots, and AI-assisted story generation from prototypes. Curtis Savage's U.S.I.D.O. Framework specifically maps AI to the "Define" phase for *"AI prioritizes features, writes PRDs, predicts feature impact on KPIs"* ([medium.com](https://medium.com/ai-for-product-people/a-framework-for-ai-product-management-df72f8a584de)). **Scope & Priority Tradeoffs** can leverage AI for impact modeling ("if we cut X, what's the projected effect on Y metric?"). **Stakeholder Communication** — keeping humans aligned — remains the most human-intensive work. As Tal Raviv notes, AI agents work best for *"least favorite, least impactful, but still necessary"* PM tasks ([lennysnewsletter.com](https://www.lennysnewsletter.com/p/make-product-management-fun-again)), freeing human energy for the judgment calls.

---

## Phase 5: RELEASE

**Core question:** *How do we put this into the world deliberately?*

### Phase Lineage

"Release" rather than "Launch" because it implies deliberate, controlled introduction — a valve, not a cannon. Modern product releases are often phased, flagged, and gradual.

**Cooper's Stage-Gate** provides the rigor: Stage 5 (Launch) is preceded by Stage 4 (Testing & Validation), with a formal gate review assessing quality of execution, business motivation, and strategic alignment before anything goes to market. Cooper's post-launch review at 12–18 months — *"the project's actual results are assessed versus those results promised when the project was approved"* — creates direct accountability back to the business case from Frame ([stage-gate.com](https://www.stage-gate.com/blog/the-stage-gate-model-an-overview/)).

**AIPMM's ProdBOK** is one of the few frameworks that separates "Launch" (the market introduction) from "Deliver" (ongoing operations and support), treating them as distinct lifecycle phases. This separation acknowledges that getting a product to market and keeping it running are fundamentally different activities.

**Pragmatic Institute's "Programs" category** encompasses launch planning, awareness campaigns, and sales enablement as peer activities — validating that release is a multifaceted effort requiring coordination across marketing, sales, customer success, and product teams ([pragmaticinstitute.com](https://www.pragmaticinstitute.com/product/framework/)).

### Components

| Component | Description | Enterprise Analog |
|---|---|---|
| **Release Readiness Assessment** | Go/no-go evaluation against pre-defined criteria: quality gates, performance benchmarks, support readiness, documentation completeness. Stage-Gate's gate review model provides the rigor template. | Product readiness assessments |
| **Phased Rollout Strategy** | Phased release strategy: internal dogfood → beta → limited GA → full GA. Feature flag strategies, canary deployments, and geographic/segment-based rollouts. The "how" and "when" of making the product available. | Release strategy definition |
| **Release Communications** | Internal and external changelogs, release notes, and stakeholder notifications. The narrative bridge between what was built and why it matters. | Release notes |
| **Launch Marketing & Enablement** | Launch campaigns, sales enablement, customer success briefings, and celebratory/recognition moments. The human energy that turns a release into momentum. | Recognition/marketing materials |

### AI-PM Emphasis

**Release Communications** are highly automatable — Lenny rates this area as 🤖🤖🤖🤖 for AI impact, with tools that generate release notes from commit logs and PRDs ([lennysnewsletter.com](https://www.lennysnewsletter.com/p/how-ai-will-impact-product-management)). The Product-Led Alliance maps AI to the launch phase for *"AI-driven messaging and targeting"* to optimize channel selection and audience segmentation ([productledalliance.com](https://www.productledalliance.com/ai-augmented-product-development/)). **Phased Rollout Strategy** benefits from AI-driven risk assessment (predicting which segments will surface issues). **Release Readiness Assessment** can leverage automated regression and quality scoring. **Launch Marketing & Enablement** remains primarily human-driven and relationship-dependent.

---

## Phase 6: MEASURE

**Core question:** *Did it work, and what do we do next?*

### Phase Lineage

"Measure" rather than "Learn" because it emphasizes empirical rigor. Learning is the *outcome* of good measurement; this phase is about the *discipline* of tracking, testing, and deciding.

**Eric Ries' Lean Startup** defined the Build-Measure-Learn loop, but critically, Ries advises planning it *in reverse*: decide what to learn first, then what to measure, then what to build. This connects Measure back to Frame — you can't measure well unless you defined success criteria clearly.

**Melissa Perri** provides the animating principle: *"Raise your hand if you went back and iterated on the last thing you shipped. Normally, 15-20% of the people raise their hands."* The build trap persists because teams don't close the loop. Her Product Kata demands that teams compare actual results to target conditions and decide whether to persevere, pivot, or stop. Perri: organizations fall into the build trap *"because they are not actually measuring the outcomes of their actions. They lose track of their strategy and vision"* ([melissaperri.com](https://melissaperri.com/book)).

**Google's HEART framework** (Happiness, Engagement, Adoption, Retention, Task Success) provides a structured way to define *what* to measure across user experience dimensions. **AARRR Pirate Metrics** (Acquisition, Activation, Retention, Revenue, Referral) organizes metrics around the growth funnel. Both supply the measurement vocabulary; this phase supplies the lifecycle discipline of *when* and *how* to act on those metrics.

**AIPMM's ProdBOK** is one of the few frameworks that treats "Retire" as an explicit lifecycle phase — acknowledging that sunsetting products and features is a first-class PM responsibility, not an afterthought.

### Components

| Component | Description | Enterprise Analog |
|---|---|---|
| **KPI & Outcome Monitoring** | Monitoring the KPIs and success metrics defined in Frame (Success Criteria & Business Case). North Star metric dashboards, OKR progress reviews, and the honest reckoning of whether the bet paid off. **The feedback loop to Frame is the most critical connection in the entire lifecycle.** Cooper's Stage-Gate builds in a post-launch review at 12–18 months where *"actual results are assessed versus those results promised when the project was approved."* | KPI tracking and management |
| **Customer Feedback Collection** | Structured feedback collection and synthesis: NPS/CSAT tracking, in-app surveys, support ticket theme analysis, user interview programs, and social listening. Torres' continuous discovery habits apply here — post-launch interviewing is just as important as pre-launch. The feedback loop to Discover starts here. | Customer feedback tracking and logging |
| **Experiment Design & Analysis** | Controlled experiments (A/B tests, multivariate tests), feature flag analysis, and statistical rigor in interpreting results. Includes experiment design, sample size planning, and the discipline to actually *act on* results rather than just collecting them. | A/B or feature flag testing & analysis |
| **End-of-Life & Deprecation Planning** | Deprecation strategy, migration paths, customer communication for end-of-life products or features, and the often-neglected work of *removing* what no longer serves. ProdBOK is one of the few frameworks that treats "Retire" as an explicit lifecycle phase. | End of life planning |

### AI-PM Emphasis

This is where AI's pattern recognition capabilities shine brightest. Curtis Savage's U.S.I.D.O. Framework maps the "Optimize" phase to AI that *"refines GTM strategy, identifies key metrics, runs experiment analysis"* ([medium.com](https://medium.com/ai-for-product-people/a-framework-for-ai-product-management-df72f8a584de)). The Product-Led Alliance describes AI's post-launch role as *"behavioral analytics, anomaly detection"* and continuous AI-driven improvement ([productledalliance.com](https://www.productledalliance.com/ai-augmented-product-development/)). Automated anomaly detection in metrics, AI-driven cohort analysis, natural language summarization of customer feedback themes, and predictive churn modeling are all production-ready today. The **Measure → Discover** feedback loop — where post-launch insights generate new opportunities — is dramatically accelerated when AI can surface patterns humans would miss.

---

## The Lifecycle as a Loop

```
    ┌──────────────────────────────────────────┐
    │                                          │
    ▼                                          │
 DISCOVER ──→ FRAME ──→ SHAPE ──→ BUILD ──→ RELEASE ──→ MEASURE
    ▲                                                       │
    │                                                       │
    └───────────────────────────────────────────────────────┘
         Measure → Discover: the strategic learning loop
         (Perri's Product Kata, Reforge's strategy feedback)
```

**Measure → Discover** is the strategic feedback loop where empirical outcomes and customer feedback generate new signals, opportunities, and problem hypotheses. This is not just "iterate on what you built" (that's Measure → Shape). This is where learning reshapes understanding of the problem space itself.

**Frame → Measure** is the accountability loop: the success criteria defined in Frame's Success Criteria & Business Case are the exact metrics evaluated in Measure's KPI & Outcome Monitoring. If these two phases aren't tightly coupled, teams ship without knowing what winning looks like.

---

## Framework Attribution Summary

| Phase | Primary Voices | Key Concepts Borrowed |
|---|---|---|
| **Discover** | Teresa Torres, Marty Cagan, Jeff Patton | Opportunity Solution Tree, weekly customer interviews, Opportunity Assessment, Opportunity Backlog |
| **Frame** | Robert Cooper, Melissa Perri, Reforge (Mehta/Winters), Pragmatic Institute | "Build the Business Case" as a gate, Product Kata / target condition, Strategy Stack, business case as first-class activity |
| **Shape** | Ryan Singer, Cagan (solution-space discovery), Torres (assumption testing), Design Council (Double Diamond) | Shaping / appetite / fat-marker sketches, four risks, assumption tests over idea tests, diverge-then-converge |
| **Build** | Cagan (Delivery Track), Lenny Rachitsky, Claire Vo, Ryan Singer | Dual-track delivery, Shape/Ship/Sync model, ChatPRD, circuit breaker |
| **Release** | Robert Cooper, Pragmatic Institute, AIPMM (ProdBOK) | Stage-Gate gate 5 + post-launch review, Programs category, Launch/Deliver separation |
| **Measure** | Eric Ries, Melissa Perri, Google (HEART), AIPMM (ProdBOK) | Build-Measure-Learn (in reverse), "done when outcome achieved," HEART framework, Retire as explicit phase |

### Key Sources Referenced

| Voice | Key Work | URL |
|---|---|---|
| Teresa Torres | *Continuous Discovery Habits* (2021); Opportunity Solution Trees | [producttalk.org](https://www.producttalk.org/opportunity-solution-trees/) |
| Marty Cagan | *Inspired* (2018); *Transformed* (2024); SVPG Product Operating Model | [svpg.com](https://svpg.com/assessing-product-opportunities/) |
| Melissa Perri | *Escaping the Build Trap* (2018) | [melissaperri.com](https://melissaperri.com/book) |
| Ryan Singer | *Shape Up* (2019) | [basecamp.com/shapeup](https://basecamp.com/shapeup) |
| Lenny Rachitsky | PM three-job model; AI impact on PM analysis | [lennysnewsletter.com](https://www.lennysnewsletter.com/p/how-ai-will-impact-product-management) |
| Robert Cooper | Stage-Gate® (1980s–present) | [stage-gate.com](https://www.stage-gate.com/blog/the-stage-gate-model-an-overview/) |
| Pragmatic Institute | 37-activity PM Framework | [pragmaticinstitute.com](https://www.pragmaticinstitute.com/product/framework/) |
| Curtis Savage | U.S.I.D.O. Framework for AI PMs | [medium.com](https://medium.com/ai-for-product-people/a-framework-for-ai-product-management-df72f8a584de) |
| Claire Vo | ChatPRD; "How I AI" podcast | [chatprd.ai](https://www.chatprd.ai/) |
| Marily Nika | Google AI PM toolkit / workflow inversion | [lennysnewsletter.com](https://www.lennysnewsletter.com/p/pms-who-use-ai-will-replace-those) |
| Product-Led Alliance | AI-augmented product development lifecycle | [productledalliance.com](https://www.productledalliance.com/ai-augmented-product-development/) |
| Tal Raviv | AI agents for PM (copilots vs. agents) | [lennysnewsletter.com](https://www.lennysnewsletter.com/p/make-product-management-fun-again) |
| Eric Ries | *The Lean Startup* (2011) | — |
| AIPMM | ProdBOK (7 lifecycle activities incl. Retire) | [aipmm.com](https://aipmm.com/) |

---

## Using This Framework as a Taxonomy

When cataloging an AI-PM technique or insight for the ai-pm-craft repository, ask:

1. **Which phase does this technique primarily augment?** Tag it there.
2. **Does it span phases?** Use the primary phase and note connections. (e.g., "AI-generated PRDs" lives in Build / Feature Specification Writing but draws from Shape / Prototyping & Risk Reduction.)
3. **Does it accelerate a component, or replace/invert it?** Nika's "prototype before PRD" doesn't just speed up Shape — it *reorders* Shape and Build. That's worth noting distinctly.
4. **Is it a technique (how), a tool (what), or a principle (why)?** The taxonomy should accommodate all three.

If an insight doesn't fit any phase cleanly, it likely belongs to one of the two cross-cutting domains: **Horizontal Product & Knowledge Work** (prompt engineering, context engineering, writing workflows) or **AI Adoption & Change Management** (scaling expertise, org restructuring, driving adoption).