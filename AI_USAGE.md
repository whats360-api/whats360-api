# Guidance for AI coding agents
- Treat these repositories as documentation derived from the whats360.live dashboard. The base URL is `https://whats360.live`.
- Never invent endpoints, parameters, responses, signatures or retry rules. If it is not in the docs, check DOCUMENTATION_GAPS.md.
- Use placeholders (`YOUR_API_KEY`, `DEVICE_ID`). Never write real tokens, phone numbers or customer data into code, tests or issues.
- Do not run the VCash USSD endpoint or any send endpoint against a real account without the owner's approval.
- whats360.live links WhatsApp numbers by QR code. Do not describe it as the Meta Cloud API, a Business Solution Provider or an official Meta product. Do not promise delivery or ban protection.
- Entry points: [llms.txt](llms.txt), [API_INDEX.md](API_INDEX.md), [INTEGRATIONS_INDEX.md](INTEGRATIONS_INDEX.md).
