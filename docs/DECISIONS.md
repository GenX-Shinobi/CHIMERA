# CHIMERA — Decision Register

This register separates owner-approved decisions from unresolved questions. See [MEMORY.md](../MEMORY.md) for context. Foundational decisions D-001–D-026 reflect the owner-approved session outcomes through 2026-11-21 and were verified intact on `main` at `7b558f5` after PR #1 merged (2026-11-22). Administrator charter design approvals of 2026-11-22 are listed separately below and consolidated in the [Administrator charter](ADMINISTRATOR_CHARTER.md).

## Approved

| ID | Decision | Notes |
|---|---|---|
| D-001 | CHIMERA is a separate public, open-source, free-to-use project. | Platform independence is a design goal. |
| D-002 | Universal statutes bind every employee and cannot be overridden by employees or project instructions. | Foundational amendments require the formal owner-approved process. |
| D-003 | Project-specific rules may be stricter, never weaker than universal statutes. | Applies across all projects. |
| D-004 | No efficiency improvement may weaken core statutes. | Safety and integrity take priority. |
| D-005 | Use bounded autonomy within owner-approved milestones. | Material changes return to the Owner. |
| D-006 | MEMORY is foundational and precedes the full employee framework. | Four levels: Working, Episodic, Semantic and Procedural. |
| D-007 | Use shared organizational memory plus individual employee working memory. | Role-based access and project separation required. |
| D-008 | The Administrator is initially ChatGPT and is governed by the same statutes. | Replaceable role; no self-authorization. |
| D-009 | Do not create a dedicated HR/Governance Manager initially. | Reconsider only if demonstrated workload justifies overhead. |
| D-010 | Every role must justify organizational overhead. | Value must exceed coordination and maintenance costs. |
| D-011 | No dedicated Trainer at this stage. | Reassess only if a demonstrated need appears. |
| D-012 | Claude may recommend employee development/hiring; Owner decides. | Administrator evaluates evidence, alternatives and overhead. |
| D-013 | Every delegation has a recipient, deliverable and completion condition. | Prevent untracked recursive delegation. |
| D-014 | Prompt Builder may be CHIMERA's first adopter only after v5.4.0 release and separate Owner authorization. | Keep governance separate. |
| D-015 | CHIMERA's acronym is formally approved as “Controlled Hierarchical Intelligence, Modularity, Efficiency, Resilience & Adaptation.” | Supersedes all provisional wording. |
| D-016 | Commitments are divided into Foundational and Controlled. | Foundational changes require formal constitutional amendment and explicit Owner approval; Controlled changes require documented proposal, review and explicit Owner approval. |
| D-017 | Optional integrations (including Claude Skills and webhooks) are adapters, never core dependencies. | Core remains portable, independently usable and free of mandatory paid services. |
| D-018 | Recruitment evolves with organizational scale. | Administrator coordinates initially; may propose a dedicated HR/Recruitment Manager when evidence justifies; Owner retains appointment approval. |
| D-019 | Four-level memory architecture is foundational. | Working, Episodic, Semantic and Procedural; shared organizational memory plus individual working memory. |
| D-020 | All persistent employee memory is governed, traceable and subject to Administrator oversight. | Memory cannot create authority or permissions; no hidden persistent memory may bypass statutes or authorization. |
| D-021 | Unauthorized or suspicious actions trigger a controlled incident response. | Detect/flag, contain, preserve evidence, investigate, correct/recover where justified, and learn/prevent recurrence. Rollback must not erase evidence. |
| D-022 | Chronological Integrity Principle. | Append-only, tamper-evident history; corrections are new entries, never silent rewrites. This is a separate history layer, not a fifth memory level. |
| D-023 | Authority hierarchy is Owner → universal foundational statutes → Owner-approved controlled commitments/policies → project rules → Administrator → Engineering Lead → employees/specialists. | Project rules may be stricter but never weaken universal statutes. Memory and recommendations are information, not authority. |
| D-024 | Foundational and Controlled amendment processes are distinct. | Foundational: proposal, impact assessment, independent review, explicit Owner decision, permanent record and controlled implementation. Controlled: documented proposal, impact assessment, explicit Owner approval, record and verification. Administrator may temporarily contain serious threats but cannot amend statutes or permanently expand authority. |
| D-025 | Organizational history and project histories remain separate while verified, approved, scoped knowledge may transfer. | New projects start with clean project histories; lessons retain source, evidence, applicability, verification status, history and usage. Retiring a lesson removes it from active recommendations, not historical evidence. |
| D-026 | Administrator oversight and intervention authority will be formally specified. | Owner agreed to proceed with this governance definition; detailed powers and limits must remain consistent with the approved authority hierarchy and temporary containment rule. |

## Open

