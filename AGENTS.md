# Kroxylicious AI Agent Guidelines

This file provides guidance for AI coding tools, such as GitHub Copilot and Claude Code, when working in Kroxylicious repositories.

Contributors using AI tools must ensure the tools can access this file and any repository-specific `AGENTS.md` file.
Please also read the [Contributing Guidelines](./CONTRIBUTING.md), in particular the section on [Use of AI Assistance](./CONTRIBUTING.md#use-of-ai-assistance).

## Contribution Process

### DCO Sign-off

All commits must be signed off with the Developer Certificate of Origin (DCO).
Use `git commit -s` to add the sign-off automatically.

### Assisted-by Trailer

Commits created with AI assistance must include an `Assisted-by` trailer identifying the tool and model.
Add the trailer to the commit message body after the sign-off:

```
<commit message>

Signed-off-by: Name <email>
Assisted-by: <Tool and model> <noreply@example.com>
```

### Commit Discipline

- Each commit must be atomic and represent a single logical change.
- Keep commits small enough to be reviewed in a few minutes.
- Commit messages should explain *why* the change was made, not *what* changed. Reviewers can see the code changes in the diff. Focus on the problem being solved, the reasoning, or the decision made.

### Pull Requests

- A pull request should address a single cohesive goal. Do not bundle unrelated changes together — each PR should tell a clear story that a reviewer can follow from start to finish.
- Submit all changes as pull requests.
- At least one human [Committer](./COMMITTERS.md) must review and approve a pull request before it is merged.
  Automated or AI-assisted reviews, such as security or style checks, can supplement human review but do not replace it.
  The decision to merge is always made by human committers following the project's [decision making](./GOVERNANCE.md#decision-making) framework.
- PR descriptions must focus on the problem being addressed, the approach taken, and any trade-offs or alternatives considered. They must also note any AI tool involvement.
- Ensure all CI checks pass before requesting review.

### Conciseness

Be concise and efficient in all generated content.
Do not produce filler, boilerplate explanations, or unnecessary verbosity.
Stay focused on the goal at hand — reviewers' time is limited and every line should add value.

### Copyright and Licensing

Do not reproduce copyrighted material in generated code, documentation, or other content.
If you are aware of controls or configuration that reduce or remove the risk of reproducing copyrighted content, ensure they are active.
All contributions must be compatible with the project's [license](./LICENSE).

### Naming and Comments

Write code that is self-describing through clear naming and structure.
A well-chosen name is almost always better than a comment.
Names must convey intent and purpose, not implementation logic, which can become outdated as quickly as a stale comment.
Use comments for reasoning or constraints that good naming alone cannot convey, but if you find yourself reaching for a comment, first consider whether a rename would make it unnecessary.

## Technical Foundations

Kroxylicious is built with Java and [Apache Maven](https://maven.apache.org/).
Use `mvn verify` to build and test unless the repository's `AGENTS.md` specifies otherwise.
Individual repositories typically include an `AGENTS.md` file with build commands, architecture details, coding conventions, and testing expectations.

When working on a specific repository, always prefer guidance from that repository's `AGENTS.md` over this file for technical matters.
