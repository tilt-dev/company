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

## How an Epic Starts

### A Team is Assigned to an Epic

When assigning a team of Tilters to an epic, we're operating on a few hypotheses:

- Projects are far more likely to succeed when the people working on it feel
  connected to the project, and feels it lets them use their skills well.

- Conversely, Tilters should be empowered to try epics they feel strongly about,
  even if other people on the team disagree. Consensus is a bad way to make
  decisions, and we shouldn't require consensus on an idea to move forward.
  
- It's anxiety-producing and not helpful when people are constantly switching
  back and forth between execution and prioritization. We don't want each Tilter
  to have to do a prioritization exercise every week when they finish their epic.

Each Tilter is responsible for reading the backlog of epics. They don't need to
understand every epic. But they should understand enough to be able to
affirmatively articulate what epics in the backlog they want to work on and why.

Every two weeks, Nick will talk to you your impressions of the backlog, and try
to get a sense of what you think is important and want to work on.

Nick will assign you to a team working on an ongoing epic, or a new epic near
the top of the backlog, trying to balance preferences and current priority order.

If there's an epic that's high in priority order but no one wants to work on,
then Nick should dig more into why. Do we need to do more research upfront?  Is
the epic defined incorrectly? Is it misaligned with what we're currently
focusing on?

There may be rare cases where someone gets assigned to an epic that they
don't want to work on, but in those cases we should explicitly call out
that this is happening and why.

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
