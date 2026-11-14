# Quick start

Practice the full workflow: save a lesson in one project, discover it in another, and record an action.

## Before you start

The app must be [installed](installation.md). You need permission to create or edit the two practice pages. Use non-sensitive example data: lessons will be visible across your Confluence site. If Atlas or Orion is already a real project, choose distinct practice names for this exercise instead of changing that project's shared data.

## 1. Capture a lesson in Project Atlas

1. Create or edit a Confluence page called **Project Atlas — learning**.
2. Insert the **Add Lessons** macro using the editor's macro picker.
3. In **Project**, enter **Project Atlas** (or your distinct practice name) and choose the option to create it. If you are repeating the exercise, select your existing practice project.
4. Choose **Save**, then publish or update the page.
5. In the macro, choose **Add Lesson**.
6. Enter the following example and select your own account as **Owner**:

| Field | Example |
|---|---|
| Title | Validate vendor API limits before integration testing |
| Problem description | Integration testing stopped when a vendor API rejected a batch of requests. |
| Root cause | The test plan did not account for the vendor's request limits. |
| Recommendation | Confirm limits with the vendor and run a small load test before the main test cycle. |
| Category | Technical |
| Phase | Testing |
| Impact | High |
| Tags | api, testing |

7. Choose **Save lesson**.

**Expected result:** the lesson appears in Project Atlas and is marked **Complete**. The page where it was created is its source page.

## 2. Set up Project Orion

1. On a second page, insert the **Use Lessons** macro.
2. Create or select **Project Orion** and save the macro configuration. Publish or update the page.
3. Open **Discover** and choose **Set project context**. If context is already configured, use **Edit context**.
4. Add the tag **api**, choose category **Technical**, and phase **Testing**.
5. Choose **Save context**.

**Expected result:** the Atlas lesson is eligible for a **Strong match**: one shared tag, the same category, and the same phase. On sites with many lessons, the suggestions list is limited; use the Hub to find a lesson that is not displayed.

## 3. Use the lesson

1. Expand the Atlas lesson in **Discover**.
2. Choose **Add to watchlist**.
3. Open **Watchlist** and expand the lesson.
4. Add a note describing Orion's planned action, select an owner if useful, and set **Review by**. Save the note with **Save** in the note editor.
5. After completing the action, choose **Mark actioned**.

**Expected result:** the watchlist item changes from **Watching** to **Actioned**. The original lesson remains part of Atlas; Orion has recorded its own use of it.

## 4. Find it in the Hub

Open **Lessons Learned Hub** from Confluence's app navigation. In **Lessons**, search for the example title or the tag **api**, then open the lesson. Review **Statistics** and **Data Quality** for broader reporting.

For ongoing use, agree on shared tags and a regular review of your project's watchlist. Remove practice lessons only after checking whether other people are using them; deletion does not mean immediate permanent erasure.

[Back to documentation](README.md) · [Projects and macros](guides/projects-and-macros.md)
