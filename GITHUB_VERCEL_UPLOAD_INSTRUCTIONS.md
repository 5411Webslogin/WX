# GitHub + Vercel Upload Instructions

## Important
Do not upload this ZIP directly to GitHub.

1. Extract the ZIP.
2. Open the extracted folder.
3. Upload the contents of the folder to GitHub, not the folder as a ZIP.
4. Your GitHub repository root must contain `package.json` directly.

Correct GitHub root structure:

```
package.json
pnpm-lock.yaml
next.config.ts
src/
public/
```

Incorrect structure:

```
vyom-nex-vercel-final/package.json
```

If your repository has the project inside a subfolder, then in Vercel set Root Directory to that subfolder.

## Vercel Settings
Framework Preset: Next.js
Root Directory: leave blank if `package.json` is in repo root
Install Command: pnpm install --frozen-lockfile
Build Command: pnpm run build
Output Directory: leave default

## Environment Variables
Add values from `.env.example` inside Vercel Project Settings > Environment Variables.
