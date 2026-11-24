# CHIMERA governance stress-test audit

**Date** November 23, 2026 (Eastern)  
**Baseline** CHIMERA commit a5daab11115617b493cedbe3a2860169c569fe8a, associated with PR #19 in the offline handoff.  
**Provenance** External AI governance review supplied by the Owner. The Administrator checked the claims below against files retrieved at the pinned GitHub commit. External spoofing, stale-approval and privilege-escalation passes were reported without case-level evidence in the supplied brief. This review verifies documentation, with runtime behavior untested.

This is project-scoped audit evidence for continuity under D-022 and D-025. Proposed changes carry no approval or operating authority. The checkpoint remains paused for runtime, H0 and Prompt Builder integration.

## Findings and follow-up

1. **OD-07 standing procedures — confirmed dependency.** The register's open-decisions table and charter introduction say S1 and R1 require standing prerequisites, and Q3 and S3 emergency exceptions require an approved procedure. Separate Owner-controlled Q3 and Owner-reserved S3 paths exist. The external brief's blanket prediction of escalation to A3/L3 is unsupported. Before consideration of pilot authority, tabletop the current pause and escalation outcome and replay against a hypothetical procedure with defined scope, triggers, expiry, notice, review and escalation under OD-01–04, OD-14 and revised SR-3/SR-6. The register already records OD-01 design tabletop work. Actual timing enforcement remains a separate validation.
2. **L2 approver — confirmed ambiguity, decision under OD-07.** Charter §5.1 and the register's Drafting observations preserve “separate approval” for L2 and explicitly name Owner approval or authorization for Q2, S2 and R2. OD-06 already requires satisfying each applicable authority and sending materially uncertain classifications to the Owner. Keep the L2-only approver as an explicit Owner question before changing the charter. Tabletop both L2-only and a correction that also changes an active restriction.
3. **OD-18 recovery — atomic rotation already approved.** OD-18 groups old-key revocation, replacement enrollment, pending-approval invalidation and recovery-code rotation in one commit. Active freeze persists. Unfreeze requires both current keys after acknowledgment of the current code. Retain tests for interruption before and after commit, unsuccessful code delivery or acknowledgment, and total credential loss during a freeze. Total loss, broader channels, production implementation and ordinary work after an integrity alarm remain open. Preserve Android and desktop parity. The external cooling-off proposal has no approved duration or identity proof, and emergency timing rules do not establish a recovery waiting period.
4. **Independent review — fallback already approved.** OD-04, OD-05 and revised SR-5 require an eligible reviewer and independent evidence. If unavailable, escalate to the Owner and leave review pending. Mark a missed deadline overdue. Neither pending nor overdue status renews emergency authority or authorizes release. The external brief establishes no 100% escalation rate. Under OD-10, evaluate deterministic checks as evidence and an optional read-only reviewer as a candidate subject to Owner designation, independence, protected access and independent verification of actual state.
5. **O-007 chronicle and sensitive payloads — design risk.** D-022 requires append-only history and OD-09 requires scoped evidence, limited access, Owner-controlled recovery and preservation during open cases. The cited baseline supports references and redacted copies where sufficient. Treat secret exclusion before append, including metadata and references, as a candidate acceptance requirement. Evaluate access-controlled payload references and authorized disposal under O-004/O-007/OD-10 while preserving audit integrity and evidence holds. Encryption or key destruction cannot retract plaintext already written or copied. The brief describes a hypothetical exposure.
6. **Decision-status drift — confirmed in roadmap and handoff.** ROADMAP.md line 40 and docs/SESSION_HANDOFF.md line 28 use broad pending language. The handoff also says the seven shared rules should not be treated as policy, although the register records revised adoption of all seven. README.md already links the register and accurately states the runtime pause. The register lists eight items with open work. Six remain open (OD-07, OD-11–14, OD-17); two have approved requirements and open work (OD-10, OD-18). Ten have recorded decisions and are outside the open-items table (OD-01–06, OD-08, OD-09, OD-15, OD-16). Several still depend on open implementation or procedural work.

## Retention and next decision

This project-scoped audit is linked from the session handoff. The consistency register remains the operational decision-status reference. The L2 wording question stays under OD-07 for an Owner decision. The review of the pinned baseline used read-only repository access.

## Pinned sources

- [Administrator Charter](https://github.com/GenX-Shinobi/CHIMERA/blob/a5daab11115617b493cedbe3a2860169c569fe8a/docs/ADMINISTRATOR_CHARTER.md)
- [Consistency Register](https://github.com/GenX-Shinobi/CHIMERA/blob/a5daab11115617b493cedbe3a2860169c569fe8a/docs/CONSISTENCY_REGISTER.md)
- [Decision Register](https://github.com/GenX-Shinobi/CHIMERA/blob/a5daab11115617b493cedbe3a2860169c569fe8a/docs/DECISIONS.md)
- [Memory Architecture](https://github.com/GenX-Shinobi/CHIMERA/blob/a5daab11115617b493cedbe3a2860169c569fe8a/docs/MEMORY_ARCHITECTURE.md)
- [Roadmap](https://github.com/GenX-Shinobi/CHIMERA/blob/a5daab11115617b493cedbe3a2860169c569fe8a/ROADMAP.md)
- [Session Handoff](https://github.com/GenX-Shinobi/CHIMERA/blob/a5daab11115617b493cedbe3a2860169c569fe8a/docs/SESSION_HANDOFF.md)
- [README](https://github.com/GenX-Shinobi/CHIMERA/blob/a5daab11115617b493cedbe3a2860169c569fe8a/README.md)
