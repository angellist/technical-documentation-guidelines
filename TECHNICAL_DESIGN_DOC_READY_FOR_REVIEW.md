# A technical design doc has explicit readiness criteria.

## We are writing for stronger collaboration, for validated understanding, and for faster execution.

Sharing a spec across the team (and/or across divisions) challenges your thinking and stress tests your assumptions. We build better when we work together.

Validating understanding of the problem means pre-planning. By pre-planning, you’ll front-load the work of understanding existing code, business context, legal constraints, etc.

The better specified the work is, the more quickly the work can be executed.

## Invariants

Each invariant relates to one or more of the readiness criteria.

### Every fact must be true.

A majority of a technical design consists of facts, and these facts must be true, and this must be easily checked through provided URLs.

If the thinking that led to the design doc led to `assert(false)`, then this exercise has not validated any understanding.

If a teammate cannot check your work without spending a signficant amount of effort, then we are less effective working together.

Corollary: every quote must be real.

Corollary: every metaphor is an assertion of "A is like B", and this assertion must also be true.

Two of AngelList's values are "Sweat the details", and "Hold ourselves accountable".

### The no-build alternative must be uncompelling.

Part of the template encourages the writer to consider design alternatives.

A technical design must include an argument for how it is better than the status quo, to validate the understanding of the current system and the proposed system.

Teammates are used to the status quo, and we must engage with this reality to work together effectively.

Specifically, for every critique of no-build based in fact, the critique must be paired with an analoguous critique of the proposed system.

Sometimes, we can explicitly prefer a design that improves some dimensions at the expense of other dimensions, and enumerating the dimensions is part of validating understanding.

### tbd

tbd

### tbd

tbd

## Appendix A: historical artifact from Notion

### Overview

*This section gives the reader a very rough overview of the landscape in which the new system is being built and what is actually being built. This isn’t a requirements doc. Keep it succinct! The goal is that readers are brought up to speed but some previous knowledge can be assumed and detailed info can be linked to. This section should be entirely focused on objective background facts.*

#### Goals

*A short list of bullet points of what the goals of the system are*.

#### Anti-goals

*A short list of bullet points of what the anti-goals of the system are*.

### The actual design

*This section should start with an overview and then go into details. Use the sections below as a starting point, but remove any that aren’t relevant, or add any that are missing for your design.*

##### System context diagram

*In many docs a system-context-diagram can be very useful. Such a diagram shows the system as part of the larger technical landscape and allows readers to contextualize the new design given its environment that they are already familiar with.*

##### Entity relationship diagram

*If the system under design includes new database models or relationships, then sketching out those in an entity relationship diagram is usually a good idea.* 

##### APIs

*If the system under design exposes an API, then sketching out that API is usually a good idea. In most cases, however, one should withstand the temptation to copy-paste formal interface or data definitions into the doc as these are often verbose, contain unnecessary detail and quickly get out of date. Instead focus on the parts that are relevant to the design and its trade-offs.*

##### Observability

*Outline any diagnostics, logging, metrics, or other observability critical to the design.* 

##### Security & Privacy

*Outline how the design impacts security or privacy.* 

### Alternatives considered

*This section lists alternative designs that would have reasonably achieved similar outcomes. The focus should be on the trade-offs that each respective design makes and how those trade-offs led to the decision to select the design that is the primary topic of the document.*

*While it is fine to be succinct about solution that ended up not being selected, this section is one of the most important ones as it shows very explicitly why the selected solution is the best given the project goals and how other solutions, that the reader may be wondering about, introduce trade-offs that are less desirable given the goals.*
