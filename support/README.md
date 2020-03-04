# User Support

## Exterminator

Every week, we name an “exterminator” to own user support triage. They triage and assign bugs, monitor support channels for new leads, and manage releases:

### SLA

First response in an hour (during business time); updates to user until either solved or triaged out:

- [Github - Tilt Issues](https://github.com/windmilleng/tilt/issues)

- [Kubernetes Slack - #tilt channel](https://kubernetes.slack.com/messages/CESBL84MV/)

Within a day:

- Email inbox (hi@windmill.engineering) (https://groups.google.com/a/windmill.engineering/forum/#!forum/hi)

- DMs or Mentions to @windmill_eng

- All new users should be researched and entered into the CRM. If they’re a
  promising lead, the exterminator should reach out to them.

For any new bugs reported by users, the Exterminator should create a Github
issue. For any existing bugs reported by users, the Exterminator should note the
request in the existing Github issue / direct the user to the existing issue and
ask them to +1 it so we know who to follow up with,

Anyone with a bug to report should slack it to #triage-bugs and, if it turns out
to be a new bug, file an issue in GitHub . Issues with a bug label are
automatically added to the [Tilt bug
triage](https://github.com/orgs/windmilleng/projects/2). Ping the exterminator
with the issue, and they will prioritize the bug. For high priority bugs, the
exterminator should assign someone to start work immediately. Low priority bugs
are assigned in planning.

Any interesting new leads should be mentioned in #triage-customers. The
exterminator should use their best judgment on who is promising enough to DM
directly (based on a combination of research on their background and how active
they are in the channel).

The exterminator is responsible for making sure loops get closed,
non-exterminators can reply but should tend to defer.

The exterminator is also responsible for making sure a
[release](https://github.com/windmilleng/tilt/blob/master/DEVELOPING.md#releasing)
happens every non-holiday week.

## Bug Priority

The exterminator picks which bugs are high-priority to deserve immediate attention. Factors include:

- Is there a workaround? (If so, the exterminator owns verifying the user is able to use it)

- How bad is the impact? Are there side effects (like data loss in the cluster)

- How common is it?

- Is it blocking a high-priority customer?

If you aren't sure, feel free to ask a teammate or in #triage-bugs.
