# EIPIP Meeting 104 Notes
### Meeting Date/Time: May 22, 2024 at 17:30 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethcatherders/EIPIP/issues/336)
### [Audio/Video of the meeting](https://youtu.be/4hHc9DMXxio)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
104.1 | **Should Proposed be a formal status?**: poojaranjan is hoping to have a discussion on the ACD meeting in future as it's specific to Core EIPs.
104.2 | **Update ERC-5585: ERC-721 NFT Authoriza… ethereum/ERCs#405** Merged
104.3 | **Update ERC-165: Clarify misleading usage of pure attribute ethereum/ERCs#283** Closed
104.4 | **Update ERC-4626: replace old repo link ethereum/ERCs#394** Closed
104.5 | **Update ERC-6672: Update erc-6672.md to fix author handle ethereum/ERCs#396** Closed
104.6 | **Update ERC-2135: fix some typos ethereum/ERCs#304** Merged
104.7 | **Update ERC-1077: Remove repetitive words ethereum/ERCs#395** Merged
104.8 | **Update EIP-1474: Update eip-1474.md Fixing the net_version usage example (adding a missed comma and deleting the excess ones)** Merged
104.9 | **Update EIP-1380: fix typo in EIP 1380 ethereum/EIPs#7961** Merged
104.10 | **Move to Withdrawn EIP** Update EIP-7623: Move to Withdrawn ethereum/EIPs#8530 - Requires author's approval. Will be on the bot to close if unresponded.

**Pooja Ranjan**
* Welcome to the Pip meeting 104 on agenda. We have some items to discuss and also maybe take a look into open issues, Pull request will take a look at call for input and some other discussions along with the EIPs insight of the month. And we'll also take a look into the open issues and PRs number as we are trying to keep a track of how well we are trying to maintain these things. 
* So starting with the first item, this is basically last minute additions to the agenda.

# Highlights for change in the EIP Process from Nyota Open Conversation [0.45](https://youtu.be/4hHc9DMXxio?t=45)
* The item here is highlights for change in the EIP process it's from Nyota Open Conversation, notes that has been shared today. So it seems like in the meetup there, the interop event client developers and, different teams joined together and they had some discussion on the EIP process, the current process, and the network upgrade process. 
* As per the notes. It seems like, the session was brainstorming. They discussed many points and also discussed certain statuses. So as for now, we know that CFI consider for inclusion is where proposals are included in the meta EIP and that is also considered for devnet. 
* So there is an alternate status. I don't know, because CFI is not a formal status, but they are proposing something this like should proposed be a formal status for EIPs? I wonder if editors have any thought on this? 

**Sam**
* Well, so I don't have a problem including like proposed for a certain fork or something as a tag on the EIP, but I think it should be separate from the status because the status is really about the document itself. but that's just me, I don't know. 

**Gajinder**
* Yeah. I mean, it could be part of status as well, but yeah, I don't have any strong opinions on the same. 

**Pooja Ranjan**
* Yeah. I mean, I would be, inclining towards Sam because we are trying to keep the status uniform, more or less. It is working. So far, so good. So it would be nice to keep, using tag instead of status. 
* And. Yeah, obviously this is something that has to be decided by client team. So I'm hoping that there would be a discussion in the all core dev meeting. Not sure if it would be tomorrow because we 
* Have an ACDE meeting there, but it's good to, yeah, collect thoughts from editors. So yeah, that was one thing. The next thing was like, the improvement process. So, there the perception that was discussed in the meeting was like, EIPIP has gone on forever, and it's not clear what the use of this. There was a potential idea to consider a different approach to implement process change going forward, in my personal opinion.
* Like when we talk about EIP it cannot be stopped at any point of time because process improvement is something that is essential and it will go on forever because that's how we will continue to improve processes, process improvement. in continuation, however, if there are different approach to implement these process and process change and come up with an alternate idea to EIPIP.
* Would be really happy to be a part of that as well. But I wonder if the present, group of editors have some thoughts on that, or maybe some suggestions around how we can perhaps improve this meeting, or maybe a part of any other meeting that is being proposed by the client. Dev. 

**Sam**
* I mean, all core devs has been going on for years and, I don't see an end for that. Maybe we should consider alternate ways of governing Ethereum as well.  I mean, obviously we need to continue having this meeting, just to deal with the issues as they come up. I don't know if we need to call it EIPIP but I like having a call every so often where I can talk to the other editors. so I'm in favor of keeping the call. 

