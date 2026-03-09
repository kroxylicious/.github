# Contributing

## Code of Conduct

This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md).
By participating, you are expected to uphold this code. 
Any unacceptable behavior should be reported to [kroxylicious-admins@redhat.com](mailto:kroxylicious-admins@redhat.com).

## About the Project

Kroxylicious is a Java project built with [Apache Maven](https://maven.apache.org/).
Individual repositories may have additional details in their `README.md` or `AGENTS.md` files.

## How can I contribute

You can contribute by:

* Reporting any issues you find using Kroxylicious
* Fixing issues by opening Pull Requests
* Reviewing Pull Requests opened by others.
* Improving documentation
* Talking about Kroxylicious

All bugs, tasks or enhancements are tracked as GitHub issues.
Issues which might be a good start for new contributors are marked with the “good-start” label.

## Finding an Issue

We have issues labelled [good first issue](https://github.com/kroxylicious/kroxylicious/issues?q=is%3Aissue%20state%3Aopen%20label%3A%22good%20first%20issue%22) for new contributors and [help wanted](https://github.com/kroxylicious/kroxylicious/issues?q=is%3Aissue%20state%3Aopen%20label%3A%22help%20wanted%22) issues suitable for any contributor. 

Sometimes there won’t be any issues with these labels. That’s ok! There is likely still something for you to work on. If you want to contribute but you
don’t know where to start or can't find a suitable issue, you can come [chat to us](https://kroxylicious.slack.com/archives/C050RNMQW8G).

Once you see an issue that you'd like to work on, please post a comment saying that you want to work on it. Something like "I want to work on this" is fine.
If later you need to change your mind, for whatever reason, that's fine too. Just post another message so others know its free.

## DCO Signoff

The project requires that all commits are signed-off, indicating that _you_ certify the changes with the [Developer
Certificate of Origin (DCO)](./DCO.txt).

This can be done using `git commit -s` for each commit
in your pull request. Alternatively, to signoff a bunch of commits you can use `git rebase --signoff _your-branch_`.

## PR Review

All changes which are to be committed in project source control must be reviewed by at least one [Committer](COMMITTERS.md) before being merged.
If the change is being authored by someone who is a Committer, that change must be reviewed by at least one other Committer before being merged.
Automated or AI-assisted reviews (such as security or style checks) may supplement but do not substitute for review by a Committer.
The decision to merge is always made by Committer(s) following the project's [decision making](./GOVERNANCE.md#decision-making) framework.
Pull requests should be focused on a single goal and sized for effective review.
We may close pull requests that are unfocused or too large to review effectively, and ask the contributor to break them into smaller, more reviewable changes.

The GitHub teams `@kroxylicious/code-reviewers` and `@kroxylicious/doc-reviewers` can be used to request a PR review from contributors.

If you're willing to provide code and/or reviews to others then let one of the [project managers](PMs.md) know and we can add you to the relevant GitHub team.

## Use of AI Assistance

Contributors may use AI tools (such as LLMs, code assistants, and similar) when preparing contributions to Kroxylicious.
Like any tool, what matters is the quality of the result and that the contributor understands what they are submitting.

When you submit a contribution you are the contributor, regardless of what tools you used to produce it.
You are responsible for understanding what you are contributing and ensuring it meets the project's standards.

### Requirements

* **You are the contributor.** When you sign off the [DCO](./DCO.txt), you are certifying the contribution as your own.
  AI-generated or AI-assisted content does not change this obligation.
* **Understand your contribution.** You must have a clear understanding of what your contribution does and why.
  Do not submit code, documentation, or other content that you do not understand.
* **Disclose AI usage.** If AI tools played a significant role in producing a contribution, note this in the pull request description.
  Commits should include an `Assisted-by` trailer identifying the tool and model used (e.g. `Assisted-by: Claude Opus 4.6 <noreply@anthropic.com>`).
  Most AI coding tools can be configured to add this automatically — see the repository's `AGENTS.md` for details.
* **Ensure originality and licensing compliance.** AI-generated content must not reproduce copyrighted material.
  You are responsible for verifying that your contribution does not introduce intellectual property or licensing concerns
  incompatible with the project's [license](./LICENSE). Where your AI tool offers controls to reduce the risk of
  reproducing copyrighted content, ensure they are enabled.
* **Meet the same quality bar.** AI-assisted contributions are reviewed to the same standard as any other contribution.
  Code must be correct, maintainable, tested, and consistent with project conventions.
  We may close pull requests where the contributor does not appear to understand the contribution they have submitted.
* **Be concise.** AI tools can generate text faster than reviewers can read it.
  Contributions, PR descriptions, and issue comments should be clear, focused, and free of unnecessary verbosity.

### AGENTS.md

Individual repositories within the Kroxylicious organisation may include an `AGENTS.md` file.
These files provide AI tools with project-specific context such as build instructions, architecture, coding conventions, and testing expectations.
If you are using an AI tool to help prepare a contribution, ensure it has access to the relevant `AGENTS.md` so that its output aligns with project norms.

## I just have a question

If you encounter any issues while using Kroxylicious, you can get help using:

- [#general channel on Kroxylicious Slack](https://kroxylicious.slack.com/)
- [Kroxylicious GitHub Discussions](https://github.com/kroxylicious/kroxylicious/discussions)
