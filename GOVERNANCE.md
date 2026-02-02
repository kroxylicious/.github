# Kroxylicious Governance

This document outlines the governance model for Kroxylicious.
This governance model is designed to uphold the principles of transparency, open collaboration, and community involvement.

[cfc]: https://www.commonhaus.org/bylaws/cf-council.html
[cdm]: https://www.commonhaus.org/bylaws/decision-making.html
[ctp]: https://www.commonhaus.org/policies/trademark-policy/
[coc]: ./CODE_OF_CONDUCT.md
[contrib]: ./CONTRIBUTING.md

## Table of Contents

<!-- TOC -->
* [Kroxylicious Governance](#kroxylicious-governance)
  * [Table of Contents](#table-of-contents)
  * [Roles and Responsibilities](#roles-and-responsibilities)
  * [Decision Making](#decision-making)
  * [Code of Conduct](#code-of-conduct)
  * [Trademark Policy](#trademark-policy)
  * [Contributing](#contributing)
  * [Becoming a Code Owner](#becoming-a-code-owner)
    * [Code Owner Criteria](#code-owner-criteria)
  * [Governance Improvement Process](#governance-improvement-process)
<!-- TOC -->

## Roles and Responsibilities

- **Code owners:** Individuals with write access to any repository within the GitHub organisation, responsible for reviewing and merging contributions, and steering project direction. 
  Those people with code ownership responsibilities will be identified in each repository (`.github/CODEOWNERS`).
  For the sake of transparency, the membership of github teams will be made public in [TEAMS.md](TEAMS.md).
- **Contributors:** Anyone who contributes to the project in any form.

Reference: [About code owners](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners)

## Decision Making

This project follows The [Commonhaus decision making][cdm] process.
This project uses the following decision making process.

1. **Consensus-seeking (lazy consensus):** The project primarily aims for a consensus-based decision-making process, where code owners and active contributors discuss and come to an agreement.
2. **Voting:** In situations where consensus cannot be reached, decisions may be made through a simple majority vote among the code owners.
3. **Conflict Resolution:** If conflicts arise, code owners are responsible for facilitating a resolution. The [Commonhaus Foundation Council][cfc] (CFC) can be asked to mediate the discussion, if necessary.

## Code of Conduct

All participants in the project are expected to adhere to the project's [Code of Conduct](./CODE_OF_CONDUCT.md). Please ensure you are familiar with its guidelines and expectations, as it's essential for maintaining a positive and collaborative environment.

## Trademark Policy

The Kroxylicious logos, icons, and domain names are protected by trademark rights. Usage of these trademarks must adhere to our [Trademark Policy][ctp].

## Contributing

We welcome all forms of contribution, from code improvements to documentation and design. For details on how to contribute and the process your contributions will follow, please read our [Contributing Guidelines][contrib].

## Becoming a Code Owner

New Code Owners can be elected by a majority vote of the existing Code Owners following the [Decision Making](#decision-making) process.

To ensure that all potential Code Owners are judged fairly and consistently the following criteria should be taken into account in electing new Code Owners:

### Code Owner Criteria

* Sustained contributions over at least 3 months ideally including non-trivial PRs.
* Reviewing other contributors’ PRs
* Contributing to multiple aspects of the project and community. For example:
  * Bug reporting, triage and fixing
  * Addressing technical debt (in code, testing and documentation).
  * Documentation (both content and structure).
  * Helping users, for example on GitHub, the mailing list, Slack, Stack Overflow, and so on.
  * Promotion of Kroxylicious, for example by blogging, speaking at conferences, and so on.
* Knowing when to ask for help or seek consensus.
* An indication of being committed to the long term success of the project.

## Governance Improvement Process

We define the following process for improving the Governance of Kroxylicious.

> **_NOTE:_**  This is the formal process for changing project Governance, but in most cases we would appreciate a conversation
> beforehand. You can reach out to us on Slack, or create an Issue in this repository to get the ball rolling.

1. **Eligibility:** Any member of our community may submit a proposal to improve our governance.
    The author is referred to as the **Proposer**.
2. **Identification:** Every proposal requires a unique ID following the pattern `GIP-000`, `GIP-001`, etc.
    * The Proposer selects the next available number based on existing files in the `decision-records` directory and the
      ids used by open PRs.
    * *Note:* If a numbering collision occurs with another open PR, the newer PR must update its ID to the next
      available number.
3. **Submission:** A Proposal is created by opening a Pull Request (PR) in this repository.
4. **Requirements:** Each PR must represent a single proposal and include:
    * **The Policy Change:** Edits to the actual governance files (e.g., `Governance.md`).
    * **The Record:** A new Governance Decision Record (GDR) file in `decision-records/`, named like
      `GIP-000-brief-description.md`. This file must follow the template located
      at [decision-records/TEMPLATE.md](decision-records/TEMPLATE.md).
    * **The Title:** A PR title containing the ID, e.g., `[GIP-000] Adopt Governance Improvement Process`.
5. **Visibility:** The Proposer must announce the PR in the `#general` channel of the Kroxylicious Slack to invite
    community review.
6.  **Review:** We discuss and amend the Proposal until it's in a good shape.
7. **Open Decision Making Period:** We follow the [Decision-Making](#decision-making) policy.
    * A **Code Owner** must announce that the Decision Making Period has started, or restarted due to significant modifications.
      This should be announced in the `#general` channel of our Community Slack.
    * Discussion, objections, and voting should be done in the PR comments.
8. **Finalization:**
    * **If Accepted:** The Proposer must update the GDR file status to "Accepted" and record the ratification date. A
      Code Owner will then merge the PR.
    * **If Rejected/Stale:** If a proposal is rejected or remains stale (no decision making period declared) for two months, the PR will be closed.
      A Code Owner will extract the GDR file from the PR, set its status to "Rejected" and commit it to this repository.