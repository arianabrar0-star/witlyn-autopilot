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

##System Architecture

            ## System Architecture

```text
                           Inbound Channels
    ┌──────────────┬──────────────┬──────────────┬──────────────┐
    │              │              │              │
 Website Form   Voice Call    WhatsApp        Email
    │              │              │              │
    └──────────────┴──────────────┴──────────────┘
                           │
                           ▼
                    Node.js Backend
                           │
                           ▼
                  n8n Workflow Engine
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
        ▼                  ▼                  ▼
 Claude Sonnet 4      Retell AI         Business Logic
        │                  │                  │
        └──────────────────┼──────────────────┘
                           │
                           ▼
                   Lead Qualification
                           │
                           ▼
                 Appointment Scheduling
                           │
            ┌──────────────┴──────────────┐
            │                             │
            ▼                             ▼
      Custom CRM                  Supabase Database
            │
            ▼
   Sales Team Notifications
```

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

## Design Principles

The system is designed around the following engineering principles:

- Event-driven workflow orchestration
- Modular service architecture
- API-first communication
- Separation of concerns
- Stateless backend services
- AI-assisted business automation
- Scalable and containerized deployment

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

## External Services

The platform integrates with multiple external services to automate the inbound lead lifecycle.

| Service | Purpose |
|----------|---------|
| Claude Sonnet 4 API | Conversational reasoning and lead qualification |
| Retell AI | AI voice receptionist |
| WhatsApp API | Customer messaging |
| Supabase | Database and persistent storage |
| Custom CRM | Lead and customer management |
| Calendar API | Appointment scheduling |

## Screenshots

The following engineering assets will be included as the project evolves.

- System Architecture Diagram
- Workflow Architecture
- n8n Workflow
- Lead Qualification Flow
- CRM Synchronization Flow
- Appointment Scheduling Flow

## Demo

A technical walkthrough will be published soon.

The demonstration will include:

- End-to-end lead processing
- AI voice conversation
- Lead qualification workflow
- Appointment scheduling
- CRM synchronization
- System architecture overview

## Future Improvements

### Platform

- Multi-tenant architecture
- Role-based access control
- Advanced analytics dashboard

### Artificial Intelligence

- Multi-language conversations
- Knowledge Base (RAG)
- Human handoff workflow

### Infrastructure

- Kubernetes deployment
- Horizontal scaling
- Centralized logging and monitoring

### Communication

- SMS integration
- Advanced email automation
- Omnichannel conversation history

## License

This repository is provided for portfolio and educational purposes only.

It demonstrates the architecture, engineering decisions, and system design of the Witlyn Autopilot platform. Proprietary implementation details, production workflows, and source code are intentionally omitted.

Commercial use, redistribution, or reproduction of this material without written permission from the author is prohibited.

© 2026 MD Nazmus Sakib. All rights reserved.

> **Engineering Portfolio Repository**
>
> This repository showcases the architecture, engineering decisions, and system design behind **Witlyn Autopilot**. Proprietary implementation details and production source code are intentionally excluded.
