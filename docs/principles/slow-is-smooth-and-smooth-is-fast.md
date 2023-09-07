---
layout: page
title: Slow is smooth, and smooth is fast
permalink: /principles/slow-is-smooth-and-smooth-is-fast
parent: Leadership Principles
---

## Slow is smooth, and smooth is fast.

Unless it's truly a matter of company survival, take the time to slow down and optimize for consistent throughput.

<!-- and invest in your Continuous Integration / Continuous Deployment (CI/CD) and test automation. -->

Examples of slow is smooth, and smooth is fast:

Slowing down to:

- Create a CI pipeline before building a project
- Create a CD pipeline to deploy a Hello World page before building actual features
- Require test suites pass before code is allowed to be merged to master
- Setup a local dev environment with auto-reload
- Require tests be written for every new feature before code goes live. While it slows you down up-front, it reduces manual regression testing effort permanently.

There are always justifications provided for not slowing down:

- The startup is on the brink of bankruptcy
- The initiative has to get done by EOY so some executive meets their goals
- We will lose a major client if the initiative is not delivered X date
- It's just a prototype / proof of concept

_Sometimes_ cutting corners are legitimately a question of survival, but often, these reasons are used to justify ignoring mounting technical debt. Worse, they are sometimes imposed by short-sighted engineering managers who don't understand the true impact of these decisions on engineering velocity.

A better question is whether the runway is long enough to receive a payoff on the effort invested.

The problem is most successful proofs of concept become production code that has to be maintained. The point when a proof of concept is gaining initial traction and tons of additional features are needed ASAP is not an ideal time to slow down. Slow down and get your pipelines in place first. You'll benefit from it even during prototyping.