**Gajinder**
* Yeah, I concur. I mean, you can call it whatever name you want. but essentially there will be a meeting or a call where we will basically come and talk about the outstanding issues. 

**Zainan Victor Zhou**
* Likewise, I am in favor of, keeping the call. if we want to change the time or change the cadence, I'm totally fine. Uh fine. And look forward to it. but I just like what Sam says. I love to be able to meet, a, meet with editors every once in a while. 

**Pooja Ranjan**
* I mean, it's highly encouraging to see all editors having almost similar views to keep this meeting. I also believe that this EIPIP meeting provides us an opportunity to discuss things which otherwise could not be discussed in all core dev meeting, because all core dev agenda is already full most of the time, and the initial idea of having this EIP discussion, the process discussion separate from all core dev meeting was to provide them enough time frame to, you know, decided discuss it and maybe implement it, whatever is the best way.
* And it will also provide an opportunity to community to participate. I'm also happy and excited with the new process that is there, these days, suggested by Sam to, like, discuss proposals and provide them for a month's time, call for input that we are doing 
* For tackling corner cases. So I am also in very much favor of keeping this meetings. But what I would encourage is like, you know, core devs, they be a part of this meeting if they have some question concerns and if they want certain processes to be changed because this meeting will give an hour long time for them 

**Gajinder**
* Outstanding issues by coders that we haven't addressed? 

**Pooja Ranjan**
* I'm not very sure. I'm hoping that, whatever, they have discussed in the Nyota conference, as per the report, it seems like Tim would be looking into the issues and they would like to come up with a formalized next step for this process improvement kind of thing. So I'm hoping to have some discussion with him. And maybe in all core dev meeting, it will be discussed, so we can get some clarity. But that's a very good question. If there is any open issue that we haven't addressed, we should highly consider that including.
* And there were certain suggestions around network upgrade process. I have shared the link of the proposed process. It seems interesting to me. I'm not sure how it's going to be implemented, but it would be. Yeah. Good to follow, what developers think in this direction. It's a very beautiful PNG here. People may check out the, agenda. 

**Sam**
* Cool. I'll take a look. 

# Update ERC-165: Clarify misleading usage of pure attribute ethereum/ERCs#283 [8:32](https://youtu.be/4hHc9DMXxio?t=512)
**Pooja Ranjan**
* Thank you. Moving forward, we have a bunch of edits, for final proposals. These proposals are already in final statuses, although people are not encouraging these kind of edits. But sometimes we receive it. Sometimes there is a general consensus of merging them, but many times it is not considered. I see that out of five, two are already being addressed. So we can perhaps start with the issues or the pull requests which haven't been addressed. The first one is for ERC 283. It is for ERC 165. What do people think here? 

**Sam**
* Yes, this is an update to some wording in 165 around the use of the peer keyword. I don't think we should make this change. but I'm happy to be overruled. 

**Pooja Ranjan**
* Sam beat me to it. Yeah. Victor, the link is shared in the chat here. Anyone in favor of merging this one? 

**Zainan Victor Zhou**
* I am not in favor. This is the finalized one already, right? This is 165. So, it's not a strong. There's nothing that I see as definitely need to update. I don't see that, helpful. Not in favor. 

**Pooja Ranjan**
* Cool. For certain proposals. Which for which, editors are not in favor, it may be a good idea to maybe add a comment and close that, because that will help us reducing the issues and pull requests, open issues and pull requests. So how do we want to go forward with that? Like, do we want to wait for a certain period? 

**Sam**
* I got a note on it. 

**Pooja Ranjan**
* Okay, perfect. Sam, just curious. Like, after you made a note on that, do we still want to wait for one week to see if anyone, like any of the other editors, shows up and say, no, I really want to merge this one because we don't have all the editors on call here. 

**Sam**
* I don't think so. We have enough people here that I think the general consensus of if we did like a call for input would be clear. 

# Update ERC-4626: replace old repo link ethereum/ERCs#394 [10:43](https://youtu.be/4hHc9DMXxio?t=643)
**Pooja Ranjan**
* Very well. Similarly, there is another one which is ERC 394. It is again to replace old repo link for a final proposal, IRC 4626. It seems like it is proposed by the team itself I mean, I don't find the name in the authors list, but I was surprised to see for Bulu, I don't know, I can't spell his name correctly. I'm Sorry about that. approve this change. Yeah. 

