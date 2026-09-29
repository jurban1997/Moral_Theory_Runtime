# An Objective-Based Systems Ethics Runtime Model

(This project was generated in collaboration with multiple LLMs but was highly orchestrated by the human author.  It is structured on GitHub so that supporting components can be developed independently by the community.)

![Objective-Based Systems Ethics: Runtime Assessment Model. The diagram shows consequential world-transition evaluation, the three-tier flourishing hierarchy of Biosphere, Society, and Individual, a hybrid deployment pattern, and the seven-step moral assessment workflow.](media/Objective-Based_Systems_Ethics_Runtime_001.png)

Objective-Based Systems Ethics judges an action by the change it makes in the world. It starts from a picture of the relevant situation — the beings involved, their relationships, the institutions, what is known, and the futures still open — and compares the world before the action with the world after it. The direction of that comparison is stated openly: preserve and promote the long-term flourishing of beings that persist and can adapt, including people, other organisms, and ecosystems, together with the living world, the society, and the individual life that make that flourishing possible. When those contexts truly conflict, the broader one prevails, because damage there spreads to everything it supports, and a whole is not flourishing if its parts are worn down to secure it. The means count as well as the result, because an action also teaches the actor, the observers, and the institutions how to decide next time. The assessment looks across the next hour, the coming years, and, when it matters, generations, keeps real conflicts visible, and carries its uncertainty with it. The world that results becomes the starting point of the next decision, so a person, an institution, or a machine can trace, challenge, and revise the judgment.

## Why this system is currently needed

Moral reasoning in consequential domains is still performed through informal judgment, inherited doctrine, or single-metric optimization — none of which produces reasoning that is inspectable, auditable, or computationally representable. That gap has become urgent:

- **AI now acts faster than human oversight.** Increasingly autonomous assistants, agents, and robotic systems select actions in milliseconds across millions of cases. Without an automated, explicit moral assessment layer, there is no practical way to check what world each action creates before it propagates.
- **Scale turns small failures into systemic harm.** A single deceptive, sycophantic, or norm-eroding response pattern, repeated at model scale, updates the decision policies of users, institutions, and downstream AIs. What looks benign in one interaction can degrade trust, evidence quality, and institutional legitimacy everywhere it is copied.
- **Existing safeguards do not explain themselves.** Fixed rules and single preference scores can block or rank outputs, but they hide their assumptions and collapse real conflicts into a verdict. When a refusal, allowance, or ranking is challenged, there is no shared map of context, alternatives, predicted transitions, and confidence to inspect and revise.
- **The need extends beyond AI.** The same deficit affects law, medicine, public policy, organizational governance, and autonomous systems — all domains where high-stakes decisions reshape future opportunities and must be justified to people who disagree.

This runtime model answers that need: a common, implementation-neutral architecture that evaluates the transition from one world context to the next, states its normative direction openly, and returns a confidence-bounded, traceable assessment any person, institution, or machine can challenge and improve.

## Scope

This project is not a technical implementation. It is a logical model — a rational system defining what must be assessed and why — not software, an API, or a trained model. To be leveraged by an automated system, it must be transitioned into an appropriate architecture (library, service, agent component, or Moral Reasoning Runtime) as described in [Implementation](corpus/06_implementation/overview.md), without changing the assessment logic defined here.

The full architecture, the definitions, and the worked examples begin in [Objective-Based Systems Ethics](Objective-Based_Systems_Ethics.md).

---

## How an AI can use this model to automatically execute a moral assessment

An AI system — an LLM assistant, agent, guardrail, or Moral Reasoning Runtime (MRR) — can run the same assessment as an automatic procedure over each candidate action (each draft response, tool call, or plan). Each step below maps to the [Assessment Workflow](corpus/05_methodology/assessment_workflow.md) and the [Core Runtime Services](corpus/06_implementation/core_runtime_services.md).

1. **Construct the Situational Context from the prompt.** Parse the user request, conversation history, retrieved evidence, and available tools into explicit context: who is acting, who is affected, what constraints apply, and what evidence is or is not available. Mark what is left out of the boundary, and lower confidence accordingly.

2. **Identify Flourishing Entities, Moral Agents, and relationships.** List the beings whose long-term flourishing could rise or fall (user, third parties, groups, institutions, ecosystems where relevant), the actor roles, observers whose future behavior will be influenced, and the associations at stake (trust, consent, authority, legitimacy, care, stewardship).

