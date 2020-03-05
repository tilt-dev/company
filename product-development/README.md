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

Victor is responsible for ensuring that the backlog of epics is continually full and that epics are increasingly being better defined. There should be no shortage of epics.

## Picking an epic to work on
When a Tilt engineer is free, they should pick a high priority epic to work on and make themself the _sole_ owner of the epic. The engineer should find other folks to collaborate on the epic as needed, but they are the [DRI](https://medium.com/@mmamet/directly-responsible-individuals-f5009f465da4) (directly responsible individual) for driving the epic to completion. There should be at most one owner on any epic, and the owner is the DRI.

The epic may have a fairly broad initial business problem. The engineer(s) should carve out and define a smaller problem, and spec out a solution that can be accomplished within a target of **_7 working days_** (counted from when the epic moves into `In Progress`, more below on states). If the solution cannot be finished within 7 days, keep reducing scope. The epic description should be updated with the smaller scope and acceptance criteria, and the engineer(s) should create additional epics and/or stories to capture the future work.

The purpose of a single epic is _not_ to completely solve a business problem. Rather, completing an epic should likely achieve incremental progress at addressing a single problem, adding incremental user value as a result. In some cases, any realized user value may only appear in future epics. 

After the epic is completed, the engineer should find the next epic to work on, either as a DRI owner, or as a collaborator. Engineers should self-organize and coordinate timelines ad hoc when picking epics. There are no stable teams, no timeboxed sprints, and no synced sprints across teams. Engineers should avoid working on multiple epics concurrently. 

### Epic owner and epic states
- An epic is in one of three states: `Unstarted`, `In Progress`, `Closed`. 
- If an epic is in `In Progress` or `Closed`, it must have exactly one owner, who is the DRI.

### DRI responsibilties and non-responsibilities as epic owner

| | Reponsibilities | Non-responsibilities |
| --- | --- | --- |
| | The DRI is responsible for maintaining the epic state, description, and attached stories updated as the single source of truth of overall work status, at least on a daily basis.<br/><br/>The acceptance criteria sections are _especially critical_, including presenting the problem and final implementation in a company meeting.<br/><br/>This encourages anyone who wants to learn about and collaborate on the epic to visit the epic itself (and it's attached stories) to see the latest updates, allowing the DRI to focus on actual work and leveraging a single place for providing updates. | The DRI is not responsible for communicating epic work status, beyond keeping the epic itself updated as the single source of truth. The DRI is not responsible for sharing work on Slack, meetings, or keeping Tilters otherwise updated. The DRI _can_ provide additional communication, but is not required to do so. Victor will help with broader general communication needs.|


- Driving the epic to completion in a timely fashion within the target **_7 working days_**.
  - The DRI epic owner should consider reducing scope (deferring valuable work to future epics) if additional work is discovered.
- Making decisions quickly amongst multiple 

  - The DRI should exercise judgment to seek collaboration and input from relevant Tilters as they see fit to meet the business goals of the epic. They should not wait too long for a response if the consulted Tilter is not responsive. We are biasing toward shipping in small increments quickly. So even if a sub-optimal change was shipped, this is preferable to _not_ shipping at all, because we want to move quickly with small changes. The risk of doing something very bad is also very small with small changes, freeing up the DRI to have more confidence in their decision making.
  
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
- Link to company meeting, where problem and final implementation were presented
- As a Tilt user, I should be able to experience this change (e.g. know how to use this new feature), after reading this section.

## :white_small_square: Updated docs and blog posts, if applicable
- Links

## :white_small_square: Out of scope, related, and/or future work, if applicable
- Clubhouse story for adding additional new statuses and colors
- We are considering surfacing some of this status information to TiltCloud in real-time. See this Clubhouse story.

## :white_small_square: Follow up customer conversations, if applicable
- Links to or screenshots of customer meetings, Slack conversations, etc.

## :white_small_square: Metrics
- Link to specific metrics and/or charts that this change targets to improve. 
- Many changes will not improve metrics in weeks or even months. That's okay. But still need to mention which specific metrics you are targeting.
- If your change introduces a new metric to measure, collecting that data should be in scope or future work should be captured. For example, if you've created a new feature, you should be tracking it with FWAU / FMAU (feature weekly/monthly active users), and link to that metric here.
- Most changes should be small and thus you should be frequently linking to [engagement metrics](https://github.com/windmilleng/company-private/blob/master/business-report/README.md).
```

Here is an example of how an epic description should look when all the acceptance criteria have been completed.

<img src="images/epic-acceptance-criteria-example.png" height="650" />
