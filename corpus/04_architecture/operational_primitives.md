[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §5.5

*Reference Architecture. This layer defines what the system is, without equations or an implementation.*

# Operational Primitives

The following primitives are **architecturally specified working definitions**. They are provisional but operationally usable: implementations and domain profiles must instantiate thresholds and evidence standards while preserving the structure defined here. Formal measurement rules appear in **Moral Assessment Methodology**; gap analysis appears in §9.4.

## Material Diminishment

**Material diminishment** is a decrease in the Long-Term Flourishing of a relevant Flourishing Entity or Moral Patient that is ethically significant under the Foundational Axiom—not every harm, but not only catastrophic harm.

An assessment evaluates material diminishment using:

  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Factor                    Role in materiality judgment
  ------------------------- --------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  Magnitude                 Scale of change in persistence, adaptive capacity, agency, suffering, or beneficial future state space

  Probability               Likelihood that the diminishment occurs or persists under stated uncertainty

  Duration                  Temporary burden versus enduring or lifelong loss

  Reversibility             Whether restoration, compensation, or adaptation can recover the lost flourishing

  Vulnerability             Dependence, powerlessness, or limited capacity to absorb harm

  Concentration             Whether harm falls on a few entities while benefits diffuse broadly

  Consent and legitimacy    Whether the affected entity autonomously accepted the harm under meaningful alternatives

  Cumulative and systemic   Repeated or structurally embedded harm that may be individually small but jointly material
  effects

  Future state space        Contraction of beneficial future state space, including extinction or irreversible foreclosure
  ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Working rule:** `MaterialDiminishment(o)` is true when the weighted significance of harm to entity `o` exceeds domain threshold `τ` and the harm is not justified as necessary, proportionate, and least-damaging among feasible alternatives documented in the assessment.

Material diminishment **blocks automatic permissibility** from aggregate benefit alone. It does not eliminate tragic choice: when every feasible action materially diminishes someone, the assessment compares severity, necessity, and distribution rather than declaring all options equally impermissible. The Foundational Axiom's tier priority (Biosphere > Society > Individual) supplies an ordering for that comparison when the sustained capacities of contexts at different tiers genuinely conflict; it does not waive this constraint (§4.7).

**Interim escalation rule.** Until `τ` and the factor weighting are formalized (§9.4.2, §10 RQ-5), any plausibly material diminishment of a vulnerable or non-consenting Flourishing Entity escalates to human review rather than resolving silently. The burden of justification lies with the actor; the assessment does not presume the diminishment justified.

## Moral-Patient Classification

The framework distinguishes **ontological type** (Object) from **moral status** (predicates applied to Objects):

  -----------------------------------------------------------------------------------------------------------------------------------------------------------
  Predicate              Meaning
  ---------------------- ------------------------------------------------------------------------------------------------------------------------------------
  `FlourishingEntity`    Persistent adaptive entity (autopoiesis and self-direction sufficient, not required) whose Long-Term Flourishing can rise or fall; the Foundational Axiom's primary object

  `MoralAgent`           Flourishing Entity with alternative selection and responsibility capacity

  `MoralPatient`         Entity that may be directly harmed, benefited, or represented though not a full Moral Agent

  `ValueBearingProcess`  Ecological, cultural, or abiotic feature valued directly or constitutively (habitat, watershed, sacred site)

  `NormativeRepresentative` Object authorized to speak or decide for entities that cannot participate directly
  -----------------------------------------------------------------------------------------------------------------------------------------------------------

**Working rule:** Sentience, suffering, vulnerability, dependency, ecological integrity, future existence, and inherent value may each ground `MoralPatient` or direct standing without requiring full self-direction. Classification under uncertainty must be reported with confidence and may trigger precaution when exclusion would foreclose moral consideration.

Humans with limited or developing agency, nonhuman animals, future persons, ecosystems, and qualifying artificial systems may each use entity-specific classification profiles (§5 — Normative Kernel and Ethical Profiles).

## Beneficial Future State Space

**Future State Space** is the set of possible future World Contexts reachable from the present. **Beneficial Future State Space (BFSS)** is the subset whose states satisfy all of:

1. **Value** — the state is good for the relevant entity or legitimately valued under an active ethical profile.

2. **Reachability** — the state is realistically attainable given conversion factors, resources, institutions, and constraints—not merely logically possible.

3. **Conversion support** — personal, social, and environmental conditions exist to convert nominal opportunities into genuine capabilities.

4. **Security** — the opportunity is not illusory, revocable without cause, or dependent on arbitrary authority.

5. **Compatibility** — the state contributes to the entity's flourishing without requiring material diminishment of other relevant entities beyond justified thresholds.

BFSS expansion is a positive indicator in transition-quality assessment. BFSS contraction—especially irreversible contraction—is a strong indicator of material harm even when immediate welfare metrics appear stable.

## Compatible Flourishing

**Compatible flourishing** requires that an entity's Long-Term Flourishing **contribute to** rather than undermine the long-term flourishing of the relevant World Context.

Compatibility excludes:

- Dominance or exploitation presented as expansion of the Actor's flourishing.

- Capability to harm others classified as positive flourishing merely because the Actor values it.

- Aggregate system metrics that treat severe harm to some entities as fully offset by gains elsewhere without separate material-diminishment analysis.

**Working rule:** an action that increases `LTF(actor)` while materially diminishing `LTF(o)` for another relevant entity requires separate justification through necessity, proportionality, and least-damage analysis; it is not automatically supportable merely because net aggregate flourishing rises.

## Assessment Boundary Selection

Assessment Boundary selection is an **explicit protocol**, not an implicit modeling choice:

1. **State purpose and system of interest** — identify the Assessed Action and the moral question.

2. **Provisional boundary** — initial entity, causal, temporal, and epistemic scope subject to revision.

3. **Entity and Association discovery** — include direct, indirect, remote, future, nonhuman, and low-power entities when plausibly affected.

4. **Tier declaration** — locate every materially affected context in its Context Tier (Biosphere, Society, Individual) with its dependency links declared; populate all three tiers (an empty tier must be justified, not assumed); record cross-tier conflicts of sustained capacity with the axiom's tier priority applied and the necessity, proportionality, and least-damage test documented; record within-tier conflicts over the meet and join of the conflicting contexts; and state and evidence any claim that a *tier's* sustained capacity is at stake separately from the interests of the context making the claim (§4.7).

5. **Exclusion log** — document excluded entities, contexts, effects, and evidence with rationale.

6. **Horizon rationale** — justify immediate through civilizational horizons used, including the characteristic horizons of the contexts materially affected at each tier.

7. **Competing models** — where causal structure is contested, represent materially plausible alternatives.

8. **Sensitivity analysis** — test whether conclusions change when boundary, tier-assignment, or model assumptions vary.

9. **Reflexivity check** — note whether the assessment process itself affects the World Context (measurement gaming, stakeholder chilling, etc.).

Boundary choices affect confidence, not merely convenience. Undocumented exclusion of vulnerable or remote entities, or of an affected context or tier, is a conformance failure; "relevant" in the Foundational Axiom means relevant under a conforming application of this protocol. See **Assessment Divisors / Assessment Boundary** for divisor dimensions and **§9.4.7** for remaining limitations.

