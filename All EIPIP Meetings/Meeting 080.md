# EIPIP Meeting 80 Notes
### Meeting Date/Time: Wednesday, May 3, 2023, at 14:00 UTC
### Meeting Duration: 0.5 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/229)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=QwQU9_Gi7GI)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION/DECISION  ITEMS

**ACTION 80.1**: In regards to  EIP bot numbering & PR-6976, No agreement on merging the PR as yet. It can use better wording. Will be discussed async on Discord or PR itself.

**ACTION 80.2**: In regards to Bug with EIP-5507 Last Call date, It looked like GitHub page issue and is resolved now.

**ACTION 80.3**: under the Reviewer working group, @xinbenlv shared about the new ERC meeting group. Ref [FEM post](https://ethereum-magicians.org/t/call-for-a-regular-allercdevs-virtual-meetup/14028)

—------------------
## AGENDA

## 1. Discuss Open Issues/PRs, and other topics

- [Update EIP-1: Clear rules regarding EIP numbering ethereum/EIPs#6976](https://github.com/ethereum/EIPs/pull/6976)

**Pooja Ranjan** [0:00](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=00s): So starting with the first item which is an update to eip1 and which is also related to Auto numbering of eips along with the permission to merge eips as draft automatically. The pull request number here is 6976, anyone on the call maybe like to give an overview of where we are in numbering these proposals like automatically numbering and what editors think about this PR to be merged. 

**Light Client** [0:48](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=48s): where's Greg?

**Pooja Ranjan** [0:54](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=54s): Oh yeah he isn't on the call.

**Light client** [0:57](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=57s): Looks like I just don't understand what we spend most of the call talking about his proposals that he's 
never here.

**Pooja Ranjan** [1:07](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=67s): That's a good question but yeah sometimes it is difficult for people to be here and we try to discuss it async as well.

**Light Client** [1:18](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=78s): So we moved the call so that he could be here. Though he hasn't been here in two months or more.

**Pooja Ranjan** [1:32](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=92s): Right,
if I understand correctly he will be available soon. I think summer vacation is coming up so he should be able to join calls regularly but yeah we can probably think I mean like a collect thoughts from other editors what they think about this pull request which is to update EIP numbering.

**Sam** [2:17](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=137s): I'm not sure. I'm totally on board with the exact wording that's there right now but we'll hammer it out in the PR.

**Pooja Ranjan** [2:31](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=151s): That makes sense.

**Light Client** [2:34](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=154s): I thought when he introduced it it was opt-in doesn't seem like it's the case now. 

**Sam** [2:39](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=159s): For what? The bot ?

**Light Client** [2:42](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=162s): I thought that editors still retained the ability to assign members. It was like if you wanted to opt in to
letting the bot assign numbers for you. You could but now the wording is replaced.

**Sam** [2:57](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=177s): Oh we're looking at something different than the clear rules regarding EIP numbering.

**Light Client** [3:03](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=183s): I was thinking of the numbering bot. 

**Sam** [3:06](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=186s): Oh! okay yeah so the bot right now doesn't work. So I turned it off. But it's yeah it just assigns the number on merge and overrides whatever's in the EIP

**Light Client** [3:20](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=200s): I mean I don't really care that much because I will probably opt in but it's just one of these things where it's not quite what we talked about.

**Sam** [3:33](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=213s): Do we want it to be opt-in or do we want it to be mandatory?

**Light Client** [3:40](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=220s): I mean if everybody is okay with opting in that's okay. I don't know if Greg was on board with opting in. 
I don't remember .

**Sam** [3:49](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=229s): I think Greg was like one of the the strongest proponents for the bot.

**Light Client** [3:55](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=235s): Okay, yeah.

**Pooja Ranjan** [4:04](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=244s): In my mind having uniform rule would be ideal instead of having it opt-in because opt-in will require some Editor to obviously chime in and provide an EIP number and it can be confusing for new Authors. So yeah either we go by editors providing numbers or maybe activate the bot for it. 

**Sam** [4:34](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=274s): I think we're just gonna have to talk to Panda about this in Discord and see what's going on there.

**Justin Florentine** [4:40](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=280s): So does anybody have any idea what “which need not be unsigned integers means”?

**Sam** [4:53](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=293s): Yeah I think that's supposed to allow using the title as the EIP number for draft eips.

**Justin Florentine** [5:04](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=304s): Got it. Thank you.

**Pooja Ranjan** [5:14](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=314s): I have noticed recently a ping going to user ABC for allocation of EIP number is that we are talking about?

**Sam** [5:30](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=330s): Oh in the PR, it says EIP editors and accounts authorised by any any EIP editor can decide numbers which need not be unsigned integers and I think that's specifically what Justin was asking about.

**Pooja Ranjan** [5:44](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=344s):  Got it.

**Gajinder** [5:45](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=345s):  But it doesn't make clear whether you know after a movement from the draft whether the EIP number  would still be. I mean any hex or any alphanumeric goes as far as ElP implementation goes. I mean they use the number to sort of signify that this particular hard Fork has this particular eips.

**Sam** [6:14](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=374s): I'll make a note of that in the PR.

**Pooja Ranjan** [6:27](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=387s):  Okay, 
so it looks like this PR 6976 requires some more edits and discussion and that could happen either on Discord or maybe on the pull request.  Well I think that is the major item for discussion today.

- EIP bot issuing numbers

**Pooja Ranjan** [6:50](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=410s):  The next one is also about the EIP bot issuing number. So what is the current status, Sam? is the bot active.

**Sam** [6:59](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=419s): Yeah, unless somebody's changed anything since it's reverted to an older version.

**Pooja Ranjan** [7:05](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=425s): All right.

## 2. Discussion continued from earlier meetings

**Pooja Ranjan** [7:14](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=434s): Okay. If there's nothing more to add on it we can probably move on to the item number two which is discussion continued from the earlier meetings. I have added only one issue here which was related to EIP. It looked like the date which is mentioned in the document is not correctly  reflecting on the website. Last date, so does panda need to maybe take a look at it or it's some bug, I'm not sure of that.

**Sam** [8:05](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=485s):  Was there an actual bug ?

**Pooja Ranjan** [8:10](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=490s):  I am not sure of this. The issue here is like the last call date that is mentioned. I have added the link here. The link is not correctly reflecting on eips.insight as eips.ethereum.org. I haven't seen this issue with any other proposal.

**Sam** [8:34](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=514s): Yeah that might be a GitHub Pages issue. I'm not sure.

**Pooja Ranjan** [8:45](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=525s): Yeah, okay and would you suggest that I create an issue in the eips repository. So someone can maybe take a look at it.

**Sam** [8:54](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=534s):  Yeah for
sure.

**Pooja Ranjan** [8:56](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=536s):  Okay I'll do that. it's like this particular proposal had an issue. Okay, I'll create an issue for that okay and that's it on the major side of it. 




## 3. EIPs Insight - Monthly EIPs status reporting.

**Pooja Ranjan** [9:17](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=557s):Since this is 3rd May, only we have three EIPs added as draft. One is informational EIP which is a Network upgrade activation trigger added by the number is 6953. It talks about all the upgrades and the activation block and time for those. There are two more erc's 6808 and 6809. one is a fungible key bound token and another one is a non-fungible keybound token. Okay there are two proposals moved to last call yesterday in the EIP editing office hour and that's pretty much all about.

**Pooja Ranjan** [10:03](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=603s): EIPs Insight we hope to add more insight as we go. Yeah, anyone else would like to discuss anything.  share talks about. Okay Victor has a proposal, please go ahead.

**Zainan Victor Zhou** [10:26](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=626s): Yeah so, hi this is Victor and since there's no more agenda item. I want to ask if there's any updates on our intention to build our work groups. So the context is set recently, I'm trying to work on a proposal that brings ERC authors and developers together in a regular meeting and would like to kind of basically gauge people's interests by their possible work groups and I do know that. I think Sam   is it you that in a big list of the reviewers you actually three people into work groups is that a good way to think of how work groups are divided and then is that a good way to kind of put people in the bracket in the future and actually we have a way of recognizing work groups in a more consistent way. I can follow the
way how you think  the work but just want to put it on the table on whether our EIP editors have thoughts and  kind of put out work groups categorizations in some way.

**Sam** [11:49](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=709s):  So I think work groups are or working groups or whatever you want to call them or are probably a good idea. It's just I don't think any of us have had time to organise them yet and I don't think we want to commit. The time for it  but if that's something you're interested in doing I think go for it. And if you want to use that big list of peer reviewers as a starting point, just to message people and see if they're interested in participating. I think that that would be great because the way I was doing it, like assigning a peer reviewer, didn't work very well.

**Zainan Victor Zhou** [12:24](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=744s): Yeah I understand. I think I am going to like to learn that and maybe the approach is to actually put people who happen to have capacity for a particular peer review.  Reviewing
at a certain time in the room and then have the author explain it to them, so that they can have some live explanation and back and forth discussion and then hopefully that trigger is more interesting in  the asynchronized on Forum discussion as well.

**Sam** [12:59](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=779s): Yeah yeah and there is the working group that I think it's and it has organised. Yeah so that one's that would probably be a good place to get started from.

**Zainan Victor Zhou** [13:11](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=791s): Right and also 4337 probably has its own work group that we can reach out to. Yeah sounds good, thanks I think I can start from there.

**Pooja Ranjan** [13:32](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=812s): For 4337, we have also connected it with Discord. The telegram working group has been connected to ethereum cat herders Discord. We have a channel dedicated for 4337 discussion so yeah you can probably reach out to people from there as well.

**Zainan Victor Zhou** [13:52](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=832s): Yeah and I'll just put the proposal here so that your editors could also be informed of this
proposal and make suggestions are very well content. We also look forward to your  participation if you're interested or have the capacity. It doesn't have to be a kind of long-term commitment; it can be sporadic and adhoc whenever you have time. Hopefully do this every two weeks and rotate the schedule so that it will be  friendly to Asia and friendly to Europe time zones in a rotating way. This is currently the plan but yeah I just put paste it in the text.

**Pooja Ranjan** [14:52](https://www.youtube.com/watch?v=QwQU9_Gi7GI&t=892s):  Anyone has got anything to share. All right this seems to be one of our shortest calls. Thank you everyone for joining us. I hope to see you in two weeks.
 
 ---------------------------------------
# Attendees

* Justin Florentine
* Gcolvin
* Pooja Ranjan
* Sam Wilson
* Light Client
* Jason Windawi
* Zainan Victor Zhou

## Date for Next Meeting: 17 May 2023 at 1400 UTC.


