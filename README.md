<p align="center"><img src="banner.svg" alt="whats360.live API Developer Platform" width="100%"></p>

# whats360.live Developer Hub

Official developer resources for [whats360.live](https://whats360.live?utm_source=github&utm_medium=repo_readme&utm_campaign=growth30&utm_content=hub-intro), a WhatsApp Business platform with a shared team inbox, CRM, bulk campaigns, an AI bot, a REST API and webhooks.

> Source of truth: the whats360.live dashboard and https://whats360.live. This hub documents only what whats360.live documents officially. Gaps are marked.

## What is whats360.live?
whats360.live helps businesses manage WhatsApp conversations as a team. Features listed on the official site:
- Shared inbox with permissions and chat assignment
- CRM: tags, notes, tasks and customer history
- Scheduled marketing campaigns with text, image, video and documents
- AI bot, auto-replies and message templates
- Multiple WhatsApp numbers and conversation flows
- REST API and webhooks to connect your own systems

## Important notes
- whats360.live links WhatsApp numbers by QR code. It is not the Meta WhatsApp Cloud API and is not a Meta Business Solution Provider.
- No guarantee against WhatsApp account restrictions is made. Follow WhatsApp's policies and message only people who agreed to receive messages.

## Repositories
| Repository | Purpose |
|---|---|
| [whats360-api-docs](https://github.com/whats360-api/whats360-api-docs) | WhatsApp API reference, quick start, errors, OpenAPI draft |
| [whats360-webhooks](https://github.com/whats360-api/whats360-webhooks) | WhatsApp webhook guide: events, payload fields, Shopify, WooCommerce, n8n |
| [whats360-nodejs-sdk](https://github.com/whats360-api/whats360-nodejs-sdk) | Node.js WhatsApp API client (no dependencies) |
| [whats360-php-sdk](https://github.com/whats360-api/whats360-php-sdk) | PHP WhatsApp API client (cURL) |
| [whats360-developer-examples](https://github.com/whats360-api/whats360-developer-examples) | Send message, send media, bulk loop, webhook receivers (Python, Node, PHP, Laravel), error handling |
| [whats360-postman-collection](https://github.com/whats360-api/whats360-postman-collection) | Importable Postman collection and environment template |

## Quick start: send a WhatsApp message by API
1. Sign in to the whats360.live dashboard and open the Developers (API) page to get your token and device ID.
2. Connect a test device and check its status.
3. Send one text to your own number:
```bash
curl "https://whats360.live/api/v1/send-text?token=YOUR_TOKEN&instance_id=DEVICE_ID&jid=201234567890@s.whatsapp.net&msg=Hello"
```
Full details: [whats360-api-docs](https://github.com/whats360-api/whats360-api-docs).

## Common questions
- **How do I use the whats360.live API?** Token plus `instance_id` query parameters on `https://whats360.live/api/v1/...` endpoints. See the API docs.
- **How do I receive webhooks?** See [whats360-webhooks](https://github.com/whats360-api/whats360-webhooks).
- **WooCommerce / Shopify / n8n?** Webhook guide covers all three using the dashboard's Incoming templates.
- **PHP or Node.js?** See the SDK repos. Python: no official example yet; the REST calls are plain HTTP.

## Links
- Website: https://whats360.live?utm_source=github&utm_medium=repo_readme&utm_campaign=growth30&utm_content=hub-links
- Pricing: https://whats360.live/#pricing?utm_source=github&utm_medium=repo_readme&utm_campaign=growth30&utm_content=hub-pricing
- WhatsApp: https://wa.me/whats360.live · Direct chat support: https://wa.me/201030741766 · Email: info@whats360.live
- Email: info@whats360.live

## Official links
- Website: https://whats360.live
- YouTube: https://www.youtube.com/@Whats360live
- Facebook: https://www.facebook.com/whats360.live
- Instagram: https://www.instagram.com/whats360.live
- TikTok: https://www.tiktok.com/@whats360.live
- Reddit (official brand account): https://www.reddit.com/user/mhmdfares
- Product Hunt: https://www.producthunt.com/products/whats360
- WhatsApp: https://wa.me/whats360.live

## Security
Never publish tokens, device IDs, webhook URLs or secrets. See [SECURITY.md](SECURITY.md).


## More repositories
| Repository | Purpose |
|---|---|
| [whats360-email-api](https://github.com/whats360-api/whats360-email-api) | Email send API documentation and examples |
| [whats360-vcash-api](https://github.com/whats360-api/whats360-vcash-api) | VCash devices, SMS, USSD and balance documentation |
| [whats360-developer-examples](https://github.com/whats360-api/whats360-developer-examples) | Send, bulk, webhook receivers (PHP, Laravel, Express, Flask), error handling |
| [whats360-integration-examples](https://github.com/whats360-api/whats360-integration-examples) | WooCommerce, OTP, payment notification, CRM forward |

Indexes: [API_INDEX.md](API_INDEX.md) · [INTEGRATIONS_INDEX.md](INTEGRATIONS_INDEX.md) · [DOCUMENTATION_GAPS.md](DOCUMENTATION_GAPS.md) · [AI_USAGE.md](AI_USAGE.md) · [ARCHITECTURE.md](ARCHITECTURE.md)
