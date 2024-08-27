# EIPIP Meeting 108 Notes
### Meeting Date/Time: Aug 21, 2024 at 14:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethcatherders/EIPIP/issues/350)
### [Audio/Video of the meeting](https://youtu.be/IVKltkrRt6w)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
108.1 | **Disabling the stale bot**: @SamWilsn will create PRs to update the bot to continue providing warnings with edits to 6 months. Send a message to provide 1 week warning before closing
108.2 | **FORK_TIMESTAMP variable that is not specified for Dencun**: @SamWilsn will like to consider the PR
108.3 | **FORK_TIMESTAMP variable that is not specified for Dencun**: @poojaranjan will work with @djrtwo to get the PR up
108.4 | **Edit to Final Proposals**: @SamWilsn created this PR to fix a small typo
108.5 | **Call For Input**: This is the deadline. There are only two comments, one in favor and one in against. It would require more Editors comment to make a decision.
108.6 | **EIP Insight**: Add Network Upgrade to EIP page, Add charts to include against the timeline
108.7 | **EIP Insight**: @SamWilsn also recommended adding EIPsInsight website link to the EIPs Website.

**Pooja Ranjan**
* Welcome to EIPIP meeting 108. This is issue number is #350 on Eth Cat Herders GitHub repository. We have pretty light agenda today for discussion of some open issues and pull requests and other topics that may require editor's attention. We have one final proposal for edit. A few call for inputs.
* Most of them are closed, so we are just going to share the decision and only one open will take a look at EIPs insight.
* And yeah, that's pretty much about it. 
* If anyone has any other item that they would like to discuss today, perhaps you can add it on the agenda as a comment and we will add it as we go. 

# 1. Discuss Open Issues/PRs, and other topics [0.46](https://youtu.be/IVKltkrRt6w?t=46)
**Pooja Ranjan**
* So starting for the very first item it is discuss open issues and PRS and other topics. The first item listed here is disabling the stale bot. I think this comment was shared by Sam Wilson. So Sam, if you would like to provide some more context and yeah, let us know what is the ask here. 

**Sam**
* Sure, the stale bot has been closing issues that still need to be resolved. It closes pull requests before editors have a chance to look at them. I think overall it's just become more annoying than it is helpful. So I'd like to propose disabling it. If anybody has any thoughts on that 

**Lightclient**
* Well, the stale bot I would. Should we just make it longer 

**Sam**
* Yeah. 

**Pooja Ranjan**
* I mean I think initially it was planned for three months. Is it less than that or do we want to make it six months now? 

**Sam**
* I'd prefer if it was smarter, like it should just never close an issue or a pull request. Rather that's waiting for an editor because like, that's our problem, not the authors. So but if we want to keep it around, I don't feel super strongly about it. 

**Lightclient**
* So I just feel like, yeah, we should review pull requests faster and not let them get closed because they're stale. But also, if the author doesn't respond and say something on the pull request like this is not stale then are they going to respond to any changes that we like? Request.
* Because I do see a problem where we like request changes after a month or two and then they just never make oh yeah, that's absolutely a problem.
*  I think it would be nice if the bot knew like that had happened. And then the author is waiting. We're waiting on the author now. I just don't really know how to do that. 

**Sam**
* So EIP board, the thing that he made can do it, but it doesn't know how to close stale issues or anything like that. So maybe that's a feature we add, but how about we change it so that it warns you a week before closing and not two months before closing, and then it just closes it without warning? 

**Lightclient**
* Yeah, that would be great. 

**Sam**
* Okay. 

**Lightclient**
* So yeah, I'm also happy to make it a bit longer, I don't think. Yeah, I'll look into that, attached to the timing. I just think it's nice to have something that's churning through old stuff at some pace, because otherwise I think we'll just get like really old stuff that no one cares about anymore. 

**Sam**
* And all right, I'll take a look at changing that. Thanks 

**Pooja Ranjan**
* Thanks for the two action item or the two changes that we are looking with. This stale bot is one number one sending message one week before closing. And number two, it should not close the message pull request which is waiting on editors review only, which is waiting on authors review. Is that the correct understanding? 

**Sam**
* That would be ideal, but I think we're just going to change the times for now. 

**Pooja Ranjan**
* Okay. So we would be changing the time. Perfect 

**Lightclient**
* Speaking of stale things, when are we going to start calling stale EIP editors again? 

**Sam**
* I was waiting for the one year anniversary of the last time I did it. I think that's October 

**Lightclient**
* Okay. 

**Sam**
* I mean, we can do it now. I don't I don't care, I just don't want to propose it. If it's,  sooner than a year 

**Lightclient**
* Yeah. That's fine 

**Pooja Ranjan**
* And when are we getting there? I mean, I'm just curious, is it in a month or so or by the end of year 

**Pooja Ranjan**
* I think it was October. 

**Sam**
* I'll double check. 

