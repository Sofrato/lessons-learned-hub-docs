# Projects and macros

Connect Confluence pages to the same project so teams share lessons and a watchlist.

## Create or select a project

1. Edit a page where you can insert a macro.
2. Insert **Add Lessons** or **Use Lessons**.
3. In the configuration dialog, search for the project in **Project**.
4. Select an existing result, or use **Create project "…"** for a genuinely new project.
5. If a similar project is suggested, check it before confirming a new name. Choose the suggested project if it is the same initiative.
6. Choose **Save** and publish or update the page.

**Expected result:** the macro displays the selected project's name and its shared data.

Project names can contain up to **120 characters**. Leading and trailing whitespace is removed, repeated spaces are collapsed, and names differing only in capitalization or spacing are treated as the same name.

## Add the other macro or another page

Insert the required macro and **select the existing project**. You can use Add Lessons and Use Lessons on the same page or on different pages.

Selecting the same project links to the same records. It does not create a copy. Editing a shared project or lesson can therefore affect what appears on several pages; refresh another open page to see the current data.

## Change a macro's project

Edit the Confluence page, select the macro, open its configuration with the editor's macro edit action, and select the intended project. Save the configuration and update the page.

Changing this link changes which project's data the macro shows. It does not move existing lessons to another project.

## Understand the project home page

The page on which a project is created becomes its **home page**. The creator and people who can edit that page can manage the project's name, context, watchlist, and Not relevant choices.

If a project has no recorded home page, only its creator can manage it. Adding the project to a different editable page does not grant project management rights. Selecting someone as a lesson or watchlist owner does not grant additional permissions.

## Rename a project

1. Open the Hub's **Lessons** tab.
2. Select a project's name from a lesson to filter the list to that project.
3. If you have project management permission, choose **Rename project**.
4. Enter the name and choose **Rename**.

The project keeps its identity and linked records. Refresh macros on other pages to see the new name.

## Remove a macro

Remove it using the Confluence editor and update the page. This removes the macro from that page; it is not a project deletion or application data erasure operation. The current documented interface does not provide a general delete-project or merge-projects workflow.

[Back to documentation](../README.md) · [Permissions](../permissions.md) · [Next: Add Lessons](add-lessons.md)
