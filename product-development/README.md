# _**The content in this page applies starting on 2020 March 30**_
There are no changes to how we work with Google docs and Clubhouse stories prior to this date.

# Product Development

## Workflow
We have a lightweight product develoment workflow that empowers individual Tilters to collaboratively solve business problems, work directly with customers, and to be accountable for achieving positive business outcomes.

<img src="images/workflow.png" height="300" />

The workflow is summarized in the image above. At the far left, we continually have conversations with customers and the community. These are synthesized into GitHub issues and Clubhouse stories. Based on this feedback and our broader company goals and strategy, we maintain a backlog of high-level initiatives as Clubhouse epics (primarily product changes). Over time, epics are further defined with scoped work and acceptance criteria, as they are eventually implemented and shipped.

### Free-form discussion in Clubhouse stories
All Tilters are encouraged to collaborate in _discussing_ general ideas in a free-form fashion, with no strict process, no structure, no specific timelines, and no specific implementation commitments. Tilters should prefer discussing ideas in Clubhouse stories, linking ideas together, thus building a web of good ideas that are easily searchable for posterity.

### Defining high-level business initiatives with Clubhouse epics
All Tilters are encouraged to collaborate in _definining_ high-level business initiatives. Similar to general ideas, there is no strict process for collaboration, except that each business initiative should be documented as a Clubhouse epic. As an epic becomes increasingly well-defined over time, it should have more and more of these components with increasing fidelity:
- Problem statement
- Solution scope
- Attached stories with relevant ideas, including designs

