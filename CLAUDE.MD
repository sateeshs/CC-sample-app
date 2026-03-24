# Next.js Project

This is a Next.js project using the App Router architecture.

## Tech Stack
- Next.js 16+ with App Router
- TypeScript for type safety
- Tailwind CSS v4 for styling
- React Server Components by default
- shadcn/ui
- ESLint + Prettier


## Project Structure
- `src/app/` - App Router pages and layouts
- `src/components/` - Reusable React components
- `src/lib/` - Utility functions and shared code
- `src/public/` - Static assets
- `src/types/` — Type definitions

## Conventions
- Use Server Components by default, add 'use client' only when needed
- Prefer named exports for components
- Use TypeScript strict mode
- Follow the Next.js file-based routing conventions
- Use next/image for optimized images
- Use next/link for client-side navigation

## Code Style
- All components must be written in TypeScript
- Prefer async/await over .then() chains
- Use early returns for cleaner code
- Keep components small and focused
- No `any` types allowed
- Prefer `type` over `interface`
- Default to Server Components; only add `"use client"` when necessary

## Off-Limits
- No code outside `src/`
- No CSS-in-JS (use Tailwind)
- No `console.log` in committed code

## Commands
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run lint` - Run ESLint