**Pooja Ranjan**
* Okay. So it's nearby. Okay. That's pretty cool 

**Pooja Ranjan**
* Yeah, we should update it. We should keep it updated because it gives incorrect impression of like there are so many people working on it and still our work is not getting done. So let's get that updated very well. The next item here is fork timestamp variable that is not specified.
* I think it is proposed by smart programmer. He mentioned that EIP 1745, which is already merged, which is already finalized, and that also does not contain the fork timestamp.
* However there is no PR as per my information.
* Please let me know if there is already an existing PR and I missed to add here, but the request here is from the editors about the action that needs to be taken.
* Should we add the fork timestamp as there was a precedence Or how do we want to handle this proposal? 

**Sam**
* If somebody opens a pull request, I'm happy to call for input and merge it. We probably shouldn't have tbds in final proposals. 

**Pooja Ranjan**
* Okay, I will try to get in touch with him and maybe check with him if he's willing to do that. If not, then maybe I will make a PR and ask him to approve it if he's limited with his bandwidth or something like that. 

**Sam**
* That works. I mean, like, we don't even need to involve him. It just I don't want to make the PR. I'm lazy 

**Pooja Ranjan**
* Yeah, I can do that. Okay. We just need to take it from the last one. And yeah, I can perhaps make it cool. So the next one is added to Final Proposal. And this is PR number 8817, which I believe has been created by Sam Wilson itself.
* And it is a very small type of fix might require other editors approval before it can be merged. 

**Sam**
* Yeah. There's just an extra T in the name of an interface. So I just removed it 

**Pooja Ranjan**
* Matt, if you could maybe take a look at it and yeah, add your comment and I think it would require two editors approval. Would it? 

**Sam**
* It might even be three. I'm not sure. But yeah, it'll need. Yeah, yeah. 

**Pooja Ranjan**
* Because you have already created. So it may be counting you as one. So the other than Matt, there would be one more editors review required oh no, he is not adding you in the list because you have created it. Okay, so three more reviewers. That's right 
* Okay. So I will share this in the discord channel as well so people can take a look and we can perhaps close it because this is a very small fix 
* Moving forward we have call for input: 343,345 and 348. All of them have been closed and there's only one open. 349 I don't know, Sam, if you would like to make maybe take a few minutes and talk about all of them and share the results. And what is 

**Sam**
* Let me just pull that up  343, changing a comment in a reference implementation. we approved it. I merged the pull request 
* 345 was deleting EIP 7212 that one still requires,  editor approvals. So I'll put that in the chat here 
* Then we have 348 which was an update to EIP 152. What was the update for this one? Yeah, it was just adding some extra zeros.  I confirmed in solidity that the behavior is the same, and,  I was the only one who commented on it, so I merged it.  
* And then we have 349, which is daxton's.  allow appending to security considerations in final proposals that one is very contentious, I think.  but I believe I'm the only editor who's commented on it.
* So Gajendra has as well, and we're on opposite sides of the argument. So if anybody who's listening to this wants to come on and, leave a comment, I'd appreciate it. Thank you 

**Pooja Ranjan**
* Thank you for sharing.  yeah, it seems like they opened,  I mean, it is still open, but the deadline has already passed. So if someone can maybe add any input by the end of this week, that should be fine. 
* Otherwise we are gonna use the power of keeper of consensus and may be able to respond to the result 
* Very well the next section is pretty much empty over here. Like,  I don't I have not received any comment like what people would like to discuss here, maybe because we are meeting after quite some time. So 
* We will look into it later on, maybe moving forward. the next one is EIPs insight. So we are trying to follow this website to collect the information on EIPs insight. 
* However, these have also been updated right over here on our usual hackmd that we follow so people can find it at both places. 
* The idea is to provide real time data on EIPs and ERCs and RIPs. So as we take a look at here, we have five new proposals in draft from EIP and three on the ERCs side. Similarly for review, last call and everything. 
* When we get to know more about it, we can also find the deadline over right here. So this proposal is supposed to be ending the last call deadline on September 5th. People can, maybe take a look and add their feedback comments on it 
* They also provide a decent chart over here that suggests, like, okay, how many proposals we have received so far under which category and things like that 
* All these information are already added here. People can also find details of each of the proposal right here, but eventually we will move out of this hackmd style and we'll try to get the information real time from this website 
* There were a couple of other updates which were shared with me.  and we are hoping to, share it with the community so people may be able to make use of this. They created a spectra page which contains all the information right here, about all the proposals which are getting into spectra. 
* One thing that the team worked on was status timeline, saying, like, how long does it take to move from one status to another status? And we are trying to bring it for all the projects, all the EIPs that will give us a very good idea of how we are doing in terms of like responding to the pull request of authors or proposals. 
* I'm just taking, for example, something different here so we can get a full view of this so, for example, moving from draft to review, it took longer.
* And then because this is like one of the most popular proposal, and we understand it took a long time to get finally onto the main net. But this gives at least a good picture of how we are moving with this.
* I wonder if there are some other thoughts on how people want to see it, does it look good or do we want to add more?  you know parameters to it? 

