# Watchlist

Use **Use Lessons → Watchlist** to track how your project responds to lessons from other projects.

## Before you start

Add a lesson from [Discover](discover-lessons.md). To change the watchlist, you must have project management permission. Other app users can view its data. The assigned watchlist owner does not receive additional permissions.

## Record your planned response

1. Open **Watchlist** and expand the lesson.
2. Enter a project-specific note, for example: "Confirm the vendor limit before booking the load test."
3. Choose **Save** in the note editor. Notes can contain up to **1,000 characters**.
4. Select a watchlist **Owner** if appropriate. This can be different from the lesson owner.
5. Set **Review by** if you want a review date; use **Clear** to remove it.

Owner and valid date changes save when selected. Wait for completion and resolve any error displayed next to the field before leaving. Although the interface labels the note **My note**, it belongs to the project's shared watchlist, not a private personal notebook. A review date is a tracking field; the current app does not provide reminder emails or scheduled notifications.

## Update status

| Status | Use it when | Available next actions |
|---|---|---|
| Watching | Your team is monitoring the lesson or has work to do | **Mark actioned**, **Dismiss** |
| Actioned | Your team has taken the relevant action | **Back to watching** |
| Dismissed | Your team decided not to pursue it | **Back to watching** |

To move from Actioned to Dismissed, or the reverse, first choose **Back to watching**. Dismissing an item keeps it on the watchlist; it does not mark it Not relevant in Discover.

**Overdue** means an item is Watching and its Review by date is earlier than today's local calendar date. An item due today is not overdue. An Actioned or Dismissed item does not show as overdue merely because its review date has passed.

## Organize the view

Use **By status**, **By project phase**, or **By category**. The initial Use Lessons view opens Watchlist when there are active watchlist items, otherwise Discover.

## Remove and undo

1. Expand the item and choose **Remove from watchlist**.
2. Use **Undo** in the confirmation message to restore that item with its existing fields.

Removing an item does not delete the original lesson. If you later add it again from Discover, the current implementation starts a fresh watchlist entry while keeping the first Actioned timestamp used for reporting. Do not rely on re-adding it to recover its old note, owner, review date, or status.

An item once marked Actioned may still contribute to historical reuse metrics after it is removed or returned to Watching. Removal is logical and is not permanent erasure.

[Back to documentation](../README.md) · [Permissions](../permissions.md) · [Next: Hub](hub.md)
