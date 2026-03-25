# Backend API

## Commands
npm run dev          # Start dev server (port 3000)
npm run test         # Run tests (Vitest)
npm run lint         # ESLint + Prettier
npm run build        # TypeScript compile
npm run db:migrate   # Run Prisma migrations
npm run db:seed      # Seed test data

## Architecture
- Express REST API on Node 22 with TypeScript
- PostgreSQL via Prisma ORM
- Handlers in src/handlers/, middleware in src/middleware/
- Shared types in src/types/
- Tests mirror src/ structure in tests/

## Conventions
- Validate all request bodies with zod schemas
- Return shape is always { data, error, meta }
- Never expose stack traces in responses
- Use the logger module (src/lib/logger.ts), not console.log
- All database queries go through Prisma, no raw SQL

## Important
- Tests hit a real local database, not mocks. Run `npm run db:test:reset` first
- Strict TypeScript: no unused imports, no any types
- Every handler needs integration tests covering happy path + error cases