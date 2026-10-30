# Authorized Scope

## Allowed

- Self-owned local Docker or source deployments
- Multi-account testing with synthetic users and dummy data
- Source-code review of the pinned release
- Read-only database verification
- Local mock services for third-party dependencies

## Not allowed

- Scanning or testing public instances
- Using real credentials, tokens, cookies, or personal data
- Destructive database changes or denial-of-service testing
- Modifying application source to manufacture a vulnerability
- Disabling authentication or security mechanisms to force a result
- Publishing unremediated exploit details

Every round records the version pin, image digest, environment, and test identity matrix before testing.
