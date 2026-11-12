# Review checklist

## Passed

- Deployed homepage matched the original repository source before editing.
- Static local HTML page, asset and fragment links pass.
- Existing support/privacy/terms main text and contact links preserved.
- Released-app App Store target verified against the official Apple listing.
- Every page links to the personal portfolio and its verified app section, `https://pond1982.github.io/Pondd-Page/index.html#apps`. This section is part of the companion portfolio PR.
- No demo forms, placeholder download links or Android claims added.
- Base New Age MIT license retained; existing hosting configuration unchanged.
- All 14 HTML pages across Landslide, 21 Counts, Stack Fighters, StackCycle and The AI Company rendered in the supported cloud browser at 320, 390 and 1365 px: no document overflow, missing H1 or broken loaded image assets.
- Browser review caught narrow-screen gutters, now corrected and retested.
- Representative visual inspection: 21 Counts desktop/mobile and StackCycle mobile.
- Shared keyboard sample on 21 Counts: first Tab reveals Skip to content, Enter reaches main, next Tab reaches the App Store hero link, and six following Tabs continue without a trap.

## Verification limits

- No axe/Lighthouse, real-mobile-device or complete accessibility audit.
- 200% zoom could not be verified with the available browser controls.
- Full external CTA navigation was not exercised.
- Navigation works without JavaScript; focus and reduced-motion styles are implemented, not a substitute for the unrun checks above.

Keep as a draft for owner review. No production merge or hosting-settings changes.
