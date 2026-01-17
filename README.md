# Novastone Website (Codex Overview)

## Project goal
Static marketing website for Novastone, built with Vite + React + Tailwind.

## Tech stack
- Vite + React (JSX, ES modules)
- Tailwind CSS (via `@tailwindcss/vite`)
- Vercel Analytics
- Supabase client (if enabled in the app)

## Folder map
- `index.html` Vite entry
- `src/main.jsx` app bootstrap
- `src/App.jsx` primary page composition
- `src/components` UI, layout, and section components
- `src/assets` images, SVGs, fonts
- `src/lib/supabase.js` Supabase client setup
- `public` static assets
- `tailwind.config.js` Tailwind configuration
- `vite.config.js` Vite config

## Scripts
- `npm run dev` local dev server
- `npm run build` production build
- `npm run preview` preview production build
- `npm run lint` ESLint

## Env setup
Copy `.env.example` to `.env` and replace values, or use `.env.development` for local Supabase.

## Notes for Codex
- This repo is a structural clone of a Tecnofit site; keep the same project layout and tooling.
- When adding new sections, follow the existing pattern in `src/components/sections`.
- Keep assets in `src/assets` and reference via relative imports in components.
