# Interview Feedback

This is a guide for Tilters filling out interview feedback forms.

The most important guideline: this feedback form is for you! 

An old meditation quote is: “You can't stop the waves, but you can learn to surf.”

Similarly, you're going to have gut reactions to candidates. And biases. That's
OK. The goal of this form is to help you observe those reactions at a distance,
and be thoughtful about which ones are about the candidate's ability to do a job,
and which are not.

The form is NOT an advocacy document where you try to persuade the other
interviewers that your interpretation is correct. It will be very obvious and
not compelling if you're treating it that way.

Below is a sample form of the kind and length of reactions that are good in an
interview feedback form. Most of them have been lifted lightly from [this
rubric](https://medium.engineering/engineering-interviews-grading-rubric-8b409bec021f).

A good rule of thumb is to fill out about half of the attributes.

## Questions Asked

Past project. They described the architecture of their muffin-sharing site, a
three-sided social network to connect people who owned muffin tins, people who
wanted to bake muffins, and people who had extra capacity to eat muffins.

## Overall Impressions

Hire. Could be convinced otherwise. 

They seem versatile, good at learning new things and adapting to new roles. They have
some of the specific data engineering expertise we need.

The downside is that they're weaker on particular subject area expertise
(e.g. kubernetes), and don't seem to care that much about the problems we're
solving (see notes in Perspective).

## Ability to Build Software

### Problem Solving

5 - They described their process for choosing a database, what solutions they looked
at, and what trade-offs they considered. I thought their analysis of different
databases was thoughful and well-reasoned, particularly when they ruled out Neo2j
because it was heavily optimized for two-sided muffin networks.

### Code Fluency

Not enough signal

### Autonomy

3 - They said that most of their career has been on teams where he had a lot of
freedom to choose tools and approaches. They sound like they really enjoyed an
environment where they had limited resources and had to resolve problems as best
they could.

But there was one incident that stood out to me -- on the database project, they
did a bunch of independent research on databases, wrote up an analysis doc, then
sent it to their product manager to make the decision. This struck me as odd,
and I'm not sure if this was about the culture of the team, or speaks to trouble
they have taking ownership of technical decisions. I wonder if this showed up in
other interviews.

### Basic Computer Science Knowledge

4 - They were able to describe the differences between NoSQL, SQL, and timeseries
databases, and why you would choose one over the others.

### System Design

Not enough signal

### Resoluteness

Not enough signal

## Ability to Learn and Teach

### Curiosity

Not enough signal

### Awareness

5 - See the section on collaboration, and their ability to change the approach
in response to feedback.

### Empathy

Not enough signal

### Communication

4 - I wish they'd actively checked my understanding more what I knew before
starting they're explanation of ORMs and how they applied to the Pareto
distribution of muffins.

I had to prompt them several times to back up and explain context.

But once we were on the same page of where my current understanding was, they
generally explained concepts clearly and when I didn't understand things, was
able to reframe or break down the concept.

### Collaboration

5 - Their muffin platform team was 2 frontend engineers, a designer, and a
product manager. They did all the database/backend work. They described an
incident where they weren't sure what the right API was for the frontend to
consume, so they had multiple working sessions with the frontend engineers to
figure out what they needed and how flexible the API needed to be as the site
scaled. 

I was very impressed with how much back and forth collaboration there was in
these sessions. Their initial approach would have been hard for the frontend to
consume, but they took this feedback in stride and changed it to make life
easier for the frontend.

### Perspective

1 - The candidate has been at Google for 10 years. At the end of the interview,
they said they were really excited to work at a startup that had been founded by
other ex-Googlers, and used Google technology like Go and Kubernetes. They asked
why I hadn't worked at Google before coming to Tilt. This really annoyed me. I'm
concerned that the candidate doesn't even care that much about the product we're
building.
