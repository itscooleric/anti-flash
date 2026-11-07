# Anti-Flash

```text
   █████╗ ███╗   ██╗████████╗██╗      ███████╗██╗      █████╗ ███████╗██╗  ██╗
  ██╔══██╗████╗  ██║╚══██╔══╝██║      ██╔════╝██║     ██╔══██╗██╔════╝██║  ██║
  ███████║██╔██╗ ██║   ██║   ██║█████╗█████╗  ██║     ███████║███████╗███████║
  ██╔══██║██║╚██╗██║   ██║   ██║╚════╝██╔══╝  ██║     ██╔══██║╚════██║██╔══██║
  ██║  ██║██║ ╚████║   ██║   ██║      ██║     ███████╗██║  ██║███████║██║  ██║
  ╚═╝  ╚═╝╚═╝  ╚═══╝   ╚═╝   ╚═╝      ╚═╝     ╚══════╝╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝
```

**Open beta · v0.1.0**

Anti-Flash is a reversible dark-mode bookmarklet for desktop browsers. It starts in **Manual** mode; **Analyze** enables optional automatic color adaptation for the current page.

## Install

1. [Download `anti-flash-installer.html`](anti-flash-installer.html) using GitHub's **Download raw file** action.
2. Open the downloaded file in your desktop browser.
3. Show the bookmarks bar (`Ctrl+Shift+B` on Windows/Linux, `Cmd+Shift+B` on macOS).
4. Drag **Anti-Flash** from the installer onto the bookmarks bar.
5. Open a webpage and click the new bookmark.

If dragging is unavailable, create a bookmark manually and paste [the bookmarklet URL](anti-flash-bookmarklet.txt) into its URL field. Managed browsers may restrict bookmarklets.

## Use

| Control | Action |
| --- | --- |
| Click the bookmark | Toggle Anti-Flash on or off |
| **Manual** | Apply selector-based dark styling without color analysis |
| **Analyze** | Adapt accessible page colors and update as the page changes |
| **Palette** | Choose Tokyo Night, Midnight, or Synthwave |
| **Remove** | Restore the original page appearance |

Reloading also removes the temporary styling. To uninstall Anti-Flash, delete the bookmark.

## Beta status

Chrome/Chromium 153, Firefox 159.0.1, and WebKitGTK 2.52.6 were tested during development. Performance and appearance can vary between pages; some sites work better in Manual mode. Live Palantir Foundry, Safari itself, and installation across Windows/macOS have not been verified.

See [beta notes](BETA.md) for known limitations, and [security guidance](SECURITY.md) before using a bookmarklet in a managed or sensitive browser.

## License and feedback

MIT — [LICENSE](LICENSE). See [attribution](ATTRIBUTION.md).

Report issues or suggestions in [GitHub Issues](https://github.com/itscooleric/anti-flash/issues), without including confidential page content.
