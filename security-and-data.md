# Security and data handling

This page describes the current implementation reviewed on **14 November 2026**. It is a product description, not a certification, a security audit result, or a guarantee about a future release.

## Data used by the app

| Data | Purpose |
|---|---|
| Project names, identifiers, creator, home page, and creation time | Shared project registry and management permissions |
| Lesson text, tags, category, phase, and impact | Capture, search, matching, completeness, and reporting |
| Atlassian account IDs for authors, owners, and recorded changes | Attribution, responsibility, permissions, and activity metadata |
| Profile display names and avatar URLs read from Confluence | Show people in the UI and owner selection |
| Source page and macro identifiers; page titles and links read from Confluence | Connect records to pages and show accessible sources |
| Page labels and project context | Suggest tags and match lessons |
| Watchlist status, shared notes, owner, review date, activity times, removal state, and first Actioned time | Follow-up and historical reuse reporting |
| Project-specific Not relevant choices | Hide unsuitable recommendations for that project |
| Operational diagnostic logs | Diagnose application errors and platform operations |

Names and avatars are retrieved from Confluence for display; the application's schema stores account identifiers rather than a separate persistent profile directory. User-entered text can itself contain personal data, so users should minimize it.

## Hosting and access

The app uses **Atlassian Forge** with **Forge SQL** for structured application records. Atlassian describes Forge SQL as hosted on its infrastructure with a database per app installation. [Forge SQL documentation](https://developer.atlassian.com/platform/forge/storage-reference/sql/)

The reviewed manifest does not declare a remote backend or external egress destinations, and no separate analytics or AI integration was identified in the reviewed application source. This does not mean no data is processed: Forge, Confluence, browser requests for Atlassian-provided resources, platform logs, and support correspondence still involve processing. Support email is a separate channel from app storage.

No claim is made here that storage is limited to the EU, that customer-selected data residency is supported by this release, or that the app has a Runs on Atlassian badge. Obtain confirmed location and supplier information before relying on such assurances.

## Permissions

The current manifest requests:

| Scope | Reason |
|---|---|
| `read:page:confluence` | Page information, page-operation permission checks, and labels |
| `read:content-details:confluence` | User search for owner selection |
| `read:confluence-user` | Current user and names/avatars for account IDs |

Confluence API calls are made as the current user. Write permissions are checked server-side against the relevant page or project creator. **App lesson read access is site-wide**, independently of whether a source page is readable. See [Permissions and visibility](permissions.md).

## Deletion, retention, and recovery

Deleting a lesson marks it deleted; removing a watchlist item marks that relationship removed. These records are not immediately physically erased. First Actioned history is retained for reporting. Removing a macro, deleting a Confluence page, and uninstalling the app are separate operations and should not be used as promises of immediate permanent erasure.

The reviewed app has no general user-facing bulk export, permanent-erasure, or deleted-lesson restore workflow. It also does not establish a complete retention schedule for app records, logs, support messages, and backups. That schedule and the request process must be finalized in the [Privacy Policy draft](legal/privacy-policy.md) before production publication. This documentation does not promise a backup, recovery window, or restoration service.

## Report a concern

Email **[contact@sofrato.com](mailto:contact@sofrato.com)** privately. Include the affected feature and enough sanitized detail to investigate. Do not publish customer data or credentials.

[Back to documentation](README.md) · [Privacy Policy draft](legal/privacy-policy.md) · [Support](support.md)
