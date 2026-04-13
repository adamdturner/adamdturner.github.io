---
layout: project
title: "Grapevine App"
date: 2025-05-01 10:00:00 -0600
description: "Mobile app (Flutter): iOS and Android referral and rewards experience tied to Firebase. Website (Next.js on Vercel): grapevinecodes.com—React, TanStack Query, layered API routes, use cases, and Firestore via Admin SDK."
duration: "5 months"
role: "Contract Developer"
status: "Ongoing"
featured: true
image: "/assets/images/projects/grapevine-app.jpg"
live_url: "https://www.grapevinecodes.com"
technologies: ["Flutter", "Dart", "Next.js", "React", "TanStack Query", "Vercel", "Firebase", "Cloud Firestore", "Firebase Auth", "Firebase Admin SDK", "Cloud Functions"]
---

## Overview

Grapevine rewards people for telling friends about products they actually use. The product idea is the same across clients: when someone uses a friend’s Grapevine referral, they can move straight into checkout; on purchase, the referrer earns a reward from the vendor, who only pays when a sale happens.

### Mobile app

The **Flutter** app is the on-the-go experience for iOS and Android—referral codes, account and vendor flows, and the same Firebase-backed data model as the web client (Auth, Firestore, Cloud Functions). I focus on mobile UI, state management, and integrating with the shared backend.

### Website

The **Next.js** site is deployed on **Vercel** at **[grapevinecodes.com](https://www.grapevinecodes.com)**. It complements the app with a full web client: **React** components never touch the database directly; **TanStack Query** drives server state; a shared HTTP client (`apiFetch`) injects auth tokens into **Next.js API routes**, which act as the API boundary. **Use cases** hold validation and business rules; **repositories** are the only layer that talk to **Cloud Firestore**, using the **Firebase Admin SDK** on the server.

```
│  UI Layer (React Components)        │  ← Never touches database
├─────────────────────────────────────┤
│  Feature Hooks (TanStack Query)     │  ← State management
├─────────────────────────────────────┤
│  HTTP Client (apiFetch)             │  ← Auth token injection
├─────────────────────────────────────┤
│  API Routes (Next.js)               │  ← API boundary
├─────────────────────────────────────┤
│  Use Cases (Business Logic)         │  ← Validation & rules
├─────────────────────────────────────┤
│  Repositories (Data Access)         │  ← ONLY place with Firestore
├─────────────────────────────────────┤
│  Firestore (Database)               │  ← Firebase Admin SDK
```

## Highlights

- **Mobile:** Cross-platform iOS and Android app (Flutter)—referral flows and Firebase integration
- **Website:** [grapevinecodes.com](https://www.grapevinecodes.com) on Vercel—React, TanStack Query, Next.js API routes, layered use cases and repositories
- Authentication with Firebase Auth (email/password, OAuth-ready)
- Real-time data with Cloud Firestore; server-side access via Admin SDK in repositories
- Cloud Functions for background tasks and integrations
- Modular, scalable architecture with a strict separation between UI and data access

## Technologies

- Flutter (Dart) — mobile client
- Next.js, React, TanStack Query — web client and API surface
- Vercel — deployment for the web application
- Firebase (Auth, Firestore, Cloud Functions, Storage)
- Firebase Admin SDK — Firestore from trusted server code only
- REST/JSON APIs


