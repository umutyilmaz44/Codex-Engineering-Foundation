# Codex Engineering Foundation

**Version:** v2.3  
**Status:** Final specification — validation coverage is maintained separately  
**Purpose:** Establish, adapt, or repair a project's agentic engineering environment and verify that it can support ongoing engineering and knowledge maintenance.

---

## 1. Purpose and Scope

The Foundation brings a project from its available starting state to a common standard of readiness for agentic engineering with Codex.

Its job is to:

1. discover the project's intent, implementation, instructions, knowledge, and working conditions;
2. identify what prevents effective ongoing engineering;
3. establish, adapt, or repair the smallest sufficient engineering environment;
4. demonstrate that the environment is usable;
5. transfer daily work and knowledge maintenance to that environment before product engineering begins.

The standard defines required capabilities. Their implementation adapts to the project.

The Foundation does not prescribe a repository template, technology stack, architecture, document set, development methodology, or agent topology. It does not require a complete PRD, final architecture, or finished implementation.

Creating documentation alone does not complete bootstrap. The resulting environment must enable meaningful engineering work without repeatedly reconstructing stable project context.

Bootstrap establishes the environment; it does not advance the product backlog. Once an environment is ready, its first feature, bug fix, migration, or other product task belongs to daily agentic engineering and must be tracked, scoped, and validated as such.

## 2. Lifecycle and Terminology

**Foundation:** This reusable guide for establishing and validating the environment.

**Bootstrap:** The bounded process of discovering, preparing, and validating a project's agentic engineering environment.

**Agentic engineering environment:** The project-specific instructions, accessible knowledge, context navigation, working tools and setup, verification practices, and continuity mechanisms needed for ongoing engineering.

**Codex-ready project:** A project whose environment satisfies the seven capabilities in Section 4 at a level appropriate to its stage and intended engineering work.

**Agentic engineering:** Daily feature development, investigation, bug fixing, refactoring, testing, migration, and maintenance performed after bootstrap.

**First meaningful work:** The next engineering task when one has been established by the user or an authoritative project source. Bootstrap prepares for it without executing it. If no next task is selected, use the intended class of daily work to assess readiness; selecting a backlog item is not a prerequisite for environment setup. Do not invent a task or choose an easier scope to bypass a genuine environment gap.

**Representative validation task:** A non-implementing walkthrough of established upcoming work or a relevant existing workflow/change. It proves that a future session can locate applicable instructions, intent or visible decision gaps, implementation areas, verification paths and prerequisites, and knowledge-maintenance locations. An existing example is navigation evidence, not a new backlog commitment or authorization to review, fix, or accept the product change.

```text
AVAILABLE PROJECT STATE
          ↓
FOUNDATION-GUIDED BOOTSTRAP
          ↓
VALIDATED ENGINEERING ENVIRONMENT
          ↓
DAILY ENGINEERING + KNOWLEDGE MAINTENANCE
```

The Foundation establishes the environment. The environment must then support daily work without depending on repeated execution of the Foundation.

## 3. Operating Principles

> Understand enough to establish the smallest environment that enables reliable, effective engineering.

- Inspect before asking; preserve useful structure before replacing it.
- Standardize capabilities, while adapting artifacts and tools to the project.
- Distinguish current implementation from accepted product intent.
- Resolve uncertainty when it materially affects readiness; deliberately defer other decisions.
- Persist durable knowledge where it belongs and reference it elsewhere.
- Verify usability rather than counting generated files.
- Keep effort proportional to project complexity, uncertainty, and risk.

Discovery should stop when remaining uncertainty does not materially affect the next bootstrap decision. Complete knowledge is not a prerequisite for useful work.

## 4. Required Readiness Capabilities

Every Codex-ready project must provide all seven capabilities. The evidence used to demonstrate them depends on the project's stage.

