# EIP Improvement Process Call #10 Notes
### Meeting Date/Time: Wednesday, June 17, 2020 at 15:00 UTC
### Meeting Duration: 1 hr
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=8P5WnOsjPzs)
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/19)
### Moderator: Hudson Jameson
### Notes: Edson Ayllon

----

# Summary


## Decisions Made

Decision Item | Description
---|---
**10.1** | EIP number registry may not be a major issue. Discussion can be dropped.
**10.2** | Continue the discussion on adding a mandatory terminology section for EIPs.
**10.3** | Future meetings, discuss onboarding EIP editors.
**10.4** | Have use of labels for PRs to EIPs.
**10.5** | Waiting on James to complete the precompile discussion item.


---

# Agenda

- [1. An EIP number registry process](#1-an-eip-number-registry-process)   
- [2. Separation of EIP process and hard-fork coordination](#2-separation-of-eip-process-and-hard-fork-coordination)   
- [3. ZIPs reference](#3-zips-reference)    
- [4. Micah's comments](#4-micahs-comments)    
- [5. Discuss the EIP-1 Brainstorming Document.](#5-discuss-the-eip-1-brainstorming-document)   
- [6. Clarifications for how a precompile address is decided.](#6-clarifications-for-how-a-precompile-address-is-decided)   
- [7. Review action items from previous meeting](#7-review-action-items-from-previous-meeting)   

---

# 1. An EIP number registry process

Video | [0:00](https://youtu.be/8P5WnOsjPzs)
-|-

**Hudson**: There was an idea for EIP editors to have a list of EIP numbers and assign numbers. Who else remembers this topic?

**Edson**: The concern was there was bloat with the EIP number, as it was tied to the Github issues. Greg brought up that currently, EIPs are numbered uniquely and in order, and editors don't need to be involved. If there are bad actors, they can be banned if necessary. If we were to have an EIP registry that EIP editors maintain, it might overwhelm EIP editors, as we don't have too many. And including this system may add a barrier of entry, which we currently don't have.

**Hudson**: Makes a lot of sense. It's something to look at. But maybe not a major problem right now. If we were to move away from Github, maybe we would need to look at solutions. As far as bloat, we have unlimited numbers on Github.

**Pooja**: Since it's the PR number, we can discuss it even before being merged. If we were to take that away, the discussion may bring confusion.

**Artem**: Another idea was to commission the development of a frontend to create EIPs. It would add complexity but would solve the numbering problem.

**Edson**: If there's a way to automate it, it can be solved, such as with the EIP bot. But right now, it may cause more complexity and inconvenience.

**Artem**: It's like we solve one minor problem and introduce some major ones.

**Hudson**: That's the consensus I'm hearing today. We can move on today.

## Decisions

- **10.1**—EIP number registry may not be a major issue. Discussion can be dropped.


# 2. Separation of EIP process and hard-fork coordination


Video | [6:48](https://youtu.be/8P5WnOsjPzs?t=408)
-|-

This item was postponed to another meeting since James Hancock and Axic were not on this call.

**Edson**: We should specify how to move from one status to another to keep the bar of acceptance high. We should also start specifying what the statuses are for hard-fork coordination.

# 3. ZIPs reference

Video | [9:27](https://youtu.be/8P5WnOsjPzs?t=567)
-|-

ZIPs are a version of PIPs or BIPs or EIPs. They include terminology as keywords.

**Edson**: ASTMs have a section for terminology which they include in their standards. A few other standards organizations also have this section. I'm not sure if we should apply ZIPs terminology, but we should consider a terminology section.

**Hudson**: You mean in EIP-1 or a sub-EIP?

**Edson**: A section in the EIP template. All EIPs.

**Alita**: I would also say that it should be required.

**Hudson**: As far as it being required, I'm not sure where I stand on that. But I agree with it being in the template.

**Alita**: Required would make it easier for editors for what's meant.

**Hudson**: We have security considerations that are required. Having another required one wouldn't be the end of the world.


## Decisions

- **10.2**—Continue the discussion on adding a mandatory terminology section for EIPs.


# 4. Micah's comments


Video | [13:36](https://youtu.be/8P5WnOsjPzs?t=816)
-|-


## 4.1 How to deal with non-normative edits?

When an edit doesn't change the meaning, only wording and grammar, and the author cannot be reached.

**Pooja**: Adding PRs for non-normative edits will increase the PR number.

**Edson**: I think the most straightforward solution is to have EIP editors deal with those.

**Hudson**: Yes. If there's consensus among editors, just make it. And Github tracks a history of changes.

**Pooja**: Another solution mentioned previously was the EIP centric process subgroup.

**Hudson**: We'd need that if there were enough EIPs to warrant that. This may be a rare issue.  

**Allita**: If the EIP is final, would you need the Author's input to reword things?

**Hudson**: It's a good idea. Outside observers can accuse editors of allowing malicious edits.

**Allita**: To me, if it's finalized, and enough time passes, the authors forfeit their leverage on that.

**Hudson**: That makes complete sense.


## 4.2 How can we improve the responsiveness of editors on actually merging PRs?

**Hudson**: This question is an entire subtopic that we haven't tackled yet. Which is, "How can we recruit and incentivize editors?"

**Edson**: We can table that towards a future meeting.

**Hudson**: It might be a good discussion topic on its own.

**Brent**: Could we have Ethereum clients assign and pay for some of their employees to be editors?

**Hudson**: That would work for core EIPs. Maybe not ERCs, which is the majority of EIPs.

**Jaye**: Maybe having a visual achievement, such as a nonfungible token, maybe KUDOS tokens, would incentivize people.

**Hudson**: Like reputation points.

**Pooja**: The issue is we don't have enough editors. We should be focusing on how to onboard more editors.

**Alita**: Are we talking about Core Editors or EIP editors?

**Pooja**: I was referencing EIP editors, but in some cases, they edit core EIPs.

**Hudson**: I don't think Core Editor is a term. Unless you mean an EIP editor which is also a Core Developer, which most EIP editors are. I don't know if they're talking about Core EIPs for responsiveness, or other EIPs too.

**Edson**: Micah would be talking about core EIPs. But I think we need more editors in general.

**Hudson**: Once we get to the point of editor recruitment, we can better coordinate on reputation and KUDOS systems.

**Alita**: It may be beneficial to have a description of what it means to be an editor. It would narrow down where we look to advertise.

**Jaye**: Whatever encourages becoming an editor should also encourage staying and participating as an editor.

**Hudson**: Good point.

## 4.3 Split EIPs into multiple repositories.

**Hudson**: Separating EIPs into multiple repositories is a lot of work. Which isn't hard to do. But to be notified, we can create RSS feeds and email notifications.

**Edson**: I agree with you, and it may mess up the EIP numbering system. There may be EIPs with overlapping numbers, as it's based on the PR.

**Artem**: We can take advantage of Github labels.

**Hudson**: Axic started using them last year, but that fell off. We can add that to the agenda for a future meeting.

**Pooja**: If we were to add labels, it may be useful to document that in EIP-1 for editors and authors.

## Decisions

- **10.3**—Future meetings, discuss onboarding EIP editors.
- **10.4**—Have the use of labels for PRs to EIPs.


# 5. Discuss the EIP-1 Brainstorming Document.


Video | [29:05](https://youtu.be/8P5WnOsjPzs?t=1745)
-|-

Tabled to another meeting as James is on vacation.

# 6. Clarifications for how a precompile address is decided.


Video | [29:26](https://youtu.be/8P5WnOsjPzs?t=1766)
-|-

**Hudson**: This isn't hard to solve, as long as the Core Developers come up with a system. It's usually discussed in the Core Devs meeting, and it's usually a yes or no. Martin commented that final precompiles may be good to include in a hard-fork meta. This may be outside of the scope of these meetings.

**Artem**: It may not be an issue, as we don't introduce precompiles daily. We may not need a system to solve a very minor problem.


## Decisions

- **10.5**—Waiting on James to complete the precompile discussion item.


# 7. Review action items from the previous meeting


Video | [31:58](https://youtu.be/8P5WnOsjPzs?t=1918)
-|-

**Hudson**: Edson did you finish that article?

**Edson**: It was published.
- https://medium.com/ethereum-cat-herders/the-eipip-roadmap-cabe41fdb908
Three different phases: Decision making, clarity, and onboarding. It may be helpful to reference before every meeting.

**Hudson**: I like how it's outlined.

**Jaye**: I like how there's an effort to continue lowering the barrier of entry.

**Hudson**: Great comment. What were the decisions for today?
1. Future meetings, discuss onboarding EIP editors.
2. Continue the discussion on adding a mandatory terminology section for EIPs
3. Have use of labels for PRs to EIPs
4. We can drop a discussion for the EIP number registry.
5. Precompile addresses. waiting for James to comment

---

# Annex

## Attendees

- Artem Vorotnikov
- Brent Allsop
- Chloe Lewis
- Edson Ayllon
- Hudson Jameson
- Jaye Harill
- Pooja Ranjan
- Wei Tang

## Next Call

Wednesday, July 1, 2020, 15:00 UTC.
