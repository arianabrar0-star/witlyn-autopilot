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

## API Integrations

## Screenshots

## Demo

## Future Improvements

## License
