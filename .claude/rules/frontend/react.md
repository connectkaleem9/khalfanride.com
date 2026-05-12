# React / Next.js Rules

- Use the App Router (`app/`) — do not mix with Pages Router
- Server Components by default; add `"use client"` only when state/events are needed
- Fetch data in Server Components or Route Handlers, not in client components
- Images: always use `next/image` with explicit `width`/`height` or `fill` + a sized parent
- Fonts: load via `next/font` — never import font CSS directly
- Avoid `useEffect` for data fetching; use server-side patterns instead
