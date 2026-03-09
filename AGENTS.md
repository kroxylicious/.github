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
- Write clear, descriptive commit messages that explain *why* the change was made, not just *what* changed.
- Keep commits small enough to be reviewed in a few minutes.

### Pull Requests

- All changes must be submitted as pull requests.
- At least one human [Committer](./COMMITTERS.md) must review and approve a pull request before it is merged.
  Automated or AI-assisted reviews (such as security or style checks) may supplement but do not substitute for human review.
  The decision to merge is always made by a human committer.
- PR descriptions should summarise the change and note any AI tool involvement.
- Ensure all CI checks pass before requesting review.

## Technical Foundations

Kroxylicious is built with Java and [Apache Maven](https://maven.apache.org/).
Individual repositories will have their own `AGENTS.md` with specific build commands, architecture details, coding conventions, and testing expectations.

When working on a specific repository, always prefer guidance from that repository's `AGENTS.md` over this file for technical matters.
