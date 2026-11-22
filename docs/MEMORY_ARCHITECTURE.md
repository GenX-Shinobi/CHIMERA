# CHIMERA MEMORY — Architecture Notes

**Status:** Approved design direction; detailed schema and implementation remain open. CH-FOUNDATION-01 (2026-11-22) reconciles documentation only; no memory implementation or access-control mechanism is authorized.  
**Parent record:** [MEMORY.md](../MEMORY.md)

## Design goal
Provide durable, portable continuity across sessions, projects and supported AI platforms without confusing remembered information with authority. The repository is the persistent source of truth; conversation context and provider-specific memory may help retrieval but must not be required for correctness.

## Four memory levels

| Level | Name | Stores | Typical lifetime |
|---|---|---|---|
| 1 | Working | Current assignment, progress, blockers, active decisions, next action | Short-lived; updated frequently |
| 2 | Episodic | Events, decisions, changes, tests, failures, outcomes and lessons | Retained historical record |
| 3 | Semantic | Identity, mission, objectives, architecture, standards and established knowledge | Durable; controlled updates |
| 4 | Procedural | Role-specific methods, workflows, tool use, rules and exceptions | Durable; versioned and reviewed |

These are logical categories, not necessarily four databases. A first implementation may use ordinary Markdown files and a simple folder structure.

## Separate chronological integrity layer
The **Chronological Integrity Principle** is not a fifth memory level. It is a separate recordkeeping layer:
- Continuous, append-only and tamper-evident chronology of organizational events, memory changes, authorization decisions and corrective actions.
- Independently verifiable and recoverable to the extent supported by the eventual implementation.
- Corrections, clarifications and reversals are new linked entries. Never silently rewrite or destroy historical evidence.
- Each consequential entry should identify source, author/role, timestamp, scope, evidence, verification state and related authorization.
- A log entry is evidence of a recorded event, not proof that the event description is true. Record what was reported versus independently verified.

## Memory ownership and separation
- **CHIMERA-wide memory:** universal statutes, approved governance, shared standards and reusable lessons.
- **Organizational Chronicle:** continuous organization-level historical record.
- **Project memory:** project mission, project-specific rules, roadmap, requirements, decisions, data and status.
- **Project Chronicle:** separate timeline for each project, starting clean without resetting organizational history.
- **Employee identity memory:** reusable role identity, charter, capabilities and boundaries.
- **Employee working memory:** current assignment and relevant working notes.
- **Handoff record:** exact deliverable, recipient, completion condition, evidence and next action.

Project-specific information must not leak into another project because the same employee is reused. Employees carry reusable role identity and approved reusable knowledge, not automatic access to prior project memory.

## Persistent memory governance
All persistent employee memory must be registered, governed, traceable and subject to Administrator oversight. Metadata should identify author, date/time, source, purpose, scope, memory level, status, version/history and access classification. Administrator oversight includes the ability to inspect and audit organizationally managed persistent memory within its authorized scope.

Employees may keep task-appropriate working notes, but may not maintain hidden persistent memory as an alternative source of authority or use it to bypass statutes, access controls or authorization. Temporary working notes must not silently become permanent organizational knowledge.

Memory cannot create authority or permissions. An employee must independently verify the governing statute, current authorization, delegated scope and permission before acting.

## Record status and provenance
Consequential records should identify, as appropriate:
- Record type and memory level.
- Status: **verified fact**, **owner-approved decision**, **reported event**, **assumption**, **recommendation**, **open question**, **disputed** or **superseded**.
- Source/evidence, author/role and date.
- Scope: CHIMERA-wide, project-specific, employee-specific or task-specific.
- Version/change reference and historical links.
- Access classification and authorized roles.

A lesson or proposal must not silently become a verified fact or approved instruction. Distinguish source report from independent verification.

## Institutional learning and project isolation
Keep Organizational and Project Chronicles independent. A new project begins with a clean project-specific history while retaining access only to relevant, approved organizational knowledge.

Each reusable lesson must retain source, supporting evidence, applicability, verification status, history and usage. Lessons may be located, selected for a project, corrected, disputed or retired. A disputed lesson should not be automatically reused until reviewed. Retiring or culling a lesson removes or supersedes it in active recommendations; it does not delete its historical evidence. Record these status changes chronologically.

Use indexing, selective retrieval and archival to limit unnecessary storage and compute overhead. Archival and consolidation must preserve historical evidence and traceability.

## Access and coordination
Use least-privilege access. Read access is limited to information required for an assignment; write access is limited to authorized memory areas. Shared organizational memory is governed and versioned. Explicit handoffs do not transfer permissions or authority. No employee may create an untracked delegation chain or recursively expand its own scope.

Every handoff must name:
1. Responsible recipient.
2. Defined deliverable.
3. Completion condition.
4. Relevant source context and access scope.
5. Evidence expected back.

## Continuity and recovery
A replacement employee or different AI platform should eventually be able to locate authoritative instructions, retrieve only authorized memory, resume from a current Working record, verify provenance/status, record new events without rewriting history, and hand off work with explicit responsibility and completion criteria.

Incident response must preserve chronology: detect and flag, contain, preserve evidence, investigate, correct/recover when justified, and learn/prevent recurrence. Rollback may restore prior memory, permissions, configuration or project state where justified, but must not erase the incident record or evidence.

## First proof of concept
1. A role reads its approved charter and assignment.
2. It retrieves a relevant approved memory item.
3. It distinguishes verified information from assumptions and recommendations.
4. It records a sourced lesson in the correct memory level.
5. It creates a bounded handoff.
6. A fresh session or replacement role resumes using repository records alone.
7. An unauthorized role cannot alter protected instructions or access restricted project memory.
8. A correction adds a new chronological entry without overwriting the original.
9. A lesson marked disputed or retired is not automatically reused.

## Unresolved implementation choices
- Exact folder layout and file naming.
- Whether a small metadata header/schema is sufficient.
- How to represent and enforce access control across platforms.
- Technical tamper-evidence, signing, verification and independent recovery.
- Optional indexing/search mechanisms with an offline/manual fallback.
