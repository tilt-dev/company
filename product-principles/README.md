# Product Principles

As we scale Tilt the company and the product, we will explore how to build a product that best serves our users. These product prinicples help align Tilters and the open source community to build Tilt in a coherent fashion, also allowing for distributed decision making to ensure we can ship quickly. We expect these product principles themselves to evolve over time, so this is always a work in progress.

## Usability over documentation
We believe that Tilt should be usable without reading a separate manual. We strive to design usable interfaces, even for complex features with powerful functionality, without relying on subsequent documentation as a crutch for poor design. We prefer to use our [documentation](https://docs.tilt.dev/) to provide context on broad features, walkthroughs, and API details.

## Declarative over imperative
Inspired by modern container orchestration like Kubernetes, Tilt is designed with a _declarative_ interface in mind. Users are encouraged to describe their desired local development system state in a Tiltfile, and Tilt will approach that state quickly, or surface errors explaining why it's not possible. We want teams focused on the hard work of building value-add apps for their business, and not struggle with the messiness of many systems and services, and their interdependencies. Tilt should simplify that for you.

At the same time, we chose Starlark (a Python dialect) as the language of Tiltfiles. Tilt thus offers users to progressively take advantage of the flexibility of Tilt with _imperative_ programming, in a simple language that users can quickly recognize and thus be productive with.
