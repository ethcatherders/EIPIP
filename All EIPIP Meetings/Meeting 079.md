# EIPIP Meeting 78 Notes
### Meeting Date/Time: Apr 19, 2023 at 14:00 UTC
### Meeting Duration: 33:04 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/226)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=7bRGFfSzo-k)
### Moderator: Pooja Ranjan
### Notes: Metago

## [Summary](https://github.com/ethereum-cat-herders/EIPIP/issues/226#issuecomment-1514878971)

Summary | Description
-|-
79.1 | Proposer will address the last comments added by the EIP editor
79.2 | PR-6840 - Generally, editors seem fine with the proposal. Someone can create a Pull Request to propose this change.
79.3 | dependency bot - @SamWilsn will create an Issue to indicate @Pandapip1 to reduce the notification pings.
79.4 | Allow BIPs as an external source. PR-#6897 - @xinbenlv will create a PR to edit it.
79.5 | EIP-3651, 3860, 3855, 4895 - Move to Final - We should wait for author's approval.
79.6 | EIP-5507 A bug - @SamWilsn will look into it.
79.7 | Yellow Paper - @SamWilsn will connect @xinbenlv with the right people to get the required permissions to maintain Yellow Paper.

## Introduction

**Pooja**
Welcome to EIPIP meeting 79. I have just shared agenda in chat. So we have a few open pull requests. One or two issues to be discussed. And there are a few suggestions left in comment. So I have tried to add them all here for discussion today. Thank you everyone for joining. 

## Discuss Open Issues/PRs, and other topics

### [Update EIP-1: Strengthen wording of status update PRs ethereum/EIPs#6894](https://github.com/ethereum/EIPs/pull/6894)

So the first pull request that is here is Update EIP 1, strengthening wording of status update. It is PR 6894. Looks like it is already approved by editors. Okay, I think there are some more comments left. Gajinder Singh, I think you are the last person to add some comments on that. Would you like to maybe talk about the changes that you are recommending here or is it just fine? 

**Gajinder**
Yeah, so I mean, those are minor comments, but just changing the wording. And one of the things I'm suggesting is that, so we use word free based instead of updated whenever to basically reflect the status of any EIP. To the different, to the different PRs that are still pending so that the commit on PR history, the commits look, still look good. 

**Pooja**
Alright, make sense. Maybe we will wait for the author to address that comment and then we can bring it back if needed. Or otherwise, I hope it will be merged before the next call. 

### [Stale last call deadlines ethereum/EIPs#6840]( https://github.com/ethereum/EIPs/issues/6840) 

Moving on, the next one is number is 6840. It's about stale last call deadlines. So a user has shared a list of proposals which have passed their deadline. And the question is what should we do about it? I see a comment from Sam Wilson suggesting that it should be there. And anyone can maybe create a new pull request to move it to the final status. But there is another proposal here. Perhaps a bot should move them back into review after six months. I'm wondering what other editors think about moving or changing the status back to review if not addressed for six months in last call. 

**lightclient**
It seems fine to me. 

**Pooja**
Okay, so I'm taking that the bot can move it back to review. But the question is like bot already moves it to stale right? 

**lightclient**
I'm not sure how it acts on the last call. 

**Pooja**
Okay, my understanding is I may be wrong, but as for my understanding, the present bot treats all of the EIP proposal or any of the pull requests in the repository, in the pull request form, move it to stagnant. And sometimes the status is changed to stagnant. So if someone wants to bring it back, it has to bring it back from stagnant to whatever the last status it was. So here the suggestion would be instead of moving it to stagnant status, it will be moved back to the review status. Are we okay with it? Are we still going to move it to stagnant irrespective of the present status of the EIP? 

**Gajinder**
Maybe after another three or four months, we can move it to stagnant. If nothing happens in review. 