| Capability | Required outcome | Readiness evidence |
|---|---|---|
| **1. Project direction** | Purpose, relevant scope, important constraints, and current versus target state are understandable. | Codex can orient a relevant daily task without inventing product intent or reconstructing basic project direction. |
| **2. Working instructions** | Project-specific rules, repository boundaries, instruction scopes, and decision boundaries are clear. | Applicable instructions can be located; material conflicts affecting work are resolved. |
| **3. Context access** | Relevant knowledge, authoritative sources, and implementation areas are discoverable progressively. | A representative task can be traced to its required context without loading the entire knowledge base. |
| **4. Ability to perform work** | Tools, dependencies, setup, and execution paths support the project's current stage. | Relevant existing commands have been attempted, or a greenfield starting path is sufficiently prepared for the first engineering task without implementing that task. |
| **5. Verification** | Meaningful changes have appropriate ways to assess correctness. | Relevant checks and acceptance criteria are identifiable; actual check results and execution limitations are distinguished. |
| **6. Continuity** | Future sessions can recover necessary decisions, constraints, and continuing work state. | Essential context is accessible outside the original conversation; a future session can find the next work and its prerequisites. |
| **7. Maintenance** | Daily work preserves useful project knowledge and instructions as the project changes. | Project-local guidance states when and where affected knowledge and navigation should be updated. |

These capabilities do not require seven documents or any particular directory structure.

Readiness is assessed for the project at its current stage and intended daily work, including a concrete initial task when one is established. State that scope honestly; do not claim that unverified platforms, components, or workflows have been validated. In a large project, provide overall navigation and identify any areas whose working conditions remain unverified.

## 5. Starting Scenarios

Classify the starting state to choose a discovery strategy. Scenarios may overlap; the list is not exhaustive. For an unfamiliar case, identify its relevant characteristics and assess the same seven capabilities.

| Scenario | Primary approach | Particular requirement |
|---|---|---|
| **Greenfield** | Discover intent and critical constraints; establish the initial working environment. | Enough direction and preparation to start meaningful engineering; no complete PRD or application implementation required. |
| **Brownfield without an agentic environment** | Inspect code, tests, configuration, runtime, and existing documentation; preserve and extend useful structure. | Derive current-state knowledge from evidence and add the missing operating guidance. |
| **Existing agentic environment repair** | Audit instructions, rules, skills, memory, indexes, and generated documents. | Resolve authority and material conflicts; repair the existing system instead of creating a parallel one. |
| **Rebuild or modernization** | Investigate AS-IS evidence and TO-BE intent separately; establish their differences. | Sufficient target intent, preservation expectations, change scope, and critical migration constraints. |
| **Recovery or unknown project** | Recover reliable minimum understanding from available evidence. | Make important uncertainty visible; prioritize understanding over architectural improvement. |

For a project already meeting the standard, validate the relevant evidence, make only justified repairs, and hand off. Re-running the Foundation should not create another layer of structure.

## 6. Starting a Bootstrap

Use the Foundation in the target project's working context with the available sources and the user's intended outcome.

An example invocation is:

> Apply the Codex Engineering Foundation to this project. Inspect its current state, identify the applicable scenarios, and establish or repair the smallest environment that satisfies the readiness capabilities. Preserve useful existing structure. Ask only for material information that cannot reasonably be discovered. Validate the resulting environment and report readiness, remaining limitations, and the handoff to daily engineering.

Adapt the request to any explicit scope, such as inspection only, a particular component, or preparation for modernization. Reading or reviewing this document is not by itself an instruction to modify a project.

Proceed through:

```text
CLASSIFY → DISCOVER → UNDERSTAND → ASSESS GAPS → RESOLVE
                  ↑                              ↓
                  └──── REVISIT AS NEEDED ────────┘
                            ↓
                 DESIGN → BUILD / ADAPT
                            ↓
                      VALIDATE → HANDOFF
```

This lifecycle is iterative. Do not require a separate document, approval, or ceremony for every phase.

## 7. Discovery and Sufficient Understanding

