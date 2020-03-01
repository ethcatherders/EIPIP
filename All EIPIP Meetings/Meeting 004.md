# EIP Improvement Process Call #4 Notes

### Meeting Date/Time: Wednesday, 26 February 2020 at 15:00 UTC
### Meeting Duration: 1 hr 
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=c0DUKVNvML0)
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/6)
### Moderator: Pooja Ranjan
### Notes: Edson Ayllon


----
	
# Summary

## Actions Needed

Action Item | Description
---|---
**4.1** | Reach out to Nick Johnson and contributors to update the EIP bot. 
**4.2** | "Hard fork," "network upgrade" terminology PR to EIP-1 to be merged. 
**4.3** | James Hancock to split PR defining kinds of network upgrades.
**4.4** | Create a guide for EIP champions.
**4.5** | Discuss possible Code of Conduct for public Ethereum messaging platforms.
**4.6** | Create some resources for developers to create new Ethereum clients (Eth1.x).
**4.7** | Update EIP specifying EFI to `accepted` or `final`, then change EIP-1 to include EFI.
**4.8** | Brent to open PRs updating EIP-3 and EIP-107 status. 
**4.9** | Create a champions list header, add to EIP-1.
**4.10** | Further discuss recommending authors and champions be introduced (background) in the discussion-to conversation linked in EIPs. 


## Decisions Made

Decision Item | Description
---|---
**4.1** | Sourcecred no longer pursued. 
**4.2** | Pursue creating some resources for developers to create new Ethereum clients (Eth1.x) to some extent. 
**4.3** | Discuss the Code of Conduct creation in a future call. 
**4.4** | Create a champions list header, add to EIP-1.
**4.5** | Further discuss recommending authors and champions be introduced (background) in the discussion-to conversation linked in EIPs. 

--- 

# Agenda


---

# 1. Review Previous Meeting

