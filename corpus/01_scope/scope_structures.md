[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §1.5

*The distinct senses of scope used by the architecture, from the document itself down to a single assessment.*

# Scope Structures

The term scope is used in several related but distinct ways within this framework. At the highest level, scope defines what this document is attempting to describe. Within the architecture, scope also determines what portion of the World Context is considered relevant, which entities are included in an assessment, which consequences are evaluated, which time horizons are considered, what information is admissible, and which implementation details are intentionally excluded.

Because moral assessment can expand without practical limit if every possible entity, relationship, consequence, and future condition is considered, the framework requires explicit scope structures. These structures do not determine the moral answer by themselves. Rather, they define the boundaries within which moral assessment is performed, the assumptions under which the assessment is valid, and the level of confidence that should be attached to the result.

## Document Scope

The scope of this document is to define a computational reference architecture for moral reasoning. It is not intended to present a complete philosophical doctrine, a single moral rule set, a closed ontology, or a finished software product. The document defines the major concepts, relationships, context structures, and assessment logic required to represent moral reasoning as a computationally inspectable state-transition process.

This document therefore includes architectural definitions, methodological guidance, implementation considerations, and validation strategy, but these must remain conceptually separated. The Reference Architecture defines what the moral reasoning system is. The Moral Assessment Methodology defines how the architecture may be used to perform assessments. The Implementation section describes how the architecture may be realized in software or institutional processes. None of these layers should be collapsed into a single implementation-specific design.

## Architectural Scope

Architectural scope defines the conceptual structures that belong inside the Reference Architecture. These include Objects, Associations, contexts, objectives, Assessed Actions, state transitions, Long-Term Flourishing, and Distributed Policy Effects. Architectural scope is concerned with what must exist in the model for moral assessment to be represented coherently.

The Reference Architecture should remain implementation-independent. It should define components, relationships, and information flow without prescribing a programming language, database structure, inference engine, mathematical formalism, user interface, or deployment platform. The purpose of architectural scope is to ensure that the framework can be implemented in many ways while preserving a stable conceptual foundation.

## Methodological Scope

Methodological scope defines how the Reference Architecture is used to perform a moral assessment. It includes evidence handling, uncertainty representation, confidence estimation, state-transition prediction, multi-horizon assessment, aggregation of flourishing changes, and generation of assessment outputs.

Methodological scope may include probabilistic reasoning, stochastic approximation, candidate state variables, and structured assessment artifacts. These elements are necessary to operationalize the architecture, but they should not be confused with the architecture itself. The methodology may evolve as better mathematical tools, empirical evidence, predictive models, or computational methods become available.

## Implementation Scope

Implementation scope defines how the architecture and methodology may be realized in a particular system. Implementations may include standalone services, embedded libraries, workflow components, agent modules, audit systems, governance tools, robotics control layers, or Moral Reasoning Runtime deployments.

A Moral Reasoning Runtime is one possible implementation path, not the architecture itself. Similarly, an LLM harness, autonomous robotics system, clinical decision-support tool, legal analysis system, or public-policy evaluation platform may implement parts of the architecture without defining the architecture. Implementation scope must therefore remain subordinate to architectural scope.

## Application Scope

Application scope defines the domains in which the framework may be used. These include human ethical decision-making, organizational governance, public policy, legal analysis, medical ethics, autonomous systems, robotics, multi-agent systems, LLM alignment, AGI safety, and other domains involving consequential action.

AI alignment is an important application, but it is not the defining scope of the framework. The framework is intended to support moral reasoning across human, institutional, biological, ecological, and artificial domains wherever actions can be represented as transformations of a World Context.

## Assessment Scope

Assessment scope defines the specific moral question being evaluated. It identifies the Assessed Action, the Actor or Actors, the relevant Objectives, the affected Objects and Associations, and the World Context transition to be assessed.

Assessment scope is narrower than document scope, architectural scope, or application scope. It applies to a particular proposed, ongoing, or completed action. For example, the framework as a whole may apply to medical ethics, but the assessment scope for a particular case may be limited to whether a physician should recommend a specific treatment to a specific patient under defined clinical uncertainty.

## Contextual Scope

Contextual scope defines which portion of the World Context is considered relevant to the assessment. The World Context represents the complete theoretical state of the world at the time of assessment. Because this complete state cannot be fully represented or evaluated in practice, the architecture uses progressively filtered context structures.

The Local Context identifies the portion of the World Context relevant to a class of assessments, such as healthcare, public policy, family obligations, environmental stewardship, or military action. The Situational Context identifies the subset of the Local Context directly relevant to the specific Assessed Action. Additional context structures, such as Decision Context, Accessible Context, and Assessment Context, define the information available to the Actor, the information reasonably obtainable through due diligence, and the information available to the assessor at the time of evaluation.

## Domain Scope

Domain scope defines the class of activity, institution, or practice within which the assessment occurs. Examples include medicine, law, organizational governance, transportation, environmental management, military operations, education, finance, robotics, and artificial intelligence.

Domain scope helps determine which Objects, Associations, norms, evidence sources, risks, obligations, and state variables are likely to be relevant. A medical decision and a public-policy decision may both use the same Reference Architecture, but they will require different Local Contexts, different evidence standards, different Associations, and different domain-specific state variables.

## Entity Scope

Entity scope defines which Objects and Flourishing Entities are included in the assessment. Not every Object in the World Context is morally relevant to every action. An Object becomes relevant when its state, relationships, future opportunities, or Long-Term Flourishing may be meaningfully affected by the Assessed Action.

Entity scope must distinguish among Objects, Flourishing Entities, Moral Agents, Actors, affected entities, observers, responders, institutions, and non-flourishing objects. A rock may be an Object in the World Context, but it is not a Flourishing Entity unless it satisfies the framework's criteria for Long-Term Flourishing. A human, animal, ecosystem, institution, or sufficiently self-directed artificial system may fall within entity scope when its flourishing can be meaningfully increased or diminished.

## Causal Scope

Causal scope defines which consequences of the Assessed Action are included in the predicted World Context transition. It includes direct effects, indirect effects, side effects, foreseeable downstream effects, changes to Associations, changes to institutions, changes to future opportunities, and changes to the decision policies of relevant moral agents.

Causal scope is necessary because moral significance is not limited to immediate outcomes. An action may produce a beneficial short-term result while also damaging trust, incentives, institutions, or future decision behavior. These causal effects must be included when they are sufficiently connected to the Assessed Action and sufficiently material to the resulting World Context transition.

## Temporal Scope

Temporal scope defines the assessment horizons over which consequences are evaluated. The default horizons include immediate, short-term, long-term, multi-generational, and civilizational timeframes. Additional horizons may be introduced when required by the domain or situation.

Temporal scope is essential because the moral character of an action may change across time. An action may produce short-term harm but long-term flourishing, or short-term benefit but long-term degradation of institutions, trust, adaptive capacity, or future state space. Confidence generally decreases as temporal scope extends farther into the future, so temporal scope must be paired with explicit uncertainty and confidence reporting.

## Epistemic Scope

Epistemic scope defines what information is considered available, reasonably obtainable, or admissible for assessment. The Decision Context includes the information reasonably available to the Actor at the time of decision. The Accessible Context includes the information a reasonably competent Moral Agent could have obtained through appropriate diligence within the same Situational Context. The Assessment Context includes information available to the assessor, including later-discovered evidence and observed outcomes.

This distinction is important because moral responsibility should not be evaluated solely according to what the Actor claims to have known. It should also consider what a competent moral agent could reasonably have known or discovered under the circumstances. Epistemic scope therefore affects both the assessment of the action and the confidence assigned to the assessment.

## Normative Scope

Normative scope defines the moral direction supplied by the Foundational Axiom and the moral-system objective of supporting Long-Term Flourishing. It determines what the assessment is ultimately trying to preserve, promote, or avoid diminishing.

Normative scope does not prescribe a single algorithm or outcome. Instead, it provides the evaluative direction against which World Context transitions are assessed. Operational objectives within a specific domain or situation may be relevant, but they cannot override the Foundational Axiom. For example, an organization's objective to survive financially cannot justify actions that materially diminish the long-term flourishing of other relevant Flourishing Entities.

## Perspective Scope

Perspective scope defines the standpoint from which the assessment is being considered. A moral assessment may need to distinguish the Actor's perspective, the affected entity's perspective, the observer's perspective, the institutional perspective, and the external assessor's perspective.

The framework should not allow perspective scope to collapse into subjective preference. Instead, perspective scope identifies which information, relationships, obligations, incentives, and policy updates are visible or relevant from a given standpoint. This allows the model to represent disagreement, asymmetry of information, and institutional role differences without abandoning objective assessment.

## Jurisdictional and Authority Scope

Jurisdictional and authority scope define the legal, institutional, organizational, or procedural boundaries within which an action occurs. These boundaries may determine who has authority to act, who has responsibility, which rules apply, which institutions are affected, and which Associations carry moral significance.

Jurisdictional scope does not determine morality by itself. A legal action may still be morally harmful, and an illegal action may sometimes be morally defensible under extreme circumstances. However, jurisdictional and authority structures are part of the World Context and may affect obligations, legitimacy, trust, institutional stability, and future policy updates.

## Computational Scope

Computational scope defines what can realistically be represented, estimated, or computed during an assessment. Exact computation of the full World Context transition will often be impossible. The framework therefore expects approximation, abstraction, probabilistic reasoning, hierarchical modeling, and confidence reporting.

Computational limits should not be hidden. When an assessment relies on incomplete information, simplified models, uncertain predictions, or bounded computation, those limits should reduce confidence rather than be ignored. Computational scope therefore defines not only what the system attempts to calculate, but also what uncertainty must be disclosed.

## Scope Interaction

The scope structures in this framework are interdependent. Application scope helps determine domain scope. Domain scope helps determine Local Context. Assessment scope identifies the specific Assessed Action. Contextual scope determines which portion of the World Context is considered. Entity scope determines which Flourishing Entities and Associations are relevant. Causal and temporal scope determine which consequences are evaluated. Epistemic scope determines what evidence is available or reasonably obtainable. Computational scope determines the confidence with which the assessment can be performed.

A complete moral assessment should therefore identify its scope assumptions explicitly. When scope boundaries are uncertain, contested, or incomplete, the assessment should state those limitations and reflect them in the resulting confidence estimate.

