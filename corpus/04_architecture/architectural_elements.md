[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §5.3

*Reference Architecture. This layer defines what the system is, without equations or an implementation.*

# Architectural Elements

The Reference Architecture is composed of conceptual elements that define what exists within a moral assessment and how those elements relate to one another. These elements are implementation-independent. They may be represented through graphs, state models, ontologies, databases, symbolic structures, probabilistic models, or future computational methods, but the architecture itself does not prescribe any particular implementation.

The architectural elements collectively support the assessment of an Assessed Action as a transformation from one World Context to another. Each element contributes to identifying what is being evaluated, who or what may be affected, what relationships matter, what objectives guide assessment, what constraints apply, and how the resulting World Context differs from the initial World Context.

## World Context

The World Context is the complete theoretical state of the world at the instant an assessment begins. It includes all Objects, Associations, states, constraints, information, institutions, decision policies, future opportunities, and relevant possibilities that could, in principle, bear on the assessment.

The World Context is not limited to what the Actor knows, what the assessor knows, or what an implementation can fully represent. It is the theoretical state container from which all narrower contexts are derived. In practice, no implementation will fully capture the World Context. The architecture therefore treats the World Context as a conceptual superset rather than a fully computable dataset.

The World Context includes both material and non-material state. It may include physical entities, biological organisms, human beings, organizations, ecosystems, artificial systems, legal rules, institutional structures, trust relationships, information states, technological capabilities, social norms, and future state space. It also includes the current policy states of relevant Moral Agents and institutions insofar as those policy states may be affected by the Assessed Action.

The World Context is morally significant because every assessment evaluates a transition from one World Context to another. The resulting World Context after an action includes not only immediate outcomes but also altered relationships, changed incentives, updated policy states, modified institutions, altered constraints, and expanded or diminished future possibilities. The architecture therefore treats World Context Transition as the principal object of moral assessment.

Every moral assessment begins with a World Context and produces a transformed World Context. This makes the World Context both the starting condition and the recursive output of the architecture.

## Assessment Boundary

The Assessment Boundary is the architectural component that determines which portions of the World Context are included in a specific assessment. It defines the boundary between the complete theoretical World Context and the narrower contexts used for evaluation.

The Assessment Boundary may be configured through scope structures such as domain, entity class, causal reach, temporal horizon, perspective, jurisdiction, authority, and available evidence. It does not determine the moral conclusion by itself. Instead, it defines the assumptions under which the assessment is performed.

A well-defined Assessment Boundary allows the assessment to remain explicit, inspectable, and confidence-sensitive. If a boundary excludes potentially relevant entities, evidence, consequences, or time horizons, that limitation should be reflected in the assessment's confidence.

## Local Context

The Local Context is the subset of the World Context relevant to a class of moral assessments. It represents the domain-level or category-level context within which a specific assessment will occur.

Examples of Local Contexts include healthcare, legal analysis, military action, environmental stewardship, organizational governance, public policy, family obligations, transportation, robotics, autonomous systems, and artificial intelligence alignment. Each Local Context identifies the kinds of Objects, Associations, institutions, norms, constraints, evidence sources, risks, and state variables that are typically relevant to that class of assessment.

The Local Context reduces complexity by excluding portions of the World Context that are not normally relevant to the class of assessment. For example, a medical ethics assessment may require patient state, clinical evidence, informed consent, family relationships, treatment alternatives, institutional obligations, and physician responsibilities. A public-policy assessment may require population effects, economic access, environmental conditions, legal authority, institutional legitimacy, and long-term civic trust. Both assessments use the same Reference Architecture, but they draw from different Local Contexts.

The Local Context should not be treated as a closed domain silo. Some assessments require cross-domain expansion. A medical decision may implicate law, family obligations, insurance structures, public health, or institutional policy. A robotics decision may implicate safety, labor, accessibility, privacy, and public trust. When cross-domain effects are material, the Local Context should be expanded or linked to additional Local Contexts.

The Local Context provides the architectural bridge between the complete World Context and the specific Situational Context. It establishes the domain-relevant background from which the specific assessment is constructed.

## Situational Context

The Situational Context is the subset of the Local Context directly relevant to the specific Assessed Action. It contains the Objects, Associations, states, constraints, information, objectives, risks, alternatives, and foreseeable consequences that bear directly on the moral assessment of that action.

The Situational Context is the immediate context in which the Assessed Action is evaluated. It identifies the Actor or Actors, the relevant Flourishing Entities, the affected Objects and Associations, the applicable operational objectives, the material constraints, the relevant evidence, and the plausible consequences across assessment horizons.

The Situational Context also functions as the primary evidentiary boundary for assessment. It determines what information is relevant to evaluating the action and what information should be considered available, reasonably obtainable, or later available to an assessor. Related epistemic contexts, including Decision Context, Accessible Context, and Assessment Context, refine how responsibility and confidence are evaluated, but they do not replace the Situational Context as the state boundary for the specific action.

The Situational Context must be specific enough to support assessment but broad enough to include material consequences. If it is too narrow, the assessment may ignore affected entities, future harms, institutional effects, or Distributed Policy Effects. If it is too broad, the assessment may become computationally infeasible or analytically unfocused. The quality of the Situational Context therefore directly affects the quality and confidence of the moral assessment.

A Situational Context may change as additional information becomes available. In proposed-action assessments, the Situational Context includes current evidence and predicted consequences. In ongoing-action assessments, it may include emerging evidence and partial outcomes. In completed-action assessments, it may include observed outcomes and later-discovered evidence. These differences should be represented explicitly rather than hidden inside the assessment.

## Relevant Objects

Relevant Objects are Objects within the assessment boundary whose state, relationships, opportunities, constraints, or role in the World Context may be materially affected by the Assessed Action.

An Object is the fundamental ontological element in the architecture. Objects may include persons, animals, ecosystems, organizations, institutions, artificial systems, physical assets, information artifacts, contracts, laws, resources, or other persistent entities within the moral domain.

Not every Object is morally relevant in every assessment. An Object becomes relevant when it participates in the Situational Context in a way that may affect the World Context Transition, the Long-Term Flourishing of a Flourishing Entity, the state of an Association, or the future behavior of Moral Agents.

## Associations

Associations are morally relevant relationships between Objects. They are the connective structure of the ethical graph and may possess their own state, attributes, history, and constraints.

Associations may represent relationships such as responsibility, authority, obligation, dependency, trust, ownership, care, governance, consent, contract, command, stewardship, representation, or institutional membership. Moral significance often arises not from Objects in isolation, but from the Associations among them.

Associations may change as a result of an Assessed Action. A decision may strengthen trust, weaken legitimacy, create obligations, violate consent, alter authority, damage dependency relationships, or transform institutional responsibilities. These Association changes are part of the resulting World Context.

## Flourishing Entities

A Flourishing Entity is an Object whose Long-Term Flourishing can be meaningfully increased or diminished by changes to its state, relationships, environment, opportunities, or future state space.

Flourishing Entities may include humans, non-human organisms, ecosystems, institutions, organizations, and future artificial systems that satisfy the framework's criteria. The classification is not limited to biological life if a non-biological system possesses the relevant self-directed and adaptive characteristics.

A Flourishing Entity is not a separate node type. It is an evaluative classification applied to an Object when that Object's flourishing is morally assessable. The architecture evaluates how the Assessed Action changes the Long-Term Flourishing of relevant Flourishing Entities across assessment horizons.

## Moral Agents

A Moral Agent is a Flourishing Entity capable of selecting among alternative Actions, evaluating those Actions against Objectives, and bearing moral responsibility.

Moral Agents are relevant because they can initiate actions, respond to actions, observe actions, update future decision policies, and participate in moral responsibility. A Moral Agent may be human, institutional, collective, artificial, or otherwise constituted if it satisfies the framework's criteria for moral agency.

Moral Agent is not a separate node type. It is an evaluative classification applied to an Object based on capabilities such as decision-making, objective evaluation, responsibility, and policy adaptation.

### Contextual Roles

Contextual Roles describe how Objects participate in a specific assessment. They are not separate ontological types. The same Object may occupy different roles in different assessments, or multiple roles within the same assessment.

Contextual Roles allow the architecture to distinguish what an Object is from what it is doing in relation to an Assessed Action. This is essential because an Object may be an Actor in one assessment, an Affected Entity in another, an Observer in a third, and an Institutional Participant in a fourth.

#### Actor

An Actor is a contextual role assumed by an Object within a specific assessment when it initiates, controls, directs, authorizes, or bears responsibility for the Assessed Action.

An Actor may be a Moral Agent when moral responsibility is being assessed. In some cases, an Object may function as a causal or operational actor without satisfying the full criteria for moral responsibility. The architecture should therefore distinguish causal control, decision authority, authorization, and moral responsibility rather than assuming they always occur together.

#### Affected Entity

An Affected Entity is an Object whose state, relationships, constraints, opportunities, policy state, or Long-Term Flourishing may be changed by the Assessed Action.

Affected Entities may include the Actor, direct targets of the action, indirectly impacted entities, dependent entities, institutions, observers, and future entities whose relevant state space is altered by the action. Affected Entities are included in the assessment when their changes are material to the World Context Transition.

#### Observer

An Observer is an Object that perceives, learns about, interprets, or is otherwise exposed to the Assessed Action or its consequences.

Observers are architecturally important because actions can modify future decision policies beyond the Actor and directly affected entities. An Observer may update its understanding of what is acceptable, rewarded, punished, legitimate, effective, or repeatable. These updates may become part of the resulting World Context.

#### Responder

A Responder is an Object that reacts to the Assessed Action or to its consequences in a way that may further alter the World Context.

Responders may include individuals, institutions, communities, regulators, courts, markets, ecosystems, autonomous systems, or other agents that respond to the initial action. Their responses may amplify, mitigate, reverse, or transform the consequences of the Assessed Action.

#### Institutional Participant

An Institutional Participant is an Object acting within, through, on behalf of, or in relation to an institution.

Institutional Participants are important because institutions shape authority, legitimacy, obligations, incentives, norms, and future behavior. An action taken by an Institutional Participant may affect not only the participant and immediate targets, but also the credibility, trustworthiness, and policy state of the institution itself.

## Assessed Action

The Assessed Action is the behavior, decision, recommendation, intervention, omission, policy, command, or system output being morally evaluated.

The Assessed Action may be proposed, ongoing, or completed. It may be performed by a person, organization, institution, autonomous system, artificial agent, collective body, or other Actor. The Assessed Action is the change-generating element that transforms the initial World Context into a predicted or observed subsequent World Context.

In this architecture, the "means" used to pursue an objective are part of the Assessed Action. They are not external to moral assessment.

## Consequences

Consequences are the effects produced or predicted to be produced by the Assessed Action. They describe how the action changes the World Context.

Consequences may alter Object states, Association states, Long-Term Flourishing, policy states, institutions, constraints, information, authority conditions, future opportunities, and future state space. They may be immediate or delayed, direct or indirect, intended or unintended, certain or uncertain.

Consequences are evaluated across assessment horizons because an action may have different moral significance over different timeframes. Short-term benefits may create long-term harms, and short-term harms may sometimes enable long-term flourishing.

## State Variables / State Descriptors

State Variables or State Descriptors identify the properties of Objects, Associations, contexts, institutions, policies, opportunities, and evidence that may change through an Assessed Action.

At the Reference Architecture level, these are conceptual descriptors rather than prescribed mathematical variables. They indicate that the architecture must be capable of representing changes in relevant states, even though the precise representation belongs to the Moral Assessment Methodology or implementation.

Examples may include health, trust, capability, legitimacy, authority, dependency, access, resilience, adaptive capacity, knowledge, risk exposure, resource availability, institutional stability, and future opportunity.

## Policy States

Policy States describe the future decision tendencies, rules, strategies, norms, dispositions, learned behaviors, or action-selection patterns of Moral Agents, institutions, or other decision-capable systems.

A Policy State may belong to an individual person, organization, institution, AI system, autonomous agent, community, or other entity capable of adjusting future behavior. Policy States are architecturally important because actions may change what future agents perceive as acceptable, useful, rewarded, punished, legitimate, or repeatable.

Policy States provide the architectural basis for modeling how means affect future moral behavior. An action that achieves a beneficial immediate result may still damage future moral decision-making by shifting policy states toward coercion, deception, cruelty, negligence, corruption, or other harmful patterns.

## Distributed Policy Effects

Distributed Policy Effects are the changes an Assessed Action produces in the future decision policies of the Actor, affected entities, observers, responders, collaborators, institutions, or other relevant Moral Agents.

These effects are distributed because they are not limited to the Actor. A single action may teach observers that a harmful means is acceptable, alter institutional norms, create precedent, shift incentives, normalize abuse, or discourage future cooperation.

Distributed Policy Effects are part of the resulting World Context. They explain why the architecture treats the means used to achieve an outcome as morally significant, rather than evaluating only immediate consequences or aggregate results.

## Institutions

Institutions are persistent social, legal, organizational, procedural, cultural, or governance structures that shape behavior, authority, legitimacy, expectations, obligations, and collective decision-making.

Institutions may be represented as Objects, as networks of Associations, or as structured patterns involving multiple Objects and rules. They may include courts, governments, companies, families, professions, markets, schools, hospitals, regulatory bodies, protocols, and governance systems.

Institutions are architecturally important because actions may preserve, strengthen, weaken, corrupt, delegitimize, or transform them. Institutional changes may significantly affect Long-Term Flourishing across large populations and long assessment horizons.

## Information / Evidence State

Information or Evidence State describes what is known, believed, observable, recorded, available, unavailable, uncertain, hidden, distorted, or later discovered within an assessment.

Information State is broader than evidence used in a particular assessment. It may include knowledge possessed by the Actor, information reasonably obtainable through diligence, information available to an assessor, public knowledge, institutional records, misinformation, uncertainty, and missing evidence.

Information and Evidence State matter because moral assessment depends on what could reasonably be known within the Situational Context. They also affect confidence, responsibility, foreseeability, and the quality of predicted World Context transitions.

## Constraints

Constraints are conditions that limit, shape, or prohibit possible actions, outcomes, or state transitions.

Constraints may be physical, biological, legal, institutional, informational, technological, financial, temporal, relational, procedural, ecological, or moral. They define what actions are available, what consequences are possible, what obligations apply, and what tradeoffs must be considered.

Constraints are not automatically moral conclusions. A constraint may be morally justified, morally neutral, or morally problematic. The architecture represents constraints because they affect the available action space and the resulting World Context Transition.

## Authority and Legitimacy Conditions

Authority and Legitimacy Conditions describe whether an Actor, institution, or process has the recognized power, standing, permission, justification, or procedural validity to take an action.

Authority concerns whether an entity has the capacity or recognized right to act within a given context. Legitimacy concerns whether that authority is justified, accepted, procedurally valid, and compatible with the relevant moral and institutional context.

These conditions are architecturally important because actions taken without legitimate authority may damage trust, institutions, obligations, consent, and future cooperation even when they produce beneficial immediate outcomes.

## Future Opportunities

Future Opportunities are possible beneficial actions, relationships, capabilities, choices, adaptations, or developments that remain available, become available, or are foreclosed as a result of an Assessed Action.

Future Opportunities matter because Long-Term Flourishing depends not only on present state but also on the preservation and expansion of beneficial future possibilities. An action may be morally harmful if it unnecessarily forecloses important future options, even when its immediate consequences appear favorable.

Future Opportunities may apply to individuals, communities, institutions, ecosystems, artificial systems, or future generations.

## Future State Space

Future State Space is the set of possible future World Contexts that may become reachable from the current World Context.

The architecture treats Future State Space as morally significant because actions do not merely produce immediate outcomes; they expand, constrain, redirect, or foreclose future possibilities. A morally preferable transition should generally preserve or expand beneficial future state space for relevant Flourishing Entities while avoiding material diminishment of others.

Future State Space is broader than Future Opportunities. Future Opportunities refer to specific available possibilities, while Future State Space refers to the broader landscape of possible future configurations.

## Assessment Horizons

Assessment Horizons are the temporal frames over which the consequences of an Assessed Action are evaluated.

Default horizons include immediate, short-term, long-term, multi-generational, and civilizational timeframes. Additional horizons may be introduced when required by the domain or situation.

Assessment Horizons are necessary because consequences may differ substantially over time. The same action may increase flourishing in one horizon while diminishing it in another. As horizons extend farther into the future, uncertainty generally increases, and confidence should be adjusted accordingly in the Moral Assessment Methodology.

## World Context Transition

Architectural element and principal object of moral assessment. See **Reference Architecture → World Context Transition**.


