# Agent Command Center

A release focused on making agent-driven development, shared QA, and product release communication feel connected from commit to customer-facing changelog.

## Highlights

- Launch isolated cloud agent dev slots from a shared EKS cluster.
- Review Mage Pro changes through a public changelog feed.
- Connect frontend QA directly to linked Mage Pro environments.

## Agent Workflows

Mage Pro now gives engineering teams a clearer path from branch to reviewable environment. Agent dev slots can publish a shared URL, keep the synced source aligned with the current commit, and expose the right environment variables without copying local `.env` files into the pod.

This makes feature review easier for product, design, and customer-facing teams because everyone can open the same build instead of relying on screenshots or local setup instructions.

## Release Communication

Release notes can now be generated into public markdown files and discovered through a simple JSON manifest. The frontend renders the newest entries first, including image tags, highlights, release dates, raw markdown links, and GitHub links when available.

This gives each audience a clearer release story:

- Product teams get feature narratives instead of commit lists.
- Operators get version-aware context before upgrading.
- Engineers get markdown files that are easy to review and automate.

## Cloud QA

Linked cloud slots make cross-repo verification more direct. A cloud frontend slot can point to a matching Mage Pro slot, keeping release pages, OAuth callbacks, and API-backed flows closer to the environment reviewers will actually use.

## Fixes And Polish

- Reduced first-load risk by avoiding server-side release feed fetches.
- Added empty-state handling for unpublished feeds.
- Improved markdown rendering for tables, links, code snippets, and section headings.

Learn more in the [Mage Pro docs](https://docs.mage.ai/).
