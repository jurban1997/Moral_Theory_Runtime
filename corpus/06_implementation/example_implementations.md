[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §7.4

*Implementation guidance. A realization of the architecture remains subordinate to the architecture.*

# Example Implementations

Example Implementations illustrate how Objective-Based Systems Ethics may be realized in practical systems. These examples are not exhaustive and are not intended to prescribe a single preferred technical design. They demonstrate how the Reference Architecture and Moral Assessment Methodology can be instantiated across different domains, risk profiles, evidence environments, and operational contexts.

Each example should preserve the same core logic: identify the relevant World Context, apply an Assessment Boundary, derive the Situational Context, identify relevant Objects and Associations, evaluate Objectives, define the Assessed Action, model State Transitions, estimate Long-Term Flourishing changes, account for Distributed Policy Updates, reason under uncertainty, evaluate multiple horizons, and produce structured Assessment Output.

The examples differ in implementation pattern, domain ontology, evidence sources, runtime requirements, human oversight, and deployment constraints. However, each remains faithful to the same underlying framework if it evaluates the Assessed Action as a transition from World Context₀ to World Context₁.

## Moral Reasoning Runtime

A Moral Reasoning Runtime, or MRR, is a standalone reference implementation of the framework.

An MRR provides runtime services for representing context, ingesting evidence, identifying affected entities, modeling State Transitions, estimating Long-Term Flourishing, evaluating Distributed Policy Updates, propagating confidence, and producing structured Assessment Output. It may expose these capabilities through APIs, user interfaces, plugins, workflow integrations, or agent-facing runtime calls.

The purpose of an MRR is not to replace the Reference Architecture or Moral Assessment Methodology. It is to instantiate them in an operational environment. The MRR acts as a practical system through which applications, agents, institutions, or human users can submit Assessed Actions and receive structured, confidence-bounded moral assessments.

An MRR may include services such as:

World Context representation.

Assessment Boundary configuration.

Evidence ingestion and provenance tracking.

Entity and Association identification.

State Representation and State Transition modeling.

Long-Term Flourishing estimation.

Distributed Policy Update estimation.

Multi-Horizon Assessment.

Probability and confidence estimation.

Structured Assessment Output.

Audit logging.

Versioned ontologies.

Human review and escalation.

Domain-specific plugins.

As a reference implementation, an MRR should prioritize architectural fidelity, transparency, traceability, extensibility, and confidence-bounded operation over narrow optimization. Its purpose is to demonstrate how the framework can be realized without making any one implementation pattern mandatory.

## LLM Safety and Harness Integration

An LLM safety or harness integration applies the framework to large language model behavior, agent actions, tool use, content generation, and autonomous or semi-autonomous decision support.

In this implementation, the Assessed Action may be an LLM response, tool call, recommendation, refusal, plan, instruction, escalation decision, memory update, or autonomous action. The system evaluates whether that action produces a supportable World Context Transition.

The Assessment Boundary may include the user's request, the conversation context, available tools, user permissions, safety policies, relevant affected entities, downstream risks, evidence quality, and likely effects of the model's output. The Situational Context may include what the model knows, what the user is asking, what the model can safely infer, what tools it may use, and what harms or benefits may follow from the response.

An LLM safety implementation may evaluate:

Whether to answer, refuse, clarify, or escalate.

Whether a tool call is safe and authorized.

Whether a recommendation creates material risk.

Whether a response could enable harm.

Whether withholding information materially diminishes a user's flourishing.

Whether a refusal protects Long-Term Flourishing.

Whether the model's response creates harmful policy updates in the user, observers, or future system behavior.

Whether the model should request more evidence because confidence is low.

Distributed Policy Updates are especially important in LLM contexts. A model response may teach users, observers, or downstream agents what is acceptable, effective, safe, or repeatable. A harmful response may update user behavior toward riskier action. A beneficial refusal may update expectations toward safer conduct. A deceptive or overconfident answer may degrade epistemic responsibility.

Structured Assessment Output in an LLM harness may produce decision-support flags such as: answer normally, answer with caveats, ask for clarification, use tool, refuse, escalate, require human review, limit detail, provide safer alternative, or monitor future interactions.

## Autonomous Robotics

An autonomous robotics implementation applies the framework to robots that perceive environments, select actions, interact with humans or other entities, and operate under physical constraints.

In this domain, the Assessed Action may be a movement, manipulation, navigation choice, emergency stop, collision-avoidance maneuver, human-interaction behavior, resource allocation decision, or task-execution plan.

The World Context may include the robot, humans, animals, physical objects, environmental hazards, property, institutions, safety rules, authority conditions, operational objectives, and future risks. The Situational Context may include sensor readings, uncertainty, time pressure, task goals, nearby entities, physical constraints, and available alternatives.

An autonomous robotics implementation may evaluate:

Whether to proceed with a planned movement.

Whether to stop or slow down.

Whether to prioritize one entity's safety over another's.

Whether to ask for human confirmation.

Whether to interrupt an assigned task.

Whether to violate a minor operational constraint to avoid severe harm.

Whether to preserve future options by choosing a safer route.

State Transitions in robotics often involve physical safety, spatial relationships, operational constraints, and future opportunity preservation. Distributed Policy Updates may include how human operators, observers, or collaborating robots update future behavior based on the robot's action. For example, a robot that consistently yields safely may strengthen trust, while a robot that optimizes task completion at the expense of human comfort may degrade trust and cooperation.

An autonomous robotics implementation should be highly sensitive to uncertainty, sensor reliability, latency, physical irreversibility, human safety, and escalation thresholds.

## Clinical Decision Support

A clinical decision-support implementation applies the framework to medical recommendations, treatment choices, consent processes, triage decisions, risk disclosure, and care planning.

In this domain, the Assessed Action may be a treatment recommendation, diagnostic plan, refusal of treatment, triage decision, medication choice, disclosure decision, escalation to specialist care, or allocation of limited medical resources.

The World Context may include the patient, clinicians, family members, care team, medical institution, clinical evidence, legal requirements, consent status, resource constraints, professional obligations, and future care options. The Situational Context may include the patient's condition, available treatments, urgency, prognosis, uncertainty, patient preferences, decision capacity, and institutional constraints.

A clinical decision-support implementation may evaluate:

Whether a proposed treatment preserves Long-Term Flourishing.

Whether the patient has sufficient information for informed consent.

Whether the clinician should disclose uncertainty.

Whether delay would materially diminish future treatment options.

Whether a less invasive alternative is available.

Whether a resource-allocation decision is supportable.

Whether institutional protocols preserve or diminish patient flourishing.

Long-Term Flourishing in clinical settings may include survival, health, autonomy, agency, future possibilities, quality of life, relational support, and adaptive capacity. Distributed Policy Updates may include effects on patient trust, clinician practice, institutional transparency, family decision behavior, and future willingness to seek care.

A clinical implementation should preserve evidence references, assumptions, uncertainty, confidence, affected entities, alternatives, and horizon-specific effects. It should not replace clinical judgment, but it may support more explicit, auditable, and confidence-bounded ethical reasoning.

## Government Policy Analysis

A government policy-analysis implementation applies the framework to public decisions, regulations, programs, emergency measures, resource allocation, legal reforms, infrastructure planning, and long-term governance choices.

In this domain, the Assessed Action may be a proposed law, regulation, executive action, budget allocation, public-health measure, enforcement policy, infrastructure investment, environmental rule, taxation policy, or emergency intervention.

The World Context may include citizens, communities, agencies, institutions, legal structures, economic conditions, environmental systems, public trust, resource constraints, authority conditions, future generations, and civilizational risk factors. The Situational Context may include policy objectives, jurisdiction, affected populations, available alternatives, evidence quality, stakeholder input, institutional legitimacy, and uncertainty.

A government policy implementation may evaluate:

Whether a policy preserves or diminishes Long-Term Flourishing.

Which populations benefit or bear burdens.

Whether the policy damages trust or legitimacy.

Whether the policy creates harmful precedent.

Whether short-term benefit creates long-term institutional harm.

Whether future generations are affected.

Whether civilizational future state space is expanded or narrowed.

Whether less harmful alternatives are available.

Multi-Horizon Assessment is central in government policy. Immediate public benefits may differ from long-term institutional effects. A policy may increase short-term compliance while diminishing legitimacy. Another may impose short-term cost while preserving public trust, ecological resilience, or future opportunity.

Distributed Policy Updates may include changes in citizen trust, institutional behavior, agency enforcement patterns, political norms, compliance expectations, and public willingness to cooperate.

A government implementation should support transparency, evidence provenance, stakeholder visibility, horizon-specific confidence, and structured decision-support flags.

## Legal Decision Support

A legal decision-support implementation applies the framework to legal reasoning, judicial decisions, regulatory interpretation, enforcement discretion, sentencing, compliance review, precedent analysis, and institutional legitimacy.

In this domain, the Assessed Action may be a judicial ruling, legal argument, enforcement decision, settlement recommendation, compliance action, regulatory interpretation, or institutional legal policy.

The World Context may include parties, courts, agencies, statutes, precedent, rights, obligations, authority, legitimacy, institutional trust, affected communities, and future legal expectations. The Situational Context may include the legal facts, applicable law, jurisdiction, procedural posture, evidentiary record, available remedies, authority constraints, and institutional consequences.

A legal implementation may evaluate:

Whether a legal action preserves procedural integrity.

Whether it respects legitimate authority.

Whether it materially diminishes affected entities.

Whether it strengthens or weakens trust in legal institutions.

Whether it creates harmful precedent.

Whether it preserves future legal remedies.

Whether it treats similarly situated entities consistently.

Whether the means used are compatible with institutional legitimacy.

Legal decision support is not a substitute for legal authority or judicial judgment. Its purpose is to make the moral structure of legal decisions more explicit, especially where legal discretion, institutional legitimacy, affected entities, and long-term policy effects matter.

Distributed Policy Updates are especially important in legal contexts because legal decisions shape future expectations, institutional behavior, compliance, enforcement norms, and public trust. A legally effective action may still degrade the resulting World Context if it undermines legitimacy, due process, or future confidence in legal institutions.

## Organizational Governance Systems

An organizational governance implementation applies the framework to corporate, nonprofit, institutional, or administrative decision-making.

In this domain, the Assessed Action may be a hiring decision, layoff, compensation policy, compliance response, internal investigation, product launch, risk acceptance, whistleblower response, governance change, crisis decision, or strategic initiative.

The World Context may include employees, customers, leaders, shareholders, communities, regulators, partners, organizational culture, policies, incentives, obligations, trust relationships, and institutional reputation. The Situational Context may include business objectives, legal constraints, stakeholder impacts, internal evidence, authority structures, resource constraints, and available alternatives.

An organizational governance implementation may evaluate:

Whether a decision preserves employee and stakeholder flourishing.

Whether it damages trust or accountability.

Whether it creates harmful internal precedent.

Whether it reinforces or degrades ethical culture.

Whether it shifts risk onto vulnerable entities.

Whether it preserves institutional legitimacy.

Whether it creates detrimental Actor or institutional Policy Updates.

Whether it produces short-term gain at long-term organizational cost.

Distributed Policy Updates are central in organizations. A leader who succeeds through deception may update the organization toward deception. A company that tolerates retaliation may degrade future reporting and accountability. Conversely, transparent correction, fair process, and responsible disclosure may strengthen institutional policy states even when costly.

Structured Assessment Output may support board review, ethics committee analysis, compliance records, audit logs, risk management, employee-relations decisions, and governance accountability.

## Cross-Domain Implementations

Some implementations may span multiple domains.

For example, an AI system used in medicine may require both LLM safety integration and clinical decision support. A robotic surgical system may combine autonomous robotics, clinical ethics, legal liability, and institutional governance. A public-sector AI deployment may combine government policy analysis, legal decision support, organizational governance, and AI safety.

Cross-domain implementations require careful Assessment Boundary design. They should identify which domain-specific ontologies, evidence standards, authority structures, and affected entities are relevant. They should also preserve the common architecture so that domain modules do not produce incompatible assessments.

A cross-domain implementation should integrate domain-specific evidence and reasoning while still producing a coherent World Context Transition assessment.

## Example Implementation Comparison

The following comparison summarizes the primary emphasis of each example implementation.

  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Example Implementation             Primary Assessed Actions                               Key Concerns                                                               Typical Output
  ---------------------------------- ------------------------------------------------------ -------------------------------------------------------------------------- -----------------------------------------------
  Moral Reasoning Runtime            Submitted actions, plans, tool calls, policy choices   General-purpose assessment fidelity, runtime services, structured output   Structured Moral Assessment

  LLM Safety / Harness Integration   Responses, refusals, tool calls, plans                 User harm, misuse, policy updates, uncertainty, safe refusal               Answer / refuse / escalate / modify

  Autonomous Robotics                Physical actions, movements, task plans                Safety, physical constraints, sensor uncertainty, human trust              Proceed / stop / reroute / escalate

  Clinical Decision Support          Treatment, consent, triage, care plans                 Patient flourishing, autonomy, evidence quality, prognosis                 Recommendation with confidence and safeguards

  Government Policy Analysis         Laws, regulations, programs, emergency actions         Public flourishing, legitimacy, distribution, future generations           Policy assessment and decision-support flags

  Legal Decision Support             Rulings, enforcement, compliance, remedies             Authority, legitimacy, precedent, procedural integrity                     Legal-ethical assessment and risk flags

  Organizational Governance          Internal decisions, policies, crisis actions           Trust, culture, accountability, stakeholder effects                        Governance assessment and mitigation guidance
  --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

This comparison is illustrative rather than exhaustive. Each implementation should be adapted to its domain while preserving the core assessment workflow.

## Example Implementation Boundary

The examples in this section are not the framework itself.

They demonstrate possible realizations of the Reference Architecture and Moral Assessment Methodology. They do not limit the framework to the listed domains, software patterns, or deployment models. Future implementations may include education systems, environmental management, international relations, military command review, infrastructure planning, financial systems, scientific research governance, personal decision support, and future artificial moral agents.

The test of any example implementation is whether it preserves the framework's central requirements: explicit representation of the Assessed Action, context, entities, Associations, Objectives, State Transitions, Long-Term Flourishing, Distributed Policy Updates, uncertainty, Assessment Horizons, World Context Transition, and structured Assessment Output.