Inspect available sources before designing the environment:

- user requirements, accepted decisions, designs, and product sources;
- repository structure, source code, tests, schemas, and API specifications;
- existing agent instructions, documentation, knowledge indexes, and skills;
- build scripts, dependency declarations, development setup, and configuration;
- runtime behavior, logs, deployment guidance, and operational constraints when relevant;
- legacy systems or external technical documentation when needed.

Synthesize enough understanding of purpose, users, workflows, business rules, architecture, data, integrations, and constraints to make the next important bootstrap decision.

Knowledge domains are discovery prompts, not mandatory documentation categories. Do not inspect every implementation detail or every external system merely because it exists.

An existing document may be stale. Source code may implement unintended behavior. A listed command may never have been verified in the current environment. Preserve these distinctions during discovery.

## 8. Evidence, Authority, and Decision State

### 8.1 Information status

Distinguish the basis of material claims when it affects engineering decisions:

- **CONFIRMED:** Established by an authoritative source or accepted decision for the question being answered.
- **OBSERVED:** Directly observed in code, configuration, runtime, or another concrete source.
- **INFERRED:** Derived from evidence but not established directly.
- **UNKNOWN:** Insufficient information.
- **CONFLICTING:** Credible sources disagree about the same question.

These labels describe information status, not a universal ranking of sources. Observed code can establish implementation behavior without establishing intended product behavior.

### 8.2 Decision state

Keep decision state separate from information status:

- **ESTABLISHED:** A decision has been accepted within its applicable scope.
- **DEFERRED:** A decision has deliberately been postponed because it does not block readiness.
- **UNRESOLVED:** A required choice remains open; assess whether it blocks bootstrap.

For material deferred decisions, record why deferral is acceptable and what event or future task requires revisiting them. Do not build an exhaustive decision register for trivial choices.

### 8.3 Authority

Authority depends on the question:

| Question | Potential authoritative source |
|---|---|
| Intended product behavior | Accepted requirement or product decision |
| Business rule | Accepted domain decision |
| Architecture direction | Accepted architecture decision |
| Current implementation | Verified code or runtime evidence |
| API contract | Applicable specification or accepted contract tests |
| Legacy behavior | Verified legacy evidence |

When sources conflict, identify the question, examine their authority and scope, and resolve the conflict deliberately when required. Do not silently select the convenient source or promote inference to fact.

Project knowledge authority does not override applicable instruction precedence, user authorization, or tool permissions.

## 9. Gap Resolution and Questions

A gap is a missing or unreliable capability that materially harms future engineering. A missing document is not automatically a gap.

For each material gap:

1. determine whether the answer can reasonably be discovered;
2. investigate available evidence where useful;
3. determine its effect on readiness;
4. resolve it if blocking, or defer it deliberately when acceptable;
5. retain only the explanation future work needs.

**Bootstrap-blocking gaps** prevent a required capability within the stated environment scope. They must be resolved before declaring readiness. Explain which capability is unavailable and why relevant engineering cannot proceed; an unfinished product task is not itself a bootstrap blocker.

**Non-blocking gaps** may remain if their limits are understood and effective engineering can proceed. Acknowledging a blocking gap does not turn it into a non-blocking one. Distinguish environment prerequisites from task acceptance: missing access necessary for the intended daily work may block readiness, while not yet having executed a future feature-specific integration test does not by itself do so. Record when each deferred prerequisite must be resolved.

| Example | Typical assessment, subject to project context |
|---|---|
| Modernization has no agreed purpose or initial target scope. | Blocking: legacy evidence cannot supply target intent. |
| Required runtime cannot be used and no viable development or verification alternative exists. | Blocking for work requiring that runtime. |
| A future hosting provider has not been selected and initial work is independent of hosting. | Deferrable. |
| A known test failure has been reproduced and the next task is to investigate or fix it. | Potentially non-blocking: the environment supports meaningful engineering. |
| A required device is unavailable, but relevant work can be checked with an adequate alternative. | Potentially non-blocking; state what the alternative cannot prove. |
| A component has no tests and no suitable way to evaluate the intended change has been established. | Blocking for that work until a meaningful verification approach is established. |