Victor is responsible for ensuring that the [backlog of unstarted epics](https://app.clubhouse.io/windmill/epics?state_ids=500008016&state_ids=500008001) is continually full and that epics are increasingly being better defined. There should be no shortage of epics. Dan B and Nick and Victor are responsible for maintaining the priority of the backlog (higher priority toward the top in the Clubhouse view, when the triangle is pointing down).

Anyone advocating for an epic's priority (or priorities in general) should @-mention Victor in an epic and/or raise a discussion in the [weekly epics meeting](https://github.com/windmilleng/company/blob/master/product-development/README.md#weekly-epics-meeting).

<img src="images/epics-priority.png" height="100" />

## Picking an epic to work on
When a Tilt engineer is free, they should pick a high priority unstarted epic to work on, or join another engineer (or engineers) already working on an `In Progress` epic. Engineers should self-organize and coordinate timelines ad hoc when picking epics. There are no stable teams, no timeboxed sprints, and no synced sprints across teams. Engineers should consider:
- Working in at least pairs on a given epic, to better facilitate product and code collaboration, avoiding working in siloes.
- Not working on too many epics concurrently, in order to focus on a smaller number of tasks to reduce context-switching.

When work has started on an epic, it is moved into the `In Progress` state and a single owner is assigned to it. That is, `In Progress` epic must have exactly one owner. That owner is the [DRI](https://medium.com/@mmamet/directly-responsible-individuals-f5009f465da4) for the epic, who is responsible for driving the epic to completion. An engineer should be the DRI of at most one `In Progress` epic at any given time.

## Picking a high priority unstarted epic
When picking a high priority unstarted epic, look at the first few epics at the top of the [backlog](https://app.clubhouse.io/windmill/epics?state_ids=500008016&state_ids=500008001) and choose a sensible one based on at least these example scenarios:
- My skill set is better suited for the third highest priority epic, so I'll pick that one, and save the first two for other folks who can finish them more quickly.
- The fourth highest priority epic looks to be small so I'll pick that one first and finish it as a quick win before the end of the week.
- My teammate has expertise in the highest priority epic and I'd like to collaborate and learn from them. But they aren't free just yet. I'll work on the third highest priority epic for now and plan to come back to pair with my teammate next week.

## Reducing scope
A given epic may have a fairly broad initial business problem. The engineer(s) should carve out and define a smaller problem, and spec out a solution that can be accomplished within a target of **_7 business days_** (counted from when the epic moves into `In Progress`, more below on states). If the solution cannot be finished within 7 business days, keep reducing scope. The epic description should be updated with the smaller scope and acceptance criteria, and the engineer(s) should create additional epics and/or stories to capture the future work. Alternatively, the engineer(s) may create a separate epic with the smaller scope and start work on that one instead (putting the original epic back into the backlog).

The purpose of a single epic is _not_ to completely solve a business problem. Rather, completing an epic should likely achieve incremental progress at addressing a single problem, adding incremental user value as a result. In some cases, any realized user value may only appear in future epics. 

### Epic owner and epic states
- An epic is in one of three states: `Unstarted`, `In Progress`, `Closed`. 
- If an epic is in `In Progress` or `Closed`, it must have exactly one owner, who is the DRI.

### DRI responsibilties
- The DRI is responsible for maintaining the epic state, description, and attached stories updated as the single source of truth of overall work status, at least on a daily basis.
- The acceptance criteria sections are _especially critical_, including presenting the problem and final implementation in a company meeting.
- The DRI is responsible for reducing scope if additional work is discovered.
- The DRI is responsible for driving the epic to completion.
  
### Example
For example, suppose usability research suggests that the Tilt Web UI right sidebar is difficult for users to learn. Two engineers develop some ideas to iterate on the existing designs in order to address the problems. But they discover that it's a better idea to first re-architect some of the frontend JavaScript and CSS to accommodate the design changes, repaying some previously incurred tech debt. In this case, the first epic's scope would simply be non-user facing code re-architecture work, that doesn't have immediate user impact, but contributes to solving the usability problem indirectly as an incremental first step. The engineers may work on the second epic right after the first one is done, or it may be given to another team, or simply deferred to a future time. By scoping work to smaller units, Tilt is more flexible in prioritizing whatever is best at (almost) any moment of time as a small organization.

### Finishing an epic with acceptance criteria
For an epic to be completed (and marked as `Closed` in Clubhouse), the epic description needs to have all the following acceptance criteria marked as completed. Copy and paste the template below into the epic description, and update it accordingly. When a section is done, replace `:white_small_square:` with `:white_check_mark:` to indicate it is done (or explain why the section is not applicable).

```
# Acceptance criteria
See [Product Development](https://github.com/windmilleng/company-private/blob/master/product-development/README.md) for details.

## :white_small_square: Problem statement and references
- Tilt users find it difficult to understand the colors in the Tilt Web UI sidebar.
- See the customer conversations here:
  - Google doc
  - Slack conversation
  - Clubhouse story

## :white_small_square: Solution scope, final implementation, and demo
- We decided to add tooltips to all the different statuses in the sidebar.
- Screenshots, gifs, or video
- Link to [weekly epics meeting](https://github.com/windmilleng/company/blob/master/product-development/README.md#weekly-epics-meeting), where problem and final implementation were presented
- As a Tilt user, I should be able to experience this change (e.g. know how to use this new feature), after reading this section.

## :white_small_square: Updated docs and blog posts, if applicable
- Links

## :white_small_square: Out of scope, related, and/or future work, if applicable
- Clubhouse story for adding additional new statuses and colors
- We are considering surfacing some of this status information to TiltCloud in real-time. See this Clubhouse story.

## :white_small_square: Follow up customer conversations, if applicable
- Customer feedback on the change introduced
- Links to or screenshots of customer meetings, Slack conversations, etc.

## :white_small_square: Metrics
- Link to specific metrics and/or charts that this change targets to improve. 
- Many changes will not improve metrics in weeks or even months. That's okay. But still need to mention which specific metrics you are targeting.
- If your change introduces a new metric to measure, collecting that data should be in scope or future work should be captured. For example, if you've created a new feature, you should be tracking it with FWAU / FMAU (feature weekly/monthly active users), and link to that metric here.
- Most changes should be small and thus you should be frequently linking to [engagement metrics](https://github.com/windmilleng/company-private/blob/master/business-report/README.md).
```

Here is an example of how an epic description should look when all the acceptance criteria have been completed.

<img src="images/epic-acceptance-criteria-example.png" height="650" />

### Weekly epics meeting

There is a weekly meeting for discussing epics where all Tilters are optionally invited. Each meeting will be recorded (with permission from participants) and shared internally for all Tilters to watch if they want, [listed here](https://docs.google.com/document/d/173tL_bu4hs73VXo5kHxU0rDSXFlmKS-gpMJokpcdWE0/edit). Tilters should add agenda topics per the following categories, preferably prior to the meeting starting. If there are no agenda topics, the meeting is cancelled for that week.

Agenda topics include:
- DRI links to and presents their epic, including problem and final implementation, preferably with a demo. (This presentation is part of an epic's [acceptance criteria](#finishing-an-epic-with-acceptance criteria)
- Victor presents epics (new or otherwise) that have recently moved to high priority.
- Somebody advocates for an epic to be high priority or otherwise discusses epic priorities.
