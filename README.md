# AI Client Acquisition Platform - Backend

This repository houses the core engine and REST APIs for the automated client acquisition system.It manages the entire lead lifecycle, runs real-time email verification gates, schedules automated follow-up sequences, and uses dual-model AI reasoning for conversation management and meeting scheduling.

### Key Features:
- **Lead Lifecycle & Validation:** Automatic deduplication constraints and real-time ZeroBounce email verification.
- **Automated Cold Outreach:** Multi-stage campaign orchestration and 3-step automated follow-up sequences using Celery Beat.
- **Mailgun Integration:** Inbound reply handling triggered immediately via secure webhooks.
- **Dual-Model AI Failover:** High-availability conversation handling using Groq (Llama 3) as primary with an automated fallback to the Gemini API.
- **Smart Booking System:** Deep integration with Google Calendar API to automatically fetch availability, find common free slots, and generate Google Meet links.

### Tech Stack:
- Python / Django / Django REST Framework (DRF) 
- Celery & Celery Beat (Task scheduling)
- PostgreSQL (Database layer) 
- Mailgun API, ZeroBounce API, Groq & Gemini APIs, Google Calendar API
