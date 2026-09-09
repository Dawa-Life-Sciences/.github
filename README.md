# .github

Default community health files for the `Dawa-Life-Sciences` organisation.

Everything here appears automatically on any repo in the org that has not
written its own version of the same file:

| File | Appears as |
|---|---|
| `.github/PULL_REQUEST_TEMPLATE.md` | The body of every new pull request |
| `.github/ISSUE_TEMPLATE/*.yml` | The choices offered when filing an issue |
| `CONTRIBUTING.md` | Linked from the issue and pull request pages |

A repo that wants something different writes its own file of that type and it
wins. That is the intended escape hatch; there is no need to argue with a
template.

## This repo is deliberately thin

Templates are reminders at the moment they are needed. They are not the place
for practice or reasoning — those live in
[`Dawa-Life-Sciences/engineering`](https://github.com/Dawa-Life-Sciences/engineering),
one home per fact, so that a rule and its explanation cannot drift apart.

If you are about to add a document here, it probably belongs there instead.

## A note on visibility

GitHub only applies these defaults org-wide from a **public** `.github`
repository — issue and pull request templates specifically will not apply from
a private or internal one. Keep that in mind when editing: everything in this
repo is world-readable, so it carries process and nothing about how anything is
secured, configured, or deployed.
