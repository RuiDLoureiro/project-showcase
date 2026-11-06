# Personal Portfolio

**Status: in development.** An English portfolio built with React, TypeScript and Vite.

## Purpose
Present software engineering experience, education and personal projects through accessible project summaries and detailed views.

## Documented implementation
- React and TypeScript frontend with Vite production builds.
- Project detail dialogs and a profile assistant interface.
- A Python assistant API maintained as a separate service.
- Server-side provider integration using public profile context.
- Input/output validation, bounded conversation context and local usage limits.
- An Azure Static Web Apps workflow committed to GitHub.

## Architecture and deployment
The frontend is compiled to static assets. The Python API needs its own runtime and deployment configuration; publishing the static frontend does not deploy the API.

An Azure Static Web Apps workflow was added during development. The [portfolio site](https://rui-loureiro-portfolio.web.app/) is the public entry point; the frontend and the assistant API have separate deployment requirements.

## Limits
In-memory request counters reset with the API process and do not provide distributed production rate limiting. Source references guide grounding but do not guarantee factual model responses.

See the [development log](CHANGELOG.md). Source code remains private. JavaScript delivered to a visitor's browser remains inspectable even when its repository is private.
