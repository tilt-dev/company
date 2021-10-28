# Product Development

## Workflow

We want a good internal workflow so we can understand our customer pain points, collaborate to solve their problems, and measure the effectiveness of what we release.

<img src="images/workflow.png" height="550" />

The illustration above maps the people, tools, and deliverables in this product development cycle. Ideally, we run a flow where conversations with customers drive an internal process where high-level strategy informs the scoped and defined product changes we ship. And when we ship to customers, we measure impact so we can continue to adjust what we strategize and deliver.

### Github for Community Support

We rely on public Github issues to engage with the Tilt community.

Tilters should encourage all users to create GitHub issues, subscribe to
existing issues, and 👍 them.

The Exterminator should create Github issues for all bugs and
feature requests. For more details, see [the exterminator
policy](../user-support/README.md#exterminator).

By subscribing to an issue, a user will get a notification when it is closed
(possibly informing them that a feature request is now implemented), bringing
them back to Tilt for further product discussion.

### Shortcut for Task Management

We use Shortcut epics to track product changes.

All Tilters are encouraged to collaborate in _discussing_ general ideas. 

Tilters should prefer discussing ideas in Shortcut, linking ideas together, thus building a web of good ideas that are easily searchable for posterity.

### Defining high-level business initiatives

All Tilters are encouraged to collaborate in _raising_ high-level problems. 

There is no strict process. As a high-level problem becomes increasingly clear and known over time, it should have more and more of these components with increasing fidelity:

- Problem statement
- Solution scope
- Attached datapoints with relevant user needs
- Link to specific metrics or user concerns that this change targets to improve

## Workstreams

### Business Need

The product manager takes input from user research, conversations with partners, changes in the industry, and other contributors in the team to synthesize business needs for the product.

This business need is outlined in a general 'workstream status' document—generally an 'Umbrella' epic that will later link to all tasks in the workstream.

A business need outlines a problem, but not necessarily a solution, how to get there, or what the definition-of-done is.

Once there's enough bandwidth a team is assembled to tackle the issue. This starts with with a kickoff meeting.

Misc:
- As a rule of thumb, a contributor should work on only _one_ workstream at a time.
- We are deliberately not concerned with deadlines, but with addressing business needs. (In other words: We work on something until we're happy with it, or we decide to table it. Dates do not matter.)

### DRI

Each workstream is assigned a [DRI](https://medium.com/@mmamet/directly-responsible-individuals-f5009f465da4). The DRI should be one of the direct contributors to the workstream.

The DRI is responsible for:
- Maintaining the umbrella epic's state, description, attached epics and docs updated as the single source of truth of overall work status
- Tracking scope if additional work is discovered
- Tactical implementation decisions
- Assigning contributors to the workstream, in conjunction with the product manager

### Kickoff Meeting

The kickoff meeting involves the following process:
- The product manager and DRI explain the business need, and go over any data that might help painting a clearer picture e.g. metrics, user research
- Contributors brainstorm potential solutions to the problem, and weigh in on any suggested solutions the product manager and DRI might have outlined beforehand. During this process every contributor should touch, whether in a structured manner or not, on the following points:
	- What do you think the team should be working on?
	- What do you think you should be working on?
	- What do you think could go wrong?
	- What is this discussion missing?
- Throughout the discussion topics should be filed as appropriate into the categories: action items, concerns, decisions, tensions
- Then the first practical steps should be outlined:
  - Enough epics should be created to provide adequate workload for every contributor
  - A definition of done should be discussed. If further exploration is still required, the matter should be revisited at the next meeting. This discussion can include:
  	- How do we know we're done with this effort? (What's in and out of scope?)
	- What does a win look like? (How are we measuring success? How can we celebrate it? What does a failure look like?)
    - What specific numerical metrics should we track?

At this point the company should subsidize one (1) free confectionery i.e. donut or bagel per contributor as a celebratory token to kick off the new endeavour. 🍩 (TODO: pending Nick's approval)

After the kickoff meeting the DRI updates the 'workstream status' document to include decisions made in the kickoff meeting, including any of: updated business goal, scope, out-of-scope, definition of done, metrics, concerns, and so on.

Since work units should directly derive from discussions with contributors (i.e. above: "What do you think you should be working on?"), it should be self-evident what each contributor should be working on next.

### Regular Check-Ins

Regularly, at a frequency defined by the group, check-in meetings take place. Regular check-ins serve to:

- Review the work done between then and the previous umbrella meeting, in terms of happy, mixed, and sad feelings
- Update our current understanding of the problem and/or its solutions
- Update the scope and definition of done with new things to do or not to do
- Define next steps so everyone has an appropriate amount of assigned work until the next check in
- All points discussed should be sorted into action items, concerns, decisions, tensions as appropriate
- Optionally, the group may decide to re-do the four-points discussion ("What do you think the team should be working on?" and so on)

After the check-in meeting the DRI updates the 'workstream status' document accordingly.

### Wrap

Once the workstream reaches its conclusion a wrap-up meeting takes place. It's a retro-style review, plus a review of goals achieved, metrics, how this should inform future work, and so on.

The DRI should gather data for a short presentation highlighting metrics, user research, and other forms of impact, to the rest of the team.

### Metrics, User Research, and DevRel

Throughout a workstream, special care should be taken to ensure that every contributor is working towards the same metrics, goals, and user needs; these should be reviewed and reiterated regularly.

During the steps described in the previous sections we should, as appropriate and at varying points of implementing a feature:
- Inform users about the new enhancement, with e.g. blogs or videos
- Measure progress towards the business goal in qualitative terms, via the [user research process](https://github.com/tilt-dev/user-research/)
- Measure progress towards the business goal in quantitative terms, via numerical metrics (process TBD)

The goals for metrics, user research, and DevRel work are multi-faceted. It's important to keep in mind that they simultaneously serve to:

  - Measure impact vs. effort e.g. the team spent a lot of work on a feature, was the ROI worth it?
  - Inform ourselves of which direction to go next that has the largest potential impact for the smallest cost
  - Generate shareable markers of success that we can use to e.g. to tell a user to adopt feature X because it has been successful at this many other teams
  - Gather data we'll need for the next stages of the company e.g. fundraising

## Individual Epics

### Epic Priortity

Once an epic has enough detail that someone can work on it, it should be assigned a date. The date makes it appear on the [roadmap](https://app.Shortcut.io/windmill/epics?state_ids=500008016&state_ids=500000003) chart.

The dates on the roadmap are not intended to be exact. We use them to express rough dependencies and relative ordering between epics.

The CEO and product manager are responsible at a high-level for ensuring that the roadmap is continually populated and that epics are increasingly being better defined. There should be no shortage of epics.

If you have a question or comment about an unstarted epic's scope, design, timeline, priority, or any other aspect, you should direct it at the workstream's DRI and/or at the product manager.

### Starting an Epic

The contributor moves the epic into the `In Progress` state.

### How an Epic Ends

A given epic may have a fairly broad problem. The engineer(s) should carve out and define a smaller problem, and spec out a solution that can be accomplished in between two umbrella check-ins at the most, with a target of **_7 business days_** (counted from when the epic moves into
`In Progress`, more below on states).

### Reducing Scope

If the solution drags beyond the expected time, the contributor and the DRI should reduce scope, break the task down into smaller parts, and create additional epics to capture future work. The epic description with smaller scope and acceptance criteria should be updated accordingly.

They may need to communicate radical changes in scope to other stakeholders; if unsure, reach out to the product manager.

The purpose of a single epic is _not_ to completely solve a given problem. Rather, completing an epic should likely achieve incremental progress at addressing a problem, adding incremental user value as a result. In some cases, any
realized user value may only appear in future epics.

### Presenting the Result

Once an epic is closed, the contributor and/or workstream DRI should present the result at the weekly company meeting.

### Epic description template

When an epic starts, the epic owner should ensure this template is in the epic description.

The "Problem statement and references" section should be completed. (Other sections can remain not yet completed.)

Copy and paste the template below into the epic description. Update each section, with as much applicable content as possible. When a section is done, replace `:white_small_square:` with `:white_check_mark:` to indicate it is done.

```
---

# Acceptance criteria
See [Product Development](https://github.com/tilt-dev/company/blob/master/product-development/README.md) for details.

When a section is done, replace :white_small_square: with :white_check_mark:

## :white_small_square: Problem statement and references
- E.g. Tilt users find it difficult to understand the colors in the Tilt Web UI sidebar
- Links to related [Tilt rollout cookbook recipes](https://docs.tilt.dev/rollout)
- Links to Shortcut/GitHub/Slack/docs

## :white_small_square: Feature discovery and adoption
- How will users discover and adopt this feature? 
- UI change to alert user?
- Assign DevEx engineer in partner team to update Tiltfile?

## :white_small_square: Final scope, implementation, and demo
- E.g. We decided to add tooltips to all the different statuses in the sidebar
- User journey, with links to Figma or screenshots
- Presented (or will present) in [weekly epics meeting](https://github.com/tilt-dev/company/blob/master/product-development/README.md#weekly-epics-meeting)

## :white_small_square: Updated docs and blog posts
- Links

## :white_small_square: Out of scope, related, and/or future work
- Links to Shortcut/GitHub/Slack/docs

## :white_small_square: Customer validation and metrics
- Links to Slack conversations
- Links to customer docs
- Links to customer metrics dashboards
- Links to internal metrics dashboards
- Links to future work to collect data
```
