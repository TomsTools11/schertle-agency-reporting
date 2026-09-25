# Angela Schertle Agency Reporting

Static GOAL reporting site for Angela Schertle Agency, deployed on Vercel from this repo. Pushes to `main` redeploy automatically.

| File | URL | Page |
| --- | --- | --- |
| `public/index.html` | `/` | Report hub |
| `public/reports/ok-auto-campaign-configuration-2026-09-25.html` | `/reports/ok-auto-campaign-configuration-2026-09-25` | OK Auto configuration |
| `public/reports/ok-home-campaign-configuration-2026-09-25.html` | `/reports/ok-home-campaign-configuration-2026-09-25` | OK Home configuration |

Everything under `public/` is served. `vercel.json` pins the output directory to `public`, enables clean URLs, and sends `noindex` headers. There is no build step: Framework Preset **Other**, no build or install command.

County maps live in `public/assets/` and load as `<img>` from the reports. Each report links back to the hub with the "All Reports" button in its sidebar.
