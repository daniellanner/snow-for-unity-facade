![](../readme-header.jpg) Artwork by [Firman Hatibu](https://www.instagram.com/firmanhatibu/?hl=en)

# SnowFS for Unity - FAQ

> ❗ ***Disclaimer** This project is in alpha state and is being actively developed. Do not use this project in a production environment and without backups of your data.* ❗

- [SnowFS for Unity - FAQ](#snowfs-for-unity---faq)
  - [What is *SnowFS for Unity*?](#what-is-snowfs-for-unity)
  - [What exactly is *SnowFS*?](#what-exactly-is-snowfs)
  - [How does it work?](#how-does-it-work)
  - [Why not git or p4?](#why-not-git-or-p4)
  - [I heard git had branching and merging. Can I merge branches in *SnowFS*?](#i-heard-git-had-branching-and-merging-can-i-merge-branches-in-snowfs)
  - [Does *SnowFS for Unity* have remote backup features?](#does-snowfs-for-unity-have-remote-backup-features)
  - [What Unity versions is *SnowFS for Unity* compatible with?](#what-unity-versions-is-snowfs-for-unity-compatible-with)
  - [What platforms is *SnowFS for Unity* compatible with?](#what-platforms-is-snowfs-for-unity-compatible-with)
  - [Can I share the versions created with *SnowFS for Unity* with others?](#can-i-share-the-versions-created-with-snowfs-for-unity-with-others)
  - [Can I use *SnowFS for Unity* with other version control tools?](#can-i-use-snowfs-for-unity-with-other-version-control-tools)
  - [I encountered a bug. How can I report it?](#i-encountered-a-bug-how-can-i-report-it)
  - [I have an idea for a feature. Where can I suggest it?](#i-have-an-idea-for-a-feature-where-can-i-suggest-it)

## What is *SnowFS for Unity*?

*SnowFS for Unity* is a rapid versioning tool to save snapshots and rollback to earlier states. It is local-only versioning with a focus on increasing single-user iterations. *SnowFS for Unity* is an integration of [*SnowFS*](https://github.com/Snowtrack/SnowFS) in the Unity editor. It is essentially a wrapper for the *SnowFS* CLI tool and helps visualize and interact with your `.snow` repository.

## What exactly is *SnowFS*?

[*SnowFS*](https://github.com/Snowtrack/SnowFS) is a high-performance command-line application and node library for Windows, macOS and Linux with a focus on binary file versioning. It is made for the graphics industry and is developed as an open-source project.

## How does it work?

Every commit of [*SnowFS*](https://github.com/Snowtrack/SnowFS) is a snapshot of changed files which are stored as objects in a local `.snow` repository. These files are backed up and can later be restored. No data is ever deleted. If you are familiar with [git](https://git-scm.com/), this will ring a bell.

## Why not git or p4?

Firstly, while the implementations of [git](https://git-scm.com/) and [p4](https://www.perforce.com/products/helix-core-apps/command-line-client) are excellent version control systems, [*SnowFS*](https://github.com/Snowtrack/SnowFS) addresses the technical challenges for graphic files by its core design.

Secondly, git and p4 come with a set of powerful features for collaboration and branch management. Unfortunately, these features are too unpractical and complicated for most people to feel safe when working with these systems. *SnowFS* focuses on an exclusive subset of features which are important for an artists workflow.

## I heard git had branching and merging. Can I merge branches in *SnowFS*?

*SnowFS for Unity* will automatically branch out to ensure the cleanest history of your project. You will never have to manually manage any branches. [*SnowFS*](https://github.com/Snowtrack/SnowFS) does not support merging of branches. It is highly specialized for artist workflows where merging branches is uncommon.

To transfer changes between commits, we encourage artists to restore a version and copy whatever data is needed. Then restore a different commit and paste the data.

## Does *SnowFS for Unity* have remote backup features?

[*SnowFS*](https://github.com/Snowtrack/SnowFS) does not offer any capabilities for remote repositories nor does it *currently* offer a syncing or backup strategy.
## What Unity versions is *SnowFS for Unity* compatible with?

The *SnowFS for Unity* CI/CD is built against the LTS versions of Unity 2018, Unity 2019 and Unity 2020. Hence, we are very confident *SnowFS for Unity* is compatible with every Unity version after the 2017 cycle.

## What platforms is *SnowFS for Unity* compatible with?

*SnowFS for Unity* is available for the following systems:

**Windows**
- Windows 8.1
- Windows 10

**MacOS**
- High Sierra
- Catalina
- Big Sur

**Linux**
- Ubuntu
- CentOS
- Fedora
- Debian

## Can I share the versions created with *SnowFS for Unity* with others?

Naturally. In case you want to share your history and all versions of your project with somebody, you can send them your `.snow` directory. The other person needs the *SnowFS for Unity* plugin installed.

## Can I use *SnowFS for Unity* with other version control tools?

*SnowFS for Unity* does not replace your teams current collaboration tool. This plugin supports artists and designers to avoid overly complicated technical workflows of established version control tools for **local development only**.

*SnowFS for Unity* works uses a `.snow` repository in the root directory of your project. Per default this hidden directory is not tracked by git or p4 repositories. This enables you to rapidly iterate on your ideas locally until you are ready to submit with your teams collaboration tool.

Depending on your setup you may want to add *.snow/* to your repository ignore file. Naturally, you can import and work on your `.snow` repository with [*Snowtrack*](https://snowtrack.io/).

## I encountered a bug. How can I report it?

[Issues](https://github.com/daniellanner/snowfs-for-unity/issues) should be used to report problems with the library, request a new feature, or to discuss potential changes before a PR is created. When you create a new Issue, a template will be loaded that will guide you through collecting and providing the information we need to investigate.

If you find an Issue that addresses the problem you're having, please add your own reproduction information to the existing issue rather than creating a new one. Adding a [reaction](https://github.blog/2016-03-10-add-reactions-to-pull-requests-issues-and-comments/) can also help be indicating to our maintainers that a particular problem is affecting more than just the reporter.

Alternatively, you can use the [*bug report tool*](meta.md#report-a-bug) by selecting *Report a bug* in the extended menu of the editor window.

## I have an idea for a feature. Where can I suggest it?

As with bugs use [issues](https://github.com/daniellanner/snowfs-for-unity/issues) to discuss potential changes before a PR is created. Additionally, hop on over to the [official Discord server](https://discord.gg/RDKPuH8dkA) to discuss and share your ideas for [*Snowtrack*](https://snowtrack.io/), [*SnowFS*](https://github.com/Snowtrack/SnowFS), *SnowFS for Unity*, and future plugins.

---

Back to [`docs`](../docs)
