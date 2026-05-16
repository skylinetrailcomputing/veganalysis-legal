# Privacy Policy — Veganalysis

**Last updated:** 2026-05-12
**Effective:** _(set when Veganalysis is first distributed beyond the
developer's own devices)_

**Publisher:** Skyline Trail Computing LLC (Colorado, USA)
**App:** Veganalysis (iOS; Android planned)
**Contact:** legal@skylinetrailcomputing.com  ·  GitHub Issues:
<https://github.com/skylinetrailcomputing/veganalysis-legal/issues>

## Summary

Veganalysis is a barcode-scanning app that identifies likely non-vegan
ingredients in packaged products. It runs on your device, holds no
account, and **Skyline Trail Computing collects nothing about you, your
scans, your usage, or your device.** There is no analytics SDK, no
telemetry, no advertising, no in-app purchases.

When the app needs to look up a product it does not already have on
your device, it sends the product's barcode to **Open Food Facts**, a
non-profit open-data project. Open Food Facts therefore sees that
someone (your IP address, the request timing) asked about that
barcode. Open Food Facts is a separate organization with its own
privacy practices: <https://world.openfoodfacts.org/>.

That outbound Open Food Facts call is the only data plane
Veganalysis initiates on its own. There is one additional path,
**user-initiated only**, described next.

## Voluntary feedback submission

Veganalysis includes two in-app features that let you compose and
send a message to Skyline Trail Computing through your own email
client: **"Send Feedback"** (which packages scans you have
flagged in-app into a feedback bundle) and **"Report a Problem"**
(a free-text draft for general app problems, with no attached
scan data). **In both cases, the contents you compose are
received by us via your email client. This is voluntary and
user-initiated; no other data is collected.**

The "Send Feedback" bundle contains only the scans you have
flagged in-app (either to report a verdict you disagree with, or
to attach a barcode for a product you scanned via the OCR
fallback). Camera frames, location, device identifiers, account
information, and product images are never included. You see the
email — including the JSON attachment — in your own mail composer
before sending; you can edit, attach, or discard at will. Nothing
is sent automatically, in the background, or without your
explicit Send action in your mail client.

The "Report a Problem" draft contains the text you write plus a
small auto-filled context block — your app version, iOS version,
device model class (e.g., `iPhone16,2`), and locale. None of
these uniquely identify you or your device. The draft has no
attachment. As with "Send Feedback", you see and can edit the
entire message in your own mail composer before sending, and
nothing is sent without your explicit Send action.

If your device does not have a configured mail account, the app
offers a system Share Sheet for "Send Feedback" so you can route
the bundle through another messaging app of your choice. For
"Report a Problem", the app surfaces our contact email address as
selectable text so you can copy it into the messaging app of your
choice. That choice remains entirely yours in either case.

## What Veganalysis stores on your device

- A bundled product database, shipped as part of the app. Read-only.
- A local cache of up to ~5,000 product lookups you have previously
  made (barcode + the product information returned by Open Food
  Facts). Stored in the app's private storage area on your device.
  **Never transmitted off your device.**
- Standard iOS app preferences (e.g., onboarding-completed flag).

iOS removes all of this when you uninstall the app.

## What Veganalysis sends over the network

**Only this:** an HTTPS GET request to the Open Food Facts API at
`world.openfoodfacts.org/api/v2/product/<barcode>.json`, sent only
when the scanned product is not already in the bundled database or
the on-device cache.

The request includes:

- The barcode you scanned.
- Standard HTTP headers your device sends, including your IP address
  and a User-Agent identifying the app (e.g., `Veganalysis-iOS/0.1`).

It does **not** include: your name, account, email, device
identifier, location, advertising identifier, contacts, photos, or
any other personal information. Veganalysis does not collect or hold
any of those things in the first place.

## What Open Food Facts may see

Because Open Food Facts receives the request directly:

- It sees the barcode looked up.
- It sees your IP address (visible to any web server you contact).
- It sees the timing of requests.
- It does not see your identity unless your IP address is
  independently identifiable to them — which Veganalysis cannot
  control.

Open Food Facts is run by the Open Food Facts Association (a French
non-profit). Their handling of any information they receive is
governed by their own privacy policy, linked above.

## Camera

Veganalysis uses your device's camera to read product barcodes.
Camera frames are processed in memory on your device and discarded
immediately after the barcode is decoded. **Camera frames are never
stored on your device, transmitted off your device, or shared with
anyone, including Skyline Trail Computing.**

iOS will ask your permission before Veganalysis accesses the camera.
You can revoke access at any time in **iOS Settings → Privacy &
Security → Camera**.

## Analytics, advertising, third-party SDKs

There are none. Veganalysis ships with no analytics SDK, no
advertising SDK, no crash-reporting SDK, no third-party data plane of
any kind. The Apple-mediated crash and usage diagnostics that you may
have opted into in **iOS Settings → Privacy & Security → Analytics &
Improvements** are sent to Apple under Apple's own policies —
Veganalysis does not see or receive that data.

## Accounts, in-app purchases, subscriptions, ads

None of these exist in Veganalysis, and there is no plan to add them.
Veganalysis is free, with no in-app purchases, no subscriptions, and
no advertising.

## Children

Veganalysis is not directed at children under 13. Because Veganalysis
does not collect any personal information from any user, it does not
knowingly collect personal information from children either. Skyline
Trail Computing has no mechanism by which any user, of any age, could
provide personal information through this app.

## Your rights (GDPR, CCPA, Colorado CPA, and similar)

Various jurisdictions give you rights over personal information about
you that a company holds. **Skyline Trail Computing holds no personal
information about you.** There is therefore nothing for us to
disclose, correct, port, or delete on request.

Open Food Facts, as a separate data processor, has its own
obligations and processes regarding any data they receive — see their
privacy policy.

## Changes to this policy

If this policy materially changes, the change will be reflected in an
updated `Last updated` date at the top of this document, in a note in
the app's release notes, and in the commit history of this repository.

## Contact

- **Email:** legal@skylinetrailcomputing.com
- **GitHub Issues:**
  <https://github.com/skylinetrailcomputing/veganalysis-legal/issues>

## A note on what this policy covers

This policy covers privacy practices only. Veganalysis identifies
likely non-vegan ingredients from product labels. **It is not a
guarantee, and it is not designed for allergen safety.** People with
allergies must contact the manufacturer for definitive ingredient and
cross-contact information. The in-app disclaimers and the App Store
listing carry the app's accuracy and allergen disclaimers in full.
