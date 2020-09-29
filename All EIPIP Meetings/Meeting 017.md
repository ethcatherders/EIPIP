# EIP Improvement Process Call #14 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, September 23, 2020 at 15:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=fl5MOhbipgY) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/33) <!-- omit in toc -->
### Moderator: Hudson Jameson <!-- omit in toc -->
### Notes: Edson Ayllon <!-- omit in toc -->

----

# Summary <!-- omit in toc -->


## Decisions Made <!-- omit in toc -->

Decision Item | Description
-|-
**17.1** | Superceded to be removed
**17.2** | Withdrawn and Stagnant to stay separate statuses to have finality
**17.3** | Lightclient to have write access for triaging

## Actions Needed <!-- omit in toc -->

Action Item | Description
-|-
**17.1** | Finalize Withdrawn status names
**17.2** | reate the status diagram with explicit arrows


---

# Contents <!-- omit in toc -->

- [1. EIP status abandoned vs withdrawn](#1-eip-status-abandoned-vs-withdrawn)
  - [Actions](#actions)
  - [Decisions](#decisions)
- [2. Network upgrade repository and process](#2-network-upgrade-repository-and-process)
- [3. EIP triaging permissions](#3-eip-triaging-permissions)
  - [Decisions](#decisions-1)

---

# 1. EIP status abandoned vs withdrawn

Video | [0:00](https://www.youtube.com/watch?v=fl5MOhbipgY)
-|-

The EIP statuses have been discussed over a period of months, reaching where they are now. Alex brought in the addition of having a reason field for Withdrawn EIPs. 

He made a PR to have this field to be added to Withdrawn EIPs, which is good. This then turned into a discussion of Withdrawn vs Stagnant again. 

James doesn't think we should open up the discussion again. If James and Axic go back and forth, and make a decisions in discord, this would ignore the contributions of everyone who had been in the discussion before this, without opening it back up for everyone to be apart of it again. 

Last meeting, we decided to do a PR to EIP-1, and leave the statuses as is, because we thought we were ready. How we add Alex's PR to that, we add the reason field to that. 

Alex's propsed EIP status is not much different than the one we've decided on. So we can easily convert from one to another. 

With Alex's proposal, however, `Withdrawn` can go back to `Draft`. This makes Withdrawn EIPs able to resurrect, reducing finality. 

*Pooja shared some Google slides, see the recording for the slides.* 

There was discussion on why EIPs can't go back to Draft, asked by Micah. The reason was to add finality for the community. This way, for controversial EIPs that become withdrawn, the community can have security. Also, this prevents low EIP number squatting. 

How do things go to Withdrawn? Things can go to Withdrawn moved by the Author, and maybe the bot after 2 years inactivity. For the bot or editors to move EIPs to Withdrawn without doing it algorithmically, such as 2 years, it may be seen as political. 

A new diagram will be made that makes implied arrows explicit. Also, `Superceded` may be removed. 

Next, the status names need to be decided again. Renaming will be done next meeting, after more discussion.

For now, Withdrawn will be author only, then a proposal can be made to add an algorithm.

## Actions

- **17.1**—Finalize Withdrawn status names
- **17.2**—Create the status diagram with explicit arrows

## Decisions

- **17.1**—Superceded to be removed
- **17.2**—Withdrawn and Stagnant to stay separate statuses to have finality

# 2. Network upgrade repository and process

Video | [46:17](https://youtu.be/fl5MOhbipgY?t=2777)
-|-

Something brought up, will there be EIPs in the network upgrade repo? 

The Serenity Phase 0 EIP didn't specify anything, however, it linked to an existing repo. When Eth1 merges into Eth2, will that require an EIP? And will it be in the Eth specs repo?

The question is, will Eth1 and Eth2 specs repo merge.

We don't know how to handle that yet. So it's on the radar. Something to coordinate with the Eth2 team. 

Does the merge happen when it's implemented on chain? Or, does it happen before that?

When Eth2 becomes Ethereum, it's probably it'll be using the EIPs repo. 

However, trying to specify Eth2 into a few EIPs may be too large a task. It may be fine to point to a repo then. 

However, once Phase 0 is launched, tweaks to it may be individual EIPs. Kind of how the Yellow Paper evolved. 


# 3. EIP triaging permissions

Video | [53:48](https://youtu.be/fl5MOhbipgY?t=3228)
-|-

This can't be done. To do so would need an upgrade of Github Enterprise account. The change would be more expensive. But Hudson can double check. 

Instead, people can have write permissions, but their role can be a more limited scope. Lightclient will be the first to be a part of this. 

Micah will also be unavailable for a few weeks, so other editors will need to cover the workload. 

## Decisions

- **17.3**—Lightclient to have write access for triaging

---

# Annex <!-- omit in toc -->

## Attendees <!-- omit in toc -->


- Brent Allsop
- Chloe Lewis
- Edson Ayllon
- Hudson Jameson
- James Hancock
- Lightclient
- Micah Zoltu
- Pooja Ranjan

## Next Call <!-- omit in toc -->

Wednesday, October 7, 2020, 15:00 UTC.
