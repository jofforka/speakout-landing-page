# SpeakOut AdSense Readiness Staging

Prepared: 2026-09-25

This branch is intentionally **not merged to main** because the currently connected GitHub repository does not match the live September 2026 production site at speakoutmentalhealth.org.

## Prepared fixes
- Site-wide Privacy Policy: `pages/privacy.html`
- Terms of Use: `pages/terms.html`
- Cookie Policy: `pages/cookies.html`
- Research page replacement with substantive, non-placeholder content: `pages/research.html`
- `ads.txt.example` template without a fabricated publisher ID

## Live-site edits still required in the actual production source
1. Homepage H1: remove duplicated text so it reads once:
   `Building healthier minds. Stronger schools. Brighter futures.`
2. Add footer links to Privacy Policy, Terms of Use and Cookie Policy across public pages.
3. Replace the current Research page placeholder section with the staged Research page content.
4. Do not place AdSense on MindCheck assessments, crisis/urgent-support pages, private portals, or pages whose activity may reveal sensitive health information or known child-directed activity.
5. Before serving ads to EEA/UK/Swiss users, configure a Google-certified CMP through AdSense Privacy & messaging (or another Google-certified TCF CMP).
6. Create live `/ads.txt` only after the exact AdSense publisher ID is available. Never use a placeholder publisher ID in production.

## AdSense implementation after cleanup
- Add the AdSense site-verification/ad script only after the live production source is connected.
- Start with limited placements on general informational/editorial pages.
- Keep ad density low initially.
- Recheck mobile layout, Core Web Vitals, broken links and policy pages before submitting for review.
