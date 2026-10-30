# Evidence Standard

Each test record must include:

1. Target version / commit / image digest
2. Attacker identity and role
3. Resource owner and intended access
4. Entry point (UI, API, MCP, CLI)
5. Preconditions and unique marker
6. Request/response summary with secrets redacted
7. Runtime log or mock-service record
8. Read-only database state before/after
9. Positive and negative controls
10. Conclusion with classification

Classifications:

- No issue observed
- Expected behavior
- Known vulnerability regression
- Candidate requiring recheck
- Confirmed vulnerability candidate

Rules:

- Raw evidence is append-only; corrections are recorded separately.
- HTTP status alone is not evidence of impact; object state must change.
- Absence of findings on tested paths must not be generalized to the whole module.
