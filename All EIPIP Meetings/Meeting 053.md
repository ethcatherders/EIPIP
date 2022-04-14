# EIP Improvement Process Call #53 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, Apr 6, 2022 at 15:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=5VbbS-3MQss) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/118) <!-- omit in toc -->
### Moderator: Pooja Ranjan <!-- omit in toc -->
### Notes: Edson Ayllon <!-- omit in toc -->

----

# Summary <!-- omit in toc -->

## ACTION ITEMS <!-- omit in toc -->
Action Item | Description
-|-
**53.1** | Have C.I. update the creation date of an EIP to the date it was first merged into the EIP repo.
**53.2** | Update the bot to not touch EIP-1
**53.3** | Update bot to have minimum 2 EIP author approvals before merge

## DECISION ITEMS <!-- omit in toc -->
Decision Item | Description
-|-
**53.1** | Only Withdrawn and Final EIPs can recieve a reference in a new EIP

---

# Contents <!-- omit in toc -->

- [1. Rename master branch to main branch Ref: Issue](#1-rename-master-branch-to-main-branch-ref-issue)
- [2. Discuss appropriate date for "Created" in EIP](#2-discuss-appropriate-date-for-created-in-eip)
  - [Actions](#actions)
- [3. Discuss EIPs status that may or may not be added to a new proposal.](#3-discuss-eips-status-that-may-or-may-not-be-added-to-a-new-proposal)
  - [Decisions](#decisions)
- [4. Core EIPs in an Executable Spec World Proposal and Discussion](#4-core-eips-in-an-executable-spec-world-proposal-and-discussion)
- [5. EIP bot Issues and eipv Issues updates](#5-eip-bot-issues-and-eipv-issues-updates)
  - [Actions](#actions-1)
- [6. EIPs Insight - Monthly EIPs status reporting.](#6-eips-insight---monthly-eips-status-reporting)
- [7. EIP editor apprenticeship meeting](#7-eip-editor-apprenticeship-meeting)
- [8. Review action items from the previous meeting](#8-review-action-items-from-the-previous-meeting)
- [Annex](#annex)
  - [Attendees](#attendees)
  - [Next Call](#next-call)

---

# 1. Rename master branch to main branch Ref: Issue

Video | [0:00](https://youtu.be/5VbbS-3MQss)
-|-

Before the call, some new participants introduced themselves. 

Victor
- Author of ERC-1202, and EIP-2135
- Joined to see how to get more adoption and consensus on his EIPs

Greg
- Core developer and EIP editor
- Put together the original EIP process

Sam Wilson
- Responsible for breaking a lot of changes Greg mentioned

Jose
- Has been trying to contribute to the EIP bot (issue 53, 55, and 58)

This was requested in the EIPIP and EIP issue section. 

Looks like there was a vote to rename it as well. Thumbs up/down on the issue.

Pooja asks if we really need to make this change.

The argument for changing this, is the term master may be offensive to some people. The argument against it is, master is a commonly used word, and doesn't have that connotation for everybody.

Micah, if we rename it, we'll offend the people against the renaming, so best to not offend anyone, we should do nothing.

Greg thought that its been master for so long, that changing it may bring confusion. 

No editors are for the proposal. 

If we do make this change, it should probably be changed on every repo under Ethereum. Also, the issue champion isn't on this call, so it shouldn't be discussed here.

# 2. Discuss appropriate date for "Created" in EIP

Video | [10:31](https://youtu.be/5VbbS-3MQss?t=631)
-|-

This was added from recommendation of last meeting. It was brought up how confusing dates can be.

For example, an EIP can be created far before it was available for anyone to see.

Micah prefers created is when the file was originally added to the repository. And this was done by CI, not done the author himself. But, there's a technical effort to do so. Otherwise, I don't see the point in even having this data.

Sam likes seeing the age of an EIP, so until there's a technical way to do this, we should keep it.

So, the action item is to get this updated by CI, and find a resource to do so.

## Actions

- **53.1** - Have C.I. update the creation date of an EIP to the date it was first merged into the EIP repo.


# 3. Discuss EIPs status that may or may not be added to a new proposal.

Video | [14:28](https://youtu.be/5VbbS-3MQss?t=868)
-|-

This item was added based on Ethereum Magicians comments. 

Micah is highly against people referencing EIPs in draft, as it is mutable, and likely to be something different in the future.

Micah's suggestion is to extract what was relevant to that draft EIP, and include it in their EIP. 

Greg suggests, just extracting a sentence isn't going to work.

Micah says it's ok for EIPs in final. But for EIPs in draft, this won't be good process.

With regards to an EIP being able to make it to final, even thought it's not adopted, this example was with core EIPs, which only make it to final if they are adopted.

Sam is for having core EIPs going to final, but adding an adopted header. 

Greg is against that. A final standard that's not on mainnet isn't final, otherwise it can get edited until it is. This happened with EIP-2315.

Micah suggests, this is to not confuse or frustrate core developers, who are familiar with a number, who then need to reference a fork EIP with a new number. 

We can create a status that is final, but not deployed, so there can be crosslinking. 

Withdrawn is immutable. So it's fine linking to withdrawn EIPs, just not Draft EIPs. 

Victor suggests adding another status after final, called adopted. 

Micah suggests there is value for seeing what is adopted, however, that should not be included in the EIP process.

Greg suggests using Living status for opcodes. If you do this immutibly, you end up with a long stack of EIPs. 


## Decisions

- **53.1** - Only Withdrawn and Final EIPs can recieve a reference in a new EIP


# 4. Core EIPs in an Executable Spec World Proposal and Discussion

Video | [36:56](https://youtu.be/5VbbS-3MQss?t=2216)
-|-

Last meeting we discussed the proposal already available by Tim Beiko in Ethereum magicians.

We were looking to see if there were any alternate proposals. Maybe we can wait until Sam is back on the call to continue this. 

Video | [51:39](https://youtu.be/5VbbS-3MQss?t=3099)
-|-

Sam came back, had nothing new to share. He's been updating the discussion thread.

Greg doesn't understand some points of this, but it doesn't sound like a good idea. His concern, is having a heap of Python to be the specification is worse, isn't human readable. 

The spec is a reference client. There may be a spec to update it. 

There are two human readable things in the spec. The annotations in the code, and markdown files in the repo.

Greg's concern is people having to learn Python to contribute the spec. Also, there's no formal specification for Python, has to look into the source code. Greg prefers the Yellow Paper.

Micah suggests learning Python will be easier for most people than learning Mathematical concepts. Everyone looking to implement this will be a software engineer.

Choices that are made due to the nature of the language is a legitimate concern. However, the readability improvements is a benefit.

Was short on time to continue this discussion. Will be pushed to a future meeting. Suggest to put this earlier in the agenda next time.

# 5. EIP bot Issues and eipv Issues updates

Video | [38:54](https://youtu.be/5VbbS-3MQss?t=2334)
-|-

Jose has been working on these bot issues. 

Jose wanted to know if the purpose of the bot to follow EIP-1 spec. He's wondering why we enforce the template. 

We're currently manually enforcing the EIP template. But we want a bot that enforces that. 

Jose suggests that there will always be an editor that approves that. So questioning the purpose of the bot doing this as well.

Micah suggests, that is the case, but it will be less work for editors.

Another topic, there were  changes to EIP-1 with a single editor approval. It was automatically merged, which shouldn't have been the case.

This seems to be a bug. The number of editor approvals required goes down over time. This is to not block, when editors are not available, ie. 1 active editor. 

Micah forgot that if you approve a PR to EIP-1, it will get auto-merged. Micah takes responsibility for it. 

Maybe, this should be a special case for EIP-1 or living EIP.

EIP-1 shouldn't change without special discussion or consensus. 

But this still seems like a bug on the bot. 

The easiest solution is to update the bot not to touch EIP-1.

Author's approval, Ref: PR

## Actions

- **53.2** - Update the bot to not touch EIP-1
- **53.3** - Update bot to have minimum 2 EIP author approvals before merge

# 6. EIPs Insight - Monthly EIPs status reporting.

Link is added to the agenda

# 7. EIP editor apprenticeship meeting

Meeting 15 Summary & Recording added to the agenda. 

# 8. Review action items from the previous meeting

All the items have been taken care of.

---

# Annex

## Attendees 

- Brent Allsop
- Greg
- Jose
- Sam Wilson
- Micah Zoltu
- Pooja Ranjan
- Zainan Victor Zhou


## Next Call 

Wednesday, April 20, 2021, 15:00 UTC.

