# Anti-Flash

```text
+----------------------------------------------------------------------------+
|                                                                            |
|   ###  #   # ##### #####       ##### #      ###   #### #   #               |
|  #   # ##  #   #     #         #     #     #   # #     #   #               |
|  #   # # # #   #     #         #     #     #   # #     #   #               |
|  ##### #  ##   #     #   ----- ####  #     #####  ###  #####               |
|  #   # #   #   #     #         #     #     #   #     # #   #               |
|  #   # #   #   #     #         #     #     #   #     # #   #               |
|  #   # #   #   #   #####       #     ##### #   # ####  #   #               |
|                                                                            |
|  ONE CLICK. LESS GLARE.                                  OPEN BETA         |
|  LOCAL BOOKMARKLET  |  MANUAL + OPTIONAL AUTO  |  NO ACCOUNT               |
+----------------------------------------------------------------------------+
```

**Dark mode for the pages that forgot it.** Anti-Flash is a lightweight, reversible browser bookmarklet that makes bright web applications easier to read. Start with a fast Manual theme, or choose **Analyze** to adapt the page's own colors.

**Open beta · v0.1.0** — usable for personal testing, with known compatibility and performance limitations. No account, extension, subscription, cloud service, or runtime dependency.

## Install in two minutes

1. **[Download the offline installer](anti-flash-installer.html)** using GitHub's **Download raw file** action.
2. Open the downloaded `anti-flash-installer.html` in desktop Chrome. Firefox is also tested; Edge uses the Chromium engine but this Auto build has not been directly field-tested in Edge.
3. Show your bookmarks bar (`Ctrl+Shift+B`; `Cmd+Shift+B` on macOS), then drag the **Anti-Flash** button from the installer onto it.
4. On a bright website, click the **Anti-Flash** bookmark to enable **Manual** dark mode.
5. Click **Analyze** in the floating panel to enable Auto color adaptation. Switch palettes whenever you want.

If dragging is restricted, create a bookmark manually using the contents of [`anti-flash-bookmarklet.txt`](anti-flash-bookmarklet.txt) as its URL. Some managed browsers prohibit bookmarklets; Anti-Flash does not bypass those policies.

## Everyday controls

| Action | Result |
| --- | --- |
| Click the bookmark | Turn Manual styling on, or toggle the current styling off/on |
| **Analyze** | Opt into Auto mode, which reads accessible page colors |
| **Manual** | Return to selector-based styling without Auto scanning |
| **Palette** | Select Tokyo Night, Midnight, or Synthwave |
| **Remove**, or reload the page | Restore the website's original appearance |
| Delete the bookmark | Uninstall Anti-Flash (no other application was installed) |

Manual uses targeted selectors for common web UI elements such as tables, forms, menus, popovers, and Blueprint components. Auto maps accessible stylesheets, CSS variables and sampled computed colors into a dark palette and watches for many dynamic page changes. Auto does not scan before you click Analyze. On some Blueprint-based pages, **Manual may be more legible than Auto**.

## What the beta has actually tested

The source project validated the M2 build on Chromium/Chrome 153, Firefox 159.0.1 and WebKitGTK 2.52.6, including real bookmark installation and clicks in Chrome, functional synthetic fixtures, dynamic page changes and tests on public websites. The original validation covered a local SPA plus six public sites.

**Not verified:** live Palantir Foundry, Safari itself, current Edge Auto mode, Windows/macOS desktop installation and mobile browsers. Some complex gradients, nested frames, cross-origin stylesheets, shadow DOM and long pages may retain bright areas or imperfect contrast. Auto can briefly pause rendering on large pages; several performance targets were missed. This is a public beta, not a production-compatibility guarantee.

For a clear overview, see [Beta notes](BETA.md). For browser and security boundaries, see [Security](SECURITY.md).

## Privacy and reversibility

Anti-Flash operates in the current browser tab. The generated installer and bookmarklet are self-contained. No accounts, telemetry, background server or external JavaScript are required. Its temporary CSS and annotations are removed by **Remove** or a reload. The bookmarklet does run with in-page JavaScript privileges: inspect the code and follow your organization's policies before running it on work websites.

The public distribution contains the self-contained installer and generated bookmark URL. It does **not** include the private project's development history, source modules, test fixtures or research logs. The compiled JavaScript inside the installer remains inspectable.

## Feedback and license

Please [report non-sensitive bugs or ideas](https://github.com/itscooleric/anti-flash/issues), including browser/version, the site type, selected mode/palette and reproduction steps. Do not include confidential screenshots, page contents, customer data or credentials.

[MIT License](LICENSE) · [Security notes](SECURITY.md) · [Beta notes](BETA.md) · [Attribution](ATTRIBUTION.md)

Anti-Flash is an independent project. It is not affiliated with or endorsed by Palantir.
