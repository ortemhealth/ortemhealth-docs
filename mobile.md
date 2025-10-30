Flutter project setup, navigation, feature flow, analytics/configuration hooks, push notification setup

# OrtemHealth Mobile Apps Documentation

## Project Structure (Flutter)

- `lib/screens/` — Patient & Doctor app screens
- `lib/widgets/` — Custom reusable components (cards, buttons, badges)
- `lib/services/` — API handlers, auth, notifications
- `lib/models/` — Data classes (appointments, profiles, prescriptions)
- `assets/` — Lottie animations, images, localization files

## Features

**Patient App:**  
- Onboarding (Lottie, multilingual)
- Login/Register with secure storage
- Book appointments (doctor search, calendar)
- AI symptom triage bot
- Health records & prescriptions
- Telemedicine (video call via Twilio/Agora API)
- In-app notifications, push alerts

**Doctor App:**  
- Onboarding (doctor animations, branded)
- Dashboard (appointments, analytics, earnings)
- Patient search and profile view
- Day schedule, appointment details
- Write e-prescriptions, save/share
- Telemedicine video consult
- Earnings dashboard and reporting
- Profile management

## UI/UX

- Material & Cupertino themes with custom colors
- Lottie onboarding, avatar animations
- Responsive design for phone/tablet
- Accessibility & internationalization (assets/localization)

## Integration

- REST API calls via `http` and custom services to backend microservices
- Secure token storage (`flutter_secure_storage`)
- Push notifications via Firebase Messaging
- Deep links for telemedicine invites

## Testing

- Use `flutter_test` for widget/unit tests
- Manual test scripts for flows (patient appointment, doctor schedule, telemedicine)

## Build & Publish

- Run `flutter pub get`
- Build debug: `flutter run`
- Generate release: `flutter build apk` or `flutter build ios`
- App store/Play Store: submit with branded assets, privacy policy, UI/UX review