Ask the user when undiscoverable intent, material ambiguity, or a consequential choice requires their judgment. Inspect first, resolve higher-level intent before dependent details, and keep questions specific and easy to answer.

Do not ask again for decisions or authorization already established. Make routine reversible choices within the authorized scope. Follow applicable permission requirements for actions outside that scope.

## 10. Modernization Requirements

Modernization requires two connected discovery tracks:

```text
AS-IS EVIDENCE       TO-BE INTENT
       \               /
        PRESERVE / CHANGE / REMOVE / INTRODUCE
                       ↓
          TARGET ENGINEERING ENVIRONMENT
```

For AS-IS, capture relevant capabilities, workflows, rules, data, integrations, permissions, platform dependencies, and operational behavior. Keep important claims traceable to evidence.

For TO-BE, establish enough intent to answer:

- **Why:** What motivates modernization?
- **Target:** What should the new system become?
- **Preserve:** Which important capabilities or behaviors must remain?
- **Change or remove:** What is intentionally allowed or expected to change or disappear?
- **Initial scope:** What should the first meaningful target-system work serve?
- **Critical constraints:** Which platform, migration, data, business, operational, or regulatory constraints govern that work?

Distinguish what the legacy system does from how it does it. Neither copying every legacy behavior nor discarding legacy domain knowledge is an acceptable default.

A complete backlog, final technology selection, or implementation-level design is unnecessary unless a particular choice is required for readiness. Sufficient TO-BE intent is mandatory.

## 11. Information Structure and Context Routing

Keep three kinds of information distinguishable:

| Kind | Meaning | Examples |
|---|---|---|
| Instructions | What Codex should do | Conventions, boundaries, verification requirements, maintenance behavior |
| Knowledge | What Codex should know | Product rules, architecture, integration behavior, accepted decisions |
| Evidence | What exists or was observed | Code, tests, schemas, configuration, runtime observations |

Give each durable piece of knowledge one authoritative home whenever practical. Reference useful existing sources instead of maintaining equivalent descriptions in parallel.

Make navigation progressive:

```text
PROJECT ENTRY POINT → TASK-RELEVANT KNOWLEDGE → IMPLEMENTATION / EVIDENCE
```

Use an appropriate operational entry point, such as AGENTS.md, to expose project identity, scoped working instructions, important constraints, setup and verification routes, knowledge navigation, and maintenance expectations. Respect existing instruction scope and hierarchy.

Keep detailed knowledge in suitable existing locations. An entry point should direct work rather than contain the entire project encyclopedia. Verify that referenced paths and relevant external sources are accessible; a link alone does not prove that a future session can use the source.

Repository knowledge should provide a durable, auditable foundation for engineering context. Existing external authoritative systems can remain authoritative when access and navigation are reliable. Preserve enough repository-local orientation to expose dependencies and access limitations without duplicating those systems or copying sensitive information.

Agent memory is supplementary. Essential engineering context must not depend solely on private memory or the original conversation.

## 12. Designing and Building the Environment

After sufficient discovery and gap assessment, determine:

- which project-specific instructions must be available immediately;
- which durable knowledge is missing and where it belongs;
- how tasks reach relevant knowledge and implementation;
- which setup, tools, dependencies, or configuration are necessary for initial work;
- how meaningful changes will be verified;
- how continuity and maintenance will work;
- which existing artifacts should be preserved, adapted, consolidated, or retired.

Create a new knowledge artifact only when its content is durable, useful for future engineering, not already adequately represented, and costly or risky to rediscover. Prefer extending a suitable existing home.

Apply the smallest justified changes. Depending on the project, these may include instructions, links, corrected setup commands, configuration examples without secrets, or a small development scaffold needed to enable initial work.

