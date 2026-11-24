# API index

| Service | Status | Docs | Auth (as documented) |
|---|---|---|---|
| WhatsApp messaging (text, image, video, audio, document) | Documented, 22 paths in OpenAPI draft | [whats360-api-docs](https://github.com/whats360-api/whats360-api-docs) | `token` query parameter |
| WhatsApp devices (create, connect, status, QR, delete) | Documented | same | same |
| Campaigns (bulk) | Documented, request body fields partly undocumented | same + [known gaps](https://github.com/whats360-api/whats360-api-docs/blob/main/known-gaps.md) | same |
| Email send | Documented from dashboard page | [whats360-email-api](https://github.com/whats360-api/whats360-email-api) | Bearer token from `/api/auth/login` |
| VCash (devices, SMS send, USSD execute, balance) | Documented from dashboard page | [whats360-vcash-api](https://github.com/whats360-api/whats360-vcash-api) | Bearer API token |
| Webhooks and HookURL | Guide, receivers | [whats360-webhooks](https://github.com/whats360-api/whats360-webhooks) | HookURL optional `X-Hook-Secret` header |

Base URL: `https://whats360.live`. Examples use placeholders only. The whats360.live owner states the documented endpoints work. The examples in these repositories were not run live by their author unless a repository says a test was run.
