# Product Principles

As we scale Tilt the company and the product, we will explore how to build a product that best serves our users. These product principles help align Tilters and the open source community to build Tilt in a coherent fashion, also allowing for distributed decision making to ensure we can ship quickly. We expect these product principles themselves to evolve over time, so this is always a work in progress.

## Usability over documentation
We believe that Tilt should be usable without reading a separate manual. We strive to design usable interfaces, even for complex features with powerful functionality, without relying on subsequent documentation as a crutch for poor design. We prefer to use our [documentation](https://docs.tilt.dev/) to provide context on broad features, walkthroughs, and API details.

## Infrastructure as Data

One of the core design principles of Kubernetes is ["infrastucture as data."](https://twitter.com/kelseyhightower/status/1164194470436302848)

Users should express their desired system state as data. The fundamental
building block of Kubernetes is a
[controller](https://kubernetes.io/docs/concepts/architecture/controller/) that
looks at the desired state, compares it to the current state, and takes steps
bring the current state closer to the desired state. If the desired state is impossible,
Kubernetes will stop and explain why.

Tilt builds on the same principles. Your Tiltfile declares the desired state of your
development environment. The Tilt engine is a controller that compares that to
the current state of your cluster, and builds what you need to start
developing. If you make a change to your Tiltfile, Tilt will see that change and
adjust its strategy.

A common misunderstanding of this principle is "all configuration should be
declarative," or, worse, "all configuration should be YAML." But that's not what
we're saying! A consequence of this principle is that all configuration *can* be
declarative. But this isn't equivalent. It's easy to have declarative
configuration for a tool that does not treat infrastructure as data, 
and doesn't offer the kind of responsive control that we want Tilt to have.

Tiltfiles [are written in
Starlark](https://docs.tilt.dev/tiltfile_concepts.html), a subset of Python. The
Tiltfile declares the state of your development environment.  A simple Tiltfile
looks declarative, like YAML. Starlark is flexible enough that you can use more
imperative code to declare the state of your dev environment, but is more
limited than a full programming language.

## Extensibility

There's an old quote that "Kubernetes competes with Bash."

We believe Tilt competes with Bash.

What we mean by that is that Kubernetes doesn't change the problems that infra
engineers are solving, just how they solve it. They're writing the same tools in
a Kubernetes framework instead of in Bash.

Similarly, Tilt is an extensible system that we expect to replace Bash for how
devs set up their dev environment. Tilt provides the control loop and a default
display engine, but users should be able to supply the data models,
functionality, and custom displays.

When we build any feature in Tilt, we should consider how users might have added
that feature.

For example, `docker_build` is a built-in that we made. But users want to create their
own builders. How could we make it so that anyone could have added `docker_build`?

Users often want a way to cancel `docker_build`. How would they add their own
built-in cancellation semantics? How baked into the control loop should it be?
