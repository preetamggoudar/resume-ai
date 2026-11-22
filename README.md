# ResumeAI — live link

GitHub Pages entry point for the ResumeAI app hosted at
<https://resume-ai-copy-2dde0a01.base44.app>.

Visiting `https://preetamggoudar.github.io/resume-ai/` (or any path under it, e.g.
`/builder`, `/analyzer`, `/pricing`) redirects to the same path on the Base44 app.

This is a redirect, not a copy of the app: Base44 owns the app code, backend, auth and AI
features. To host the app itself here, export the Base44 source and replace these files
with the built frontend.

## Custom domain

No custom domain is configured. A `resumeaiapp.com` setup was attempted and reverted
because that domain was never purchased; GitHub was redirecting the working GitHub Pages
URL to the dead domain.

To try again later: buy the domain, add the standard GitHub Pages `A`/`CNAME` records,
add a `CNAME` file with the domain to this repo, and set it under Settings → Pages.

Note: this page redirects to the Base44-hosted app, so the address bar will show the
Base44 URL after loading. Keeping your own URL visible requires connecting the domain
directly in Base44 (paid Starter plan) instead.