**Sam**
* Which one was this? 394

**Pooja Ranjan**
* That's right. 

**Sam**
* The link is broken. It's fine. I'll just leave it be broken is my opinion. 

**Pooja Ranjan**
* Okay? So do we want to close this one as well 

**Pooja Ranjan**
* And like it will be interesting to see how that was approved in the first place because we don't allow external link. 

**Sam**
* Yeah. This would have been before. if makes sense. 

**Pooja Ranjan**
* Do we allow like I mean, I think going forward we should not allow reference link to the third project. Right. It was coming up from Rari Capital and they are trying to just update it for transmissions 11. I guess they have renamed their project name there. 

**Sam**
* Yeah, exactly. I mean, this whole discussion came up with ERC 20 as well there were links to I think it was consensus implementation and Openzeppelin implementation of ERC 20, and people felt like it gave their implementations an unfair advantage to be linked to directly from the EIP. and I think that would also be true here. yeah. So I think we should just leave it broken and, not change it 

**Pooja Ranjan**
* Yeah, that is a fair point. We do not want to promote any project. 

**Zainan Victor Zhou**
* For the record, I sorry, Sam. Go ahead. Didn't mean to interrupt you. 

**Sam**
* No, I was going to say we just can't copy it in because it's GP. 

**Zainan Victor Zhou**
* Okay. So for the record, I vote against. Because this is a final, I didn't, share the view that we shouldn't point to people's preference limitation, and that'll be a longer conversation. But, yeah, I concur the decision with a different reason 

**Pooja Ranjan**
* Very well. At least we have a decision to close this one, and then we will take the other one, maybe some other day. So maybe we can just add a comment and close this one as well. the next one here is a 

# Update ERC-2135: fix some typos ethereum/ERCs#304 [13:53](https://youtu.be/4hHc9DMXxio?t=833)
**Pooja Ranjan**
* ERC 304. It seems like everything is done there, but it is still not merged. May require force merging. 

**Zainan Victor Zhou**
* And sharing since they're trying to edit multiple ERC at once 

**Sam**
* Yeah, they just don't have all of the approvals they need. we need what? One more ERC editor. And I guess one author for this to merge. I'm okay forced merging this if you guys are, like, they're just typos. 

**Zainan Victor Zhou**
* I'm fine. I think these are typos. And if they are drafts, fixing them is good. 

**Gajinder**
* I'm good with it. 

**Pooja Ranjan**
* Cool. That covers it. And, the next section is about stagnant proposal. So stagnant as we know, those proposals are not being actively pursued by the author. However, intermittently, we are receiving some edits. Either those are typo edits or making some small changes to the proposals.
* So I have collected some of the PRS, to fix or typo or remove repetitive words kind of thing. We can perhaps take a look at that, and maybe we can try to define this thing. Should we entertain a proposal? pull request for stagnant proposal If they really want to update the proposal or want to pursue the proposal, they should move it out of the stagnant status to draft, to review or whatever a status. Yeah. The first one here is ERC 395. 

# Update ERC-1077: Remove repetitive words ethereum/ERCs#395 [15:46](https://youtu.be/4hHc9DMXxio?t=946)
**Sam**
* This is a non author updating it. Yeah okay I mean yes. Yeah I don't care if they're fixing typos I mean I'd rather the typos be fixed than not fixed. It looks better on on the EIP website but I don't really care that strongly. 

**Pooja Ranjan**
* Yeah I mean I agree to that part. But when proposals are in stagnant status, most likely it is not visited by anybody because they understand it is not being like pursued 

**Gajinder**
* I mean, I would not want to entertain so that we can just reduce the PR load that we have. Other than that, it doesn't matter. 

**Sam**
* Sure. Okay. So, we'll just do we want to close it or do you want to just let it stale out 

**Sam**
* I guess. 

**Gajinder**
* I mean, we should close it because, again, we should not let open PRS pile up. 

**Sam**
* Sure. Okay. 

**Gajinder**
* Are you good? Am I just, the point is that, they shouldn't consume any of anybody's attentions since, the status is already in. Withdrawn. 

