[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §6.1

*Moral Assessment Methodology. This layer defines how the architecture is used to perform an assessment.*

# Assessment Workflow

The Assessment Workflow describes the sequence through which the Moral Assessment Methodology applies the Reference Architecture to an Assessed Action. It provides a repeatable structure for moving from an initial World Context to a confidence-bounded moral assessment of the resulting World Context Transition.

The workflow should be understood as a methodological sequence rather than a mandatory software execution pipeline. Implementations may perform these steps iteratively, recursively, in parallel, or through domain-specific computational methods. A conforming implementation should preserve the meaning of each step even if the computational order varies.

At the highest level, the workflow is:

World Context\
→ Assessment Boundary\
→ Local and Situational Context\
→ Relevant Objects and Associations\
→ Objectives\
→ Assessed Action\
→ Predicted State Transition\
→ World Context Transition\
→ Moral Assessment

This sequence begins with the broadest possible state of the world and progressively narrows the assessment to the specific action, affected entities, relevant relationships, applicable objectives, predicted consequences, and final transition judgment. The purpose is not to produce certainty, but to produce a structured, inspectable, probabilistic assessment with explicit assumptions and confidence estimates.

## Establish the Initial World Context

The workflow begins by identifying the initial World Context: the complete theoretical state of the world at the moment the assessment begins.

In practice, the full World Context cannot be completely represented. The methodology therefore begins by identifying the available representation of the World Context, including known Objects, Associations, institutions, constraints, information states, policy states, future opportunities, and relevant uncertainties.

This step establishes the starting condition for the assessment. It should identify what is known, what is unknown, what is assumed, and what portions of the broader World Context may need to be excluded because of computational, evidentiary, or practical limits.

The initial World Context should include, where relevant:

Objects and Flourishing Entities that may be affected.

Associations among those Objects.

Current state descriptors for entities, relationships, institutions, and policies.

Existing constraints, obligations, authority structures, and legitimacy conditions.

Known information, missing information, uncertain evidence, and conflicting evidence.

Relevant future opportunities and current future state space.

The initial World Context is not yet the assessment. It is the starting state from which the assessment proceeds.

## Apply the Assessment Boundary

The next step is to apply the Assessment Boundary. The Assessment Boundary determines which portions of the World Context are included in the assessment and which are excluded or treated at lower resolution.

This step operationalizes the relevant scope structures. These may include domain scope, entity scope, causal scope, temporal scope, epistemic scope, perspective scope, jurisdictional scope, authority scope, and computational scope.

The Assessment Boundary should make explicit:

The class of assessment being performed.

The domain or domains involved.

The entities and relationships initially considered relevant.

The temporal horizons to be evaluated.

The causal range of consequences to be considered.

The evidence boundary for the assessment.

The perspective or authority position from which the assessment is being conducted.

The practical limits of representation or computation.

The Assessment Boundary should not be treated as a hidden assumption. If a boundary excludes a possible consequence, entity, time horizon, or evidence source, that exclusion should be visible and should affect the confidence of the resulting assessment when material.

## Derive the Local Context

The Local Context is the subset of the World Context relevant to a class or domain of moral assessments.

Although the compressed workflow sometimes moves directly from Assessment Boundary to Situational Context, the methodology should preserve the Local Context as an intermediate step when domain structure matters. This is especially important in healthcare, law, public policy, environmental stewardship, robotics, organizational governance, autonomous systems, and AI alignment.

The Local Context identifies the domain-relevant background for the assessment, including typical entity classes, relevant Associations, institutional norms, evidence standards, obligations, domain-specific risks, operational objectives, and applicable constraints.

For example, a medical ethics Local Context may include patient autonomy, clinical evidence, informed consent, professional responsibility, family relationships, and institutional care obligations. A legal Local Context may include precedent, authority, due process, jurisdiction, proportionality, legitimacy, and institutional trust.

The Local Context reduces the World Context to a domain-relevant field of assessment without yet narrowing the evaluation to a single action.

## Derive the Situational Context

The Situational Context is the subset of the Local Context directly relevant to the specific Assessed Action.

This step identifies the immediate state boundary for evaluation. It defines the situation in which the action occurs, the relevant Actors, the affected entities, the available alternatives, the applicable constraints, the operational objectives, and the evidence reasonably available for assessment.

The Situational Context should include:

The Actor or Actors involved.

Affected entities and potentially affected Flourishing Entities.

Relevant Associations among the Actor, affected entities, observers, responders, and institutions.

Material constraints, including legal, physical, informational, institutional, temporal, and moral constraints.

Available alternatives to the Assessed Action.

Known risks, uncertainties, and foreseeable consequences.

Relevant authority and legitimacy conditions.

Decision Context, Accessible Context, and Assessment Context, when responsibility and evidence quality must be distinguished.

The Situational Context is the primary evidentiary and state boundary for evaluating the action. If it is too narrow, the assessment may ignore material harms, affected entities, institutional effects, or Distributed Policy Effects. If it is too broad, the assessment may become analytically unfocused or computationally impractical.

## Identify Relevant Objects and Associations

Once the Situational Context has been established, the methodology identifies the relevant Objects and Associations within that context.

Relevant Objects are those whose states, relationships, opportunities, constraints, or flourishing may be materially affected by the Assessed Action. Relevant Associations are the morally significant relationships among those Objects, including responsibility, authority, obligation, dependency, trust, consent, ownership, care, governance, command, stewardship, legitimacy, or institutional membership.

This step should distinguish among:

Objects that are merely present in the context.

Flourishing Entities whose Long-Term Flourishing may be affected.

Moral Agents capable of decision, evaluation, and responsibility.

Actors who initiate, control, authorize, direct, or bear responsibility for the action.

Affected entities whose states may change.

Observers whose future policy states may be updated.

Responders whose reactions may further alter the World Context.

Institutions that may be strengthened, weakened, legitimized, corrupted, or transformed.

The purpose of this step is to identify the morally relevant structure of the assessment. Moral significance often arises not from isolated entities but from the relationships among them.

## Identify Relevant Flourishing Entities and Moral Agents

The methodology should explicitly identify which relevant Objects qualify as Flourishing Entities and which qualify as Moral Agents.

A Flourishing Entity is included when its Long-Term Flourishing can be meaningfully increased or diminished by the Assessed Action. A Moral Agent is included when an entity is capable of selecting among actions, evaluating those actions against objectives, and bearing moral responsibility.

This step is necessary because not all Objects are morally assessable in the same way. A rock may be an Object in the World Context, but it is not a Flourishing Entity. A corporation, ecosystem, human, animal, institution, or sufficiently self-directed artificial system may require assessment if its flourishing or future state space may be materially affected.

The methodology should identify:

Which Flourishing Entities are directly affected.

Which Flourishing Entities are indirectly affected.

Which Moral Agents are responsible for, observing, responding to, or learning from the action.

Whether the Actor is also an affected Flourishing Entity.

Whether future entities or future artificial systems fall within the assessment boundary.

This step supports later evaluation of Long-Term Flourishing, responsibility, and Distributed Policy Effects.

## Identify Objectives

The workflow then identifies the Objectives relevant to the assessment.

This includes both moral-system objectives and operational objectives. The moral-system objective is derived from the Foundational Axiom and concerns preserving and promoting Long-Term Flourishing while avoiding material diminishment of other relevant Flourishing Entities. Operational objectives are the specific goals pursued by the Actor, institution, system, or domain.

The methodology should distinguish:

The Foundational Axiom or moral-system objective.

Domain-specific objectives.

Operational objectives of the Actor.

Objectives of other relevant entities or institutions.

Conflicting objectives.

Objectives that may be achieved, frustrated, corrupted, or transformed by the action.

This distinction is essential because an operational objective cannot override the Foundational Axiom. An action may pursue a legitimate operational goal but still be morally deficient if the means or consequences materially diminish Long-Term Flourishing, corrupt policy states, damage institutions, or foreclose important future opportunities.

## Define the Assessed Action

The methodology then defines the Assessed Action with sufficient precision to evaluate it.

The term Assessed Action should be preferred over Proposed Action because the methodology may evaluate proposed, ongoing, completed, or omitted actions. The Assessed Action may be a behavior, decision, recommendation, intervention, omission, policy, command, system output, institutional decision, or autonomous action.

This step should identify:

What action is being assessed.

Whether the action is proposed, ongoing, completed, or omitted.

Who or what performs, authorizes, controls, directs, or bears responsibility for the action.

What means are used to pursue the operational objective.

What alternatives were reasonably available.

What constraints shaped the available action space.

What information was known, reasonably obtainable, or unavailable at the time of action.

The means used to pursue an objective are part of the Assessed Action. They must not be hidden inside the stated objective. For example, the Assessed Action should not be stated merely as "save the organization" if the actual action is "falsify financial statements to obtain emergency financing."

## Identify Available Alternatives

A moral assessment should identify the alternatives reasonably available within the Situational Context.

Alternatives are important because the moral status of an action often depends on whether less harmful, more legitimate, more transparent, or more flourishing-preserving options were available. The methodology does not require every imaginable alternative to be modeled. It requires that materially relevant alternatives be represented when they affect the assessment.

Alternatives may include:

Taking a different action.

Delaying action.

Seeking consent.

Escalating to a legitimate authority.

Disclosing information.

Choosing a less harmful means.

Adding safeguards.

Narrowing the scope of intervention.

Declining to act.

Intervening earlier or later.

This step supports responsibility assessment and comparative evaluation of candidate World Context Transitions.

## Represent Relevant State Variables

Before predicting the transition, the methodology identifies the state variables or state descriptors that may change.

These may include entity states, Association states, policy states, institutional states, information states, constraint states, opportunity states, and future state-space descriptors. At this stage, the methodology identifies what must be tracked for the assessment to preserve fidelity.

Relevant state descriptors may include:

Health, safety, autonomy, capability, access, resources, resilience, and adaptive capacity.

Trust, legitimacy, authority, obligation, dependency, consent, and responsibility.

Institutional stability, precedent, accountability, enforcement pattern, and public confidence.

Information quality, evidence availability, misinformation, uncertainty, and record integrity.

Policy states of Actors, observers, responders, institutions, and artificial systems.

Future opportunities and reachable future state space.

Long-Term Flourishing dimensions relevant to the entities being assessed.

This step prepares the assessment for state-transition modeling without requiring the Reference Architecture to prescribe a particular mathematical representation.

## Predict Consequences Across Assessment Horizons

The methodology then predicts or identifies the Consequences of the Assessed Action across relevant Assessment Horizons.

The default horizons include immediate, short-term, long-term, multi-generational, and civilizational timeframes, with additional horizons added when required by the context. The assessment should not assume that consequences have the same moral significance across all horizons.

This step should consider:

Direct consequences.

Indirect consequences.

Intended consequences.

Unintended consequences.

Foreseeable consequences.

Uncertain or contested consequences.

Consequences to Objects.

Consequences to Associations.

Consequences to Long-Term Flourishing.

Consequences to institutions.

Consequences to information and evidence state.

Consequences to constraints.

Consequences to future opportunities and future state space.

Consequences to policy states.

Predicted consequences should include both expected effects and material risks. Low-probability consequences may still be relevant when the potential harm is severe or irreversible.

## Estimate Distributed Policy Updates

The methodology should explicitly estimate Distributed Policy Updates as part of the predicted state transition.

These updates describe how the Assessed Action may change the future decision policies of the Actor, affected entities, observers, responders, institutions, and artificial systems. Distributed Policy Updates are essential because they explain why harmful means may degrade future moral decision-making even when immediate outcomes appear beneficial.

This step should consider whether the action:

Makes the Actor more likely to repeat similar means.

Teaches observers that the means are acceptable, rewarded, tolerated, or legitimate.

Changes institutional precedent or enforcement expectations.

Alters the trust, cooperation, resistance, or compliance behavior of affected entities.

Updates the behavior of autonomous or artificial systems.

Normalizes, discourages, reinforces, or corrupts future decision policies.

Distributed Policy Updates are not merely explanatory commentary. They are state changes in the resulting World Context.

## Estimate Long-Term Flourishing Transitions

The methodology then estimates how the Assessed Action changes the Long-Term Flourishing of relevant Flourishing Entities.

Long-Term Flourishing should be evaluated across the relevant horizons and across the dimensions relevant to each entity. Candidate dimensions may include persistence, adaptive capacity, future possibilities, constructive participation, resilience, agency, relational stability, environmental compatibility, and contribution to the larger relevant World Context.

This step should distinguish:

Which entities experience increased flourishing.

Which entities experience diminished flourishing.

Which entities experience mixed effects.

Which effects are immediate versus long-term.

Which effects are uncertain.

Whether any entity's flourishing is materially diminished.

Whether apparent expansion is actually flourishing or merely growth, power, replication, or control.

Flourishing transitions should inform the assessment, but they should not replace the broader World Context Transition.

## Estimate Aggregate Flourishing Effects

The methodology may estimate aggregate flourishing effects across relevant Flourishing Entities.

Aggregate flourishing can help summarize the direction, magnitude, and distribution of impact. It may support comparison among candidate actions, prioritization of risks, or structured reporting. However, aggregate flourishing is not the moral assessment itself.

This step should avoid hiding morally significant structure. A positive aggregate change may conceal severe harm to a vulnerable entity, corruption of institutional legitimacy, degradation of policy states, or loss of future state space. A negative short-term aggregate change may sometimes accompany a transition that preserves long-term flourishing.

Aggregate effects should therefore be treated as informative assessment artifacts, not as substitutes for the World Context Transition.

## Construct the Predicted State Transition

The Predicted State Transition integrates the expected consequences, state changes, Long-Term Flourishing transitions, Distributed Policy Updates, and horizon-specific effects into a coherent transition model.

This step describes how the initial relevant state is expected to change if the Assessed Action occurs, continues, or is treated as completed. It may include multiple candidate transitions when several outcomes are plausible or when comparing alternative actions.

The Predicted State Transition should include:

Predicted changes to entity states.

Predicted changes to Association states.

Predicted changes to institutional states.

Predicted changes to information and evidence states.

Predicted changes to constraints and authority conditions.

Predicted changes to future opportunities.

Predicted changes to future state space.

Predicted changes to policy states.

Predicted changes to Long-Term Flourishing.

Uncertainty and confidence associated with each material prediction.

This step is the methodological bridge between consequence identification and World Context Transition evaluation.

## Construct the World Context Transition

The World Context Transition represents the transformation from the initial World Context to the resulting World Context after the Assessed Action and its consequences are considered.

This is the principal object of moral assessment. The methodology should not collapse this transition into a single score, a single consequence, a single objective, or a simple aggregate flourishing value.

The World Context Transition should include all material changes identified in the workflow:

Objects and Flourishing Entities.

Associations.

Moral Agents and contextual roles.

Operational and moral-system objectives.

Consequences.

Long-Term Flourishing transitions.

Distributed Policy Updates.

Information and evidence state.

Institutions.

Constraints.

Authority and legitimacy conditions.

Future opportunities.

Future state space.

Assessment horizons.

Confidence and uncertainty.

The resulting World Context becomes the starting condition for future assessments. This recursive feature must be preserved because actions alter the moral conditions under which later actions will be evaluated.

## Evaluate Against the Foundational Axiom

The methodology then evaluates the World Context Transition against the Foundational Axiom.

This evaluation asks whether the transition preserves and promotes the Long-Term Flourishing of relevant Flourishing Entities---including the sustained capacity of the contexts, at every tier, that enable it---and fosters the adaptive development of moral agents, while avoiding actions that, based on the best available evidence within the Situational Context, materially diminish the Long-Term Flourishing of other relevant Flourishing Entities.

This step should consider:

Whether the Assessed Action promotes Long-Term Flourishing.

Whether any relevant Flourishing Entity is materially diminished.

Whether the sustained capacity of any affected context is diminished, and---where contexts at different tiers genuinely conflict---whether the axiom's tier priority and the anti-sacrifice corollary have been applied as §4.7 requires.

Whether the action fosters or degrades the adaptive development of the moral agents involved.

Whether the means used corrupt future policy states.

Whether the action damages legitimate Associations or institutions.

Whether future opportunities or future state space are preserved, expanded, narrowed, or foreclosed.

Whether the Actor's operational objective remains subordinate to the moral-system objective.

Whether the assessment changes across horizons.

Whether uncertainty materially limits confidence.

The Foundational Axiom provides the normative direction for assessment, but the evaluation remains grounded in the World Context Transition.

## Produce the Moral Assessment

The final step is to produce the Moral Assessment.

The Moral Assessment should be a structured, confidence-bounded result that explains how the Assessed Action transforms the World Context and how that transition should be evaluated under the framework.

The assessment may include:

Assessment summary.

Assessed Action.

Actor or Actors.

Relevant Objects and Associations.

Relevant Flourishing Entities and Moral Agents.

Operational objectives and moral-system objectives.

Assessment Boundary and scope assumptions.

Situational Context.

Relevant alternatives.

Predicted or observed Consequences.

Long-Term Flourishing transitions.

Distributed Policy Updates.

World Context Transition summary.

Aggregate flourishing effects, if calculated.

Confidence estimates.

Evidence references.

Known assumptions.

Unresolved uncertainties.

Decision-support recommendation, permissibility judgment, risk flag, or comparative ranking, where appropriate.

The Moral Assessment should distinguish the assessment result from the evidence, assumptions, predictions, and confidence values that support it. This preserves transparency and allows later review, audit, revision, or comparison.

## Handle Confidence, Uncertainty, and Revision

The workflow should explicitly represent uncertainty at every stage.

Uncertainty may arise from incomplete information, unreliable evidence, ambiguous context boundaries, contested causal relationships, model limitations, prediction uncertainty, long assessment horizons, or unknown future responses. The methodology should propagate these uncertainties into the final confidence estimate.

When new evidence becomes available, the assessment may be revised. A proposed-action assessment may later become an ongoing-action assessment or a completed-action assessment. A completed-action assessment may still be revised as later consequences, policy effects, or institutional impacts become visible.

The workflow therefore supports continuous refinement without requiring the Reference Architecture to change.

## Workflow Summary

The expanded Assessment Workflow can be summarized as follows:

1.  Establish the initial World Context.

2.  Apply the Assessment Boundary.

3.  Derive the Local Context.

4.  Derive the Situational Context.

5.  Identify relevant Objects and Associations.

6.  Identify relevant Flourishing Entities and Moral Agents.

7.  Identify moral-system and operational Objectives.

8.  Define the Assessed Action.

9.  Identify available alternatives.

10. Represent relevant state variables.

11. Predict consequences across Assessment Horizons.

12. Estimate Distributed Policy Updates.

13. Estimate Long-Term Flourishing transitions.

14. Estimate aggregate flourishing effects where useful.

15. Construct the Predicted State Transition.

16. Construct the World Context Transition.

17. Evaluate the transition against the Foundational Axiom.

18. Produce the Moral Assessment.

19. Report confidence, uncertainty, assumptions, and evidence.

20. Revise the assessment when new evidence or outcomes become available.

This expanded workflow preserves the compressed architecture-level sequence while adding the methodological fidelity required for actual assessment.

