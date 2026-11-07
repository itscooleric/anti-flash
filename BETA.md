# Anti-Flash — Open beta v0.1.0

**Release status:** public-facing beta candidate. This document does not itself publish a GitHub Release or make a private repository public.

Anti-Flash is an offline browser bookmarklet for reversible dark styling. The beta has **Manual** mode for common component selectors, and **Auto**, which runs after an explicit **Analyze** click to map accessible page colors. Auto can adapt when menus, dialogs, and other parts of a single-page app change.

## Quick trial

Download the single-file [installer](anti-flash-installer.html), open it on desktop Chrome, drag the bookmarklet to the bookmarks bar, then open a bright page. Click the bookmark, switch to Analyze if Manual leaves difficult regions, change the palette, and press Remove to restore the page.

No build system or Python is needed to use this distribution.

## Validation and limitations

- **Observed in the private development project:** Chrome/Chromium 153, Firefox 159.0.1 and WebKitGTK 2.52.6 functional tests; Chrome installer drag and real bookmark/Analyze clicks; test sites and local SPA; removal/restoration.
- **Not established by this distribution:** an additional release-specific browser test, compatibility with actual Palantir Foundry, Safari/Windows/macOS installation, support for mobile browser bookmarks, or guaranteed accessibility contrast on all websites.
- **Known constraints:** Auto cannot directly inspect cross-origin stylesheets; shadow DOM and iframes may be missed; 1,500-element sampling may leave far-down content partly bright; gradients and certain CSS constructs can be difficult. Long pages may incur momentary browser restyling pauses.
- **User control:** Manual mode starts by default. Auto is opt-in. Remove or reload to restore. Installation is a regular bookmark; there is no background extension or persistence service.
- **Managed browser policy:** some enterprise browsers disable bookmarklets. Do not try to bypass these policies.

This candidate incorporates the generated M2 browser distribution from the private development snapshot dated November 6, 2026. The installer and bookmarklet are copied byte-for-byte and not rebuilt in this public packaging.

## Updating and rollback

Bookmarklets do not auto-update. To update, download a newer installer and replace your bookmark. To roll back to the original page appearance, use **Remove** or reload; to uninstall, delete the bookmark.

Report reproducible issues at [GitHub Issues](https://github.com/itscooleric/anti-flash/issues). For sensitive security concerns, use private vulnerability reporting if enabled, not a public issue.

See [README](README.md), [security guidance](SECURITY.md), and [MIT license](LICENSE).
