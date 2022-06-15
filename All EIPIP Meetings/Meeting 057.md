# EIPIP Meeting 57 Notes
### Meeting Date/Time: Wednesday, June 1, 2022, at 14:00 UTC
### Meeting Duration: 27:26 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/141)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=k_EJIA3tHcc)
### Moderator: Pooja Ranjan
### Notes: Metago

----

## ACTION ITEMS

**ACTION 57.1**: Pooja will keep the Core EIPs in an Executable Spec World agenda item for next meeting, and try to get Tim, Greg, Sam, Micah and others in the meeting to discuss and make a decision on the item.

**ACTION 57.2**: Pooja will create an issue of the topic of and collect feedback from Matt, Greg, Alex, Micah, Sam and others regarding closing the final, stagnant, withdrawn EIPs 
 
**ACTION 57.3**: Pooja will collect feedback regarding one time NFT sale of unused EIP numbers.

**ACTION 57.4**: EIP Bot and EIPV Bot issues and pr topic will be on the agenda for next meeting to check on updates.

**ACTION 57.5**: Pooja will verify whether the EIP bots take 4 weeks to move to stagnant, and take action regarding improving the text to include a warning message during the process.

**ACTION 57.6**: Pooja will reach out to the devops team to add contributors for EIP's Github repo. 

## AGENDA

