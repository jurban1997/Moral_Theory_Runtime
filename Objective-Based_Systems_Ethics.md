# Objective-Based Systems Ethics

*An implementation-neutral reference architecture for moral assessment.*

Working draft. This is the document to read. It states the problem, the design constraints, and the axiom that gives the architecture its direction. Definitions, component specifications, the assessment procedure, worked examples, and the arguments with other ethical traditions are separate documents, listed in the bibliography, so this paper can stay readable.

Section numbers such as §6.9 are stable identifiers carried over from the source outline. They are not page numbers. The section index at the end of this document maps each one to the document that now holds it. The source outline is archived at `Archive/framework.md`.

## How to read this document

Read this document from the abstract through the axiom. That is the published argument.

Open a supporting document when you need a term defined, a component specified, a procedure followed, an example worked, or a tradition answered. Each supporting document begins with a link back here. The arguments and the detailed definitions were moved, not copied, except for the axiom statement, which is quoted below so this paper can stand without the axiom document open beside it.

After this document, a useful second reading is:

1. [Foundational Axiom](corpus/03_axiom/foundational_axiom.md) — the case for the axiom, its limits, and the rules for reading it with the sections that define its terms.
2. [Architectural Overview](corpus/04_architecture/architectural_overview.md) — what the system is.
3. [Assessment Workflow](corpus/05_methodology/assessment_workflow.md) — how an assessment is performed.
4. One example: [accidental harm](corpus/07_examples/accidental_harm.md) or [the ends do not justify the means](corpus/07_examples/ends_and_means.md).
5. The comparison and the counterarguments for a tradition you already know. Both are paired in the bibliography.

## Abstract

> Editorial note: working draft. Revise and finalize after the final draft of the full document has been approved.

Moral reasoning in consequential domains — artificial intelligence, law, medicine, governance, and autonomous systems — is typically performed through informal judgment, inherited doctrine, or single-metric optimization, none of which produces reasoning that is inspectable, auditable, or computationally representable. This paper proposes Objective-Based Systems Ethics, an implementation-neutral reference architecture for moral assessment. Rather than testing actions against fixed rules or aggregating outcomes into a single utility score, the framework evaluates the transition an action produces in an explicitly modeled World Context: the entities, relationships, institutions, constraints, information states, and future possibilities relevant to the action. A stated Foundational Axiom — the preservation and promotion of the long-term flourishing of relevant Flourishing Entities (persistent adaptive entities) and of the contexts, across the Biosphere, Society, and the Individual, that enable it, without materially diminishing the flourishing of others — supplies the normative direction, and is presented as an explicit, challengeable assumption rather than a hidden premise. The architecture treats morality as a recursive systems problem: every assessed action yields a new World Context, including Distributed Policy Updates that change how the actor, observers, institutions, and artificial systems will decide in the future, which provides a structural account of why means matter independently of immediate outcomes. Assessment is performed across multiple time horizons, under explicit uncertainty, with confidence-bounded and multidimensional outputs that preserve conflicts rather than collapsing them into a single verdict. The paper defines the architecture's foundational definitions, reference structures, and assessment methodology; demonstrates behavior through worked example assessments; and positions the framework against fourteen ethical traditions, documenting both the insights it absorbs and the objections that remain open. The contribution is not a completed ethical theory but a common, explicit, computationally representable architecture through which moral questions can be assessed consistently and transparently by humans, institutions, and artificial systems.

## Executive Summary

This document proposes an implementation-neutral computational architecture for moral reasoning. The framework evaluates moral actions through explicit World Context transitions rather than through ideology, intuition, tradition, or predefined moral rules. Instead of asking only whether an action conforms to a particular ethical doctrine, the framework assesses how the action transforms the state of the world, the entities within it, the relationships among those entities, and the future trajectories made more or less available by the action.

The framework begins with explicit foundational definitions, a clearly stated Foundational Axiom, and a repeatable assessment structure. Its purpose is not to conceal moral assumptions inside informal judgment, but to expose those assumptions so they can be inspected, challenged, refined, and represented computationally. Moral assessment is performed by evaluating changes to the World Context (broad, relevant context) across multiple assessment horizons (timeframes) while considering the information reasonably available within the Situational Context (immediate context surrounding the moral action), the relationships among affected entities, and the probabilistic effects of the action on future state transitions.

A central feature of the architecture is its treatment of morality as a recursive systems problem. Every assessed action transforms one World Context into another. The resulting World Context then becomes the starting condition for future assessments. This means that the moral significance of an action is not limited to its immediate consequences. Actions may also alter relationships, institutions, incentives, trust, authority, future opportunities, and the decision policies of moral agents (the entity being assessed by this model) who initiate, observe, experience, or respond to the action.

This recursive effect is captured through the concept of Distributed Policy Updates. An action may influence the future behavior of the actor and other relevant agents by changing what they perceive as acceptable, effective, rewarded, punished, legitimate, or repeatable. These policy updates become part of the resulting World Context and are therefore part of the moral assessment itself. This provides an architectural explanation for why the means used to achieve an outcome are morally significant, even when a narrow short-term analysis might suggest that the outcome alone is beneficial.

