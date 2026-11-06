# WhatsApp Appointment Automation

An n8n workflow that processes WhatsApp messages, reads appointment/customer records from Google Sheets, sends WhatsApp replies or notifications, and updates message status.

## Included workflow

- `whatsapp-business-bot-for-customer-service-automation.json` — 15-node workflow export.

## Requirements

- n8n with WhatsApp Business Cloud and Google Sheets nodes.
- A Google Sheet with the columns referenced by the workflow, plus a WhatsApp Business Cloud account and configured webhook.

## Import and configure

1. Import the JSON workflow into n8n.
2. Assign your own Google Sheets and WhatsApp credentials; exported credential bindings were removed.
3. Replace the sheet/document references and WhatsApp phone number/recipient placeholders in node settings.
4. Configure Meta’s webhook to reach the n8n trigger, review schedule/trigger settings, and test with a non-production number.

## Notes

No credentials, live phone IDs, sheet IDs, or personal message data are included. Validate the expected sheet columns and appointment behavior against your own setup before activation.

