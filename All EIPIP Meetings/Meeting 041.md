# EIP Improvement Process Call #41 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, Apr 21, 2021 at 15:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://youtu.be/54j6VK6ska0) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/85) <!-- omit in toc -->
### Moderator: Pooja Ranjan <!-- omit in toc -->
### Notes: Edson Ayllon <!-- omit in toc -->

----

# Summary <!-- omit in toc -->

## Decisions Made <!-- omit in toc -->
Decision Item | Description
-|-
**41.1** | Networking will follow the same EIP process as other EIPs. And outstanding networking EIPs will be updated to progress through the process towards final. 
**41.2** | Stagnant bot will prioritize bug fixing and not opening a PR if an existing PR is open for the same EIP
**41.3** | Bot will show a notice to new issues to make a discussion thread on Ethereum Magicians instead. All discussion focused issues will be closed by the editors, encouraging to happen on Ethereum Magicians.


---

# Contents <!-- omit in toc -->

- [1. Process for Networking EIPs](#1-process-for-networking-eips)
  - [Decisions](#decisions)
- [2. Progress update on moving to "Stagnant" by bot. Ref: eip-bot](#2-progress-update-on-moving-to-stagnant-by-bot-ref-eip-bot)
  - [Decisions](#decisions-1)
- [3. Decision on closing Issues](#3-decision-on-closing-issues)
  - [Decisions](#decisions-2)
- [4. EIPs Insight - Monthly EIPs status reporting](#4-eips-insight---monthly-eips-status-reporting)
- [5. Review action items from the previous meetings](#5-review-action-items-from-the-previous-meetings)
- [6. Closing Discussion](#6-closing-discussion)
- [Annex](#annex)
  - [Attendees](#attendees)
  - [Next Call](#next-call)

---


# 1. Process for Networking EIPs

Video | [0:00](https://www.youtube.com/watch?v=54j6VK6ska0)
-|-

PRs have been created to change several EIP statuses. 

This topic is to reconsider the standardization of networking proposals. 

People who write networking EIPs expressed dissatisfaction with the EIP process. They should either follow the process, or create another process. 

There are only 2 people who do networking EIPs. The process may be fine, but they write the EIP, and leave it.

It looks like they are using the EIP process as a way to advertise. But that may not be the proper use of the EIP process.

They're annoyed that it's a final EIP, but they have to go through each stage.

Micah's concern just moving these to final is there will become an incentive to avoid the EIP process by just waiting long enough.

Felix communicated the EIP process is OK. And may work for networking EIPs of the future. However, the networking EIPs of the past were made in a different time, with a different EIP process.

The point of the EIP process is to aid client developers. For client consensus it makes sense, because they all have to implement the same thing. There, things can be verified with tests, because there exists a specification.

Felix believes it's not important for networking to be 100% aligned. It's possible for clients to implement things outside of EIPs. It's not regulated so tightly as Ethereum consensus is. Clients just need to connect. 

Half of the clients don't implement all of the specs. And clients may implement their own extension, which may not have a spec. There's no canonical way to do it. To have all clients network in the same way, it may never happen.

Unlike other consensus changes, the networking does have a website that is spec'd out.

This website was just to document what the protocol currently is. It's just documentation of what the clients are really doing. It's not a spec first approach.

The networking EIPs have an independent purpose from the spec which lays out the change in advanced. Once it's implemented, we can define the spec from what we've learned. 

Felix doesn't want to create it's own process.

For Eth2, they have a specs repo. They don't use the EIP process. They have PRs, and people review, and when it's merged, then it's final. It's much more lightweight.

One issue is we don't have a repo in Ethereum for that. The networking EIPs is a way we can move to that.

Felix prefers to maintain the spec himself, and have changes proposed by EIPs. Because EIPs require you to make the proposal in a formal format. Namely the rational. In just a PR, there wouldn't be a rational, it would get lost. You won't reject a PR because the description isn't 100%, but you would with an EIP. 

In the changelog of the spec, we can link the EIP, and see all the material leading to the decision. 

There's only no value for the older EIPs, because they are already implemented, and essentially done. 

It's good to get people reviewing these old EIPs so the EIP can get more clarification, even if the spec itself won't change. If an EIP is in Draft, most people haven't looked at it.

The process is simple, make a PR, set it to Review, then Last Call.

Conversation moved to click block choice rule. There is an EIP for the click. And not Geth specific, implemented by other teams as well. The Click protocol EIP is final. This is an extension of that, and is in review. The question is who should review it. And should be brought up in All Core Devs. It's something everyone would have to implement.

It's a click consensus change, but technically it is a Core EIP. It may be a networking EIP by mistake.

We have talked about networking EIPs in All Core Devs, however, a long time ago. Felix plans to present future networking EIPs in the All Core Devs call.

Pooja wants to move to change these PR's statuses, the open old networking EIPs. 

## Decisions

- **41.1** - Networking will follow the same EIP process as other EIPs. And outstanding networking EIPs will be updated to progress through the process towards final. 
 

# 2. Progress update on moving to "Stagnant" by bot. Ref: eip-bot

Video | [27:37](https://youtu.be/54j6VK6ska0?t=1657)
-|-

Alita left some comments on the Agenda.

Some issues have been closed regarding modifying the bot. 

Alita implemented features for the stagnant bot.
- Auto cleans backlog
- If it creates a new PR by mistake, that's a repeat, it will delete duplicates on the next check
- Deployed several bugfixes

Currently there are 200 PRs for the stagnant bot. 

Alita is mainly focused on bugfixes and feature requests. Please leave any feature requests or bugs in the eip bot repo.

Currently, the bot automatically merges them after 2 weeks. If we don't want them to merge, we need to close it with those 2 weeks. However, currently, it reopens after another week.

The bot doesn't look if there is an existing PR against that EIP. Of all the features, that would be the highest priority one. Waiting for an editor to review may take a week or more.

The current plan is to fix bugs first, then implement features.

## Decisions

- **41.2** - Stagnant bot will prioritize bug fixing and not opening a PR if an existing PR is open for the same EIP


# 3. Decision on closing Issues

Video | [33:13](https://youtu.be/54j6VK6ska0?t=1993)
-|-

Historically, the issue section was used for discussion. But we want discussion moved to Ethereum Magicians. It's not a healthy practice to have a lot of open issues.

We were thinking of creating a bot, marking them as stale issues.

How do we encourage people to open an issue if there's an issue, not for general discussion?

EIP editors may have to go through these issues and close them.

What are ways of encouraging Ethereum Magicians for discussion, and only post issues if there are issues?

Micah suggests just being firm with people.

We currently have the bot have them look at EIP-1 when they create an issue. We can add some phrase to say, if it's an issue for discussion, to use Ethereum Magicians instead.

## Decisions

- **41.3** - Bot will show a notice to new issues to make a discussion thread on Ethereum Magicians instead. All discussion focused issues will be closed by the editors, encouraging to happen on Ethereum Magicians.


# 4. EIPs Insight - Monthly EIPs status reporting

Video | [40:02](https://youtu.be/54j6VK6ska0?t=2402)
-|-

Pooja recently started curating a list of EIPs which are changings statuses. This will be used a very niche audience. But Pooja expects it to be used longterm. It's a monthly report.

If anyone has suggestions, please let Pooja know. 


# 5. Review action items from the previous meetings

Video | [40:57](https://youtu.be/54j6VK6ska0?t=2457)
-|-

We are now following once a month EIPIP meetings. 

# 6. Closing Discussion

Video | [42:08](https://youtu.be/54j6VK6ska0?t=2457)
-|-

There's been discussion to Rollups. Optimism is changing their approach to rollups. It would be 1 for 1 compatible with mainnet. For users, it looks like using an Ethereum sidechain. It has the security of a rollup, but looks like Polygon to a user.

Does anyone have thoughts of developing an open rollup specification? And where should things like that live?

Micah: Isn't the idea of rollups that we don't standardize, so people can experiment?

Lightclient: People want all the tools to work like it works on Ethereum. There may be value for specification that's one for one with Ethereum with regards to rollups.

Micah: If people want to create an EIP for rollups, it would probably be an ERC. Rollups may not be the best place for standardization. It's not how we progress, it's how we do the same thing. 

Lightclient: Roll up teams are re-engineering the same work. That's not a problem?

Micah: There's re-engineering, but also exploration and experimentation. 

Lightclient: There's the exploration and experimentation of the runtime environment. It's a different virtual machine. And there's the backend which the users don't see, but allows verification on mainnet. Now we're trying to make a standard to verify on mainnet. Which part are you referring to with exploration?

Micah: Both. Arbitrum had a different mechanism for fraud proofs. Optimism may be switching to Arbitrums solution. That's valuable, that Arbitrum tried something different. When we introduce standards, people are more likely to follow the standard, than exploring other solutions.

Lightclient: I'm on board with people building different runtimes. I'm worried when people have an endgoal of people recreating Ethereum. When you have 3-4-5 teams implementing this, there's a lot of people doing the same work. If they just worked together it may be better.

Micah: It sounds like you want an open source project instead of a rollup. There would be a library repository where both teams contributed to. If they want to share code, the best place is opensource. 

Lightclient: Both are opensource, with different licenses. 

Micah: We have several flavors of Linux, but the same kernal. That's reasonable. However, writing a standard may not be the right solution.

Lightclient: Curious on thoughts. The way Ethereum was launched, we didn't have a mechanism to fund the development of the protocol. We may be passed where it's possible to introduce this in L1? What do we think about rethinking this in L2?

Micah: I like the idea of someone getting paid to build useful things. The problem is deciding who gets paid, and how much. It's easy when a company is doing this, and they decide. It's harder when there's no company, and just a group of people working together. There's the Ethereum Foundation, but they're not running things. For rollups, if we had a central development team, then there's no problem. If they're trying to build a rollup that's decentralized and leadership, there may be issues.

Lightclient: I think there may be ways of doing it. Some bad, some not as bad. What I'm thinking, why can't someone just fork it and deploy their own rollups.

Micah: I think the feeburning is a good place. It exist for decentralization systems. We have to send them somewhere. They can go anywhere. Why we decided to burn them in L1, it is too conentious for them to go somewhere else. I think fee burning is a good opportunity in L2. 

Lightclient: My end goal is having some social pressure for those funds to go to public goods. It would be great if there was more friction to changing where fees go than changing a line of code. Similar to how eth2 was originally described. Shards of execution which communicate well, because they move forward together, and go back together. There may be coordinated rollups, communicated between blocks for rollups. People can create a new rollup, but they'd have slower finality.

Micah: The warning I'd give, everytime charitable donations have been forced, they've been captured. By allowing people to do charitable donations on their own, it's a strong determinant on capture. If we enforce people sending there money somewhere. It is very sticky, then there will be incentive to capture. If it's optional, then it's harder to capture.

Separate discussion.

Do we want to continue the 1 month? Or continue the biweekly calls, then cut it short?

We'll go back to 2 weeks.

---

# Annex

## Attendees 

- Alita Moore
- Brent Allsop
- Edson Ayllon
- Felix
- Lightclient
- Micah Zoltu
- Pooja Ranjan


## Next Call 

Wednesday, October 06, 2021, 15:00 UTC.

