# OrtemHealth Backend Developer Documentation

## Overview
Platform backend is built as scalable microservices: Auth, User, Doctor, Patient, Appointment, Notification, Payment, API Gateway, AI/ML.

## Code Structure
- `apps/` — Each microservice
- `libs/shared/` — DTOs, entities, common validators
- `prisma/` — Database ORM, migrations
- `.env` — Configurations

### Microservices
| Service             | Port | Purpose                                 |
|---------------------|------|-----------------------------------------|
| Auth               | 3001 | JWT, login, register, RBAC              |
| Appointment        | 3003 | Appointment book, list, reschedule      |
| Notification       | 3004 | Audit, deliver, retry, push/email/SMS   |
| Payment            | 3005 | Billing, payment gateway, refunds       |
| Doctor/Patient     | 3006/7| Profile, schedule, search, history      |
| AI/ML              | 7000 | Predict no-shows/triage/risk scoring    |

## API & Swagger
Each service includes Swagger docs at `/api-docs`.  
Run each service locally and view at `http://localhost:PORT/api-docs`

## Error Handling
All API error responses:
