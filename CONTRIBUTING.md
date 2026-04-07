# Contributing

## Code of Conduct

This project and everyone participating in it is governed by the [Code of Conduct](CODE_OF_CONDUCT.md).
By participating, you are expected to uphold this code. 
Any unacceptable behavior should be reported to [kroxylicious-admins@redhat.com](mailto:kroxylicious-admins@redhat.com).

## How can I contribute

You can contribute by:

* Reporting any issues you find using Kroxylicious
* Fixing issues by opening Pull Requests
* Reviewing Pull Requests opened by others.
* Improving documentation
* Talking about Kroxylicious

All bugs, tasks or enhancements are tracked as GitHub issues.
Issues which might be a good start for new contributors are marked with the “good-start” label.
Public API changes are required to follow the [Design Process](#design-process)

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
The GitHub teams `@kroxylicious/code-reviewers` and `@kroxylicious/doc-reviewers` can be used to request a PR review from contributors.

If you're willing to provide code and/or reviews to others then let one of the [project managers](PMs.md) know and we can add you to the relevant GitHub team.

## Design Process

All Public API changes must begin with a design proposal. This includes:

* New APIs or API endpoints
* Changes to existing API signatures or behavior
* Removal or deprecation of APIs

Public APIs include (but are not limited to):
* Proxy configuration YAML
* Filter configuration YAML
* Kubernetes CRDs
* Operator manifested resources (like public bootstrap server addresses)
* Filter API (and other plugins) interfaces
* Wire-protocol changes (e.g. format of encrypted data emitted by Proxy)

Design proposals should be submitted to the [design repository](https://github.com/kroxylicious/design).

## I just have a question

If you encounter any issues while using Kroxylicious, you can get help using:

- [#general channel on Kroxylicious Slack](https://kroxylicious.slack.com/)
- [Kroxylicious GitHub Discussions](https://github.com/kroxylicious/kroxylicious/discussions)
