---
layout: page
title: Software Engineering Best Practices
permalink: /software-engineering-best-practices/
---

# Software Engineering Best Practices

## On Improving Stability & Quality

- Require all code changes to meet minimum quality controls before going into the main/master branch. (See [Slow is smooth, and smooth is fast.](/principles/slow-is-smooth-and-smooth-is-fast))
- Gate code changes on passing test suites.

## On Automated Testing

- **Prioritize the stability of your test suite over the quantity of tests.** A failing test suite should be a critical or blocker level priority for at least one team. Flaky tests introduce noise and undermine trust.
- **Require BDD tests for critical-path user stories.**
- The point of manual testing is to catch bugs before they reach customers, and the point of automated testing is to catch bugs before they reach manual testers.
- It is generally fastest and easiest to fix bugs at the time they are introduced, so invest in catching regressions early. A unit test that fails locally within seconds is far superior to an end to end test that fails on a build pipeline hours later, and that end to end test is far superior to a manually tester finding the bug days later.
- **_Everyone_ is responsible for quality.**
- **_Developers_--not testers--are responsible for writing code that works.**
- **Write tests at the lowest layer possible**: unit tests, then integration tests, then e2e/API tests. Recognize that BDD tests can be written in any layer, but most of them will live in higher layers (e.g. e2e). This is more important than the pyramid vs trophy debate, but IMO leads to a pyramid shape.
- Static analysis and compile time eliminates a whole class of runtime bugs and unit tests.
- Unit tests are highest ROI at preventing regressions because they're cheapest to write and maintain and execute fastest, but they are limited in scope and won't prevent most regressions.
- The point of integration tests is to catch bugs before e2e tests. The point of unit tests is to catch bugs before integration tests.
- If you can't reliably ship without introducing regressions, prioritize writing e2e tests for your critical path.
- **Make deployments a non-event.** Automate them. Make them frequent. Rely on automated tests (including performance tests) to inform the team of regressions. It's generally less risky to ship one change than many.
- Apply TDD's red-green-refactor to bugs: Where possible, write a failing automated test before fixing the bug. The best way to know whether a test will fail when the code is broken and pass when the code works is to write the test and see it fail before fixing the bug and seeing it pass.

## On Architecture

- Architecture is the stuff that's hard to change.
- Minimize the number of things that are hard to change.
- When it comes to software, gardener is a better term than architect. A building architect creates elaborate blueprints and then builds exactly that. A software architect is continually refining like a gardener: pulling weeds here, planting new plants there.
