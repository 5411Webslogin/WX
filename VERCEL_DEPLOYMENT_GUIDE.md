# Vyom Nex — GitHub + Vercel Deployment Guide

## What to upload to GitHub
Upload the extracted contents of this folder, not the ZIP file itself.

This is a Next.js project using the `src/app` structure, so the app routes are inside:

```text
src/app/
```

## Required files/folders included

```text
src/
public/
supabase/
package.json
pnpm-lock.yaml
next.config.ts
tailwind.config.ts
tsconfig.json
postcss.config.mjs
.env.example
.gitignore
README.md
```

## Deploy on Vercel

1. Create a GitHub repository.
2. Upload all extracted files and folders to the repository root.
3. In Vercel, click **Add New Project**.
4. Import the GitHub repository.
5. Framework preset should be **Next.js**.
6. Install command: `pnpm install`
7. Build command: `pnpm build`
8. Output directory: leave blank/default.
9. Add environment variables from `.env.example`.
10. Click **Deploy**.

## Environment variables
Check `.env.example`. You will likely need Supabase keys before the admin/database features work.
