# EIP Improvement Process Call #10 Notes
### Meeting Date/Time: Wednesday, August 12, 2020 at 15:00 UTC
### Meeting Duration: 1 hr
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=mkz9eJ3GDTI)
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/26)
### Moderator: Hudson Jameson
### Notes: Edson Ayllon

----

# Summary


## Decisions Made

Decision Item | Description
---|---
**14.1** | Hardfork coordination upgrade talk awaiting until James joins. 
**14.2** | EIP repo scope constraint awaiting until James joins.
**14.3** | Small working groups to be tested.
**14.4** | Get final approval from ACD on new EIP statuses. 
**14.5** | Create triaging permissions for Github.
---

# Agenda

- [1. Network upgrade process](#1-network-upgrade-process)   
- [2. Constraining the EIP repository scope](#2-constraining-the-eip-repository-scope)   
- [3. Explore the idea of working groups](#3-explore-the-idea-of-working-groups)   
- [4. New EIP validator](#4-new-eip-validator)   
- [5. Onboarding EIP editors](#5-onboarding-eip-editors)   
- [6. Discussion on Muir Glacier postmortem report PR-2809 and Network upgrade postmortem template PR-2810](#6-discussion-on-muir-glacier-postmortem-report-pr-2809-and-network-upgrade-postmortem-template-pr-2810)   

---

# 1. Network upgrade process

Video | [0:00](https://www.youtube.com/watch?v=mkz9eJ3GDTI)
-|-

Edson presented ideas for the network upgrade process. The focus was on statuses for hardfork coordination.

[See full document here](https://gist.github.com/edsonayllon/e9b91a2c3a8e2d4e242cfc236162e106).

The group liked a combination of statuses from the options mentioned, which included the following:
1. Stage 1: Eligible for Inclusion - Open for discussion for entering a hardfork
2. Stage 2: Implementation - Decision to have clients include the EIP, before testing
3. Stage 3: Testing - Decision to have EIP tested, testnet/state tests/fuzzing, etc.
4. Stage 4: Staged - Decision to go to mainnet and decision on which date to release (block number)
5. Stage 5: Deployed - EIP is live
6. Stage 6: Maintenance - Review/monitering period after EIP is launched on mainnet
7. Rejected - An EIP fails moving from one step to another, can happen at any time.

The remaining pieces will be discussed when James Hancock is on the call.

Pooja [shared her proposal as well](https://docs.google.com/document/d/18TkCXfsW5Qm4Na1U2Fk-iPcSLpjD6IFbZTlBJfQ1kRI/edit?usp=sharing).

Her proposal includes:
1. Proposed
2. Accepted
3. Testnet
4. Staged
5. Deployed in Hardfork

With additional information on socializing the EIP.

Lightclient brought up on how to move from one stage to another. His emphasis was on avoiding chainsplits. He brought up defining core Ethereum principles that can justify a hard-fork even in the presence of a potential chain split.

## Decisions

- **14.1**—Hardfork coordination upgrade talk awaiting until James joins. 

# 2. Constraining the EIP repository scope

Video | [30:00](https://youtu.be/mkz9eJ3GDTI?t=1800)
-|-

Postponed until James can be on the call.

## Decisions

- **14.2**—EIP repo scope constraint awaiting until James joins.


# 3. Explore the idea of working groups

Video | [30:24](https://youtu.be/mkz9eJ3GDTI?t=1824)
-|-

Working groups addresses the following problems:
1. Low quality proposals
2. There are not a lot of people willing to make unpopular decisions in the EIP repository to have higher quality EIPs.

Working groups introduces heirarchy. It's something every standards organization has.

Example working groups:
- Meta
- EVM
- Clients
- Networking
- ERC
- RPC
- Eth1.x
- Eth2.0

**Hudson**: Starting small may be helpful. As well as utilizing Github's triage level permissions.

**Lightclient**: Working groups don't need to have write access. They are there to aid editors.

**Alita**: Is your suggestion to have a panel of experts to audit changes to certain categories of EIPs?

**Lightclient**: I was looking more for a proactive group. They would be drafting EIPs, in addition to giving feedback to incoming EIPs.

## Decisions

- **14.3**—Small working groups to be tested.


# 4. New EIP validator

Video | [40:42](https://youtu.be/mkz9eJ3GDTI?t=2442)
-|-

[New EIP validator was integrated](https://github.com/ethereum/EIPs/pull/2860). The EIP validator makes sure the EIP is syntactically valid.

The new EIP statuses won't be added to the EIP validator until after recieving final approval from the All Core Devs.

## Decisions

- **14.4**—Get final approval from ACD on new EIP statuses. 


# 5. Onboarding EIP editors

Video | [43:19](https://youtu.be/mkz9eJ3GDTI?t=2599)
-|-

Survey has been sent out.

Triaging permissions still need to be made.

## Decisions

- **14.5**—Create triaging permissions for Github.


# 6. Discussion on Muir Glacier postmortem report PR-2809 and Network upgrade postmortem template PR-2810

Video | [44:48](https://youtu.be/mkz9eJ3GDTI?t=2688)
-|-

No comment. If we move to a hardfork repo, this would be moved to there.

If we figure out the numbering issue, it can be dealt with in the new repo.

There is a repo for Eth1.0 specs.

**Lightclient**: I think the Yellowpaper should be in Eth1.0 specs.

**James**: I like having everything needed for writing a client in Eth1.0 specs.

What's included in the Eth1.0 specs repo:
- Hardfork coordination
- EIPs in mainnet
- Yellow Paper
- Retrospectives of hardforks

**Hudson**: Moving the Yellowpaper might be weird. But coordination for updating it can be in that repo. Moving the Yellowpaper out of the old repo will lose all its history. We can link the Yellowpaper.

---

# Annex

## Attendees


- Brent Allsop
- Chloe Lewis
- Edson Ayllon
- Hudson Jameson
- James Hancock
- Jaye Harill
- Lightclient
- Micah Zoltu
- Pooja Ranjan

## Next Call

Wednesday, August 26, 2020, 15:00 UTC.