**Pooja**
All right, that sounds good to me. Maybe we can look forward for a pull request for a specific change that is being suggested here. And we can take it from there. We are just joined by Sam as well so if I can quickly catch his thought as well before writing summary for this meeting…Sam, we were discussing issue number 6840, where Pandapip has suggested to move proposals from last call to review after six months past the deadline. 

**Sam**
Don't really have a problem with it. Rather neutral about it. 

**Pooja**
Yeah, that seems like a general understanding here. So as a summary, I'm going to mention that we can hope for a pull request to have this change updated by bot. Very well. 

### Dependency bot [05:42]( https://www.youtube.com/watch?v=7bRGFfSzo-k&list=PL4cwHXAawZxpLrRIkDlBjDUUrGgF91pQw&index=1&t=1696s) 

Moving on to the next one is a dependency bot. I think Matt mentioned this as a comment, assuming that he may want to look for some change. Matt, if you would like to give us an overview and what changes are expected here. 

**lightclient**
I just want a quieter bot. This thing is creating so many PRs. And it's just not really that important to be updating all these dependencies every time the author decides to push something to master. So I don't know what our bot situation was before. I don't know what the landscape of the bots look like, but I think that this renovate bot is too much. 

**Pooja**
I don't see Panda on the call wonder anyone else has any information about this bot. 

**Sam**
We can probably open a PR to make it do it less frequently. I don't think that would be an issue. 

**lightclient**
Or even if it batched the changes once a month or once every two weeks, that would be fine as well. It's just every time the author decides they want to push the master, we get another PR. 

**Pooja**
Okay. So looks like sorry, I was muted. Okay, it looks like the recommendation here is to update the dependency bot to kind of do the batch. Or only for status change, not for any other PR. Is that the correct understanding, Matt? 

**Sam**
This is for the like dependencies, not for EIPs. So it's like it'll make a PR to update it when somebody changes Jekyll, for example. 

**Pooja**
Oh, got it. 

**Sam**
I'll make a good issue to get Panda to configure it so that it does it once a week. It looks like we can do that. 

**lightclient**
Thanks. 

**Pooja**
Thank you. Moving on to the next one is allow BIP as external resources. I don't see Victor on the call. This was proposed by him. So probably we can take it later today. I hope he joins. 

### Update Proposals [07:57]( https://www.youtube.com/live/7bRGFfSzo-k?feature=share&t=477) 

I have added a few pull requests here. Those are two update proposals of Shanghai Shanghai upgrade proposal to move to the final status. I'm assuming at present they are waiting for authors to approve. But considering these proposals are already deployed and they are final, I wonder if editors can force merge them or we have to wait for authors to approve it. Alright, I'll ping authors on discord and we'll wait for them for another week or so. If not then we can reach out to editors. See if we can force merge them. 

Next one is a pull request number 6556. So I believe this pull request is for EIP 5507 that was merged yesterday during the EIP editing office hour. However, I do not see the status change on the eips.ethereum.org. I wonder if that is a bug. Yesterday there were two proposals which were merged. But I see this issue with only one. 

**Sam**
What was the issue again or the EIP?

**Pooja**
EIP number is 5507 that was moved to last call but that is not showing as is on eips.ethereum.org. It still shows as review status.  

**Sam**
I'll like into it. 

**Pooja**
Thank you. And that's all on discussion for like new topics. 

### Discussion continued from earlier meetings [10:24]( https://www.youtube.com/live/7bRGFfSzo-k?feature=share&t=624) 

Moving on to number two that is discussion continued from earlier meetings. Greg requested for yellow paper discussion. Greg you mentioned in the chat with some issue related to microphone. Is it okay? Are you able to hear us now? 

**Greg**
Victor’s not on the call so I don’t think it would be as useful to discuss it without him. He's been reaching out to people who have been contributing and just trying to see who's still interested in it. I'll probably bring it up in the next ACDE meeting, just find out if there's any interest in it and try and push it myself. I just think it would be a huge loss to the community….?

**Pooja**
All right. We can obviously bring it back in the next meeting when Victor is around. How it said that that's going to make our meeting the shortest one for today. Moving on to the item number three…

