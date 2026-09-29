[Objective-Based Systems Ethics](../../Objective-Based_Systems_Ethics.md) · §5.2

*Reference Architecture. This layer defines what the system is, without equations or an implementation.*

# Assessment Divisors / Assessment Boundary

The Assessment Boundary is the architectural component that determines which portions of the World Context are relevant enough to be included in the assessment. It defines the boundary between the complete theoretical World Context and the narrower contexts used for evaluation. See **Architectural Elements → Assessment Boundary** for the architectural definition of this element.

Assessment Divisors are the dimensions used to configure or apply the Assessment Boundary. These may include application scope, domain scope, entity scope, causal scope, temporal scope, epistemic scope, perspective scope, jurisdictional scope, authority scope, and computational scope. The Assessment Boundary is the architectural mechanism; the Assessment Divisors are the selected scoping dimensions that determine how the boundary is drawn.

The Assessment Boundary does not determine the moral conclusion by itself. Instead, it defines the assumptions under which the assessment is performed. A boundary that excludes relevant entities, consequences, time horizons, or evidence may produce a lower-confidence assessment or an incomplete moral conclusion. For this reason, the boundary should be explicit, inspectable, and revisable.

The Assessment Boundary is first applied broadly to reduce the World Context into a Local Context. It is then applied more specifically to derive the Situational Context used to evaluate the Assessed Action. In complex assessments, the boundary may be iteratively refined as new relevant Objects, Associations, causal pathways, or evidence become apparent.

The Assessment Boundary should preserve traceability. A moral assessment should be able to identify why certain Objects, Associations, consequences, horizons, or evidence sources were included or excluded. When the boundary is uncertain or contested, that uncertainty should be carried forward into the confidence assessment in the Moral Assessment Methodology.

## World Context

In this section, the World Context is the complete theoretical superset from which the Assessment Boundary selects the portions included in a specific assessment. See **Architectural Elements → World Context** for the architectural definition. 

## Local Context

In this section, the Local Context is the domain-level subset produced when the Assessment Boundary is applied broadly to the World Context.  See **Architectural Elements → Local Context** for the architectural definition. 

## Situational Context

In this section, the Situational Context is the action-specific subset produced when the Assessment Boundary is applied to derive the evidentiary and state boundary for the Assessed Action.  See **Architectural Elements → Situational Context** for the architectural definition. 

## Relationship Among Context Layers

The Context Stack is a progressive filtering structure. The World Context is the theoretical superset. The Assessment Boundary determines what is relevant enough to consider. The Local Context narrows the assessment to a domain or class of moral questions. The Situational Context narrows the assessment further to the specific Assessed Action.

This structure allows the framework to remain both comprehensive and practical. It acknowledges that moral actions occur within a complete world state, while also recognizing that assessments must operate within bounded contexts. The goal is not to pretend that the selected context is complete, but to make the selection explicit, inspectable, and confidence-sensitive.

The Context Stack also supports recursive assessment. Once an Assessed Action is evaluated, the resulting World Context may alter future Local Contexts and Situational Contexts. For example, a decision that damages institutional trust may change the context for future governance decisions. A harmful AI response may change a user's future decision policy. A legal precedent may alter the Local Context for future legal assessments. These recursive effects are part of the architecture because the output of one assessment becomes part of the input state for future assessments.

The Context Stack therefore performs three essential architectural functions. First, it bounds the assessment so that moral reasoning can be represented and performed. Second, it preserves traceability by making contextual assumptions explicit. Third, it supports recursive World Context transitions by showing how the result of one action becomes part of the context for future moral reasoning.

See **Architectural Overview → Context Stack** for the overview-level flow and **Architectural Elements** for definitions of the World Context, Assessment Boundary, Local Context, and Situational Context.

