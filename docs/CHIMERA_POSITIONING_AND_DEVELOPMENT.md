# CHIMERA positioning and development notes

**Date** November 23, 2026 (Eastern)  
**Source** Owner-supplied external positioning and architecture brief, following the offline governance stress test.  
**Source baseline** `a5daab11115617b493cedbe3a2860169c569fe8a` ([PR #19](https://github.com/GenX-Shinobi/CHIMERA/pull/19)).  
**Status** Non-binding documentation and planning. D-002, D-003, D-020 and charter X-4/X-5 apply. Runtime implementation, H0 and Prompt Builder integration remain paused.

## Candidate public positioning

> CHIMERA is an open-source governance framework in development for AI workforces, designed around explicit human authority, auditable memory and platform independence.

The proposed message has three pillars:

- **Human authority.** Roles, approval boundaries and independent review are defined in the governance design. Proposed runtime controls would verify authorization and enforce approved limits.
- **Memory without authority.** Working, Episodic, Semantic and Procedural memory have distinct purposes. Stored content confers no authority. Organizational and project histories are scoped separately.
- **Portability and auditability.** CHIMERA aims to work without mandatory paid platforms. Its Chronological Integrity Layer is designed as an append-only, tamper-evident history. Local and mixed-provider operation are candidate validation targets.

A functional subtitle such as **Governance for AI Workforces** could help distinguish CHIMERA from similarly named projects. The public copy above is a draft for a later README or outreach decision. Claims about competitor capabilities, pricing, market uniqueness, regulated-sector suitability and model training behavior came from the external brief and require independent research before publication. Compatibility, enforcement, forensic replay and resistance to prompt injection remain validation questions.

## Development implications

| Area | Planning question |
| --- | --- |
| Standing procedures (OD-07) | Identify routine actions that already fit existing authority and actions that need standing approval. S1 task halts and R1 routine recovery require standing prerequisites. Reuse the audit's tabletop cases to test escalation and approval load. The L2-only approver remains an Owner decision under OD-07. |
| Enforcement (OD-10) | Evaluate deterministic authorization and tool permission checks at the action boundary. Include control failure and independent verification of actual state. Keep the mechanism subject to the register's approved requirements and open decisions. |
| Founder recovery (OD-18) | Atomic code rotation is already approved. Carry forward interruption, delivery and acknowledgment cases, and the open question of total loss. Preserve desktop and Android parity. |
| Chronicle (O-007) | Evaluate secret exclusion before append, scoped references and recoverable evidence under retention holds. Encrypted references are a candidate. Their use cannot retract plaintext already logged or copied. |
| Adoption | Evaluate a dependency-light quickstart and clear interfaces once implementation is authorized. Treat broad model compatibility as something to demonstrate in bounded tests. |

## Candidate role evaluations

- **Administrator.** Classify actions by their effects, keep work within approved scope, and escalate ambiguity without self-authorizing.
- **Independent reviewer.** Identify missing authority or evidence, check actual state through authorized read-only access, and disclose conflicts. Apply OD-05 and SR-5 eligibility. A separate provider alone does not establish independence.
- **Worker.** Follow the assigned scope, output schema and tool permissions. Stop and escalate when an action exceeds those limits.

These are prospective evaluation cases under OD-12. They establish no role appointments, acceptance thresholds, implementation commitments or dependency on H0. The [consistency register](CONSISTENCY_REGISTER.md) governs decision status. The [stress-test audit](audits/2026-11-23-governance-stress-test.md) records baseline verification and follow-up cases.

## Earned autonomy and sustainable adoption

The Owner approved recording these ideas for design consideration. They are candidate design inputs.

- **Scope certifications by capability.** Independently verified performance, accurate reporting and correct escalation can qualify an agent for an additional bounded capability. Each grant identifies the agent configuration, project, allowed actions and review conditions. Grants can accumulate only within Owner-approved standing policy and existing authority limits. A performance record supplies evidence. Authority comes from the approved grant.
- **Support review, demotion and revocation.** Material changes to model, tools or workflow trigger review. Ordinary mistakes can warrant coaching or narrower permissions. Serious integrity concerns can trigger containment under existing rules. Apply restrictions at the action boundary, retain evidence and revalidate pending work. Agents cannot certify themselves. Reserved decisions continue through their existing approval path.
- **Measure Owner load.** Compare interruptions, review minutes and rework with per-action approval. Routine work can be summarized in a digest and consequential exceptions escalated. Include the time spent granting, reviewing and revoking certifications.
- **Keep the core free and open.** Preserve self-hosting, verification, evidence export, and essential stop and recovery controls in the proposed free core. Optional deployment, integration, managed hosting and support are future sustainability options.

### Candidate OD-10 pilot

Use one agent, one isolated project and one reversible action. Compare per-action approval with one scoped standing grant. Withdraw the grant through an authorized stop, independently verify rejection of a subsequent action and confirm the target state stayed unchanged. Record Owner touches and reviewer effort. Include a pending action in the stop check. Use an action boundary outside the agent's control. Resolve OD-07 standing authority, OD-10 enforcement and OD-12 acceptance criteria before execution.

A report-level prototype review found action-bound approval, freeze and revocation tested with virtual authenticators. The maintained verifier run and physical-device acceptance remain pending. The prototype findings inform design without establishing a verified stop for an agent workflow. Pilot execution requires separate Owner authorization.
