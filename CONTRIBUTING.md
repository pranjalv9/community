# Contributing Guidelines

[![](https://img.shields.io/badge/made%20by-Protocol%20Labs-blue.svg?style=flat-square)](http://ipn.io)
[![](https://img.shields.io/badge/project-IPFS-blue.svg?style=flat-square)](http://ipfs.io/)
[![](https://img.shields.io/badge/freenode-%23ipfs-blue.svg?style=flat-square)](http://webchat.freenode.net/?channels=%23ipfs)

![](https://github.com/jbenet/contribute-ipfs-gif/raw/master/img/contribute.gif)

[`IPFS Main Repo`](https://github.com/ipfs/ipfs#ipfs---the-permanent-web) • [`IPFS Project Directory`](https://github.com/ipfs/ipfs#project-directory)

Want to hack on IPFS? Awesome! Here are instructions to get you started. They are not perfect yet. Please let us know what feels wrong or incomplete.

IPFS is an Open Source project and we welcome contributions of all sorts. There are many ways to help, from reporting issues, contributing code, and helping us improve our community.

## Topics

- [Security Issues](#security-issues)
- [Community Guidelines](#community-guidelines)
- [Dive Right In](#dive-right-in)
- [Reporting Issues](#reporting-issues)
- [Protocol Design](#protocol-design)
- [Implementation Design](#implementation-design)
- [Community Improvement](#community-improvement)
- [Translations](#translations)
- [Helping in other ways](#helping-in-other-ways)
- [Code Contribution Guidelines](#code-contribution-guidelines)
  - [Discuss big changes as Issues first](#discuss-big-changes-as-issues-first)
  - [Pull Requests always welcome](#pull-requests-always-welcome)
  - [Conventions](#conventions)
    - [Go Code Contributing Guidelines](#go)
    - [JavaScript  Code Contributing Guidelines](#javascript)
    - [Git](#git)
    - [Commit messages](#commit-messages)
      - [Subject line should not be more than 80 characters long](#subject-line-should-not-be-more-than-80-characters-long)
      - [A "License" and a "Signed-off-by" trailers are required](#a-license-and-a-signed-off-by-trailers-are-required)
      - [Commit message examples](#commit-message-examples)
    - [Code](#code)
    - [Tests](#tests)
    - [Documentation](#documentation)
    - [Pull Requests](#pull-requests)
    - [Code Review](#code-review)
    - [Rebasing](#rebasing)
    - [Merge Approval](#merge-approval)
- [Credits](#credits)


## Security Issues

The IPFS protocol and its implementations are still in heavy development. This means that there may be problems in our protocols, or there may be mistakes in our implementations. And -- though IPFS is not production-ready yet -- many people are already running nodes in their machines. So we take security vulnerabilities very seriously. If you discover a security issue, please bring it to our attention right away!

If you find a vulnerability that may affect live deployments -- for example, expose a remote execution exploit -- please send your report privately to security@ipfs.io, please DO NOT file a public issue. The GPG key for security@ipfs.io is [4B9665FB 92636D17 7C7A86D3 50AAE8A9 59B13AF3](https://pgp.mit.edu/pks/lookup?op=get&search=0x50AAE8A959B13AF3).

If the issue is a protocol weakness or something not yet deployed, just discuss it openly.

## Community Guidelines

We want to keep the IPFS community awesome, growing and collaborative. We need your help to keep it that way. To help with this we've come up with some general guidelines for the community as a whole:

- Be nice: Be courteous, respectful and polite to fellow community members: no regional, racial, gender, or other abuse will be tolerated. We like nice people way better than mean ones!
- Encourage diversity and participation: Make everyone in our community feel welcome, regardless of their background and the extent of their contributions, and do everything possible to encourage participation in our community.
- Keep it legal: Basically, don't get anybody in trouble. Share only content that you own, do not share private or sensitive information, and don't break laws.
- Stay on topic: Make sure that you are posting to the correct channel and avoid off-topic discussions. Remember when you update an issue or respond to an email you are potentially sending to a large number of people. Please consider this before you update. Also remember that nobody likes spam.

There is also a more extensive [code-of-conduct](code-of-conduct.md).

## Dive Right In

If you're curious to hack on IPFS right now and you just need an issue to focus on, check out [this search](https://github.com/search?utf8=%E2%9C%93&q=label%3A%22difficulty%3Aeasy%22+label%3A%22help+wanted%22+user%3AIPFS+is%3Aopen+&type=Issues) for issues tagged as "help wanted". Generally, these should be easier for newcomers, and are great places to start hacking away. Have fun!

## Reporting Issues

If you find bugs, mistakes, inconsistencies in the IPFS project's code or documents, please let us know by filing an issue at the appropriate issue tracker (we use multiple repositories). No issue is too small.

The main issues for bug reporting are as follows:
- [go-ipfs/issues](https://github.com/ipfs/go-ipfs/issues) - Issues related to running the Go implementation of IPFS.
- [js-ipfs/issues](https://github.com/ipfs/js-ipfs/issues) - Issues related to running the js implementation of IPFS.
- [notes/issues](https://github.com/ipfs/notes/issues) - For general notes and ideas.
- [specs/issues](https://github.com/ipfs/specs/issues) - For protocol discussions.

The [go-ipfs](https://github.com/ipfs/go-ipfs) issues use a template that will guide you through the process of reporting a bug. We will be adding this kind of issue template to other repositories as bug reports become more common.

For all other questions/discussions, please visit the [discussion forum](https://discuss.ipfs.io)

## Protocol Design

When considering protocol design proposals, we are looking for:

- A description of the problem this design proposal solves
- Discussion of the tradeoffs involved
- Review of other existing solutions
- Links to relevant literature (RFCs, papers, etc)
- Discussion of the proposed solution

Please note that protocol design is hard, and meticulous work. You may need to review existing literature and think through generalized use cases.

## Implementation Design

When considering design proposals for implementations, we are looking for:

- A description of the problem this design proposal solves
- Discussion of the tradeoffs involved
- Discussion of the proposed solution

## Community Improvement

The IPFS community requires maintenance of various "public infrastructure" resources. These include documentation, github repositories, CI build bots, and more. There is also helping new users with questions, spreading the word about IPFS, and so on. Soon, we will be planning and running conferences. Please get in touch if you would like to help out.

## Translations

Things that are ready to be translated can be found at https://www.transifex.com/ipfs/public/

This community moves very fast and documentation swiftly gets out of date. For
now, we are encouraging would-be translators to hold off from translating large
repositories, unless [they are listed on Transifex](https://www.transifex.com/ipfs/public/).

If you would like to add a translation for a project or a language that is not
on Transifex, please open an issue and ask the leads for a given repository to
get familiar with [ipfs/i18n](https://github.com/ipfs/i18n) before filing a PR,
so that there is no wasted effort.

If anyone has any issues understanding the English documentation, please let us know! We are very sensitive to language issues, and do not want to turn anyone away from hacking because of their language.

## Helping in other ways

Protocol Labs occasionally is able to hire developers for part time or full time positions, to work on IPFS. If you are interested, check out [the job listings](http://protocol.ai/join). If you'd like to help in other ways, propose your ideas on the IPFS forums at https://discuss.ipfs.io.

## Code Contribution Guidelines

### Discuss big changes as Issues first

Significant improvements should be documented as GitHub issues before anybody starts to code. This gives other contributors a chance to point you in the right direction, give feedback on the design, and maybe point out if related work is under way.

Please take a moment to check whether an issue already exists. If it does, it never hurts to add a quick "+1" or "I have this problem too". This helps prioritize the most common problems and requests.

### Pull Requests always welcome

We are always thrilled to receive pull requests, and do our best to process them as quickly as possible. Not sure if that typo is worth a pull request? Do it! We will appreciate it.

If you don't get a response to a pull request within a few days, feel free to mention it in the #ipfs IRC channel. We may be able to get to it faster.

We're also trying very hard to keep IPFS focused. This means that we might decide against incorporating a new feature. However, there might be a way to implement that feature on top of (or below) IPFS.

If your pull request is not accepted on the first try, don't be discouraged! If there's a problem with the implementation, hopefully you received feedback on what to improve.

### Conventions

Each repository will have its own code and test conventions. Please make sure to review those before jumping in. Some general conventions are listed below.

#### Go

Please look at the [Go Contribution Guidelines](./CONTRIBUTING_GO.md).

#### JavaScript

Please look at the [JS Contribution Guidelines](./CONTRIBUTING_JS.md).

#### Git

We use a simple git branching model:

- `master` must always work
- create feature-branches to merge into `master`
- all commits must pass testing so that git bisect is easy to run

Just stay current with master (rebase).

##### Commit messages

Commit messages must start with a short subject line, followed by an optional,
more detailed explanatory text which is separated from the summary by an empty
line.

For some of our repositories (and we'd prefer all), we check commit messages
automatically using [GitCop](https://gitcop.com). This checks that commit
messages are properly written.

**If you are brand new to IPFS**, you'll need to run a script that adds `License` and `Signed-off-by` to each of your commits. These trailers mean that the author agrees with the [Developer Certificate of Origin (DCO)](docs/developer-certificate-of-origin) and with licensing the work under the [MIT license](docs/LICENSE). This is important for our team and our users, legally. The [setup_commit_msg_hook.sh](dev/hooks/setup_commit_msg_hook.sh) script will setup a Git commit-msg hook that will add these trailers to all the commit messages you write in that repository. This is not as complicated as it sounds: it is similar to typing `git commit --signoff` every time you commit. Just download the script and run it once from the root folder of whatever Git repository you are in (for example, go-ipfs, or ipfs).

The Developer Certificate of Origin (DCO) is a document that certifies you own and/or have the right to contribute the work and license it appropriately. The DCO is used instead of a --much more annoying--
[CLA (Contributor License Agreement)](https://en.wikipedia.org/wiki/Contributor_License_Agreement). With the DCO, you retain copyright of your own work :). The DCO originated in the Linux community, and is used by other projects like Git and Docker. To learn more about the DCO see this [posts on elinux.org](http://elinux.org/Developer_Certificate_Of_Origin) or how [docker uses the DCO](https://blog.docker.com/2014/01/docker-code-contributions-require-developer-certificate-of-origin/).

GitCop checks for two possible problems that are described below.

##### Subject line should not be more than 80 characters long

The first line of a commit message, called the subject line, should not be more than 80 characters long and should be separated from the rest of the commit message using an empty blank line.

Most editors can help you count the number of characters in a line. And these days many good editors recognize the Git commit message format and warn in one way or another if the subject line is not separated from the rest of the commit message using an empty blank line.

See also the [documentation about amending commits](https://help.github.com/articles/changing-a-commit-message/) for an explanation about how you can rework commit messages.

##### A "License" and a "Signed-off-by" trailers are required

The commit message should end with the following trailers:

```
License: MIT
Signed-off-by: User Name <email@address>
```

where "User Name" is the author's real (legal) name and email@address is one of the author's valid email addresses.

There should also be an empty blank line before the "License" trailer.

As explained in more details above, this is easy to fix by running once the [setup_commit_msg_hook.sh](dev/hooks/setup_commit_msg_hook.sh) script in your repository.

See also the [documentation about amending commits](https://help.github.com/articles/changing-a-commit-message/) for an explanation about how you can rework commit messages.

##### Commit message examples

Here is an example commit message:

```
parse_test: improve tests with stdin enabled arg

Now also check that we get the right arguments from
the parsing.

License: MIT
Signed-off-by: Christian Couder <chriscool@tuxfamily.org>
```

And here is another longer one:

```
net/p2p + secio: parallelize crypto handshake

We had a very nasty problem: handshakes were serial so incoming dials would wait for each other to finish handshaking. this was particularly problematic when handshakes hung-- nodes would not recover quickly. This led to gateways not bootstrapping peers fast enough.

The approach taken here is to do what crypto/tls does: defer the handshake until Read/Write[1]. There are a number of reasons why this is _the right thing to do_:
- it delays handshaking until it is known to be necessary (doing io)
- it "accepts" before the handshake, getting the handshake out of the
  critical path entirely.
- it defers to the user's parallelization of conn handling. users
  must implement this in some way already so use that, instead of
  picking constants surely to be wrong (how many handshakes to run
  in parallel?)

[0] http://golang.org/src/crypto/tls/conn.go#L886

License: MIT
Signed-off-by: Juan Benet <juan@ipfs.io>
```

### Code

Write clean code. Universally formatted code promotes ease of writing, reading, and maintenance.

### Tests

If the repository you are working on has a testing suite, submit tests with your changes. Take a look at existing tests for inspiration. Run the full test suite on your branch before submitting a pull request.

For command line tool changes, please write appropriate sharness tests.

### Documentation

Update documentation when creating or modifying features. Test your documentation changes for clarity, concision, and correctness, as well as a clean documentation build.

### Pull Requests

Pull requests descriptions should be as clear as possible. Err on the side of overly specific and include a reference to all related issues. If the pull request is meant to close an issue please use the Github keyword conventions of [closes, fixes, or resolves]( https://help.github.com/articles/closing-issues-via-commit-messages/). If the pull request only completes part of an issue use the [connects keywords]( https://github.com/waffleio/waffle.io/wiki/FAQs#prs-connect-keywords). This helps our tools properly link issues to pull requests. 

### Code Review

We take code quality seriously; we must make sure the code remains correct. We do code review on all changesets. Discuss any comments, then make modifications and push additional commits to your feature branch. Be sure to post a comment after pushing. The new commits will show up in the pull request automatically, but the reviewers will not be notified unless you comment.

We use the `needs review` as a signal that something needs review. If you can't add one to your own PR, feel free to request that the maintainers add the label to it.

### Rebasing

Pull requests **must be cleanly rebased ontop of master** without multiple branches mixed into the PR. If master advances while your PR is in review, please keep rebasing it. It makes all our work much less error-prone.

Before the pull request is merged, make sure that you squash your commits into logical units of work using `git rebase -i` and `git push -f`. After _every commit_ the test suite must be passing. This is so we can revert pieces, and so we can quickly bisect problems. Include documentation changes and tests in the same commit so that a revert would remove all traces of the feature or fix.

### Merge Approval

We use LGTM (Looks Good To Me) in comments on the code review to indicate acceptance. A change **requires** LGTMs from the maintainers of each component affected. If you know whom it may be, ping them. 

### Reverting Changes

When some change is introduced, and we decide that it isn't beneficial and/or it causes problems, we need to revert it.

To make the review process and the changes easier, use git's `revert` command to revert those changes.

This suits a few purposes. First, it is much easier to see if some change was reverted by just looking into the history of the file. Imagine a commit with the title: _Add feature C_. There are many ways one could form the title for a commit reverting it, but by using `git revert`, it will be _Revert: "Add feature C"_ and thus very clear.
Second, by using `git revert` we are sure that all changes were reverted. It is much easier to start again for state 0 and apply changes on it, than try to see if some transformation transforms state 1 to state 0.

#### What if a commit that is supposed to be reverted contains changes that are also good?

This usually means that commit wasn't granular enough. If you are the person that initially created the commit, in the future try to make commits that focus on just one aspect.

This doesn't mean that you should skip using `git revert`. Use it, then use `git cherry-pick --no-commit` to pull changes into your working tree and use interactive add to commit just the wanted ones. If interactive add is not enough to split the changes, still use interactive add to stage a superset of wanted changes and use `git checkout -- <file>` to remove unstaged changes. Then proceed to edit the files to remove all unwanted changes, and add and commit only your wanted changes.

This way your log will look like:

```
AAAAAA Revert "Fix bug C in A"
BBBBBB Re-add feature A tests that were added in "Fix bug C in A"
```

## Credits

This document is based on [Contributing to Docker](https://github.com/docker/docker/blob/master/CONTRIBUTING.md), the [Docker](https://github.com/docker/docker) contribution guidelines.
