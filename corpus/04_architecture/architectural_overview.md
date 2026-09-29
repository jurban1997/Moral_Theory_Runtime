[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §5.1

*Reference Architecture. This layer defines what the system is, without equations or an implementation.*

# Reference Architecture

> The Reference Architecture should contain no equations. It defines components, relationships, and information flow. Formal notation belongs in Moral Assessment Methodology.

## Architectural Overview

The Reference Architecture defines the conceptual structure required to perform moral assessment as an explicit, inspectable, and computationally representable state-transition process. It does not prescribe a specific algorithm, equation, database model, inference engine, programming language, artificial intelligence architecture, or deployment pattern. Its purpose is to define what must exist in the moral reasoning system and how those architectural elements relate to one another.

Intuitively, the architecture begins from the observation that every morally relevant action changes the world. Some changes are immediate and visible, while others unfold across relationships, institutions, incentives, decision policies, future opportunities, and the long-term flourishing of affected entities. A moral assessment therefore cannot be limited to whether an action satisfies a rule, maximizes a single metric, or produces an isolated outcome. It must evaluate how the action transforms the relevant state of the world.

Architecturally, the framework represents moral reasoning as a recursive, graph-based, state-transition model. The World Context before the action contains Objects, Associations, states, constraints, information, institutions, objectives, policy states, and future possibilities. The Assessed Action operates within a progressively filtered context derived from that World Context. The action then produces predicted consequences that alter Objects, Associations, policy states, opportunities, institutional conditions, and the Long-Term Flourishing of relevant Flourishing Entities. The result is a transformed World Context that becomes the starting condition for future assessments.

The primary object of moral assessment is the World Context Transition. Individual state changes, changes in Long-Term Flourishing, and aggregate flourishing metrics are important inputs to assessment, but they do not replace evaluation of the resulting World Context as a whole. This distinction prevents the architecture from collapsing into a single-score consequentialist model. The assessment asks not merely whether some isolated outcome improved, but whether the resulting world state better preserves and promotes long-term flourishing without materially diminishing other relevant Flourishing Entities.

The architecture is graph-based because morally relevant reality is modeled as a network of Objects and Associations. Objects are the fundamental ontological elements. Associations connect Objects and may carry morally relevant attributes such as obligation, authority, dependency, trust, responsibility, legitimacy, or ownership. Actor, affected entity, observer, responder, institution, and similar terms are contextual roles that Objects may occupy within a specific assessment. Flourishing Entity and Moral Agent are evaluative classifications applied to Objects when they satisfy the framework's criteria.

The architecture is recursive because every assessment produces a new World Context. The output of one assessment becomes part of the input state for subsequent assessments. This recursion is morally significant because actions do not merely change material conditions; they also change expectations, precedents, institutional norms, incentives, and future decision policies. A harmful means used to achieve a beneficial short-term result may degrade the Actor's future policy state or teach observers that similar means are acceptable. These Distributed Policy Effects are part of the resulting World Context and therefore part of the moral assessment.

The Reference Architecture is constrained by the Foundational Axiom but does not itself define the mathematical method for applying that axiom. The axiom supplies the normative direction of assessment: the architecture evaluates whether a transition preserves and promotes the long-term flourishing of relevant Flourishing Entities---and fosters the adaptive development of moral agents---while avoiding material diminishment of other relevant Flourishing Entities, with the flourishing of entities and of the contexts they participate in (across the Biosphere, Society, and Individual tiers) treated as mutually constitutive. The architecture defines the structures through which this evaluation is represented; the Moral Assessment Methodology defines how particular assessments are performed.

The architectural flow can be summarized as follows:

World Context\
→ Assessment Boundary\
→ Local Context\
→ Situational Context\
→ Relevant Objects and Associations\
→ Objectives\
→ Assessed Action\
→ Predicted Consequences\
→ World Context Transition\
→ Moral Assessment

This flow should be understood as architectural information flow rather than a required software pipeline. Implementations may perform these steps iteratively, recursively, in parallel, probabilistically, or through future computational approaches. A conforming implementation must preserve the meaning of the architectural elements, but it need not implement them using any particular computational structure.

The Reference Architecture therefore provides a stable conceptual foundation for many possible implementations. It may support human decision-making, organizational governance, legal analysis, medical ethics, public policy, robotics, autonomous systems, LLM alignment, AGI safety, or a Moral Reasoning Runtime. These implementations may differ substantially, but they remain aligned with the architecture if they preserve the core semantics: context selection, relevant Objects and Associations, assessment of an Assessed Action, predicted state transition, Distributed Policy Effects, Long-Term Flourishing, and evaluation of the resulting World Context Transition.

### Context Stack

The Context Stack defines how the architecture progressively narrows the complete theoretical World Context into the portion of the world that is relevant for a specific moral assessment. It exists because moral assessment would be computationally and analytically unbounded if every possible Object, Association, state variable, causal pathway, and future consequence had to be considered at full resolution.

Intuitively, the Context Stack answers the question: "Which part of the world must be considered in order to assess this action responsibly?" It does not deny that the full world exists, nor does it imply that excluded information has no moral significance in principle. Rather, it defines the working boundary within which assessment can be performed with explicit assumptions and an appropriate confidence level.

Architecturally, the core Context Stack consists of four primary layers:

World Context\
→ Assessment Boundary\
→ Local Context\
→ Situational Context

Each layer performs a distinct architectural function. The World Context is the complete theoretical state container. The Assessment Boundary defines how that state is partitioned for assessment. The Local Context identifies the subset relevant to a class of moral assessments. The Situational Context identifies the directly relevant evidentiary and state boundary for evaluating the specific Assessed Action.

The Context Stack is *epistemic*: its layers filter what an assessment must consider. It is the mirror of the *ontological* structure the Foundational Axiom names---the three Context Tiers (Biosphere, Society, Individual) and the lattice of contexts within them (see **Foundational Definitions → Context Tier** and §4.7). The World Context is the state container in which the tiers and their contexts are represented; the Assessment Boundary must locate every materially affected context in its tier (see **Operational Primitives → Assessment Boundary Selection**). The Stack therefore tracks real structure rather than being a modeling convenience.

The Context Stack should be treated as the default architectural structure rather than as an immutable limit on future refinement. Additional intermediate context layers may be introduced when required by a domain, implementation, or future extension of the architecture, provided they preserve the semantics of progressive filtering from broader world state to assessment-specific context.

See **Architectural Elements** for definitions of the World Context, Assessment Boundary, Local Context, and Situational Context.

