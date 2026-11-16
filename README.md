<p align="center">
  <img src="public/spica-logo.svg" alt="SpicaAnalytics Logo" width="760" />
</p>

<p align="center">
  <strong>Sovereign Privacy-First Enterprise Web &amp; Product Analytics Engine</strong><br>
  <em>Zero Cookies, Zero Tracking Banners, Real-Time Conversion Funnels, and Complete Data Sovereignty</em>
</p>

<p align="center">
  <a href="https://github.com/wtfear/SpicaAnalytics/actions/workflows/ci.yml"><img src="https://github.com/wtfear/SpicaAnalytics/actions/workflows/ci.yml/badge.svg" alt="CI Status" /></a>
  <img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT" />
  <img src="https://img.shields.io/badge/Script_Size-%3C2KB-emerald.svg" alt="<2KB Embed" />
  <img src="https://img.shields.io/badge/Stack-Next.js_+_TypeScript-black.svg" alt="Next.js + TypeScript" />
  <img src="https://img.shields.io/badge/ORM-Prisma_+_PostgreSQL-indigo.svg" alt="Prisma + PostgreSQL" />
  <img src="https://img.shields.io/badge/Constellation-Virgo_%CE%B1-cyan.svg" alt="Virgo Alpha Star" />
</p>

---

## 🌟 Executive Overview

**SpicaAnalytics** is an institutional-grade, self-hosted web and product analytics platform built for agencies, SaaS operators, and regulated enterprises. Named after **Spica**, the luminous blue-white spectroscopic binary star in the constellation Virgo (the 16th brightest star in the sky), SpicaAnalytics replaces bloated, surveillance-heavy analytics suites (Google Analytics 4, Mixpanel, Amplitude) with a blazing-fast, privacy-compliant telemetry engine.

Operating completely without cookies or personal identifiable information (PII) collection, SpicaAnalytics eliminates annoying GDPR cookie consent banners while capturing full-fidelity visitor metrics, custom event funnels, and campaign attribution under a 100% permissive MIT license.

---

## 🏛️ Agency & Enterprise Capabilities

### 1. 🛡️ Absolute Privacy Sovereignty (Zero Cookie Banners)
- Complies out-of-the-box with **GDPR, CCPA, PECR, and HIPAA** data residency requirements.
- Never tracks users across websites, never saves cookies on client browsers, and never sells or transmits visitor metrics to third-party ad networks.
- Bypasses ad-blockers and privacy extensions cleanly via self-hosted reverse-proxy endpoints.

### 2. ⚡ Featherweight Tracker (<2KB Embed)
- Ultra-compact tracking script (<2KB) executes asynchronously without render-blocking.
- Zero impact on Google Core Web Vitals, Largest Contentful Paint (LCP), or Cumulative Layout Shift (CLS).
- Custom script masquerading: easily rename `script.js` to `telemetry.js` to prevent DNS-level network blocking.

### 3. 🎯 Custom Event Telemetry & Conversion Funnels
- Track granular user actions: button clicks, form submissions, modal opens, and checkout completions.
- Visualize multi-step onboarding funnels and user drop-off points to optimize SaaS trial conversions.
- Tag and segment custom user properties and e-commerce cart values dynamically via JavaScript SDK.

### 4. 🌐 Real-Time Multi-Tenant Agency Portals
- Manage dozens of client domains, subdomains, and marketing microsites from one centralized master dashboard.
- Generate secure, shareable public or password-protected reporting links for executive stakeholder reviews.
- Real-time visitor activity stream with geographical country mapping, OS/browser breakdowns, and UTM campaign tracking.

### 5. 🔒 Deterministic Self-Hosted Infrastructure
- Runs on your private cloud (AWS, GCP, Azure, Bare-Metal, Render, Docker) with standard PostgreSQL or MySQL storage.
- Scale to 50,000,000+ monthly pageviews without per-seat or per-event pricing penalties.
- Built-in data export (CSV / JSON) and automated database retention policies for long-term historical records.

---

## 🛠️ Technology Stack

| Layer | Technologies |
| :--- | :--- |
| **Frontend & Dashboard** | Next.js 15, React 19, Tailwind CSS, Radix UI, Lucide Icons |
| **Backend API** | Next.js API Routes, Node.js 20+, OpenAPI 3.0 |
| **Database & ORM** | Prisma ORM, PostgreSQL 15+ (or MySQL / SQLite) |
| **Tracker Client** | Rollup, TypeScript, Vanilla JS (<2KB gzip) |
| **Orchestration** | Docker, Docker Compose, Render Blueprint (`render.yaml`) |

---

## 🚀 Instant Deployment

### Local / Production Docker Compose

Ensure Docker and Docker Compose are installed:

```bash
git clone https://github.com/wtfear/SpicaAnalytics.git
cd SpicaAnalytics

# Launch SpicaAnalytics and PostgreSQL
docker compose up -d
```

Open `http://localhost:3000` in your browser. Default login:
- **Username:** `admin`
- **Password:** `umami` *(Change immediately upon first sign-in)*

---

### Cloud 1-Click Deployment (Render)

Deploy production-grade SpicaAnalytics with managed high-availability PostgreSQL in one click using Render:

1. Push this repository to your GitHub organization.
2. In Render, select **Blueprints** -> **New Blueprint Instance**.
3. Select this repository; Render will parse [`render.yaml`](./render.yaml) and provision:
   - `spica-analytics-web` (Docker Web Application)
   - `spica-analytics-db` (Managed PostgreSQL 15 Database)

---

## 📂 Repository Structure

```
SpicaAnalytics/
├── src/                  # Next.js application source
│   ├── app/              # App router pages, layouts, and API endpoints
│   ├── components/       # UI charts, visitor maps, and dashboard widgets
│   ├── lib/              # Database utilities, geoip resolution, and session helpers
│   └── tracker/          # Ultra-lightweight <2KB client tracking library
├── prisma/               # Database schema definition and migration history
├── public/               # Public assets and Spica binary star brand vectors
│   └── spica-logo.svg    # Primary brand vector emblem
├── docker-compose.yml    # 1-Click production multi-container orchestration
├── render.yaml           # Turnkey Render Infrastructure-as-Code specification
├── package.json          # Package manifest and build scripts
└── README.md             # Institutional documentation
```

---

## 📜 Licensing

SpicaAnalytics is open-source software licensed under the permissive **[MIT License](LICENSE)**.

---

<p align="center">
  Built with pride by the <strong>WTFear</strong> Open-Source Enterprise Initiative.
</p>
