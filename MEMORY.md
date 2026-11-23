# CHIMERA — Project Memory

**Purpose:** Durable, human-readable continuity record.  
**Authority:** This file records context and decisions; it does not grant permissions or override statutes.  
**Repository:** https://github.com/GenX-Shinobi/CHIMERA  
**Checkpoint:** 2026-11-22 — CH-FOUNDATION-01 merged (`main` `7b558f5`); Administrator charter design approved. CH-GOVERNANCE-02 documentation merged on 2026-11-23 (`8279b92`).

## Identity and mission
- Project: **CHIMERA** — **Controlled Hierarchical Intelligence, Modularity, Efficiency, Resilience & Adaptation**. The acronym expansion is formally approved.
- Mission: free-to-use, open-source, platform-independent framework for building, governing and coordinating reusable AI workforces.
- CHIMERA is separate from AI Prompt Builder Hub. Prompt Builder may become its first adopter only after v5.4.0 is publicly released and the Owner separately authorizes integration.

## Roles
- **Owner:** ultimate authority; approves statutes, scope, permanent employee/instruction changes, permissions, merges and releases.
- **CHIMERA Administrator:** initially ChatGPT; administers governance, evaluates proposals, coordinates work and prepares controlled changes. It is subject to the same statutes as all employees and cannot self-authorize changes, appoint employees or change its own permissions.
- **Engineering Lead:** Claude Code; implements owner-authorized technical work, coordinates authorized specialists and submits evidence-based improvement or hiring recommendations.
- **Specialists:** perform bounded assignments and provide evidence and recommendations within assigned permissions.

Roles must remain replaceable. CHIMERA must not depend on one model, provider or conversation history.

## Approved design directions
1. CHIMERA is a separate public repository intended to remain open source and free to use.
2. Universal statutes bind every employee and cannot be overridden by project instructions, employee instructions, milestone briefs or efficiency proposals.
3. Project-specific rules may be stricter than universal statutes but may not weaken or contradict them.
4. No speed or efficiency improvement may weaken core statutes.
5. Use bounded autonomy within owner-approved milestones; material changes return to the Owner.
6. Start from the approved roadmap, requirements and known constraints. New ideas enter a backlog rather than silently becoming active work.
7. Correction and retesting should be automated where safe and practical. Tests, requirements and statutes must not be weakened or suppressed to obtain a passing result.
8. The Administrator initially coordinates governance reviews and recruitment. It may propose a dedicated HR/Recruitment Manager when demonstrated workload and complexity justify the overhead; the Owner retains appointment approval.
9. Every organizational role must justify its overhead through measurable value to the mission and delivery.
10. Claude may recommend employees or improvements based on recurring, evidenced needs. The Administrator evaluates alternatives and overhead; the Owner makes the final hiring decision.
11. A dedicated Trainer is not approved at this stage.
12. MEMORY is foundational and should be designed before the full employee framework.
13. Use shared organizational memory with role-based access plus individual employee working memory.
14. Memory is not authority. A remembered event, lesson or proposal does not automatically become an approved instruction, fact or permission.
15. Every delegation must identify a responsible recipient, a defined deliverable and a completion condition. Prevent untracked recursive delegation.
16. Keep project-specific knowledge, credentials, data and instructions separate from universal employee identity and reusable CHIMERA knowledge.
17. Repository files are the durable source of truth. AI conversation context and provider memory are continuity aids, not authoritative records.
18. Keep collaboration concise: one subject or decision at a time, plain-English owner-facing explanations and one primary action at a time.
19. Commitments are **Foundational** or **Controlled**. Foundational commitments protect core identity/purpose and require formal constitutional amendment and explicit Owner approval. Controlled commitments may evolve only through documented proposal, impact assessment, review and explicit Owner approval.
20. External integrations such as Claude Skills and webhooks are optional adapters, never core dependencies. The core remains independently usable, portable and free of mandatory paid services.
21. All persistent employee memory must be governed, traceable and subject to Administrator oversight. Employees may have task-appropriate working space, but no hidden persistent memory may bypass statutes or authorization. Memory cannot create authority or permissions.
22. Suspicious or unauthorized actions trigger incident response: detect and flag, contain, preserve evidence, investigate, correct/recover when justified, and learn/prevent recurrence. Rollback must not erase evidence. Distinguish mistakes and ambiguity from malicious conduct.
23. The **Chronological Integrity Principle** requires continuous, tamper-evident, append-only history of organizational events, memory changes, authorization decisions and corrective actions. Corrections are new entries; history is never silently rewritten or destroyed. This is a separate history layer, not a fifth memory level.
24. Authority hierarchy: Owner → universal foundational statutes → Owner-approved controlled commitments/policies → project-specific rules → Administrator → Engineering Lead → employees/specialists. Project rules may be stricter, never weaker. No employee self-grants authority; memory and recommendations are information, not authority.
25. Foundational amendments require proposal, impact assessment, independent review, explicit Owner decision, permanent historical record and controlled implementation. Controlled amendments require documented proposal, impact assessment, explicit Owner approval, record and verification. Administrator may temporarily restrict affected operations/permissions to contain a serious threat, but cannot amend statutes or permanently expand authority.
26. Maintain an Organizational Chronicle and separate Project Chronicles. Verified, approved, appropriately scoped lessons may transfer between projects with source, evidence, applicability, verification status, history and usage. New projects start with clean project-specific histories. Retiring a lesson removes it from active recommendations, not historical evidence.

