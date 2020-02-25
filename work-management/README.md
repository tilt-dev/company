# Work Management
We aim to track all work at Tilt in [Clubhouse](https://app.clubhouse.io/windmill) and Google docs, together as the single source of truth, system of record. In particular, this includes future plans and discussions, prioritization and existing work, and past work. This includes product changes, as well as other typical activities requiring collaboration (e.g. planning for a conference).

## User interactions
In addition to email, Tilters communicate with non-Tilter users via [Kubernetes Slack](https://slack.k8s.io/) in the `#tilt` channel. Users are encouraged to submit feature requests and bugs in [GitHub issues](https://github.com/windmilleng/tilt/issues), where they can subscribe to notifications, discuss ideas with Tilters, and with other users. Open source contributors are also encouraged to participate in the same repo.

## Link GitHub issues and Clubhouse stories together
All GitHub issues in all [Tilt repos](https://github.com/windmilleng) should have a corresponding Clubhouse story, since all work should be tracked in Clubhouse. (The reverse is not true.) [Private Tilt repos](https://github.com/windmilleng?type=private) should have their respective issue trackers disabled, so that Tilters won't mistakenly create GitHub issues in those cases.

A GitHub issue should only be created in these scenarios:
- A user creates an issue as a feature request, improvement, or bug.
- A Tilter creates an issue on a user's behalf (e.g. in response to a Slack conversation).
- A Tilter intentionally wants to share planned or ongoing work with the community to get feedback. They create a GitHub issue (associated with an already created Clubhouse story).

We are [considering how to to easily link GitHub issues to Clubhouse stories](https://app.clubhouse.io/windmill/story/4692). For now, a GitHub issue's description should contain a Clubhouse story URL. A Clubhouse story that has one or more associated GitHub issues should indicate those GitHub URLs using the [Clubhouse external links feature](https://help.clubhouse.io/hc/en-us/articles/360000272903-Using-the-Zendesk-Integration-and-External-Ticket-Support).
