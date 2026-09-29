[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §7.5

*Implementation guidance. A realization of the architecture remains subordinate to the architecture.*

# Core Runtime Services

Core Runtime Services describe the functional capabilities that a practical implementation may provide when Objective-Based Systems Ethics is deployed as an operational system, service, runtime, agent component, workflow engine, or Moral Reasoning Runtime.

These services are implementation-level components. They do not redefine the Reference Architecture or Moral Assessment Methodology. Instead, they describe runtime capabilities that help instantiate the architecture and methodology in software or operational workflows.

A minimal implementation may provide only a subset of these services manually or semi-automatically. A mature implementation may provide them as modular, independently versioned, auditable runtime services. The purpose of identifying these services is to clarify what practical systems may need in order to construct assessments, manage evidence, estimate transitions, propagate confidence, generate structured outputs, and preserve auditability.

The core runtime services include Context Construction, World Model Management, Assessment Engine, State-Transition Prediction, World Context Evaluation, Confidence Propagation, Structured Output Generation, and Audit Artifact Generation.

## Context Construction

Context Construction is the runtime service that builds the assessment context from available inputs, evidence, prior state, user-provided information, domain knowledge, and system-accessible data.

This service operationalizes the movement from broad World Context to Assessment Boundary, Local Context, and Situational Context. It identifies what information is relevant to the Assessed Action and organizes that information into a form the assessment process can use.

Context Construction may include:

Identifying the Assessed Action.

Identifying the Actor or Actors.

Applying the Assessment Boundary.

Selecting relevant domain context.

Constructing the Situational Context.

Identifying relevant Objects.

Identifying relevant Associations.

Identifying affected Flourishing Entities.

Identifying Moral Agents and contextual roles.

Identifying operational and moral-system Objectives.

Identifying constraints, authority conditions, and available alternatives.

Identifying evidence sources and evidence gaps.

Context Construction should be traceable. A reviewer should be able to understand why certain entities, relationships, evidence sources, horizons, or constraints were included or excluded.

This service is especially important because errors in context construction propagate through the entire assessment. If the relevant context is too narrow, the system may miss affected entities, institutional effects, Distributed Policy Updates, or long-term consequences. If the context is too broad, the assessment may become unfocused or computationally impractical.

## World Model Management

World Model Management is the runtime service that maintains the represented state of the relevant World Context.

The World Model is the implementation-level representation of Objects, Associations, entities, roles, institutions, constraints, information states, policy states, future opportunities, and future state space. It may be implemented as a graph, ontology, database, document store, state-vector system, simulation model, hybrid knowledge representation, or another technical form.

World Model Management may include:

Maintaining entity records.

Maintaining Association records.

Tracking state variables.

Managing ontology versions.

Representing institutional structures.

Representing policy states.

Representing information and uncertainty states.

Representing future opportunities.

Representing future state-space assumptions.

Tracking baseline and resulting World Context states.

Managing updates from new evidence.

Maintaining historical versions of assessments and world states.

The World Model should support both World Context₀ and World Context₁ representations. It should also support revised states when new evidence becomes available.

World Model Management should not be confused with complete knowledge of the world. The represented World Model is always partial, scoped, and confidence-bounded. It should therefore include metadata about evidence quality, uncertainty, provenance, versioning, and scope limitations.

## Assessment Engine

The Assessment Engine is the runtime service that orchestrates the Moral Assessment Methodology.

It coordinates the workflow through which an Assessed Action is evaluated. It may call other runtime services, assemble intermediate results, apply domain-specific rules or models, estimate State Transitions, evaluate Long-Term Flourishing, account for Distributed Policy Updates, propagate confidence, and produce the final Assessment Output.

The Assessment Engine may perform or coordinate:

Assessment request intake.

Assessment Boundary application.

Context Construction.

Relevant entity and Association identification.

Objective identification.

Alternative-action comparison.

State Representation.

State-Transition Prediction.

Flourishing Transition estimation.

Aggregate Flourishing calculation, where used.

Distributed Policy Update estimation.

Multi-Horizon Assessment.

Probability and confidence estimation.

World Context Transition construction.

Assessment Result generation.

Decision-support flag generation.

The Assessment Engine should preserve intermediate results. It should not operate as an opaque conclusion generator. Each major assessment step should produce inspectable artifacts that can be reviewed, audited, revised, or used by downstream systems.

In a mature implementation, the Assessment Engine may operate as an orchestrator rather than a single monolithic reasoning component. It may coordinate symbolic models, probabilistic models, LLM components, simulations, expert rules, human review steps, and domain-specific plugins.

## State-Transition Prediction

State-Transition Prediction is the runtime service that estimates how relevant state variables may change as a result of the Assessed Action.

This service operationalizes the State Transition Model. It estimates changes to entities, Associations, policy states, institutions, information states, constraints, future opportunities, and future state space. It may operate prospectively, retrospectively, or in an ongoing assessment mode.

State-Transition Prediction may include:

Predicting entity-state changes.

Predicting relationship-state changes.

Predicting Policy Updates.

Predicting institutional effects.

Predicting information-state effects.

Predicting constraint changes.

Predicting future opportunity changes.

Predicting future state-space changes.

Predicting Long-Term Flourishing changes.

Estimating horizon-specific effects.

Generating alternative transition scenarios.

Estimating probability and uncertainty for each transition.

This service may use different techniques depending on domain and implementation. It may use expert rules, causal models, simulations, statistical models, probabilistic inference, historical analogies, machine-learning models, LLM-assisted reasoning, or human expert review.

The service should distinguish between predicted, observed, inferred, and revised transitions. It should also identify uncertainty and confidence for material predictions.

A State-Transition Prediction service should avoid reducing prediction to immediate consequences alone. A conforming implementation should preserve relational, institutional, behavioral, informational, and future-oriented transitions when they are material.

## World Context Evaluation

World Context Evaluation is the runtime service that evaluates the transition from World Context₀ to World Context₁.

This service integrates the results of context construction, state representation, transition prediction, flourishing estimation, policy-update estimation, multi-horizon assessment, and confidence propagation. It determines how the resulting World Context should be assessed under the framework.

World Context Evaluation may include:

Constructing World Context₀.

Constructing predicted or observed World Context₁.

Comparing World Context₀ and World Context₁.

Identifying material state changes.

Evaluating entity changes.

Evaluating Association changes.

Evaluating Long-Term Flourishing changes.

Evaluating Aggregate Flourishing, where used.

Evaluating Distributed Policy Updates.

Evaluating institutional effects.

Evaluating information and uncertainty changes.

Evaluating constraint and authority changes.

Evaluating future opportunity changes.

Evaluating future state-space changes.

Evaluating horizon-specific conflicts.

Evaluating the transition against the Foundational Axiom.

The output of this service should be a structured World Context Transition summary. It should explain what changed, for whom, across which horizons, with what confidence, and with what moral significance.

World Context Evaluation is where implementation most directly preserves the framework's core commitment: moral assessment evaluates the transition from one World Context to another, not merely the immediate outcome of an action.

## Confidence Propagation

Confidence Propagation is the runtime service that tracks uncertainty and confidence across the assessment workflow.

It ensures that uncertainty in evidence, context construction, state representation, transition prediction, flourishing estimation, policy-update estimation, and horizon analysis is reflected in the final Assessment Output.

Confidence Propagation may include:

Tracking evidence quality.

Tracking evidence completeness.

Tracking source reliability.

Tracking baseline-state uncertainty.

Tracking causal uncertainty.

Tracking model uncertainty.

Tracking prediction uncertainty.

Tracking stochastic approximation error.

Tracking uncertainty across Assessment Horizons.

Tracking uncertainty in Long-Term Flourishing estimates.

Tracking uncertainty in Distributed Policy Updates.

Tracking confidence in the World Context Transition.

Producing final confidence estimates and confidence explanations.

Confidence Propagation should distinguish probability from confidence. Probability estimates the likelihood of an event or transition. Confidence estimates the reliability of the probability estimate or assessment conclusion.

This service should also support graceful degradation. When information is incomplete, the implementation should reduce confidence, identify missing information, and flag material uncertainty rather than failing silently or producing false certainty.

## Structured Output Generation

Structured Output Generation is the runtime service that produces the assessment artifact.

The structured output should contain the Assessment Result and the supporting artifacts needed for review, audit, explanation, visualization, downstream use, or future revision. It should preserve the distinction between the assessment artifact itself and any human-readable explanation generated from it.

Structured Output Generation may include:

Assessment Result.

Confidence Level.

Assessed Action.

Assessment Boundary.

Situational Context.

Evidence References.

Assumptions.

Intermediate Results.

Affected Entities.

Affected Associations.

Flourishing Transitions.

Aggregate Flourishing, if used.

Distributed Policy Updates.

World Context Transition summary.

Assessment Horizons.

Uncertainty and limitations.

Recommendations.

Decision-support flags.

Revision status.

Assessment metadata.

Structured output may be represented as JSON, XML, database records, reports, graph artifacts, event logs, workflow records, or another implementation-specific format. The methodology does not prescribe a single schema at this level.

The key requirement is that structured output remain machine-readable, inspectable, traceable, confidence-bounded, and faithful to the underlying assessment.

## Audit Artifact Generation

Audit Artifact Generation is the runtime service that preserves the evidence, intermediate reasoning, assumptions, model versions, ontology versions, confidence estimates, and output artifacts needed to review or reconstruct an assessment.

Auditability is essential because moral assessments may influence high-stakes decisions, institutional governance, autonomous behavior, legal review, medical recommendations, AI safety decisions, or public policy. A system that cannot explain or reconstruct its assessment may not be suitable for responsible deployment.

Audit artifacts may include:

Assessment request records.

Input evidence and evidence references.

Evidence provenance metadata.

Assessment Boundary decisions.

Context Construction records.

Entity and Association identification records.

Ontology versions.

Model versions.

State variable selections.

Baseline World Context representation.

Predicted State Transition records.

Flourishing Transition estimates.

Policy Update estimates.

Probability estimates.

Confidence propagation records.

Intermediate results.

World Context Transition summary.

Final Assessment Output.

Human review actions.

Escalation decisions.

Revision history.

Audit artifacts should support traceability from final Assessment Result back to the evidence and assumptions that produced it. They should also support later revision when new evidence becomes available.

Audit Artifact Generation should be designed with security, privacy, access control, retention policy, and institutional accountability in mind. Not every audit artifact should be visible to every user, but material reasoning artifacts should be preserved for appropriate review.

## Runtime Service Interaction

The core runtime services should operate as an integrated assessment pipeline or orchestrated service network.

A typical runtime flow may proceed as follows:

1.  Context Construction identifies the relevant assessment context.

2.  World Model Management provides or updates the relevant World Context representation.

3.  The Assessment Engine orchestrates the methodology.

4.  State-Transition Prediction estimates material changes.

5.  World Context Evaluation integrates those changes into the World Context₀ to World Context₁ transition.

6.  Confidence Propagation tracks uncertainty and reliability.

7.  Structured Output Generation produces the assessment artifact.

8.  Audit Artifact Generation preserves the reasoning trail.

This flow may be linear, iterative, recursive, or distributed depending on implementation. For example, State-Transition Prediction may reveal missing evidence, causing Context Construction to run again. Confidence Propagation may flag insufficient evidence, causing the Assessment Engine to request human review. World Context Evaluation may identify severe uncertainty, causing the system to generate mitigation recommendations.

The runtime should therefore support iteration rather than assuming that assessment is always a single-pass process.

## Runtime Service Modularity

Core Runtime Services should be modular when practical.

Modularity allows implementations to replace or improve one service without rewriting the entire system. A new evidence ingestion component should not require changes to the World Context Evaluation logic. A better prediction model should not require changes to the structured output schema. A revised ontology should not require rewriting the Assessment Engine.

Modularity supports:

Testing.

Versioning.

Domain adaptation.

Component replacement.

Human review integration.

Scalability.

Auditability.

Extensibility.

Independent improvement of models.

A modular runtime also supports hybrid implementation patterns. For example, a system may use an embedded library for local context construction, a microservice for State-Transition Prediction, a distributed service for World Model Management, and a workflow component for human review.

## Runtime Service Boundary

Core Runtime Services describe implementation capabilities, not architectural requirements.

A conforming implementation does not need to expose each service as a separate software component. A simple implementation may perform several services manually or within one application. A mature runtime may separate them into independently deployable services.

The requirement is functional rather than structural. An implementation should be able to construct context, manage or represent world state, orchestrate assessment, predict transitions, evaluate the World Context Transition, propagate confidence, generate structured output, and preserve audit artifacts at a level appropriate to the domain and risk.

Core Runtime Services should therefore be understood as a reference decomposition for implementation. They help designers build practical systems while preserving the framework's central commitment to explicit, confidence-bounded assessment of the transition from World Context₀ to World Context₁.

