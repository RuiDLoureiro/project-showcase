# Agenda AI

**Status: in development.** A Flutter calendar and task planner exploring AI-assisted scheduling.

## Purpose
Bring tasks, routines and calendar planning into one interface, with AI assistance for scheduling requests.

## Documented implementation
- Calendar and task interface built with Flutter and Dart.
- On-device persistence, task groups, routine onboarding and reminders.
- Read-only device-calendar import on Android and an EventKit bridge for iOS.
- Firebase Authentication and Firestore synchronization described in the implementation documentation.
- Collaborative groups with expiring invitation links and shared task updates.

## Engineering decisions
Private calendar synchronization coalesces local changes and checks metadata before downloading item documents. Shared groups use separate real-time listeners. Provider credentials belong on the backend for distributed builds.

## Limits
The checked-in documentation describes calendar import as unavailable on web and desktop. Store release, production synchronization and current provider deployment have not been independently verified for this showcase. The product direction uses Gemini through a backend; the available repository documentation still references an earlier provider integration, so this showcase does not present the migration as complete.

See the [development log](CHANGELOG.md). Source code remains private.