**Sam**
* That's really cool. I really like that.  I don't have anything off the top of my head, but that's really neat. 

**Pooja Ranjan**
* Okay, one other thing that we are trying to do is like, just add the network upgrade category, and I hope that would be, done by the,  next week or so few other things that, was informed, I was informed that they have worked on, but I am not sure if this is working exactly the way it is expected.
* But let's quickly take a look at it. So for example here, this is about all the proposals reviewed by each of the 
editor. And I can perhaps demo it here that was shared with me. Okay. So what we are trying to do here is try to figure out like how many pull requests were created over a period of time so people can just enter their start date, end date, and we can, fetch the information right here.
So when we enter the date, it's suggest that how many pairs are created.
We also validated it by getting into the GitHub repository.
And it shares the exact same number. The ask here is like what kind of UI we are looking at? Is it okay to just put it across like that? Or maybe we can create a Google sheet which can be referred. 

**Sam**
* So they're looking for like how to visualize the information. 

**Pooja Ranjan**
* Yes 

**Sam**
* I mean like a bar chart would probably be fine or like, I don't know, maybe like a like a line chart that shows like, as of each month, the total number of EIPs reviewed by each author or each editor, maybe. I'm not sure. 

**Pooja Ranjan**
* I think part of it was done. This is like still a work in progress. Not very neat. so the EIP editor review is this one. Like here we can see since 2015, how many proposals have been reviewed by each of the editors is right here. Oh, yeah. 

**Sam**
* Yeah, I'm saying over. So take this chart and then put it over time 

**Pooja Ranjan**
* Yeah. Okay. That's very good suggestion. We can perhaps do that right now. What it does is like we can enter any individuals name here. And that will showcase, for example, if I put Oops. It's breaking. 

**Sam**
* Yeah, I had the same problem, but, uh. 

**Pooja Ranjan**
* But yeah, I will inform the team. Why is it breaking? Maybe they can take a look at it. Okay. Fair enough. So I think the suggestion here is that we should try to make it against time so people can visualize it, even better. 

**Sam**
* Yeah. Maybe not instead of maybe in addition to. But yeah. That's okay. Yeah. 

**Pooja Ranjan**
* Okay. Perfect. So the four, tasks that the team are working on, number one, adding network upgrade on the  EIP. 
* We worked on the date and we will work on the closed and open issues as well as the editors review thing. 
* I think that would help us to evaluate, like how many proposals are we able to actually attend to and do we need more reviewers? Obviously we need more reviewers, but how many reviewers should we get on board? It might help to get to that decision 
* Yeah, that's looking awesome. We should, put a link to this somewhere on the Eth website at some point. If there isn't one already, there isn't. But let's try to fix the issues first, and then I will ask the team. Yeah, okay Was to update it there. 
* Okay. that's pretty much about the Eth inside.  we had EIP editing office hour meeting 42 yesterday. 
* We reviewed 19 proposals. That was quite a lot to, like, look at in one hour. But,  it was a great achievement. Like,  we try to respond to people who had shown up for their questions and help merge their pull requests in the same meeting. If anyone listening to this call are planning to join the EIPIP editing office server, it happens every two weeks. 
* So two weeks from yesterday. there is another meeting at 1400 UTC. You can always leave your PR if you cannot attend the meeting as a comment, and we will try to address it in that meeting. Any question, any question related to a pull request, merge issues or documentation.
* Please join us over there and we hope that you are able to make your proposal move forward in different statuses 
* The last one here is action item from the last meeting on a high level, I am not sure if I find any open action item. Only one call for input. Open to collect input for decision making. Has it been closed 349 , you already did it. Okay, perfect. I think we covered pretty much everything that were listed on agenda today 
* Anyone has anything else to bring up for today? Or maybe for the next meeting 

**Sam**
* I'm good 

**Pooja Ranjan**
* Well thank you. That's great. Less issues, less,  problem. And better for the editors to continue doing what they are doing. 

**Sam**
* Yeah. Thanks for organizing everything, Pooja. Really appreciate it. 

**Pooja Ranjan**
* Thank you. It's my pleasure. And, thanks for all the effort and time that you guys are spending to support all these new contributors may be able to make their contribution to the Ethereum ecosystem. 
* Well, thank you all for joining us here today. I understand that we have agreed to keep this meeting only once a month, and that too on the third Wednesday of the month. So the next meeting is planned on September 18th at 1400 UTC. 
* If you have got anything to add to the agenda, please feel free to do so. I will add a new agenda item for the next meeting. Right after this meeting 
* Thank you everyone for joining us here today. Have a great one. 
---------

## Date and Time for the next meeting

Sep 18, 2024 at 14:00 UTC

---------
## Attendees

* Pooja Ranjan
* Sam
* Akash
* Lightclient



