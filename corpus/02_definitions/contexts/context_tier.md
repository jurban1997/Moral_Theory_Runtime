[Objective-Based Systems Ethics](../../../Objective-Based_Systems_Ethics.md) · §3

*Foundational definition. Read the intuitive meaning, then the architectural role, then the formal specification.*

# Context Tier

## Intuitive

The three nested levels at which the world an action affects can be viewed: the living planet, the human (and institutional) world within it, and the individual within that.

## Architectural

One of three exhaustive, ordered levels---**Biosphere**, **Society**, **Individual**---at which the contexts affected by an Assessed Action are located. Within each tier, contexts overlap and nest (ecosystems within the Biosphere; families, institutions, and cultures within Society; the immediate situation of each Individual within the Individual tier), forming a connected lattice of dependency. Each narrower tier draws its enabling conditions from the tiers containing it; each broader tier's flourishing is constituted by the sustained capacity of the contexts and Flourishing Entities within it. The Foundational Axiom orders the tiers by enabling priority (Biosphere before Society, Society before the Individual) for genuine cross-tier conflicts of sustained capacity; that ordering is one of enabling dependency, not moral worth, and never by itself justifies material diminishment (§4.7). The Biosphere tier is the living system of the world in which the assessment occurs.

## Formal

Function `Tier(c) ∈ {Biosphere, Society, Individual}` over contexts, with strict order `Biosphere ≻ Society ≻ Individual`. Within a tier, contexts form a lattice under containment with meet (shared constituents) and join (smallest containing context). Cross-tier conflicts of sustained capacity are resolved by `≻` subject to the Material Diminishment primitive; within-tier conflicts are evaluated over meet and join (resolution rules open, §10 RQ-6). Tier assignment of edge-case contexts is an interpretable, evidence-revisable parameter declared in the Assessment Boundary. Introduced 2026-09-27 with axiom v2.4.

