# Easy SWA migration fixture

Synthetic development data only. A plain HTML/CSS site with two public pages,
no SWA configuration, APIs, authentication, secrets, or framework dependencies.

Build with `npm run build` on Node.js. Source is in `site/`; output is `dist/`.
Azure source metadata uses this repository, branch `main`, app location `/`,
and output location `dist`. Deployment is manual with Azure Developer CLI
from the separate fixture orchestrator workspace; there is no Actions workflow.

Expected later assessment: straightforward static-site migration candidate.
This expectation is not a guarantee that every target or migration tool
supports it. No migration has been performed.

Verification markers:
- `/`: `swa-migration-easy-v1`
- `/about.html`: `swa-migration-easy-about-v1`
- `/styles.css`: public stylesheet

Hosting resource: `jordan-swa-migration-easy`, Free SKU, East US 2, in
`jordan-embr-workspace`. Do not migrate or remove it without a separate request.
