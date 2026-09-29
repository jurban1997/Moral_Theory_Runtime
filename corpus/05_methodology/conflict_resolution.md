[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §6.15

*Moral Assessment Methodology. This layer defines how the architecture is used to perform an assessment.*

# Conflict-Resolution Decision Model

Assessment Output preserves conflict: axis findings may disagree, profiles may diverge, and "justified indeterminacy" is a valid output state. But an actor who must act cannot execute an indeterminacy. This section defines the layer between findings and action: a **minimum decision rule** guaranteeing that every assessment that supports a decision terminates in exactly one of three defined ways --- a selected action with a recorded rationale, a structured escalation, or a pre-declared default. The rule has two mandatory operations, in order: the **contextual hierarchy is assessed** (every conflict is located in, and disciplined by, the Foundational Axiom's tier and lattice structure), and the **subsequent state is jointly optimized** (candidates are compared by the resulting World Context *and* the resulting state of the moral agent, together).

## Purpose and Status

This model is deliberately a *minimum*. It does not supply the complete conflict-resolution procedure that §9.4.2 records as open --- it does not fix the materiality threshold's weighting method, cross-axis commensurability rules, within-tier sibling rankings, or a population axiology (§10 RQ-5, RQ-6). What it guarantees is structural: a defined decision path exists from multidimensional findings to a selection or a governed escalation, so that indeterminacy is never resolved silently, by omission, or by the actor's untracked preference. The full procedure, when developed, must refine this rule's comparison stages; it may not bypass them.

The rule is constrained by three prior commitments it must not violate: kernel item 4 (material diminishment is not overridden by aggregate benefit), kernel item 8 and the Integration Protocol (no composite moral score replaces axis-specific reasoning --- so "optimize" below never means scalar maximization), and the Foundational Axiom's tier priority with its anti-sacrifice corollary (§4.7: the ordering governs genuine cross-tier conflicts of sustained capacity and never by itself justifies a material diminishment).

## Decision Inputs

The model consumes artifacts the methodology already requires:

- The **feasible candidate set** (Stage 0) and, for each candidate, the predicted **World Context Transition** (World Context₀ → World Context₁) with confidence bounds;

- **Axis findings** for each candidate (Multidimensional Assessment Axes), including interaction notes;

- The **tier declaration** from Assessment Boundary Selection step 4: every materially affected context located in its Context Tier with dependency links, populated across all three tiers;

- **Material Diminishment findings** for every relevant Flourishing Entity, with the actor's justification burden stated;

- Predicted **Distributed Policy Updates** for the Actor, observers, and institutions (§6.9), which carry the agent's subsequent policy state;

- The **characteristic horizons** of every materially affected context (§6.13), so that sustained capacity is compared as level and trend at each.

## The Minimum Decision Rule

> Among feasible candidate actions that survive the side-constraint screen, the assessment first locates every materially affected context in the contextual hierarchy and resolves cross-tier conflicts under the axiom's tier priority and within-tier conflicts over the meet and join of the conflicting contexts. It then selects the candidate whose **subsequent state** --- the resulting World Context and the resulting moral-policy state of the agent --- is **jointly optimized**: no feasible alternative produces a better resulting World Context without degrading the agent's policy state or materially diminishing others, and no alternative produces a better agent state at the expense of the resulting World Context. Where joint comparison does not select uniquely, the tier ordering and then preservation of beneficial future state space decide; where these do not decide, the conflict escalates under a pre-declared default policy. The decision, its stage, and its discarded alternatives are recorded without collapsing the axis findings.

The two optimization objects are not an arbitrary pairing: they are the axiom's recursion rendered as a decision criterion. The resulting World Context carries the flourishing of affected entities and the sustained capacity of the contexts they participate in; the agent's subsequent policy state carries the feedback mechanism by which contexts are improved (§4.7, mutual constitution and adaptive development). A candidate that improves the world while corrupting the agent degrades the mechanism all future improvement depends on; a candidate that develops the agent at others' material expense fails the side-constraint. Optimizing either object alone reproduces, at the decision layer, exactly the failure the axiom forbids at the constitutional layer.

## Stage 0 --- Feasible Candidate Set

Enumerate the credible alternatives, not only the proposed action: inaction, delay, partial implementation, mitigation, delegation, staged experimentation, system redesign, and escalation-as-action. Inaction is a candidate like any other --- it produces its own World Context Transition and is assessed identically, never treated as a neutral baseline that requires no justification. The declared baseline for comparison is recorded.

## Stage 1 --- Side-Constraint Screen

Remove every candidate that materially diminishes the Long-Term Flourishing of another relevant Flourishing Entity where a feasible alternative avoids that diminishment. If every surviving candidate materially diminishes someone --- the tragic case --- no candidate is removed on this ground; instead the comparison proceeds under the Material Diminishment primitive's tragic-choice discipline (severity, necessity, and distribution, with the burden of justification on the actor) and the axiom's tier priority supplies the ordering where the sustained capacities of contexts at different tiers genuinely conflict (§4.7). The **interim escalation rule** applies throughout: any plausibly material diminishment of a vulnerable or non-consenting Flourishing Entity escalates to human review rather than resolving silently.

## Stage 2 --- Contextual-Hierarchy Assessment

No comparison of candidates may proceed on an undeclared or partial hierarchy. The tier declaration must be complete before Stage 3: every materially affected context located in exactly one tier (Biosphere, Society, Individual) with its dependency links declared, an empty tier justified rather than assumed, and any claim that a *tier's* sustained capacity is at stake stated and evidenced separately from the interests of the context making the claim.

Each conflict the candidates raise is then classified and disciplined:

1. **Cross-tier conflicts** --- where a candidate's effects on the sustained capacities of contexts at different tiers genuinely conflict, the broader tier's sustained capacity prevails (tier priority), subject in full to the anti-sacrifice corollary and the necessity, proportionality, and least-damage test. The priority orders enabling conditions, not moral worth; it decides *whose capacity weighs more* in the comparison, and never itself licenses a diminishment.

2. **Within-tier conflicts** --- where sibling contexts in the same tier conflict (family against firm, one ecosystem against another), the candidates are compared by their effect on the sustained capacity of the **meet** (what the siblings share) and the **join** (the smallest context containing both) of the conflicting contexts. A residual ranking rule among siblings when meet-and-join analysis does not decide remains open (§10 RQ-6); until it exists, an undecided within-tier conflict is a Stage 4 escalation, not an assessor's discretion.

The output of this stage is a set of hierarchy constraints --- which candidates are ruled out or ordered by the tier discipline --- that bind Stage 3.

## Stage 3 --- Joint Subsequent-State Optimization

For each surviving candidate `a`, the assessment holds two predicted objects:

- `W₁(a)` --- the resulting World Context: the Long-Term Flourishing of affected Flourishing Entities, the sustained capacity (level *and* trend, at each affected context's characteristic horizons) of the contexts declared in Stage 2, and the beneficial future state space preserved, expanded, or foreclosed.

- `P₁(a)` --- the agent's subsequent moral-policy state: whether the candidate strengthens or degrades the Actor's own decision policies, deliberative capacities, and dispositions, and what Distributed Policy Updates it propagates to observers and institutions (§6.9).

Candidate `a` **jointly dominates** candidate `b` when `a` is at least as good as `b` on every mandatory comparison dimension of `W₁` and on `P₁`, and strictly better on at least one. All comparisons are axis-preserving: dimensions are compared each on their own terms, and no scalar aggregate is formed (kernel item 8).

Selection proceeds in order; the first step that selects uniquely, decides:

1. **Joint dominance.** If one candidate jointly dominates every alternative, select it.

2. **Non-degradation preference.** Among non-dominated candidates, discard any that purchases World Context gains through degradation of the agent's policy state --- corrupting means --- where a feasible alternative achieves comparable World Context results without that degradation; and symmetrically, discard any that develops the agent's capacities at the cost of a worse resulting World Context that a feasible alternative avoids.

3. **Hierarchy ordering.** Among remaining candidates, prefer the candidate that better preserves the sustained capacity of the broadest tier genuinely affected, applying the Stage 2 constraints (tier priority under the anti-sacrifice corollary).

4. **Future-possibility preservation.** Among remaining candidates, prefer the candidate that preserves or expands beneficial future state space --- the more reversible, more correctable, less foreclosing option --- so that residual uncertainty in the comparison can be repaired by later reassessment.

5. **Residual indeterminacy.** If no unique selection results, the indeterminacy is *justified* --- and it is handed to Stage 4, never resolved by silent default.

## Stage 4 --- Escalation and Pre-Declared Defaults

A conforming implementation must declare, before deployment, how residual indeterminacy resolves:

- **Escalation path** --- the designated human or institutional authority that receives the full decision record, and the authority type (Authority Matrix) that legitimates its choice;

- **Response deadline** --- the time by which escalation must resolve, matched to the decision's tempo;

- **Default action policy** --- for time-critical contexts where escalation cannot resolve in time (the autonomous-system case the Motivation raises): the default is the Stage-1-surviving candidate that best preserves future state space and reversibility --- typically the most interruptible, least foreclosing option --- executed with an automatic reassessment trigger. A default policy may never be "proceed with the originally proposed action because no objection resolved in time."

Indeterminacy is thereby preserved as information (the disagreement remains visible in the record) while the system's behavior remains defined.

## Decision Record

Every decision this model produces appends to the Assessment Output:

- The candidate set, the declared baseline, and each discarded candidate with the stage and ground of its removal;

- The Stage 2 hierarchy declaration and conflict classifications relied upon;

- The selection stage that decided (dominance, non-degradation, hierarchy ordering, future-possibility, or escalation) and the comparison it rested on;

- The axis findings, unmodified --- selection never rewrites or collapses findings;

- For escalations: the record transmitted, the deciding authority, and the disposition;

- Reassessment triggers: the evidence changes under which the selection must be re-run.

## Methodological Boundary and Open Elements

This model defines the minimum decision layer, not the complete procedure. Open elements, tracked in §9.4.2 and §10: the materiality threshold's structure and weighting method (RQ-5); commensurability and structured-balancing rules across axes and profiles (RQ-6); the within-tier sibling ranking rule (RQ-6); population-affecting comparisons (RQ-11); and the audit mechanism for hierarchy declarations (RQ-7). Refinements must preserve this section's guarantees: the side-constraint screen precedes optimization, the hierarchy is assessed before candidates are compared, both subsequent-state objects are mandatory, and no refinement may reintroduce a composite score or an unrecorded default.

