[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §6.3

*Moral Assessment Methodology. This layer defines how the architecture is used to perform an assessment.*

# State Representation

State Representation defines how the Moral Assessment Methodology describes the condition of the relevant World Context before and after an Assessed Action. The Reference Architecture identifies what exists; State Representation identifies which aspects of those elements must be represented so that change can be evaluated.

A moral assessment requires more than identifying Objects, Associations, Actors, Objectives, and Consequences. It must also describe the state of those elements at the beginning of the assessment, estimate how those states may change, and evaluate the significance of those changes. State Representation therefore provides the methodological foundation for State Transition modeling, Long-Term Flourishing assessment, Distributed Policy Updates, confidence estimation, and World Context Transition evaluation.

State Representation does not require that every possible feature of the world be represented at full resolution. The World Context is theoretically complete, but practical assessment requires abstraction. The methodology should represent the state variables that are material to the assessment, identify the variables that are uncertain or unavailable, and disclose the confidence limits created by those gaps.

## Purpose of State Representation

The purpose of State Representation is to make moral assessment inspectable and computationally representable.

Without state representation, the framework could describe moral concepts in narrative form but could not evaluate how an Assessed Action changes the World Context. State Representation allows the methodology to identify the relevant pre-action state, estimate the post-action state, compare those states, and produce a structured assessment of the transition.

State Representation supports several methodological functions:

It identifies the initial condition of relevant Objects, Associations, institutions, information states, policy states, and future opportunities.

It identifies which variables may change as a result of the Assessed Action.

It supports prediction of State Transitions.

It supports estimation of Long-Term Flourishing changes.

It supports evaluation of Distributed Policy Updates.

It supports confidence estimation by identifying uncertainty in evidence, representation, and prediction.

It supports auditability by making assumptions and intermediate representations visible.

State Representation therefore acts as the bridge between the conceptual architecture and the evaluative methodology.

## State Variables

A state variable is a represented attribute, condition, descriptor, or property of an architectural element that may be relevant to moral assessment.

State variables may describe Objects, Associations, institutions, policy states, information states, constraints, authority conditions, opportunities, or the broader World Context. A state variable is included when a change in that variable may materially affect the assessment of the Assessed Action.

Examples of possible state variables include health, safety, autonomy, trust, legitimacy, authority, consent, dependency, obligation, knowledge, uncertainty, resilience, adaptive capacity, access, resource availability, institutional stability, evidence quality, policy tendency, future opportunity, and risk exposure.

State variables may be quantitative, qualitative, ordinal, categorical, probabilistic, narrative, relational, or symbolic. The methodology should not require all state variables to be reducible to precise numbers. Some variables may be represented through structured categories, confidence-bounded estimates, or qualitative descriptors when quantitative measurement is not practical or justified.

A state variable should be explicit enough that an assessor can identify:

What is being represented.

Which architectural element it belongs to.

Why it is relevant.

How it is known or estimated.

Whether it is uncertain.

How it may change through the Assessed Action.

State variables should be selected based on materiality to the World Context Transition, not merely because data happens to be available.

## Baseline State

The baseline state is the represented state of the relevant World Context before the Assessed Action occurs or before the assessment begins.

The baseline state provides the reference point for evaluating change. Without a baseline, the methodology cannot distinguish between conditions that already existed and conditions caused, worsened, improved, or made more probable by the Assessed Action.

The baseline state should represent the relevant condition of:

Relevant Objects.

Relevant Associations.

Relevant Flourishing Entities.

Moral Agents and Actors.

Institutions.

Information and evidence.

Constraints.

Authority and legitimacy conditions.

Policy states.

Future opportunities.

Future state space.

The baseline state may itself be uncertain. When the pre-action state is incomplete, disputed, or only partially observable, that uncertainty should be represented explicitly rather than hidden. Baseline uncertainty affects the confidence of any predicted or observed State Transition.

## Entity State Vectors

An Entity State Vector represents the relevant state of an Object or Flourishing Entity within the assessment.

The term "vector" is used here to indicate a structured collection of state descriptors, not necessarily a prescribed mathematical form. The precise formal representation may vary by methodology or implementation. At this level, the requirement is that relevant entity conditions be represented in a way that can support comparison before and after an Assessed Action.

An Entity State Vector may include dimensions such as:

Physical condition.

Health or biological integrity.

Safety.

Autonomy.

Agency.

Knowledge.

Capability.

Resource access.

Social connection.

Legal status.

Institutional role.

Vulnerability.

Resilience.

Adaptive capacity.

Future opportunities.

Long-Term Flourishing dimensions.

For a human patient, the entity state vector might include health status, decision capacity, informed consent, treatment options, family dependency, and future quality of life. For an ecosystem, it might include biodiversity, resilience, ecological connectivity, invasive species pressure, regenerative capacity, and long-term stability. For an institution, it might include legitimacy, trust, authority, procedural integrity, capability, accountability, and policy state.

Entity State Vectors should be tailored to the type of entity and the Situational Context. Different entities may share some dimensions while requiring different relevance weights, descriptors, or interpretations. A state variable that is material for a human may not be material in the same way for an ecosystem, institution, or artificial system.

## Flourishing State Representation

Because Long-Term Flourishing is central to the methodology, the state of relevant Flourishing Entities should include a representation of flourishing-related dimensions.

Flourishing State Representation describes the current and predicted capacity of a Flourishing Entity to persist, adapt, develop, preserve beneficial future opportunities, and participate constructively in the larger relevant World Context. It should not be reduced to mere survival, expansion, preference satisfaction, short-term benefit, or power.

Candidate flourishing dimensions may include Persistence, Adaptive Capacity, Future Possibilities, Constructive Participation, resilience, agency, relational integrity, environmental compatibility, and contribution to the larger system. The precise set of dimensions remains open to refinement and may vary by entity type and assessment domain.

The methodology should distinguish flourishing from expansion. A system may expand while diminishing the flourishing of others or degrading the broader World Context. Conversely, a temporary contraction or restraint may preserve long-term flourishing.

Flourishing State Representation is developed further in Section 6.6, but it must be introduced here because it is one of the primary state representations used in moral assessment.

## Relationship State Variables

Relationship State Variables represent the state of Associations among Objects.

Associations are morally significant because many duties, vulnerabilities, dependencies, authorities, and expectations arise through relationships rather than through isolated entities. Relationship state variables therefore capture how the Assessed Action may change the connections among relevant Objects.

Examples of relationship state variables include:

Trust.

Authority.

Legitimacy.

Consent.

Obligation.

Dependency.

Responsibility.

Care.

Stewardship.

Ownership.

Contractual status.

Command relationship.

Representation.

Reliance.

Cooperation.

Conflict.

Institutional membership.

A medical decision may change trust between patient and physician. A legal decision may change legitimacy between citizen and court. A corporate action may change obligation and trust between employer and employee. An environmental intervention may change stewardship obligations between a community and ecosystem.

Relationship State Variables should be represented explicitly because moral harms and benefits often appear first as relational changes. A narrow entity-state analysis may miss the moral significance of damaged trust, violated consent, corrupted authority, or weakened obligation.

## Policy State Variables

Policy State Variables represent the future decision tendencies, rules, habits, norms, strategies, incentives, learned behaviors, or action-selection patterns of Moral Agents, institutions, artificial systems, and other decision-capable entities.

Policy states are central to Distributed Policy Updates. They describe how an Assessed Action changes what future agents are likely to do. An action may make a harmful means more likely to be repeated, make observers more likely to imitate the behavior, or make institutions more likely to encode the behavior as precedent.

Policy state variables may describe:

Propensity to repeat the Assessed Action.

Tolerance for harmful means.

Commitment to transparency.

Reliance on coercion.

Likelihood of deception.

Responsiveness to evidence.

Respect for consent.

Deference to legitimate authority.

Trust in institutions.

Risk tolerance.

Compliance behavior.

Retaliatory tendency.

Cooperation tendency.

Institutional enforcement pattern.

Artificial system action-selection behavior.

Policy State Variables may be explicit, such as written rules or system parameters, or implicit, such as habits, incentives, norms, or learned behavioral tendencies. The methodology should represent policy states when they materially affect future World Contexts.

## Institutional State Variables

Institutional State Variables represent the condition of institutions within the assessment.

Institutions may be formal or informal, public or private, human or artificial, centralized or distributed. Their states matter because institutions shape authority, legitimacy, incentives, accountability, norms, resource allocation, and future decision behavior.

Institutional state variables may include:

Legitimacy.

Public trust.

Procedural integrity.

Accountability.

Authority recognition.

Rule consistency.

Enforcement reliability.

Transparency.

Corruption level.

Competence.

Resilience.

Institutional memory.

Norm stability.

Policy precedent.

Capacity to correct errors.

An Assessed Action may preserve, strengthen, weaken, corrupt, delegitimize, bypass, or transform an institution. These changes may be especially significant across long-term, multi-generational, and civilizational horizons.

Institutional states should be represented separately when they are not adequately captured by individual entity states or relationship states.

## Constraint State Variables

Constraint State Variables represent limits, requirements, prohibitions, or enabling conditions that shape available actions and possible transitions.

Constraints may be physical, biological, legal, institutional, technological, informational, financial, temporal, ecological, procedural, relational, or moral. They affect what actions are possible, what alternatives are available, what risks are unavoidable, and what obligations apply.

Constraint state variables may include:

Available time.

Available resources.

Legal restrictions.

Technical limitations.

Physical feasibility.

Medical limitations.

Environmental conditions.

Institutional authority.

Information access.

Safety requirements.

Consent requirements.

Emergency conditions.

Computational limits.

An Assessed Action may alter constraints by creating new limitations, removing existing limitations, expanding available choices, narrowing future action space, or changing what is feasible for future agents.

## Opportunity State Variables

Opportunity State Variables represent beneficial possibilities available to relevant Flourishing Entities or Moral Agents.

Future Opportunities are important because Long-Term Flourishing depends partly on the preservation and expansion of beneficial future possibilities. Opportunity state variables therefore capture what options, adaptations, relationships, capabilities, and developmental pathways remain available before and after the Assessed Action.

Opportunity state variables may include:

Treatment options.

Educational opportunities.

Economic mobility.

Relationship repair.

Institutional reform.

Ecological recovery.

Technological development.

Future cooperation.

Ability to exit harmful conditions.

Ability to seek help.

Capacity for adaptation.

Access to alternative actions.

Preservation of future agency.

An action may produce immediate benefit while foreclosing important future opportunities. Conversely, an action may impose immediate cost while preserving critical future options.

## World Context State

World Context State is the integrated state of the relevant portion of the World Context represented for assessment.

It includes the combined state of relevant Objects, Associations, institutions, constraints, information, policy states, future opportunities, future state space, and other context-specific variables. It is the methodological representation of the world-state used to evaluate the Assessed Action.

World Context State should not be treated as merely the sum of isolated entity states. It includes relational, systemic, institutional, informational, and future-oriented structure. A World Context may worsen even if some individual variables improve, because the relational or institutional structure has been damaged. Similarly, a World Context may improve even if some short-term burdens occur, because long-term resilience, trust, legitimacy, or future state space has been preserved.

The methodology should distinguish:

Initial World Context State.

Predicted World Context State.

Observed World Context State.

Revised World Context State.

Alternative World Context States under different candidate actions.

This distinction supports prospective assessment, retrospective review, comparison among alternatives, and continuous refinement.

## Information State

Information State represents what is known, unknown, believed, uncertain, hidden, available, unavailable, distorted, recorded, or contested within the assessment.

Information State may include the Actor's Decision Context, the Accessible Context, the Assessment Context, evidence quality, evidence provenance, evidence completeness, evidence conflicts, model assumptions, and known uncertainties.

Information State is itself part of the World Context. An Assessed Action may improve the Information State by producing transparency, documentation, explanation, or reliable evidence. It may degrade the Information State through deception, concealment, misinformation, destruction of records, ambiguity, or epistemic negligence.

Because future moral assessment depends on information quality, changes to Information State may have direct moral significance. A harmful Information State can reduce future decision quality, weaken accountability, damage trust, and impair future World Context evaluation.

## Uncertainty State

Uncertainty State represents the degree and source of uncertainty associated with the state variables used in the assessment.

Uncertainty may arise from incomplete evidence, ambiguous definitions, measurement limitations, conflicting information, causal uncertainty, model uncertainty, prediction uncertainty, unknown future responses, computational limits, or long assessment horizons.

The methodology should represent uncertainty explicitly rather than hiding it inside a final conclusion. Each material state variable may have its own uncertainty profile. The final assessment may have different confidence levels for different claims, such as what happened, what was foreseeable, which entities were affected, how flourishing changed, and how policy states may evolve.

Uncertainty State may include:

Known unknowns.

Evidence gaps.

Confidence in baseline state.

Confidence in predicted transition.

Confidence in observed outcomes.

Confidence in causal attribution.

Confidence in Long-Term Flourishing estimates.

Confidence in Distributed Policy Updates.

Confidence across different Assessment Horizons.

The methodology should carry uncertainty forward into the State Transition Model and the final Moral Assessment.

## Temporal State Representation

State variables should be represented across relevant Assessment Horizons.

The same variable may change differently across immediate, short-term, long-term, multi-generational, and civilizational horizons. A state may improve immediately but deteriorate later, or worsen temporarily while improving long-term adaptive capacity.

For example, a medical intervention may reduce immediate risk but create long-term dependency. A legal decision may impose immediate punishment while improving long-term institutional trust. A deceptive institutional action may preserve short-term stability while degrading future legitimacy.

Temporal State Representation allows the methodology to evaluate horizon-dependent effects without collapsing them into a single undifferentiated outcome.

## Granularity of State Representation

State Representation must be detailed enough to capture morally material changes, but not so detailed that assessment becomes impossible.

Granularity should be determined by the Assessment Boundary, materiality, evidence quality, computational feasibility, and the expected significance of the variable to the World Context Transition. Some assessments may require coarse state categories. Others may require detailed, domain-specific state variables.

For example, an emergency assessment may represent a patient's state using urgent survival indicators. A retrospective medical ethics assessment may require a more detailed representation of diagnosis, consent, risk disclosure, treatment alternatives, family dependency, and institutional procedures.

The methodology should allow state representations to be refined when finer detail materially improves assessment quality.

## Materiality and State Selection

Not every possible state variable should be included in every assessment.

A state variable should be represented when it is material to evaluating the Assessed Action, the predicted State Transition, the Long-Term Flourishing of relevant entities, the condition of important Associations, Distributed Policy Updates, or the resulting World Context Transition.

Materiality may depend on severity, probability, duration, reversibility, affected entities, institutional significance, impact on future opportunities, impact on policy states, or impact on confidence. A low-probability state change may still be material if the potential consequence is severe or irreversible.

The methodology should identify why a state variable is included and should avoid allowing data availability alone to determine relevance.

## Cross-Entity Comparability

State variables may be shared across different entities, but they may not carry the same meaning, relevance, or moral weight for every entity.

For example, persistence, adaptive capacity, resilience, and future opportunities may be relevant to humans, ecosystems, institutions, and artificial systems, but the interpretation of those variables differs by entity type. A state change that materially diminishes a human may not have the same significance for a tree, an institution, or an artificial system, and vice versa.

The methodology should therefore support shared state dimensions where useful while preserving entity-specific interpretation. This is especially important for Long-Term Flourishing assessment across humans, non-human organisms, ecosystems, organizations, institutions, and future artificial systems.

## State Representation and Long-Term Flourishing

Long-Term Flourishing is represented as a multidimensional relational state of relevant Flourishing Entities.

The State Representation section prepares for the Long-Term Flourishing Model by identifying the entity, relationship, policy, opportunity, and World Context states that may contribute to flourishing. Section 6.6 develops the flourishing model more directly.

At this stage, the requirement is that State Representation preserve the variables needed to assess whether Long-Term Flourishing is preserved, promoted, diminished, or made uncertain. This includes not only internal entity condition, but also relational, institutional, environmental, informational, and future-oriented conditions.

## State Representation and Distributed Policy Updates

Distributed Policy Updates require explicit representation of Policy State Variables before and after the Assessed Action.

The methodology should represent the relevant policy states of the Actor, affected entities, observers, responders, institutions, and artificial systems when those policy states may materially change. This allows the assessment to evaluate how the means used in an action affect future moral decision-making.

For example, an action that relies on deception may change the Actor's propensity to deceive, observers' expectations about acceptable conduct, and institutional norms regarding truthfulness. These changes must be represented as state changes, not merely as narrative commentary.

## State Representation and Confidence

State Representation directly affects confidence.

An assessment based on well-defined, well-evidenced, relevant state variables can support higher confidence than an assessment based on vague, incomplete, contested, or poorly measured variables. Conversely, when important state variables are missing, uncertain, or only weakly represented, the final assessment should disclose lower confidence.

Confidence should be affected by:

Completeness of state representation.

Quality of evidence supporting state variables.

Stability of variable definitions.

Measurement uncertainty.

Entity-specific interpretation uncertainty.

Temporal uncertainty.

Causal uncertainty.

Prediction uncertainty.

Computational limits.

State confidence should be propagated into transition confidence and final assessment confidence.

## Representation Format

The methodology does not prescribe one required representation format.

State may be represented through structured tables, graphs, ontologies, vectors, categories, narratives, probabilistic distributions, symbolic descriptors, model parameters, or future computational representations. Different implementations may choose different formats depending on domain, evidence quality, computational requirements, and audit needs.

The methodological requirement is not that all states be numerical. The requirement is that state representations be explicit, inspectable, comparable across the relevant transition, and capable of supporting confidence-bounded moral assessment.

## Minimum State Representation Requirements

A minimally adequate assessment should represent:

The relevant baseline World Context State.

The relevant Objects and their material states.

The relevant Associations and their material states.

The relevant Flourishing Entities and flourishing-related states.

The relevant Moral Agents and their policy states when material.

The relevant institutions and institutional states.

The relevant constraints and authority conditions.

The relevant Information and Evidence State.

The relevant uncertainty associated with material variables.

The future opportunities or future state-space conditions affected by the action.

The predicted or observed post-action state.

The transition between baseline and post-action states.

If any of these are omitted because they are unavailable, immaterial, or computationally infeasible, the assessment should state the omission and reflect it in confidence where appropriate.

## Methodological Boundary

This section defines the kinds of state representation required for moral assessment. It does not prescribe a specific mathematical notation, database schema, graph representation, scoring method, vector formalism, or implementation architecture.

Those details may be developed in later methodology sections, appendices, or implementation guidance. The requirement at this level is that the methodology represent morally material states explicitly enough to support State Transition modeling, Long-Term Flourishing assessment, Distributed Policy Updates, uncertainty propagation, and evaluation of the World Context Transition.

