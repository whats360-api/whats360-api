# Documentation gaps across all services
Collected from each repository. Nothing here is guessed in the repos.
- WhatsApp API: campaign recipients body, campaign create fields beyond name and message_content, per-endpoint response fields, plan rate limits.
- Webhooks: outgoing webhook signature and retry policy. HookURL link format and event payload shape.
- Email: token lifetime, attachments, cc/bcc, HTML body, rate limits.
- VCash: error format, USSD result retrieval after `pending`, SIM slot values, rate limits.
- Dashboard-only features with no documentation provided: CRM board, deals pipeline, labels, satisfaction ratings, analytics reports, SMS gateway, number warm-up, WhatsApp tools. These appear in the dashboard menu only.
- A public developer portal: https://whats360.live/developers is a login page, not public docs.
Send corrections to info@whats360.live.

## Dashboard export review (104-page PDF; page headers carry screenshot dates between 2026-05-07 and 2026-05-27)

Every page was opened at least at thumbnail size. Pages marked 'read at full size' were read closely. For all other rows, 'Dashboard only' means what was visible at thumbnail size and does not prove that no endpoint or field exists there.

| Pages | Content seen | Status |
|---|---|---|
| 1-4 | Subscriptions, plans, upgrade dialog | Dashboard only. Plan limits and prices not published. |
| 5-9 | Developer portal: send, device and campaign endpoints, access token | Documented in whats360-api-docs |
| 10-13 | Number warm-up, webhook pages | Warm-up: dashboard only. Webhooks documented in whats360-webhooks |
| 14-28 | Email plans, Email Send API, templates, bots, campaigns, lists, mailboxes, DKIM domains | Email API documented in whats360-email-api. Other pages are dashboard features, not documented as API. |
| 29-32 | SMS gateway and campaign dialog | p29-30 read at full size, summarised in whats360-crm-integrations/sms-gateway-dashboard.md. No SMS API seen on those pages. p31-32 thumbnail only. |
| 33-35 | VCash guide and developer portal | Documented in whats360-vcash-api |
| 36-47 | Reports, transactions, services, VCash SMS lists | Dashboard only. Contains private data, not reproduced. |
| 48-64 | CRM settings, dashboard, notes, contacts, staff | Dashboard only. See whats360-crm-integrations for the CRM PDFs. |
| 65 | Persona editor | Read at full size and matched to persona-ai-assistant.md. |
| 66-78 | Persona editor states | Thumbnail only. Look like the same form. Not compared field by field. |
| 79-80 | CRM auto-status rules | Partly read at full size. See bots-dashboard.md. |
| 81-88 | Bot dialogs (AI bot tabs, simple bot) | Read at full size. Dashboard fields summarised in whats360-crm-integrations/bots-dashboard.md. No bot API seen on these pages. |
| 89-90 | Templates gallery | Not read in detail. |
| 91-104 | Queues, chat view, appearance, support, billing | Dashboard only. Contains private data, not reproduced. |