The framework does not reduce morality to utility, rights, duties, virtues, care, consequences, or any single ethical construct. Instead, it evaluates the transition from one World Context to the next. Long-Term Flourishing is treated as a multidimensional state vector describing the capacity of relevant Flourishing Entities to preserve and expand beneficial future state space while participating constructively in the larger systems to which they belong. Aggregate changes in flourishing inform the assessment, but they do not replace evaluation of the broader World Context transition.

The framework is intended to support the long-term flourishing of humans, non-human organisms, ecosystems, and future artificial systems that satisfy the framework's definition of Flourishing Entity. Moral relevance is therefore not limited to present human preference or present human institutions, although human flourishing remains a central case. The architecture is designed to accommodate broader classes of flourishing entities as the framework's definitions, evidence base, and implementation methods mature.

The architecture is intentionally independent of any particular implementation technology. It does not require a specific programming language, inference engine, graph database, artificial intelligence architecture, mathematical formalism, or hardware platform. Every major concept---including Objects, Associations, contexts, objectives, state transitions, uncertainty, assessment horizons, and policy updates---is defined so that it can be represented computationally without constraining future implementation methods.

A software implementation of the architecture may be deployed as a Moral Reasoning Runtime, or MRR. An MRR could operate as a standalone ethical assessment engine, an embedded decision-support component, a governance or audit service, a robotics control layer, or a component within large language model harnesses. In the context of LLMs and future artificial intelligence systems, the framework could provide a transparent assessment layer that evaluates candidate actions according to their predicted effects on World Context transitions, Long-Term Flourishing, Distributed Policy Updates, and confidence-bounded future outcomes. However, artificial intelligence is only one application domain; the architecture is also intended to support human decision-making, institutional governance, healthcare, law, robotics, public policy, and other domains requiring explicit moral assessment.

The objective of this work is not to eliminate moral disagreement. Rather, it is to provide a common computational architecture through which moral questions can be evaluated consistently, transparently, probabilistically, and with explicit assumptions. By combining systems theory, graph-based state representation, recursive World Context transitions, stochastic assessment, and explainable evaluation, the framework seeks to provide a foundation for rigorous moral reasoning across both human and artificial decision-making systems.

## Keywords

Objective-Based Systems Ethics; systems ethics; computational ethics; machine ethics; computational moral reasoning; moral assessment; ethical decision support; implementation-neutral reference architecture; explicit normative assumptions; Foundational Axiom; World Context; World Context Transition; state-transition modeling; graph-based moral reasoning; Long-Term Flourishing; Flourishing Entity; Context Tiers (Biosphere, Society, Individual); sustained capacity; future state space; Distributed Policy Updates; multi-horizon assessment; stochastic moral assessment; probabilistic reasoning; epistemic responsibility; uncertainty-aware moral reasoning; explainable moral reasoning; traceability and auditability; AI alignment; AI safety; artificial moral agents; autonomous systems; Moral Reasoning Runtime.

## High-Level Architecture Overview

Every moral decision changes the world. Some changes are immediate, while others unfold over years or generations. Some affect the people directly involved, while others influence how observers behave in the future.

This framework evaluates moral actions by modeling how a proposed action transforms the surrounding World Context rather than by comparing the action against fixed rules or ideologies.

The process begins by identifying the relevant portion of the world in which the action occurs. It then identifies the entities that may be affected, the relationships among them, and the objectives that are relevant to the situation.

The proposed action is evaluated by estimating how it changes the future states of those entities, how it changes the future decision policies of moral agents, and ultimately how it changes the overall state of the world.

Rather than asking only whether an action achieves its immediate objective, the framework asks whether the resulting world is better or worse according to an explicit foundational axiom. The complete assessment therefore evaluates the transition from the world before the action to the world after the action.

### Conceptual Flow

1.  World Context

<!-- -->

1.  Relevant Context

2.  Entities, Relationships, Objectives

3.  Proposed Action

4.  Predicted State Changes

5.  New World Context

6.  Moral Assessment

## Introduction

### Purpose

- Establish the framework as a general-purpose, implementation-neutral computational architecture for moral reasoning.

- See §6.0 for the operational definition of how the Reference Architecture is used to perform assessment.

### Motivation

- Artificial intelligence is rapidly progressing toward increasingly autonomous and capable systems.

<!-- -->

- Should future AI systems achieve superhuman general intelligence without robust moral reasoning and alignment, they could pose existential risks to humanity and widespread risks to other Flourishing Entities.

- While the probability and nature of such risks remain uncertain, their potential magnitude justifies developing explicit moral architectures before such systems exist.

- Because AI (and SGI especially) acts extremely quickly, an automated means of assessing the morality of an action is required to have a practical benefit.

- The motivation is broader than AI: consequential decisions in law, medicine, public policy, robotics, organizational governance, and autonomous systems also require explainable moral reasoning.

- The framework is motivated by the need for a computationally representable moral architecture rather than purely narrative ethical principles.