| ID | Question | Why it matters |
|---|---|---|
| O-004 | Final portable memory schema and access-control enforcement mechanism. | Needed for reliable cross-platform memory. |
| O-007 | Exact implementation mechanics for the append-only, tamper-evident chronicle. | Must be independently verifiable and recoverable. |
| O-008 | Detailed Administrator inspection, correction, quarantine, suspension and restoration powers. | Define precise operational boundaries, approval thresholds, review and appeal/escalation. **Status (2026-11-22):** powers, limits, safeguards and principles approved as charter design (AC-1–AC-7 below); operational thresholds, procedures and mechanisms are tracked in the [consistency register](CONSISTENCY_REGISTER.md#owner-decisions-required). The Owner approved the [OD-01 initial 60-minute emergency authority cap](CONSISTENCY_REGISTER.md#od-01--emergency-duration) as a design requirement on 2026-11-23. The Owner also approved [OD-02 emergency renewal](CONSISTENCY_REGISTER.md#od-02--emergency-renewal) on 2026-11-23. One verified Owner-approved renewal may add up to 30 minutes, for a 90-minute total cap. Runtime enforcement and response-window validation remain pending. The Owner approved the [OD-05 independent-review policy](CONSISTENCY_REGISTER.md#od-05--independent-review-of-administrator-conflicts) on 2026-11-23. Enforcement remains open under OD-10. The Owner approved [OD-06 cross-authority classification](CONSISTENCY_REGISTER.md#od-06--cross-authority-classification) on 2026-11-23. The Owner approved [OD-08 overlapping restrictions](CONSISTENCY_REGISTER.md#od-08--overlapping-restrictions) on 2026-11-23. The Owner approved [OD-09 protected evidence](CONSISTENCY_REGISTER.md#od-09--protected-evidence) on 2026-11-23. The Owner approved [OD-10 control verification and failure behavior](CONSISTENCY_REGISTER.md#od-10--control-verification-and-failure-behavior) as a design requirement on 2026-11-23. The enforcement mechanism remains open. The Owner approved [OD-15 approval validity](CONSISTENCY_REGISTER.md#od-15--approval-validity) on 2026-11-23. The Owner approved [OD-18 Owner approval authentication](CONSISTENCY_REGISTER.md#od-18--owner-approval-authentication) as a design requirement on 2026-11-23. The Founder credential model is approved: one primary key, one recovery key, and an offline single-use recovery code. Broader communication channel selection, implementation, and hardware validation remain open. |
| O-009 | Detailed lesson indexing, retrieval, transfer and retirement mechanics. | Preserve institutional learning while controlling project isolation and overhead. |
| O-010 | Future milestones and acceptance criteria after the current pause. | Public release verified 2026-11-22; future milestones still require separate Owner authorization. |

## Administrator charter design approvals (2026-11-22)

Owner-approved charter **design** decisions recorded in the PR #1 thread. They specify the authority contemplated by D-026 and do not alter D-001–D-026. Implementation, enforcement and tests are not authorized. Full text: [Administrator charter](ADMINISTRATOR_CHARTER.md).

| ID | Decision | Record | Charter |
|---|---|---|---|
| AC-1 | Inspection: Option B, bounded read-only inspection authority. | [S1](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7076060217) | [§4](ADMINISTRATOR_CHARTER.md#4-inspection-authority) |
| AC-2 | Correction: strengthened Three-Level Bounded Correction Authority; 10 safeguards. | [S2](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7076171915) | [§5](ADMINISTRATOR_CHARTER.md#5-correction-authority) |
| AC-3 | Quarantine: Three-Level Bounded Quarantine Authority; 12 safeguards; Quarantine Vault direction. | [S3](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7076271162) | [§6](ADMINISTRATOR_CHARTER.md#6-quarantine-authority) |
| AC-4 | Suspension: Three-Level Bounded Suspension Authority; 15 safeguards; Independent Owner Control Mechanism direction. | [S4](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7076384538) | [§7](ADMINISTRATOR_CHARTER.md#7-suspension-authority) |
| AC-5 | Restoration: Three-Level Bounded Restoration Authority; 16 safeguards; Verified Recovery Framework direction. | [S5](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7076469959) | [§8](ADMINISTRATOR_CHARTER.md#8-restoration-authority) |
| AC-6 | Accountability: Three-Level Accountability; 18 safeguards; Independent Governance Assurance Framework direction. | [S6](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7076832115) | [§9](ADMINISTRATOR_CHARTER.md#9-accountability) |
| AC-7 | Inspection retrospective: 16 safeguards, universal test and strengthened principle; original powers unchanged; 87 scenarios total. | [S1R](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7076915462) | [§4](ADMINISTRATOR_CHARTER.md#4-inspection-authority), [§10](ADMINISTRATOR_CHARTER.md#10-scenario-inventory) |

The [cross-subject audit](https://github.com/GenX-Shinobi/CHIMERA/pull/1#issuecomment-7077003997) findings and its seven shared rules are **not** approved decisions; they are tracked in the [consistency register](CONSISTENCY_REGISTER.md).

## Exploratory backlog — not approved requirements

- Interactive Workforce Designer: a guided session that gathers organizational goals, workflows, tasks, workload, constraints and automation needs, then drafts a minimum-justified workforce plan, roles, responsibilities, task assignments, dependencies, capabilities, permissions and staged implementation. CHIMERA may draft recommendations/configuration, but cannot appoint or activate employees or grant permissions without Owner approval.
- Future use of accumulated AI Prompt Builder Hub roadmap ideas as practical CHIMERA test material, only after Prompt Builder v5.4.0 is publicly released.

## Change control

- Do not change the meaning of an approved decision without Owner approval.
- New proposals remain open until explicitly decided.
- Record date, rationale and affected documents when a decision changes.
- Preserve superseded decisions in history rather than deleting their existence.
