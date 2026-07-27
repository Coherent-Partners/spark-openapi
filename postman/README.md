# Coherent Spark — Postman Collection

Opinionated Postman collection and environment for exploring Coherent Spark APIs. Use it as a practical starting point for common workflows — not as a complete mirror of the [User Guide](https://docs.coherent.global/spark-apis/getting-started).

> **This collection is opinionated.** Request shapes, examples, folder layout, and which endpoints are included reflect curated usage patterns. They do **not** match the documented APIs in the User Guide 100%. Prefer the User Guide (and the OpenAPI specs in this repo) as the source of truth for the full surface area.

## What's covered

| Area | Highlights |
| --- | --- |
| **Auth / Keycloak** | Client-credentials token, Spark config |
| **Folders** | Create, update, find, delete; categories |
| **Services** | Upload → compile → publish; schema, download, swagger, recompile, search |
| **Execute** | APIv3 and APIv4 locators, metadata options, common usecases |
| **Metadata / WASM / Validation** | Lookup by folder/service, service id, or version id |
| **API Call History** | Call detail, Excel rehydration, CSV/JSON log download jobs |
| **Transforms** | JSONata and Node transforms; upload, validate, list, get, delete |
| **ImpEx** | Export/import jobs (start, status, cancel/describe) |
| **Batch** | Pipeline flow (start → chunks → status → results → close/cancel) |

Also includes a smaller **Public APIs** set (metadata, WASM, validation, execute, health) useful for unauthenticated or lightly authenticated exploration.

## Getting started

1. Import `coherent-spark.postman_collection.json` and `coherent-spark.postman_environment.json` into Postman.
2. Set `environment`, `tenant`, and auth (`api_key` and/or OAuth `client_id` / `client_secret` / `access_token`).
3. Fill folder/service locators (`folder`, `service`, `version`, ids as needed) for the requests you run.
