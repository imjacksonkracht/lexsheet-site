# LexSheet marketing site agent instructions

## Purpose and deployment

This public dependency-free static site is deployed with GitHub Pages and `CNAME` set to `lexsheet.app`. It embeds the calculator from `calc.lexsheet.app` using a public license identifier.

## Local use

```bash
python3 -m http.server 8000
```

## Constraints

- Keep the site statically deployable unless a build system is explicitly approved.
- Do not invent product functionality, legal claims, prices, customer claims, security guarantees, or privacy promises.
- Keep marketing claims aligned with the deployed calculator and gateway.
- The privacy policy must distinguish ordinary client-side calculations from optional lead submission, which sends contact and estimate context to the gateway for storage and email delivery.
- Changes to `privacy.html` and `terms.html` require explicit legal review; do not present generated copy as legal advice or final approval.
- Preserve iframe accessibility, responsive behavior, and calculator availability.

## Verification

- Serve locally and test navigation, CTA links, calculator embed, policy links, representative viewport sizes, console errors, and missing assets.
- Validate HTML, accessibility basics, external links, CNAME, and a deployed smoke test when deployment is authorized.

## Code review rules

- Flag false or outdated privacy statements, broken calculator embedding, inconsistent pricing/claims, inaccessible controls, and accidental exposure of non-public configuration.
