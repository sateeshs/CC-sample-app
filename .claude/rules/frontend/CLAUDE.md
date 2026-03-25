# Frontend Rules
- Prefer Server Components
- "use client" only when necessary
- Use Tailwind CSS v4 utility classes

## TypeScript Configuration

### Code generation rules
1. `as any` is banned. No exceptions.
2. `as Type` casting is only allowed after a type guard or Zod validation
3. All function parameters and return types must have explicit type annotations
4. Use `unknown` instead of `any`, then narrow with type guards
5. Rely on type inference where possible (excessive explicit annotations are also bad)

### Required verification
After generating any code, run `npx tsc --noEmit`.
Fix all type errors before submitting. Do not return code with type errors.