**Pooja Ranjan**
* Yeah. I mean, I'm just wondering if, like, for these, like, there are these are three numbers. Not big deal. We can perhaps merge or close or whatever it is, but we do not want to entertain certain pull requests should should be the message that I think if we can communicate it to people would be nice. Same goes with withdrawn.
* So if people want to work on the proposal, bring it back from the stagnant status, keep it in active status and when it is withdrawn that then we know that it is already been withdrawn.
* There would not be any further changes to it. So there is no point making typo or error or anything like that. 

**Gajinder**
* I think we should take the path of least resistance. Explaining it to people is even bit, you know, putting it more effort. So in that case I will just accept it 

**Pooja Ranjan**
* No, I think adding one line on EIP one, along with the status where we are explaining these statuses, we can just add one line like, whether we encourage, or whether we discourage or encourage pull request. 

**Gajinder**
* And this unless the board itself, does not allow one to make a PR. Yeah. then I think it is possible that we can basically have it in the EIP-1. And, but if the board is allowing to make PR, then somebody has to look at it at least and see what, what is happening.
* So it basically takes away the cognitive load that I wouldn't want, if I'm checking a proposal or if any of the other authors are checking the proposal. But, if it for example, if we have to explain it to the contributing members and sort of write it, then it's easier to just accept it.
* So I mean, whatever is the best or whatever is the least resistance path is what we should just take it, because having the type of anyway is a good thing. so if someone feels that okay, they can just approve it, then it's good to go. 

**Pooja Ranjan**
* That's an interesting point, Sam. do we think that EPW bot can maybe check the status and, maybe leave a message? 

**Sam**
* So EPW doesn't really consider status changes. so not really. No EIP review bot like the the one that PandaPip worked on would be able to do it. but I'm not super familiar with that code. 

**Pooja Ranjan**
* Is that still working? Like, are we using a preview bot for our presenting? I think so, yep. Yeah. All right. Maybe we can, put it out as an issue and, look for some contributors who are willing to look into issues and may be able to help us there. 

**Gajinder**
* So basically our merge bot could just review it and auto close the PR. 

**Pooja Ranjan**
* That would be the best. 

**Sam**
* Yeah, we can it can definitely do that. yeah. It's just I'm not super confident in my ability to edit that bot 

**Pooja Ranjan**
* But someone maybe, maybe create an issue there. Then I can, like, pass that issue to a group of people who are willing to look into, ways to support EIP editing process. Yeah. If if someone can just document it and just put it as an issue, I'll be taking it forward 

**Pooja Ranjan**
* Thank you. All right. for the these three proposals now, like, are we fine merging them or do we want to, like, say no right away? What are we doing with these if if everybody is okay with me just merging typo fixes, I'll just merge typo fixes. 
* Cool. Anyway, we have not given them enough. I have no objection. Yeah, we have not given them enough time to say no. So let's merge this one. Thank you. Sam 

# Update EIP-7623: Move to Withdrawn ethereum/EIPs#8530 [21:59](https://youtu.be/4hHc9DMXxio?t=1319)
**Pooja Ranjan**
* All right, so there is this one proposal 7623, which is, proposed here to be moved to withdrawn. I notice, it, like it is done, like they have done everything, but I don't see this is merged. I wonder if requires editors approval or what is blocking this PR. 

**Gajinder**
* I think because the proposal is not the author. 

**Pooja Ranjan**
* 763 is not the author. Oh. All right. And I mean, this is available, EIP I mean, I think as far as I understand that this is a viable EIP. 

**Gajinder**
* So this person is might just be, I don't know, doing EIP sniping or whatever 

**Pooja Ranjan**
* He is an author for sure. I know he is an active contributor as well. So may not be that case. perhaps we should add comment that this seems to be viable, and if you really want to move it to withdrawn, we might want to get consent from the original authors. It may be possible that there there may have been some discussion around the internally. Yeah. 

**Sam**
* So EIP bot or if bot has tagged the correct people and if they want to merge this they can approve the PR. 

**Pooja Ranjan**
* I'm trying to remember like what is our current period. Is it three months or six months for moving into stale or stagnant? 

**Sam**
* I think it's, two weeks for the warning and then six months after that. But. Yeah. Oh, you mean to sorry to go into stagnant or to go into, to close the PR, close the PR, so, yeah, PRS is like six months or something like that. 

