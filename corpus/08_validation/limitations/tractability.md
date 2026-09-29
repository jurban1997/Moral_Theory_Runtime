[Objective-Based Systems Ethics](../../../Objective-Based_Systems_Ethics.md) · §9.4.12

*A known limitation of the framework and the research required to address it.*

# Computational tractability and implementation consistency

This section should establish that implementation neutrality does not imply ethical interchangeability. Different algorithms, data sources, approximations, computational resources, and privacy techniques may produce materially different classifications, predictions, and moral conclusions.

## Limitation Statement

Explain that a reference architecture can remain implementation-independent while implementations produce inconsistent results because of data, modeling, approximation, resource, and governance differences.

## Computational Tractability Versus Architectural Completeness

Distinguish what the architecture requires conceptually from what a particular implementation can represent or calculate within available time and resources.

## Resource and Time Constraints

Address processing capacity, memory, storage, latency, energy, staffing, evidence-collection cost, and deadlines that constrain assessment depth.

## Implementation Neutrality Versus Normative Equivalence

Clarify that implementations may use different technologies without silently changing the Foundational Axiom, normative constructs, protected minimums, assessment axes, or decision semantics.

## Invariant Normative Kernel

Define the concepts, rules, classifications, disclosures, and output distinctions that every conforming implementation must preserve.

## Profile-Governed Variation

Identify variations permitted only through a declared ethical, entity, domain, risk, or jurisdictional profile, including capability dimensions, ecological indicators, thresholds, and decision policies.

## Implementation-Discretionary Variation

Identify technology choices that may vary freely when they preserve required semantics, such as programming language, database, interface, deployment architecture, or specific numerical solver.

## Nonconforming Variation

Define changes that create a materially different ethical framework, including undisclosed changes to standing, value weights, constraints, thresholds, uncertainty treatment, or decision outputs.

## Scaling and Decomposition Strategies

Evaluate hierarchical modeling, modular analysis, graph partitioning, distributed computation, incremental assessment, scenario reduction, sampling, abstraction, and prioritization by materiality.

## Moral Risks of Decomposition

Address loss of cross-boundary effects, marginalized entities, feedback loops, correlated harms, relational meaning, and system-level emergence when assessments are divided into smaller components.

## Approximation Taxonomy

Distinguish numerical, sampling, temporal, spatial, causal, boundary, scenario, aggregation, heuristic, model-reduction, surrogate-model, and qualitative-coding approximations.

## Approximation Error Budgets

Allocate and track permitted error by source, component, entity class, assessment axis, horizon, and decision significance.

## Decision-Significant Error

Define approximation as material when it could change standing, threshold crossing, permissibility, ranking, responsibility, confidence, monitoring, or remedy.

## Error Propagation and Correlation

Track how data, model, numerical, boundary, and qualitative interpretation errors interact rather than assuming that errors are independent.

## Directional and Distributional Bias

Identify approximations that systematically underrepresent remote, low-frequency, low-data, vulnerable, nonhuman, or computationally expensive effects.

## Threshold-Proximity Rules

Require greater precision and escalation when an estimated value is close to a protected minimum, materiality threshold, tipping point, or prohibition boundary.

## Minimum Evidence Requirements

Define the evidence necessary before an implementation may issue exploratory, advisory, operational, high-stakes, or irreversible-action conclusions.

## Insufficient-Evidence Outputs

Require conditional, indeterminate, or restricted-use findings when minimum evidence is absent. Missing evidence should not silently be treated as absence of harm.

## Evidence Quality and Coverage

Evaluate provenance, recency, representativeness, affected-entity coverage, missingness, qualitative evidence, subgroup reliability, causal support, and independence.

## Privacy--Accuracy Trade-Offs

Assess how data minimization, de-identification, aggregation, access restrictions, noise addition, or privacy-preserving computation affect accuracy and representation.

## Minimum Necessary Data

Require collection only of data materially necessary to the assessment and prohibit additional surveillance merely because greater data could improve model precision.

## Qualitative Evidence and Computational Reduction

Prevent narrative, testimony, cultural meaning, and tacit knowledge from being discarded or reduced to unreliable categorical scores merely to simplify computation.

## Stochastic and Nondeterministic Implementations