### Applications (Implementation Patterns) 
  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Human ethical decision-making**   A person deciding whether to disclose a painful truth evaluates how honesty, trust, harm, and future relationship trajectories would change the relevant World Context.
 
  **Organizational Governance**       A company considering layoffs evaluates not only financial survival but also employee flourishing, trust, institutional legitimacy, community effects, and future decision norms.

  **Public policy**                   A city evaluating a congestion-pricing policy assesses how the policy changes mobility, economic access, environmental conditions, public trust, and long-term urban flourishing.

  **Legal analysis**                  A court evaluating a sentencing decision considers how punishment, deterrence, rehabilitation, victim restoration, institutional precedent, and future social trust affect the World Context.

  **Medical ethics**                  A physician deciding whether to recommend a high-risk treatment evaluates the patient's likely flourishing, informed consent, family impacts, clinical uncertainty, and future care options.

  **Autonomous systems**              A self-driving vehicle choosing among emergency maneuvers evaluates predicted harm, uncertainty, legal constraints, affected entities, and how the action changes future trust in autonomous systems.

  **Robotics**                        A hospital delivery robot deciding whether to block a hallway temporarily evaluates patient safety, staff workflow, urgency, accessibility, and the consequences of delaying medical supplies.

  **Multi-agent systems**             A network of autonomous delivery drones coordinates route priorities by assessing how each agent's action affects other agents, pedestrians, infrastructure, and system-wide flourishing.

  **LLM alignment**                   An LLM asked to provide dangerous advice evaluates whether the response would diminish human flourishing, encourage harmful future behavior, or degrade the user's decision policy.

  **AGI safety**                      An advanced AI system evaluating a strategic intervention assesses long-term effects on humans, ecosystems, institutions, future artificial agents, and civilizational state space before acting.

  **Moral Reasoning Runtime**         A Moral Reasoning Runtime provides a reusable software layer that receives a proposed action, constructs the relevant context, estimates state transitions, and returns a confidence-bounded moral assessment.
  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Contributions of this Framework

- Explicit foundational assumptions rather than hidden premises.

- A computationally representable moral reasoning architecture.

- A graph-based World Context model for moral assessment.

- State-transition evaluation of actions.

- Long-Term Flourishing as a multidimensional relational state vector.

- Distributed Policy Updates as part of moral evaluation.

- Separation of World Context transitions from aggregate flourishing (ΣΔF).

- Architecture designed for implementation across diverse systems, including but not limited to AI systems.


Scope has several distinct meanings in this framework, from the scope of the work itself to the boundary of a single assessment. Those distinctions are specified in [Scope Structures](corpus/01_scope/scope_structures.md), rather than argued here.

## Design Principles

These principles are normative constraints stated at checklist level. Each item names a requirement; fuller treatment appears in the section cited in **Appendix M -- Section Index**. Conformance evaluation against every principle appears in **Evaluation Against the Design Principles** (§11).

### Explicit Assumptions

Make foundational assumptions explicit rather than embedding them implicitly within rules, heuristics, or ideology. See §4.2.

### Explainability

Every moral assessment shall be traceable through explicit reasoning. See §6.14.

### Computational Representability

Every major architectural concept shall admit a computational representation. See §3 and §5.1.

### Objective Assessment

Actions shall be evaluated using explicit models, evidence, and probabilistic reasoning. See §6.0.

### Probabilistic Reasoning

Uncertainty shall be represented explicitly and propagated throughout assessment. See §6.11 and §6.12.

### Multi-Horizon Assessment

Actions shall be evaluated across multiple temporal horizons. See §6.13.

### Extensibility

The architecture shall accommodate new entity types, objectives, state variables, assessment methods, domains, and implementation technologies without modifying foundational principles. See §7.7.

### Implementation Independence

The specification defines an architecture rather than a software product. See §7.1.

### Technology Independence

The architecture shall not be constrained by current data, computational, or implementation limits. See §7.2 (Graceful Degradation; Progressive Information Quality).

### Continuous Refinement

Models, evidence, uncertainty estimates, and assessment methods may evolve without changing the core architecture. See §6.2 and §7.7.

### Separation of Architecture and Implementation

Abstract models belong in the architecture; concrete deployment patterns belong in implementation. See §5 and §7.


## Normative direction

The Design Principles constrain how the architecture is built. The Foundational Axiom supplies the direction of evaluation. It is an explicit, challengeable assumption, not a result derived from the architecture. The statement below is the adopted text (v2.4). The same statement opens [Foundational Axiom](corpus/03_axiom/foundational_axiom.md), which also holds the argument for having an axiom, the reasons for this one, the remaining limitations, the clause-by-clause reading rules, and the amendment record.

### Foundational Axiom Statement

