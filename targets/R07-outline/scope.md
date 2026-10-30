# R07 Scope

## Target

- Outline v1.12.0 (pinned tag)
- Local Docker: Postgres, Redis, MailHog, Outline
- Synthetic accounts and dummy documents only

## In scope

- Personal document access isolation
- Collection/document permission boundaries
- API key scope enforcement
- API vs MCP authorization consistency
- Attachments, revisions, search index, sharing
- Permission revocation and stale token/session behavior
- Regression checks for public Outline advisories

## Out of scope

- Public instances
- Real third-party OAuth providers
- Destructive database operations
- Denial of service, brute force, or mass enumeration
