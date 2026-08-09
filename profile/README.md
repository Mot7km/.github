<div align="center">

<img width="220" height="220" alt="Mot7km logo" src="https://github.com/user-attachments/assets/cbee268c-51f3-465c-975b-c0b72b018218" />

# Mot7km <sub>متحكم</sub>

### Smart Restaurant Control

**Take control of your business — anywhere.**

Mot7km is a multi-sided SaaS platform for restaurants, cafés, and F&B businesses: a **web dashboard** for owners, **mobile & desktop apps** for staff, and a **QR-based digital menu** for customers — all connected in one system.

[![Status](https://img.shields.io/badge/status-in%20development-orange)]()
[![Stack](https://img.shields.io/badge/backend-ASP.NET%20Core-512BD4)]()
[![Stack](https://img.shields.io/badge/mobile-Flutter-02569B)]()
[![Stack](https://img.shields.io/badge/web-Next.js-black)]()
[![License](https://img.shields.io/badge/license-Proprietary-lightgrey)]()

[Overview](#overview) • [Why Mot7km](#why-mot7km) • [What It Does](#what-it-does) • [Who It's For](#who-its-for) • [Architecture](#architecture) • [Roadmap](#roadmap) • [Team](#team)

</div>

---

## Overview

Most small and mid-sized F&B businesses run on a patchwork of tools — a POS here, a spreadsheet there, a paper logbook for staff attendance, and no real visibility into what's actually happening across branches. Owners end up managing their business by chasing information instead of making decisions with it.

**Mot7km replaces that patchwork with one connected system**, built around a simple principle:

> **Web = Thinking & Control.**  Business owners plan, configure, and analyze from a full-featured web dashboard.
> **Mobile = Execution & Speed.**  Managers and staff act fast from lightweight mobile apps.
> **Desktop = Reliability & Operations.**  Cashiers get a fast, offline-resilient POS built for the floor.

## Why Mot7km

- 🎯 **One source of truth** — menu, products, branches, staff, and analytics, in one place instead of five.
- ⚡ **Built for daily use, not just setup** — mobile tools are designed for speed, not dashboard parity.
- 🧱 **Grows with the business** — starts as a smart QR menu, scales up to full ordering, POS, staff ops, and finance.
- 🔐 **Role-based by design** — owners, managers, cashiers, and workers each get exactly the access they need.
- 🌍 **Bilingual-first** — built with Arabic and English typography and layout in mind from day one.

## What It Does

| Module | Description |
|---|---|
| 📋 **Smart QR Menu** | No-install, branded digital menu customers reach by scanning a code — products, images, ingredients, availability, and reviews. |
| 🛒 **Ordering & POS** *(v1+)* | QR ordering with cart, cashier POS, manual payments, receipts, and shift management. |
| 👥 **Staff Operations** *(v1.5+)* | Attendance via internal QR, shift scheduling, salary/bonus/penalty tracking, task assignment. |
| 📊 **Analytics & Reports** | Menu views, product performance, ratings, sales, and branch comparisons. |
| 🏢 **Multi-Branch Management** | Branch-level menus, staff, and reporting under one business account. |
| 🛠️ **SuperAdmin Layer** | Platform-level control: tenants, subscription plans, support, and marketing site content. |

## Who It's For

Built for small and medium operational F&B businesses, including:

- Cafés
- Restaurants
- Juice shops
- Ice cream stores
- Similar service-based businesses

## Architecture

```
Customer QR Menu (Next.js, no install)
        │
        ▼
┌─────────────────────────────┐
│   ASP.NET Core (source of   │   Node.js / NestJS
│   truth: tenants, users,    │   (engagement layer:
│   branches, products,       │◄──reviews, notifications,
│   subscriptions, reports)   │   logs)
└─────────────────────────────┘
        │
        ▼
Web Dashboard (React/Next.js) · Mobile Apps (Flutter) · Desktop POS (Flutter)
```

**Backend:** ASP.NET Core · PostgreSQL · Entity Framework Core · JWT/Refresh Tokens · SignalR
**Engagement service:** Node.js / NestJS
**Web:** React · Next.js · TypeScript · Tailwind CSS
**Mobile & Desktop:** Flutter · Cairo (Arabic) / Inter (English) typography

## Roadmap

- [x] **v0 — Smart QR Menu Starter**: browse-only digital menu, product management, admin mobile app, owner web dashboard
- [ ] **v1 — Ordering + POS MVP**: QR ordering with cart, Flutter Desktop POS, manual payments, receipts, shift management
- [ ] **v1.5 — Staff Operations**: manager & worker mobile apps, attendance, scheduling, salary calculation
- [ ] **v2 — Business Operations Pro**: expenses, revenue reports, inventory lite, advanced reporting
- [ ] **v3 — Platform Growth**: subscription automation, payment gateway, landing page CMS, support ticketing

## Team

Built by:

- **Ibrahim Nasser**
- **Amr Atef**
- **Ahmed El-Shazly**

---

<div align="center">

**Mot7km** — Built for businesses that need control.

</div>
