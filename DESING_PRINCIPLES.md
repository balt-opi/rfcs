# OPI Design Principles

The following are general guiding principles to consider as you're iterating through your projects design.


## Expressive by being precise

OPI projects should provide concepts that build a strong mental model for the user's project, and this model should remain intuitive as the user's requirements grow.

Concepts should precisely outline their motivation and intended workflows. Friction and complexity resulting from the imprecise application of a concept should be a cue to introduce new ideas.


## Versatile by being universal

OPI projects should be able to do a lot with a little. New concepts should only be introduced if their intended workflow cannot be precisely expressed in terms of existing concepts.

Concepts should not be highly specialized for one domain or introduce tight coupling to specific technologies.


## Safe by being destructible

OPI projects should prevent [anti-patterns](https://github.com/concourse/concourse/wiki/Anti-Patterns) and the accumulation of technical debt. Projects should make good practices feel intuitive and bad practices feel uncomfortable.

Automation should be self-contained and reproducible in order to maintain business continuity when recovering from disaster scenarios (e.g. total cluster loss).