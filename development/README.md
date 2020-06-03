# Development

## Bugs

### Definition
We define a bug as any experience that breaks the _intended_ functionality of a user experience in [Tilt](https://docs.tilt.dev/), including [Tilt Cloud](https://cloud.tilt.dev/). In particular, we may have shipped a feature that failed to meet a certain user's expectation, but that may not necessarily qualify as a bug. In this case, we should nonetheless track the user problem as a non-bug to improve Tilt.

We should express our intentions through [documentating Tilt functionality](https://docs.tilt.dev/) exhaustively, to better support users and manage their expectations.

Non-user facing problems are not classified as bugs.

### All bugs
All known open bugs should be listed in the [Bugs Clubhouse space](https://app.clubhouse.io/windmill/stories/space/4729/bugs). Some bugs are also listed in [GitHub issues](https://github.com/windmilleng/tilt/labels/bug). But these should be a subset of the entire set of open bugs in the Clubhouse space.

### Fix a bug at any time
We believe in shipping a quality experience for both Tilt and Tilt Cloud. So Tilters are encouraged to use their own judgment in picking up a bug to fix at anytime, if they think it's the best use of their time at that moment, ahead of other priorities. Nobody should ever need permission to fix a bug.

### Exterminator assigns bugs
The [Exterminator](../user-support/README.md#exterminator) is responsible for triaging user support requests, including bugs. The Exterminator may fix a bug themself, or assign another Tilter to fix it, coordinating appropriate people and circumstances.

### Assign yourself a bug
Tilters should regularly assign bugs for themselves to fix. A good rule of thumb is to fix two bugs after you have finished working on an [epic](../product-development/README.md#picking-an-epic-to-work-on) (whether as the DRI or a collaborator), before moving on to the next epic.

### Pick a high priority bug
When picking a bug to work on, Tilters are encouraged to pick a high priority bug that they can finish in a sensible time period for that bug. The [Bugs Clubhouse space](https://app.clubhouse.io/windmill/stories/space/4729/bugs) has higher priority bugs toward the top of columns. 
If a bug cannot be fixed within a day or two, consider creating a more thorough plan (possibly [creating an epic to track it](../product-development/README.md#defining-high-level-business-initiatives-with-clubhouse-epics)) and consulting with other Tilters, before beginning the work.

### Close associated GitHub issue
If the bug you have fixed is logged as a GitHub issue (in addition to being logged as a Clubhouse story, which it should already have been), be sure to close the GitHub issue, preferably with a link to the pull request fix, helping inform external users that the bug has now been fixed.

## Metrics
Extracting data from Clubhouse (by [exporting all stories](https://help.clubhouse.io/hc/en-us/articles/360021168791-CSV-Export) from the single project we use), we track the number of bugs created, number of bugs closed, and the total number of open bugs, over time. Note that open bugs is impacted by bugs created, bugs closed, non-bugs being converted to bugs, and bugs being converted to non-bugs. So the week over week change of open bugs is not only impacted by bugs created and bugs closed.

See charts and data in the [Google sheet](https://docs.google.com/spreadsheets/d/13L7Yg4x5lDCwevwVbzNJjMW_sLQxBZj73CuFlC_vkV8/).

## Code Review

Code review is higher priority than writing code. Don’t review details if
high-level changes are needed.

PR titles should start with the prefix of the code they modify.

Helpful links that explain how we like to think  about code review:
https://kickstarter.engineering/a-guide-to-mindful-communication-in-code-reviews-48aab5282e5e

We strive to ship small diffs. An ideal pull request is just a couple dozen
lines, and no more than a couple hundred. The reasons are: 

- Small diffs are easier to reason about 

- Code isn’t proven correct until our users are running it, so no point in being
precious about it

## Spec Review

Specs are committed to github (e.g., [tilt
specs](https://github.com/tilt-dev/tilt.specs) and reviewed via GitHub PRs.

When creating and/or picking up a spec story, make sure you’ve considered the
appropriate review audience.
