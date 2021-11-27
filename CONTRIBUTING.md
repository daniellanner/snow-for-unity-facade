# Contributing to SnowFS for Unity

:heart: A big welcome and thank you for considering contributing to **SnowFS for Unity** :heart:

Reading and following these guidelines will help us make the contribution process easy and effective for everyone involved. It also communicates that you agree to respect the time of the developers managing and developing these open-source projects. In return, we will reciprocate that respect by addressing your issue, assessing changes, and helping you finalize your pull requests.

## Table of Content

- [Contributing to SnowFS for Unity](#contributing-to-snowfs-for-unity)
  - [Table of Content](#table-of-content)
  - [Code of Conduct](#code-of-conduct)
  - [Getting Started](#getting-started)
    - [Issues](#issues)
    - [Commit Messages](#commit-messages)
      - [Format of commit messages](#format-of-commit-messages)
      - [Wording of commit messages](#wording-of-commit-messages)
      - [Commit Prefixes](#commit-prefixes)
    - [Pull Requests](#pull-requests)
  - [Getting Help](#getting-help)

## Code of Conduct

We take our open-source community seriously and hold ourselves and other contributors to high standards of communication. By participating and contributing to this project, you agree to uphold our [Code of Conduct](CODE-OF-CONDUCT.md).

## Getting Started

Contributions are made to this repo via Issues and Pull Requests (PRs). A few general guidelines that cover both:

- Search for existing Issues and PRs before creating your own.
- We work hard to makes sure issues are handled in a timely manner but, depending on the impact, it could take a while to investigate the root cause. A friendly ping in the comment thread to the submitter or a contributor can help draw attention if your issue is blocking.
- If you've never contributed before, see [the first timer's guide on the *auth0* blog](https://auth0.com/blog/a-first-timers-guide-to-an-open-source-project/) for resources and tips on how to get started.

### Issues

Issues should be used to report problems with the library, request a new feature, or to discuss potential changes before a PR is created. When you create a new Issue, a template will be loaded that will guide you through collecting and providing the information we need to investigate.

If you find an Issue that addresses the problem you're having, please add your own reproduction information to the existing issue rather than creating a new one. Adding a [reaction](https://github.blog/2016-03-10-add-reactions-to-pull-requests-issues-and-comments/) can also help be indicating to our maintainers that a particular problem is affecting more than just the reporter.

### Commit Messages

#### Format of commit messages

- A commit message consists of a subject line and a description
- Separate subject from description with a blank line
- Limit the subject line to 50 characters
- Capitalize the subject line
- Do not end the subject line with a period
- Wrap the description at 72 characters
- Use the description to explain what and why vs. how

#### Wording of commit messages

- Use the present tense ("Add feature" not "Added feature")
- Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
- Do not reference issues and pull requests within the subject line
- Reference issues and pull requests liberally within the description

A properly formed Git commit subject line should always be able to complete the following sentence:

"*If applied, this commit will* \<insert your subject line here\>"

**Example**
*If applied, this commit will* update documentation for readability ✔️
*If applied, this commit will* updated documentation for readability ❌
*If applied, this commit will* documentation being updated to know wtf is going on ❌

#### Commit Prefixes

Optionally you can add an applicable emoji to your commit message (recommended for squashed or large commits containing significant amount of changes)

- :star: `:star:` when adding a feature
- :memo: `:memo:` when writing docs
- :bug: `:bug:` when fixing a bug
- :green_heart: `:green_heart:` when improving configuration
- :broom: `:broom:` when refactoring or fixing code smells
- :racehorse: `:racehorse:` when improving performance
- :non-potable_water: `:non-potable_water:` when plugging memory leaks
- :penguin: `:penguin:` when fixing something on Linux
- :apple: `:apple:` when fixing something on macOS
- :checkered_flag: `:checkered_flag:` when fixing something on Windows
- :wastebasket: `:wastebasket:` when removing code or files
- :robot: `:robot:` when fixing the CI/CD
- :white_check_mark: `:white_check_mark:` when adding tests
- :lock: `:lock:` when dealing with security
- :arrow_up: `:arrow_up:` when upgrading dependencies
- :arrow_down: `:arrow_down:` when downgrading dependencies
- [WIP] `[WIP]` when submitting work in progress in feature branches
- No prefix when submitting small self-contained work in feature branches

### Pull Requests

PRs to our libraries are always welcome and can be a quick way to get your fix or improvement slated for the next release. In general, PRs should:

- Only fix/add the functionality in question **OR** address wide-spread whitespace/style issues, not both.
- Add unit or integration tests for fixed or changed functionality (the test strategy for *SnowFS for Unity* is currently still under consideration).
- Address a single concern in the least number of changed lines as possible.
- Include documentation in the [`docs`](./docs).
- Be accompanied by a complete Pull Request template (loaded automatically when a PR is created).

For changes that address core functionality or would require breaking changes (e.g. a major release), it's best to open an Issue to discuss your proposal first. This is not required but can save time creating and reviewing changes.

In general, we follow the ["fork-and-pull" Git workflow](https://github.com/susam/gitpr).

1. Fork the repository to your own Github account
2. Clone the project to your machine
3. Create a branch locally with a succinct but descriptive name
4. Commit changes to the branch
5. Following any formatting and testing guidelines specific to this repo
6. Push changes to your fork
7. Open a PR in our repository and follow the PR template so that we can efficiently review the changes.

## Getting Help

Join us on [Discord](https://discord.gg/RDKPuH8dkA) and post your question there in the correct category with a descriptive tag.