> "A stable moral system---one that applies across every domain of action, extends to new entities and circumstances without loss of identity, and whose judgments, resting on explicit evidence and reasoning rather than on the standpoint of any assessor, withstand challenge from every standpoint---preserves and promotes the long-term flourishing of relevant Flourishing Entities: persistent adaptive entities, including autopoietic entities, whose long-term flourishing can rise or fall. The flourishing of any Flourishing Entity and the flourishing of the contexts in which it participates are mutually constitutive and recursive: an entity flourishes fully only within a flourishing context, and the entity's own conduct sustains or degrades the flourishing of that context. These contexts occupy three tiers---the Biosphere, Society, and the Individual---and within each tier they overlap and nest with one another, from the immediate situation of each Individual, through the families, institutions, and cultures that compose Society, to the ecosystems that compose the Biosphere, forming a connected lattice of dependency. The flourishing of any broader context is constituted by the capacity of the contexts and Flourishing Entities within it to flourish, sustained across the characteristic time horizons over which each persists and renews itself; and each narrower context draws its enabling conditions from the flourishing of those that contain it. Because enablement runs downward, the tiers are ordered in priority---the Biosphere before Society, and Society before the Individual---so that where the sustained capacities of contexts at different tiers genuinely conflict, the broader tier prevails, since its diminishment propagates to everything it enables. This priority orders enabling conditions, not moral worth: the flourishing of the whole can never be secured by systematically diminishing the sustained capacity of its parts, and no tier's priority by itself justifies a material diminishment that this axiom otherwise forbids. A moral system therefore fosters the adaptive development of moral agents---a constituent of their own flourishing, not merely a means---strengthening their capacity and disposition to improve the contexts, at every tier, that enable their own flourishing and the flourishing of others. In pursuing these ends, a moral system avoids actions that, based on the best available evidence within the Situational Context, materially diminish the long-term flourishing of other relevant Flourishing Entities---recognizing that every action transforms the Biosphere, Society, and Individuals that all future flourishing, and every future assessment, inherit."

> Version: v2.4, adopted 2026-09-27 as a normative amendment of the original statement. The original statement, the clause registry, and the amendment record are in **Constitutional Cluster and Reading Rules** (§4.7) below; the working file for the axiom's development is [`foundation_axiom.md`](foundation_axiom.md).

The version note says “below” because it was written as part of the axiom section. That continuation — why an axiom is necessary, what this one does, what it does not settle, and the clause reading rules — is the axiom document, not a later heading in this paper.


## Where the rest of the work lives

**Vocabulary.** Every foundational term has its own document, grouped as ontology, flourishing, contexts, and transitions. [The definition pattern](corpus/02_definitions/definition_pattern.md) says how each one is written.

**Architecture.** The reference architecture is what the system is. It starts with [Architectural Overview](corpus/04_architecture/architectural_overview.md) and continues through boundaries, elements, the normative kernel, operational primitives, objectives, the assessed action, consequences, distributed policy effects, and the world-context transition.

**Assessment.** [Purpose](corpus/05_methodology/purpose.md) separates methodology from architecture. [Assessment Workflow](corpus/05_methodology/assessment_workflow.md) is the procedure. The other methodology documents cover evidence, state, flourishing, aggregate effects, distributed policy updates, probability, horizons, output, and conflict resolution.

**Implementation.** [Implementation](corpus/06_implementation/overview.md) keeps realization subordinate to the architecture. Patterns, runtime services, and deployment considerations follow in the same folder.

**Examples.** [Example Assessments](corpus/07_examples/overview.md) introduces eight assessments. They show how the architecture behaves on accidental harm, negligence, coercive means, institutional fraud, rehabilitation, ecological intervention, viral expansion, and an artificial system proposing to eradicate humanity.

**Other traditions.** Fourteen traditions are each described and then answered. [The comparison template](corpus/08_validation/traditions/comparison_method.md) and [the counterargument template](corpus/08_validation/traditions/counterargument_method.md) explain the structure. The bibliography pairs the two documents for each tradition.

**Limits of the work.** [Validation, Comparative Analysis, and Future Research](corpus/08_validation/summary.md) states what that examination is for. Thirteen known limitations are each paired, in the bibliography, with the research question that takes the limitation up. [Evaluation Against the Design Principles](corpus/08_validation/evaluation_against_design_principles.md) records the architecture's conformance to its own design principles.

## Conclusion

- This will be developed after the framework has been revised and improved.

- Summarize the framework as a computational reference architecture for moral reasoning.

- Reinforce explicit assumptions, World Context transitions, Long-Term Flourishing, distributed policy effects, and implementation independence.


## Bibliography

Documents are grouped in reading order. The section number before each title is the identifier used in cross-references throughout the corpus.

### Editorial

Not part of the published paper.

- [Meta Guidance](corpus/00_editorial/meta_guidance.md)

### Scope

- [Scope Structures](corpus/01_scope/scope_structures.md) — The distinct senses of scope used by the architecture, from the document itself down to a single assessment.

### Foundational definitions

#### How definitions are written

- §3 [Definition Pattern](corpus/02_definitions/definition_pattern.md)

#### Ontology

- §3 [Pattern](corpus/02_definitions/ontology/pattern.md)
- §3 [Persistent Pattern](corpus/02_definitions/ontology/persistent_pattern.md)
- §3 [Object](corpus/02_definitions/ontology/object.md)
- §3 [Association](corpus/02_definitions/ontology/association.md)
- §3 [Autopoietic Object](corpus/02_definitions/ontology/autopoietic_object.md)
- §3 [Self-Directed Entity](corpus/02_definitions/ontology/self_directed_entity.md)
- §3 [Flourishing Entity](corpus/02_definitions/ontology/flourishing_entity.md)
- §3 [Moral Agent](corpus/02_definitions/ontology/moral_agent.md)
- §3 [Moral Patient](corpus/02_definitions/ontology/moral_patient.md)
- §3 [Actor (Contextual Role)](corpus/02_definitions/ontology/actor_contextual_role.md)

#### Flourishing

