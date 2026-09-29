[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §5.4

*Reference Architecture. This layer defines what the system is, without equations or an implementation.*

# Normative Kernel and Ethical Profiles

Objective-Based Systems Ethics is a **normatively committed, pluralistic reference architecture** for structured moral assessment. It is not a value-neutral modeling toolkit and not a presently complete ethical theory. Its moral structure consists of an invariant **normative kernel** that every conforming implementation must preserve, plus optional **ethical profiles** that extend evaluation without replacing the kernel.

## Invariant Normative Kernel

The following commitments are **mandatory** for any implementation claiming conformance with this framework:

1. **Constitutional Foundational Axiom.** The Foundational Axiom (§4.1), read together with the supporting sections named in §4.7 (the constitutional cluster), supplies the primary normative direction. Replacing it, or amending its normative content, ordinarily defines a different framework variant rather than another conforming implementation (see the amendment record in §4.7).

2. **World Context Transition as primary assessment object.** Moral assessment evaluates the complete transition from World Context before the action to World Context after it—not an isolated metric, rule label, or aggregate score alone.

3. **Explicit assumptions and evidence.** Foundational assumptions, boundary choices, evidence sources, and reasoning steps remain inspectable. Objective assessment means explicit and auditable reasoning, not value-neutrality.

4. **Material-diminishment constraint.** Pursuit of Long-Term Flourishing does not automatically justify materially diminishing other relevant Flourishing Entities or Moral Patients. Aggregate metrics inform but do not silently override concentrated or severe harm.

5. **Distributed Policy Effects.** Changes to future decision policies of Actors, observers, institutions, and systems are part of the morally assessed transition, not optional side notes.

6. **Multi-horizon evaluation.** Consequences are evaluated across materially relevant Assessment Horizons with explicit uncertainty and confidence.

7. **Assessment Boundary traceability.** Entity, causal, temporal, epistemic, and computational scope choices are documented; exclusions and sensitivity limits affect confidence.

8. **Multidimensional output.** Assessment produces separate findings across the axes defined in **Moral Assessment Methodology → Assessment Output → Multidimensional Assessment Axes**, not a single collapsed verdict.

Implementations may differ in representation, algorithms, and domain ontologies. They may not omit these kernel elements without ceasing to implement this framework.

## Ethical Profiles

An **ethical profile** is a registrable extension that adds interpretive lenses, constraints, evaluative dimensions, or procedural requirements drawn from established ethical traditions (§9.2). Profiles are **optional** but, once activated for an assessment, must be declared and applied consistently.

Each profile specification includes:

- **Profile identifier and source tradition** (for example, `rights-constraints`, `capability-thresholds`, `ecological-standing`).

- **Normative function** — interpretive lens, measurement method, hard constraint, independent evaluative axis, domain scope rule, or procedural requirement.

- **Activation conditions** — domain, institution, jurisdiction, entity types, or assessment purpose that trigger the profile.

- **Inputs required** — evidence, entities, Associations, or state variables the profile needs.

- **Outputs produced** — separate axis finding, constraint violation flag, threshold report, or procedural deficiency notice.

- **Integration maturity level** (0–5 per §9.4.3). The term **incorporated** is reserved for levels 4–5.

Illustrative profiles include:

  ------------------------------------------------------------------------------------------------------------------
  Profile (illustrative)          Primary function
  ------------------------------- ----------------------------------------------------------------------------------
  Rights and deontology           Constraints, permissions, claims, and means impermissibility

  Care and relational ethics      Relational findings, responsibility-for-care, participation tests

  Capability and substantive      Effective access, conversion factors, protected capability thresholds
  freedom

  Ecological standing             Nonhuman intrinsic value, precaution, non-substitutability flags

  Contractarian legitimacy        Consent, public justification, procedural fairness

  Virtue and agent quality        Disposition and practical-judgment axis (distinct from transition quality)

  Systems and boundary critique   Boundary disclosure, competing models, reflexivity requirements
  ------------------------------------------------------------------------------------------------------------------

Profiles may be combined. When profiles conflict, the assessment must report **separate findings per profile and axis** and record unresolved disagreement explicitly. Detailed conflict-resolution methodology is reserved for future development (§9.4.2).

## Integration Protocol

When multiple profiles and kernel criteria apply:

1. **Kernel constraints apply to all assessments** regardless of active profiles.

2. **Profiles add findings; they do not silently replace kernel outputs.** A favorable transition-quality result does not override a rights-constraint violation reported on the action-and-means axis.

3. **No composite moral score replaces axis-specific reasoning.** Integrative summaries may be produced for decision support but must cite which axes and profiles support them.

4. **Unresolved conflict is a valid output state.** "Justified indeterminacy" with disclosed disagreement is preferable to false precision. When a decision must nonetheless be made, selection and escalation are governed by the **Conflict-Resolution Decision Model** (§6.15); indeterminacy is never resolved by silent default.

5. **Profile shopping is prohibited.** Selective activation of profiles to reach a predetermined conclusion violates conformance.

## Authority Matrix

  ---------------------------------------------------------------------------------------------------------------------------------------
  Authority type              What it governs                                    Typical holder
  --------------------------- -------------------------------------------------- --------------------------------------------------------
  Philosophical authority     Foundational Axiom interpretation, kernel status   Framework authors, philosophical review body

  Interpretive authority      Profile selection, threshold interpretation        Domain ethics board, institutional review

  Institutional authority     Adoption, deployment, enforcement                  Organization, regulator, governance body

  Revision authority          Kernel amendment, profile registry changes         Documented governance process; axiom change = new variant
  ---------------------------------------------------------------------------------------------------------------------------------------

Every Assessment Output should identify which authority type justified profile activation, boundary selection, and threshold choices when those choices materially affect the result.

## Conformance

An implementation **conforms** when it preserves the invariant normative kernel, supports multidimensional output, and documents active ethical profiles. An implementation that replaces the Foundational Axiom, collapses assessment to a single utility score without axis preservation, or hides boundary exclusions produces a **distinct ethical framework**, not a conforming variant.

See §9.4.1 (*Framework Identity and Normative Authority*) for limitation analysis, failure modes, and research deliverables remaining open.