# Core EIPs in an Executable Spec World [Proposal]( https://notes.ethereum.org/@timbeiko/executable-eips)
[0:14]( https://youtu.be/k_EJIA3tHcc?t=14) 

And [discussion]( https://ethereum-magicians.org/t/core-eips-in-an-executable-spec-world/8640)

**Pooja**: All right, welcome to EIPIP meeting 57. I have shared agenda in chat for people who joined just now, may have missed it, so I'm gonna re-share it. The first item listed here is Core EIPs in an Executable Spec World. We have been discussing this item for past few weeks, and I remember in last meeting, there was a comment by Greg that we should postpone the final decision on this item. Sam did mention about some async discussion in Eth R&D channel. I'm not sure if there are further updates that you would like to share, Sam?

**Sam**: Nope, nothing really. There hasn't been much discussion since the last meeting.

**Pooja**: Right, so I wonder like we still have some few open questions, like where are we on this, like new Executable Spec World and is there any action item for anyone or, if and when we would like to have this item on the agenda for the EIPIP discussion. 

**Sam**: So we're starting on the Berlin hard fork. I think that's where we're at in the specs and I’m not sure when it should come up on the agenda for EIPIP. It really needs Greg to be here to talk about it, so I guess whenever he can be here. Yeah.

**Pooja**: All right. So I think there was one point that…I know Tim is not present in the meeting today and he mentioned that he would be talking to rest of the client team members to maybe seek thoughts on if they are comfortable going ahead with the python specs. I'm okay keeping it on the agenda and I will bring it back in the next meeting and I'll also try to get Greg, Tim, you, all of us together, in this call, so we can probably make a decision on this item.

**Sam**: Sounds good. 

# From EIPs GitHub [2:18]( https://youtu.be/k_EJIA3tHcc?t=138) 

[Close a few more issues]( https://github.com/ethereum/EIPs/issues/5119)

**Pooja**: Thank you. Moving on to the next item, EIP’s Github so this item is selected from EIPs Github. We have requested the users to leave issues if they would like to be brought into EIPIP meeting discussion. I have picked up two items from there, one is a list of close a few more issues. Pandapip1 created this list and I thinks that it can probably be closed, I wanted to bring it to EIP editor's attention, is it a fair approach of closing issues yeah.

**Micah**: So as for my comment in in there, I already addressed the first four. That big list afterwards though, we need to discuss and decide how we want to handle, so currently we are recommending all new EIPs get their discussions to link, sent over to Ethereum magicians, however any existing EIPs can who already have their discussions to pointing at GitHub issues, we allow that to continue. We don't have a plan for migrating data and so the question is, do we just want to leave those issues open forever, do we want to close them but allow discussion to continue on the closed issue that's probably fine or do we want to develop some sort of plan for getting people to getting this information somehow migrated to eth magicians.

**Pooja**: That's a very good question, yeah. I came across a proposal, I think 1202 which seems to be an old one and they are still having their discussion and discussion tool link. So yeah, this is a valid question do we have any proposal on migrating maybe?

**Micah**: None that I’ve seen. We've briefly talked about it and we just decided to leave them there for now. At one point we talked about maybe closing them when the EIP becomes final, and so that way at least the only ones would be open more EIPs that are not final and I think we also discussed possibly closing when they become withdrawn or stagnant as well the idea being that just so they're not in the list anymore. You can still comment on they wouldn't be locked, it would just not be listed in the issues. Another potential option is just to close them all and just close with a comment saying continue discussions here, we're closing it, so it stops showing up on our list of issues. I'm I don't feel strongly about any of these.

**Pooja**: I may have a slightly weakly opinion on the first one maybe to close on the final withdrawn and closed issues, close them all, could be like, you know, we can get strong and resistance from authors that…why are you closing it but I definitely like the idea of proposals which are closed like final withdrawn or stagnant because bot is continuously working on making stagnant to the proposal which are over six months and not into active discussion. That can be a slow but steady approach to get this number of issues lower. I don't know, Sam, if you have any preferences here?

**Sam**: Sorry, I lost my mute button there. No, I don't think so.

**Pooja**: Could we try the first approach, closing the final withdrawn and stagnant or any closed EIPs?

**Micah**: I'm okay with it. I would like to get feedback from Matt, Greg, and Alex, if possible if any of them just have thoughts.

**Pooja**: Yeah maybe I can create that as an issue like whatever proposal we are discussing here we can add that as an issue and try to collect feedback from them. If they are fine I mean no major objections are there, then we can probably start moving in that direction. This sounds like a plan because we definitely would like to decrease the number of open issues at the same time, we respect the sentiments of author that if there is a discussion to link, it cannot be closed like forever if we do not have any proposal on migrating them to eth magicians page, then probably this is a good approach to begin with, but we'll try to collect more feedbacks on it. Thank you for bringing it up. Other than that, do you think rest of the list that he has added here are good to be closed?

**Micah**: I’ve already addressed the other four. I think one was deleted, two are closed, one's left open, I gave them a comment as to why. 

**Pooja**: Thank you. Maybe we can see more EIP editors here, if they would like to provide any feedback that would be nice. Thank you. 

# [One-time NFT Sale of unused EIP numbers]( https://GitHub.com/ethereum/EIPs/issues/5082)
[7:39]( https://youtu.be/k_EJIA3tHcc?t=459) 

**Pooja**: The next sub item is here from the same EIP GitHub repository. It is one time NFT sale for unused EIP numbers. I know there are a lot of comments already and I just have added it to see if there is any appetite for async discussion on this. I'm not sure if there is any plan or plan in place to put this into action, what is proposed here or is it just like that.

**Micah**: I did not have any concrete plans at this time.

**Sam**: Yeah, it's still really early in the planning stage I think.

**Pooja**: But do we want to pursue it, like if so then we can probably start engaging more people to add more feedback thoughts there, how to implement this, run this.

**Micah**: I am weakly in favor of it but I would definitely like to solicit more feedback and ?  for example had some feelings on it, I'd like to hear more on that. 

**Sam**: I'm not opposed to it, so yeah. 

**Pooja**: All right, I'm not sure if we…

**?**: Sounds good. 

**Pooja**: All right. Maybe I can share this issue with him if he has to document any of his thought. Cool, cool, just wanted to have a temperature check what do people want to do with this. All right I'll try to collect some more information and bring it up in the next meeting.

# EIP bots related discussion, updates, agreement on merging PRs & closing Issues]
[9:24]( https://youtu.be/k_EJIA3tHcc?t=564) 

[eip-bot Issues and Pull Request](https://GitHub.com/ethereum/EIP-Bot/pulls) 

[eipv Issues and Pull Request](https://GitHub.com/ethereum/eipv/pulls) 

**Pooja**: Moving on, the next item, is EIPs bot related discussion updates, so lately I have not seen any updates on EIPV site. I will definitely go back and check with the contributor but we do see some action on the EIP bot side. I see there are a few open pull requests and Micah has already given a lot of comment. Jose yeah Jose is on the call so Jose if you would like to provide update.

**Jose**: Hello. Yeah that's basically what you say, you have three pull requests uh ready for testing. I gonna be able to do that testing this week well as soon as we test these three pull requests and they pass the test I guess that with the they are the foundation for at least five or six more issues that we're going to be able to pull, I would say easily merge after it. So I think that yeah we're making progress. I don't know Micah is here Micah has been supporting and helping a lot so maybe Micah can add something if he likes but from my point of view I think that we are moving slowly but getting there that's what I have yeah…

**Micah**: As Jose said we just need to get them tested make sure there's no bugs and everything works and then I think all of them are fine.

**Pooja**: I see a few more issues are open but it's good that we are making some progress over there. Yeah we will try to keep this item on the agenda and we'll try to have more updates in upcoming weeks. 

# [EIPs Insight - Monthly EIPs status reporting]( https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/) 
[11:31]( https://youtu.be/k_EJIA3tHcc?t=691)

**Pooja**: Moving on, item number four is EIPs Insight, so for the month of May, the report is ready. I have added link here in the agenda. We have got two final proposals and the repository has received 17 new EIPs as draft. We have potential nine proposals which are yet to be merged as draft, and three EIPs are moved to review. One is moved to the last call. The details are available in the report that I have added to the agenda. I’m yet to publish this on the other forums, we'll do it right after this call. So I mean EIP insight at least gives us one information very clearly is that like the number of EIPs we are able to move to the final status is really low in comparison to number of EIPs that we are getting every month in the repository. I don't know if people have any thought on how to manage it.

**Sam**: Like so is that is that actually a bad thing like I feel like we shouldn't be trying to get everything to final and maybe the metric we should be looking at is getting EIPs just into draft, and that would be probably an indication that editors are doing their jobs well, I don't know.

**Micah**: I think that I weakly agree with Sam there are many EIPs that in my personal opinion shouldn't go to final because I think they're bad ideas or they shouldn't be standards. Sometimes they're good ideas but they shouldn't be standardized. And so a lot of EIPs that fall into that category I think the fact they're not making a final is a good thing. One thing we may want to look at is like are we being aggressive enough with moving things to stagnant, maybe we should turn that up if we're finding that like everything that makes it, that doesn't get merged as a draft, or doesn't get, make progress in two months always ends up going to stagnant, then we should just bump that stagnant threshold to two months, instead of six months or whatever it is right now, but I’m, I don't feel strongly about that, like I’m okay with the current numbers as well. 

**Pooja**: So in my experience, a normal tenure for any proposal from draft to go to the final status, the shortest one is three months, so I'm not sure that I'm like very confident about moving stagnant to inactivity for two months though inactivity yeah…

**Micah**: Keep in mind that the stagnant is only if it's inactive not if like if it's making progress then it's fine like I think, nick munch for example is constantly
updating standard and it's been going on for like years but he's always touching it like he's always doing things with it so it doesn't move to stagnant.  The ones that get most stagnant are ones where no one has done anything on it for a substantial amount of time and so I want to make sure that we are distinguishing between EIPs that are making progress but going slowly which is totally acceptable as EIPs that are not making progress at all.

**Pooja**: Yeah, I totally understand that yes I was coming to the same point that if a proposal is making progress if they have to be like if we are expecting them to see in finance status in next three months, they would definitely be making progress at some point, but sometimes what happens like others get confused and they are not clear about what to do and that may be one of the reason of not moving the proposal. With the EIP editors internship meeting we have started inviting more authors to come and talk and share their questions and they are doing that. We are trying to share information around it so we are hoping that the proposal will be moving faster. You can see that quite a few proposal in this particular month itself which was in draft that moved to review and which was in last call that is final now. I mean it's not delaying anymore. Definitely editors are doing a great job here. It's just that we might want to give some room for new authors to maybe understand the process properly and start working in that direction. Yeah, I mean it may be my request that making stagnant a little more aggressive, we can probably give some more time or if not two months, maybe we can give a little bit more time I don't know.

**Micah**: The other thing to keep in mind is that the bot will first write a note in the EIP, saying that this has been stagnant for a while and then I think two weeks later it will actually move to stagnant, if ever correctly and so often just having that bot write the note kind of reminds the author hey we're waiting for you to do something, or if they didn't know they're waiting, they'll often reply saying oh what am I supposed to do I thought I was waiting on someone else, and so I think bumping the stagnant bot to be more aggressive, I don't, it may just result in people moving their EIPs faster, because they will, the bot reminds them basically, when it drops a note in the EIP. 

**Pooja**: Yeah, I think I'm coming around…

**Micah**: Yeah we should verify that the bot actually does that I might be thinking…

**Pooja**: No, no, you are right it gives a two weeks’ notice period over there yeah it does give two weeks’ notice period.

**Micah**: Because there's two different bots, one for the stack for moving a draft EIP to stagnant, there's another one for closing open pull requests and another one that closes open pull requests, give us two week notice I actually don't know how the stagnant bot works, does it create the pr and then wait two weeks to merge it? 

**Pooja**: If I remember correctly that's the process but I would like to revisit that thing. Yeah when I saw it last when I had this notification on for bot making an announcement that this pull request or this proposal is has no activity for past six months, it gives a two weeks period time. 

**Miah**: Okay, all right.

**Pooja**: So if I have to sum up this proposal here if the process is still that bot gets two weeks’ notice to author of a proposal stating inactivity we can probably pump the bot to three months instead of six months for making it stagnant.

**Micah**: That would be fine with me if it got to that would be fine with me if it got too much trouble we can always move back.

**Pooja**: Jose, I did not understand the comment here, EIP bot does not do it now but can may do it. 

**Jose**: Well yes. I don't see the bot can do now the warning to the outers but it can be done I don't know, you just need to define the time that you want to as make a mention that you want to let everybody know and yeah we can send the messages, we can add a comment, whatever we would like to do, the bot can do it, but that's, right now as it is that's not, that's what I was commenting in the chat okay.

**Pooja**: I mean, be missing here I just have shared a full request in the chat that is one of the last stagnant activity I noticed I do not see a mention of two weeks’ time period here but it definitely gives a warning I have to maybe check.

**Micah**: So it looks like for that one the bots showed up on April 10th and then merged it on May 8th so I'm guessing it's certainly set to four weeks, so it opens the pull request waits four weeks then merges if I had any guess it'd be good to find like maybe two others, and see if they all had the same behavior. I think I can share a couple of more, probably would help to probably be good to also adjust the text to let authors know if you're still working on this, please reply saying as much, so we can close the pr or something, just letting the author know this is automated and it's okay if they're still working on, they just need to say something.

**Pooja**: All right. So I'm taking action items here improve that text for a warning message and be sure it gives some time for authors to respond back before it is closing. Yeah, like I said, that one looks like it's about four weeks and we should verify them.

**Jose**: Correct.

**Pooja**: Okay so as an action item may be first we will create an issue in EIPs bot to update the parts checking from six month to three months and then see if this can be done with the updated text, updated warning text for authors. Cool, so yeah that's basically all on the EIPs Insight side. I have started adding charts and in addition to this I’m also trying to get this thing updated on maybe some form of website, so we can move it from hackmd file. I may be looking for one information here. What is the backend used here for these numbers to be displayed…for eips.ethereum.org?

**Micah**: Oh, Jekyll, which is Ruby.

**Pooja**: Jekyll, okay, yeah, I thought so. I found it over there, but someone, I mean like one of my developers said that please check if it is php or not so I was just trying to be sure of it, well, thank you.

**Micah**: The tooling is Jekyll, depending on what the person is interested in helping with it, doesn't might not actually need Jekyll or Ruby knowledge, it might be like handlebars or something.

**Pooja**: Okay, maybe I'll ping you offline. I may have a few more questions on this. 

**Micah**: Okay, so yeah. I'll ping you offline. 

# EIP editor apprenticeship meeting
Meeting 18 [Agenda]( https://GitHub.com/ethereum-cat-herders/EIPIP/issues/140), [Recording]( https://youtu.be/Mr6G2823-S0) 
[23:13]( https://youtu.be/k_EJIA3tHcc?t=1393) 

**Pooja**: All right, that's all about EIP's insight. Moving on to the next item, EIP editor apprenticeship meeting, we had this meeting yesterday. I have added agenda and recording. Unfortunately the recording is really bad zoom recording there, but we have the agenda in which we have listed all the proposals which were discussed and shared on the screen sharing done by Matt, so if anyone has any question, please reach out to us on cat herders discord. We'll try to help you out there. Most likely answers are already there because Matt left some comment, we had some discussion that can obviously be caught on the video, and some had good suggestions for how to improve and how to make sure that your proposals are viewed by project implementers, so please follow those things. That way, you'll be able to increase awareness of about your EIP and it can be implemented in projects when you are trying to push your proposal towards final, the next meeting is two weeks from yesterday so if you are interested to join meeting is generally available on events section of Ethereum catalog justice card.

# [Review action items from the previous meeting](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20056.md)
Contributor's permission to EIP GitHub repo for Sam Wilson
[24:33](https://youtu.be/k_EJIA3tHcc?t=1473) 

**Pooja**: The last item listed here is review action from the previous meeting and from previous meeting it suggests that splitting out EIP repo from EIPs and ERCs will be put on hold. Obviously there were no decision in the last meeting, and with the education specs coming up we'll see how it turns out if needed, then we will bring back discussion on agenda. No changes will be made to that repository, that's fine. One other thing that was brought up in the last meeting was a contributor's promotion to EIP's GitHub repo for Sam some I put this thing based on the discussion from the previous meeting of EIP editors internship you mentioned that you were not able to open and summon the ? 

**Sam**: Yeah, so I'm okay with not being a contributor. I just think like being able to paste it or put a comment in or something that that re-triggers the bot would be nice. 

**Pooja**: Well just to add some context here, in the last meeting we were discussing that we should have like two to three contributors, Micah is there, lightclient is there, but there was another girl which may not be there anymore because she is not an active contributor right now, so if at all you would be interested we can probably make a room there. All right. Okay, for this item only, do I need to reach out to a devops team? Micah would you recommend me doing that or is it something that can be vanished?

**Micah**: I think the devops needed to do it I couldn't figure out how to add real people to teams.

**Pooja**: Okay, another problem then. I'll try to reach out to him and see if this can be done. Well, that concludes the meeting for today. It's short, within 30 minutes. Anything else anyone would like to bring up no looks like it's been a quiet week and we didn't have much action on EIP site though where there are a lot of actions on merge site. So yeah, thank you everyone for joining us today, hope to see you in two weeks. I will share the recording very soon. 

Everyone thanks each other. Meeting ends.

 
---------------------------------------
# Attendees

* Pooja Ranjan
* Micah Zoltu
* Sam Wilson
* Jose

# Date for Next Meeting: 15 June 2022 at 1400 UTC.