Require disclosure and control of random seeds, sampling procedures, model stochasticity, run-to-run variation, and the stability of conclusions across repeated assessments.

## Reproducibility and Audit Replay

Define the records needed to reproduce an assessment, including data versions, model versions, configurations, profiles, assumptions, software environment, random state, and human interventions.

## Reproducibility Under Privacy Constraints

Permit controlled audit environments, synthetic test data, secure access, or verified summaries when original sensitive evidence cannot be redistributed.

## Cross-Implementation Comparability

Establish common input definitions, ethical profiles, benchmark cases, output schemas, and trace records for comparing independent implementations.

## Conformance Testing

Test normative identity, ontology, evidence processing, assessment procedure, uncertainty treatment, decision outputs, traceability, privacy protections, and governance.

## Theory-Discriminating Benchmark Cases

Use cases designed to reveal whether an implementation preserves rights, thresholds, intentions, relational obligations, ecological effects, future entities, and moral uncertainty.

## Metamorphic and Invariance Testing

Verify expected properties when irrelevant details change, affected entities are reordered, equivalent units are used, or morally material factors are added or removed.

## Sensitivity and Robustness Testing

Determine whether conclusions remain stable across reasonable changes to data, parameters, weights, boundaries, models, horizons, and approximation methods.

## Divergent Implementation Results

Require diagnostic comparison of inputs, assumptions, profiles, causal models, approximation budgets, and normative rules when conforming implementations disagree.

## Material-Variation Rules

Define when two implementations are ethically equivalent, conditionally comparable, materially divergent, or implementations of different frameworks.

## Real-Time and Time-Constrained Assessment

Establish which minimum checks may never be skipped, what may be deferred, and when time pressure requires a conservative default, escalation, or human decision.

## Degraded and Fallback Modes

Require explicit labeling when data, services, models, or computational resources are unavailable. A reduced-capability result should not appear equivalent to a complete assessment.

## Human Review and Override

Define when human review is mandatory, what evidence reviewers receive, how overrides are justified, and how repeated overrides trigger model reassessment.

## Environmental and Institutional Cost of Computation

Include energy, hardware, water, labor, infrastructure, opportunity cost, and concentration of computational authority when material to the ethical assessment.

## Implementation Access and Capability Inequality

Address the risk that only wealthy institutions can perform high-fidelity assessments, while less powerful communities receive simplified or less protective implementations.

## Certification and Continuing Conformance

Require initial testing, periodic reassessment, change-triggered recertification, incident reporting, benchmark updates, and withdrawal of obsolete conformance claims.

## Versioning and Migration

Record changes to architecture versions, ethical profiles, models, data schemas, thresholds, and algorithms and explain how prior assessments should be interpreted after changes.

## Failure Modes and Exposure

Analyze opaque approximation, false precision, benchmark overfitting, privacy laundering, model monoculture, nonreproducibility, silent degraded operation, low-data exclusion, implementation capture, and unjustified equivalence claims.

## Interim Safeguards and Mitigations

Require declared conformance profiles, error budgets, minimum evidence gates, sensitivity testing, version locking, independent benchmark testing, privacy review, and escalation of decision-unstable results.

## Research Deliverables and Acceptance Criteria

Require a conformance specification, test suite, approximation registry, error-budget standard, evidence tiers, reproducibility protocol, divergence procedure, and implementation-variation policy.

## Residual Risk

Acknowledge that technically conforming implementations may still diverge because of irreducible uncertainty, qualitative judgment, local evidence, stochastic behavior, and unresolved normative interpretation.

## Conformance layers

  -------------------------------------------------------------------------------------------------------------------------
  Conformance layer          Required consistency
  -------------------------- ----------------------------------------------------------------------------------------------
  **Normative identity**     Foundational Axiom, normative kernel, ethical-profile status, and protected constraints

  **Semantic**               Definitions of entities, relationships, flourishing, standing, actions, effects, and outputs

  **Procedural**             Required assessment stages, alternatives, boundaries, review, and escalation

  **Evidence**               Provenance, minimum quality, qualitative evidence, exclusions, and uncertainty

  **Computational**          Approximation disclosure, error propagation, stochastic controls, and threshold handling

  **Output**                 Required assessment axes, conclusion vocabulary, confidence, dissent, and remedies

  **Traceability**           Ability to connect each conclusion to evidence, assumptions, models, and normative rules

  **Privacy and security**   Minimum protections for sensitive evidence and affected entities

  **Robustness**             Sensitivity, adversarial, boundary, competing-model, and repeated-run testing

  **Governance**             Versioning, review, appeal, incident response, and continuing conformance
  -------------------------------------------------------------------------------------------------------------------------

