# Protocol Health — Website Spec

## Overview

**Brand:** Protocol Health
**Type:** Health & Longevity Clinic
**Purpose:** A shareable website that shows the services Protocol Health offers and walks prospective patients through a health questionnaire funnel.

---

## Current Scope

This is a V1 demo site — no real booking, no payments, no calendar.

1. **Services Offered** — displays all services, treatments, and diagnostics → see `SERVICES.md`
2. **Questionnaire Funnel** — multi-step form collecting health goals and symptoms, ends on a confirmation screen → see `BOOKING_FUNNEL.md`

Not included in V1:
- Calendar / appointment scheduling
- Payments / Stripe
- User accounts or data storage

---

## Tech Stack

| Layer | Decision |
|---|---|
| Framework | Next.js (App Router) |
| Styling | Tailwind CSS |
| Hosting | Vercel |
| Funnel | Custom multi-step React component |

---

## Design Direction

- **Tone:** Clean, clinical, trustworthy, approachable
- **Layout:** Single-page scroll; two clear sections
- **Mobile-first:** Most users on mobile
- **Colors / UX:** TBD — inspiration site pending
- **Typography:** Sans-serif, modern (e.g., Inter, DM Sans)

---

## Open Items

- [ ] Share inspiration site for colors / UX direction
- [ ] Clinic address, phone, email, hours
- [ ] Brand colors and typography
- [ ] Photography / imagery