For greenfield projects, a scaffold may include empty layers, composition wiring, dependency declarations, a placeholder screen, or a liveness check when they are necessary to demonstrate setup. It must not implement a product vertical slice, seed product data, expose a business endpoint, or add a real workflow merely to prove readiness. Record every bootstrap code change and why it enables the environment rather than product behavior.

Do not expand bootstrap into feature implementation or product architectural refactoring. Limit repository organization, configuration and tooling changes to the smallest authorized environment repair. Substantial infrastructure provisioning is separate work unless explicitly included in setup scope. A product task may be used for navigation, but new implementation or product acceptance must not be performed to manufacture bootstrap evidence. Existing code and tests remain valid discovery and working-condition evidence. If readiness requires substantial remediation beyond the authorized scope, identify that work and report the unresolved blocker rather than claiming completion.

No specific CI provider, hosting service, skill, multi-agent arrangement, memory system, vector database, or knowledge graph is required. Introduce tooling only when it has demonstrated value for the project.

## 13. Working Environment and Verification Setup

For an existing implementation, identify and, where relevant and authorized, attempt the smallest useful set of development and verification commands. Capture the working directory, prerequisites, and necessary non-secret configuration so another session can reproduce them.

For greenfield work, prepare enough to begin the actual first task. A runnable application is not mandatory before code exists. If the next task is initial implementation, required platform and setup choices must be sufficiently resolved to start it. If the next task is a necessary architectural investigation, establish its inputs and decision criteria; do not use an artificial investigation task to bypass a known implementation blocker. Do not start the task while preparing for it.

Verification can include tests, builds, static checks, contract checks, runtime observations, UI checks, or explicit acceptance criteria. Select methods appropriate to the work; do not mandate every method for every project.

Distinguish check outcomes:

- **PASSED:** Executed successfully for the stated scope.
- **FAILED:** Executed and failed; report the failure and its readiness impact.
- **BLOCKED:** Could not execute because a prerequisite, access, or environment condition was unavailable.
- **NOT RUN:** Not attempted; explain when the omission matters to readiness.
- **NOT APPLICABLE:** Does not apply at the current project stage; identify the appropriate alternative where needed.

Never represent a documented command as a successful check. When execution is unavailable, assess whether an adequate alternative supports meaningful work. If not, readiness remains blocked.

Existing product defects and failing tests do not automatically make the engineering environment unusable. Conversely, a successful build alone does not establish the seven readiness capabilities. Inspect command and import side effects before execution; a development label or dry-run flag does not establish isolation. Existing relevant isolated checks can demonstrate working conditions without invoking external systems. Document what those checks cannot prove and when broader verification becomes necessary.

## 14. Continuity and Daily Maintenance

Transfer the following behaviors into project-specific operating guidance. Leaving them only in the Foundation is insufficient.

### 14.1 Starting and finishing daily work

Future tasks should begin from the applicable project instructions, load task-relevant knowledge, inspect relevant implementation, perform the work, and verify the result appropriately.

When work establishes useful durable understanding, locate its authoritative home and update it. Update navigation if the information's location changes. Do not create a document for every task.

### 14.2 Maintenance triggers

Within the same work, update affected authoritative knowledge when a change alters:

- a documented product or business rule;
- an accepted architectural decision or material constraint;
- an API or integration contract;
- a development, execution, or verification command;
- an important repository boundary or knowledge location;
- an operational assumption that future engineering depends on.

When a task reveals materially stale or conflicting guidance, correct it if the resolution is established and within scope. Otherwise make the uncertainty visible at the relevant location and identify the decision needed. Do not silently overwrite intent with observed behavior.

### 14.3 Continuing work across sessions

For unfinished work that must continue elsewhere, preserve only the necessary current state: objective, relevant decisions, completed changes, verification results, blockers, and next action. Use the project's existing task or handoff mechanism when adequate.

