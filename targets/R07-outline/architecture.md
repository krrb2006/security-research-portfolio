# R07 Architecture (local lab)

- Outline application (Node.js/React) on `127.0.0.1:3000`
- PostgreSQL 18 (documents, collections, users, policies, revisions)
- Redis 7 (sessions, queues, collaboration)
- Local file storage in the `outline-data` volume
- MailHog SMTP/UI on `127.0.0.1:8025` for magic-link sign-in
- MCP endpoint served by Outline; OAuth/API-key authentication

Trust boundaries to review:

- HTTP API -> policy layer (`server/policies/`)
- MCP tools -> document/collection policy checks
- API key scopes -> endpoint authorization
- personal documents -> search, revisions, attachments, sharing
- role change / user disable / deletion -> existing tokens and sessions
