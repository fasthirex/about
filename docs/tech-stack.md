# Tech stack

A high-level view of how FastHireX is built. Each feature is kept modular, so it can be built and tested on its own.

## Clients

- **Web:** Next.js with TypeScript, styled with Tailwind CSS and shadcn/ui.
- **Mobile:** React Native with Expo.
- **Desktop:** Electron wrapping the web app, so one codebase serves all three.

## Backend and data

- **API:** FastAPI (Python).
- **Database:** PostgreSQL, one store across every service.

## Approach

- A clean, layered architecture: client, application, and data.
- Features are modular by design, which keeps them independently buildable and testable.
- The skill evaluation runs as a background job, so submitting one returns immediately and the result is written when it is ready.

> This page is intentionally high-level. It describes the shape of the system, not its internals.