Temporary work state is distinct from durable project knowledge. Retire or archive it when its purpose ends. A transcript or chronological activity log is not a substitute for current authoritative guidance.

## 15. Safety and Preservation

Respect existing user work, instruction scope, and tool permissions throughout bootstrap.

Before deleting or replacing documentation, assess its authority and continuing value. Preserve useful historical knowledge through appropriate references or archives where necessary; do not retain obsolete guidance as current instruction.

Treat credentials, secrets, production configuration, permissions, migrations, destructive changes, and irreversible actions according to the applicable authorization requirements. A bootstrap request is not blanket authorization for production changes or destructive remediation.

Do not persist secrets in project instructions or knowledge. Describe required configuration and access without exposing sensitive values.

## 16. Practical Readiness Validation

Validate the resulting environment from the perspective of a future session, using three proportional checks.

### 16.1 Task navigation

Select a representative validation task as defined in Section 2. If the user has requested only environment setup, a relevant existing workflow or change is sufficient; do not require a new product assignment. Starting from the project entry point, locate:

- applicable instructions and constraints;
- relevant accepted intent and authoritative knowledge;
- the implementation area, or the intended starting area when no implementation exists;
- an appropriate verification method and prerequisites;
- the place to record any durable knowledge affected by the task.

Use the resulting project artifacts and accessible sources, not unstated knowledge retained from the bootstrap conversation. Stop after demonstrating context acquisition and planned verification. Do not write a product feature, create business data, invoke a live integration, or convert the validation task into daily engineering. Additional examples are justified only when materially different project areas need coverage. Creating a separate agent or session is optional, not a requirement.

### 16.2 Working conditions

Attempt the relevant basic command or check described in Section 13. Record actual outcomes and evaluate failures or unavailable prerequisites against the stated daily-work scope, without performing product acceptance testing merely to finish bootstrap.

When no executable project exists, validate the initial setup path and the criteria for the first task. State clearly what cannot yet be executed.

Do not implement a feature, add artificial tests, create business data, or modify application code solely to produce evidence of readiness. If a check needs a project scaffold, keep that scaffold generic and record its bootstrap purpose.

### 16.3 Handoff independence

Confirm that future work can identify its purpose, start from local project instructions, reach required context, verify changes, and maintain affected knowledge without rereading this Foundation or reconstructing the original conversation.

Also check that material conflicts and deferrals are visible, navigation resolves, useful existing structure remains, and temporary bootstrap notes are not presented as permanent instructions.

Report the evidence concisely. A separate permanent validation document is unnecessary unless it provides continuing value.

## 17. Completion Gate

Bootstrap is complete only when:

1. all seven capabilities are supported at a level appropriate to the project stage and stated readiness scope;
2. practical validation provides evidence for that assessment;
3. no unresolved environment gap prevents required capabilities within the stated daily-work scope;
4. deferred decisions and remaining limitations are explicit where they affect future work;
5. daily operating and maintenance guidance exists in the resulting environment;
6. temporary bootstrap material has been consolidated, retired, archived, or retained only for continuing value;
7. meaningful engineering can proceed without repeating full bootstrap discovery; and
8. no product backlog work has been misrepresented as bootstrap validation.

Modernization additionally requires the TO-BE intent in Section 10.

Report the result as **READY**, with any non-blocking limitations, or **NOT READY**, with the specific blockers and required next actions. Do not use file creation, a checklist filled without evidence, or acknowledgement of a blocker as proof of completion.

Readiness does not mean that the product is defect-free, all requirements are complete, all environments are available, or all future engineering decisions have been made.

## 18. Handoff

Provide a concise summary of:

- the scenario and readiness scope;
- what was preserved, established, repaired, or consolidated;
- the project entry point and relevant knowledge locations;
- readiness evidence, commands or checks attempted, and their outcomes;
- established decisions, material observations, assumptions, conflicts, and deliberate deferrals where relevant;
- remaining limitations or blockers and their impact;
- established next work, if any; otherwise the supported daily-work scope and how a future task starts, including knowledge maintenance;
- the readiness conclusion and its basis.

