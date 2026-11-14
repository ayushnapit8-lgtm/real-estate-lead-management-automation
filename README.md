# real-estate-lead-management-automation
# Real Estate Lead Management Automation

An AI-powered lead management workflow built with **n8n, Ollama, Qwen 2.5, Google Sheets, and Gmail**.

## Project Overview

This project automates the process of capturing real estate enquiries, classifying leads by buying timeline, storing lead information in a CRM spreadsheet, and generating AI-powered lead analysis.

## Workflow Architecture

**Customer Enquiry Form → Data Processing → Lead Classification → Google Sheets CRM → AI Analysis → Merge → Gmail Notification**

## Key Features

- **Automated Lead Capture:** Collect customer enquiries through an n8n form.
- **Lead Prioritization:** Classify leads as High or Normal based on buying timeline.
- **CRM Integration:** Store lead records in Google Sheets.
- **AI Lead Analysis:** Use Qwen 2.5 through Ollama to generate:
  - Lead Summary
  - Buying Intent
  - Recommended Next Action
  - Reason for the assessment
- **Email Notifications:** Send lead details and AI analysis through Gmail.

## Technology Stack

| Technology | Purpose |
|---|---|
| n8n | Workflow automation |
| Ollama | Local AI model runtime |
| Qwen 2.5 (3B) | AI lead analysis |
| Google Sheets | Lead database |
| Gmail | Email notifications |

## How It Works

1. A customer submits a property enquiry form.
2. n8n processes and organizes the submitted information.
3. An IF node classifies the lead as High or Normal priority.
4. Lead information is saved to Google Sheets.
5. The AI model analyzes the lead and recommends the next action.
6. The Merge node combines the lead information with the AI output.
7. Gmail sends an automated notification.

## Project Files

- `workflow/` — Sanitized n8n workflow export.
- `screenshots/` — Project screenshots and execution evidence.

## Setup Notes

To run this workflow, you need:

- An n8n instance
- Ollama with the `qwen2.5:3b` model
- Google Sheets OAuth credentials
- Gmail OAuth credentials

Import the workflow JSON into n8n and configure your own credentials, Google Sheet, and email settings before running it.

## Learning Outcomes

This project helped me practice workflow automation, conditional logic, API integrations, local AI model integration, data processing, and automated notifications.

## Disclaimer

This is a learning and portfolio project. The workflow export does not include working credentials. Configure and test your own integrations before using it with real customer data.
