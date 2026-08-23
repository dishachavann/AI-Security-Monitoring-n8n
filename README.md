```text
# AI Security Monitoring & Alerting Workflow

An AI-powered security monitoring workflow built with n8n that receives
security events through a webhook, analyzes them using an AI model,
classifies the threat level, and sends an email alert.

## Architecture
Webhook
   ↓
AI Security Analysis
   ↓
IF Risk Classification
   ↓
 ┌──────────────┐
 │              │
HIGH           LOW
 │              │
 ▼              ▼
Gmail Alert   Gmail Notification

## Features

- Webhook-based security event ingestion
- AI-powered SOC analysis
- Threat/risk classification
- Automated HIGH-risk detection
- Email security alerts
- Automated security-event reporting

## Technologies Used

- n8n
- Google Gemini / AI model
- Webhooks
- Gmail API
- JSON
- AI-assisted security analysis

## Workflow

1. A security event is received through the webhook.
2. The AI model analyzes the event.
3. The event is classified according to risk level.
4. The IF node checks whether the result contains `HIGH`.
5. The appropriate Gmail notification is triggered.

📂 Files
workflow/ — n8n workflow JSON
screenshots/ — Workflow screenshot
examples/ — Sample security-event data

🔐 Security

No API keys, passwords, OAuth tokens, or other sensitive credentials should be committed to this repository.

🎯 Purpose

This project demonstrates how AI and workflow automation can assist with SOC monitoring and security alerting.

Built for educational and defensive cybersecurity purposes.

👩‍💻 Author

Disha Chavan

Cybersecurity | Network Security | Security Automation
