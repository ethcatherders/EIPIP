# EIP Improvement Process Call #8 Notes
### Meeting Date/Time: Wednesday, 20 May 2020 at 15:00 UTC
### Meeting Duration: 1 hr
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=OP5Z8BVSlqs)
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/16)
### Moderator: Hudson Jameson
### Notes: Edson Ayllon

----

# Summary

## Actions Needed

Action Item | Description
---|---
**2.1** | Contact Nick Johnson on whether to put supplemental information about EFI in EIP-1 or the EFI EIP.

## Decisions Made

Decision Item | Description
---|---
**2.1** | The EIPIP survey will be finalized by 2 weeks from this meeting (by the next meeting).

---

# Agenda

- [1. EIP centric model subgroup, next steps](#1-eip-centric-model-subgroup-next-steps)   
- [2. EFI to its own EIP, referenced in EIP-1](#2-efi-to-its-own-eip-referenced-in-eip-1)
- [3. EIPIP Survey](#3-eipip-survey)    
- [4. Making decision-making async from ACD calls](#4-making-decision-making-async-from-acd-calls)   
- [5. Separation of EIP process and hard-fork coordination](#5-separation-of-eip-process-and-hard-fork-coordination)   


---

# 1. EIP centric model subgroup, next steps

Video | [0:00](https://www.youtube.com/watch?v=OP5Z8BVSlqs)
-|-

Conversation slated for another meeting.

# 2. EFI to its own EIP, referenced in EIP-1

Video | [1:46](https://youtu.be/OP5Z8BVSlqs?t=105)
-|-

This topic is on deciding having more information about EFI in EIP-1 or the EFI EIP, with documenting hard-fork coordination. No decision was made in regard to this in previous meeting.

The next step is to contact Nick Johnson on where to place this information.

Nick Johnson's original position was not to have the process of specifications and deployment both in EIP-1. So the hard-fork meta EIP was made instead of being included in EIP-1. But later his opinion was thought to have changed.

## Actions

- **2.1**—Contact Nick Johnson on whether to put supplemental information about EFI in EIP-1 or the EFI EIP.


# 3. EIPIP Survey

Video | [5:36](https://youtu.be/OP5Z8BVSlqs?t=336)
-|-

The survey was sent out to everyone who has pushed their EIP all the way to final status. This represents sampling bias in not directly contacting EIP authors who have not completed the EIP process to completion by not having their EIP be in `final`. However, the list of EIP drafts is quite long. The decision is to finalize the EIPIP survey by next meeting to start acting on suggestions.

Findings of what respondants like about the current process may be helpful to know what parts of the process not to change. They are as follows:

- The current EIP process is well defined and structured, focuses on the technical aspects, and has legitimacy.
- The barrier to entry is low, anyone who wants to take part in the process can.
- The process for approving EIPs is democratic, transparent, and allows for a fair and thorough review with a high bar of acceptance.

For how to continue from the feedback from the survey, the higher order concerns requiring the most change will be addressed first, and then the smaller suggestions will be put into place of the newer process.

- https://medium.com/ethereum-cat-herders/the-feedback-that-improves-ethereum-ff4f3f36a8e2

## Decisions

- **2.1**—The EIPIP survey will be finalized by 2 weeks from this meeting (by the next meeting).

# 4. Making decision-making async from ACD calls

Video | [13:32](https://youtu.be/OP5Z8BVSlqs?t=812)
-|-

This current topic is still undecided.

**Tim Beiko**: We just mentioned trying to get Nick Johnson's opinion, and he can't come to these calls. In general, if we're moving the hard-fork coordination process outside of the EIP process, we should look into how to make both those processes less reliant on the calls. It may be easier for the EIP process vs the hard-fork coordination process.
- It would be more inclusive
- Comments are much clearer in writing
- Text is searchable

**Edson Ayllon**: Making the calls async was feedback also. One feedback was that the decision making process was too reliant on live calls. It may be that those who want to get involved can't due to timezones.

**Hudson Jameson**: I agree with that assessment. We may push things more to the Ethereum Magician's forum for example.

**Edson Ayllon**: Artem last time recommended Zulip.

**Hudson Jameson**: He made a Zulip and I joined it. I haven't seen progress on that. I don't think we can get people to move to Zulip. Getting a new tool involved isn't impossible, but may be a lot of friction.

**Pooja Ranjan**: Eth Magicians may be the best place to do that.

**Hudson Jameson**: Changing EIP-1 to say, definitely go to Eth Magicians, rather than going to one of many.

**Pooja Ranjan**: EIP-1 suggests Eth Magicians. We may want to work with the words there.

**Hudson Jameson**: I agree.


# 5. Separation of EIP process and hard-fork coordination

Video | [17:20](https://youtu.be/OP5Z8BVSlqs?t=1040)
-|-

Axic's model seeks to simplify the EIP procses by reducing the number of statuses, and seeks to decouple the EIP process from the hard-fork coordination process.

The major change is the review step. `Review` is for EIPs to recieve feedback before `Last Call`. Many people don't want to give feedback if the EIP is still changing. However, `review` specifies that the EIP author isn't addiing more changes himself, an is looking for more external review.

Axic's model reduces `Withdrawn` and `Abandoned` to only `Withdrawn`.

In this model, `Final` means that the specification will no longer be changed, that it is frozen, rather than stating that it's in a hard-fork. Once an EIP is final, in this model, it is ready to be decided on for hard-fork coordination, facilitating the EIP centric process.

If the network upgrade process has its own review process, and an issue is found, then the change should be made in a new revision EIP under a new number.

Jame's model is the same, except it introduces `Inactive` to replace `Abandoned`.

**Edson Ayllon**: I think it's good that final means the spec is frozen. That way final can mean the same thing for every track.

**Tim Beiko**: And I really like this state that calls for a broader community review. There have been instances in the past where an EIP isn't looked at until it's scheduled for a hard-fork. And it's also not possible to go through each EIP that's in `Draft`.

**Pooja Ranjan**: Do we keep `Active` after review or after `Last Call`? `Last Call` increases visibility and adds to the RSS feed.

**James Hancock**: With `Review` and `Active` once made `Active` it can go back into `Review` to increase visibility before becoming active again.

**Hudson Jameson**: The purpose of `Last Call` is to make it into the RSS feed.

**James Hancock**: We should make a feed for `Review`. Make the feed fit the process, rather than make the process fit the feeds.

**Axic**: There was a PR for having a feed for every status that wasn't completed. Making a feed for each one shouldn't be hard. `Active` was originally for EIP-1, but then extended to registries. I don't know the right process for getting to `Active`. Instead, we should define which EIPs can become `Active`. I don't think it's good to get rid of it.

**Hudson Jameson**: I don't think we should get rid of it either, going through superceding EIP-1 for every small change. It adds more bueracracy for no gain.

**Pooja Ranjan**: We can at least follow the steps of other EIPs.

**Axic**: I think your reasoning makes sense. There's no particular reason I put `Active` there. But `Last Call` is the last step before you make it final. The reason is you want to make sure it's right because then you can't make changes. However, this isn't the case with `Active` as it can undergo changes.

**James Hancock**: I would agree. It's an uneccessary extra step.  `Last Call` and `Final` come together.

**Hudson Jameson**: For Pooja's argument, we have no process between `Review` and `Active` to how it becomes `Active` again.

**James Hancock**: That should be up to the actual registry. The EFI list was stated on the call, so it's updated. Chain ID has it's own process

**Hudson Jameson**: So each EIP has it's own Champion which decides how it gets updated, right?

**James Hancock**: Right, or processes decides that. Some changes wouldn't need to go into `Review`. If I was adding an EFI EIP, it shouldn't go back to `Review`. But if I was adding a step to the process, it should, to signal to people there are significant changes.

**Hudson Jameson**: I like that each has its own process, as long as that process is defined in the EIP itself.

**Pooja Ranjan**: I have no "over my dead body" feeling on this. I'm willing to go with the decision of the group.

**Brent Allsop**: Just a comment. I'm not seeing much decision making being formalized. Where do we make decisions? And where does ProgPow fit in this.

**Hudson Jameson**: The reason we're separating decision processes is that there are so many dependant on the track. How are decisions made, if we were to combine them, it would add complexity. We haven't started thinking about decision-making yet.

**Edson Ayllon**: Another comment. One of the frustrations among a lot of people I was seeing was politics in the EIP process. It was hard to understand what people meant by that. But we can start addressing that by isolating that part from the EIP process. To put it in its own section where its addressed formally.  As far as the decision making process, I think it should start with EFI.

**Hudson Jameson**: And for Core EIPs in general.

**James Hancock**: Whatever the new process ends up becoming.

**Brent Allsop**: I think it answered my question. And does ProgPow fit anywhere?

**James Hancock**: It would be in `Final`, because the specification is final. Really they should be making a new EIP at this point, since this was clarified. But it would be reflected in the network upgrade process as not going into mainnet.

**Pooja Ranjan**: We are trying to separate the hard-fork process and the EIP process.

**Brent Allsop**: Sounds good. Makes me nervous. Everyone's afraid to touch decisions.

**James Hancock**: The new graph stemed from the conversation of `Withdrawn` vs `Abandoned`. I'd like to add automation with the EIP bot. Also, make it clear for the community if it's withdrawn because no one is working on, or if it was intentially stopped.

**Hudson Jameson**: The one thing is, `Inactive` sounds too much like active.

**James Hancock**: `Active` could be changed.

**Hudson Jameson**: I've thought about it. I don't have a better word.

**James Hancock**: I haven't thought about it either. I don't want them to be thought of as connected either.

**Axic**: Automation is a great idea. However the EIP number could be inflated because of small PRs upating whitespace to keep it from being `Inactive`.

**James Hancock**: I'm concerned about the EIP number inflation as well. We could decide a new method EIP numbers are assigned. As far as the editing goes, changing one thing to keep it in `Review` means they're actively looking at the repository.

**Hudson Jameson**: Regardless of EIP numbering, it's good to have two separate statuses for communnity clarity. There's no where in the EIP stating why it became `Withdrawn`. For an outside viewer, they can accuse an author of being lazy with the EIP and that they didn't care.

**Axic**: EIP-1 specifies a resolution header. Using that may clarify the reason. Wouldn't that be a better solution than having 2 status fields?

**Hudson Jameson**: It's already in there, so not much work needs to be done.

**Edson Ayllon**: In regards to automation and the PR number, RFC has a timer of 24 months, 2 years, to be questioned if it's in `Withdrawn`. We can have the EIP bot open a PR based on the creation date after X months, and ping the author. If there's no response, it should be merged as Withdrawn.

**Hudson Jameson**: I like that automation.

**Pooja Ranjan**: One thing is missing, which is EIPs getting resurrected after moving to Abandoned. And EIPs changing their ownership. I'm more towards having one status with a broader explanation.

**Hudson Jameson**: I think we're getting to utilizing the resolution header.

**James Hancock**: If the PR explosion number was resolved, would this resolve pieces for this?

**Axic**: I'm personally worried adding more statuses than we need. If we make use of the resolution field, we don't need the `Inactive` phase.

**James Hancock**: The part we would be missing is with navigating EIPs. Someone trying to understand where it is may take some time going through each one.

**Axic**: One thing to consider is who the target audience. Why would the person care if it's `Withdrawn` or `Inactive`.

**James Hancock**: It would matter for controversial EIPs. If they are `Inactive` people may be worried it may resurrect.

**Axic**: However, you're deciding not to work on it. Someone else may be able to resurrect it.

**James Hancock**: But it would have to be a new number. The community members can see it was something proposed, and it's no longer proposed.

**Axic**: We should clarify if `Withdrawn` can be resurrected. I understood any `Withdrawn` could be. The second is, aren't we mixing the specification process with the hardfork process?

**Hudson Jameson**: The problem is, the community could say, "It can be snuck in at any time." They're doing that with ProgPow right now. I know it's not accurate. But they're conflating EIP-1 for their own narrative. If we can make it more strict, it's harder to do that. There's a finality to it.

**Axic**: But there's no finality since it still can be resurrected.

**James Hancock**: Techincally yes, but the community interprets it differently.

**Edson Ayllon**: Well, an EIP can be final even if it's controversial, because `Final` means it's frozen. And `Withdrawn` just means the spec isn't being worked on to be made `Final`.

**James Hancock**: Another EIP that would be `Withdrawn` is Martin's EIP. It was withdrawn for Oil and Gas, as it was superceded.

**Axic**: The resolution field couldn't explain this?

**Hudson Jameson**: Not quickly.

**Axic**: It can be displayed in the listing as well. The resolution header. I would just do resolution text, a single sentance.

**Hudson Jameson**: Having a status would have people going into the sentance explanation knowing if it was intentional.

**Axic**: Having this special meaning for `Withdrawn` if it can be resurrected makes no sense. If `Withdrawn` has finality, then I see a reason for `Inactive`.

**Hudson Jameson**: I think that's good.

**James Hancock**: I'd be fine with that. You'd have to make a new EIP to pursue it.

**Axic**: What would accurately explain that is `Rejected` which is in the network upgrade process.

**Hudson Jameson**: We wouldn't need that.

**Axic**: Wouldn't it be rejected by community?

**James Hancock**: It's different.

**Hudson Jameson**: This might be good to pick up for next time. Except for `Withdrawn`/`Abandoned` section, we're coming close to a resolution, which would be a large step.

---

# Annex

## Attendees

- Alex (axic)
- Brent Allsop
- Edson Ayllon
- Hudson Jameson
- James Hancock
- Jim Bennett
- Pooja Ranjan
- Wei Tang

## Next Call

Wednesday, June 3, 2020, 15:00 UTC.