**Pooja Ranjan**
* Yeah. Then this would be like increasing the number without any reason for very long period of time, like the if authors do not respond to them in next two weeks or three weeks, it is clear they are not willing to move this proposal to withdrawn. In that case, there's no point keeping this on active will increase the number. 

**Sam**
* Yep. so my partner Nicky has been working on a little tool that should make this a bit easier. They have, they're working on, like, a dashboard that displays the pull requests to be reviewed, and it filters out ones that, editors don't need to look at. So it should make it a little bit easier to ignore these. 

**Pooja Ranjan**
* I think it will make it a lot easier. Not a little bit, especially for editors. Thanks. Very well. So I think, just for summary purpose, we are leaving it as is, and we'll be waiting for original authors response to this pull request. Ideally by bot. It will be closed in next six months, but if we can get back to it sooner to get it closed will be nicer to have.
* And I have listed a few issues and, peers. I'm not sure if they are actually spam, but they seem like spam. The first one is issue 425 from IRC 425. 

**Sam**
* That one was definitely spam. I deleted that one already. The other two are real. 

**Pooja Ranjan**
* Yeah, okay, they are real. Then I would remove them. So, like it comes along with a pull request, but there was no request number mentioned so I could not get that. 
* Okay. Author. Yes, I think there is another question. We can perhaps help them, but it would require original authors support to the proposal. Very well. So I will just remove these two. Next is call for input. It seems like we have closed all the call for inputs. 
* Last three call for inputs from the earlier meetings and kind of added result. Sam, if you would want to add anything on top of that because I don't see anything new here. 

**Sam**
* Sure. there were a few author name updates that I merged I closed Gajendra's, policy on typo correction PRs just because there wasn't anything clear there. feel free to reopen it if you want to talk some more about it. yeah, that's about it 

**Pooja Ranjan**
* It was kind of quiet past couple of weeks. So we don't have new, call for inputs, which is a good thing to have. We want to go it smoothly only for, like, very difficult situation. Call for inputs. Should be there. 
* Moving on to the next agenda item. we don't have many things new. just the first one here is like create how to how to create a more inclusive environment to increase community participation for upcoming proposals.
* So recently, Ethereum cat herders, started this protocol study group in which we are talking to a group of new contributors and assigning them some issues which are already existing in different Ethereum repositories. 
* As for now, because I'm more familiar with the issues which are on EP, ERC and RIP repository, we are trying to make use of that.  I understand that most of them could be new. 
* May not be able to review these proposals right away, but they could be useful and helpful in terms of updating our bots. So we have collected a few issues from EIP bots, and some of the, contributors are working on that. I hope to see this, experiment going good in future and we receive more community participation, more volunteers to maybe take a look into the proposals or issues there. 
* So, this will encourage them to make a open source contribution and maybe just test the water of Ethereum ecosystem in general. If people have any thoughts, suggestions on this initiative, or may want to recommend anyone to this one, please feel free to share your thoughts here. 
* And I also want to mention, I also want to shout out to Sam, who has been actively supporting, this initiative. Like because this is EIP related issues. So there are many questions. Not many people are familiar with how our bot works initially. So Sam is trying to take our time to explain the process and kind of help them get those issues done. 

**Sam**
* Happy to help. 

**Pooja Ranjan**
* Very well. we will continue to collect thoughts and feedbacks on that. People can reach out to me even on discord and DM me. I'm open to the ideas and suggestions there to encourage more community contributors here. 
* The next one is web page rendering to include EIP, ERC, RIP is there is a long pending, pull request to kind of provide the boilerplate to RIP. So that hasn't been merged. And so far we have not received any editor on EIP meeting. So we didn't get an opportunity to discuss how do we want to, like take those things forward. 
* So that's kind of a blocker there right now. The eip.ethereum.org is very well representing EIP and ERCs. I wonder if there is any updates on the charter side that you would like to share? 

**Sam**
no, I haven't been working on it. 

