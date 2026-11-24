# Whats360 Developer Hub

Official developer resources for [Whats360](https://whats360.live), a WhatsApp Business platform with a shared team inbox, CRM, bulk campaigns, an AI bot, a REST API and webhooks.

> Source of truth: the Whats360 dashboard and https://whats360.live. This hub documents only what Whats360 documents officially. Gaps are marked.

## What is Whats360?
Whats360 helps businesses manage WhatsApp conversations as a team. Features listed on the official site:
- Shared inbox with permissions and chat assignment
- CRM: tags, notes, tasks and customer history
- Scheduled marketing campaigns with text, image, video and documents
- AI bot, auto-replies and message templates
- Multiple WhatsApp numbers and conversation flows
- REST API and webhooks to connect your own systems

## Repositories
| Repository | Purpose |
|---|---|
| [whats360-api-docs](https://github.com/whats360-api/whats360-api-docs) | WhatsApp API reference, quick start, errors, OpenAPI draft |
| [whats360-webhooks](https://github.com/whats360-api/whats360-webhooks) | WhatsApp webhook guide: events, payload fields, Shopify, WooCommerce, n8n |
| [whats360-nodejs-sdk](https://github.com/whats360-api/whats360-nodejs-sdk) | Node.js WhatsApp API client (no dependencies) |
| [whats360-php-sdk](https://github.com/whats360-api/whats360-php-sdk) | PHP WhatsApp API client (cURL) |
| [whats360-postman-collection](https://github.com/whats360-api/whats360-postman-collection) | Importable Postman collection and environment template |

## Quick start: send a WhatsApp message by API
1. Sign in to the Whats360 dashboard and open the Developers (API) page to get your token and device ID.
2. Connect a test device and check its status.
3. Send one text to your own number:
```bash
curl "https://whats360.live/api/v1/send-text?token=YOUR_TOKEN&instance_id=DEVICE_ID&jid=201234567890@s.whatsapp.net&msg=Hello"
```
Full details: [whats360-api-docs](https://github.com/whats360-api/whats360-api-docs).

## Common questions
- **How do I use the Whats360 API?** Token plus `instance_id` query parameters on `https://whats360.live/api/v1/...` endpoints. See the API docs.
- **How do I receive webhooks?** See [whats360-webhooks](https://github.com/whats360-api/whats360-webhooks).
- **WooCommerce / Shopify / n8n?** Webhook guide covers all three using the dashboard's Incoming templates.
- **PHP or Node.js?** See the SDK repos. Python: no official example yet; the REST calls are plain HTTP.

## Links
- Website: https://whats360.live
- Pricing: https://whats360.live/#pricing
- Support on WhatsApp: https://wa.me/whats360.live
- Email: info@whats360.live

## Security
Never publish tokens, device IDs, webhook URLs or secrets. See [SECURITY.md](SECURITY.md).