**Greg**
Yeah. I don't mind discussing it now. I just think it'll be more useful when Victor’s here. 

**Pooja**
So Matt if you have to you if you would like to share anything about it,it's fine. 

**lightclient**
Let's wait. Let's wait for Victor. I agree with Greg. I think that Victor should be here. 

**Pooja**
Not a problem. So we will bring it back in the next meeting if he does not join before we end up the call. 

### [EIPW bot Issues]( https://github.com/ethereum/eipw/issues) [12:13]( https://www.youtube.com/live/7bRGFfSzo-k?feature=share&t=733) 

So the next item is EIPW bot issues. I suppose there were some testing pending. Jose on the call, if you would like to provide any updates on that. 

**JA**
Hello. Yeah. Well, Sam is here. So I think that we are already done with the testing. I believe that we are almost there. Sam, maybe you can contribute or correct me. Thank you. 

**Sam**
This is for the like issue number five?

**JA**
For five. Yeah. 

**Sam**
I mean, we're this is your your PR. You know where we are on it. Yeah. 

**Pooja**
Okay. 

**Greg**
Victor’s here. 

**Pooja**
Yeah. Thank you, Victor for joining. We were waiting for you for two items that you have added here for discussion today. One is allow BIPs as external sources and, yellow paper. I think we are done with major sections only EIP’s Insight is left there on agenda. So if you would like to maybe talk about the BIP as external resources that was on the first item. 

### [Allow BIPs as external source. ethereum/EIPs#6897]( https://github.com/ethereum/EIPs/issues/6897) [13:41]( https://www.youtube.com/live/7bRGFfSzo-k?feature=share&t=821) 

**Victor**
Yeah. So I'd like to propose BIPs external source as allowed external source. I believe that when we talk about the link permission file when as Sam was drafting 5757, there was a specific…Sam was saying that external source needs to be stable for 10 years. I think that term was proposed. We were using EIP as one of the example for external. So I was under impression that the BIP was allowed. It turns out that the last EIP, EIP editing office hour author some author was proposing to refer to BIP. I believe it's BIP 39. And it was not allowed. 

I think it's reasonable that a lot of things in EIP was referring to some BIP. As early as the EIP one we have referring to BIP one. And also there is hierarchical deterministic wallets that was referring to BIP 32. So generally I think there's it's not harmful to refer to BIP. Its stable enough. And it's a legitimate list. So I like to propose it to be allowed as external source. 

**Sam**
I have no objections. I think it's reasonable. It's in a Git repository right? 

**Victor**
It is. Yeah. 

**Sam**
So I have no objections, unless anybody else objects? 

**lightclient**
I don’t object.

**Pooja**
Awesome. That was pretty quick. So I think we should be just expecting a full request to make that change in EIP one. 

### Yellow paper [15:42]( https://www.youtube.com/live/7bRGFfSzo-k?feature=share&t=942) 

The next item we were waiting was the discussion of yellow paper, Victor, I know that you were reaching, if you would like to share new updates on that?

**Greg**
Yeah. I know you were reaching out Victor. 

**Pooja**
Victor you may be muted if you're talking. 

**Victor**
So thanks to Tim Beiko and Greg who pointed out the last known maintainers of yellow paper and the people Andrew responded. Nick Saber has not responded. Andrew says that he to his best knowledge doesn't know anyone else other than him has continued to maintain the yellow paper after him. He himself loved to help, but he's having personal life commitment so that he will be happy if someone is interested in continue to maintain it. 

He will be happy to help review. Help get those people up to speed. And I'm still waiting for Nick Saber to respond. But my understanding is that one, EIP yellow paper is not being actively maintained, which is like obvious, and the second is that that people who from Tim Beiko and from other a few of other, a handful of other all core developers. They're interesting help out reviewing. And so this is the updates. 

