# Backend and Cloud Architecture

## Related Documents

- [TypeScript Interfaces and JSON Schemas](../05_ENGINEERING/typescript-interfaces-and-json-schemas.md)
- [Developer Playbook](../05_ENGINEERING/developer-playbook.md)
- [Testing and Quality Assurance Manual](../07_QA/testing-and-quality-assurance-manual.md)

## Migrated Content

## Math Adventure 15 – Backend & Cloud Architecture

Version 1.0 Production Infrastructure Blueprint

## Purpose

This document defines the future production architecture for Math Adventure once the application evolves beyond a local-first family app. It specifies cloud services, authentication, AI infrastructure, synchronization, security, monitoring, and deployment principles.

## 1. Architectural Goals

- Maintain an offline-first experience while enabling cloud backup.

- Synchronize progress across multiple devices.

- Protect child privacy and parent data.

- Scale to thousands of families without changing the application architecture.

- Keep AI services isolated behind secure server-side endpoints.

## 2. Recommended Production Stack

| Layer | Recommended | Purpose |
| --- | --- | --- |
| Frontend | React + Vite PWA | Installable cross-platform application |
| Hosting | Vercel | Fast deployments and edge delivery |
| Backend | Serverless Functions | Business logic and AI gateway |
| Database | Supabase PostgreSQL | Profiles, progress and reporting |
| Authentication | Supabase Auth | Secure parent accounts |
| Storage | Supabase Storage | Worksheet uploads and assets |
| AI | OpenAI via server-side API | Tutor explanations and study plans |
| Monitoring | Sentry + Analytics | Error tracking and performance |

## 3. Authentication Model

- Parent owns the account.

- Children do not require email addresses.

- Multiple child profiles belong to one family workspace.

- Role-based permissions support additional caregivers in future versions.

## 4. Cloud Synchronization

- Local changes are queued while offline.

- Automatic synchronization when connectivity returns.

- Conflict resolution uses latest timestamp for non-critical fields.

- Learning history is never silently discarded.

## 5. AI Service Layer

- Frontend never communicates directly with the LLM.

- Server validates every request.

- Curriculum metadata accompanies every tutoring request.

- Responses are logged only when parents opt in.

- Fallback to local Tutor Mode if AI is unavailable.

## 6. Database Domains

- Families

- Child Profiles

- Learning Profiles

- Mission History

- Rewards & Purchases

- Badges

- Calendar

- Adventure Progress

- AI Usage Logs (optional)

- Audit Events

## 7. API Endpoints

- POST /missions/generate

- POST /tutor/explain

- POST /worksheet/analyze

- GET /reports/weekly

- POST /sync

- POST /rewards/request

- POST /rewards/approve

## 8. Security

- No API keys stored in the client.

- HTTPS only.

- Encrypted authentication tokens.

- Input validation on every endpoint.

- Rate limiting for AI endpoints.

- Parent-only access to sensitive information.

## 9. Privacy

- Collect the minimum personal data required.

- Parents can export or delete family data.

- No advertising.

- No sale of personal information.

- Children are never publicly searchable.

## 10. Monitoring & Reliability

- Application error logging.

- API latency monitoring.

- Database health checks.

- AI request success rates.

- Scheduled backups.

- Disaster recovery procedures.

## 11. Deployment Pipeline

- Feature branch development.

- Pull request review.

- Automated build validation.

- Preview deployment.

- Merge to main.

- Production deployment.

- Post-release monitoring.

## 12. Future Expansion

- Teacher accounts.

- Classroom mode.

- International curricula.

- Reading, Science and Financial Literacy modules.

- Voice tutoring.

- Real-time collaborative family challenges.

## Acceptance Criteria

- Architecture supports both local-first and cloud-enabled operation.

- AI remains secure behind backend services.

- Child data is protected by design.

- Infrastructure can scale without major architectural changes.
