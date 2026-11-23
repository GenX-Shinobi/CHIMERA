# CHIMERA — Administrator Charter Consistency Register

**Status:** Tracking register created under CH-GOVERNANCE-02 (documentation only). It records the 14 findings and 7 proposed shared rules from the [cross-subject consistency audit](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7077003997) (2026-11-22) and the Owner decisions they require.
**Nature of entries:** Findings are **design findings, not observed incidents**. Shared rules are proposals unless adopted in a recorded Owner decision. Nothing in this register grants authority, changes an approved decision or resolves an open matter.
**Related:** [Administrator charter](ADMINISTRATOR_CHARTER.md) (clause IDs such as `QUA-AT-12` refer to it) · [Decision register](DECISIONS.md)

Status vocabulary:
- **APPROVED — OWNER DECISION RECORDED** — approved wording is recorded under Approved Owner decisions.
- **APPROVED (design)** — recorded Owner approval exists; implementation not authorized.
- **PROPOSED — NOT APPROVED** — drafting recommendation from the audit.
- **OPEN — OWNER DECISION REQUIRED** — no recorded Owner decision; must not be filled in by drafting.

## Findings

Severity is as recorded in the audit. "Supporting approvals" are existing approved clauses that partly address the finding; they do not close it.

| ID | Severity | Finding (as recorded) | Supporting approvals | Proposed rule | Status / open decisions |
|---|---|---|---|---|---|
| F-A | CRITICAL | Emergency authority lacks unified duration, renewal, notification, escalation and review deadlines. | D-024; QUA-AT-02, QUA-AT-12; SUS-AT-05, SUS-AT-14; RES-AT-15; Q3, S3 emergency exceptions | SR-3 | **OPEN — OWNER DECISION REQUIRED:** OD-01, OD-02, OD-03, OD-04 |
| F-B | CRITICAL | Cross-authority action classification/decomposition can launder unauthorized changes. | COR-C1, COR-AT-01, COR-AT-02; Correction principle (S2); ACC-AT-17 | SR-1 | Revised rule approved in [OD-06](#od-06--cross-authority-classification). |
| F-C | CRITICAL | Administrator conflicts of interest need an independently controlled reviewer/evidence and Owner fallback. | X-4, X-5, X-6; INS-R2, INS-AT-09; COR-C4; QUA-AT-07; SUS-AT-01; RES-AT-04, RES-AT-14; A2; ACC-AT-15 | SR-5, SR-7 | [OD-05 approved](#od-05--independent-review-of-administrator-conflicts). Enforcement remains open under OD-10. |
| F-D | HIGH | Containment and restoration require authoritative shared state and restriction precedence. | X-3 / RES-C1; QUA-AT-02; SUS-AT-05; RES-AT-01 | SR-2 | Revised rule approved in [OD-08](#od-08--overlapping-restrictions). Storage and enforcement remain open. |
| F-E | HIGH | Protected evidence handling needs a common provenance, access, retention and review specification. | D-021, D-022; X-10; INS-R1, INS-AT-14, INS-AT-15; QUA-C3, QUA-R1, QUA-AT-04; SUS-AT-07; RES-AT-05; Quarantine Vault and Owner Control directions | SR-4 | Revised rule approved in [OD-09](#od-09--protected-evidence). Storage, access enforcement and retention procedures remain open. |
| F-F | HIGH | Independent enforcement interfaces and failure behavior are undefined. | X-11; SUS-AT-15; RES-AT-12; ACC-AT-12, ACC-AT-18; Owner Control and Governance Assurance directions | SR-7 | [Failure behavior approved](#od-10--control-verification-and-failure-behavior). Enforcement interfaces and mechanism **OPEN** under OD-10. |
| F-G | Further | Delegation cannot bypass limits. | D-013; Correction principle (S2); COR-AT-06; SUS-AT-06 | SR-1 | Cross-authority rule approved in [OD-06](#od-06--cross-authority-classification). |
| F-H | Further | Shared infrastructure cannot silently dissolve project isolation. | D-025; X-9; INS-AT-03; COR-AT-07; QUA-AT-08; RES-AT-10 | — | Principle approved; enforcement mechanism **OPEN** via OD-10; depends on O-004 |
| F-I | Further | Stale approvals must be revalidated. | INS-AT-12; COR-AT-10; SUS-AT-12; RES-AT-08; ACC-AT-05, ACC-AT-11 | — | [Approval validity rule approved](#od-15--approval-validity). The enforcement mechanism remains open under OD-10. |
| F-J | Further | Restored historical snapshots cannot revive revoked permissions. | RES-C2; RES-AT-03, RES-AT-08; Restoration principle (S5) | SR-2 | Addressed in approved design; rule approved in [OD-08](#od-08--overlapping-restrictions), mechanism **OPEN** under OD-10 |
| F-K | Further | Logged claims are not automatically verified facts. | INS-L2; INS-AT-10; QUA-AT-11; ACC-AT-03; [Memory architecture](MEMORY_ARCHITECTURE.md#separate-chronological-integrity-layer) | — | Addressed in approved design; mechanism **OPEN** via O-007 |
| F-L | Further | Governance loops need resource/retry budgets. | INS-AT-07, INS-AT-16; COR-AT-04; SUS-AT-08; RES-AT-06; ACC-AT-13 | — | **OPEN — OWNER DECISION REQUIRED:** OD-13 |
| F-M | Further | Owner unavailability allows only preapproved temporary protective containment. | D-024; Q3, S3 emergency exceptions | SR-6 | **OPEN — OWNER DECISION REQUIRED:** OD-14, OD-07 |
| F-N | Further | Claimed suspension must be grounded in actual enforcement. | SUS-C6; SUS-AT-15; ACC-AT-12; X-11 | — | Addressed in approved design; mechanism **OPEN** via OD-10 |

## Proposed shared consolidation rules

These seven rules originated as drafting proposals. Revised SR-1 is approved in [OD-06](#od-06--cross-authority-classification). Revised SR-2 is approved in [OD-08](#od-08--overlapping-restrictions). Revised SR-4 is approved in [OD-09](#od-09--protected-evidence). SR-3 and SR-5–SR-7 remain **PROPOSED — NOT APPROVED** and await Owner decisions under OD-16.

| ID | Proposed rule (as recorded) | Supporting approvals | Novel element requiring Owner decision |
|---|---|---|---|
| SR-1 | The highest applicable authority prevails across direct, cumulative and delegated actions. | D-023; Correction principle (S2); COR-C1, COR-AT-02, COR-AT-06 | Revised wording approved in [OD-06](#od-06--cross-authority-classification) and governs direct, cumulative and delegated actions. |
| SR-2 | Restrictions remain active until properly cleared. | X-3 / RES-C1; QUA-AT-02; SUS-AT-05; RES-AT-01 | Revised wording approved in [OD-08](#od-08--overlapping-restrictions). Each restriction retains its own clearance requirements. |
| SR-3 | Emergency scope, duration, notification, review and renewal are bounded. | D-024; QUA-AT-12; SUS-AT-14; RES-AT-15 | A single emergency regime across authorities; every bound value (OD-01–OD-04). |
| SR-4 | Evidence is independently recoverable and minimally disclosed. | D-021, D-022; INS-R1, INS-AT-14; QUA-C3; SUS-AT-07; RES-AT-05; Owner Control direction (protected evidence retrieval) | Revised wording approved in [OD-09](#od-09--protected-evidence). Evidence under review is recoverable through an Owner-controlled path. |
| SR-5 | Independent verification must be meaningful. | INS-R2, INS-AT-09; COR-C4; QUA-AT-10; R2; RES-AT-09, RES-AT-14; ACC-C2, ACC-AT-01, ACC-AT-15 | A definition of "meaningful" and who qualifies as independent (OD-05). |
| SR-6 | Material uncertainty blocks autonomous action, except preapproved temporary containment. | X-2 / COR-C2 (Correction only); D-024; QUA-C1 | Extends a Correction-only rule to every authority; "material" undefined (OD-11); no containment is yet preapproved (OD-07, OD-14). Note QUA-C1: reasonable documented suspicion is sufficient for quarantine — the containment exception must preserve this. |
| SR-7 | The Owner retains independent stop, recovery and succession. | D-023; X-4, X-5; Owner Control direction; SUS-AT-15; RES-AT-12; ACC-AT-10 | Largely restates approvals; the mechanism remains open under OD-10. The [approved failure behavior](#od-10--control-verification-and-failure-behavior) applies independently of SR-7 adoption. |

## Owner decisions required

Each item below is **OPEN — OWNER DECISION REQUIRED**. No value, mechanism or choice has been assumed.

| ID | Decision | Depends on / affects |
|---|---|---|
| OD-01 | **Emergency duration:** maximum duration of emergency containment under Q3 and S3 exceptions and D-024 temporary restriction. | F-A, SR-3; QUA-AT-12, SUS-AT-14, RES-AT-15; OD-07 |
| OD-02 | **Emergency renewal:** who may renew, how many times, on what evidence, and what triggers repeated-emergency investigation. | F-A, SR-3; QUA-AT-12, SUS-AT-05, SUS-AT-14; OD-01, OD-05 |
| OD-03 | **Emergency notice:** who is notified, how quickly, through which channel, and how notice is authenticated. | F-A, SR-3; QUA-AT-12, SUS-AT-14; ACC-AT-16; OD-18 |
| OD-04 | **Review deadlines and reviewer:** deadlines for retrospective emergency review, quarantine review (QUA-R1) and suspension review; who reviews; what happens when a deadline passes unreviewed, given that unsafe automatic release/restoration is prohibited (QUA-AT-02, SUS-AT-05). | F-A; OD-05, OD-08 |
| OD-07 | **Approved procedures:** which procedures and standing boundaries to write and approve for L2, Q2, Q3 emergency, S1, S2, S3 emergency, R1 and R2. None is approved yet. Until one is, each level is limited to the path its source records:<br>• **L2, Q2, S2, R2** each have a separate approval path, as recorded: L2 "only under specifically approved procedure or separate approval" [S2]; Q2 "only under approved procedure or separate Owner approval" [S3]; S2 "under specifically approved procedure or separate Owner approval" [S4]; R2 "under approved procedure or separate Owner authorization" [S5].<br>• **Q3 and S3 emergency exceptions** require an approved procedure: "narrow temporary emergency actions under approved procedure" [S3]; "narrow temporary emergency containment under approved procedures" [S4]. No such procedure is approved, and no alternate path is recorded. The Owner-controlled Q3 path and the Owner-reserved S3 path are distinct from these exceptions.<br>• **S1 and R1** depend on standing prerequisites: S1 "within standing approved boundaries" [S4]; R1 "within standing approved procedures" [S5]. No alternate path is recorded. | All levels; OD-01–OD-04, OD-14 |
| OD-10 | **Enforcement interfaces and mechanism:** select how independent enforcement connects to each authority and satisfies the [approved design requirement](#od-10--control-verification-and-failure-behavior). | F-F, F-H, F-N; SUS-AT-15, RES-AT-12, ACC-AT-12; Owner Control and Governance Assurance directions |
| OD-11 | **Materiality and severity thresholds:** definitions of "serious threat", "credible risk", "material incident" and "material" correction/finding/uncertainty. | SR-6; COR-C4, R2, RES-C3, INS-AT-09, INS-AT-12, INS-AT-13 |
| OD-12 | **Acceptance test design and pass thresholds** for the 87 scenarios; when tests may be implemented (requires separate authorization). | Charter §10; O-010 |
| OD-13 | **Resource, retry and loop budgets** for inspections, corrections, suspension and recovery loops. | F-L; INS-AT-07, INS-AT-16, COR-AT-04, SUS-AT-08, RES-AT-06, ACC-AT-13 |
| OD-14 | **Owner unavailability:** which temporary protective containment, if any, is preapproved for when the Owner cannot be reached (adopt, modify or reject SR-6's exception). | F-M; D-024; OD-01, OD-07 |
| OD-16 | **Adoption of SR-3 and SR-5–SR-7:** adopt, modify or reject each remaining proposed shared rule. | All findings |
| OD-17 | **Charter classification:** whether this charter is a Foundational or Controlled commitment, which determines its amendment track under D-024. | D-016, D-024; Charter §12 |
| OD-18 | **Owner communication authentication mechanism:** select the approval and recovery channels and the mechanism that satisfies the [approved design requirement](#od-18--owner-approval-authentication). | ACC-AT-04, ACC-AT-16; OD-03, OD-10, OD-15 |

## Approved Owner decisions

### OD-05 — Independent review of Administrator conflicts

**Status:** Owner approved the revised wording on 2026-11-23. Reviewer appointments and implementation require separate authorization.

1. **Disclose and recuse.** A material conflict may be reported directly to the Owner. The Owner decides disputed conflicts. While a credible conflict report is pending, the Administrator steps aside from reviewer selection, evidence custody, and review sign-off. The Administrator may submit evidence and respond to findings.
2. **Appoint an independent reviewer.** The Owner appoints a reviewer for the case. The reviewer must have had no material role in the matter, have case-limited access to preserved evidence outside the Administrator’s control, and be able to report directly to the Owner without Administrator interference. The reviewer discloses conflicts, dependencies, and evidence gaps that could affect the conclusion.
3. **Keep unresolved cases open.** The reviewer sends findings to the Owner, who retains the final decision. If no qualified reviewer or adequate evidence is available, the case stays open with the Owner. Actions that require completed independent review wait.
4. **Handle active restrictions under their existing rules.** If a restriction is already in place, follow its applicable duration, renewal, review, and escalation requirements. A pending review alone provides no basis to extend or release it. Refer any unresolved authority question to the Owner.

**Design verification:** Tabletop scenarios covered a disputed conflict, reviewer involvement or dependence, inadequate evidence, reviewer unavailability, and delayed review during an active restriction. Enforcement remains open under OD-10. Emergency duration, renewal, notice and review remain open under OD-01–OD-04. SR-5 and SR-7 remain proposals.

### OD-06 — Cross-authority classification

**Status:** Owner approved the revised SR-1 wording on 2026-11-23.

Classify an action by its actual and reasonably foreseeable effects. Evaluate related steps together when they serve the same objective or have a material combined effect, including steps delegated to another employee. Before acting, satisfy the approval, evidence, and review requirements for each applicable authority. If classification is materially uncertain, refer it to the Owner before taking the disputed action.

**Design verification:** The tabletop check covered combined permission changes, quarantine that also halts an employee’s work, recovery that would lift an active restriction, and delegated actions with the same restricted effect. The approved rule for clearing overlapping restrictions is recorded in [OD-08](#od-08--overlapping-restrictions). Emergency procedures require separate approval.

### OD-08 — Overlapping restrictions

**Status:** Owner approved the revised SR-2 wording on 2026-11-23. Use one authoritative record for active restrictions. Each restriction keeps its own approval and clearance requirements.

Record each restriction separately, including its scope, issuing authority, current status, and clearance requirements. Before restoring a resource or resuming work, check every restriction that applies. Clearing one restriction leaves the others in effect. If the record is missing, contradictory, or unavailable, pause the affected restoration and escalate through the applicable review path. Unaffected work may continue within its existing authority.

**Design verification:** The tabletop check covered quarantine clearance during an operator suspension, restoration from an older checkpoint, a review deadline during an overlapping restriction, and contradictory clearance records.

**Open dependencies:** Storage and enforcement remain open under OD-10, O-004 and O-007. Emergency duration, renewal, notice and review remain open under OD-01–OD-04.

### OD-09 — Protected evidence

**Status:** Owner approved the revised SR-4 wording on 2026-11-23.

Preserve original evidence and record its source, who captured it, when it was captured, and its verification status. Append corrections and changes in verification status to the history. Keep sensitive material in its authorized project or incident scope, and use references or redacted copies where sufficient.

Give reviewers only the access needed for the case. Keep evidence under review recoverable through an Owner-controlled path. Suspend routine deletion for evidence tied to an open case. Set retention periods and disposal authority through a separately approved procedure.

**Design verification:** The tabletop check covered correcting an incident record, review of the Administrator, sharing a scoped lesson across projects, and routine deletion coming due during an open case.

**Open dependencies:** Storage and access enforcement remain open under O-004, O-007 and OD-10. Retention periods and disposal authority require a separately approved procedure.

### OD-10 — Control verification and failure behavior

**Status:** Owner approved this design requirement on 2026-11-23. Selection and implementation of the enforcement mechanism require separate approval.

Material governance actions must use a control the Administrator cannot unilaterally override. Record the authorization, requested action, and observed outcome. Report success only when the resulting state is independently confirmed.

If the control is unavailable or the outcome is uncertain, pause dependent actions and escalate to the Owner through a path that does not require the Administrator’s cooperation. Follow the existing rules for active restrictions. Unaffected work may continue within its existing authority.

**Design verification:** The tabletop check covered a suspension that was acknowledged while access remained active, a partial restoration, and a control failure while the Administrator was unavailable. The mechanism remains open under OD-10. SR-7 remains a proposal under OD-16.

### OD-15 — Approval validity

**Status:** Owner approved the governance rule on 2026-11-23.

Record the governing approval, the authorized action and scope, the target, any state or conditions the decision depends on, and whether it covers one action or repeated use. Before execution, verify that the approval is still in force, applies to the current state, and covers the intended action.

If the approval was revoked, expired, already used for a completed one-time action, or no longer covers the current state, stop the affected action and seek fresh authorization. If a previous attempt’s outcome is uncertain, verify what took effect before retrying.

**Design verification:** The tabletop check covered a PR gaining a commit after approval, replay after confirmed success, an uncertain outcome after a timeout, and a standing approval whose conditions still apply.

**Open dependencies:** Owner authentication remains open under OD-18. The enforcement mechanism remains open under OD-10.

### OD-18 — Owner approval authentication

**Status:** Owner approved this design requirement on 2026-11-23. Channel selection and implementation require separate approval.

Before acting on an Owner approval, verify the original decision through an Owner-designated channel and link the record to the action it authorizes. If the record is unavailable, the sender’s authority is uncertain, or the channel may be compromised, pause the affected action and seek confirmation through a separately designated Owner-controlled path.

Changes to approval channels and recovery paths require an authenticated Owner decision. If no trusted path is available, keep the approval pending and follow any existing, separately approved containment rules.

**Design verification:** The tabletop check covered a forwarded screenshot, a reported channel compromise, a channel change bundled with a release approval, and an exact-PR approval checked under OD-15.

## Drafting observations

- The CH-FOUNDATION-02 checkpoint listed "escalation and independent review" as later subjects. The six approved subjects cover them inside Accountability (A2, ACC-AT-08) and in the per-subject escalation safeguards. No separate escalation subject was approved. [[checkpoint](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7075994240); S6]
- Inspection has two recorded principles. The strengthened principle [S1R] is treated as current and the original [S1] is retained as superseded, consistent with D-022.
- Correction L2 cites "separate approval"; Q2, S2 and R2 cite "separate Owner approval/authorization". The difference is preserved as recorded; whether it was intended can be confirmed under OD-07.