And now this is the subjective part of my personal feeling. I think I am with Greg that having a mathematical way of representation out there as like yellow paper helps bridge the gap between the execution spec, which is the developer side. As with the research. Within the ethereum ecosystem and also within academia. So there's high value there. And I do understand there's a controversy for allowing linking to yellow paper at this current state. But I think it would be beneficial. I'm proposing to allow it to be linked today. But I think it would be good for us to look into how can we facilitating resuming of editing for yellow paper. 

My…that's my subjective feeling. And my proposed next step is to connect with the all core devs. And the any. And the consensus sync sync meeting. To see, to gouge the interest. For people who are currently developing in this space. For the core developer, whether they are interested, any volunteers who love to come over and either review or directly edit the yellow paper. And then we can start reviving it. We might need to get some help from the Ethereum Foundation to set up our Git repository permissions to start that conversation. 

I wonder. In that case, with who is the best person to talk to or should it be Pooja. Or who do we know is the best to kind of set up Git repository permissions to yellow paper. 

**Sam**
Who do you want to give permissions to? I mean, just talk to me, I guess we can figure it out. 

**Victor**
Oh, yeah. I think I can. Yeah, then we can continue the conversation. Basically, we want to have a few people who are interested helping out. And then we can start to propose permissions. Propose pull request. And then people who are committed to review them have the permission to review them. Actually a bot can help in that case so we can make it even more easier to add or review people who have the permission. Or if the bot is not available yet, you can, we can set them to just use GitHub roles in the first place. So yeah. Should it be you, Sam?

**Sam**
Yeah, we can talk offline. I can connect you with the right people. 

**Victor*8
Yeah. Okay. Yeah. That's. That's my. The updates. And then also my. I share my subjective feeling. Any feedback comments?

**Greg**
I think clearly that if we have the yellow paper going, whoever's taking responsibility for that, he needs to coordinate with the executable, the reference implementation and the EIPs. I would see the yellow paper as being at the very end of that process. I don't think that's a problem. And I don't think referring to it now is a problem. Most of it doesn’t change. Remains valid and referring to it is …concepts as normative…saw code now…executable…it’s a really difficult way to express this take…transition…stake…so that would just be my ask, that we can allow link to it now rather than wait out an uncertain process. 

**Victor**
I'll be in support of that. I know. I do know that Sam and Matt have strong concern about linking to it. Which is we try to discuss last time. And we believe that we are not bringing back this topic backup until certain time passed or things to significantly change because even though Greg, you and I really really think that yellow paper should be linkable. I think we have made a strong enough case to convince them. Yet. 

**Greg**
So I've got a couple proposals which are in withdrawn status but heavily depend on the yellow pages, are incomprehensible without it. Even though they are withdrawn, I want to do a little bit more work on them so that they are left in a correct consistent state simply as a published documentation of those concepts. And is the bot going to let me? Let me work on those? Or is it going to refuse to let me merge them back? 

**Sam**
Are they currently withdrawn or stagnant? 

**Greg**
They're currently withdrawn. Yeah. But. 

**Sam**
So they they are in the same place is final. So you won't be able to edit them. Regardless of whether there's yellow paper or not. But to be clear on this particular point, I think we should actually allow links to the yellow paper. I don't know if I've said that in a while. I think the yellow paper meets the criteria set out in 5757. 

**Greg**
So I basically should have left them stagnant. 

**Sam**
Yeah. Yeah, withdrawn rather than immutability like guarantees is final as far as I'm. 

**Greg**
Oh shit. Yeah, because I wanted them withdrawn to make clear that they were not being proposed. Given the EOF is there. I wanted to put the correct validation algorithm in. So that as a record of the final, the concept it would be correct. Okay. 

**Sam**
I mean, could open the PR and then we can talk about it. I think it's a good idea to make a right. 

**Greg**
Right. Right. It'll be some time before I have time. But essentially it's very and I translated the validation algorithm. I broke it. 

