# Code Style

- TypeScript strict mode — no `any`, prefer explicit types at module boundaries
- Named exports over default exports (except Next.js pages/layouts which require default)
- Prefer `const` functions over `function` declarations for components
- File names: `kebab-case` for files, `PascalCase` for component files (`Button.tsx`)
- Keep components small and single-purpose; extract logic into custom hooks
