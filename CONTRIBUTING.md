# Contributing

Full guidance lives in [`Dawa-Life-Sciences/engineering`](https://github.com/Dawa-Life-Sciences/engineering).
This is the short version, and it is what appears on every repo that has not
written its own.

## Pick a track

Not every change earns the same ceremony. **Full is the default** — drop below
it deliberately, and say so in the pull request.

| Track | When | Chain |
|---|---|---|
| **Full** | New capability; a security boundary; anything touching identity, audit, or regulated evidence | grill → PRD (on a branch) → issues → TDD → PR → merge |
| **Direct** | A fix with a known cause and a bounded blast radius | issue → TDD → PR → merge |
| **Mechanical** | Version bumps, deploy pins, dependency updates, docs | PR → merge |

**Size does not decide the track.** A small change to session or role handling
is Full, because the diff is short and the consequence is not.

## Build it test-first

Write the test, watch it fail, then make it pass. One behaviour at a time — not
every test up front, which produces tests of imagined behaviour rather than real
behaviour.

Test through the public interface, and test the refusals as well as the happy
path. Refusals are exercised least in development and matter most later.

Put the assertion that failed into the pull request. It is the one thing that
shows the test *can* fail.

## Layer names

New repos and new top-level modules:

`domain` · `application` · `infrastructure` · `interface`

Tests in `tests/`, mirroring the layer they cover. Existing repos differ and are
not being renamed — see the engineering handbook for what each one calls things.

## Before you open the pull request

- The suite passes.
- Anything you found but did not fix is a filed issue, not a PR comment. Comments
  disappear when the PR merges.
- The PR template's evidence lines are filled in, or honestly marked as not run.

## Where the reasoning is

This page says what to do. The engineering handbook says why, and what was
traded away to get there — including the parts that were deliberately not built.
Read it before proposing a change to any of this.