## Four-level memory model — approved
- **Level 1 — Working:** current assignment, progress, blockers, active decisions and next action.
- **Level 2 — Episodic:** events, decisions, changes, tests, failures, lessons and supporting evidence.
- **Level 3 — Semantic:** identity, mission, objectives, architecture, concepts, standards and established knowledge.
- **Level 4 — Procedural:** how an employee performs work, including rules, tools, workflows and exceptions.

Memory should be portable, human-readable and versioned. Preserve provenance and distinguish verified facts, owner-approved decisions, assumptions, recommendations and unresolved questions. All persistent memory is auditable; provider-side memory is a convenience, not the source of authority.

## Separate project: AI Prompt Builder Hub
- Repository: https://github.com/GenX-Shinobi/Prompt-Builder
- Its mission, architecture, release gates and authority remain governed by its own repository documents.
- v5.4.0 was publicly released on 2026-11-21 ([release](https://github.com/GenX-Shinobi/Prompt-Builder/releases/tag/v5.4.0)). CH-FOUNDATION-01 is authorized for documentation reconciliation only; implementation and integration require separate authorization. Private Prompt Builder evidence preservation remains separate.
- After v5.4.0 is public, future Prompt Builder roadmap work may be considered as practical CHIMERA test material under a separate bounded plan.
- CHIMERA does not inherit Prompt Builder project rules or release authority; Prompt Builder does not automatically inherit CHIMERA employee or memory permissions.

## Open questions and backlog
- Exact portable memory schema and enforceable access-control mechanism.
- Technical implementation of append-only, tamper-evident chronicle and independent recovery.
- Administrator charter: powers, limits, safeguards and principles were approved as design on 2026-11-22 and are consolidated in the [Administrator charter](docs/ADMINISTRATOR_CHARTER.md). Operational thresholds, procedures and enforcement mechanisms remain open — see the [consistency register](docs/CONSISTENCY_REGISTER.md).
- Lesson indexing, retrieval, transfer, retirement and dispute handling.
- Interactive Workforce Designer (exploratory): guided analysis of goals, workflows, tasks, workload, constraints and automation needs; drafts a justified workforce plan, roles, responsibilities, dependencies, capabilities, permissions and staged implementation. CHIMERA may draft recommendations/configuration but cannot appoint/activate employees or grant permissions without Owner approval.

## Memory governance
- Record facts with source/evidence and date where practical.
- Mark proposals as proposals until approved.
- Preserve superseded decisions in history.
- Do not store secrets, credentials or unnecessary sensitive information in shared memory.
- Apply least-privilege access.
- Never infer authority from a memory entry alone; consult current statutes, charters and Owner authorization.
- When records conflict, stop and surface the conflict rather than silently choosing one.
