# EIP Improvement Process Call #31 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, Apr 21, 2021 at 15:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=n1E1dreOMFE) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/65) <!-- omit in toc -->
### Moderator: Pooja Ranjan <!-- omit in toc -->
### Notes: Edson Ayllon <!-- omit in toc -->

----

# Summary <!-- omit in toc -->

## Decisions Made <!-- omit in toc -->
**31.1** | ERC authors must go to the EIP repo to assign themselves a number.

## Actions Needed <!-- omit in toc -->

Action Item | Description
-|-
**31.1** | Create ERC repo
**31.2** | Update https://eips.ethereum.org with changes to EIP/ERC repo
**31.3** | Create a bounty for JSON RPC API spec
**31.4** | Complete EIP repo bot
**31.5** | Determine pay rate for EIP Editors
**31.6** | Add an ERC dedicated editor

---

# Contents <!-- omit in toc -->

- [1. Splitting out EIP repos into EIPs & ERCs Ref: Issue](#1-splitting-out-eip-repos-into-eips--ercs-ref-issue)
  - [Actions](#actions)
  - [Decisions](#decisions)
- [2. Progress on JSON RPC API spec in Eth1.0 repo](#2-progress-on-json-rpc-api-spec-in-eth10-repo)
  - [Actions](#actions-1)
- [3. Progress on EIP GitHub repo action bot. Ref: Issue](#3-progress-on-eip-github-repo-action-bot-ref-issue)
  - [Actions](#actions-2)
- [4. Progress on 'canonical source for EIPs'](#4-progress-on-canonical-source-for-eips)
- [5. Review action items from the previous meeting](#5-review-action-items-from-the-previous-meeting)
- [6. Open Discussion](#6-open-discussion)
  - [Actions](#actions-3)
- [Annex](#annex)
  - [Attendees](#attendees)
  - [Next Call](#next-call)

---


# 1. Splitting out EIP repos into EIPs & ERCs Ref: Issue

Video | [0:00](https://youtu.be/n1E1dreOMFE)
-|-

This topics continues from previous meetings.

The challenge with splitting to separate repos is the numbering scheme. Suggested solutions included a bot, or a notification system. 

One proposal was creating an issue in the EIPs main repo to get the ERC number.

Hudson suggested the editors just doing it manually, like its done now.

A bot would need to see open PRs, in addition to looking for conflicts. Lightclient suggests it may just be easier to have a spreadsheet that tracks it, instead of building automation.

Micah says ERC authors going to the EIP repo to grab a number may do the same thing as a spreadsheet, without introducing a new tool. The next step would be automating.

Lightclient suggests, notifications won't be improved by separating the repos if we have ERC authors go to the EIP repo and open an issue.

The group agreed on ERC authors going to the EIP repo for getting the number. Single line issues.

The final blocker is getting the ERC repo created. Hudson will connect the EF admins with Micah and Lightclient.

Ethereum Cat Herders may publish a blog stating the ERC repo changes.

Updates may need to be changed on eips.ethereum.org.

## Actions

- **31.1**—Create ERC repo
- **31.2**—Update https://eips.ethereum.org with changes to EIP/ERC repo

## Decisions

- **31.1**—ERC authors must go to the EIP repo to assign themselves a number.

# 2. Progress on JSON RPC API spec in Eth1.0 repo

Video | [16:17](https://youtu.be/n1E1dreOMFE?t=977)
-|-

Alita not completely sure if she's going to continue working on this. She worked on ethCall, and submitted the Eth block number spec.  Expected to have ethCall this week.

Pooja proposed having a list to track this to Thomasz as an issue. Then having a group of reviewers, reviewing the PRs before being merged.

Tomasz said we're starting with block number, then ethCall. When ethCall is finished, this will give an estimate for the effort on the remaining specifications.

After that, we can make it more open. Publish it as a gitcoin bounty. If other people want to participate, or compete for the spot, it may be the way to go. 

Alita opened a JSON RPC discord channel. The reviewers should be client team developers. But it may be too early to use everyone's time.

The client developers can approve all the edge cases. The technical approvers, it's up to the cat herders to decide. Feedback can be recieved from the client teams.

Pooja says, the cat herders may not be technical enough to see if it is done.

Are we planning to share this information to the discord group?

Tomasz says it will be on the ACD channel when the full spec is ready. Work in progress specs will be shared in the channel Alita made.

## Actions

- **31.3**—Create a bounty for JSON RPC API spec

# 3. Progress on EIP GitHub repo action bot. Ref: Issue

Video | [25:22](https://youtu.be/n1E1dreOMFE?t=1522)
-|-

The last comment is 5 days ago. What is the status, can it be closed?

Alita says we are making progress. This week, it may be done, depending on the bandwidth of reviewers. 

It's starting to get close to functional. It has hacks, but less than the bot that is currently used.

Shout outs to Micah and Alita for this. 

## Actions

- **31.4**—Complete EIP repo bot


# 4. Progress on 'canonical source for EIPs'

Video | [29:09](https://youtu.be/n1E1dreOMFE?t=1749)
-|-

Still working on it. Trouble getting time to get it done. Progress is slow, buot making progress.


# 5. Review action items from the previous meeting

Video | [29:38](https://youtu.be/n1E1dreOMFE?t=1778)
-|-

- EIP and ERC repo progress made
- JSON RPC spec being worked on
- We have updated remove testing greenlight from EIP process
- Going forward with  a different approach for reducing EIP/ERC number overlap
- Tomasz made plan for bounty
- Tim Beiko still needs to bring up changes to EIP process to ACD, maybe next meeting


# 6. Open Discussion

Video | [31:43](https://youtu.be/n1E1dreOMFE?t=1903)
-|-

We are considering on getting EIP/ERC editors funded. Can anyone suggest a pay rate?

Estimating how something should be worth is difficult. And it also depends on how much funding we get.

Do we want editors that understand the Ethereum ecosystem? Or those who just know how to write a good standard. 

The ones who understand the EVM, those will be very expensive, since the supply is low, and they have a lot of experience.

Is the intention to pay active editors? Or bring up new editors?

Pooja and Hudson says it is both.

Maybe offline, we should prepare what would be a fair rate from Lightclient and Micah.

Maybe we can do a full-time and part-time role, separate funding rates.

Or we can model based on the ETF. There are editorial roles, then overseeing comittee. 

Someone with deep Ethereum knowledge is required, for at least moving EIPs to final. 

The people who this kind of role would attract are those without a fulltime job already. A freelancer inside of Ethereum.

We're looking for an ERC only editor. ERCs make up about half of all EIPs. And they tend to be lengthy. So just getting them to editorial standards is time consuming.

## Actions
- **31.5**—Determine pay rate for EIP Editors
- **31.6**—Add an ERC dedicated editor

---

# Annex

## Attendees 

- Alita Moore
- Brent Allsop
- Hudson Jameson
- Lightclient
- Micah Zoltu
- Pooja Ranjan
- Tomasz Stanczak
- Trenton Van Epps

## Next Call 

Wednesday, May 05, 2021, 15:00 UTC.

