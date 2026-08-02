# JetZero

JetZero is a Long Beach, California aerospace company founded in 2021 by Tom O'Leary and Mark Page to bring the blended wing body (all-wing) airframe to commercial aviation. Its flagship program is the Z4, a 250-seat international-range jetliner the company says will burn up to 50% less fuel than comparable tube-and-wing airliners, plus the Jet1 full-scale demonstrator being built with Scaled Composites in Mojave, California ahead of a first flight targeted for 2027.

- Website: https://www.jetzero.aero/
- Newsroom: https://www.jetzero.aero/newsroom
- Careers: https://job-boards.greenhouse.io/jetzero
- Secondary-market listing (harvest source): https://forgeglobal.com/jetzero_stock/

## API surface

**None.** JetZero is an aircraft manufacturer, not a software or data provider. As of 2026-08-01 the enrichment pipeline found no public API, developer portal, API documentation, SDK, OpenAPI/GraphQL/AsyncAPI contract, MCP server, or A2A agent card.

Contract discovery probed, and missed, all of:

- `/openapi.json`, `/openapi.yaml`, `/swagger.json`, `/api-docs` on both `jetzero.aero` and `www.jetzero.aero` — all 404.
- `/.well-known/security.txt`, `/openid-configuration`, `/oauth-authorization-server`, `/api-catalog`, `/ai-plugin.json`, `/agent-card.json`, `/agent.json` — all 404 (recorded in `well-known/jetzero-well-known.yml`).
- `/llms.txt` — 404.
- DNS for `api.`, `app.`, `portal.`, `status.`, `my.`, `supplier.`, `suppliers.`, `data.`, `dev.`, `developers.`, `graphql.`, `mcp.`, `partners.` — none resolve.

No `/.well-known/security.txt`, vulnerability disclosure policy, bug bounty, or trust center was found either.

## Artifacts

| Path | Type | Method |
|---|---|---|
| `security/jetzero-domain-security.yml` | DomainSecurity | probed |
| `well-known/jetzero-well-known.yml` | (negative result — no pointer wired) | probed |
| `llms/jetzero-llms.txt` | LLMsTxt | generated |
