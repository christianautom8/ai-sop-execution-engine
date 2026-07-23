# Setup Guide

## Requirements

- n8n
- Airtable Account
- Google Gemini API Key
- GitHub Account

---

## Setup Steps

1. Clone the repository.
2. Import the workflow into n8n.
3. Create the Airtable base.
4. Configure Airtable credentials.
5. Configure the Google Gemini credentials.
6. Update the webhook URL.
7. Execute the workflow.

---

## Test Payload

```json
{
  "company_name": "OpenAI",
  "contact_name": "Sam Altman",
  "email": "sam@openai.com",
  "industry": "Artificial Intelligence",
  "service": "Workflow Automation",
  "client_type": "Enterprise"
}
```
