---
Title: StageCall iOS Spec Sheet (Rev2)
Description: Technical implementation and Firestore integration specs for StageCall MVP (2025-10-05).
AutoAttach: true
---

# StageCall iOS Specification Sheet – Rev2 (2025-10-05)

## 🎯 Purpose
Defines technical architecture, Firebase schema, and concurrency model for the StageCall iOS app.

## 🧩 Architecture Overview
- Pattern: MVVM + Service Layer
- Frameworks: SwiftUI, Firebase Firestore, Firebase Auth, OSLog, Network
- Language: Swift 6.2+ (Strict Concurrency Checking = Complete)

## 🔥 Firebase Integration
- Host writes: `/sessions/{id}/state/host`
- Patrons write: `/sessions/{id}/queue`
- Guardrails: 30–180s timeout

## 🧠 Authentication
- Sign in with Apple for Host/Patron
- Anonymous sign-in for Quick Play only

## 🧩 Accessibility & Privacy
- 44×44pt touch targets, VoiceOver labels
- Minimal PII, no tracking or analytics

## 🧱 Definition of Done (MVP)
- Host ↔ Patron flow operational
- Deep links functional
- Offline sync verified
- Zero warnings or runtime crashes

_End of StageCall iOS Spec Sheet — Rev2_
