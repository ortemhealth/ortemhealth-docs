React/Flutter architecture, package/dependency setup, folder structure, major components/screens/widgets
# OrtemHealth Frontend Developer Documentation

## Overview
Frontend delivers the admin/clinic dashboard (React/Next.js).  
Supports appointment management, patient intake, analytics, notification center, and settings.

## Structure
- `pages/` — All screens/routes (`/dashboard`, `/appointments`, `/patients`, etc.)
- `components/` — Shared UI widgets, forms, & buttons
- `services/` — API bindings (REST calls to backend microservices)
- `styles/` — Material UI theme extensions, branding

## Quick Start
Install packages:  
`npm install`

Run dev:  
`npm run dev`

## API Integration
Configure base API endpoint in `services/api.js`. Each function maps to backend microservice.

## Theming & UX
Material-UI configured. Update `/styles/theme.js` for brand colors and typography.

## Internationalization
Stencil for i18n and locale packs. Add/update strings in `/locales/`.

## Deployment
Build:  
`npm run build`

Production:  
`npm run start`