**Pooja Ranjan**
* All right. at least we have EIP and ERC is being rendered on one of their website, which is working absolutely fine. I hope RIP's, team approve them. the pull request, or may adjust their repository in a way that we would be in a position to retrieve the proposals from there and be able to add it. 
* Till then, this is it. All right. that's, about, the other discussion. next section here is EIPs insights. So I have added this, list Of open not list of count of open issues and pull requests and small dashboard which is added to the EIPs insight Hackmd file. If we take a look at it, we are trying to improve the numbers like get it to lower.
* However, we see that, since January this tracker is tracking it since January 2024. 
* In January, for EIPS, we were around 100, including issues and pull requests, but right now it is around 69. So definitely a progress there. that hasn't been that good with ERCs. We started with 76 and we are at 97, but I understand we receive more proposal on application side than we receive it on the core side. 
* And for core side, we know that if one proposal is superseded or like the idea is, overtaken by another better proposal, people generally try to withdraw that. So the number keeps decreasing 

* We would definitely like to bring the number down of open issues and pull requests, even on the ERC side. On EIP repository, we started with just two one issue and one PR. Currently we are at 11. this is increasing because this is a new repository we should be expecting more, proposals for roll up, projects. 
* And yeah, right now we have only one issues and ten PRs. We hope to see these PRs getting merged or closed eventually. So that's on the dashboard. And we continue. We will continue to keep a track of that. That is kind of our performance report how we are doing in managing these issues and addressing them on time on EIPs insight. I think we have, what, ten new drafts added? 
* out of those ten, nine are EIP and one ERC. Oh wow. Seven move to stagnant and one proposal to withdrawn. Pretty basic information. I have added link to both EIPs insight and Hackmd to maybe take a look at the different charts and the dashboards that we are maintaining Anyone has any questions? Thoughts?

**Sam**
* That's awesome. Thank you for keeping track of all that pressure. 

**Pooja Ranjan**
* Thanks to the team. I'm sorry, Victor, when you mentioned link, I think I missed the chat. Is it related to the that's that's long gone. 

**Zainan Victor Zhou**
* Yeah. No worries. thank you for the great effort. we should give community more visibility to these great effort that you have. Keep track and everything. Yeah. We're not doing, the the same level of, visibility than it should. It deserves. We should we should give them more visibility. 

**Pooja Ranjan**
* Appreciate the kind words here. Thank you so much. The next one is EIP editing office hour. We could not have office hour last week but we hope to have it at the next week. so we have added the agenda here, because we could not have it. 
* There are already 8 PRs merged. like before the next meeting, when editors get time, they try to take a look into the pull request, which are already listed in the agenda and out of the peers added there for review.
*  Some of them are closed. So we hope to get more, PRS, merge reviewed in the next meeting. 
* If you have any open pull requests or any questions around how EIPs are merged or ERCs are merged or around process, please join our editing office. 
* Our, we hope to respond to all the questions you may have. And, yeah, I think that's kind of end of the meeting. I'm quickly taking a look at the, summary section. If there were any open action item, it doesn't look like that. 
* So, yeah I think we are pretty much done for the agenda of today. anyone would like to add, discuss or mention anything? 

**Sam**
* I'm good. 

**Zainan Victor Zhou**
* I'm good too. but yeah. Sam and and gajendar. Uh 

**Zainan Victor Zhou**
* I want to kind of book time with you guys each individually just to grab a virtual coffee. I think we work, but we didn't get enough to socialize as well. I just want to, like, get to learn you about you. And, of course, we meet multiple times. But, yeah, getting to know you guys from a personal level. not just as a GitHub handle, is great. 

**Sam**
* Sure. Yeah. Just, I'm busy for, like, the next 14 days, but after that, feel free to send me an invite. 

**Zainan Victor Zhou**
* Yeah, I will send you my calendar. And you can pick or reschedule however you want. And gajendar too 

**Gajinder**
* Yeah, we we you will be coming to Devcon. Right. So we'll part there. 

**Zainan Victor Zhou**
* I yeah, I think 90%. I'm going to Devcon. yes. 

**Pooja Ranjan**
* Sounds good. Awesome. Well, thank you everyone for joining us today. Hope to see you around 

**Pooja Ranjan**
* Closing pull requests and addressing issues and answering questions. Have a great rest of the day everyone. 

**Sam**
* You too. Thank you. 

**Zainan Victor Zhou**
* Thank you everyone.


---------

## Date and Time for the next meeting

June 05, 2024 at 17:30 UTC


---------
## Attendees

* Pooja Ranjan
* Sam
* Gajinder
* Zainan Victor Zhou