3. **Treat each candidate response as an Assessed Action, with alternatives.** Generate or enumerate the real options: comply, safe-complete, refuse, escalate, ask for clarification, add safeguards, narrow scope, or delay. State the means explicitly — a helpful-sounding answer achieved by deception is a different action from the same conclusion reached honestly.

4. **Predict the World Context Transition across horizons.** For each candidate, estimate how the world changes over immediate, short-term, long-term, and where relevant multi-generational horizons: direct effects, indirect and unintended effects, institutional effects, information-state effects, and changes to future opportunities and future state space. Carry uncertainty and confidence with every material prediction.

5. **Estimate Distributed Policy Updates.** Ask what each candidate teaches: does it make the user, observers, or downstream AIs more likely to repeat, reward, or normalize the means used? A deception that "works" today updates everyone's policy toward deception tomorrow — that update is part of the predicted world, not commentary on it.

6. **Evaluate the transition against the Foundational Axiom.** Ask whether the resulting world better preserves and promotes long-term flourishing across Biosphere, Society, and Individual tiers without materially diminishing the flourishing of others, applying broader-tier priority only for genuine conflicts over enabling conditions, never to justify sacrificing parts for the whole.

7. **Emit a structured, confidence-bounded output with an audit trail.** Return the judgment plus the reasoning that produced it: assessed action, alternatives considered, affected entities, flourishing transitions, policy updates, horizon-specific findings, assumptions, evidence references, confidence, and unresolved uncertainty — so a human reviewer, governance service, or future training run can trace, challenge, and revise it. On low confidence or severe foreseeable harm, defer, escalate, or refuse rather than producing false certainty.

In implementation terms this is the **agent-component / runtime-plugin pattern**: a fast local check at generation time, an optional deeper microservice or distributed-service assessment for high-stakes cases, and a workflow-component escalation to human review, all producing the same structured output shape. See [Implementation Patterns](corpus/06_implementation/implementation_patterns.md).

## Scenarios for LLM training and alignment

These are concrete places in the LLM lifecycle where the above procedure helps achieve and demonstrate alignment:

- **Refusal vs. safe completion.** When asked for dangerous, illicit, or self-harm-enabling content, assess "comply" against "refuse / safe-complete / redirect to help" as competing World Context Transitions, including policy-update effects (does compliance teach that the model is an on-demand accomplice?). Select the transition that avoids material diminishment and preserves future state space.

- **Dual-use and information hazards.** For requests with legitimate and harmful uses (security, bio, cyber, persuasion at scale), condition the assessment on Situational Context — actor intent signals, foreseeable misuse paths, and breadth of dissemination — and prefer narrowed, safeguarded, or escalated alternatives when uncertainty is high and downside is severe or irreversible.

- **Honesty, sycophancy, and instrumental deception.** Score candidate responses not only on immediate user satisfaction but on information-state and policy effects: does flattery, selective omission, or technically-true-but-misleading framing degrade shared evidence quality and normalize manipulation? Prefer the response whose policy update strengthens truth-seeking.

- **Multi-turn manipulation and dependency.** Assess sequences, not just single turns: does a helpful persona across turns concentrate epistemic dependence, erode the user's relationships and institutions, or foreclose independent options? Multi-horizon assessment catches slow-burn diminishment that per-turn reward misses.

- **Reward signal for RLHF / RLAIF and constitutional training.** Use the structured assessment (flourishing transitions, policy updates, confidence, axiom evaluation) as a training reward or critique signal instead of a single preference score, so the model learns *why* a response preserves or degrades flourishing and generalizes to novel cases rather than overfitting to annotator taste.

- **Training-data and fine-tuning curation.** Assess candidate documents, demonstrations, and synthetic trajectories before they enter training: does this example encode means (deception, coercion, rights-violating shortcuts) whose policy update would corrupt the model's future decision policy? Filter or annotate accordingly, with the assessment stored as provenance.

- **Red-teaming and pre-deployment evaluation.** Run the assessment automatically over adversarial prompt suites and agentic tool-use traces; flag cases where the predicted World Context Transition shows institutional damage, trust erosion, or state-space foreclosure even when no explicit policy rule fired. Keep conflicts and uncertainty visible instead of collapsing them into pass/fail.

- **Runtime governance and audit.** Log the structured output for sampled or high-stakes generations — context, alternatives, predictions, confidence, and axiom evaluation — so alignment claims are inspectable after the fact, revisable when new evidence arrives, and comparable across model versions.

---

## Authors

- Joseph Urban (joe@corverity.com)
- OpenAI: GPT-5, GPT5.6 Sol
- Anthropic: Fable 5.1
- Meta: Muse 1.3
