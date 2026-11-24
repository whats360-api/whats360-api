# Architecture of the whats360.live developer hub

```mermaid
flowchart LR
  App[Your app or store] -->|REST| API[whats360.live API\nwhats360.live/api/v1]
  API --> Dev[Connected phone\nWhatsApp / SMS / VCash]
  Store[Shopify, Salla, Zid, WooCommerce] -->|events| Hook[HookURL / Webhook]
  Hook --> Dash[whats360.live dashboard\nrules, bots, CRM]
  Dash --> Dev
  Ext[Your customer API] -->|phone lookup| Dash
```

Repositories: docs (`whats360-api-docs`), webhooks, Node.js and PHP clients, Postman, developer examples, integration examples, email API, VCash API. See [API_INDEX.md](API_INDEX.md).