**`video`** [`2:20`](https://youtu.be/c0DUKVNvML0?t=140)

Updates on [previous action items](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20003.md):
- Updates to the EIP bot haven't been made yet. Nick Johnson can be reached out to for that. 
- Tim Beiko [opened PR](https://github.com/ethereum/EIPs/pull/2516) for updating terminology in EIP-1. PR is still outstanding.
- James Hancock's PR defining different kinds of upgrades and updating format and adding to the list of upgrades still not split.
- Guide for EIP champions not completed.
- The code of conduct was to be discussed but may need to be pushed to the next meeting.
- James Hancock brought up https://sourcecred.io/ on Telegram, no longer recommends this resource for the EIP repo

## Actions

- **4.1**—Reach out to Nick Johnson and contributors to update the EIP bot. 
- **4.2**—"Hard fork," "network upgrade" terminology PR to EIP-1 to be merged. 
- **4.3**—James Hancock to split PR defining kinds of network upgrades.
- **4.4**—Create a guide for EIP champions.
- **4.5**—Discuss possible Code of Conduct for public Ethereum messaging platforms.


## Decisions

- **4.1**—Sourcecred no longer pursued. 


# 2. Keeping Ethereum Resources Up-To-Date

**`video`** [`9:03`](https://youtu.be/c0DUKVNvML0?t=543)

There's often a delay in getting contents on the yellow paper, beige paper, etc. up to date. 

**Tim Beiko:** Proposes using grants to update these resources following each hard fork. 

**Hudson Jameson:** This kind of change may be out of the scope of these meetings. And updating these papers, there may be controversy as to deciding what EIPs are considered canonical.

**James Hancock:** For someone wanting to develop a new client, sorting through all EIPs to know what to develop may be a barrier. Suggests possibly opening community grants. 

**Hudson Jameson:** It's a good idea, but not a high priority. If it can't be completed, because of funding, or not finding resources to do so, it should be ok being left not done. 

**GuthL:** Creating a book, similar to Programming Bitcoin, may be a good solution for developers wanting to create a client.

**Hudson Jameson:** If the book is created for Eth1.x, would the work go to waste if it's completed after Eth2.0 is live?

**GuthL:** The timeline for Eth2.0 is unknown, and concepts would carry over if Eth1.x was replaced by that time.

**William Swab:** Investing in a process like this would teach us how to invest in a process like this, which would carry over to Eth2.0. Whatever we invest in Eth1.x may find uses elsewhere also. 

**GuthL:** Thomas, from Nethermind, has a long print-out going into the EVM. We should reach out to him.

**Hudson Jameson:** All sounds like a great idea. My mind is changed. We should pursue this at some level. 

## Actions

- **4.6**—Create some resources for developers to create new Ethereum clients (Eth1.x).

## Decisions

- **4.2**—Pursue creating some resource for developers to create new Ethereum clients (Eth1.x) to some extent. 

# 3. Code of conduct

**`video`** [`17:45`](https://youtu.be/c0DUKVNvML0?t=1065)

In a previous meeting, there was a suggestion to create a Code of Conduct enforced in the Ethereum Gitter channels, and other communication platforms to limit bad behavior. A Code of Conduct was created for the Ethereum Cat Herders. That may be used as a reference, but with a different scope for the All Core Devs. 

**James Hancock:** Something to consider is how Github's features may allow something unintended for the EIP repo. 

Discussion to be continued when Danno is present. 

## Decisions

- **4.3**—Discuss the Code of Conduct creation in a future call. 

# 4. Progress on EIP Repo Cleanup

**`video`** [`20:53`](https://youtu.be/c0DUKVNvML0?t=1253)

Pooja created a presentation outlining the current EIP process. See the video to see the presentation. 

**Pooja Ranjan:** For the clean-up process, we should identify the type, sub-type, and what the status options are for that given EIP to move to the next phase. If an EIP meets the requirements for a status change, a status change can be proposed. 

**Hudson Jameson:** Add to the spreadsheet if the EIP author had been reached out to, and what their response was. Something to think about: If throughout the EIPIP we decide to change how the current EIP process works, we may need to perform this cleanup process again. 

**Pooja Ranjan:** Once an EIP is abandoned, if a new author/champion decides to continue it, the header information may change.

**Hudson Jameson:** We may need to update the EIP-1 template, to ensure changes in authors and champions stay within the history of the EIP. 

**Pooja Ranjan:** The Eligible for Inclusion (`EFI`) status is not mentioned in EIP-1. James has a PR for EIP-1, but the EIP which talks about EFI is still in the `draft` status. I recommend first updating the EFI EIP to `accepted` or `final` status before updating EIP-1. 

**James Hancock:** I suggest having a champion section in the EIP header, as there are champions who don't want to be authors, displaying 1-2 names. Knowing who the current champion is would be helpful to know who to reach out to. And have the authors being the history of authors, newest to oldest, as to have a standard of changing the authors header. 

**Pooja Ranjan:** 
1. We should create a checklist for requirements allowing an EIP status change to quickly update stale EIPs. 
2. We don't have a template for each EIP category. We can create those templates, and add it to EIP-1.

**James Hancock:** Any thoughts on having a champions section, and the order of authors? I'm more comfortable updating a champions section than adding new authors. 

**Brent Allsop:** Wanted to comment that the authors of EIP-3 and EIP-107 have been contacted. The pull requests for those [are ready to be made](https://github.com/BrentAllsop/EIPs/blob/master/EIPS/eip-3.md). 

**Hudson Jameson:** Can we make the EIP status cleanup spreadsheet into a Google Sheet?

**Pooja Ranjan:** Will do. Any final comments?

**Edson Ayllon:**  Yes, for the champions header, if we were to keep a history of champions, if we assume there can be more than one champion at a given time, it may be good to label the current champions as current (ie. `John Doe (current)`).

**James Hancock:** The author list is the history of authors. The champion list is just the current champion, limited to 1-2. When I was the community champion for BLAKE2B, I would have preferred not to be included in the authors list, as I wasn't changing the technical specification. 

**Edson Ayllon:** Makes sense. 

**GuthL:** Regarding the champions, should we require new champions/authors to disclose their motivation for pushing an EIP forward? This may help identify conflicts of interest. How an EIP benefits the authors/champions should be public. 

**James Hancock:** I like the idea to know where people are coming from with EIPs. 

**Hudson Jameson:** We have a motivations section. 

**GuthL:** Motivations section is limited to technical motivations. 

**Hudson Jameson:** What is the benefit of people knowing why an EIP exists outside of a technical purpose?

**GuthL:** It creates transparency. For ProgPoW, there was information that was revealed that wasn't disclosed prior. Similar issues happened with BLAKE2. 

**Hudson Jameson:** A compromise may be to expand the motivations section to include technical and nontechnical subheadings. 

**GuthL:** I think people should be transparent on their motivations. 

**William Swab:** Adding a section to an EIP may not guarantee that people use it honestly. 

**Hudson Jameson:** Also, for technical standards, motivations shouldn't exceed the technical purpose of a standard (I want to use this for that). 

**James Hancock:** Also, coming to terms that if someone suggests an EIP, it will most likely always benefit them somehow, or they would never suggest it. 

**William Swab:** It's unfair to assume that if something benefits the author, that it negatively affects everyone else. Anytime anyone invests effort into anything, it would be because they receive some sort of utility from it. 

**Edson Ayllon:** Maybe a disclosure like that may be more appropriate in the "Discussion-to" section. There the champion is introduced if they are changed. 

**Hudson Jameson:** Yes. That's something we can highly recommend in the discussion-to. Not in the header, but within the linked discussion. 

**James Hancock:** That would be a great thing to add to the recommendations. An author needs to introduce themselves, and why they're stepping up to champion. 

**Hudson Jameson:** I like that idea. We may need to talk it some more. 

**James Hancock:** Luis, does that fit what you were looking for?

**GuthL:** I didn't catch that last part. I think we should discuss it in EthCC. 

## Actions

- **4.7**—Update EIP specifying EFI to `accepted` or `final`, then change EIP-1 to include EFI.
- **4.8**—Brent to open PRs updating EIP-3 and EIP-107 status. 

## Decisions

- **4.4**—Create a champions list header, add to EIP-1.
- **4.5**—Further discuss recommending authors and champions be introduced (background) in the discussion-to conversation linked in EIPs. 

# 5. Closing Remarks

**`video`** [`54:15`](https://youtu.be/c0DUKVNvML0?t=3254)

**William Swab:** How can someone contribute to helping update the yellow paper, etc.?

**Hudson Jameson:** I would ask in Telegram, and me and others can help.

**William Swab:** Is anyone getting together in EthCC? 

**Hudson Jameson:** I would make a Telegram chat for those going. 

---

# Annex

## Attendees

- Anett Rolikova
- Brent Allsop
- Edson Ayllon
- GuthL
- Hudson Jameson
- James Hancock
- Pooja Ranjan
- Tim Beiko
- William Schwab

## Next Call

Wednesday, March 11, 2020, 15:00 UTC.
