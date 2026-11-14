# Troubleshooting and FAQ

Start by refreshing the page and checking the selected project and filters. Avoid uninstalling the app as a first troubleshooting step.

## The app or macros are missing

Ask a site administrator to confirm installation on the correct Confluence Cloud site. Search the macro picker for **Add Lessons** or **Use Lessons**, and check Confluence's app navigation for **Lessons Learned Hub**. A source-code repository or documentation link is not an app installation.

## A macro asks me to select a project

Edit the page and the macro's configuration, choose an existing project or create one, save, and publish or update the page. Use the same existing project when connecting another page to shared data.

## Add Lesson, Edit, or Fill in is missing

Check [Permissions](permissions.md). Adding requires edit permission on the calling macro's page. Editing an existing lesson requires edit permission on its source page. Assigned ownership alone does not grant access.

## I can read lessons but cannot change context or the watchlist

Project management belongs to the creator and editors of the project's home page. Having edit access to a different page with the same project's macro is insufficient. Ask the creator or your Confluence administrator about the home page's permissions.

## Discover shows no suggestions

Check that context is set and can reach a match score of at least 2. One shared tag is enough; a category alone or a phase alone is not. Suggestions come from other projects and exclude lessons on this project's watchlist or marked Not relevant. Use the Hub to search outside the limited recommendation list.

## A lesson disappeared from Discover

Check the project's Watchlist. Adding a lesson there removes it from Discover. Someone with project management permission may also have marked it Not relevant, changed context, or the original lesson may have been edited or deleted. Not relevant is a shared project choice; only the immediate confirmation offers Undo in the current interface.

## A source shows Restricted page

The page may be restricted, unavailable, or deleted. Ask a Confluence administrator if you need access. The lesson can remain readable because app lessons have site-wide visibility independently of source-page restrictions.

## Owner search returns no matching person

Enter at least **two characters** of the person's name. Search results depend on the Confluence users available to you. **Unknown user** can appear when Confluence no longer returns a profile or cannot provide it. It does not by itself prove that the lesson was deleted.

## Saving reports a validation error

Check required title, problem description, and owner fields, field lengths, and valid selections. Notes are limited to 1,000 characters; a review date must be a real calendar date. See [Reference](reference.md).

## The same project looks different on two open pages

Confirm both macros link to the same project and refresh the other page. App views do not promise live synchronization across already open browser tabs. Similar project names can refer to different records.

## Reports do not match my expectation

Check period, project, category, recurring threshold, and minimum coverage settings. Data Quality has no period filter. Reuse records first Actioned history, not every status change or page view. Removed watchlist items can still contribute to historical reuse. See [Metrics](reference.md#metrics).

## A new installation shows empty data or a write fails

An empty Hub is normal before the first lesson. The database may also still be initializing after an installation or update. Refresh and try again after a short interval. If writing continues to fail, ask the administrator to confirm the app is current and contact support. Do not repeatedly uninstall and reinstall.

## Can I export, restore, or permanently erase records?

The current documented interface does not provide a general bulk export, deleted-lesson restore, or permanent-erasure workflow. Watchlist removal has its own immediate Undo action. Contact support for data requests; do not treat app deletion actions as permanent erasure.

## How do I report a problem?

Email **contact@sofrato.com** with the app area, steps, expected result, actual result, and time of the issue. Include a sanitized screenshot if useful. Do not put private lessons, personal data, credentials, or unredacted logs into public GitHub issues. See [Support](support.md).

[Back to documentation](README.md) · [Support](support.md)
