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

