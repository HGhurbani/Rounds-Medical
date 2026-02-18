# Rounds Medical

Rounds Medical is a Flutter-based mobile application designed to support clinical teams in day-to-day hospital workflows. The app centralizes patient follow-up, team collaboration, daily rounds, and medical record interactions in one place.

## Overview

The project provides a role-focused experience for doctors and care teams to:

- Manage and review patient information.
- Record and follow daily round activities.
- Track vital signs, labs, radiology, notes, and reports.
- Collaborate with teams and monitor assigned patients.
- Access educational, consent, and media-related clinical resources.

## Key Features

- **Authentication & account flows**
  - Login, signup, and password reset interfaces.
- **Patient management**
  - Patient lists, profiles, and detailed patient information views.
- **Daily rounds workflow**
  - Add/view daily round entries and section-based round records.
- **Clinical documentation modules**
  - Laboratories, radiology, non-radiology results, medications, reports, consents, and notes.
- **Vitals & monitoring**
  - Add and display vital signs with dedicated screens.
- **Team collaboration**
  - Team screens and doctor-to-team assignment flows.
- **Media & attachments**
  - Support for images, videos, and documents in clinical context.
- **Notifications & utilities**
  - Notification pages, sharing tools, and PDF-related utilities.

## Tech Stack

- **Framework:** Flutter (Dart)
- **Platforms:** Android, iOS, Web (project scaffolding available)
- **Backend/Services (via dependencies):**
  - Firebase (Auth, Firestore, Storage, Realtime Database)
  - REST/network integrations via `dio` and `http`
- **Other capabilities:**
  - File/image picking and cropping
  - Audio recording and speech-to-text
  - Video playback
  - Local notifications
  - PDF generation/viewing/sharing

## Project Structure

```text
lib/
├── AddScreens/                 # Create/add flows for medical records and entities
├── Screens/                    # Main application screens
├── Details/                    # Detailed views for results and records
├── UserLogin/                  # Authentication-related UI
├── Network/                    # Data models and API response models
├── Models/                     # UI model components/cards
├── BottomNavigationBarItems/   # Main navigation sections
├── Policy/                     # Terms and privacy screens
├── recording/                  # Audio/speech recording features
└── main.dart                   # App entry point
```

## Getting Started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install)
- Dart SDK (included with Flutter)
- Android Studio / Xcode (for device emulators and builds)
- Firebase project configuration (if backend features are enabled)

### Installation

1. Clone the repository:

   ```bash
   git clone <your-repo-url>
   cd Rounds-Medical
   ```

2. Install dependencies:

   ```bash
   flutter pub get
   ```

3. Run the app:

   ```bash
   flutter run
   ```

## Build Commands

```bash
# Android APK
flutter build apk

# iOS (macOS only)
flutter build ios

# Web
flutter build web
```

## Configuration Notes

- Ensure Firebase configuration files are set correctly for each target platform.
- Update application identifiers/signing config before production release.
- Review permissions for camera, microphone, storage, and notifications as required by your deployment platform.

## Contributing

Contributions are welcome. If you plan to contribute:

1. Fork the repository.
2. Create a feature branch.
3. Commit clear, focused changes.
4. Open a pull request with a concise description.

## License

This project currently does not include a license file. Add a license (e.g., MIT, Apache-2.0) before public distribution.

