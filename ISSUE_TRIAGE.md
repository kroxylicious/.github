# Issue Triage

The Kroxylicious team uses a triage process to triage the upstream backlog. This document describes the triage process and how to participate.

## Triage Process

When triaging an issue, work through the following steps in order:

### 1. Validate the Issue

Is this a legitimate issue or request for the Kroxylicious project?

- Does it describe a real problem or request for Kroxylicious?
- Is it on-topic for this project, or would it be better served elsewhere?

**If clearly no**: Close the issue with a comment explaining why (e.g., spam, off-topic, should go to a different project).

**If unclear or potentially valid**: Proceed to check completeness.

### 2. Check Completeness

Does the issue have sufficient information to understand and act on?

- For bug reports: Does it include steps to reproduce, expected behavior, and actual behavior?
- For feature requests: Is the use case and desired outcome clear?
- For questions: Would this be better served on the [mailing list](https://kroxylicious.io/join-us/mailing-lists) or [Slack](https://kroxylicious.slack.com/)?

**If no**: Ask the issue author to provide the missing details. If the author doesn't respond after a reasonable time, the issue may be closed.

### 3. Flag for Discussion

Does this issue require synchronous discussion at a community call?

- Does it involve a significant architectural decision?
- Is it a public API change? (See [Design Process](CONTRIBUTING.md#design-process))
- Would team discussion help clarify the scope or approach?

**If yes**: Add the `discuss-sync` label to prompt discussion at the next community call.

### 4. Add Labels

Apply labels to help categorize and route the issue:

- **good-first-issue**: Issues suitable for new contributors
- **help-wanted**: Issues open to community contributions
- **kind/bug**: Bug report
- **kind/feature**: Feature request or enhancement
- **kind/documentation**: Documentation improvement
- **design-process-needed**: Public API changes that require a design proposal (see [Design Process](CONTRIBUTING.md#design-process))
- Other relevant area or component labels as appropriate

### 5. Set a Milestone

If possible, assign a tentative milestone to help with planning and prioritization.

### 6. Leave a Triage Comment

Leave a comment on the issue recording that it has been triaged. Include:

- A summary of the triage assessment (e.g., "This looks like a valid feature request for...")
- Any next steps or action items (e.g., "Awaiting clarification from the author", "Flagged for discussion at the next community call", "Ready for implementation")

This provides transparency to the issue reporter and other community members about the triage outcome.

## Participation

Triage is an ongoing activity. Issues are reviewed regularly and new contributors are welcome to help.

For details on upcoming triage meetings or to ask questions about the process, reach out on the [Kroxylicious Slack](https://kroxylicious.slack.com/).
