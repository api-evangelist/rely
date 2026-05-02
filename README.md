# Rely.io

Rely.io is an internal developer portal that aggregates engineering data, provides software catalogs with blueprints and entities, engineering scorecards, self-service developer actions, and workflow automation for platform engineering teams. The platform integrates with CI/CD pipelines, incident management, observability tools, and cloud providers to create a centralized service catalog with real-time data.

The Rely.io Public REST API provides full CRUD access to blueprints, entities, scorecards, self-service actions, and automations using Bearer token authentication.

## Links

- **Website:** https://www.rely.io
- **Documentation:** https://docs.rely.io
- **Public API Docs:** https://docs.rely.io/public-api
- **Demo:** https://demo.rely.io
- **GitHub:** https://github.com/Rely-io

## APIs

### Public API
- **Base URL:** https://api.rely.io
- **Authentication:** Bearer token (API key from Plugins settings, valid 10 years)
- **Documentation:** https://docs.rely.io/public-api
- **OpenAPI:** [openapi/rely-openapi.yml](openapi/rely-openapi.yml)

**Endpoint Groups:**
- Blueprints — CRUD for entity type schemas
- Entities — CRUD for catalog instances (services, teams, deployments)
- Scorecards — CRUD for engineering standard evaluations
- Self-Service Actions — CRUD for developer workflow automation
- Automations — CRUD for catalog event-driven rules
- Users — User invitation management

## Authentication

```
Authorization: Bearer {your_api_key}
```

Generate API key in Rely.io: Settings → Plugins → Generate Token

## Integrations

GitHub, GitLab, PagerDuty, Datadog, AWS, Kubernetes, and 50+ more via the Galaxy plugin framework.

## Artifacts

| Type | File |
|---|---|
| OpenAPI | [openapi/rely-openapi.yml](openapi/rely-openapi.yml) |
| JSON Schema (Blueprint) | [json-schema/rely-blueprint-schema.json](json-schema/rely-blueprint-schema.json) |
| JSON Schema (Entity) | [json-schema/rely-entity-schema.json](json-schema/rely-entity-schema.json) |
| JSON Structure | [json-structure/rely-blueprint-structure.json](json-structure/rely-blueprint-structure.json) |
| JSON-LD Context | [json-ld/rely-context.jsonld](json-ld/rely-context.jsonld) |
| Spectral Rules | [rules/rely-rules.yml](rules/rely-rules.yml) |
| Vocabulary | [vocabulary/rely-vocabulary.yml](vocabulary/rely-vocabulary.yml) |

## Capabilities

| Capability | Description |
|---|---|
| [platform-engineering.yaml](capabilities/platform-engineering.yaml) | Full platform engineering portal workflow |
| [shared/rely.yaml](capabilities/shared/rely.yaml) | Rely.io Public API shared definition |

## Examples

- [List Blueprints](examples/rely-list-blueprints-example.json)
- [Create Entity](examples/rely-create-entity-example.json)
