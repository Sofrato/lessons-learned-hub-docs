# Hub

Open **Lessons Learned Hub** from Confluence's app navigation to search across projects, review patterns, and improve incomplete lessons. The precise navigation location depends on your Confluence interface.

## Lessons

1. Open the **Lessons** tab.
2. Search using **Search lessons, tags, projects**. The search covers titles, problem descriptions, project names, and tags; it is not a full-text search of every field.
3. Optionally choose a category, select a project from a lesson's project name, or switch **Sort** between **Newest** and **Impact**.
4. Choose **Load more** when available to extend the list.
5. Open a lesson to see its detail panel, source page, and **Used by** projects.

Use **Edit** or **Fill in** when available to update a lesson. Editing requires permission on its source page. New lessons are created from Add Lessons macros, not directly from the Hub. Use a project's Add Lessons macro for the documented deletion workflow.

**Used by** lists current watchlist relationships. It should not be interpreted as a list of completed actions: each relationship has its own status.

## Statistics

Use **Period**, **Projects**, and **Category** to set the reporting scope. The default period is **Last 90 days**. The project filter refers to the app's projects, not Confluence spaces.

- **Total lessons** counts lessons added in the selected period and scope.
- **Contributing projects** counts projects with at least one such lesson.
- **Recurring issues** counts tags appearing in lessons from enough distinct projects. Adjust the threshold to change what counts as recurring.
- **Lessons reused** counts distinct lessons with qualifying first Actioned activity in another project. It is not a count of views or every status change.

Charts provide a **View as table** option. Trends compare with the previous period of equal length; **All time** has no trend comparison.

Some sections intentionally use different time or category rules:

- **Lessons over time** shows the last 12 calendar months.
- **Lessons by category** ignores the category filter so that you can compare categories.
- Incomplete lessons in **Needs attention** remain relevant regardless of their creation period.

See [Metric definitions](../reference.md#metrics) before interpreting the numbers.

## Data Quality

1. Open **Data Quality**.
2. Select projects and a category if needed. This tab has no period filter.
3. Review completeness, missing fields, and low-coverage projects.
4. Set the minimum lesson count for coverage: **3**, **5**, or **10**; the default is **5**.
5. In the incomplete lessons list, use **Fill in** where available, complete the missing information, and save the lesson.

The oldest incomplete lessons are listed first. You may see lessons without a Fill in action if you cannot edit their source pages. Ask someone with the relevant permission to complete them.

Project and category filters are shared between Statistics and Data Quality while the Hub remains open. The Lessons tab has its own search and filters.

[Back to documentation](../README.md) · [Reference](../reference.md) · [Troubleshooting](../troubleshooting.md)