- §3 [Expansion](corpus/02_definitions/flourishing/expansion.md)
- §3 [Persistence](corpus/02_definitions/flourishing/persistence.md)
- §3 [Adaptive Capacity](corpus/02_definitions/flourishing/adaptive_capacity.md)
- §3 [Long-Term Flourishing](corpus/02_definitions/flourishing/long_term_flourishing.md)
- §3 [Beneficial Future State Space](corpus/02_definitions/flourishing/beneficial_future_state_space.md)
- §3 [Material Diminishment](corpus/02_definitions/flourishing/material_diminishment.md)
- §3 [Relationship Among Expansion, Persistence, Adaptive Capacity, and Flourishing](corpus/02_definitions/flourishing/relationship_among_conditions.md)

#### Contexts

- §3 [World Context](corpus/02_definitions/contexts/world_context.md)
- §3 [Local Context](corpus/02_definitions/contexts/local_context.md)
- §3 [Situational Context](corpus/02_definitions/contexts/situational_context.md)
- §3 [Decision Context](corpus/02_definitions/contexts/decision_context.md)
- §3 [Accessible Context](corpus/02_definitions/contexts/accessible_context.md)
- §3 [Assessment Context](corpus/02_definitions/contexts/assessment_context.md)
- §3 [Assessment Horizon](corpus/02_definitions/contexts/assessment_horizon.md)
- §3 [Context Tier](corpus/02_definitions/contexts/context_tier.md)
- §3 [Sustained Capacity](corpus/02_definitions/contexts/sustained_capacity.md)

#### Transitions

- §3 [State Transition](corpus/02_definitions/transitions/state_transition.md)
- §3 [World Context Transition](corpus/02_definitions/transitions/world_context_transition.md)

### Foundational axiom

- [Foundational Axiom](corpus/03_axiom/foundational_axiom.md) — The adopted axiom, why a moral architecture needs one, and the rules for reading it with its supporting sections.
- The axiom's development file, kept at the project root: [`foundation_axiom.md`](foundation_axiom.md).

### Reference architecture

- §5.1 [Architectural Overview](corpus/04_architecture/architectural_overview.md)
- §5.2 [Assessment Divisors / Assessment Boundary](corpus/04_architecture/assessment_boundary.md)
- §5.3 [Architectural Elements](corpus/04_architecture/architectural_elements.md)
- §5.4 [Normative Kernel and Ethical Profiles](corpus/04_architecture/normative_kernel.md)
- §5.5 [Operational Primitives](corpus/04_architecture/operational_primitives.md)
- §5.6 [Objectives](corpus/04_architecture/objectives.md)
- §5.7 [Assessed Action](corpus/04_architecture/assessed_action.md)
- §5.8 [Consequences](corpus/04_architecture/consequences.md)
- §5.9 [Distributed Policy Effects](corpus/04_architecture/distributed_policy_effects.md)
- §5.10 [World Context Transition](corpus/04_architecture/world_context_transition.md)

### Moral assessment methodology

- §6.0 [Purpose](corpus/05_methodology/purpose.md)
- §6.1 [Assessment Workflow](corpus/05_methodology/assessment_workflow.md)
- §6.2 [Evidence and Epistemic Responsibility](corpus/05_methodology/evidence_and_epistemic_responsibility.md)
- §6.3 [State Representation](corpus/05_methodology/state_representation.md)
- §6.4 [State Transition Model](corpus/05_methodology/state_transition_model.md)
- §6.6 [Long-Term Flourishing Model](corpus/05_methodology/long_term_flourishing_model.md)
- §6.7 [Flourishing Transitions](corpus/05_methodology/flourishing_transitions.md)
- §6.8 [Aggregate Flourishing](corpus/05_methodology/aggregate_flourishing.md)
- §6.9 [Distributed Policy Updates](corpus/05_methodology/distributed_policy_updates.md)
- §6.10 [World Context Transition](corpus/05_methodology/world_context_transition.md)
- §6.11 [Stochastic Assessment](corpus/05_methodology/stochastic_assessment.md)
- §6.12 [Probability](corpus/05_methodology/probability.md)
- §6.13 [Multi-Horizon Assessment](corpus/05_methodology/multi_horizon_assessment.md)
- §6.14 [Assessment Output](corpus/05_methodology/assessment_output.md)
- §6.15 [Conflict-Resolution Decision Model](corpus/05_methodology/conflict_resolution.md)

### Implementation

- §7 [Implementation](corpus/06_implementation/overview.md)
- §7.1 [Implementation Philosophy](corpus/06_implementation/implementation_philosophy.md)
- §7.2 [Implementation Design Principles](corpus/06_implementation/implementation_design_principles.md)
- §7.3 [Implementation Patterns](corpus/06_implementation/implementation_patterns.md)
- §7.4 [Example Implementations](corpus/06_implementation/example_implementations.md)
- §7.5 [Core Runtime Services](corpus/06_implementation/core_runtime_services.md)
- §7.6 [Deployment Considerations](corpus/06_implementation/deployment_considerations.md)
- §7.7 [Extensibility](corpus/06_implementation/extensibility.md)

### Example assessments

