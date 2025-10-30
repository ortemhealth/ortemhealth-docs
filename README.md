# OrtemHealth Platform

OrtemHealth is a next-generation healthcare SaaS solution. It empowers clinics, doctors, and patients with advanced appointment booking, telemedicine, AI triage, and secure health records—all delivered via scalable microservices, modern mobile apps, and rich analytics.

## Main Components
- **Backend:** Modular microservices on NestJS/Prisma
- **Frontend:** Admin/Clinic dashboard (React/Next.js)
- **Mobile:** Flutter apps for Patients & Doctors
- **Infrastructure:** Cloud-native IaC, CI/CD, containerization
- **AI/ML:** No-show prediction, symptom triage, risk scoring

## Quickstart
1. Clone all repositories (`backend`, `frontend`, `doctor-app`, `patient-app`, `ai-ml`, `infrastructure`)
2. Create and setup `.env` in backend and mobile (`DATABASE_URL`, JWT secrets)
3. Run migrations: `npx prisma migrate dev`
4. Start with Docker Compose or scripts provided in infra
5. Default API ports: 3000-3010, AI-ML services: 7000+
