# AI SOP Execution Engine

An AI-powered workflow automation system that executes a company's Standard Operating Procedures (SOPs) after a new client is signed.

Instead of manually coordinating multiple departments, a single event starts an automated workflow that validates client information, checks for duplicate records, generates an AI-powered operational summary, and prepares the client for onboarding.

---

## Project Overview

This project simulates how a business can automate its client onboarding process using n8n.

The workflow begins when a new client enters the system. Before any department starts working, the workflow validates the client's information, generates a unique client ID, checks whether the client already exists, and uses Google Gemini to create an operational assessment.

The long-term goal is to expand this workflow into a complete onboarding engine that coordinates Sales, Operations, Finance, IT, Notifications, and Reporting from a single trigger.

---

## Current Features

- Receive new client data through a webhook
- Normalize incoming client information
- Validate required fields
- Generate unique client IDs
- Detect duplicate clients using Airtable
- Generate AI-powered client summaries with Google Gemini
- Return structured responses for duplicate records

---

## Planned Features

- Client routing based on client type
- CRM automation
- Project creation
- Finance and billing setup
- IT workspace provisioning
- Email and notification automation
- Audit logging
- Reporting dashboard
- Error handling and retry logic

---

## Workflow Overview

Current workflow:

```
Receive New Client
        │
        ▼
Normalize Client Data
        │
        ▼
Required Fields Validation
        │
        ▼
Generate Client ID
        │
        ▼
Search Existing Client
        │
        ▼
Duplicate Client?
   ├──────────────► Duplicate Response
   │
   ▼
AI Client Summary
```

---

## Tech Stack

| Component | Technology |
|----------|------------|
| Workflow Automation | n8n |
| Database | Airtable |
| AI | Google Gemini |
| Trigger | Webhook |
| Version Control | GitHub |

---

## Repository Structure

```
docs/
    architecture.md
    workflow-breakdown.md
    airtable-schema.md
    setup-guide.md
    screenshots/

workflow/
    ai-sop-execution-engine-v1.json
```

---

## Documentation

Additional documentation is available inside the `docs` folder.

- Architecture
- Workflow Breakdown
- Airtable Schema
- Setup Guide

---

## Current Progress

The foundation of the workflow has been completed.

Completed modules:

- Webhook Trigger
- Data Normalization
- Required Field Validation
- Client ID Generation
- Duplicate Detection
- AI Client Summary

The next phase focuses on department-specific automation for Sales, Operations, Finance, IT, Notifications, and Reporting.

---

## Purpose

I built this project to strengthen my skills in workflow automation and operations. Instead of creating isolated automations, I wanted to design a workflow that reflects how different business functions can work together through a single automated process.

The project is still being developed, and additional modules will be added over time as the workflow grows.
