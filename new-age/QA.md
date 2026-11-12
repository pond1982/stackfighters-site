# Review checklist

- Verified deployed homepage exactly matches the original repository source before edits.
- Local HTML page, asset and fragment links pass static checks.
- Existing support/privacy/terms main text and contact links preserved.
- Verified released-app App Store target from the official Apple listing.
- All pages include personal portfolio and app directory links. The app directory is part of a separate portfolio change and may not be live until that is merged.
- No placeholder download links, demo forms or Android claims added.
- Base New Age MIT license retained. Existing hosting configuration unchanged.
- Responsive CSS, keyboard focus and reduced-motion rules provided; no JavaScript is required for navigation.

## Still to verify before merge

Rendered desktop/mobile/200% zoom and keyboard tests were not run: installed Chromium aborts with `socket() Operation not permitted` in this execution environment. Static checks are not a substitute for browser QA. Keep this PR in draft until these checks are completed.
