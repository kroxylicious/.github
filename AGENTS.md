# Kroxylicious AI Agent Guidelines

This file provides guidance to AI coding tools (such as GitHub Copilot, Claude Code, and similar) when working on repositories within the Kroxylicious organisation.

Contributors using AI tools should ensure their tool has access to this file and any repository-specific `AGENTS.md`.
Please also read the [Contributing Guidelines](./CONTRIBUTING.md), in particular the section on [Use of AI Assistance](./CONTRIBUTING.md#use-of-ai-assistance).

## Contribution Process

### DCO Sign-off

All commits must be signed off with the Developer Certificate of Origin (DCO).
Use `git commit -s` to add the sign-off automatically.

### Assisted-by Trailer

Commits produced with AI assistance must include an `Assisted-by` trailer identifying the tool and model.
The trailer should be added to the commit message body, after the sign-off:

```
<commit message>

Signed-off-by: Name <email>
Assisted-by: <Tool and model> <noreply@example.com>
```

### Commit Discipline

- Each commit should be atomic and represent a single logical change.
- Keep commits small enough to be reviewed in a few minutes.
- Commit messages should explain *why* the change was made, not *what* changed. Reviewers read diffs — they can see what changed. Focus on the problem being solved, the reasoning, or the decision made.

### Pull Requests

- A pull request should address a single cohesive goal. Do not bundle unrelated changes together — each PR should tell a clear story that a reviewer can follow from start to finish.
- All changes must be submitted as pull requests.
- At least one human [Committer](./COMMITTERS.md) must review and approve a pull request before it is merged.
  Automated or AI-assisted reviews (such as security or style checks) may supplement but do not substitute for human review.
  The decision to merge is always made by human Committer(s) following the project's [decision making](./GOVERNANCE.md#decision-making) framework.
- PR descriptions should focus on the problem being addressed, the approach taken, and any trade-offs or alternatives considered. Note any AI tool involvement.
- Ensure all CI checks pass before requesting review.

### Copyright and Licensing

Do not reproduce copyrighted material in generated code, documentation, or other content.
If you are aware of controls or configuration that reduce the risk of reproducing copyrighted content, ensure they are active.
All contributions must be compatible with the project's [license](./LICENSE).

### Naming and Comments

Prefer code that is self-describing through clear naming and structure.
A well-chosen name is almost always better than a comment.
Names should convey intent and purpose, not encode implementation logic — logic in a name will drift from reality just as quickly as a stale comment.
Reserve comments for reasoning or constraints that good naming alone cannot convey, but if you find yourself reaching for a comment, first consider whether a rename would make it unnecessary.

## Technical Foundations

Kroxylicious is built with Java and [Apache Maven](https://maven.apache.org/).
Individual repositories will have their own `AGENTS.md` with specific build commands, architecture details, coding conventions, and testing expectations.

When working on a specific repository, always prefer guidance from that repository's `AGENTS.md` over this file for technical matters.
