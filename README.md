# veganalysis-legal

Public-facing legal documents for Veganalysis (iOS / Android), published
by Skyline Trail Computing LLC (Colorado, USA).

## Status — public, Pages enabled

Flipped public on 2026-05-16 to support the Veganalysis F&F TestFlight
period. The in-app EULA and Privacy Policy reference
`https://skylinetrailcomputing.github.io/veganalysis-legal/privacy.html`,
and that URL must resolve for F&F testers who tap through — flipping
at F&F prep rather than at App Store submission eliminates the
F&F-period 404 window.

`docs/privacy.md` and `docs/eula.md` are the authoritative sources;
GitHub Pages publishes them as HTML from `main`.

The `Effective` date in both documents stays a placeholder until
Veganalysis is first distributed beyond the developer's own devices
(F&F TestFlight start). The `Last updated` date is set whenever the
content materially changes.

Pre-launch checklist still owed against this repo:

1. Verify the Open Food Facts privacy-policy deep-link in
   `docs/privacy.md` still resolves; update if their URL has shifted.
2. Set the `Effective` dates in `docs/privacy.md` and `docs/eula.md`
   on the day F&F TestFlight invitations first go out.
3. Wire the Privacy Policy URL into App Store Connect → App Privacy,
   and into Google Play Console when the Android submission lands.

## Contents

- `docs/privacy.md` — Privacy Policy.
- `docs/index.md` — landing page linking the policy and EULA.
- `docs/eula.md` — **v1 draft landed 2026-05-16** (v0 same day; v1
  adds arbitration + class-action waiver §11, Feedback license §8,
  "Needs review" verdict semantics in §5.1, OFF query precision in
  §3, and an HTML-comment Clement-review flag on §2). Covers
  license grant, restrictions, OFF/ODbL data attribution,
  App-specific disclaimers (accuracy, allergen safety, OFF data
  quality, not medical/dietary advice), limitation of liability,
  feedback license, Apple/Google third-party-beneficiary framing,
  arbitration and class-action waiver, and Colorado governing law.
  **Producer-driven draft pending refinement by Ryan Clement /
  Business & Technology Legal Group via the client portal** — per
  `~/claude-workspace-2026/knowledge/legal-entity-for-apps.md` §10
  status 2026-05-15 and the producer-driven posture captured in
  Veganalysis memory `attorney_posture_producer_driven.md`. Set
  `Last updated` / `Effective` placeholders at the top of the file
  when the refined version is approved for distribution.

## Cross-references

- Veganalysis app: `github.com/bradleypmartin/veganalysis` (private
  until the OSS migration; tracked in that repo's `NEXT.md`).
- Skyline Trail Computing LLC — Colorado, formed 2026-04-26.
