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
| 14-15 | Device management (list, add device dialog, device counter) | Read at full size. Device endpoints already in whats360-api-docs. Pages show real device numbers, not reproduced. |
| 16 | Professional embedding | Read at full size, matches whats360-crm-integrations/professional-embedding.md (token masked on page, not reproduced). |
| 17 | Email plans | Read at full size earlier. Prices not published. |
| 18 | Email Send API | Read at full size. Required fields corrected in whats360-email-api (body not marked required). |
| 19-26 | Email templates, bots, campaigns, mailing lists, mailboxes | Read at full size. See whats360-email-api/dashboard-email-features.md. Pages show real list names, counts and addresses, not reproduced. |
| 27-28 | DKIM domains, email dashboard | Read at full size (p28 cut off on the right in the export). Pages show real domains and DKIM data, not reproduced. Dashboard features, not documented as API. |
| 29-32 | SMS gateway and campaign dialog | p31-32 also read at full size (empty states). p29-30 read at full size, summarised in whats360-crm-integrations/sms-gateway-dashboard.md. No SMS API seen on those pages. |
| 33-35 | VCash guide and developer portal | Documented in whats360-vcash-api |
| 36-39 | Reports and transactions | Dashboard only. Contains financial data, not reproduced. Not read for documentation. |
| 41 | vCash USSD orders | Read at full size. Dashboard form: device, USSD code, SIM 1 or SIM 2, run button, four quick codes and an order log with a pending status. No API shown. Result retrieval is not documented. |
| 42-43 | vCash SMS list | Read at full size. A send form (device, recipient, text, SIM) and a filtered list. List content is private message data, not reproduced. |
| 44-45 | vCash dashboard and main dashboard | Read at full size. Summary cards, quick actions, plan usage and charts. Shows private numbers, not reproduced. |
| 46 | My services | Read at full size. Five service cards (WhatsApp, SMS service, e-wallets, email, professional embedding) and a "customize your services" box. Dashboard only. |
| 47 | CRM settings, conversation statuses | Read at full size. Summarised in whats360-crm-integrations/crm-settings-dashboard.md. |
| 48-64 | CRM settings, dashboard, notes, contacts, staff | Dashboard only. See whats360-crm-integrations for the CRM PDFs. |
| 65 | Persona editor | Read at full size and matched to persona-ai-assistant.md. |
| 66-71 | Persona editor states | p66-71 read at full size. Same form as p65 with sample entries (health adviser, customer service, sales representative) and the empty list and template cards on p70-71. Field names match persona-ai-assistant.md. No persona API shown. |
| 72-77 | Conversation bot templates, quick setup, new bot form | Read at full size. Summarised in whats360-crm-integrations/bots-dashboard.md. No bot API or webhook payload shown. |
| 40 | vCash USSD campaigns form | Read at full size. Dashboard form with a masked PIN, not reproduced. No API shown. |
| 78 | Empty conversation bot list | Read at full size, empty state. |
| 35 | vCash message patterns form | Read at full size. Summarised in whats360-vcash-api/README.md. |
| 79-80 | CRM auto-status rules | Partly read at full size. See bots-dashboard.md. |
| 81-88 | Bot dialogs (AI bot tabs, simple bot) | Read at full size. Dashboard fields summarised in whats360-crm-integrations/bots-dashboard.md. No bot API seen on these pages. |
| 89-90 | Templates gallery | Not read in detail. |
| 91-104 | Queues, chat view, appearance, support, billing | Dashboard only. Contains private data, not reproduced. |
