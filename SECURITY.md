# Security and privacy

Anti-Flash is a browser bookmarklet. It runs within the active page, not in a separate sandboxed browser extension. Only install and execute code you trust and that your browser or workplace policy permits.

## Scope and data

- Manual mode applies temporary CSS to a page. Auto mode analyzes accessible style rules and sampled computed colors **only after** you explicitly click **Analyze**.
- The bookmarklet does not intentionally send telemetry, make network requests, retain site content, read credentials for its own use, or modify website records and forms. It has no remote service or runtime account.
- The browser still executes it as page JavaScript; this is a meaningful trust boundary. Review the generated code if you will run it on sensitive sites.
- Cross-origin stylesheets, restricted frames and managed-browser settings are not circumvented.
- **Remove** and reload restore original page presentation in supported tests. Check the original styling of critical alerts, warnings and operational status labels before relying on recolored meanings.

## Beta limitations

The public beta was tested in desktop Chromium/Chrome and Firefox, plus WebKitGTK as an engine. The exact build has not been validated on live Palantir Foundry or every browser/OS combination, and known large-page performance and CSS edge cases remain. Consult [BETA.md](BETA.md).

## Reporting security concerns

Use GitHub's private vulnerability reporting feature if enabled, or contact the maintainer privately by an existing trusted route. Do not place exploit details, confidential screenshots, private page HTML, credentials or customer data in public issues.

## License

Distributed under the [MIT license](LICENSE), including its AS-IS warranty and liability disclaimer. This license does not eliminate all legal or operational risk.