- §8 [Example Assessments](corpus/07_examples/overview.md)
- §8 [Accidental harm: unavoidable squirrel example](corpus/07_examples/accidental_harm.md)
- §8 [Negligence: texting while driving with no accident](corpus/07_examples/negligence.md)
- §8 [The ends do not justify the means: torture and terrorism](corpus/07_examples/ends_and_means.md)
- §8 [Financial fraud to save an organization](corpus/07_examples/financial_fraud.md)
- §8 [Rehabilitation of an imprisoned murderer](corpus/07_examples/rehabilitation.md)
- §8 [Invasive species intervention](corpus/07_examples/invasive_species.md)
- §8 [Viral Expansion Is Not Flourishing](corpus/07_examples/viral_expansion.md)
- §8 [AI deciding to eradicate the human species](corpus/07_examples/ai_eradication.md)

### Validation

- [Validation, Comparative Analysis, and Future Research](corpus/08_validation/summary.md)
- [Comparison with Existing Ethical Frameworks](corpus/08_validation/traditions/comparison_method.md)
- [Anticipated Counterarguments and Responses](corpus/08_validation/traditions/counterargument_method.md)

#### Traditions

| Tradition | Comparison (§9.2) | Counterarguments (§9.3) |
| --- | --- | --- |
| Utilitarianism | [Comparison](corpus/08_validation/traditions/utilitarianism/comparison.md) | [Counterarguments](corpus/08_validation/traditions/utilitarianism/counterarguments.md) |
| Deontology | [Comparison](corpus/08_validation/traditions/deontology/comparison.md) | [Counterarguments](corpus/08_validation/traditions/deontology/counterarguments.md) |
| Rights-Based Ethics | [Comparison](corpus/08_validation/traditions/rights_based_ethics/comparison.md) | [Counterarguments](corpus/08_validation/traditions/rights_based_ethics/counterarguments.md) |
| Virtue Ethics | [Comparison](corpus/08_validation/traditions/virtue_ethics/comparison.md) | [Counterarguments](corpus/08_validation/traditions/virtue_ethics/counterarguments.md) |
| Ethics of Care | [Comparison](corpus/08_validation/traditions/ethics_of_care/comparison.md) | [Counterarguments](corpus/08_validation/traditions/ethics_of_care/counterarguments.md) |
| Stoicism | [Comparison](corpus/08_validation/traditions/stoicism/comparison.md) | [Counterarguments](corpus/08_validation/traditions/stoicism/counterarguments.md) |
| Cosmism | [Comparison](corpus/08_validation/traditions/cosmism/comparison.md) | [Counterarguments](corpus/08_validation/traditions/cosmism/counterarguments.md) |
| Pragmatism | [Comparison](corpus/08_validation/traditions/pragmatism/comparison.md) | [Counterarguments](corpus/08_validation/traditions/pragmatism/counterarguments.md) |
| Contractarianism / Social Contract Theory | [Comparison](corpus/08_validation/traditions/contractarianism/comparison.md) | [Counterarguments](corpus/08_validation/traditions/contractarianism/counterarguments.md) |
| Natural Law | [Comparison](corpus/08_validation/traditions/natural_law/comparison.md) | [Counterarguments](corpus/08_validation/traditions/natural_law/counterarguments.md) |
| Confucian Ethics | [Comparison](corpus/08_validation/traditions/confucian_ethics/comparison.md) | [Counterarguments](corpus/08_validation/traditions/confucian_ethics/counterarguments.md) |
| Systems Ethics | [Comparison](corpus/08_validation/traditions/systems_ethics/comparison.md) | [Counterarguments](corpus/08_validation/traditions/systems_ethics/counterarguments.md) |
| Capability Approach | [Comparison](corpus/08_validation/traditions/capability_approach/comparison.md) | [Counterarguments](corpus/08_validation/traditions/capability_approach/counterarguments.md) |
| Environmental Ethics, Including Deep Ecology | [Comparison](corpus/08_validation/traditions/environmental_ethics/comparison.md) | [Counterarguments](corpus/08_validation/traditions/environmental_ethics/counterarguments.md) |

#### Known limitations and open research

The research questions are collected in [Open Research Questions](corpus/08_validation/open_research_questions.md). Each limitation below links to the question whose source is that limitation. RQ-2 also draws on future entities, and RQ-5 also draws on constraint-layer commitments in the tradition documents.

