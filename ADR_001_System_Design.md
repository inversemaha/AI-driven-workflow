# ADR-001: System Architecture Decision

## Status
Accepted

## Context

The system needs to:
- Collect job data
- Run AI scoring
- Trigger email automation
- Track applications

Scalability and modularity are required for future SaaS expansion.

---

## Decision

Adopt modular service-based architecture:

- FastAPI backend
- React frontend
- PostgreSQL for persistence
- Redis for background jobs
- APScheduler (Phase 1)
- Celery (Future scaling)

AI scoring will be stateless and versioned.

---

## Consequences

Positive:
- Scalable
- Maintainable
- Replaceable AI provider
- SaaS-ready

Negative:
- Slightly higher initial complexity
