# ResumeAI — GitHub-hosted frontend

Live at **https://preetamggoudar.github.io/resume-ai/**

This is a GitHub Pages copy of the ResumeAI frontend. It keeps the visible URL on
`github.io` while Base44 continues to provide auth, data, AI and file storage.

## How it works

- `index.html` loads the built React app from `assets/`.
- The bundle's Base44 SDK is configured with the original app's server URL and app id.
- An inline shim strips the `/resume-ai` path prefix for the router, re-prefixes internal
  navigation, and sends `/api/...` calls to Base44.
- `404.html` sends deep links back through `index.html` so client-side routing works.

## Limitations

- This is a build mirror, not the original source. It won't update automatically when the
  Base44 app changes — re-export/rebuild to sync.
- Login, AI features and data still run on Base44. Only the frontend is hosted here.
- To move everything off Base44 requires the real source code and a replacement backend.
