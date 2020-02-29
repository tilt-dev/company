# Product Development

## Workflow
We have a lightweight product develoment workflow that empowers teams to solve business problems, working directly with customers, and to be accountable for achieving positive business outcomes.

<img src="images/workflow.png" height="300" />

The workflow is summarized in the image above. At the far left, we continually have conversations with customers and the community. These are synthesized into GitHub issues. Based on this feedback and our broader company goals and strategy, we maintain a backlog of high-level initiatives as Clubhouse epics (primarily product changes). Over time, epics are further defined with scoped work and success criteria, as they are eventually implemented and shipped.

### Defining High-level Business Initiatives (Epics)
All Tilters are encouraged to collaborate in defining high-level business initiatives (Clubhouse epics) over time. This is an ongoing task with no specific timelines. Victor is responsible for ensuring that the backlog of epics is continually full. There should be no shortage of epics.

### Incrementally Solving Business Problems
When a Tilt engineer is free, they should pick a high priority epic to work on. They may consider finding another engineer to work as a two-person team.

The epic may have a fairly broad initial business problem. The team should carve out and define a smaller problem, and spec out a solution that can be accomplished within **2 weeks**. The epic description should be updated with the smaller scope and success criteria, and the team should create additional epics to capture the future work.

The purpose of a single epic is **not** to completely solve a business problem. Rather, completing an epic should likely achieve incremental progress at addressing a single problem, adding incremental user value as a result. In some cases, any realized user value may only appear in future epics. 

After the epic is completed, the team is disbanded, and individuals should find the next epic to work on, with the next team. Engineers should self-organize and coordinate timelines when picking epics. Engineers should avoid working on multiple epics concurrently. 

### Example
For example, suppose usability research suggests that the Tilt Web UI right sidebar is difficult for users to learn. A team develops some ideas to iterate on the existing designs in order to address the problems. But they discover that it's a better idea to first re-architect some of the frontend JavaScript and CSS to accommodate the design changes, repaying some previously incurred tech debt. In this case, the first epic would simply be non-user facing code re-architecture work, that doesn't have immediate user impact, but contributes to solving the usability problem indirectly as an incremental first step.

### Epic Acceptance Criteria
For an epic to be completed (and marked as such in Clubhouse), the epic description needs to contain the following as acceptance criteria:
- Finalized problem statement
- Explanation and scope of solution
- Links to updated metrics; why if not applicable (metrics may improve later over time)
- Links to follow up customer conversations; why if not applicable
- Links to updated docs; why if not applicable
- Attached screenhots, gifs, or video, showing the implemented change
- Links to future work, if applicable
- Link to company meeting, where the problem and the implemented change were presented