A conformance suite should test expected structural and ethical properties rather than assuming one predetermined answer exists for every moral case.

## Permissible implementation variation

  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Variation class                    Examples                                                                                                        Treatment
  ---------------------------------- --------------------------------------------------------------------------------------------------------------- ------------------------------------------------------------------------------------
  **Invariant**                      Foundational commitments, required assessment axes, provenance, uncertainty disclosure, protected minimums      May not vary within the same framework version

  **Profile-governed**               Capability lists, ecological indicators, thresholds, jurisdictional rules, domain evidence                      May vary only through a declared and governed profile

  **Implementation-discretionary**   Programming language, storage engine, user interface, numerical solver                                          May vary if required semantics and outputs are preserved

  **Material divergence**            Different standing criteria, hidden weights, omitted axes, altered prohibitions, incompatible output meanings   Must be disclosed as a different framework variant or nonconforming implementation
  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Two implementations should not be considered ethically equivalent merely because both follow the same architectural diagram.

## Approximation error-budget record

Every material approximation should identify:

- Approximation type and purpose;

- Component or dataset affected;

- Entities and assessment axes exposed;

- Expected magnitude and direction of error;

- Correlation with other errors;

- Effect across time horizons;

- Proximity to thresholds or tipping points;

- Probability of changing the decision classification;

- Validation or comparison method;

- Mitigation and monitoring;

- Responsible owner; and

- Maximum permitted use.

If the approximation could plausibly change a decision from permissible to impermissible---or reverse a protected-minimum finding---the implementation should improve the analysis, escalate review, or report the conclusion as unstable.

## Minimum evidence tiers

  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Tier                               Intended use                                                       Minimum conclusion
  ---------------------------------- ------------------------------------------------------------------ ---------------------------------------------------------------------------------------------
  **Exploratory**                    Hypothesis formation and early analysis                            No operational moral authorization

  **Advisory**                       Low-stakes, reversible decision support                            Conditional recommendation with disclosed limitations

  **Operational**                    Material but monitorable decisions                                 Full provenance, alternatives, affected-entity coverage, and sensitivity testing

  **High-stakes**                    Serious rights, capability, ecological, or institutional effects   Independent review, competing models, stronger evidence, and enforceable monitoring

  **Irreversible or catastrophic**   Potential permanent or civilization-scale effects                  Highest evidence burden, adversarial testing, protected constraints, and explicit authority
  ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Reproducibility requirements

A reproducible assessment should preserve:

1.  Framework and ethical-profile versions;

2.  Input-data identifiers and collection dates;

3.  Evidence provenance and exclusions;

4.  Boundary and horizon definitions;

5.  Model and algorithm versions;

6.  Parameters, weights, thresholds, and assumptions;

7.  Approximation methods and error budgets;

8.  Random seeds and repeated-run distributions;

9.  Software and computational environment;

10. Human judgments, overrides, and interpretive decisions;

11. Intermediate axis-level findings; and

12. Final output and explanation.

## Rules for implementation divergence

Implementation variation should be considered **material** when it changes:

- Which entities receive moral consideration;

- Whether a protected threshold is crossed;

- Whether an action is required, permissible, or prohibited;

- Which party is assigned responsibility;

- Whether consent or legitimacy is valid;

- Whether a transition is beneficial or detrimental;

- Whether evidence is sufficient;

- Whether escalation or stopping is required; or

- Which remedies are owed.

When materially divergent results occur, the system should not average them. It should identify the source of divergence, classify the conclusion as conditional or unstable, and escalate the normative or architectural question for governance review.

The section's central conclusion should be:

> Implementation neutrality permits technological diversity, not silent normative variation. A conforming implementation must preserve the framework's normative kernel, assessment semantics, required axes, evidence standards, and traceability. Approximation is acceptable only when its decision significance is measured and disclosed; if implementation choices can reverse the moral conclusion, the result must be escalated, restricted, or classified as indeterminate.

