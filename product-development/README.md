# Product Development

## Workflow
We have a lightweight product develoment workflow that empowers teams to solve business problems, working directly with customers, and to be accountable for achieving positive business outcomes.

<img src="images/workflow.png" height="300" />

The workflow is summarized in the image above. At the far left, we continually have conversations with customers and the community. These are synthesized into GitHub issues. Based on this feedback and our broader company goals and strategy, we maintain a backlog of high-level initiatives as Clubhouse epics (primarily product changes). Over time, epics are further defined with scoped work and success criteria, as they are eventually implemented and shipped.

### Defining high-level business initiatives (Epics)
All Tilters are encouraged to collaborate in defining high-level business initiatives (Clubhouse epics) over time. This is an ongoing task with no specific timelines. Victor is responsible for ensuring that the backlog of epics is continually full. There should be no shortage of epics.

### Incrementally solving business problems
When a Tilt engineer is free, they should pick a high priority epic to work on. They may consider finding another engineer to work as a two-person team.

The epic may have a fairly broad initial business problem. The team should carve out and define a smaller problem, and spec out a solution that can be accomplished within **2 weeks**. The epic description should be updated with the smaller scope and success criteria, and the team should create additional epics to capture the future work.

The purpose of a single epic is **not** to completely solve a business problem. Rather, completing an epic should likely achieve incremental progress at addressing a single problem, adding incremental user value as a result. In some cases, any realized user value may only appear in future epics. 

After the epic is completed, the team is disbanded, and individuals should find the next epic to work on, with the next team. Engineers should self-organize and coordinate timelines ad hoc when picking epics. There are no stable teams and no timeboxed sprints and no synced sprints across teams. Engineers should avoid working on multiple epics concurrently. 

### Example
For example, suppose usability research suggests that the Tilt Web UI right sidebar is difficult for users to learn. A team develops some ideas to iterate on the existing designs in order to address the problems. But they discover that it's a better idea to first re-architect some of the frontend JavaScript and CSS to accommodate the design changes, repaying some previously incurred tech debt. In this case, the first epic's scope would simply be non-user facing code re-architecture work, that doesn't have immediate user impact, but contributes to solving the usability problem indirectly as an incremental first step. The team may work on the second epic right after the first one is done, or it may be given to another team, or simply deferred to a future time. By scoping work to smaller units, Tilt is more flexible in prioritizing whatever is best at (almost) any moment of time as a small organization.

### Finishing an epic with acceptance criteria
For an epic to be completed (and marked as such in Clubhouse), the epic description needs to contain the following as acceptance criteria. Copy and paste the template below into the epic description, and update it accordingly. Mark a section as done by checking the checkbox.

```
## Problem statement and references
- [ ] Section done
- Tilt users find it difficult to understand the colors in the Tilt Web UI sidebar.
- See the customer conversations here:
  - Google doc
  - Slack conversation
  - Clubhouse story

## Solution scope, final implementation, and demo
- [ ] Section done
- We decided to add tooltips to all the different statuses in the sidebar.
- Screenshots, gifs, or video
- Link to company meeting, where problem and implementation were presented
- As a Tilt user, I should be able to experience this change (e.g. know how to use this new feature), after reading this section.

## Updated docs and blog posts, if applicable
- [ ] Section done
- Links

## Out of scope, related, and/or future work, if applicable
- [ ] Section done
- Clubhouse story for adding additional new statuses and colors
- We are considering surfacing some of this status information to TiltCloud in real-time. See this Clubhouse story.

## Follow up customer conversations, if applicable
- [ ] Section done
- Links to or screenshots of customer meetings, Slack conversations, etc.

## Metrics
- [ ] Section done
- Link to specific metrics and/or charts that this change targets to improve. 
- Many changes will not improve metrics in weeks or even months. That's okay. But still need to mention which specific metrics you are targeting.
- If your change introduces a new metric to measure, collecting that data should be in scope or future work should be captured. For example, if you've created a new feature, you should be tracking it with FWAU / FMAU (feature weekly/monthly active users), and link to that metric here.
- Most changes should be small and thus you should be frequently linking to the [engagement metrics](https://github.com/windmilleng/company-private/blob/master/metrics/README.md).
```