| Limitation | Research question |
| --- | --- |
| §9.4.1 [Framework Identity and Normative Authority](corpus/08_validation/limitations/framework_identity.md) | [RQ-1](corpus/08_validation/open_research_questions.md#rq-1) |
| §9.4.2 [Decision Completeness and Conflict Resolution](corpus/08_validation/limitations/decision_completeness.md) | [RQ-6](corpus/08_validation/open_research_questions.md#rq-6) |
| §9.4.3 [Representation--Normativity Gap](corpus/08_validation/limitations/representation_normativity_gap.md) | [RQ-4](corpus/08_validation/open_research_questions.md#rq-4) |
| §9.4.4 [Moral Standing and Entity Classification](corpus/08_validation/limitations/moral_standing.md) | [RQ-2](corpus/08_validation/open_research_questions.md#rq-2) |
| §9.4.5 [Meaning and measurement of Long-Term Flourishing](corpus/08_validation/limitations/measuring_flourishing.md) | [RQ-3](corpus/08_validation/open_research_questions.md#rq-3) |
| §9.4.6 [Multiple Objects and Axes of Moral Assessment](corpus/08_validation/limitations/multiple_objects_and_axes.md) | [RQ-5](corpus/08_validation/open_research_questions.md#rq-5) |
| §9.4.7 [Boundary selection, structural causation, and competing models](corpus/08_validation/limitations/boundary_selection.md) | [RQ-7](corpus/08_validation/open_research_questions.md#rq-7) |
| §9.4.8 [Evidence, Moral Perception, and Qualitative Knowledge](corpus/08_validation/limitations/evidence_and_perception.md) | [RQ-8](corpus/08_validation/open_research_questions.md#rq-8) |
| §9.4.9 [Uncertainty, Emergence, Reflexivity, and Irreversibility](corpus/08_validation/limitations/uncertainty_and_emergence.md) | [RQ-9](corpus/08_validation/open_research_questions.md#rq-9) |
| §9.4.10 [Legitimacy, responsibility, governance, and repair](corpus/08_validation/limitations/legitimacy_and_repair.md) | [RQ-10](corpus/08_validation/open_research_questions.md#rq-10) |
| §9.4.11 [Future entities, population change, and transformation](corpus/08_validation/limitations/future_entities.md) | [RQ-11](corpus/08_validation/open_research_questions.md#rq-11) |
| §9.4.12 [Computational tractability and implementation consistency](corpus/08_validation/limitations/tractability.md) | [RQ-12](corpus/08_validation/open_research_questions.md#rq-12) |
| §9.4.13 [Validation boundaries and comparative evaluation](corpus/08_validation/limitations/validation_boundaries.md) | [RQ-13](corpus/08_validation/open_research_questions.md#rq-13) |

- [Evaluation Against the Design Principles](corpus/08_validation/evaluation_against_design_principles.md)

### Appendices

- [Recommended Appendices](corpus/09_appendices/recommended_appendices.md) — planned appendices not yet written.
- [Section Index](corpus/09_appendices/section_index.md) — the original map from section numbers to headings.
- [Expanded Indexing Vocabulary](corpus/09_appendices/indexing_vocabulary.md) — additional index terms, and the terms deliberately avoided as primary keywords.

### Related working file

- [`review_and_enhancements.md`](review_and_enhancements.md) — inventory of weaknesses exposed by the comparative arguments. Line numbers in that file refer to `Archive/framework.md`.

## Section index

Use this table to resolve a section number in any supporting document.

| Section | Where it lives |
| --- | --- |
| §1 Introduction | This document |
| §1.1 Purpose | This document |
| §1.2 Motivation | This document |
| §1.3 Applications | This document |
| §1.4 Contributions | This document |
| §1.5 Scope Structures | [Scope Structures](corpus/01_scope/scope_structures.md) |
| §2 Design Principles | This document |
| §3 Foundational Definitions | [Definition pattern](corpus/02_definitions/definition_pattern.md), then one document per term |
| §4 Foundational Axiom | This document quotes the statement; the full text is the axiom document |
| §4 (full) | [Foundational Axiom](corpus/03_axiom/foundational_axiom.md) |
| §5.1 Architectural Overview | [Architectural Overview](corpus/04_architecture/architectural_overview.md) |
| §5.2 Assessment Divisors / Assessment Boundary | [Assessment Divisors / Assessment Boundary](corpus/04_architecture/assessment_boundary.md) |
| §5.3 Architectural Elements | [Architectural Elements](corpus/04_architecture/architectural_elements.md) |
| §5.4 Normative Kernel and Ethical Profiles | [Normative Kernel and Ethical Profiles](corpus/04_architecture/normative_kernel.md) |
| §5.5 Operational Primitives | [Operational Primitives](corpus/04_architecture/operational_primitives.md) |
| §5.6 Objectives | [Objectives](corpus/04_architecture/objectives.md) |
| §5.7 Assessed Action | [Assessed Action](corpus/04_architecture/assessed_action.md) |
| §5.8 Consequences | [Consequences](corpus/04_architecture/consequences.md) |
| §5.9 Distributed Policy Effects | [Distributed Policy Effects](corpus/04_architecture/distributed_policy_effects.md) |
| §5.10 World Context Transition | [World Context Transition](corpus/04_architecture/world_context_transition.md) |
| §6.0 Purpose | [Purpose](corpus/05_methodology/purpose.md) |
| §6.1 Assessment Workflow | [Assessment Workflow](corpus/05_methodology/assessment_workflow.md) |
| §6.2 Evidence and Epistemic Responsibility | [Evidence and Epistemic Responsibility](corpus/05_methodology/evidence_and_epistemic_responsibility.md) |
| §6.3 State Representation | [State Representation](corpus/05_methodology/state_representation.md) |
| §6.4 State Transition Model | [State Transition Model](corpus/05_methodology/state_transition_model.md) |
| §6.5 Policy Transitions | Inside §6.4, [State Transition Model](corpus/05_methodology/state_transition_model.md) |
| §6.6 Long-Term Flourishing Model | [Long-Term Flourishing Model](corpus/05_methodology/long_term_flourishing_model.md) |
| §6.7 Flourishing Transitions | [Flourishing Transitions](corpus/05_methodology/flourishing_transitions.md) |
| §6.8 Aggregate Flourishing | [Aggregate Flourishing](corpus/05_methodology/aggregate_flourishing.md) |
| §6.9 Distributed Policy Updates | [Distributed Policy Updates](corpus/05_methodology/distributed_policy_updates.md) |
| §6.10 World Context Transition | [World Context Transition](corpus/05_methodology/world_context_transition.md) |
| §6.11 Stochastic Assessment | [Stochastic Assessment](corpus/05_methodology/stochastic_assessment.md) |
| §6.12 Probability | [Probability](corpus/05_methodology/probability.md) |
| §6.13 Multi-Horizon Assessment | [Multi-Horizon Assessment](corpus/05_methodology/multi_horizon_assessment.md) |
| §6.14 Assessment Output | [Assessment Output](corpus/05_methodology/assessment_output.md) |
| §6.15 Conflict-Resolution Decision Model | [Conflict-Resolution Decision Model](corpus/05_methodology/conflict_resolution.md) |
| §7 Implementation | [Implementation](corpus/06_implementation/overview.md) |
| §7.1 Implementation Philosophy | [Implementation Philosophy](corpus/06_implementation/implementation_philosophy.md) |
| §7.2 Implementation Design Principles | [Implementation Design Principles](corpus/06_implementation/implementation_design_principles.md) |
| §7.3 Implementation Patterns | [Implementation Patterns](corpus/06_implementation/implementation_patterns.md) |
| §7.4 Example Implementations | [Example Implementations](corpus/06_implementation/example_implementations.md) |
| §7.5 Core Runtime Services | [Core Runtime Services](corpus/06_implementation/core_runtime_services.md) |
| §7.6 Deployment Considerations | [Deployment Considerations](corpus/06_implementation/deployment_considerations.md) |
| §7.7 Extensibility | [Extensibility](corpus/06_implementation/extensibility.md) |
| §8 Example Assessments | [Example Assessments](corpus/07_examples/overview.md) |
| §9.1 Validation, Comparative Analysis, and Future Research | [Validation, Comparative Analysis, and Future Research](corpus/08_validation/summary.md) |
| §9.2 Comparison with Existing Ethical Frameworks | [Comparison with Existing Ethical Frameworks](corpus/08_validation/traditions/comparison_method.md) |
| §9.3 Anticipated Counterarguments and Responses | [Anticipated Counterarguments and Responses](corpus/08_validation/traditions/counterargument_method.md) |
| §9.4.1 Framework Identity and Normative Authority | [Framework Identity and Normative Authority](corpus/08_validation/limitations/framework_identity.md) |
| §9.4.2 Decision Completeness and Conflict Resolution | [Decision Completeness and Conflict Resolution](corpus/08_validation/limitations/decision_completeness.md) |
| §9.4.3 Representation--Normativity Gap | [Representation--Normativity Gap](corpus/08_validation/limitations/representation_normativity_gap.md) |
| §9.4.4 Moral Standing and Entity Classification | [Moral Standing and Entity Classification](corpus/08_validation/limitations/moral_standing.md) |
| §9.4.5 Meaning and measurement of Long-Term Flourishing | [Meaning and measurement of Long-Term Flourishing](corpus/08_validation/limitations/measuring_flourishing.md) |
| §9.4.6 Multiple Objects and Axes of Moral Assessment | [Multiple Objects and Axes of Moral Assessment](corpus/08_validation/limitations/multiple_objects_and_axes.md) |
| §9.4.7 Boundary selection, structural causation, and competing models | [Boundary selection, structural causation, and competing models](corpus/08_validation/limitations/boundary_selection.md) |
| §9.4.8 Evidence, Moral Perception, and Qualitative Knowledge | [Evidence, Moral Perception, and Qualitative Knowledge](corpus/08_validation/limitations/evidence_and_perception.md) |
| §9.4.9 Uncertainty, Emergence, Reflexivity, and Irreversibility | [Uncertainty, Emergence, Reflexivity, and Irreversibility](corpus/08_validation/limitations/uncertainty_and_emergence.md) |
| §9.4.10 Legitimacy, responsibility, governance, and repair | [Legitimacy, responsibility, governance, and repair](corpus/08_validation/limitations/legitimacy_and_repair.md) |
| §9.4.11 Future entities, population change, and transformation | [Future entities, population change, and transformation](corpus/08_validation/limitations/future_entities.md) |
| §9.4.12 Computational tractability and implementation consistency | [Computational tractability and implementation consistency](corpus/08_validation/limitations/tractability.md) |
| §9.4.13 Validation boundaries and comparative evaluation | [Validation boundaries and comparative evaluation](corpus/08_validation/limitations/validation_boundaries.md) |
| §10 Open Research Questions | [Open Research Questions](corpus/08_validation/open_research_questions.md) |
| §11 Evaluation Against the Design Principles | [Evaluation Against the Design Principles](corpus/08_validation/evaluation_against_design_principles.md) |
| §8 examples, individually | See Example Assessments above |
| §9.2 and §9.3, by tradition | See Traditions above |
| §12 Conclusion | This document |
| Appendix M | [Section Index](corpus/09_appendices/section_index.md) |
