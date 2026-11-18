# Next.js Full-Stack App Rules (`CLAUDE.md`)

Instructions for Claude Code when developing production full-stack Next.js applications using the App Router.

---

```markdown
# Next.js App Router Guidelines

## Technology Stack
- Next.js 15 (App Router paradigm)
- TypeScript in strict mode
- Tailwind CSS
- Zod for server and client payload validation

## Architecture Principles
- Default to React Server Components (RSC) unless interactivity or browser APIs are explicitly needed (`use client`).
- Isolate server mutations inside Server Actions located in `app/actions/`.
- Validate all incoming network input using Zod schemas before database queries.
- Structure route groups cleanly: `(marketing)` for public landing pages, `(app)` for authenticated dashboard views.

## Verification Commands
- Local development: `npm run dev`
- Lint & format check: `npm run lint`
- Full typecheck and build: `npm run build`
```
