# Release Feed Smoke Test

A visual QA release that proves the Mage Pro changelog page updates from public markdown content instead of frontend code changes.

## Highlights

- Publish release notes as markdown without changing the frontend.
- Show new releases automatically from the public manifest.
- Verify the changelog experience with live browser screenshots.

## Release Automation

This entry was added directly to the public `mage-pro-releases` repository. The Mage Cloud frontend reads the manifest, fetches this markdown file, and renders it as the newest release because it has the highest sequence value.

## Customer Communication

The release note copy is intentionally product-focused. It describes what customers can do now, why the update matters, and how teams can use the changelog during upgrades or shared QA.

## Visual QA Checklist

This sample includes markdown structures that should be visible on the release page:

- A top-level title
- Product summary copy
- Highlight bullets
- Multiple sections
- Inline `code`
- A public link to the [Mage Pro release feed](https://github.com/mage-ai/mage-pro-releases)

## Expected Frontend Result

When the frontend refreshes the manifest, this release should appear above `2026.06.10` with the title **Release Feed Smoke Test** and version `2026.06.10-smoke`.
