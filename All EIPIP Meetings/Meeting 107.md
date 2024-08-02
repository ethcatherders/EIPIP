# EIPIP Meeting 107

**Meeting Date/Time: July 17, 2024 at 14:00 UTC**

**Meeting Duration: 34 mins**

**[Github Agenda](https://github.com/ethcatherders/EIPIP/issues/346)**

**[Audio/Video of the meeting:](https://www.youtube.com/watch?v=DgdzaxHWFcA)**

**Moderator: Pooja Ranjan**

**Notes: Aliyu Adeniji**

### Summary
| S No | Agenda | Summary |
| -------- | -------- | -------- |
| 107.1 | Discuss Open PRs and proposals | Final decisions on some isssues and proposals were taken,they include EIP, ERC, and RIP repos. |
| 107.2 | Other discussions and updates from past meetings | It was concluded that some EIP should be moved to RIP repository.
|  |   | Changes to EIP-152 and final proposal 152 were also accepted |
|  |  | It was discussed if PRs for which their authors are not present should be merged and it was concluded that call for input should be made so that other members of the community can contribute to the discussion and reach a final decision as soon as possible. |
|  |  | Discussion on security consideration and security disclosure in EIPs where only problems that lead to verifiable loss of funds should be added to the security considerations, and Sam mentioned that he will make a formal request for that. |
|  |  | Call for input on the proposal for the security consideration will give the proposal more visibility within the general community and not only among the editors only, Sam also said that he will open a formal call for input and inform the community within 30 days.  |
| 107.3 | EIPs Insight - Monthly EIPs status reporting | Pooja mentioned that she has added uo the total number of update on the number of EIP, ERC, and RIP issues and PRs which are 162 in number, and efforts are ongoing to keep them minimal as possible. |
|  |  | It is worth mentioning that there is a remaning proposal from the last call section which is the wallet call API deadline is 24th July. |
| 107.4 | EIP Editing Office Hour | Pooja said that she added the recording for meeting [40](https://youtu.be/gAtkU7YeSRU) and [41](https://github.com/ethcatherders/EIPIP/issues/347) Agenda for absent members, she also advised that memebers of the community should help in creating more awareness about the EIP editing hours holding every tuesday at 1400 UTC. |
| 107.5 |  Review action items from earlier meetings | There is a call for input for EIP-152 which was created in this meeting and frequency of meeting was decided to be once in every month. |
|  |  | Dex also asked pooja wants on getting more visibility for the program on various platforms and communties such as a telegram channel with about 57k members.|
|  |  | The next meeting is scheduled to hold on August 21st at 1400 UTC |



## 1. Discuss Open PRs and proposals

### Final decisions on some isssues and proposals taken

**Pooja** [0:00:](https://youtu.be/DgdzaxHWFcA?t=0) Welcome to EIPIP meeting 107 this is issue number 346 on ethcatherders EIPIP GitHub repository, on agenda we have some open issues and pull requests to be discussed, we'll take a look at some miscellaneous issues, as well as PRs, and we'll collect editor feedback, thoughts, whether we should keep it or close it,  we'll take a look at call for inputs added here and then discussions from earlier meetings I see there is a request for discussion that happened in the last meeting, we can hear about that and we'll get some updates on working group discussion that happened in the middle of the week.

#### https://github.com/ethereum/ERCs/pull/403

**Pooja** [0:47:](https://youtu.be/DgdzaxHWFcA?t=47) So starting from the very first item we do have a list of pull requests the first one is 1363 it seems that it has been already approved earlier but the author has added some new changes, I wonder what the editors think, is it good to be merged or do we want to get some more clarification from the author.

**Sam** [1:18:](https://youtu.be/DgdzaxHWFcA?t=78) This is editing a final proposal and I think it's editing it too much in my opinion.
 
**Pooja** [1:29:](https://youtu.be/DgdzaxHWFcA?t=159) Anyone else has any thoughts on that? Yeah I remember 1363 had a bunch of PRs for editing a final proposal. Okay let's try to get something on this one, just considering this open PR number 403, do we want to Merge it or do you want to give a push back, I don't know how significant the change they are trying to push here.

**Sam** [2:09:](https://youtu.be/DgdzaxHWFcA?t=141) It's not too bad but it is just changes in general. 

**Pooja** [2.25:](https://youtu.be/DgdzaxHWFcA?t=175) Matt Gajinder, is there any objection to merging on this one or do we want to not merge this and just close it.

**Matt Gajinder** [2.40:](https://youtu.be/DgdzaxHWFcA?t=160) I don't think we should merge it,  because it seems like there are already changes in the text. 

**Sam** [2:57:](https://youtu.be/DgdzaxHWFcA?t=177) All right I'll close the PR.

**Pooja** [3:02:](https://youtu.be/DgdzaxHWFcA?t=182) Right, moving on to the next item which is PR on ERC 342, it's updating ERC 2098, it seems like we have already received one input from RickMoore and seems okay for him, not sure he ever got a chance to get into it again, do we still want to wait for any more updates, we can perhaps give him another ping or anyone else from the ecosystem another ping to take a look if not, are we in a position to merge it?.

**LightClient** [4:02:](https://youtu.be/DgdzaxHWFcA?t=242)  I mean I think we need to verify that it's correct or someone needs to.

**Pooja** [4:10:](https://youtu.be/DgdzaxHWFcA?t=250) So we want to wait a little bit more on that.

**Sam** [4:20:](https://youtu.be/DgdzaxHWFcA?t=260) Well, I don't think it's a waiting thing, it's like somebody needs to tell us if this is correct or not. I mean he does have an example here that I'm trying to understand, it seems Richard is one of the authors and he says that at first look, it looks like they are correct.

**LightClient** [4:49:](https://youtu.be/DgdzaxHWFcA?t=289) I mean I guess we could plug this into.

**Sam** [4:52:](https://youtu.be/DgdzaxHWFcA?t=292) Cuts in; a signature Checker and see.

**LightClient** [4:55:](https://youtu.be/DgdzaxHWFcA?t=295) I mean it does have this solidity example, so if I could run this quickly, we could know.

**Sam** [5:10:](https://youtu.be/DgdzaxHWFcA?t=310) All right, we'll leave that to you to verify and get back to us.

**Pooja** [5:16:](https://youtu.be/DgdzaxHWFcA?t=316) Sounds good, Matt, whatever comment you have for that, please add it to this PR and we'll take it from there. Moving on, for some open issues and PRs there is an update to 1175,  it seems like it's not only for 1175, they have pinged a bunch of ER and ERCs so what do we want to do about it is I don't know if it is a potential spam I could not even go through the entire PR.

**Sam** [5:56:](https://youtu.be/DgdzaxHWFcA?t=356) No, it's correct, it's not spam it's just, because of how we built the system they have to be EIP, I'll make a comment and close it.

**Pooja** [6:10:](https://youtu.be/DgdzaxHWFcA?t=370) Okay, perfect, thank you so much. The next one is the update EIP 4788 PR number 8590, it seems that it has been approved by one and not many and we were waiting on matt’s comment here it, Matt I mean is there any way to change your mind or you are still on it and we need to close this because it seems we did not get any consensus on this one. 

**LightClient** [6:55:](https://youtu.be/DgdzaxHWFcA?t=415) I mean I think there's other final EIPs that have TBD in their fork, so I don't really see why we should update this here.

**Pooja** [7:08:](https://youtu.be/DgdzaxHWFcA?t=428) I'm not sure that was a field earlier, that is a new practice I guess that started from the past year or so.

**LightClient** [7:16:](https://youtu.be/DgdzaxHWFcA?t=436) I feel like that's been since 2016.

**Sam** [7:19:](https://youtu.be/DgdzaxHWFcA?t=439) Yeah like the earliest EIPs include a fork block and then later EIPs don't for exactly this reason I don't care if you want to like if you don't want us to merge this I'm okay just closing with.

**LightClient** [7:37:](https://youtu.be/DgdzaxHWFcA?t=457) I mean I guess I don't really care either.

**Pooja** [7:44:](https://youtu.be/DgdzaxHWFcA?t=464) Okay I think in that case we should add that because that is the right thing to do here and it's because it's a core proposal it will give I mean it will add value.

**Sam** [7:52:](https://youtu.be/DgdzaxHWFcA?t=472) It'll look better if we merge it yeah I'm if you're okay with it I'll merge it then Matt.

**LightClient** [7:53:](https://youtu.be/DgdzaxHWFcA?t=473) Yeah it's fine.

**Pooja** [8:05:](https://youtu.be/DgdzaxHWFcA?t=485) Very well the next one here is EIP 3712 multiple fungible token, it seems like this is a wrong repository for this PR we already have mentioned it to the author but author hasn't taken any step to move it to the ERC, how do we want to move about it, should we move like just move as merge or I just close the PR.

**Sam** [8:35:](https://youtu.be/DgdzaxHWFcA?t=515) So we want to move it because it's interface.

**Pooja** [8:40:](https://youtu.be/DgdzaxHWFcA?t=520) It's ERC on the EIP GitHub repository.

**Sam** [8:48:](https://youtu.be/DgdzaxHWFcA?t=528) No no I'm looking at it but it is not an ERC, it's an interface proposal, we're saying shouldn't be an interface proposal?.

**Pooja** [8:56:](https://youtu.be/DgdzaxHWFcA?t=536) No my bad, so I think I looked on the earlier version where it was mentioned as category ERC now I see an update on category interface, so this can be here because it is a core proposal

**LightClient** [9:10:](https://youtu.be/DgdzaxHWFcA?t=550) I just think it's still an interface and they saw that there was an error and we're like wow, we need to fix that but they didn't read the text that says the ERCs go to a different repo.

**Sam** [9:22:](https://youtu.be/DgdzaxHWFcA?t=562) Yeah this is definitely talking like it has solidity code in it so yeah this is definitely,  I'll close this and redirect them.

**Pooja** [9:33:](https://youtu.be/DgdzaxHWFcA?t=573) Yeah but we might want to consider that because so far we are still having interface category proposal on core, I mean like EIP GitHub repository so it will depend if they want to pursue this as an interface one then it has to.

**Sam** [9:53:](https://youtu.be/DgdzaxHWFcA?t=593) Yeah this is definite like it's a solidity contract this is a clearcut like this is not ERC.

**Pooja** [9:56:](https://youtu.be/DgdzaxHWFcA?t=596) Okay and the number suggest that this is pretty old one and yeah by now it should have received at least, category classification very well we can then perhaps close this one

**Sam** [10:08:](https://youtu.be/DgdzaxHWFcA?t=608) Yeah I'll take care of that.

**Pooja** [10:12:](https://youtu.be/DgdzaxHWFcA?t=612) Perfect uh there are a couple of more, and the first one here is an update to a stagnant proposal 1078 so stagnant definitely can be brought back to life if someone wants to and sees value in that proposal, I am not very sure though, with this pull request they are trying to do that or just fix typo and make a commit in the EIP repository so maybe editor can take a look the number is 540 and this is to fix two proposals 1078 and 1129, though we discussed earlier that we should not welcome any PR to stagnant proposal because um sorry it was for withdrawn yeah it was for withdrawn I guess we should not welcome any changes to withdrawn proposal we can definitely welcome for stagnant, okay any thoughts on merging both of these?

**Sam** [11:44:](https://youtu.be/DgdzaxHWFcA?t=704) I'm just looking through it,  yeah I'm okay with this it's fixing spelling mistakes. I'm just going to first Force merge this like it's not contentious, all right cool.

**Pooja** [12:15:](https://youtu.be/DgdzaxHWFcA?t=735) All right, the next one here seems like spam PR number 8734.

**Sam** [12:31:](https://youtu.be/DgdzaxHWFcA?t=751) Correct, yeah I'll close it .

## 2. Other discussions and updates from past meetings

### Conclusion on some EIP that were to be moved to RIP repository

**Pooja** [12:33:](https://youtu.be/DgdzaxHWFcA?t=753) Okay and the last one here is, PR 8724, it seems like it is not merging and it may require Force merge people try to open and close but it oh it's merged now, sorry my bad I don't know why it was showing to me still open or was it force merged right now, okay perfect, very well that covers all the open issues and PRs, we have few call for inputs the first one here is 343 which is to fix ERC 3448 okay with change, I don't know Matt if you have any thoughts you, would like to add the last date is still July 28 but it seems like two people, I mean two editors are already in favor of it so your vote will definitely make a difference here, we'll get three or more if you are in favor if not then we'll wait till the end of the deadline. The next one is issue 345 on EIPIP GitHub repository, this is to Mark EIP 7212 has moved because this proposal has moved into RIP repository and now we have RIP 7212 because we follow the same number system for all three repositories, it generally makes sense to me that we have only one number in one repository, and it could be moved the way we have moved the ERC proposals out of the EIP GitHub repository however, this this is open for core input, it seems like Sam is already in favor, and the author of the Proposal is also in favor. I have added a note from the last all core dev execution meeting where one of the RIP editors also shared the same interest of having a new proposal instead of continuing with the same name, but I think input from other editors may add value and we will be able to make decision on this pull request, anyone has any quick thought to add right over here? I want to take time and look into it Async.

**Sam** [15:08:](https://youtu.be/DgdzaxHWFcA?t=908) Sounds like it's going to be asynchronously.

**Gajinder**: [15:15:](https://youtu.be/DgdzaxHWFcA?t=915) Just delete it, we should just delete from the EIP repo.

**Pooja** 15:19:[](https://youtu.be/DgdzaxHWFcA?t=919) Yeah so all the ERCs were marked as moved and then we are not like counting it over there, so not marked as moved was it why do we mention it as an unusual status how did we deal with ERCs?

**Sam** [15:37:](https://youtu.be/DgdzaxHWFcA?t=937) No, they're not marked moved aren't they they're just no they're just hyperlink to the ERC's repo I mean it's not a status like this has been moved too, right  that's what you're referring to but it's not like a status for the EIP.

**Pooja** [16:04:](https://youtu.be/DgdzaxHWFcA?t=964) My preference would be to treat this as very much like ERC the way we have treated ERC and to not create any new and special status for this particular proposal if that makes sense. 

**Sam** [16:21:](https://youtu.be/DgdzaxHWFcA?t=981) Yes we do mark them as status moved, that might be me that did that but.

**LightClient** [16:35:](https://youtu.be/DgdzaxHWFcA?t=995) Okay that I didn't do that.

**Sam** [16:35:](https://youtu.be/DgdzaxHWFcA?t=995) Yeah I had to add  a little header to each one to get the bot to work again. 

**LightClient** [16:45:](https://youtu.be/DgdzaxHWFcA?t=1005) I see I still feel like we should just delete it.

**Sam** [16:50:](https://youtu.be/DgdzaxHWFcA?t=1010) Yeah I mean deleting it would be fine too I don't really care.

**Pooja** [16:59:](https://youtu.be/DgdzaxHWFcA?t=1019) I remember hearing about like breaking of EIPs inside when this Fork happened like when we moved everything from EIP github to ERC GitHub maybe because of this status moved I do not have clear recollection of that uh but if right now we are in a stage when we have a copy of all of these proposals everywhere unless we want to save the history, this can be deleted however we can definitely refer to older history by keeping it, but the status moved is not being reflected on like anywhere. 

**Matt Gajinder** [17:35:](https://youtu.be/DgdzaxHWFcA?t=1055) Older history will always be in the git repository, so that is not an issue.

**Pooja** [17:44:](https://youtu.be/DgdzaxHWFcA?t=1064) Okay so just to clarify it for notes taker, are we deciding on deleting all ERCs which has been marked as move and EIP which has been marked on move to the RIP repo?

**Sam** [18:01:](https://youtu.be/DgdzaxHWFcA?t=1081) I can try deleting everything and make sure it doesn't cause any problems and if it doesn't I'll open up PR

**LightClient**** [18:11:](https://youtu.be/DgdzaxHWFcA?t=1091) Cuts in, deleting the ERCs?

**Sam** [18:14:](https://youtu.be/DgdzaxHWFcA?t=1094) Deleting everything with status moved and RIP or EIP 7212 

**LightClient** [18:20:](https://youtu.be/DgdzaxHWFcA?t=1100) I mean I don't know if we should delete everything with status moved because there are a lot of like lingering hyperlinks to the Github   repos I mean that to me is the reason why that link is there and why it wasn't deleted in the first place. 

**Poojan** [18:40:](https://youtu.be/DgdzaxHWFcA?t=1120) Okay then, in that case for this PR, the resolution is that it can be marked as moved.

**Sam** [18:54:](https://youtu.be/DgdzaxHWFcA?t=1134) I think we're just going to delete this one yeah we'll delete this one and everything else stays as moved.

### Changes to EIP-152 and final proposal 152 are accepted

**Pooja** [19:00:](https://youtu.be/DgdzaxHWFcA?t=1140) Okay perfect, moving on the next one here is a call for input for merge update EIP-152, just to provide some background here there is a small update to a final proposal 152, it seems that author is not around to approve the pull request, however this has been already approved by editors as it seems like trivial change and people are generally fine, so I have created this call for input just today, sorry for the delay here, but the idea is to collect consensus on, can this be a process? 

### Discussion on whether PRs for which their authors are not present should be merged and call for input on final proposals

There are so many proposals for which authors are not around. Can we merge old requests, if editors are on board with merging the PRs in case authors are not around. We can definitely define a timeline that we want to keep the PR open for so everybody gets to see that proposal, and if needed create a call for input for even more eyes on it because I have just created it. I do not see many people have added their comment, I will definitely add but any editor here on the call if you have any thoughts on that.

**Sam** [20:25:](https://youtu.be/DgdzaxHWFcA?t=1225) So I'm against creating a general policy for this because I think that leads to like not potentials for abuse but it kind of limits in Us in how we can consider each proposal so for this one, I'm okay merging it because it's like a very trivial obvious change but for other changes to final proposals. I might not feel so confident merging it without an author approval so I don't think we should make a general policy, but I am in favor of merging this one proposal.

**Pooja** [21:01:](https://youtu.be/DgdzaxHWFcA?t=1261) Sounds good, yeah we can definitely take it case by case as it was mentioned earlier as well we'll try to bring up here and call for input if needed, but for this one people please add your thoughts and yeah we will take it from there, that's all about item number one moving on to the next item it is discussions from the earlier meeting, there was a meet to discuss about working group update I think Sam you would be the best person to maybe summarize that and say where we are on that.

**Sam** [21:44:](https://youtu.be/DgdzaxHWFcA?t=1304) Sure so I think the current plan is to abandon a formal approach to working groups so we will not be adding separate repositories for each working group we won't be  creating working group Charters or anything like that but some of the work I did will be used I'm going to open up Pull request to convert away from Jackal and switch to a different rendering engine called Zola and uh so that'll be a little bit different and then, we were also planning on introducing um a like formal recognition for non-editors who have PR approval rights, or permissions rather uh and we would call them probably EIP reviewers, and yeah so that that's kind of the approach we're having that would let us delegate some powers and enable people to make informal working groups uh with their own reviewers if they want to um yeah so I think that's that's kind of the plan moving forward. 

**Pooja** [22:48:](https://youtu.be/DgdzaxHWFcA?t=1368) Thank you for summarizing that I do not see Victor on the call I think he was one of the person very much interested in learning more about what is the decision on that I hope the some on the call will be able to help him and I don't know maybe um pull editors can uh find out some people who can be good reviewers maybe we can reach out to individual teams to volunteer people similarly for ERC group there is all ERC Dev meeting happening we can share this information in that meeting, and try to have some volunteers to be added as reviewers and I see there is a wallet Dev meeting plan today, maybe it can be mentioned over there to get some more reviewers for wallet proposals. I sincerely hope this will be helpful. Does anyone have any other thoughts to add to it?. 

### Discussion on security consideration and security disclosure in EIPs where only problems that lead to verifiable loss of funds should be added to the security considerations

Very well, the next item here is security consideration and security disclosure in EIPs,  we discussed some of it in the past meeting and Dex has added a detailed comment about what does he want to say here, what is his proposal and things like that so let me invite de to yeah share his thought and what do we want to get as a resolution from this particular meeting today hopefully to be there.

**Dex** [24:26:](https://youtu.be/DgdzaxHWFcA?t=1466) Yes so basically on the previous meeting I was requested to provide some links and here is my comment no discussion followed my comment so I'm here to bring it back again and in general I think that final means no change rule is simply wrong because it doesn't allow us to disclose security considerations and problems in final EIPs and this is the stage at which most of the problems will be discovered, because it is a normal life cycle of a software, most of the software has bug bounty programs for this, and I was proposing to make security considerations an exception from this Rule and modify the EIP-1 to make a new rule that if there is some verifiable loss of funds which can be verified through the blockchain history, then this can be added to the security considerations, we don't want to  focus on some small issues, our goal is to inform the implementers about the most critical stuff that they need to worry about and uh here is the proposal.

**Sam** [25:50:](https://youtu.be/DgdzaxHWFcA?t=1550) All right I will open a formal call for input, and we will get our thoughts out on them and we'll let you know in 30 days.

### Call for input on the proposal for the security consideration will give the proposal more visibility within the general community and not only among the editors only

**Pooja** [26:12:](https://youtu.be/DgdzaxHWFcA?t=1572) I think call for input will give this proposal even more visibility and we should try to collect thoughts not only from editors but also from the community. I think when the link is available we should share it on other social media as well if people want to chime in and share their thoughts, although, the decision made on call for inputs are basically from editors, but that would be good to see what is a general recommendation coming up from the community and if we would want to bring up any changes in future.

**Sam** [26:52:](https://youtu.be/DgdzaxHWFcA?t=1612) So just to make sure I understand your suggestion correctly here Dex, you wanted to make it so that you can modify everything or you can modify only the security consideration section only by appending to it and only if there is a financial loss, is that a reasonable resolution?. 

**Dex** [27:10:](https://youtu.be/DgdzaxHWFcA?t=1570) Only security consideration only append okay

**Sam** [27:13:](https://youtu.be/DgdzaxHWFcA?t=1633) I'll make a formal request for that.

**Dex** [27:18:](https://youtu.be/DgdzaxHWFcA?t=1638) Okay, I remember the comment regarding the controversial contracts, do I need to address it once again or we can just skip it?.

**Sam** [27:29:](https://youtu.be/DgdzaxHWFcA?t=1649) It's fine like once we decide how to handle security considerations, we'll apply the same rule to 223 as ERC-20.

**Dex** [27:39:](https://youtu.be/DgdzaxHWFcA?t=1659) Okay I want to follow this discussion and provide some maybe comments uh where can it be shared and followed Which social media?.

**Sam** [27:54:](https://youtu.be/DgdzaxHWFcA?t=1674) Yeah so it'll be in our EIP editor Discord Channel probably um or here on this call

**Dex** [28:01:](https://youtu.be/DgdzaxHWFcA?t=1681) Okay.

## 3. EIPs Insight - Monthly EIPs status reporting

### There is an update on the number of EIP, ERC, and RIP issues and PRs, and efforts are ongoing to keep them in reasonble numbers 

**Pooja** [28:07:](https://youtu.be/DgdzaxHWFcA?t=1687) Perfect thank you, moving on to the next item I have just added total number of issues and PR open numbers are reasonable, not blowing up absurdly, but yeah, we are in process of trying to decrease the number of open issues and pull request so we really appreciate any thought, feedbacks, and people who would want to add review comments that would help editors to may be able to close this pull request or merge these sooner rather than later, on EIPs insights I'm just taking a quick look at the website, and it seems like we have received three new draft proposal on EIP GitHub repository as well as five new proposal on EIP GitHub repository and three new draft on the ERC side.

### Wallet call API deadline is 24th July, and EIP editing hours every tuesday at 1400 UTC 

We have one proposal in the last call section that is an interface proposal 5792 wallet call Api and the deadline is 24th July, so if people have any thoughts comments with respect to wallet call Api proposal please make sure to add your comment on Fellowship of ethereum magician page, the discussion tool link page for this particular proposal, and it could be addressed by the authors for details, the link is added here on the agenda. 

## 4. EIP Editing Office Hour

### Recording for meeting [40](https://youtu.be/gAtkU7YeSRU) and [41](https://github.com/ethcatherders/EIPIP/issues/347) Agenda added for absent members

We did have EIP editing office hour, I have added the recording for meeting 40 and agenda for meeting 41 for people who aren't aware EIP editing office hour is 1 hour dedicated for EIP editing, and you can come up with your open pull request number, if you have any questions you did not understand the comment of reviewers or editors or you don't know what to do next I think this is the best place, even if you are someone who is trying to make their first pull request to create the first EIP for the ethereum ecosystem and you do not know the process this is the place for you to come, so if you are the one or you know someone who is looking for any help or support in documentation of proposal, moving a proposal from one status to another status, please let people know about EIP editing office hours, that happens every other Tuesday on 1400 UTC, and we always try to add agenda in advance so people can come and add their Pull request.

## 5. Review action items from earlier meetings

### Call for input for EIP-152 created in this meeting and frequency of meeting was decided

The next one is review action items from the earlier meetings, I think there was one open action item for call for input for EIP-152 that we have already created today, one last thing that we wanted to discuss was about the next meeting date and time I think Matt has already dropped but he was suggesting that we can decrease the frequency of EIPIP meeting, right now the Cadence is once in two week do we want to keep it the same or do we want to decrease and make it once a month? I wonder what editors thinks about it.

**Sam** [31:32:](https://youtu.be/DgdzaxHWFcA?t=1892) I'm okay with once a month.

**Matt Gajinder** [31:42:](https://youtu.be/DgdzaxHWFcA?t=1902) Yeah, same here.

###  Discuss on getting more visibility for the program on various platforms and communties.

**Pooja** [31:45:](https://youtu.be/DgdzaxHWFcA?t=1905) perfect in that case, we will try to create an agenda in advance and that would be for August 21st and we can keep it as a cadence just for people to easily remember on third Wednesday of a month, we will have the EIPIP meeting at 1400 UTC, is it generally good with people? okay perfect that brings us to the conclusion of items listed on the agenda. I wonder if anyone else has anything to share, add, or maybe propose for the next EIPIP meeting.

**Dex** [32:38:](https://youtu.be/DgdzaxHWFcA?t=1958) Just a side question, I've seen that you are publishing the records of these meetings on your YouTube channel but this doesn't have a lot of  reviews, do you want to attract some attention so I have some telegram channels like with 57k members and I have a Twitter account I'm found of, one of the ethereum classic teams I can share something on ethereum classic Discord is it a good idea or do you just want to keep it small and free from site Participants.

**Pooja** [33:15:](https://youtu.be/DgdzaxHWFcA?t=1995) I think it is always good to get the visibility the reason we organize this public call is we want people to get engaged, any support in creating awareness about EIPIP meeting or EIP editing office meeting will be highly appreciated, feel free to share the link and we will also try to start sharing this on Twitter and webcast so people know more about these kinds of meetings happening.

**Dex** [33:39:](https://youtu.be/DgdzaxHWFcA?t=2019) Okay got it, thank you.

**Pooja** [33:40:](https://youtu.be/DgdzaxHWFcA?t=2020) Thank you so much, anyone else has anything to share and propose very well thank you everyone for joining us today and I hope to see you all in the next call which is scheduled for August 21st at 1400 UTC, have a great rest of the day everyone.

**Sam** [34:15:](https://youtu.be/DgdzaxHWFcA?t=2055) Thanks Poojan, take care.

**Zarathustra** [34:20:](https://youtu.be/DgdzaxHWFcA?t=2060) Thank you everyone.

## Next Meeting Date/Time: August 21st, 2024 at 14:00 UTC


## Attendees

**Pooja Ranjan**

**Sam**

**Matt**

**Dex**

**Zarathusta**

**Kelvin King**

**Akash Kshirsagar**


