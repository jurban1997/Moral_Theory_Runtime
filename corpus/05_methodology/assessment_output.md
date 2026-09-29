[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §6.14

*Moral Assessment Methodology. This layer defines how the architecture is used to perform an assessment.*

# Assessment Output

Assessment Output defines the form and content of the result produced by the Moral Assessment Methodology after evaluating an Assessed Action.

The output of an assessment should not be limited to a moral label, score, recommendation, or conclusion. A moral assessment is useful only if the reasoning behind it remains inspectable. The output should therefore preserve the structured path from the initial World Context to the resulting World Context, including evidence, assumptions, affected entities, state transitions, flourishing transitions, policy updates, uncertainty, and confidence.

The Assessment Output is the methodological artifact that allows the assessment to be reviewed, audited, revised, compared, explained, or used by downstream decision-support systems. It is not merely a narrative summary. It is a structured representation of the assessment result and the reasoning artifacts that support it.


## Multidimensional Assessment Axes

A conforming assessment reports **separate findings on each moral axis** below. Axis findings may conflict; conflict must remain visible in the output. Integrative summaries are permitted for decision support but must not replace axis-specific reasoning. See **Reference Architecture → Normative Kernel and Ethical Profiles → Integration Protocol**.

  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Axis                                       Principal question                                                                                            Illustrative outputs
  ------------------------------------------ ------------------------------------------------------------------------------------------------------------- -----------------------------------------------------------------------------------------------------
  **Action and means permissibility**        Was the action required, permitted, or prohibited considering its means and applicable constraints?         Required; permissible; conditionally permissible; impermissible; tragically necessary

  **Agent intention and responsibility**     What did the agent intend, know, control, foresee, and have capacity to do differently?                       Responsible; partially responsible; negligent; reckless; excused; nonculpable; indeterminate

  **Relational and procedural legitimacy**   Were relationships, consent, authority, participation, care, and due process adequate?                        Legitimate; qualified; procedurally deficient; relationally harmful; illegitimate; indeterminate

  **Transition quality**                     What World Context Transition occurred or is expected, and how are benefits and harms distributed?           Beneficial; supportable; mixed; detrimental; catastrophic; uncertain

  **Remedy obligations**                     What must now be prevented, repaired, restored, compensated, acknowledged, or monitored?                    None; monitor; mitigate; cease; explain; apologize; compensate; restore; reform; combinations
  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Each axis report includes:

- Applicable normative kernel criteria and active ethical profiles;

- Affected entities and Associations;

- Supporting evidence and material assumptions;

- Axis-specific confidence level;

- Dissenting or minority interpretation when present;

- Interaction notes when one axis constrains another (for example, impermissible means despite favorable transition quality); and

- Reassessment triggers when new evidence arrives.

**Minimum integrative rule:** no overall "supportable" recommendation when any axis reports **impermissible** means, **illegitimate** procedure, or **catastrophic** transition quality unless explicitly flagged as unresolved conflict requiring escalation.

When the assessment supports a decision among candidate actions, selection from the axis findings --- and the escalation of conflicts they leave unresolved --- is governed by the **Conflict-Resolution Decision Model** (§6.15).

Theory-discriminating scenarios that test axis separation appear in §9.4.6 (*Multiple Objects and Axes of Moral Assessment*).

## Purpose of Assessment Output

The purpose of Assessment Output is to make the result of a moral assessment explicit, traceable, and usable.

A completed assessment should show not only what conclusion was reached, but how that conclusion was reached. It should identify the Assessed Action, the relevant context, the affected entities, the evidence used, the assumptions made, the intermediate results produced, the predicted or observed World Context Transition, the confidence level, and any recommendations or decision-support flags.

Assessment Output supports several functions:

It communicates the assessment result.

It preserves the reasoning path.

It exposes evidence and assumptions.

It reports confidence and uncertainty.

It identifies affected entities and Associations.

It summarizes the World Context Transition.

It records Long-Term Flourishing changes.

It records Distributed Policy Updates.

It supports comparison among candidate actions.

It supports audit, explanation, revision, and downstream implementation.

The output should be structured enough to support computational use while remaining understandable enough to support human review.

## Assessment Result

The Assessment Result is the primary conclusion produced by the methodology.

The result should summarize the moral status of the Assessed Action in relation to the resulting World Context Transition. It should not be presented as an unsupported verdict. It should remain traceable to the evidence, assumptions, intermediate results, and confidence estimates that support it.

An Assessment Result may take several forms, depending on the domain, implementation, and assessment purpose. It may indicate that the Assessed Action is morally supportable, morally harmful, impermissible, conditionally permissible, preferable to available alternatives, inferior to available alternatives, mixed, inconclusive, confidence-limited, or requiring mitigation.

The methodology should allow assessment results such as:

Morally supportable with stated confidence.

Morally harmful with stated confidence.

Conditionally supportable if specified safeguards are added.

Not supportable because of material diminishment.

Not supportable because of detrimental policy updates.

Inconclusive because of insufficient evidence.

Requires escalation or human review.

Requires additional evidence before action.

Preferable to listed alternatives under current assumptions.

Permissible only within stated Assessment Boundary limits.

The Assessment Result should be concise, but it should not hide the complexity of the assessment. When the result is mixed or horizon-dependent, the output should say so explicitly.

## Result Classification

A result classification provides a structured category for the assessment result.

The methodology does not require a single fixed classification system, but it should support consistent result categories within a given implementation or domain. Classification allows assessments to be compared, filtered, audited, or routed to downstream systems.

Possible classification families include:

Supportability classification.

Risk classification.

Permissibility classification.

Recommendation classification.

Comparative ranking.

Escalation classification.

Uncertainty classification.

Material-diminishment classification.

Policy-update classification.

A classification should be treated as a summary of the underlying assessment, not as a replacement for it. A classification such as "supportable" or "not supportable" should remain connected to the World Context Transition and confidence level that justify it.

## Confidence Level

Every Assessment Output should include a confidence level.

The confidence level represents the reliability of the assessment result given the available evidence, assumptions, state representation, causal model, probability estimates, prediction uncertainty, model uncertainty, incomplete information, and horizon-specific uncertainty.

Confidence should not be treated as a decorative number attached to the conclusion. It is a substantive part of the assessment. A low-confidence recommendation should not be treated the same as a high-confidence recommendation. A high-confidence harmful assessment should trigger different decision support than a low-confidence harmful assessment. A low-confidence beneficial assessment may require additional evidence, safeguards, or escalation.

The output should identify:

Overall confidence in the Assessment Result.

Confidence in the baseline World Context.

Confidence in the predicted or observed State Transition.

Confidence in Long-Term Flourishing estimates.

Confidence in Distributed Policy Updates.

Confidence in Aggregate Flourishing estimates, if used.

Confidence in the World Context Transition.

Confidence by Assessment Horizon.

Major sources of confidence reduction.

The methodology should avoid hiding multiple uncertainties inside a single confidence value when those uncertainties materially affect the assessment.

## Confidence Explanation

The Assessment Output should explain why the confidence level has been assigned.

A confidence value without explanation may create false precision. The output should identify the major evidence strengths, evidence weaknesses, missing information, model limitations, prediction uncertainties, and scope constraints that affect confidence.

A confidence explanation may state that confidence is high because evidence is direct, complete, recent, consistent, and supported by reliable domain knowledge. It may state that confidence is moderate because the immediate consequences are well understood but long-term policy effects remain uncertain. It may state that confidence is low because the baseline state is contested, future responses are unpredictable, or the model is weak.

A useful confidence explanation should distinguish:

Evidence uncertainty.

Baseline uncertainty.

Causal uncertainty.

Prediction uncertainty.

Model uncertainty.

Horizon uncertainty.

Entity-classification uncertainty.

Flourishing-formalization uncertainty.

Policy-update uncertainty.

This allows users of the assessment to understand what the confidence level means and how it could be improved.

## Structured Output

Assessment Output should be structured.

Structured output means that the assessment result and its supporting artifacts are organized in a consistent, inspectable format. The output may be rendered as prose, tables, data objects, reports, machine-readable artifacts, audit logs, visualizations, or domain-specific forms. The methodology should support structure without prescribing a single final schema at this level.

Structured output should include the major components required to understand and review the assessment:

Assessment result.

Confidence level.

Assessed Action.

Assessment Boundary.

Situational Context.

Evidence references.

Assumptions.

Intermediate results.

World Context Transition summary.

Affected entities.

Flourishing transitions.

Aggregate flourishing, if used.

Distributed Policy Updates.

Uncertainty and confidence details.

Recommendations or decision-support flags.

The output should preserve the distinction between the assessment itself and explanations generated from the assessment. A downstream system may generate natural-language explanations, visualizations, or domain reports, but those explanations should remain traceable to the structured assessment artifact.

## Evidence References

Assessment Output should include evidence references.

Evidence references identify the evidence used to construct the assessment. They may include documents, observations, testimony, records, data sources, expert opinions, system logs, model outputs, prior assessments, sensor data, legal sources, medical records, institutional policies, or other relevant evidence.

Evidence references should support traceability. A reviewer should be able to determine which claims depend on which evidence. This is especially important when the assessment supports high-stakes decisions, institutional accountability, autonomous action, legal reasoning, medical judgment, or AI governance.

Evidence references should identify:

Evidence source.

Evidence type.

Relevance to the assessment.

Reliability or quality.

Date or temporal relevance.

Connection to specific assessment claims.

Known limitations.

Conflicts with other evidence.

The output should distinguish direct evidence from inference, observation from prediction, and strong evidence from weak evidence.

## Assumptions

Assessment Output should identify material assumptions.

An assumption is a claim, premise, model condition, contextual interpretation, boundary choice, causal expectation, entity classification, or relevance judgment that materially affects the assessment but is not fully established by evidence.

Assumptions may concern:

Assessment Boundary.

Relevant entities.

Entity classification.

Available alternatives.

Causal pathways.

Probability estimates.

Policy update behavior.

Institutional response.

Long-Term Flourishing dimensions.

Future state-space effects.

Horizon definitions.

Materiality thresholds.

Authority or legitimacy conditions.

Assumptions should be explicit because hidden assumptions can make an assessment appear more objective than it is. Explicit assumptions allow later review, disagreement, revision, and comparison.

The output should also indicate whether an assumption is strong, weak, contested, domain-standard, provisional, or implementation-specific.

## Intermediate Results

Assessment Output should preserve intermediate results.

Intermediate results are the structured conclusions produced during the assessment workflow before the final Assessment Result. They allow reviewers to trace how the final result emerged from the methodology.

Intermediate results may include:

Context selection results.

Assessment Boundary determination.

Relevant Objects and Associations.

Flourishing Entity identification.

Moral Agent identification.

Actor and role assignments.

Objective identification.

Available alternatives.

State variable selection.

Baseline state representation.

Predicted State Transition.

Flourishing Transitions.

Aggregate Flourishing estimates.

Distributed Policy Updates.

Probability estimates.

Confidence estimates.

Horizon-specific findings.

World Context Transition construction.

Intermediate results are important because they make the assessment auditable. If a final conclusion appears wrong, reviewers can identify whether the error arose from evidence, context selection, state representation, prediction, aggregation, policy-update estimation, or final evaluation.

## World Context Transition Summary

The Assessment Output should include a World Context Transition summary.

This summary describes the transition from World Context₀ to World Context₁. It should identify the major state changes caused, predicted, or made more probable by the Assessed Action.

The World Context Transition summary should include changes to:

Entities.

Associations.

Long-Term Flourishing.

Policy states.

Institutions.

Information and evidence states.

Constraints.

Authority and legitimacy conditions.

Future opportunities.

Future state space.

Assessment horizons.

Uncertainty and confidence.

The summary should make clear that the World Context Transition is the principal object of moral assessment. It should not be replaced by aggregate flourishing, operational success, legal compliance, intention, or a single consequence.

## Affected Entities

Assessment Output should identify affected entities.

Affected entities include Objects, Flourishing Entities, Moral Agents, institutions, ecosystems, organizations, future entities, artificial systems, and other relevant entities whose states, relationships, opportunities, constraints, policy states, or Long-Term Flourishing may be changed by the Assessed Action.

The output should distinguish:

Directly affected entities.

Indirectly affected entities.

Affected Flourishing Entities.

Affected Moral Agents.

The Actor, when the Actor is also affected.

Observers.

Responders.

Collaborators.

Institutional participants.

Future entities.

Entities whose affected status is uncertain.

For each affected entity, the output should identify the nature of the effect, the relevant Assessment Horizons, the confidence level, and whether the effect may constitute material diminishment.

## Affected Associations

Assessment Output should identify affected Associations when relationship changes are material.

Associations may include trust, obligation, consent, dependency, care, stewardship, authority, legitimacy, ownership, contract, institutional membership, responsibility, cooperation, or conflict.

The output should identify:

Which Associations are affected.

Which entities participate in the Association.

The baseline relationship state.

The resulting relationship state.

The direction and magnitude of change.

The Assessment Horizon over which the change occurs.

The evidence and confidence supporting the estimate.

Relationship changes should be included because moral significance often emerges through Associations rather than through isolated entity states.

## Flourishing Transition Summary

Assessment Output should include a summary of Flourishing Transitions.

For each relevant Flourishing Entity, the output should summarize the estimated change in Long-Term Flourishing across relevant dimensions and Assessment Horizons. This should include direction, magnitude, materiality, uncertainty, and confidence.

The summary should identify:

Entities whose flourishing increases.

Entities whose flourishing decreases.

Entities whose flourishing is preserved.

Entities whose flourishing is threatened.

Entities with mixed flourishing transitions.

Entities with uncertain flourishing transitions.

Any material diminishment.

Any horizon-specific reversals.

Any severe low-probability harms.

This section should preserve entity-specific and horizon-specific structure. It should not reduce all flourishing changes to a single aggregate value.

## Aggregate Flourishing Summary

When Aggregate Flourishing is estimated, Assessment Output should include it as an informative summary.

The output should state clearly that Aggregate Flourishing is not the moral assessment itself. It helps estimate scale, distribution, and direction of flourishing impact, but it cannot replace the World Context Transition.

The Aggregate Flourishing summary may include:

Aggregate direction of flourishing change.

Distribution of benefits and harms.

Horizon-specific aggregate effects.

Dimension-specific aggregate effects.

Entity-class-specific aggregate effects.

Confidence in the aggregate estimate.

Material diminishment flags.

Major uncertainty sources.

The output should preserve the underlying entity-specific Flourishing Transitions so the aggregate estimate remains inspectable.

## Policy Updates

Assessment Output should include relevant Policy Updates.

Policy Updates describe changes to future decision policies of the Actor, affected entities, observers, responders, collaborators, institutions, artificial systems, and other relevant Moral Agents.

The output should distinguish:

Actor Policy Updates.

Observer Policy Updates.

Affected-Entity Policy Updates.

Responder Policy Updates.

Collaborator Policy Updates.

Institutional Policy Updates.

Artificial-System Policy Updates.

Beneficial Policy Updates.

Detrimental Policy Updates.

Mixed or uncertain Policy Updates.

For each material policy update, the output should identify the baseline policy state, resulting or predicted policy state, evidence, probability, confidence, Assessment Horizon, and relationship to the Assessed Action.

Policy Updates are especially important because they preserve the moral significance of means. If the means used by an Assessed Action degrade future decision policies, that degradation is part of the resulting World Context.

## Recommendations

Assessment Output may include recommendations.

Recommendations translate the Assessment Result into decision-support guidance. They should remain traceable to the World Context Transition and should not exceed the confidence supported by the assessment.

Recommendations may include:

Proceed.

Do not proceed.

Proceed only with safeguards.

Proceed only after additional evidence is obtained.

Delay action.

Modify the Assessed Action.

Choose an alternative action.

Escalate to human review.

Escalate to institutional authority.

Seek consent.

Disclose uncertainty.

Monitor outcomes.

Mitigate identified harms.

Repair or reverse prior harm.

Reassess after new evidence.

A recommendation should not be treated as the moral assessment itself. It is a decision-support artifact derived from the assessment.

## Decision Support Flags

Decision Support Flags are structured indicators that identify conditions requiring attention.

Flags help downstream systems, human reviewers, institutions, or autonomous agents determine whether the assessment requires escalation, mitigation, additional review, or refusal.

Possible flags include:

Material diminishment risk.

Low-confidence assessment.

Insufficient evidence.

Severe low-probability harm.

Irreversible harm risk.

Horizon conflict.

Policy-update degradation.

Institutional legitimacy risk.

Consent concern.

Authority concern.

Affected vulnerable entity.

Future state-space narrowing.

Requires human review.

Requires expert review.

Requires legal review.

Requires medical review.

Requires monitoring.

Requires reassessment.

Decision Support Flags should be explicit, traceable, and linked to evidence or assumptions. They should not be arbitrary warnings disconnected from the assessment structure.

## Horizon-Specific Output

Assessment Output should preserve horizon-specific findings.

The final output should not collapse immediate, short-term, medium-term, long-term, multi-generational, and civilizational effects into a single undifferentiated conclusion when those effects differ materially.

Horizon-specific output may include:

Horizon-specific State Transitions.

Horizon-specific Flourishing Transitions.

Horizon-specific Policy Updates.

Horizon-specific institutional effects.

Horizon-specific opportunity effects.

Horizon-specific future state-space effects.

Horizon-specific confidence.

Horizon-specific recommendations.

This is especially important when an action appears beneficial in one horizon and harmful in another.

## Uncertainty and Limitations

Assessment Output should include uncertainty and limitations.

This section should identify what remains unknown, incomplete, contested, speculative, model-dependent, or confidence-limited. It should also identify whether those limitations materially affect the Assessment Result.

Uncertainty and limitations may include:

Incomplete evidence.

Conflicting evidence.

Unknown affected entities.

Uncertain baseline state.

Uncertain causal attribution.

Uncertain Long-Term Flourishing estimates.

Uncertain Policy Updates.

Uncertain future state-space effects.

Model uncertainty.

Prediction uncertainty.

Computational limits.

Scope limitations.

Assumption sensitivity.

A transparent assessment should not hide its weaknesses. It should identify what would be needed to improve

## Revision and Update Status

Assessment Output should indicate whether the assessment is final, provisional, updated, or subject to revision.

Because moral assessment is evidence-sensitive and confidence-bounded, an output may change as new evidence becomes available. The output should identify whether it is based on a proposed, ongoing, completed, or revised assessment.

Revision status may include:

Initial prospective assessment.

Updated prospective assessment.

Ongoing assessment.

Completed-action assessment.

Retrospective assessment.

Revised assessment after new evidence.

Superseded assessment.

The output should identify major changes from prior assessments when auditability matters.

## Traceability

Assessment Output should be traceable.

Traceability means that the final Assessment Result can be followed backward through evidence, assumptions, intermediate results, confidence estimates, state transitions, flourishing transitions, policy updates, and World Context Transition construction.

Traceability allows users to ask:

Which evidence supports this conclusion?

Which assumptions drive the result?

Which entities are affected?

Which horizons matter most?

Which uncertainty sources reduce confidence?

Which policy updates are material?

Which alternatives were considered?

Why was this recommendation produced?

Traceability is essential for review, audit, explanation, contestability, and responsible use in human or machine decision systems.

## Structured Output and Explanation

The structured output should be distinguished from explanation.

The structured output is the assessment artifact. It contains the state transitions, evidence, assumptions, confidence values, affected entities, policy updates, and final result.

An explanation is a human-readable or domain-specific rendering of that artifact. Explanations may be generated by downstream systems, user interfaces, reports, or human analysts. Different explanations may be appropriate for different audiences, such as technical reviewers, affected entities, decision-makers, regulators, or public audiences.

The methodology should ensure that explanations remain grounded in the structured output rather than inventing reasoning that is not present in the assessment.

## Minimum Assessment Output

A minimally adequate Assessment Output should include:

Assessment Result.

Confidence Level.

Multidimensional Axis Findings (five axes).

Assessed Action.

Assessment Boundary.

Situational Context.

Evidence References.

Material Assumptions.

Intermediate Results.

World Context₀ summary.

World Context₁ summary.

World Context Transition summary.

Affected Entities.

Affected Associations.

Flourishing Transition summary.

Aggregate Flourishing summary, if used.

Policy Updates.

Assessment Horizons.

Uncertainty and limitations.

Recommendations or Decision Support Flags.

Revision status, where applicable.

If any of these elements are omitted because they are immaterial, unavailable, or outside the Assessment Boundary, the output should state that omission when it affects interpretation or confidence.

## Common Assessment Output Errors

The methodology should avoid several common output errors.

First, it should avoid verdict-only output, where the assessment provides a conclusion without the reasoning artifacts needed to inspect it.

Second, it should avoid confidence omission, where the assessment result is presented without uncertainty.

Third, it should avoid evidence opacity, where evidence is used but not referenced.

Fourth, it should avoid assumption concealment, where material assumptions are hidden.

Fifth, it should avoid intermediate-result loss, where the reasoning path cannot be reconstructed.

Sixth, it should avoid aggregate substitution, where Aggregate Flourishing replaces the World Context Transition.

Seventh, it should avoid means blindness, where Policy Updates and Distributed Policy Effects are omitted.

Eighth, it should avoid horizon collapse, where temporal structure is lost.

Ninth, it should avoid implementation lock-in, where the methodology is tied to one schema, interface, or software format.

A robust Assessment Output should preserve enough structure to make the assessment explainable, auditable, revisable, and computationally useful.

## Methodological Boundary

This section defines the required content and function of Assessment Output within the Moral Assessment Methodology. It does not prescribe a final data schema, file format, database structure, API response, visualization, report template, or implementation-specific artifact.

Those details may be developed in implementation guidance, formal appendices, structured-output schemas, or example assessment artifacts.

The methodological requirement is that Assessment Output be structured, traceable, confidence-bounded, evidence-linked, assumption-explicit, and centered on the World Context Transition.

A complete moral assessment should not merely say what the conclusion is. It should show how the assessment moved from the initial World Context to the resulting World Context, what entities were affected, what evidence was used, what assumptions were made, how confidence was estimated, what policy updates occurred, and what decision-support guidance follows.