**Victor**
Well, same. Did I understand you correctly that in one particular case, you're allowing yellow paper to be linked? What is that particular case?

**Sam**
 I think the yellow paper is a valid origin of…like to link to according to the rules 5757…

**Victor**
Okay. 

**Sam**
So it should be allowed. 

**Victor**
Okay. I'm going to make a proposal to add EIPIP and I'm waiting for Matt has changed the position where or…

**Sam**
I don’t think Matt has changed his position.

**Victor**
Okay, then

**Sam**
There's a PR to allow the yellow paper already open. 

**Victor**
Okay. So then is Matt the only one who's currently opposing it or do we know other people stands? 

**Pooja**
Maybe we can like you know add comments on the pull request, which is already existing there. Right? So we can collect signal on that. If most of the editors approve it, it should go in right? 

**Sam**
It will, but I think we want to reach like consensus before we make any many changes like that. 

**Pooja**
Okay. It sounds like we have some way forward with respect to yellow paper as well as with respect to BIP external link. I mean BIP being added as a link in EIPs. Any other thing that you would like to mention or discuss today, Victor. 

**Victor**
That's all the topic I brought up I think. I don't have other topics I believe. 

**Pooja**
Anyone else would like to say anything before we move on to the next item?

Okay. Cool. I'm going to add summary after this call in the agenda itself. And I'm taking that Victor, you maybe looking into creating your pull request to add or update EIP one for external source. 

### EIP Insight [29:12]( https://www.youtube.com/live/7bRGFfSzo-k?feature=share&t=1752) 

Next one is EIP’s Insight…. status reporting. So far we have seven final EIPs in this month. There are seven proposals in last call including those four on the core side which we are hoping to get merged soon. And three other proposals which are in last call are going to meet deadline soon enough. 

Proposals are ERC 6220 which is 18th of April. It was yesterday so author can create new pull request to move it to the final status if there are no significant feedback from community or from editor on either on FEM or on the GitHub pull request itself. The next is ERC 6105 - no intermediary NFT trading protocol. The deadline was April 4th so author can anytime change it to the final status. Another ERC is 6381, deadline is May 2nd. Anyone having thoughts on this proposal getting into final, this is public non-fungible token remote repository. Please share your thoughts feedback as soon as possible before the deadline period is over so author can take a look.

And the last on the list is ERC 5507 refundable token. So this proposal is not showing the last on deadline on eips.ethereumm.org as of now. But the deadline is May 2nd. So if you are interested in this proposal and you have feedback comments starts to be shared with authors this is the time before it moves into final because we are discouraging people to make any changes after the proposal gets into final. So please take a look. And you can find this on HackMd added here in the link as well as the website added here. 

### EIP Editing Office Hour [31:18]( https://www.youtube.com/live/7bRGFfSzo-k?feature=share&t=1878) 

Next one is EIP editing office hour. I have added that recording for last meeting that happened yesterday, meeting 15 and agenda for meeting 16 is already up. If you have any pull request in the GitHub repository and you are not sure why it is not being merged, please reach out to us on please add a comment to the agenda and we will discuss it. 

You are also welcome to discuss the same before the meeting on Cat Herders discord. So please share your questions comments so that can be addressed as soon as possible. But if in any case it is not addressed till the meeting is there please join the meeting and editor Sam Wilson will help you out with the problem. Hopefully that will be resolved and your proposal will be merged. That's all from the agenda. 

Now quickly taking a look at this summary from the last meeting. Looks like we have already addressed all the issues from the last meeting. Yeah we do have some time if anyone has anything to bring up or discuss. Cool. Thank you everyone for joining us today. Hope to see you in two weeks. The meeting will be at 14:00 UTC. Have a great one everyone. Thank you. Bye. Thank you.


## Attendees
* Pooja Ranjan
* gcolvin
* JA
* Victor Zhou
* Jason Windawi
* Adam Egyed
* Gajinder
* Edson (dhedge)
* lightclient
* Combo (@1Combo)

