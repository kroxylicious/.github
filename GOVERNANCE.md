# Kroxylicious Governance

This document outlines the governance model for Kroxylicious.
This governance model is designed to uphold the principles of transparency, open collaboration, and community involvement.

[cfc]: https://www.commonhaus.org/bylaws/cf-council.html
[cdm]: https://www.commonhaus.org/bylaws/decision-making.html
[ctp]: https://www.commonhaus.org/policies/trademark-policy/
[coc]: ./CODE_OF_CONDUCT.md
[contrib]: ./CONTRIBUTING.md
[dco]: ./DCO.txt
[committers]: ./COMMITTERS.md
[PMs]: ./PMs.md

# Purpose

The purpose of the Kroxylicious Project is to develop a Kafka protocol proxy with an open source license, and to make the resulting software and documentation available to Users.

## Code of Conduct

All participants in the project are expected to adhere to the project's [Code of Conduct][coc]. Please ensure you are familiar with its guidelines and expectations, as it's essential for maintaining a positive and collaborative environment.

## Participants

- **Users:** Anyone using the software is a User. 
    While the Project exists to provide the software to Users, the other participants' duties are to all current and potential Users collectively, any not to the interests of any one User, or subset of Users.

- **Contributors:** Anyone who contributes to the project, in any form, is a Contributor.
    Contributions can take a variety of forms, but many of them, such as source code and documentation, need to be approved before being accepted by the Project.
    The most common kind of contribution requiring such approval is a github Pull Request (PR); the merging of the PR signifies its approval.
    The duty of a Contributor is to offer a contribution in good faith, to the best of their ability, and to be honest when signing off on the [Developer Certificate of Origin][dco].

- **Committers:** Committers are those individuals with write access to any repository within the Kroxylicious GitHub organisation, except for the repository containing this `GOVERNANCE.md` file.
    These people are listed in [COMMITTERS.md][committers].
    The duty of a Committer is to help Contributors make high quality contributions to the Project.
    As such, Committers are responsible for reviewing and merging contributions. 
    An individual may act as both a Contributor and a Committer for a contribution.
    
- **Project Managers:** Project Managers are Committers who also have write access to the repository containing this `GOVERNANCE.md` file within the Kroxylicious GitHub organisation.
    These people are listed in [PMs.md][PMs].
    Project Managers are tasked with sustaining the project, in part by identifying individuals who have made valuable contributions which further the Project's purpose. 
    They can collectively decide to invite a Contributor to become a Committer; or to invite a Committer to become a Project Manager. 

## Contributing

We welcome all forms of contribution, from code improvements to documentation and design. For details on how to contribute and the process your contributions will follow, please read our [Contributing Guidelines][contrib].

## Decision Making

This project follows The [Commonhaus decision making][cdm] process.

This project uses the following decision making process for PRs in all repositories except for the repository containing this `GOVERNANCE.md`:

1. **Consensus-seeking (lazy consensus):** The project primarily aims for a consensus-based decision-making process, where committers and active contributors discuss and come to an agreement.
2. **Voting:** In situations where consensus cannot be reached about a PR, decisions may be made through a simple majority vote among the committers.
3. **Conflict Resolution:** If conflicts arise, project managers are responsible for facilitating a resolution. The [Commonhaus Foundation Council][cfc] (CFC) can be asked to mediate the discussion, if necessary.

This project uses the following decision making process for PRs in the repository containing this `GOVERNANCE.md`, [COMMITTERS.md][committers] and [PMs.md][PMs] files:

1. **Voting:** Decisions may be made through a simple majority vote among the project managers who participate in a vote, as tallied 7 days after the start of the voting process.
2. **Conflict Resolution:** If conflicts arise, project managers are responsible for facilitating a resolution. The [Commonhaus Foundation Council][cfc] (CFC) can be asked to mediate the discussion, if necessary.

## Becoming a Committer

Existing Committers are encouraged to:

* inform the Project Managers about the review burden they're experiencing.
* suggest to the Project Managers other individuals who they consider meet the Committer criteria below.

The Project Managers should endeavour to match the number of active committers to the reported review burden, by inviting Contributors to become Committers.

New Committers are elected by the Project Managers following the above [Decision Making](#decision-making) process to approve a PR which adds an individual to the [COMMITTERS.md][committers] file.

To ensure that all potential Committers are judged fairly and consistently, the following criteria should be taken into account in electing new Committers:

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

## Becoming a Project Manager

New Project Managers are elected by the existing Project Managers following the above [Decision Making](#decision-making) process to approve a PR which adds an individual to the [PMs.md][PMs] file.

To ensure that all potential Project Managers are judged fairly and consistently, the following criteria (in addition to those for being a Committer) should be taken into account in electing new Project Managers:

* Sustained contributions _as a committer_ over at least 3 months.
* Reviewing and merging other contributors’ non-trivial PRs.
* Knowing when to ask for help or seek consensus.
* Continued commitment to the long term success of the project.

Unlike the situation for Committers, the need for more Project Managers is not driven by the review burden, and is left to the discretion of the existing Project Managers.

The Commonhaus [Extended Governance Committee](https://www.commonhaus.org/bylaws/cf-council.html#extended-governance-committee-egc) has a [primary and secondary](https://github.com/commonhaus/foundation/blob/main/CONTACTS.yaml) representitive from the Project. 
These will be selected from, and by, the Project Managers.
Other aspects of this representation are left to the discretion of the Project Managers using the [Decision Making](#decision-making) process.


## Ceasing participation

A Committer or Project Manager can voluntarily cease their involvement in the project by opening a PR removing themselves from the [COMMITTERS.md][committers] and/or [PMs.md][PMs] files in this repository.
Such PRs will be deemed as approved automatically, without recourse to the [Decision Making](#decision-making) process.

All other changes to the Committers or Project Managers are, by definition, a change to the `COMMITTERS.md` and/or `PMs.md` files in this repo, which are handled by the decision making processes described above.

## Trademark Policy

The Kroxylicious logos, icons, and domain names are protected by trademark rights. Usage of these trademarks must adhere to our [Trademark Policy][ctp].

