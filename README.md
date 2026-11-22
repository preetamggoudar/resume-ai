# ResumeAI — old URL (redirect only)

This repository now only redirects to the live site at **https://resumeaiapp.github.io/**.

This is a GitHub Pages copy of the ResumeAI frontend. It keeps the visible URL on
`github.io` while Base44 continues to provide auth, data, AI and file storage.

## How it works

- `index.html` loads the built React app from `assets/`.
- The bundle's Base44 SDK is configured with the original app's server URL and app id.
- The router uses `/resume-ai` as its basename, so links stay under the Pages path.
- An inline shim restores deep links from `404.html` and sends `/api/...` calls to Base44.
- `404.html` sends deep links back through `index.html` so client-side routing works.

## Verified

Landing page, `/interviews` (40 questions / 37 companies), company and practice pages,
`/pricing`, direct deep links, and the login flow all load on the `github.io` URL without
redirecting to `base44.app`.

## Limitations

- This is a build mirror, not the original source. It won't update automatically when the
  Base44 app changes — re-export/rebuild to sync.
- Login, AI features and data still run on Base44. Only the frontend is hosted here.
- To move everything off Base44 requires the real source code and a replacement backend.
