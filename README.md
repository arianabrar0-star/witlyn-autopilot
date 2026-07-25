# Witlyn Autopilot

An AI-powered revenue operating system that captures, qualifies, and books inbound leads automatically for high-value service businesses.

## Overview

Witlyn Autopilot is an AI-powered revenue operating system designed for high-value service businesses.

The system automates the complete inbound lead lifecycle—from the moment a prospect submits a form, calls the business, or sends a WhatsApp message until the lead is qualified, booked, scored, and synchronized with the CRM.

The platform combines AI voice reception, LLM-powered qualification, workflow automation, calendar scheduling, CRM synchronization, and real-time notifications into a single production workflow.

The primary objective is to reduce response time, eliminate manual lead handling, and improve operational efficiency through end-to-end AI automation.

## Problem

Service businesses frequently lose qualified leads because their inbound sales process depends on manual intervention.

Common operational challenges include:

- Slow response to website forms and inbound calls
- Missed after-hours and weekend inquiries
- Manual lead qualification by sales staff
- Inconsistent follow-up across communication channels
- Manual CRM updates and fragmented customer data
- Delayed appointment scheduling

These operational bottlenecks increase response time, reduce conversion rates, and create unnecessary administrative work for sales teams.


## Solution

Witlyn Autopilot automates the complete inbound lead lifecycle through an event-driven workflow.

The platform receives inbound requests from multiple communication channels, processes customer interactions using Large Language Models (LLMs), qualifies prospects based on configurable business rules, schedules appointments automatically, synchronizes customer data with CRM systems, and notifies sales teams in real time.

The system is designed as a modular architecture where each component performs a dedicated responsibility while remaining loosely coupled through APIs and workflow automation.

## System Workflow

```text
Website Form
      │
      │
Phone Call
      │
      │
WhatsApp
      │
      │
Email
      │
      ▼
Inbound Trigger
      │
      ▼
Retell AI Voice Receptionist
      │
      ▼
n8n Workflow Engine
      │
      ▼
Claude Sonnet 4
      │
      ▼
Lead Qualification
      │
      ▼
Appointment Booking
      │
      ▼
Custom CRM
      │
      ▼
Supabase Database
      │
      ▼
Sales Team Notification
```

##System Architecture Diagram

                Website Form
                      │
Phone ────────────────┤
                      │
WhatsApp ─────────────┤
                      │
Email ────────────────┘
                      │
                      ▼
             Inbound Gateway
                      │
                      ▼
               Node.js Backend
                      │
        ┌─────────────┴─────────────┐
        │                           │
        ▼                           ▼
    Retell AI                 Claude Sonnet 4
        │                           │
        └─────────────┬─────────────┘
                      ▼
               n8n Workflow Engine
                      │
        ┌─────────────┼─────────────┐
        ▼             ▼             ▼
   Appointment     Custom CRM   Notifications
      Booking
                      │
                      ▼
                 Supabase DB

## Key Features

- Multi-channel inbound lead capture (Website, Voice, WhatsApp, Email)
- AI-powered lead qualification using Claude Sonnet 4
- Automated workflow orchestration with n8n
- AI voice receptionist using Retell AI
- Automatic appointment scheduling
- Custom CRM synchronization
- Real-time lead scoring and routing
- Centralized customer data storage with Supabase
- Docker-based deployment architecture
- Modular and event-driven system design

## Technology Stack

### Backend

- Node.js

### Artificial Intelligence

- Claude Sonnet 4

### Workflow Automation

- n8n

### Voice AI

- Retell AI

### Database

- Supabase

### Deployment

- Docker

### Communication

- WhatsApp
- Voice
- Email
- Website Forms

### CRM

- Custom CRM

## Project Structure

```text
witlyn-autopilot/
│
├── README.md
│
├── backend/
│   └── Documentation for backend architecture
│
├── docs/
│   ├── Architecture
│   ├── API Overview
│   ├── Deployment Guide
│   └── Design Decisions
│
├── workflows/
│   └── n8n workflow documentation
│
├── prompts/
│   └── Example AI prompts
│
├── screenshots/
│   └── Architecture and workflow screenshots
│
└── demo/
    └── Demo documentation
```

## API Integrations

The system integrates multiple external services to automate the inbound sales process.

| Service | Purpose |
|----------|---------|
| Claude API | Lead qualification and conversational reasoning |
| Retell AI | AI voice receptionist |
| WhatsApp API | Customer communication |
| Supabase | Database and data persistence |
| Custom CRM API | Customer and lead management |
| Calendar API | Appointment scheduling |

## Screenshots

The following screenshots will be added:

- System Architecture
- End-to-End Workflow
- n8n Automation Flow
- CRM Dashboard
- Lead Qualification Flow
- Appointment Booking Flow

## Demo

A complete walkthrough of the system will be available soon.

The demo will showcase:

- Inbound lead capture
- AI voice interaction
- Lead qualification
- Appointment booking
- CRM synchronization
- Notification workflow

## Future Improvements

- Multi-language AI conversations
- Multi-tenant architecture
- Role-based access control
- Analytics dashboard
- Human handoff capability
- Knowledge Base (RAG)
- SMS integration
- Email automation
- Conversation history dashboard
- Kubernetes deployment

## License

This repository is published for portfolio and educational purposes.

The implementation details, architecture, and documentation are shared to demonstrate engineering capabilities.

Commercial use, redistribution, or reproduction of the proprietary Witlyn Autopilot platform is not permitted without written permission from the author.

© 2026 MD Nazmus Sakib
