---
layout: project
title: "Grapevine App"
date: 2025-05-01 10:00:00 -0600
description: "Referral and rewards platform: Flutter mobile app plus a Next.js web app on Vercel, with a layered stack (React, TanStack Query, API routes, use cases, Firestore via Admin SDK)."
duration: "5 months"
role: "Contract Developer"
status: "Ongoing"
featured: true
image: "/assets/images/projects/grapevine-app.jpg"
technologies: ["Flutter", "Dart", "Next.js", "React", "TanStack Query", "Vercel", "Firebase", "Cloud Firestore", "Firebase Auth", "Firebase Admin SDK", "Cloud Functions"]
---

## Overview

Grapevine is a cross-platform product: a **Flutter** mobile application and a **Next.js** web application, both tied to the same Firebase backend. It is designed to allow users to tell their friends about products and services they buy. People are already doing this everyday, so Grapevine steps in to reward people for telling each other about the stuff they own. When someone scans their friend's Grapevine referral code, they are taken immediately to a checkout page to buy the item. Upon purchase, the one who referred the item gets a cash reward directly from the vendor. Vendors don't have to pay for advertising upfront, they only pay people when a purchase is made.

The **web app** is deployed on **Vercel**. The UI layer (React components) does not access the database directly. Feature hooks use **TanStack Query** for server state; a shared HTTP client (`apiFetch`) injects auth tokens and calls **Next.js API routes**, which enforce the API boundary. **Use cases** hold validation and business rules; **repositories** are the only layer that talk to **Cloud Firestore**, using the **Firebase Admin SDK** on the server.

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

- Cross-platform mobile app for iOS and Android (Flutter)
- Web app on Vercel: React, TanStack Query, Next.js API routes, layered use cases and repositories
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


