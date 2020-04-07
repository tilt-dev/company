# User Support

## Exterminator

Every week, we name an “exterminator” to own user support triage. They triage
and assign bugs, monitor support channels, and manage releases.

### SLA

First response within 3 hours (during business time):

- [Github - Tilt Issues](https://github.com/windmilleng/tilt/issues)

- [Kubernetes Slack - #tilt channel](https://kubernetes.slack.com/messages/CESBL84MV/)

Within a day:

- Email inbox [hi@tilt.dev](https://groups.google.com/a/tilt.dev/forum/#!forum/hi)

- DMs or Mentions to [@tilt_dev](https://twitter.com/tilt_dev)

### Support Tracking

When users request support, they may be reporting a bug, requesting a feature, asking
for docs/examples, or vaguely describing a general problem that they're having
trouble solving with Tilt.

These user support requests may lead to work that we need to track.

We have two systems for tracking this work:

- GitHub issues for all public, user-reported issues

- Clubhouse for internal tracking and prioritization

GitHub issues that we are actively working on should be tracked in
Clubhouse. The reverse is not true - we have internal work
that is not expressed in GitHub issues.

### Support Triage

When a user reports an issue, the Exterminator should ensure there's a Github issue.

The exterminator should confirm with the user that the issue write-up accurately
expresses their problem, and ask them to +1 it or comment with additional context.

We use these votes and comments to decide which issues to prioritize. That
_doesn't_ mean "the issue with the most votes wins". It's just one variable we
use in prioritization.

The exterminator should assign labels to the ticket that match our current
work-tracking best practices. Issues with a bug label are automatically added to
the [Tilt bug triage](https://github.com/orgs/windmilleng/projects/2).

Any interesting new users should be mentioned in #triage-customers. The
exterminator should use their best judgment on who is promising enough to DM
directly (based on a combination of research on their background and how active
they are in the channel).

### Internal Support Triage

When a Tilter has a problem with Tilt, they should report it in the #triage-bugs Slack
channel.

The exterminator should determine whether the problem belongs in Github Issues or
Clubhouse, based on whether users have noticed and who it affects, and file it
in the appropriate place.

### Request Priority

The exterminator picks which support requests are high-priority to deserve
immediate attention. Factors include:

- Is there a workaround? (If so, the exterminator owns verifying the user is able to use it)

- How bad is the impact? Are there side effects (like data loss in the cluster)

- How common is it?

- Is it blocking a high-priority team?

If you aren't sure, ask a teammate or in #triage-bugs.

For high priority requests, the exterminator should assign someone to start work
immediately.

Low priority requests should be tracked in Clubhouse. Teams should make their own
judgements about how to prioritize them.

If the exterminator sees a request that they know how to fix quickly, they
should consider fixing it right away.

### Releases

The exterminator is responsible for making sure a
[release](https://github.com/windmilleng/tilt/blob/master/DEVELOPING.md#releasing)
happens every non-holiday week.

Each release should have a summary [release notes section](https://github.com/windmilleng/tilt/releases)
highlighting major exciting changes, changes that break existing workflows, and upcoming
deprecations, in addition to the automatically generated changelog section.

### Handoff

On the last day of the week, the current exterminator is responsible for passing
along any important context to the next exterminator. The current exterminator
should:

- Fill out [the Exterminator Rotation Form](https://docs.google.com/forms/d/e/1FAIpQLSfArwFScYVP7ytFSJDAE6VWQJr4daaEZFPoCwRC0brkuX9bKg/viewform?usp=sf_link)

- Meet for 15 minutes with the next exterminator, and ask for clarifying
  questions on the form results

## Support Load

Over time, we want to be able to track the overall support load on the
exterminator so we can adjust the process. We use two main metrics:

- The exterminator handoff form asks for a count of how many unique users
  filed a Github issue or asked a question in the Slack channel each day.
  (As the goal of this metric is to track exterminator support load, this
  number should not reflect Tilter-initiated Github issues.)

- For all new Github issues that we want to track,
  the exterminator should run the [**github -> clubhouse import script**](https://github.com/windmilleng/exterminator).
  The script will add an exterminator label so that we can count
  the number of exterminator-created tickets each week.

Nick is responsible for tracking these two metrics over time.

## Lead Tracking

We name a “Lead Tracker” to own user support leads triage.  They monitor support
channels for teams that are asking interesting questions, and might need more
support to get set up with Tilt.

Currently, the Lead Tracker is Nick.

### Responsibilities

When new users ask a question in the Slack channel or Github repo, 
the Lead Tracker should:

- Research who they are and what team they're on

- Enter that info into the CRM

- Decide if it's worth reaching out to them

Either the Lead Tracker or the Exterminator may do the reach out, depending
on how much the exterminator has been talking to the user already and how
much bandwidth they have.
