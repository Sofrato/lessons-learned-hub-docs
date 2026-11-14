# Reference

Field values, limits, matching rules, and reporting definitions for the current application.

## Lesson fields

| Field | Required to save? | Values or limit |
|---|---|---|
| Title | Yes | Up to 200 characters; whitespace-only titles are rejected |
| Problem description | Yes | Up to 5,000 characters; must contain text |
| Owner | Yes | A selected Atlassian user |
| Root cause | No | Up to 5,000 characters |
| Recommendation | No | Up to 5,000 characters |
| Category | No | Technical, Process, Vendor, Communication, Team, Other |
| Phase | No | Initiation, Planning, Execution, Testing, Deployment, Closure |
| Impact | No | High, Medium, Low |
| Tags | No | Up to 10 unique tags, each up to 50 characters |

Tags are trimmed, lowercased, and repeated whitespace is collapsed. Empty and duplicate tags are removed. For example, `Data Migration` and `data migration` become the same tag.

**Complete** means the saved lesson has root cause, recommendation, category, phase, impact, and at least one tag, as well as the required fields. **Incomplete** means one or more completeness fields are missing.

Author and source page are assigned from the creation context. An owner identifies responsibility and does not confer permission.

## Project and watchlist limits

- Project name: up to **120 characters**, with uniqueness checked after normalizing case and whitespace.
- Project context: up to **10 tags**, up to **50 characters** each; categories from the lesson category list; an optional phase from the phase list. At least one tag, category, or phase must be supplied.
- Watchlist note: up to **1,000 characters**.
- Watchlist status: **Watching**, **Actioned**, or **Dismissed**.
- Review by: an optional valid calendar date. Watching items become Overdue only after that day has passed, using the viewer's local calendar day.

## Discover matching

The match score is:

```text
2 × number of shared tags
+ 1 if the lesson's category is in the project context
+ 1 if the lesson's phase equals the project context phase
```

Scores below **2** are not suggested. Scores **2–3** show Good match; scores **4+** show Strong match. The visual indicator is capped at five dots.

Ties prefer Complete lessons, then impact (High, Medium, Low, unspecified), then newer lessons. The current implementation ranks up to 500 recent matching candidates and returns up to 50 recommendations.

Discover excludes the current project's own lessons, logically deleted lessons, project-specific Not relevant choices, and lessons already on the project's active watchlist.

## Metrics

| Metric | Definition and interpretation |
|---|---|
| Total lessons | Non-deleted lessons added during the selected period, within selected source projects and category |
| Contributing projects | Distinct source projects with at least one qualifying lesson; compared with all registry projects or the selected project set |
| Lessons reused | Distinct lessons first marked Actioned on another project's watchlist during the selected period; project filters apply to the lesson's source project |
| Recurring issue | A tag found in lessons from at least the selected number of distinct projects; threshold 2–5, default 3 |
| Complete lessons | Share of lessons satisfying all completeness fields; not a content approval score |
| Low-coverage projects | Projects below the selected minimum lesson count (3, 5, or 10; default 5); category filters affect the count |
| Oldest open gap | Age in days of the oldest incomplete lesson in scope, regardless of the Statistics period |
| Used by | Projects with a currently non-removed watchlist relationship to the lesson, including the relationship's status |

The first Actioned timestamp is retained when a watchlist item changes status, is removed, or is added again. Historical reuse numbers can therefore remain after those operations; changing status back to Actioned does not create a fresh first-use date for that relationship.

Time-bound reports generally use the selected period and the previous period of equal length. Month-based charts use UTC calendar months; the watchlist Overdue badge uses the viewer's local calendar day. The period labelled Last 12 months uses the application's rolling 365-day filter. See the [Hub guide](guides/hub.md) for sections with different filter behavior.

[Back to documentation](README.md) · [Hub guide](guides/hub.md)
