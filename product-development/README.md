# Product Development

TODO(L): This documents needs to be reviewed for consistency.

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

### Clubhouse for Task Management

We use Clubhouse stories and epics to track product changes.

All Tilters are encouraged to collaborate in _discussing_ general ideas. 

Tilters should prefer discussing ideas in Clubhouse stories, linking ideas together, thus building a web of good ideas that are easily searchable for posterity.

### Defining high-level business initiatives with Clubhouse epics

All Tilters are encouraged to collaborate in _definining_ high-level problems. 

There is no strict process for collaboration. As an epic becomes increasingly well-defined over time, it should have more and more of these components with increasing fidelity:

- Problem statement
- Solution scope
- Attached stories with relevant ideas, including designs
- Link to specific metrics and/or charts that this change targets to improve

## Before an Epic Starts

### Epic Priortity

Each week, L, Nick, and Dan review the
[roadmap](https://app.clubhouse.io/windmill/epics?state_ids=500008016&state_ids=500000003).

Once an epic has enough detail that we think someone can work on it, we assign
it a date. The date makes it appear on the roadmap chart.

The dates on the roadmap are not intended to be exact. We use them to express rough dependencies
and relative ordering between epics.

L is responsible for ensuring that the roadmap is continually full and that
epics are increasingly being better defined. There should be no shortage of
epics.

If you have a question or comment about an unstarted epic's scope, design,
timeline, priority, or any other aspect, you should direct it at L.

<img src="images/epics-priority.png" height="100" />

### Epic description template

When an epic starts, the epic owner should ensure this template is in the epic
description.

The "Problem statement and references" section should be completed. (Other
sections can remain not yet completed.)

Copy and paste the template below into the epic description. Update each section, with as much applicable content as possible. When a section is done, replace `:white_small_square:` with `:white_check_mark:` to indicate it is done.

```
---

# Acceptance criteria
See [Product Development](https://github.com/tilt-dev/company/blob/master/product-development/README.md) for details.

When a section is done, replace :white_small_square: with :white_check_mark:

## :white_small_square: Problem statement and references
- E.g. Tilt users find it difficult to understand the colors in the Tilt Web UI sidebar
- Links to related [Tilt rollout cookbook recipes](https://docs.tilt.dev/rollout)
- Links to Clubhouse/GitHub/Slack/docs

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
- Links to Clubhouse/GitHub/Slack/docs

## :white_small_square: Customer validation and metrics
- Links to Slack conversations
- Links to customer docs
- Links to customer metrics dashboards
- Links to internal metrics dashboards
- Links to future work to collect data
```

## Workstreams

### Process

The product manager takes input from user research, conversations with partners, changes in the industry, and other contributors in the team to synthesize business needs for the product.

This business need is outlined in a general 'workstream status' document. A business need outlines a goal, but not necessarily how to get there, or what the definition-of-done is.

Once there's enough bandwidth a team is assembled to tackle the issue. This starts with a kickoff meeting.

The kickoff meeting involves the following process:
- The product manager explains the business need
- Contributors outline their thoughts in the following structure:
	- "What do you think the team should be working on?"
	- "What do you think you should be working on?"
	- "What do you think could go wrong?"
	- "What is this discussion missing?"
- Once these are outlined they are first reviewed to triage things that might be out of scope of the business need, or concerns that might be off topic
- Then every contributor goes over their points, and these are sorted into work units or concerns as appropriate
- As part of the discussion, taking into account available bandwidth and what a minimum viable deliverable should be, the team should define:
	- How do we know we're done with this effort? (What's in and out of scope?)
	- What does a win look like? (How are we measuring success? How can we celebrate it? What does a failure look like?)

After the kickoff meeting the project manager updates the 'workstream status' document to include the decisions made in the kickoff meeting, including any of: updated business goal, scope, out-of-scope, definition of done, metrics, concerns, and so on. The project manager then organizes the work units and assigns contributors to them, and work begins.

Regularly, at a frequency defined by the group in question, 'retro-planning' meetings take place. During these, the work that has already taken place is reviewed in terms of happy, mixed, and sad feelings, any tensions are discussed, and any new ideas stemming from these are then integrated into the workstream status document.

Once the workstream reaches its conclusion a wrap up meeting takes place. It contains the retro element from the retro-planning meeting, plus a review of goals achieved, metrics, how this should inform future work, and so on.

Misc:
- As a rule of thumb, a contributor should work on only -one- workstream at a time.
- We are deliberately not concerned with deadlines, but with addressing business concerns. (In other words: we work on something until we're happy with it (or we decide to table it), and dates do not matter.)

### DRIs 

Each epic's assigned team has a [DRI](https://medium.com/@mmamet/directly-responsible-individuals-f5009f465da4), 
set by Nick.

The DRI is responsible for:
- maintaining the epic state, description, and attached stories updated as the single source of truth of overall work status
- reducing scope if additional work is discovered
- driving the epic to completion

### Specify Epic Team Members

Each in progress epic has team members, specified by whoever is an owner
of the Clubhouse epic. (A Clubhouse epic can have multiple owners). The DRI
of the epic is specified in the epic description.

Nick is responsible for maintaining team membership in each in progress epic.

### Starting an Epic

The DRI moves the epic into the `In Progress` state.

### How an Epic Ends

A given epic may have a fairly broad problem. The engineer(s) should carve out
and define a smaller problem, and spec out a solution that can be accomplished
within a target of **_7 business days_** (counted from when the epic moves into
`In Progress`, more below on states).

### Reducing Scope

If the solution drags beyond the expected time, keep reducing scope.

The DRI should update the epic description with smaller scope and acceptance
criteria. They may need to communicate radical changes in scope to other
stakeholders, but it's ultimately the DRI's call. If the DRI isn't sure what to
cut, they should reach out to L for help.

The DRI may create additional epics and/or stories to capture the future
work. Alternatively, they may create a separate epic with the smaller scope and
start work on that one instead (putting the original epic back into the
backlog).

The purpose of a single epic is _not_ to completely solve the problem. Rather,
completing an epic should likely achieve incremental progress at addressing a
single problem, adding incremental user value as a result. In some cases, any
realized user value may only appear in future epics.

### Presenting the Result

Once an epic is closed, the DRI should present the result at the weekly company
meeting.
