# DIFY Battery Operations Platform

A dispatcher web application and native technician app for coordinating mobile vehicle-battery service—from customer intake and battery selection to field work and payment reconciliation.

**Developer:** [Noah Serrault](https://www.linkedin.com/in/noah-serrault-549a56252/) · Sole software developer

**Stack:** TypeScript · Next.js · React · React Native / Expo · PostgreSQL / Supabase

**Status:** Active development and staging validation; production-candidate platform.

This is a portfolio case study. Application source code, operational data, and credentials remain private. The scope below describes implemented functionality, not a claim that every workflow has completed production rollout or device validation.

## Why I built it

DIFY Battery delivers battery replacement service at the customer's location. Dispatchers and technicians need to coordinate vehicle compatibility, quotes, appointments, installation documentation, and payments across the same service job.

After working in DIFY's field operations and helping launch its Austin market, I returned as the company's sole software developer while pursuing my B.S. in Data Science at the University of Wisconsin–Madison. That operational experience informs the software: the goal is to consolidate workflows across multiple SaaS tools and make service knowledge easier for dispatchers and new employees to use.

## Application scope

| Area | What the platform supports |
| --- | --- |
| Customer intake and quoting | Capture service requests, look up vehicle-to-battery compatibility, and generate quotes using shared database pricing rules. |
| Scheduling and dispatch | Assign technicians, manage appointments and job status, and view map-based planning information. |
| Technician field app | View assigned jobs and route information, document installations with photos, and submit field updates through a React Native / Expo interface. |
| Service records | Keep job history, installation documentation, warranty information, and operational audit records connected to each job. |
| External integrations | Connect Square payment workflows, Twilio customer messaging, and Google Maps mapping and routing. |

### My role

As the sole software developer, my work spans workflow design, web and mobile interfaces, backend APIs, database modeling, third-party integrations, and automated testing. I translate the needs of dispatchers and technicians into a shared application rather than separate tools for each role.

## Backend engineering highlights

- **Shared business rules:** PostgreSQL command functions handle business-critical changes and pricing so web and mobile clients use the same authoritative rules.
- **Access control:** Role-based authorization and row-level security restrict access to operational data; service photos use private storage and authorized access.
- **Payment reconciliation:** Square webhooks and scheduled reconciliation connect provider-confirmed payment information to service jobs instead of treating a client-side checkout response as proof of payment.
- **Retry-safe processing:** Idempotency keys and an outbox-based retry mechanism support repeatable requests and external-service delivery without blindly duplicating work.
- **Field connectivity:** Queued mobile mutations and photo workflows address interrupted connectivity, with server-side validation when requests reach the backend.
- **Verification:** Vitest unit tests, Playwright browser tests, and separate mobile checks support development. Native device and payment validation are distinct from browser and unit testing.

See the [engineering overview](docs/ENGINEERING.md) for the architecture and design tradeoffs.

## Visual walkthrough

The planned walkthrough follows one service job through dispatch and the technician app:

1. Dispatcher overview and scheduling.
2. Vehicle selection, compatible battery lookup, and quote.
3. Technician job details and installation documentation.
4. Service history and payment review.

Screenshots will be added after capture using synthetic demonstration data. No customer or employee records will be published. The [capture plan](docs/SCREENSHOT_PLAN.md) defines the views and captions.

## Technology

| Layer | Technologies |
| --- | --- |
| Web | Next.js, React, TypeScript |
| Mobile | React Native, Expo |
| Backend and data | Next.js server-side APIs, PostgreSQL, Supabase Auth / Storage / Realtime |
| Integrations | Square, Twilio, Google Maps |
| Testing and monitoring | Vitest, Playwright, Sentry |
| Delivery and version control | Vercel, Git, GitHub Actions |

## Contact

[LinkedIn](https://www.linkedin.com/in/noah-serrault-549a56252/) · [GitHub](https://github.com/notannon)

For a walkthrough or a discussion of the implementation, please contact me through LinkedIn.
