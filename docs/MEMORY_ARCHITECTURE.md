# CHIMERA MEMORY — Architecture Notes

**Status:** Approved design direction; detailed schema and implementation remain open.  
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

## Memory ownership and separation
- **CHIMERA-wide memory:** universal statutes, approved governance, shared standards, reusable lessons and framework architecture.
- **Project memory:** project mission, project-specific statutes, roadmap, requirements, decisions, data and status.
- **Employee identity memory:** reusable role identity, charter, capabilities and boundaries.
- **Employee working memory:** current assignment and relevant working notes.
- **Handoff record:** exact deliverable, recipient, completion condition, evidence and next action.

Project-specific information must not leak into another project because the same employee is reused. Employees carry reusable role identity and approved reusable knowledge, not automatic access to prior project memory.

## Record status and provenance
Consequential records should identify, as appropriate:
- Record type and memory level.
- Status: **verified fact**, **owner-approved decision**, **assumption**, **recommendation**, **open question** or **superseded**.
- Source/evidence, author/role and date.
- Scope: CHIMERA-wide, project-specific, employee-specific or task-specific.
- Version/change reference.
- Access classification and authorized roles.

A lesson or proposal must not silently become a verified fact or approved instruction.

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

## First proof of concept
1. A role reads its approved charter and assignment.
2. It retrieves a relevant approved memory item.
3. It distinguishes verified information from assumptions and recommendations.
4. It records a sourced lesson in the correct memory level.
5. It creates a bounded handoff.
6. A fresh session or replacement role resumes using repository records alone.
7. An unauthorized role cannot alter protected instructions or access restricted project memory.

## Unresolved implementation choices
- Exact folder layout and file naming.
- Whether a small metadata header/schema is sufficient.
- How to represent and enforce access control across platforms.
- Change history, archival and conflict reconciliation.
- Optional indexing/search mechanisms with an offline/manual fallback.
