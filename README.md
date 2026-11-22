# ResumeAI — live link

GitHub Pages entry point for the ResumeAI app hosted at
<https://resume-ai-copy-2dde0a01.base44.app>.

Visiting `https://preetamggoudar.github.io/resume-ai/` (or any path under it, e.g.
`/builder`, `/analyzer`, `/pricing`) redirects to the same path on the Base44 app.

This is a redirect, not a copy of the app: Base44 owns the app code, backend, auth and AI
features. To host the app itself here, export the Base44 source and replace these files
with the built frontend.

## Custom domain

Configured for **`resumeaiapp.com`** (`CNAME` file + GitHub Pages custom domain).

At your registrar, point the domain at GitHub Pages:

| Type | Name | Value |
| --- | --- | --- |
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |
| CNAME | `www` | `preetamggoudar.github.io` |

Once DNS propagates, GitHub issues the certificate automatically. Enable “Enforce HTTPS”
under Settings → Pages, then visit `https://resumeaiapp.com`.

Note: the page still redirects to the Base44-hosted app, so the address bar will show the
Base44 URL after loading. Keeping the custom URL requires connecting the domain directly
in Base44 (paid Starter plan) instead.