Not every category needs a separate heading or artifact. Do not describe accepted decisions as unknown, deliberate deferrals as accidental omissions, or untested setup as verified.

The handoff completes the Foundation's active role. Daily engineering now operates through the project-specific environment.

## 19. Foundation Retention and Reuse

Keep the Foundation available as a reusable, versioned setup guide. It need not be copied into every target repository.

A project-local copy or version reference is optional when it helps audit or repeat setup. If retained, identify its setup role and keep it outside the routine context path. Do not instruct daily tasks to reread the whole Foundation or rerun bootstrap.

Before removing a project-local copy, ensure that required daily instructions and maintenance behavior exist independently. Do not remove an existing copy automatically merely because setup is complete.

Revisit the Foundation when conditions materially justify it, such as a major modernization, severe knowledge degradation, significant restructuring, or a broken agentic environment. Reassess affected capabilities and preserve valid existing work; ordinary knowledge updates should remain ordinary engineering maintenance.

## 20. Failure Patterns to Avoid

- **Template-first setup:** Generating identical structures regardless of project needs.
- **Documentation-only readiness:** Producing instructions without establishing usable working and verification paths.
- **Implementation as intent:** Treating observed code, especially legacy code, as the target specification.
- **Question explosion:** Asking for discoverable information or decisions unrelated to current readiness.
- **Unbounded discovery:** Continuing analysis after sufficient understanding exists.
- **Knowledge duplication:** Maintaining equivalent authoritative descriptions in parallel.
- **Permanent assumptions:** Presenting inference or unresolved choices as accepted facts.
- **Context inflation:** Loading or persisting everything encountered instead of relevant durable knowledge.
- **Unverified success:** Claiming checks passed because their commands are documented.
- **False deferral:** Labelling a genuine readiness blocker as deferred to pass the gate.
- **Process inflation:** Adding tools, agents, or infrastructure without demonstrated value.
- **Bootstrap permanence:** Making routine engineering repeatedly execute project-wide setup.
- **Bootstrap drift:** Implementing or completing acceptance of a product task while claiming to validate the engineering environment.
- **Task invention:** Turning an illustrative workflow or existing change into a user-assigned next task.
- **Project leakage:** Embedding application names, local paths, domain decisions, test logs or project readiness states in this reusable guide.
- **Acceptance confusion:** Blocking environment handoff solely because a future product change has not passed its own acceptance checks.

## 21. Maintaining and Evaluating This Foundation

Keep this guide project-independent. Project identities, local paths, domain rules, configuration, implementation findings and readiness decisions belong in the relevant project's knowledge. When evaluating the Foundation itself, keep scenario evidence and experiment outcomes in a separate evaluation record outside the reusable guide. That record is not a required artifact in every target project or part of the daily instruction chain.

Revise the Foundation only when evidence supports a reusable improvement. State the general failure mode and the rule that prevents it; do not embed the case history or encode one project's architecture, toolchain or document layout as the standard.

Assess representative starting scenarios and boundaries: new projects, existing code without agent guidance, repair of an existing environment, modernization with distinct current and target intent, already-ready environments, unavailable prerequisites, and existing user changes. Check proportionality, preservation, authority, navigation, executable evidence, maintenance, handoff independence and the stop boundary before product work.

Distinguish real project execution from document review or simulated walkthroughs. Keep untested cases and execution limitations visible in the evaluation record. Finalizing the specification does not certify every scenario or every project. A target project's readiness is always determined by its own evidence under Section 17.

## 22. Final Principle

> The Foundation succeeds when it leaves behind an engineering environment that supports useful work, preserves necessary knowledge, and no longer needs the Foundation for daily operation.

Optimize for reliable engineering, clear direction, accessible context, meaningful verification, and the smallest structure that sustains them.
