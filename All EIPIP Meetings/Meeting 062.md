# EIP Improvement Process Call #62 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, Aug 10, 2022 at 14:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://youtu.be/3uizzELjrAY) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/168) <!-- omit in toc -->
### Moderator: Pooja Ranjan <!-- omit in toc -->
### Notes: Edson Ayllon <!-- omit in toc -->

----

# Summary <!-- omit in toc -->

## DECISION ITEMS <!-- omit in toc -->
Decision Item | Description
-|-
62.1 | Decision was against auctioning past EIP numbers
62.2 | Bot to assign future EIP numbers
62.3 | The group decided not to be too strict whether the author refers to it as EIP or ERC. 
62.4 | Halt discussion of Executable Spec inside EIPIP


## ACTION ITEMS <!-- omit in toc -->
Action Item | Description
-|-
62.1 | Make a bot that counts up and assigns numbers at merge time. The decision is to be regardless of PR number, so there's no more gaps.
62.2 | Change branch protection settings after https://github.com/ethereum/EIPs/pull/5400 is merged.
62.3 | Continue discussion off call as to what license to use for EIP assets.
62.4 | Add ECH Discord Channel to EIP Page Index 
62.5 | Create Meta EIP for Executable spec.


---

# Contents <!-- omit in toc -->

- [1. Make EIP authorship depend on ENS](#1-make-eip-authorship-depend-on-ens)
- [2. From GitHub Issue or Pull Request](#2-from-github-issue-or-pull-request)
  - [How should we pick EIP numbers?](#how-should-we-pick-eip-numbers)
  - [Fix EIP Bot](#fix-eip-bot)
  - [Use settings.yml ethereum/EIPs#5414 & Add settings.yml ethereum/EIPs#5422 Discussion Thread](#use-settingsyml-ethereumeips5414--add-settingsyml-ethereumeips5422-discussion-thread)
  - [Add License Checker](#add-license-checker)
  - [Add ECH Discord Channel to EIP Page Index](#add-ech-discord-channel-to-eip-page-index)
  - [[Bug]: Explain in text that ERC was renamed to EIP](#bug-explain-in-text-that-erc-was-renamed-to-eip)
  - [Create an EIP ExternalLinkArchiveBot (EIP ELABot)](#create-an-eip-externallinkarchivebot-eip-elabot)
  - [PandaPip1 added as a maintainer of the EIP-Bot repository.](#pandapip1-added-as-a-maintainer-of-the-eip-bot-repository)
  - [Remove Contributors section from README](#remove-contributors-section-from-readme)
  - [Actions](#actions)
  - [Decisions](#decisions)
- [3. EIP bots related discussion, updates, agreement on merging PRs & closing Issues.](#3-eip-bots-related-discussion-updates-agreement-on-merging-prs--closing-issues)
- [4. Past meeting discussion continued](#4-past-meeting-discussion-continued)
  - [Meta EIP for the Executable Spec process for Core EIPs](#meta-eip-for-the-executable-spec-process-for-core-eips)
  - [Actions](#actions-1)
  - [Decisions](#decisions-1)
- [5. EIPs Insight - Monthly EIPs status reporting.](#5-eips-insight---monthly-eips-status-reporting)
- [6. Review action items from the previous meeting](#6-review-action-items-from-the-previous-meeting)
- [Annex](#annex)
  - [Attendees](#attendees)
  - [Next Call](#next-call)

---

# 1. Make EIP authorship depend on ENS

Video | [0:00](https://youtu.be/3uizzELjrAY)
-|-

If there's no mechanism to enforce that a person has ownership of an ENS name, then it's not doing its job, and only adding an extra step.

And if its not required, then Lightclient doesn't think there's a reason to do so.

It may add more work to the process.

Gavin John brought up that this may be a solution if Github bans the Ethereum repo like they did Tornado Cash. 

This then brought the conversation to how to backup the EIP repo, as it was suggested this issue does not actually solve a Tornado Cash event.

Discussion ended there. Further discussion can be done in the EIP repository.


# 2. From GitHub Issue or Pull Request

Video | [4:53](https://youtu.be/3uizzELjrAY?t=293)
-|-

## How should we pick EIP numbers? 

[ethereum/EIPs#5294](https://github.com/ethereum/EIPs/issues/5294). 

No conclusion yet. This was suggested by Sam. There was discussion on making a bot for it. There was discussion around if there was a conflict between this direction and having EIP numbers be NFTs. Sam was for the simplest solution, having the EIP number be on a counter, but wasn't opposed to it. 

Tim talked to the NFT idea with client devs, and there was pushback. They said this isn't a decision an EIP editor should make. If we did go down the NFT route, we should get much broader input on it. If we decide to do it, but don't tell more people, there will be frustration. This requires a broader buy in. It's bad if we auction off NFTs, and then there's pushback.

Tim thinks the core devs don't care how the EIP numbers are assigned, but may be opposed to selling the numbers. Some NFTs would be free, and the notable ones would be auctioned.

Tim thinks we should consult the core devs first. 

Greg is opposed to it, and signaled he wouldn't agree to it. Greg is opposed into going back in the sequence and getting old numbers from the gaps. He's more for using a bot to assign new numbers.

The decision for now is to make a bot that counts up and assigns numbers at merge time. The decision is to be regardless of PR number, so there's no more gaps.


## Fix EIP Bot

https://github.com/ethereum/EIPs/pull/5400

PR is ready. Micah wants an additional EIP editor to approve before merge. Lightclient will look at it.

After the PR is merged, there will need to be changes to the branch protection settings.

## Use settings.yml ethereum/EIPs#5414 & Add settings.yml ethereum/EIPs#5422 Discussion Thread

- https://github.com/ethereum/EIPs/issues/5414
- https://github.com/ethereum/EIPs/pull/5422

Discussion for these happening on EIP issues and ECH discord.

## Add License Checker 

[ethereum/EIPs#5379](https://github.com/ethereum/EIPs/pull/5379)

Micah had objected to this. So the scope was changed to being CC0 1.0. This forces you to write identifiers.

Sam doesn't think we should limit to CC0, and it should be any open source license that isn't copy left. 

Currently, EIP-1 states that the EIP needs to be CC0, not that the assets need to be. Any assets linked in the EIP isn't part of the EIP itself.

Continue discussion off call as to what license to use for EIP assets.

## Add ECH Discord Channel to EIP Page Index 

[ethereum/EIPs#5415](https://github.com/ethereum/EIPs/pull/5415)

This was there for the apprenticeship meeting. But it may be good to have a broader consensus on this.

A link to the EIP gitter is there (Gitter is no longer used). Decision if the gitter is there, then we can put the ECH discord there.

## [Bug]: Explain in text that ERC was renamed to EIP 

[ethereum/EIPs#5424](https://github.com/ethereum/EIPs/issues/5424)

Sam doesn't really care what people refer to outside of the markdown file. Everything in the repo should be referred to as EIP. We also shouldn't refer to issues as EIPs. 

If people want to merge legacy issues in withdrawn state, we should allow that.

Greg brings up ERCs cluttering the EIP repo from the core EIPs.

The bot for EIP vs ERC, it needs test written. Right now the bot is EIP only. EIP-1 says it needs to be referred to with EIP.

The group decided not to be too strict whether the author refers to it as EIP or ERC. 

## Create an EIP ExternalLinkArchiveBot (EIP ELABot) 

[ethereum/EIPs#5408](https://github.com/ethereum/EIPs/issues/5408)

Sam Wilson says this is out of scope for the EIP editors. If someone wants to pursue it, they can.

## PandaPip1 added as a maintainer of the EIP-Bot repository. 

There is an ongoing discussion on [Discord](https://discord.com/channels/916516304972824576/916713912970412103/1005597767588134962).

There seems to be consensus among EIP editors.

This is so PandaPip1 can merge pull requests, as Micah is the only one who can do that currently.

Pooja has already asked the devops team to give access to Sam Wilson.

PandaPip1 is not requesting admin permissions. But he is requesting write permissions.

PandaPip1 reported he already has write access.

## Remove Contributors section from README

Pooja wants this section removed.

PandaPip1 suggests that people can go into the repo, and look at insights. Victor is in favor of maintaining a contributors list. Victor wants it maintained somewhere, doesn't need to be in the readme. PandaPip1 says it's already in the Repo public analytics.


## Actions

- 62.1 - Make a bot that counts up and assigns numbers at merge time. The decision is to be regardless of PR number, so there's no more gaps.
- 62.2 - Change branch protection settings after https://github.com/ethereum/EIPs/pull/5400 is merged.
- 62.3 - Continue discussion off call as to what license to use for EIP assets.
- 62.4 - Add ECH Discord Channel to EIP Page Index 

## Decisions 

- 62.1 - Decision was against auctioning past EIP numbers
- 62.2 - Bot to assign future EIP numbers
- 62.3 - The group decided not to be too strict whether the author refers to it as EIP or ERC. 

# 3. EIP bots related discussion, updates, agreement on merging PRs & closing Issues.

Video | [42:33](https://youtu.be/3uizzELjrAY?t=2553)
-|-

Looking to reach consensus to merge these PRs.

eip-bot [Issues](https://github.com/ethereum/EIP-Bot/issues) and [Pull Request](https://github.com/ethereum/EIP-Bot/pulls)

Remove Outdated Assertions [ethereum/EIP-Bot#109](https://github.com/ethereum/EIP-Bot/pull/109) (Fully E2E tested, confirmed working) already merged.

Require multiple editor approvals to merge unknown files ethereum/[EIP-Bot#105](https://github.com/ethereum/EIP-Bot/pull/105) (Added test cases, they pass). Micah didn't want this merged until there was full testing on it. PandaPip1 did some automated tests with no editors approve, and 1-3 editors approving. 

JA suggested that if he did do the tests, all he needed to do was document the PR with the test. That was the last instruction from Micah. That's the standard procedure.

PandaPip1 says it's fine, but why add the test cases if we're doing tests manually as well?

The rational of adding automated tests is for making it easier for future contributors.

PandaPip1 set up a clone of the EIP repo, then had Sam approve a change with an EIP number, and saw if the bot made changes.

Decision was to merge.

Remove contributors list [ethereum/EIP-Bot#111](https://github.com/ethereum/EIP-Bot/pull/111) (Doesn't change code)

# 4. Past meeting discussion continued

Video | [54:09](https://youtu.be/3uizzELjrAY?t=3249)
-|-

## Meta EIP for the Executable Spec process for Core EIPs

Was discussed on the ACD last Thursday. Do we continue discussion on EIPIP?

From the Core Dev meeting, people were generally in favor. The one thing left is the creation of the Meta EIP.

There still isn't a possible proposal yet.

We don't need to continue discussion in EIPIP, and can pick it up again after a Meta EIP is drafted.

## Actions

- 62.5 - Create Meta EIP for Executable spec.

## Decisions

- 62.4 - Halt discussion of Executable Spec inside EIPIP

# 5. EIPs Insight - Monthly EIPs status reporting.

Video | [56:16](https://youtu.be/3uizzELjrAY?t=3376)
-|-

See changes here: https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/https%3A%2F%2Fhackmd.io%2F%40poojaranjan%2FEIPsInsightAugust2022. 

# 6. Review action items from the previous meeting
Sam Wilson and Tim Beiko will create a Meta EIP for the Executable Spec process before showing the proposal to the core devs. Remaining EIP editors to give their view on using the executable spec in the EIP process

Discussed already.

---

# Annex

## Attendees 

- Pooja Ranjan
- Sam Wilson
- Tim Beiko
- Greg Colvin
- Lightclient
- JA
- PandaPip1
- Victor Zhou
- Anett Rolikova


## Next Call 

Aug 24, 2022, 15:00 UTC.

