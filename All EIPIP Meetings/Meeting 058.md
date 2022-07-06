# EIP Improvement Process Call #58 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, June 15, 2022 at 14:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://youtu.be/--jGL4_PCac) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/146) <!-- omit in toc -->
### Moderator: Pooja Ranjan <!-- omit in toc -->
### Notes: Edson Ayllon <!-- omit in toc -->

----

# Summary <!-- omit in toc -->

## ACTION ITEMS <!-- omit in toc -->
Action Item | Description
-|-
58.1 | Pooja will collect feedback regarding one time NFT sale of unused EIP numbers.
58.2 | Sam Wilson and Tim Beiko will create a Meta EIP for the Executable Spec process before showing the proposal to the core devs
58.3 | Remaining EIP editors to give their view on using the executable spec in the EIP process

---

# Contents <!-- omit in toc -->

- [1. PRs need discussion](#1-prs-need-discussion)
- [2. EIPs Discussion-to place](#2-eips-discussion-to-place)
- [3. GitPoap badges](#3-gitpoap-badges)
- [4. EIPs GitHub permissions & support](#4-eips-github-permissions--support)
- [5. EIP bots related discussion, updates, agreement on merging PRs & closing Issues.](#5-eip-bots-related-discussion-updates-agreement-on-merging-prs--closing-issues)
- [6. EIPs Insight - Monthly EIPs status reporting.](#6-eips-insight---monthly-eips-status-reporting)
- [7. EIP editor apprenticeship meeting](#7-eip-editor-apprenticeship-meeting)
- [8. Core EIPs in an Executable Spec World Proposal](#8-core-eips-in-an-executable-spec-world-proposal)
  - [Actions](#actions)
- [8. Review action items from the previous meeting](#8-review-action-items-from-the-previous-meeting)
- [Annex](#annex)
  - [Attendees](#attendees)
  - [Next Call](#next-call)

---

# 1. PRs need discussion

Video | [0:00](https://youtu.be/--jGL4_PCac)
-|-

PR was discussed that needs merging where an author was added to EIP-1.

Remove greeting bot ethereum/EIPs#5124 (will need manual merge due to @eth-bot bug). Waiting to get feedback from comments before responding.

Revise EIP-2535 ethereum/EIPs#5120 (might need manual merge if author does not respond). EIP editor in the PR suggested to move it from Last Call to Draft, however, it should be moved back to Review. It needs to be moved out of draft, and needs some edits. Doesn't need a manual merge.



# 2. EIPs Discussion-to place

Video | [5:07](https://youtu.be/--jGL4_PCac?t=307)
-|-

Proposals to close EIP Discussion Issues Ref: https://github.com/ethereum-cat-herders/EIPIP/issues/146. 

Looks like the most liked option was the third: Admin closes "discussion-to" Issues for proposals in Final, Stagnant, Withdrawn status. 

Looks like this was executed, and the issue can now be closed.

# 3. GitPoap badges

Video | [7:10](https://youtu.be/--jGL4_PCac?t=430)
-|-

ECH GitPOAP is live. https://www.gitpoap.io/gp/133

Past contributors to ECH repos can claim.



# 4. EIPs GitHub permissions & support

Video | [8:32](https://youtu.be/--jGL4_PCac?t=512)
-|-

Contributor's permission to EIP GitHub repo for Sam Wilson.
Spamming issue was communicated. Sam from ethereum.org mentioned he may be available to help.

# 5. EIP bots related discussion, updates, agreement on merging PRs & closing Issues.

Video | [9:32](https://youtu.be/--jGL4_PCac?t=573)
-|-

As Jose was not on the call, this topic was skipped.

# 6. EIPs Insight - Monthly EIPs status reporting.

Video | [9:50](https://youtu.be/--jGL4_PCac?t=590)
-|-

EIP-2464 and EIP-2364, long pending proposals moved to final. 

6 EIPs moved to draft.

2 more proposals are being reviewed before merging as draft.

Gavin John has been added as a new EIP editor.

Graphs and charts related to activity: https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight. 


# 7. EIP editor apprenticeship meeting

Video | [10:44](https://youtu.be/--jGL4_PCac?t=644)
-|-

Meeting 19 Recording https://www.youtube.com/watch?v=7hhXX2CfKzQ&feature=youtu.be.

Meeting happened yesterday. 


# 8. Core EIPs in an Executable Spec World Proposal
and Discussion

Video | [10:53](https://youtu.be/--jGL4_PCac?t=653)
-|-

This was to make the spec for an Ethereum client written in Python.

Greg was not able to make the last meeting. He asked if there was an EIP for it.

There is no formal proposal to change EIP-1 yet. 

Sam is weakly in favor for making it required with core EIPs. The core devs have to agree too, since they have to read them.

The core devs seemed unsure about it. No clear direction yet.

Greg doesn't read Python. He says it's not useful for understanding.

Micah suggests that regardless of the language chosen, there will be peop[e who don't understand it, even English. 

Greg suggests that specs are declarative, while Python is procedural. You'd have to reverse engineer the rules from the algorithm, which wouldn't be easy.

Micah predicts people will still write human readable values, in markdown. 

The proposal is to change where things are made. In addition to asking to write a reference implementation, and reference tests, where the tests pass. For that to work, there needs to be a shared reference implementation.

If we accept those conditions, the next step is asking what language is most accessible to developers? Python may meet that.

This is a way to make sure each EIP has tests and reference implementations. 

If you were to submit a draft, is it expected you already have the reference implementation in code? Or only the markdown version?

Greg points out the Epsilon team creates PRs against a C++ implementation. He doesn't want to run a Python environment, and understand the Python implementation to be a contributor. We did it this way for the CL layer, but they started out with a Python implementation.

We would have to get into a position of getting a working Python implementation, and then all the Core Contributors have to understand it. And it would create another bar of entry.

Some points still pointing to Python. To unify the beacon spec and the execution spec. Sure the systems are different today, but we're going to merge in a couple months. Having one Python spec, and one complicated math paper where we rely on 3 volunteers to update, it's pretty bad.

The other point, Tim thinks we're more bottlenecked by client developers than EIP proposals, which has been true for a couple years. The client teams he has spoken to, they generally prefer the executable spec approach.

Having something that maps from execution to consensus layer, you'd need a unified standard.

Will the Python client be able to sync to mainnet? Or will it be too slow to sync up? It can do a block every 12-13 seconds on a regular laptop. If you have a beefier machine it should be fine. 

If you're testing individual blocks it should be fine. And there's no reason to sync mainnet on a development machine. It is consensus compatible, but not designed for performance.

It's suggested to describe the EIP in english in some markdown file. And as things progress, there will be a requirement to get the code in. Then others can help to get the reference implementation written in Python.

Once a change has been proposed to go into a hardfork, on the consensus layer, there are people on the Ethereum Foundation who make a PR to the spec before it goes live. But to do that in live implementations, Geth, Besu aren't going to create a reference implementation in their client for any random EIP.

Another example, say Geth makes a reference implementation, the other teams need to use Geth for a reference to the spec. Some teams can't due to licensing. It makes the process harder.

There are cases where there are concerns about the EIPs once tests are being written for the EIPs.

The level of skill required to read the Yellow paper, if you can read it, then Tim is confident you'll be able to write a spec in Python. The Yellow paper is 10x less approachable, even more than the system we have now with the Yellow paper plus several EIPs.

The reference client isn't "client code." It's a translation of the Yellow Paper into Python, more than it is client code.

Even if you can read the Yellow Paper and Python equally well, the Yellow paper doesn't show differences as easily, than you would by looking at code on Github.

However, we could add the tooling to the Yellow paper for differences with the right process.

Greg brings up, that if we stop maintaining the Yellow Paper, many others who use it, like academics, it would affect them. 

However, after the merge, the Yellow paper will be out of date, since that spec is written in Python. 

There's also no barrier for volunteers to keep maintaining the yellow paper. It may not have the consensus layer, but the people who do use it, can continue using it.

Greg can go through specification written in English and math and eventually understand a concept, but he can't do the same with Python.

Given that the consensus layer will be using EIPs, it'll be good to have a process similar to what they are already using. 

It hasn't been brought up with client teams yet. Currently, the devs are working on the merge, so the time they can spend on this is quite small. Additionally, the py spec isn't up to date with mainnet yet. 

Currently, the py spec is at the Berlin hardfork. One fork behind. That's just code completion. After that, literate programing is next to start.

We have a spec for the merge, and we're not going to do this for the merge.

Then Shanghai. So this project may not be ready until after a year.

Before Sam and his team put in another year into this, it would be good to get buy ins from client teams. As well as concerns and potential solutions.

One thing Greg mentioned is, there is no formal EIP to propose this change in process.

The reason this hasn't been brought up to core devs yet, is that Sam wants to first have a consensus from EIP editors. Then we can go to Core Devs. 

But since we can't reach consensus here, Sam can go with something less fully baked.

Micah suggests, even if we ignore Greg's concerns, we're not totally there.

Greg would like there to be a reference specification. But wouldn't want to push that responsibility to EIP authors. 

Greg suggests testing it first before requiring it for everyone.

Tim suggests making a process for Shanghai may be a way to do this. It would be a way to iron out the bumps. And the EIPs doing this will be limited to EIPs going into the hardfork.

Next step is to get the opinion from the remaining EIP editors for this.

Sam has notes that are closest to what a proposal can be. Sam and Tim can collaborate for making the EIP for this.

## Actions

- 58.2 - Sam Wilson and Tim Beiko will create a Meta EIP for the Executable Spec process before showing the proposal to the core devs
- 58.3 - Remaining EIP editors to give their view on using the executable spec in the EIP process

# 8. Review action items from the previous meeting

Collect feedback on NFT sale of unused EIP numbers still needs to be acted on.

---

# Annex

## Attendees 

- Pooja Ranjan
- Sam Wilson
- Tim Beiko
- Greg Colvin
- Lightclient
- Micah Zoltu
- Ryan


## Next Call 

June 29, 2022, 15:00 UTC.

