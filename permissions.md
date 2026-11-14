# Permissions and visibility

Understand who can see information and which Confluence pages control changes.

## Read access

**Lessons are shared with users of the Confluence site where the app is installed.** Project information and watchlist data are also available through app views. The current app does not provide private projects or lesson-level read restrictions.

A lesson is stored as application data. Restricting its source page does **not** make the lesson private. The app may show **Restricted page** instead of a page title or link when the current user cannot access that page, while continuing to show the lesson itself.

Site-wide means this Confluence site, not the public internet and not every other customer installation. Do not use the app to store information that requires narrower access than its sharing model provides.

## Change permissions

| Action | Who can do it |
|---|---|
| Add a lesson | A user who can edit the page hosting the linked project's Add Lessons macro |
| Edit or complete a lesson | A user who can edit that lesson's source page |
| Delete a lesson | Its author, or a user who can edit its source page |
| Rename a project | Its creator, or a user who can edit the project's home page |
| Change project context | Its creator, or a user who can edit the project's home page |
| Add, change, or remove watchlist items | Its creator, or a user who can edit the project's home page |
| Mark a lesson Not relevant for a project | Its creator, or a user who can edit the project's home page |

**Source page:** the page where a lesson was created.

**Project home page:** the page where the project was created. If no home page is recorded, project management is limited to the creator.

An action can be unavailable if the required page no longer exists or its permissions cannot be verified. An app user does not get a separate write override merely by being a Confluence administrator.

## Common misunderstandings

- **"I am the owner."** Lesson and watchlist ownership identifies responsibility; it does not grant editing rights.
- **"I wrote the lesson."** Authorship permits deletion, but editing still requires source-page edit permission.
- **"I can edit the page containing this macro."** That may allow adding a lesson there. It does not grant permission to edit lessons created on another page or manage a project created elsewhere.
- **"I added the same project to my own page."** Linking a macro to a project does not change the project's management permissions.
- **"I restricted the source page."** That restricts access to the page, not to the lesson stored in the app.

## Request access

For lesson changes, ask the source page owner or your Confluence administrator about page edit access. For project context or watchlist changes, contact the project creator or an editor of its home page.

For privacy or permanent erasure requests, use the [Privacy Policy contact](legal/privacy-policy.md). Deleting a lesson or removing a watchlist item is a logical removal and does not immediately erase all stored records.

[Back to documentation](README.md) · [Security and data handling](security-and-data.md)
