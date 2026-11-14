# Installation

Install Lessons Learned Hub on a Confluence Cloud site, then verify that its macros and Hub are available.

> **Installation availability:** the publisher has not yet supplied an approved Marketplace listing or installation link. Request the current installation route at **contact@sofrato.com**. This page does not imply the app is already publicly listed.

## Before installation

- Use **Confluence Cloud**. These instructions do not cover Confluence Data Center.
- Ask an administrator authorized to install apps on the target site to perform the installation.
- Review the [Privacy Policy draft](legal/privacy-policy.md), [Terms of Use draft](legal/terms-of-use.md), and [data visibility rules](permissions.md). Obtain the finalized terms from the publisher before production use.
- Decide whether site-wide lesson sharing is suitable for your organization.

Users read the documentation in a browser. They do not need Git, Node.js, Forge CLI, or access to the source code.

## Install

1. Obtain the publisher's official Marketplace listing or Forge installation link.
2. Sign in with the administrator account for your intended site.
3. Follow the installation screen and select the correct **Confluence Cloud site**.
4. Review the requested permissions. The current app reads page information and permissions, page labels, and user profile information needed for its features.
5. Approve the installation according to your organization's process.

The screen and available actions depend on whether the app is distributed through Marketplace or a Forge installation link. See Atlassian's [Forge distribution guide](https://developer.atlassian.com/platform/forge/distribute-your-apps/).

## Verify installation

1. Open Confluence's app navigation and find **Lessons Learned Hub**. The exact navigation location depends on your Confluence interface.
2. Open the Hub. An empty state is expected before anyone adds lessons.
3. Create or edit a test page you are allowed to edit.
4. Open the page editor's macro picker and search for **Add Lessons**.
5. Insert the macro, create a clearly named test project, choose **Save**, and publish or update the page.
6. Follow the [Quick start](quick-start.md) to save a test lesson and verify it appears in the Hub.

**Expected result:** the app opens, a project can be selected, and a saved lesson is visible in both its Add Lessons macro and the Hub.

## Updates

An administrator may need to approve updates that request additional permissions. Follow the update prompt in Atlassian's app management interface, review the permissions, and consult the publisher's release notes. Do not reinstall the app as a routine troubleshooting step.

## Removal

An authorized administrator can uninstall the app through Atlassian's app management interface. Plan any data requirements with your administrator and the publisher first. Removing a macro or deleting a page is not a documented way to erase all application data, and uninstalling does not establish immediate permanent erasure. See [Security and data handling](security-and-data.md).

[Back to documentation](README.md) · [Next: Quick start](quick-start.md)
