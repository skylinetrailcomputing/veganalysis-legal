# veganalysis-legal

Public-facing legal documents for Veganalysis (iOS / Android), published
by Skyline Trail Computing LLC (Colorado, USA).

## Status — currently private

This repo will flip to **public**, with **GitHub Pages enabled**, when
Veganalysis App Store submission first requires a stable Privacy Policy
URL. Until then it stays private.

The flip trigger sits at the end of the F&F gate sequence:

D-U-N-S issued → STC org Apple Developer account opened → App Store
Connect submission for Veganalysis → Privacy Policy URL required → flip
this repo public.

See `~/veganalysis/DISTRO_CHECKLIST.md` and
`~/claude-workspace-2026/knowledge/legal-entity-for-apps.md` for the
gating items.

When the flip happens:

1. Apply the standard OSS protections:
   `~/claude-workspace-2026/scripts/oss-repo-protect.sh skylinetrailcomputing/veganalysis-legal`
   (per `~/claude-workspace-2026/knowledge/oss-repo-policy.md`).
2. Enable Pages: Settings → Pages → Source = Deploy from a branch,
   branch = `main`, folder = `/docs`.
3. Confirm the served URL is reachable:
   `https://skylinetrailcomputing.github.io/veganalysis-legal/privacy.html`.
4. Set the `Effective` date in `docs/privacy.md` (currently a
   placeholder).
5. Verify the Open Food Facts privacy-policy deep-link in
   `docs/privacy.md` still resolves; update if their URL has shifted.
6. Wire the URL into App Store Connect → App Privacy → Privacy Policy
   URL, and into Google Play Console when the Android submission lands.

## Contents

- `docs/privacy.md` — Privacy Policy.
- `docs/index.md` — landing page linking the policy and EULA.
- `docs/eula.md` — **v0 draft landed 2026-05-16.** Custom End User
  License Agreement covering license grant, restrictions, OFF/ODbL
  data attribution, App-specific disclaimers (accuracy, allergen
  safety, OFF data quality, not medical/dietary advice), limitation
  of liability, Apple/Google third-party-beneficiary framing, and
  Colorado governing law. **Producer-driven draft pending refinement
  by Ryan Clement / Business & Technology Legal Group via the
  client portal** — per
  `~/claude-workspace-2026/knowledge/legal-entity-for-apps.md` §10
  status 2026-05-15 and the producer-driven posture captured in
  Veganalysis memory `attorney_posture_producer_driven.md`. Set
  `Last updated` / `Effective` placeholders at the top of the file
  when the refined version is approved for distribution.

## Cross-references

- Veganalysis app: `github.com/bradleypmartin/veganalysis` (private
  until the OSS migration; tracked in that repo's `NEXT.md`).
- Skyline Trail Computing LLC — Colorado, formed 2026-04-26.
