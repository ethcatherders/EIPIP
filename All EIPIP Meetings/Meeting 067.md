# EIP Improvement Process Call #67 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, Oct 19, 2022 at 14:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://youtu.be/nox00vRkET8) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/185) <!-- omit in toc -->
### Moderator: Pooja Ranjan <!-- omit in toc -->
### Notes: Edson Ayllon <!-- omit in toc -->

----

# Summary <!-- omit in toc -->

## DECISION ITEMS <!-- omit in toc -->
Decision Item | Description
-|-
67.1 | New meeting time is 15:00 UTC

## ACTION ITEMS <!-- omit in toc -->
Action Item | Description
-|-
67.1 | Continue discussion of external links
67.2 | Get final EIP author feedback into changing to ERC-# format before implementing it

---

# Contents <!-- omit in toc -->

- [1. Discuss](#1-discuss)
  - [1.a. New process issues:](#1a-new-process-issues)
  - [1.b. Process issues that haven't reached consensus:](#1b-process-issues-that-havent-reached-consensus)
- [Closing Discussion](#closing-discussion)
- [Annex](#annex)
  - [Attendees](#attendees)
  - [Next Call](#next-call)

---


# 1. Discuss

## 1.a. New process issues:

Video | [0:00](https://youtu.be/nox00vRkET8)
-|-

- [Create an EIP External Link Archive ethereum/EIPs#5408](https://github.com/ethereum/EIPs/issues/5408) - [Allow external links when archived link provided  ethereum/EIPs#5733](https://github.com/ethereum/EIPs/issues/5733)
- [Add EIP-5757: Propose process for allowing external links ethereum/EIPs#5757](https://github.com/ethereum/EIPs/pull/5757)

External link policy. Has been under discussion for some time. 
- https://github.com/ethereum/EIPs/issues/5408
- https://github.com/ethereum/EIPs/issues/5733

It's a process for providing an external link. Was proposed by Sam. It's a process for getting external source approved. Once approved, it moves to a living document.

Adding a new source goes into its own EIP. The purpose is to have individual EIPs as discussions. The individual EIPs for the sources are not living.

Lightclient wants to minimize the living status. The list of accepted 5757 sources goes into EIP-1. And 5757 goes to final.

Victor Zhou mentioned it takes months for EIPs to go into final. There are some EIP authors forced to drop the links that provide context.

There are 2 types of people that post links: Scammers, and well intenioned authors. Victor thinks we've been to conservative with links, forcing most to drop them.

Then there's the argument that external sources to be free access. Citing things that aren't free access are things contained in books. He also thinks we should consult lawyers whether we can move copyrighted content into EIPs, as non-free access material is copyrighted. Asking for everything moved to us or everything to be free access may be too far away. The intention is good. But we're living in a non-perfect world.

Victor's feedback was to get Greg and Panda's feedback, that having an EIP would be too much, and that third we should be considered free access.

Victor thinks our credibility is how much people want to propose EIPs, since they can propose somewhere else. We've seen valuable EIPs go to stagnant.

Sam thinks Victor brings up a lot of great points. But he doesn't agree with including non-free links. He doesn't think requiring people to copy things into our repos is illegal, as that's how many open source repos work. Sam agrees getting the feedback from Greg and Panda.

Victor compared it to GPL. 

Sam thinks GPL isn't what we want to do. We don't want to encomber with more requirements of implementors of the spec. We don't use GPL for the EIPs repo, or anywhere near GPL.

Victor then thinks we approach the EIP repo too much like GPL, restricting the EIPs.

Sam states we don't want to restrict users of finalized EIPs, but we want to restrict the authors work getting included in the EIP repo. This includes excluding paid content.

From Pooja's perspective, she's inclined to Sam's point of view. The standards are made for people to build projects from. If authors have issues with the copyrighted materials to be included. They are free to create their standard externally with copyright material. But once it's in the repo, it should be copyright free.

Victor isn't convinced. But he also thinks the conversation isn't at the state for any side to be convinced.

Victor instead wanted to talk about requiring an EIP for each external source. Wants to see if an editor's discussion would be sufficient. If there's any way to expedite the process.

Sam doesn't see why it wouldn't be ok to have the core devs approve the source in a call. He specifies a source isn't an individual link.

Victor stated we're currently censoring links. And this process only helps not good authors. Good authors want to make convincing evidence. 

Sam suggests that we should be against closed source, in fear that it overtakes our governance process.

Victor suggests we should bootstart the EIP with an allowlist to start with. Things that we're already referencing.

Also, Victor wants to get Alex's opinion as well.

Pooja suggests that any external link you want to share, you can share it in the discussion-to, in Ethereum Magicians.

Victor disagrees with this alternative. He disagrees copying code and putting it in the assets folder, given they have licenses. 

Sam says we don't change the licenses when we put it in the assets folder. We can't change people's licenses of external sources.

Victor says, copying material is touching copyright. Which we should avoid.

This topic discussion was moved to a future meeting, and suggested we do an async discussion.

This EIP has a discussion-to link, so this discussion is documented.

Victor brought up that we should have alternatives to Ethereum Magicians. Like Ethereum research.

Pooja brings up that earlier there were multiple places. And we had a long discussion to keep it in a centralized place.

Victor said this discussion he doesn't see where it was mentioned only keep it in Ethereum Magicians. He suggests for this case, maybe we should have an ERC for it.

Victor brought up that Consensus was thinking of publishing their standards somewhere else, or keep it in their repo.


**Propose a contributor field in pre-emble to allow author recognize contributors of an EIP ethereum/EIPs#5762**

Video | [33:41](https://youtu.be/nox00vRkET8?t=2021)
-|-

The EIP Editors on the call were against this proposal. 

Sam doesn't have a problem of displaying contributors, but it shouldn't be in the preamble. We can setup Jeckle to show contributors.

Victor's intention was to have authors showcase who helped them, without having them be an author.


## 1.b. Process issues that haven't reached consensus:

Video | [35:53](https://youtu.be/nox00vRkET8?t=2153)
-|-

[Update EIP-1: Reference ERCs by ERC-X ethereum/EIPs#5273](https://github.com/ethereum/EIPs/pull/5273)

Lightclient said everyone in the community is already referring to EIPs that are ERCs as ERC-#. Even Vitalik is frustrated that we're calling them EIPs in the standards repo, and not ERCs.

Pooja wants consistency even in documentation. Not only in EIP-1, but everywhere.

Sam and Panda are against it. Sam doesn't like it from a consistency point of view. ERC-20s have an interface that's called ERC-20, but the EIP is EIP-20.

Lightclient agrees that it's not consistent. But the community has already decided against it, and it's hostile to go against that.

Lightclient thinks it would be preferable to change the md filenames, the problem is that would break links to them.

Pooja thinks we should start with EIP-1 if we're making this change.

Sam thinks it's an hour and a half of work to make the ERC change.

Victor agrees with changing it to ERC, but we need to address the broken links problem. Once backwards compatiblity is solved, we can move forward.

Victor says we should get PandaPip's opinion before coming to a conclusion. 

The pull request was opened by PandaPip.

Pooja is now asking if it would be confusing to replace the EIPs with ERCs.

We can keep it for one more meeting to ask PandaPip and Greg.

Video | [35:53](https://youtu.be/nox00vRkET8?t=2918)
-|-

[New contract interface and EIPs should be required to include a privacy considerations section ethereum/EIPs#5682](https://github.com/ethereum/EIPs/issues/5682)

Sam think it's not applicable to the majority of EIPs. And the ones it is applicable to, we can include it in the Security Considerations section.

Victor isn't a big fan of putting privacy considerations under privacy considerations. He'd prefer a new section, or updating the section title to "Security and Privacy consideration."

Pooja says we should place our comments in  the issue.

# Closing Discussion

Video | [50:26](https://youtu.be/nox00vRkET8?t=3026)
-|-

The group was deciding on a new meeting time. 1430 or 1500 UTC was brought up. 

There was discussion around having it during the weekend, but there was pushback since this is considered work for many participants, and didn't want to intrude on personal time.

Either time worked for those present. 1500 UTC was decided from those there.

Axic was brought up for this decision, he actually wanted to reduce his weekly calls.

Couldn't get to all issues. The rest will be addressed async, and the following meeting.

---

# Annex

## Attendees 

- Pooja Ranjan
- Sam Wilson
- Lightclient
- Victor Zhou
- Cyrus


## Next Call 

Nov 2, 2022, 15:00 UTC.

