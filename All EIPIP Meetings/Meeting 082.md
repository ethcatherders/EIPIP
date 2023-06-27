# EIP Improvement Process Call #82 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, May 31, 2023 at 14:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://youtu.be/1IsNR4ZpCPk) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/235) <!-- omit in toc -->
### Moderator: Pooja Ranjan <!-- omit in toc -->
### Notes: Edson Ayllon <!-- omit in toc -->

----

# Summary <!-- omit in toc -->

## DECISION ITEMS <!-- omit in toc -->
Decision Item | Description
-|-
82.1 | Links to unmerged spec are allowed in Draft EIPs as long as the link contains the diff and commit hash
82.2 | ERCs should have a reference implementation before going to review, though it's not a strict requirement

---

# Contents <!-- omit in toc -->

- [1. Discuss Open Issues/PRs, and other topics](#1-discuss-open-issuesprs-and-other-topics)
  - [Patents: Add EIP: Asset-bound Non-Fungible Tokens ethereum/EIPs#6956 (comment)](#patents-add-eip-asset-bound-non-fungible-tokens-ethereumeips6956-comment)
  - [Issue with Auto Review bot](#issue-with-auto-review-bot)
  - [Issues with CL Link Validation](#issues-with-cl-link-validation)
  - [ERC's status advancement criteria Ref: Comment](#ercs-status-advancement-criteria-ref-comment)
  - [Changes to Final proposal; Update EIP-2612: fix misplaced bracket ethereum/EIPs#7077](#changes-to-final-proposal-update-eip-2612-fix-misplaced-bracket-ethereumeips7077)
  - [Decisions](#decisions)
- [Annex](#annex)
  - [Attendees](#attendees)
  - [Next Call](#next-call)

---



# 1. Discuss Open Issues/PRs, and other topics

Video | [0:00](https://youtu.be/1IsNR4ZpCPk)
-|-

## Patents: Add EIP: Asset-bound Non-Fungible Tokens ethereum/EIPs#6956 (comment)

Video | [0:25](https://youtu.be/1IsNR4ZpCPk?t=25)
-|-


Has already been [merged](https://github.com/ethereum/EIPs/pull/6956).

## Issue with Auto Review bot 

Video | [0:38](https://youtu.be/1IsNR4ZpCPk?t=38)
-|-

[Ref. here](https://discord.com/channels/916516304972824576/916713912970412103/1113084522175676496).


Will return to this topic when Matt joins the call.

Lightclient says there are still problems with the bots. One being having to close a PR, then re-open for the PR to be merged.


## Issues with CL Link Validation 

Video | [1:14](https://youtu.be/1IsNR4ZpCPk?t=74)
-|-


[ethereum/EIPs#7064](https://github.com/ethereum/EIPs/issues/7064)

Issue created by Tim Beiko. Also discussed on EIP office hours.

When people draft PRs, they mention pull requests. The expectation is that these proposals should be allowed in Draft. In draft there is discussion going on. PRs may be covering a large number of files.

This would add one comit to the EIP specification. 

Sam has a concern with allowing links in draft, and removing them going into review. One, things stay in Draft longer than they should. And the other one, is it may prevent an EIP going to Review when it should be able to. But those are minor concerns.

Has a concern relaxing standards in draft may lead to more relaxing in the future. 

Victor is for allowing more EIPs to enter draft.

Gajinder is also in favor of this.

Lightclient had questions of how useful this would be. And examples were given. Lightclient then was confused why they didn't merge the two examples that linked to a PR.

Lightclient doesn't think we should be adding diffs to EIPs like this.

Lightclient and Sam doesn't think we should allow links to Pull Requests. Victor is for them.

Greg is confused on why we would link to PRs instead of the latest spec. Greg sounds like he's for it.

Lightclient thinks this is an issue with the process, and solving it by linking to a PR isn't the correct solution.

Victor disagrees with blocking this.

Greg wants to allow it. Sam suggests they link to the most recent commit of the PR. The alternative is you can't add the draft until the consensus spec it's referring to is merged.

Sam thinks you should link to the commit in the PR, because PRs can have more commits added, which would confuse the discussion.

Greg sees a problem when a consensus spec and an execution spec that depend on each other can't be moved to final unless both are moved together. Both of them enter a limbo.

Sam is for linking to consensus specs, just not linking to PRs.

Pooja suggests allowing this, but enforcing it through the bot to make sure the link PR is merged before changing state. Which is what the proposal was.

I think the consensus is to link to the diff instead of the PR.

Lightclient asks if that's what the bot is already checking for.

The diff has the master, and the commit.

Sam is ok with the link, as long as it has a commit hash.

The link wouldn't be to the pull request, but can go to the commit in the pull request.

Greg thinks these problems won't fully resolve until we pull the consensus specs into the EIP process.

Sam states that the consensus outside of the EIP editors is to not pull together the processes more than they already are.

## ERC's status advancement criteria Ref: Comment

Video | [29:36](https://youtu.be/1IsNR4ZpCPk?t=1775)
-|-

[Proposed by Victor](https://ethereum-magicians.org/t/discussion-of-guideline-for-advancing-eip-status-a-straw-man-proposal/11995).

Vcitor made a presentation for this, powerpoint.

The goal is to improve how ERCs can move through statuses.

Common practice is to require adoption to finalize. Implied requirements are soundness and usefulness.

RFCs are also doing it. They require 2 independent implementations to be considered a standard.

Proposal is no requirement for a draft, require 1 implementation to move to Review, and 2 or 3 independent implementation to go to Last Call.

The open question is how many implementations should we require, if at all.

And should we use the word "status" or shoulde we create a different preamble. 

Sam asks, how much work is required to verify that a reference implementation is actually a reference implementation?

The mandate to require a reference implementation would bring more overheard to the editors, or technical peer reviewers. That could be solved if we have a boundary of what to review.

Greg says this looks good. Doesn't see much problem with it. The status boundaries are fine as they are now. Greg sees that if it runs on mainnet and passes test cases, it's an implementation. Greg thinks that should be a requirement before going to review.

Lightclient thinks 3 is too high.

Sam asks if the test cases need to run against the 3 implementations? Victor thinks we can ask the author to do that for the editors, shift the overheard to the author. The author writes the test cases, and the implementors can see if they comply.

Sam says it sounds like we're asking authors to ask chatgpt to re-write their reference implementation 3 times. This will work for good-faith authors. Bad faith authors can create multiple accounts for the reference implementations. Like a civil attack.

The alternative is we don't require it. Having the requirement for the reference implementation is no worse than the current scenario.

If we treat it as a security problem, we can't fully prevent it. But, most authors have track records. 

Sam asks what the goal is for getting more than 1 reference implementation.

Victor says the move from status to status seems arbitrary based on the editor. The goal is to make it less arbitrary.

Lightclient asks what problem this is solving. Sam and Victor state subjectivity. Lightclient says we don't have many ERCs going to final. 

Victor states, we don't have many requirements for moving things to final. It's subjective, doesn't check for soundness, or usefulness.

Sam, when he reviews, asks if there is a minimum of multiple consumers/implementors. And does it meet the formatting requirements, in addition to proofreading and grammar.

Sam doesn't think checking for multiple implementors requires multiple people to actually implement it. Just to write reasoning on who the target implementors are. Victor states that is pretty subjective.

Sam thinks the problem Victor is trying to solve is increasing the reputation of EIPs. While, Sam thinks anyone can apply ERCs, we approve them, and then the market decides on the usefulness once live.

The link argument came up. Linking is about the process, not the EIPs itself. So EIPs gaurantee availability but not soundness.

Greg would be happy enough to see a requirement for one reference implementation and test cases. Greg doesn't see the need for multiple implementations. Teams don't want to implement something that isn't already a standard or close to it.

Sam isn't strongly objecting to requiring one. He's slightly negative, but not blocking it.

Lightclient thinks editors should enforce it themselves, make the suggestion and not a requirement. Make it a should, not a must.

Victor wants to put this suggestion in EIP-1.

Greg is happier with must, but should is strong enough. And if it does help, we can move it to must. It would help with the current process.

## Changes to Final proposal; Update EIP-2612: fix misplaced bracket ethereum/EIPs#7077

Video | [55:17](https://youtu.be/1IsNR4ZpCPk?t=3317)
-|-

This has already been moved to Final.

It's just formating changes, and moving a bracket to a new line. It'll need an author approval before merging, then it can be merged.

## Decisions

- 82.1 - Links to unmerged spec are allowed in Draft EIPs as long as the link contains the diff and commit hash
- 82.2 - ERCs should have a reference implementation before going to review, though it's not a strict requirement


---

# Annex

## Attendees 

- Pooja Ranjan
- gcolvin
- TB
- maintainer.eth
- gajinder
- tl;dv
- lightclient
- Sam
- Victor Zhao


## Next Call 

June 14, 2023, 14:00 UTC.

