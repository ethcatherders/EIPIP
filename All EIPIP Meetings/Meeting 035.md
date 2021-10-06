# EIPIP Meeting 35 Notes
## Meeting Date/Time: Wednesday 16 June at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/72)
### [Audio/Video of the meeting](https://youtu.be/VgsK8xnrL3U)
### Moderator: Pooja Ranjan
### Notes: Jim Bennett

----
## DECISION ITEMS

**DECISION 35.1**: Anything that wants to be an Ethereum standard need to go through the Ethereum GitHub repository [See 3:37](https://youtu.be/VgsK8xnrL3U?t=217)

**DECISION 35.2**: Alita to investigate a bot exclusion to EIP-1. [See 11:58](https://youtu.be/VgsK8xnrL3U?t=718)

**DECISION 35.3**: EIP-1 changes to only require two editors to approve. [see 19:37](https://youtu.be/VgsK8xnrL3U?t=1177)

**DECISION 35.4**: Mark the JSON RPC API spec in the Eth 1.0 as deprecated internally until after London goes to mainnet, and then remove it from the spec repo after that. [see 42:07](https://youtu.be/VgsK8xnrL3U?t=2527)

**DECISION 35.4**: Change the name of Eth 1.0 APIs repo after London is shipped. [see 46:37](https://youtu.be/VgsK8xnrL3U?t=2798)

## AGENDA

**ECH - Pooja**
Welcome to EIPIP meeting 35. I'm going to share [the agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/72) in the chat.

#1. [ERC process & standardization](https://youtu.be/VgsK8xnrL3U?t=11)

So the first item on the agenda is ERC process and standardization. Oh, my god! Okay, so there has been some discussion around this ERC process. I have tried to add a couple of links. One is [the process that I'm proposing](https://hackmd.io/@poojaranjan/ERC-Process) that can be done to improve the current process and help push most of the ERCs which are still in Draft status, to let them go in and assign whatever is the appropriate status for that proposal. And there is an another proposal from Eth Magicians. It's [a rework of the ERC process](https://ethereum-magicians.org/t/rework-erc-process-from-eips/6488) that should be something different from EIPs.

I'm happy to go through my proposal, if that helps. So it just suggests that whatever ERC already, stack stage, Draft, or maybe in any other state for over a long period of time, maybe over three months, we should reach out to them. I'm happy to engage Cat Herders to get that work done if that is the way we would want to go ahead with it. We could reach out to them and define what is the current status, whether they want to push it or not. And unless a proposal is in the Final status, that should not be considered as ERC standard. That is my proposal. But according to the other proposal, ERCs do not need a state of finalization, that is Request for Comment. And it does not have to follow the standard process. I'm not sure where we can bring this topic up. So I thought of bringing it to the EIPIP meeting because of two reasons. One, we have a lot of editors here and another is the process improvement meetings. So I'm opening upfor  anyone to share their thoughts.

**Hudson Jameson**
I think lightclient did a good job of responding in the thread that you linked in the agenda, about Annette wanting to change some pieces of the ERC process and that highlighted some misconceptions people have with the ERC process. So I think education above all is going to be helpful here. If people want to come in and suggest changes to the process, that’s great. I think a big overhaul, Annette seems to be indicating that's probably a bit too much.

**lightclient**
I think something that might give a good win is just to not assign numbers to ERCs until they reach a Draft status - force there to be a pre-status for ERCs, something like the Idea stage. It feels like as soon as they get a number, they just run off and start telling everybody about their ERC.

**ECH - Pooja**
That's another concern that I have. Even if that is not in the pull request, if it is in somebody else's GitHub repository, they are still calling it an ERC. So that is my biggest concern. If they want it to be an Ethereum standard, it has to be in the Ethereum GitHub repository at least.

**lightclient**
Agreed. Yeah. This actually mirrors how the IETF handles RFCs. They have some pre-RFC process where it doesn't receive an RFC number. And that lets people work on it some before it reaches the stage where it's considered a Draft RFC, or, I forget if they have a different name for it, but there's actually official stages that have to happen before you are assigned a number. And I think just forcing that is going to significantly cut out the number of junk ERCs that we have to deal with.

**ECH - Pooja**
Right. So if I understand correctly, there would be two important points that we have to consider at this point of time. Maybe one for upcoming ERCs is how to deal with the ERC number and for the existing proposals which are already there, pushing them. And the suggestion for the upcoming proposals here is to not add the number. Any other thoughts or comments on this?

**Brent Allsop**
It may not be related, but for things that require some kind of bridge, or some kind of something to achieve, I don't know if everyone's ready to do this yet. But we've got the CoreDev thing that CoreDevs can rank each other and determine who is and is not a CoreDev, if that got further developed, then we can develop an algorithm on Canonizer where if you had X number of CoreDevs signed on, and there's various techniques we could do like that. So that is something would have to be signed on by a certain number of people or certain number of CoreDevs and stuff like that. And in any way, just an idea for possible future things for whenever something has to cross a bridge. In my opinion, that would be a good way to achieve those kinds of things, so that no one can just say, “Well, I’m an ERC already.” But it shows how much support any ERC may have in a quantitative way for which you can set a bar where you can say something isn't an ERC until it meets that bar. Just FYI.

**ECH - Pooja**
Right. With the ERC, the challenge is it's not core proposal, so it cannot go to the AllCoreDev meetings. It's difficult to get the set of people here on one call, or at least on this EIPIP call to make a call, like how they would want to see. I think the trend is good that Matt has started. And we can continue discuss discussing the future process. But I hope the candidates are still good to go ahead and look into the older proposals. Does anyone have any strong feelings, or should we wait for some time?

**lightclient**
So what would you be looking to the older proposals at?

**ECH - Pooja**
So far, just 20% of ERCs that have been proposed are in Final status, and over 100 ERCs are either in Draft or in Last Call, or somewhere else. They are obviously being used and treated as standard in many places. But they are not standard according to the standards. So I was hoping to push them to get a destined status.

**lightclient**
I see. Yeah, I mean, that sounds like a good idea to me.

**ECH - Pooja**
Yeah, I think that would also help us clean a lot of eips.ethereum.org's list, because I'm not sure if we really have over 100 ERCs active and usable. Some of them might have been superseded or may not have been moved for a very, very long time, though the pull requests are closed, so we can reach out to them. One related task, I was just reminded. So we have created an issue on EIPIP GitHub that was discussed on the last meeting, that we are also looking for someone to work on a bot to identify these proposals not only for ERCs, but for all different types of EIPs so we can identify Ethereum and mark them as Closed or Withdrawn if they are no more in use. Anyone who is listening to the meeting and interested in work, the issue number is 73. Please respond to the issue if you are interested in working on that.

**Alita Moore**
Also, just to kind of jump in here, if no one else is able to do it or wants to or whatever, I'm happy to hop on it. Or even just if someone starts working on it in his questions, feel free to reach out. I'm sure I can help with its implementation.

**ECH - Pooja**
Yeah, right. So Alita has already worked on some of the bot-related work for EIP GitHub repositories. If you have any questions, feel free to reach out. Alright, any more questions or comment on this?

#2. [Updating EIP-1](https://youtu.be/VgsK8xnrL3U?t=613)

Okay, moving on. The next item is updating EIP-1. So I have created this pull request with very, very small changes. I think that it has been approved. But I still see here as not much. So I will try to look into it. My concern here is it requires approval of two of the authors mentioned in the proposal, EIP-1. I am not sure, Hudson, one is you and the other one is Martin. But I'm not sure either of those emails are active anymore, or how this can be solved. If it is not,

**Micah Zoltu**
You can ignore the bot for EIP-1. Because it's technically an EIP, as far as the bot is concerned, it does its normal path. But our process for EIP-1 is just making sure that the editors agree. Historically, my policy has been create a PR for EIP-1, wait for other editors to speak up. If no one speaks up after a month, then I just merge it. It'd be nice if we could get more interaction from more editors, but that doesn't always happen. So just wait a month. And if no one says no, then I go forward. That being said, with this one, I mean, it's basically just corrections and edits. I don't have a problem just merging it as it is, since no one's responded negatively.

**ECH - Pooja**
All right. Yeah, I responded to the bots thing. That requires approval, and I was trying to dig into that.

**Alita Moore**
Do you want me to add an exclusion for EIP-1? I can do that.

**Micah Zoltu**
It wouldn't hurt. EIP-1 doesn't get touched very frequently, so it's not a huge deal. But if it's a simple thing like a one-line change, sure.

**Alita Moore**
Alright.

**Micah Zoltu**
Do we have automerge on now? If we disable the bot for that, it's just going to instant merge?

**Alita Moore**
I think it actually requires that the bot be, I'm not saying disabled. by the way. I'm just saying fail it every time, more or less. The error would be, like, "EIP-1 is not suipported at the moment.""

**lightclient**
Well, I wouldn’t do that. I would just not automerge EIP-1 changes. Just request that editors only merge...

**Alita Moore**
Surprisingly, there's more problems than you would expect to not do that. So at the current moment, using editors  fail. So you need the bot.

**lightclient**
Yeah, I think I just would not want to have failures as the common state, rather things be passing. Because then, if we have to force a merge,   don't even have access to force merge if the bot fails, for instance, but also, I would rather have passing CI show on the master branch.

**Micah Zoltu**  13:30
So the problem is that GitHub automerge is just when CI goes green automerge. So either you fail CI, or it merges automatically. And so we don't want people just be able to submit a PR for EIP-1 and just have it automerge because there's no checks against it. But at the same time, we don't want it to be blocked. This is where there is notable engineering to work around this. It's not as simple as just let it go. We have to do one or the other. Either we don't have any auto working whatsoever.

**lightclient**
Can we not, instead, be using the authors, just have a list of the EIP editors and ping them the same way that the bot is pinging authors. And then on approval, check to see if an author approved or an EIP editor approved it.

**Micah Zoltu**  
That is on the To Do list, that feature just in general. So specifically for when we transition between Draft and Review, rather than just having the author approve the PR, it would take an author plus an editor to approve the PR, and that would let it go through a state transition. So from Draft to Review, Review to Last Call, Last Call to Final. We could have something in theory similar for EIP-1 where we require editors to approve. That is definitely much more within the realm of possibility. It just requires some small changes to the bot. So that's a smaller, much smaller engineering task. Caveat: Are we okay with EIP-1 changes after a single editor approves?

**lightclient**
Yeah, I was gonna say that's kind of unfortunate that we can't let it sit there for a while and just have other editors approve as they have the time to review.

[Crosstalk]

What do you mean in draft EIP?

I'm sorry, not a draft EIP, a draft pull request. The pull request of the draft, they won't automerge.

**Alita Moore**
And then, just to be clear, The things you're talking about, lightclient. I think they're possible to add to the bot. The question is whether or not we want to. Like if it's a one line change, just to fail a bot if it’s to EIP-1. But then to add the different criteria and stuff, it's getting easier because I'm cleaning up the logic, but I don't know, it's slightly more complicated and probably just generally not worth it.

**lightclient**
I mean, I just don't want the default for EIP-1 changes to be failing. It's fine if it fails until it is approved and merged. But I don't want the default for the CI to be failing on Master. In an ideal world, the CI on master would never fail. We would only merge on success.

**Alita Moore**
I mean, that's fine, I'm gonna go ahead and investigate, because I don't know. Essentially, the way that automerge works is you're given a list of required checks that need to pass, and once they pass, it merges. And I don't know if that considers if a check was skipped. And then in that case, it wouldn't be failing, but it still wouldn't automerge. So I'm gonna look into that. But more importantly, that sounds good. I'll address that problem.

**lightclient**
Thanks.

**Micah Zoltu**
I think, in my opinion, the ideal solution, given the constraints of the tooling available, is to have for state transition PRs, it requires author plus editor review. And so there'll be maybe two checks or one check that does both or whatever. And once that happens, it'll automerge. And then for EIP-1, I like the idea to have two of three or two of N editors approve. So once you get two editors approval on an EIP-1 change, then we'll merge automatically. That way, we get what lightclient wants, which is that we always have green CIs. There's ways to get CI to pass without having to bypass it, which we're doing right now. And at the same time, it makes it so EIP-1 doesn't automerge just as soon as the first person approves it. You have to get a couple of approvals at least.

**lightclient**
Yeah, that's better. But it's just not ideal, because then you have people like Alex who comes in, and you've maybe approved and I haven't got around to approving, and he reads it. And he says, “Oh, this works. This is good.” And he approves, and then it merges, and then he's just sitting on his computer, like, “Why the hell did it just merge? That’s weird."" And so he's not sure what just happened. And then I don't probably review because I look and I see all that was merged, so it's fine.

**Micah Zoltu**  
So I think I think the other thing we can do that's low-hanging fruit is just to have a general kind of policy amongst editors that when you're making changes to EIP-1, do it as a Draft PR, until you have lots of eyes on it.

**lightclient**
Yeah, these seem okay. I don't know if there's actually a way to do this properly with GitHub actions. I know you can do it with some of the other auto GitHub managers.

**lightclient**
with enough engineering, we could make pretty much anything happen.

**Micah Zoltu**
Now, it doesn't look like it can actually be done with GitHub actions.

**lightclient**
Because they probably use GitHub action through the API. So the GitHub action would then call it GitHub API, which would then call back into GitHub, then merge.

**Alita Moore**
It's a complete nightmare. And then in some cases, when the REST API isn't good enough, then we can start using graph QL. But whatever the point is is that that sounds great, and I will look into adding those those exceptions. Just to actually clarify, are we in agreement, are you all in agreement that the EIP-1 change should require two editor approvals, and then that's it?

**lightclient**
Given that we only have two editors that actually pay attention. I feel like any higher than that and we're just asking to never merge anything. And lower than that, it’s just basically the first person to see it merges it. So two feels pragmatic.

**Alita Moore**
Okay, I'll add that.

**ECH - Pooja**
Sounds good. Thank you. So another small point I wanted to bring up here was related to EIP-1. If we go to EIP-1, there is this section of core EIPs. I'm going to share the link in the chat for people to refer to. So there is this section of core EIPs. The first statement of it suggests that for a core EIP to be given that kind of dimension, it is considered a final EIP process. Now that we have separated the EIP process and the network upgrade process, my understanding is that here we should have the network upgrade process. Because the EIP process that is pointed here below is basically the EIP statuses. These seem like a big changes for me to do it right away in the pull request. So I wanted to bring it up in the meeting first before I can create a pull request for that. So is it something we need to change here, it should be network upgrade process, because we are talking about core EIPs?

**Micah Zoltu**
I'm of two minds on this. On the one hand, I would like to rip out that whole core EIPIP section and just treat core EIPs like all other EIPs and follow one consistent process. On the other hand, I recognize that a lot of people don't understand the whole Ethereum change control process in general, and sometimes they end up starting out on EIP-1. And this kind of circles back to the whole our documentation on the Ethereum change control process is distributed across a number of different places. And I think getting that consolidated will help with this and will allow us to have this document focus just on the EIPs repository stuff and not have to worry about describing "What does it mean to get a change into Ethereum?" And just focus on "what does it mean to define a standard" will be this document. As to what we should do right now? Eh, whatever.

**ECH - Pooja**
Yeah, this point, I also figured,, while I was going through this document again and again, I figured that at many places, instead of writing just EIPs, we could have just proposals, and that will cover all. It's not only for core, it's not only for that particular type. If we address them as proposals or improvement proposals, that would have helped a lot. But for this particular section, I think here, because this was before we had two separate processes, my understanding is for under bracket, it should be network upgrade. And when we are talking about the below that is labeled as EIP process should be actually the EIP statuses. I don't know. Please, somebody help here.

**Micah Zoltu**
You're talking about in the EIP workflow section, the sub section, core EIPs, right?

**ECH - Pooja**
Right.

**Micah Zoltu**  
Yeah, I really think we can just delete the whole thing. I'm reading it right now. And all of this is basically outdated. I don't think any of this actually is correct or applies anymore. If there's information that we want to retain, it should be moved over to Eth 1.0 specs repo,

**ECH - Pooja**
Right. So we already have added that in the README file of Eth 1.0's own spec repo.

**Micah Zoltu**  
Yeah, I'd say just delete it. I don't even think we need a pointer. Just delete all of it. Most of this is wrong. It's from years ago, and it's doesn't actually reflect the process we actually follow.

**ECH - Pooja** 24:14
All right. About this diagram, I remember I mentioned it in some of the channels about this Stagnant that it is a state and it should not be considered a status. But later on by looking into ERCs, I felt like it should be a status for those proposals which are stuck somewhere.

**Micah Zoltu**
Yeah, I'm fine with that. I think we talked about having it be a status, but it wouldn't take effect for a year or something. When we're usually talking about it, we we said something like if the EIP sits for six months or 12 months or something, I don't remember what the exact amount was, then we'll just move it to Stagnant just to indicate that no one's doing anything.

**ECH - Pooja**
Alright, I just wanted to correct like I mentioned it somewhere. So I think you're right there. So yeah, just wanted to bring it out again. Alright, so we will revisit this EIP-1 one more time to try to figure out how it can be improved. Because I have seen that people have started using it lately, because we have been talking in different forums that the best place for you to start learning the EIP process or destination process is to go read EIP-1. So unless they make that up to date, it would be difficult for asking people to follow the right process. Any more comment or question on this topic? Fine.

#3. [New EIP editors onboarding, funding, and related processes.](https://youtu.be/VgsK8xnrL3U?t=1543)

Moving on to number three item: New EIP editors onboarding, funding, and related processes. So in the last meeting, we discussed about having a couple of more resources like interns, or maybe apprentices for EIP editing. And for that, I just have created a small document that is a handbook for reference for new people. We have seen people visiting us on Discord and other channels asking how to support. So this is just listing what is the right set of places to visit or the documents to refer, and a few frequently asked questions. I'm not sure if there is any actual work that has started and people have started working on it. Anyone have any info on that?

**Micah Zoltu**
I can confidently say that I have not done anything.

**Hudson Jameson**
Yeah, samesies. I think you set up the channel on Discord since last time, and there was a little bit of movement from - who was it? Spore? But are they here today?

**ECH - Pooja**
I don't see any of them today here on the call, actually.

**Hudson Jameson**
Yeah, so we might have to table this one until we get them back in here.

**lightclient**
Trent, are you still interested in doing some EIP editing? Or is that phase passed in your life?

**Trenton Van Epps**
I am definitely interested in learning from you guys. Sure. I can't contribute at the same level for sure. But I'd be curious to at least try to engage a bit more.

**Micah Zoltu**
I think you may be overestimating the level at which we contribute.

**Trenton Van Epps**
Cool, then sign me up.

**Hudson Jameson**
Yeah. So let's add Trent to the chat, Pooja.

**ECH - Pooja**
Yeah, I'll do that. And Trent, I know you are very much familiar with the process and everything else. But in case if you have any questions, you can refer to that document. But yes, that is a good way to start. I'm not sure, Tim, if you have any further questions on that, like, you wanted to discuss something?

**Tim Beiko**
Sorry, I didn't have time to look at all.

**ECH - Pooja**
All right. No problem. Okay, as far as the onboarding is related, I think the general process here would be people start looking into pull requests and issues and start adding comments. And as we see more comments getting in, eventually it will be easier for them to put them into full time. Not full time obviously, like the EIP editor as we have a few people here. Okay, any more question on that? We can continue discussing this in the channel that we have created recently.

#4. [Progress on EIP GitHub repo action bot.](https://youtu.be/VgsK8xnrL3U?t=1745)

Moving on to the next item, it's the Progress on EIP GitHub repo action bot. So I was curious to understand. My understanding has been that it is almost done and it's about to be finished. So I just wanted to make sure if we are done with the primary task of renaming the bot, script has been transferred to Ethereum GitHub repository and the bit is working as functional, and can we mark this task as complete?

**Alita Moore**
Yeah, it's complete.

I'm not sure if it's only me or someone else who see it's the bot with the same name. I heard that you mentioned that you are human more again, but it is still...

**Alita Moore**
Oh, do you mean like the actual repo bot? Yeah, we just decided not to rename it because the EIP bot is pretty self explanatory in terms of its purpose. I suppose it can be renamed. I don't know what the impetus was behind renaming it to begin with. I think maybe that was moreso in reference to moving it from my private repo to the Ethereum repo and/or transferring ownership, which we have done. So I'm not holding my breath that it's going to be renamed. Nor do I think it's necessary.

**Micah Zoltu**  30:35
Isn't the bot currently named Alita Moore?

**ECH - Pooja** 30:37
Yeah, that's what I see here. So I'm wondering if it is renamed, why is it not showing to me?

**Alita Moore**
No, it's so it's currently named Eth-Bot now.

**Micah Zoltu**
Ok, I think the task is done, then. It used to be named Alita Moore.

**Alita Moore**
Yeah. So I created the new bot to then take over my role. I think the reason why there might be some confusion, Pooja, is because I did it last night. And so it really hasn't updated yet.

**ECH - Pooja**
So it's good to say that the new bot name is Eth-Bot.

**Alita Moore**
Correct.

**ECH - Pooja**
Then we'll start using that one instead of EIP-bot. Good to know. Okay, then, I know that you have created [an issue.](https://github.com/ethereum-cat-herders/EIPIP/issues/59) Could you please mark it closed? I saw some last comments that were a month old. If you could just answer to that and close that issue, that would be great. We'll mark that task as completed.

**Alita Moore**
I think I closed the issue. Yeah, sounds good.

**ECH - Pooja**
Thank you so very much. Okay.

#5. [Progress on JSON RPC API spec in Eth1.0 repo](https://youtu.be/VgsK8xnrL3U?t=1922)

I see the next item on the agenda is also for you to speak on. I see your comment that you would like to update us on JSON RPC API spec in Eth1.0 repo the work that you have done and your team is doing. Please take it away.

**Alita Moore**
Yeah, so the JSON RPC is admittedly taking longer than I'd like. It is turning out to get the GitHub actions is a significantly more complicated procedure than you might expect. But there's a plan. There's a vision for it. And I just recently onboarded Jared, who is on the call right now, to basically help with producing things, because I don't work full time. I work, I don't know, like 12 to 16 hours a week on all this. And so it's hard to make a lot of progress. But Jared's been working full time with me, I'm going to be kind of project managing him. I'm kind of training him today and tomorrow to hopefully ramp up production in terms of getting these edge cases made and everything. I don't know if anybody was aware of this promise, but I did promise to have EIP 1474 converted to Open RPC such that we no longer had to rely on the Ethereum Classic Open RPC, which that is not done, that is being delayed because it's more important that I onboard Jared and get that production rolling. So in addition to that, every EIPIP meeting, I'm going to be covering the endpoints, I'm going to be educating, or we're going to be edge casing. And then, essentially, it'll be a time where if, for whatever reason, I don't know, Tim, maybe you know, 1559 has a high importance right now. Or if there's some endpoint with high priority, then people can let me know, and I can prioritize those above others and drop some things that we're working on. Whatever, just to try to keep some visibility into what's being done.

**Tim Beiko**
Yeah, I think the most important thing right now is the CCL spec. I was talking about that with my client this morning. So that seems reasonable. Yeah, I think all the 1559 stuff is either done or it's not blocked. There's no 1559 changes that are needed. We might decide to do more in the future, but I think people will submit PRs for those. So yeah, I don't think there's anything left for you to handle there.

**lightclient**
I posted in the chat, but I ended up rewriting the spec under CCL yesterday, so I recommend basing work off that.

**Micah Zoltu**
Oh, you did.

**Alita Moore**
Wait, did you just do all my work for me? What?

**lightclient**
No, it's it's pretty basic sketch, I just was basically copying the information from the Eth wiki. So there's still probably some bugs and stuff.

**Alita Moore**
Lightclient, stop doing my work for me, but yeah, sounds good. Thanks. I'm gonna use that for sure.

**lightclient**
Do we want to break the JSON RPC stuff to a new repo? Was anything decided on that?

**Alita Moore**
This is the first I'm hearing about that.

**Tim Beiko**
Oh, yeah. So lightclient and I were talking about that, but it seems like the Eth 1.0 specs repo and the JSON, basically contains two things right? There's JSON RPC, and there's the consensus specs, it seems like those two things are very tightly coupled right now. And there's not a ton of reason to have that. Eth 2.0 basically has two separate repos - they have Eth 2.0 specs and Eth 2.0 API. And I feel like it might be a good idea to do a similar thing, just because especially if we move to a spot where we do have an executable spec for each one. There's just gonna be such different things, the executable spec and the JSON RPC spec. Yeah, so that was the idea there. Let me see if I can find the GitHub issue I had for it.

**lightclient**
See if anyone had commented on it.

**Tim Beiko**
Yeah, people might have just missed it. I think I posted it in the JSON RPC channel.

**lightclient**
I posted in the chat here.

**Tim Beiko**
Yeah. And another thing, too. I feel I'm a terrible maintainer for the JSON RPC stuff. I just have very little hands-on experience with it. I think I'm okay to maintain the specs repo. But it would be good to also separate those concerns. Right now, it's not the end of the world. I'm happy doing it. But I think having two different repos. And I don't know how urgent that is. I'm not sure. It's not something I would do before London hits mainnet, for sure. Because we've been pointing everybody towards the single repo. But if it's something everyone agrees to, then maybe right after London is a reasonable time to split this.

**Alita Moore**
This makes sense to me. Just to reiterate and be clear, we want to split it because of the fact that like the edge casing, and the base specification are kind of two different things.

**Tim Beiko**
No, so I would remove even the JSON RPC spec from that repo, basically. It just feels to me like the consensus spec, the actual core EIPs in the hard forks are very different from the JSON RPC spec. And that's what I would want to split. So everything JSON RPC related would go into the separate repo, and everything consensus spec related would stay in the Eth 1.0 specs repo. So if you look in the issue I shared, Eth 2.0 exactly that. And one thing this would allow us also, aside from just a better separation of concerns, it would allow us to version the JSON RPC spec much easier. So Micah, and lightclient both had proposals where we could have a master branch, which is like the stable spec, but then we could create a dev branch and have changes go first into the dev branch, and maybe every month or so, depending on the frequency of changes, we review them, and then we merge dev and the master. So you know, in this case, for example, for London, it would have been really nice to have a specific dev branch that has all the 1559 stuff, especially as we're still iterating on it. And then maybe once London actually goes live to mainnet, then you merge that in the back in the master or something. And obviously, that's something that gets really awkward to do if we also want to do the same thing with the consensus specs, right? I think we want to move to a spot where if we have full consensus specs for Eth 1.0, then we can do a similar thing where we have a branch for hard forks and stuff like that.

**Alita Moore**
Alright, yeah, that sounds good to me. Whatever you think is best to keep things clean.

**Tim Beiko**
Yeah. And lightclient, you're saying, what would you PR?

**lightclient**
So, you know, I've written most of the JSON RPC spec under CC, like the absolute bare bones with the methods and the types, but there's still a lot of descriptions that are filled out or anything. And so I can PR that into the Eth 1.0 repo, because the problem is that any work that we're doing on top of the spec that exists right now goes under Apache 2 license. And so the sooner we transition to CCL, all the work becomes CCL that's built on top of that. So I can either PR into the Eth 1.0 repo, or we can just start a new Eth 1.0 API repo and put some deprecated notices in the Eth 1.0 specs repo that point to it. That's my preference.

**Tim Beiko**
I think I would slightly prefer waiting until after London, just because we've been pointing and we have a bunch of London documentation that points there. So it's not the end of the world even if it's marked as deprecated, but it feels like just having one spot might reduce confusion for the next month or so.

**Alita Moore**
Can we just like mark it as deprecated internally and not socialize that publicly until London?

**lightclient**
Yeah, we can do that, or we can also do a sub module within it, and then it looks the same to everyone else, but the information is coming from another repo, so it doesn't really change anything. It's just after London, we'll like remove it from the spec repo.

**Tim Beiko**
I'm fine with that. Does anyone have thoughts or objections?

**ECH - Pooja**
Well, I'm about to say to lightclient why not make a PR? Now it is clear why are hesitant, so I'm in favor of that.

**Tim Beiko**
And so the only thing you would need for me, then, is to actually create the repo, lightclient?

**lightclient**
Yeah, you can create the repo.

**Tim Beiko**
Okay. So I can't, but I can ping the DevOps people, so it should be done today or tomorrow.

**lightclient**
Great. And then if you can add me as admin so I can maintain the CI stuff on it.

**Tim Beiko**
Cool. Yeah.

**lightclient**
We'll figure out whether we want to just build it out separately, and then after London kind of announce this thing or if you want to do the sub module, check and see how it looks either way.

**Tim Beiko**
Okay. Um, what do people feel about names? Should we ask in AllCoreDevs what people think?

**lightclient**
That could delay this decision by two weeks.

**Tim Beiko**
No, I meant on the chat. No. Yeah, that could delay the decision. Okay. Yeah, okay. So going for Eth 1.0 APIs?

**Micah Zoltu**  43:59
No, no Eth 1.0 we should be terminatingthe name Eth 1.0, Eth 2.0. It should die in fire.

**Tim Beiko**
Yeah, I agree that like we should remove that at some point. But I would do that change when we do the [crosstalk]

**Micah Zoltu**  44:22
The longer we wait to change these names, the more they're going to get seeded in, and the harder it's going to be. Changing names is really hard to do, especially with a large community. We should rename that right away. We should be renaming things today. Once a week, I ping Danny and say hey, can we please rename the channels in Ethereum Discord because it's hurting us the longer we don't do this. And he's like, yeah, we should do that. And then a week later, I'm pinging him again.

**Tim Beiko**
I think the time to do that is after London and Altair. Because we point people to all these places, if you start changing the names, there's already a bunch of dead links in my old 1559 stuff. So yeah, we really need to rename it. But yeah, I would wait until after that.

**Micah Zoltu**
So with with GitHub repositories, when you rename them, as long as you don't create another repository with the old name, it will 302 redirect, so you don't have to worry about links dying if you rename the repository.

**Tim Beiko**
I think we probably want to rename everything, right? I think the worst spot is if half of it is execution, and half of it is Eth 1.0, right? I would do a full rename of the Discord, the repos, and I don't know about this other stuff.

**Micah Zoltu**
I agree that that is the worst spot is to have half and half. My concern is because there's different people in charge of each of those places and human coordination is hard, everybody is waiting for someone else to do it all at once. And no one actually is in a position to do it all at once.

**Tim Beiko**
I think Danny and me could get 95% to 99% of it done if we coordinate.

**Micah Zoltu**  
I don't know what I would have to do to convince Danny and you to sit in a room and just rename a bunch of stuff for a day.

**Tim Beiko**
I think to convince me is to wait until London is shipped. That's my biggest concern.

**Micah Zoltu**  
I'll say this. I'll agree to lay off until London is shipped, but you have to recognize that as soon as London ships, I will be on your ass, like daily. That's the trade you're making here.

**Tim Beiko**
I can live with that. So we call it Eth 1.0 APIs for now. It'll live under that name for six weeks. And then it will have a renaming. That's fine for me.

**Alita Moore**

What are you renaming it to?

**Micah Zoltu**
Don't ask that question yet.

**Tim Beiko**
That's Micah's job.

**Micah Zoltu**
Right? I would be fine with Execution API.

**Tim Beiko**
If we rename everything Execution, I'm fine with swapping Eth 1.0 for Execution everywhere, basically. That's generally okay.

**Micah Zoltu**
That's my preference. And that seems to be the direction that's getting the most traction of all the options available.

**Tim Beiko**
Okay, so I'll ask to create Eth 1.0 APIs today. Ping me after London, and I promise I will make this a priority and I'll also ping Danny and try to get it a priority on his list, too. Okay, so I'll ping the DevOps team to open it today. I don't think I can create a new repo in the ethereum org. Nope. I just checked, I cannot.

**ECH - Pooja**
One more thing on a similar note, maybe Micah, you can help me understand, I saw some messages related to some admin issues that you were not able to solve, and you were looking for some help. Is that being resolved? Or do you still need some help on that?

**Micah Zoltu**
No, I still need to deal with that. So I don't know who the admins of the EIPs repo are, but there's someone who is spamming it. And normally, I report them to GitHub and GitHub bans them. Unfortunately, this person realized that, hey, if I just pay GitHub $5, they will let me spam infinitely and will never ban me.

**Tim Beiko**
Can an Ethereum admin ban them?

**Micah Zoltu**
Yeah, so an Ethereum admin can ban them from the Ethereum org, so they can stop spamming us, at leas. They can still continue spamming the rest of GitHub, but at least we'll stop spamming us.

**Tim Beiko**
Okay, yeah, just get me their handle and I can get that resolved, too.

**Micah Zoltu**
Okay.

**ECH - Pooja**
All right. So I'm just wondering, is it possible to get some kind of access to at least editors, like Micah and lightclient to be handling these issues?

**Tim Beiko**
Yeah, I guess the short answer is, it depends. The long answer is if there's a specific ask that's easier, like so you know, making lightclient an admin for JSON RPC, that was a pretty specific request. And I think we're able to do it. I managed to get some guy admin for the yellow paper, too, who's done a bunch of PRs to it. So I think, in general if there's a specific reason and a specific history of contributing to the thing with high quality, it's fine. But there's no process, unfortunately. I said that to the DevOps people and I write to GutHub to get a good enough description of why I think it makes sense. And if people are content with that, it tends to get approved.

**Micah Zoltu**
So in this case, I don't actually need admin access. I just need to know who the right people to talk to are when this happens. It's happen like once before as well.  So

**Tim Beiko**
Yeah, I'm happy to act as a router in those cases. Jamie Pitts is probably the best person from the EF if you want to go direct, but he he does get a lot of like random inbound. So if he doesn't answer, it's kind of my job to answer the random inbound, whereas his job is to actually do DevOps stuff.

**Micah Zoltu**  50:30
I see. I'm sorry.

**Tim Beiko**
No, but yeah, ping me or Jamie if you want to go directly, but I can make sure that Jamie sees it eventually.

**ECH - Pooja**
Okay. Sounds good. All right.

#6. [Progress on 'canonical source for EIPs' WIP doc](https://youtu.be/VgsK8xnrL3U?t=3049)

So we are almost at the last agenda item about canonical source for EIPs. Brent, do you have any update on that?

**Brent Allsop**
Yeah, I haven't had time to even look at this, especially since I've been offline on vacation over the last week at Lake Powell. So sorry about that.

**ECH - Pooja** 51:07
No worries. We are almost out of time, but I can quickly go through the last meeting notes. I'm sorry, the link is missing here. I'm sharing here in the chat.

#7. [Review action items from the previous meeting](https://youtu.be/VgsK8xnrL3U?t=3079)

So according to this, there were a couple of action items. For me, creating the Discord channel for new EIP editors and have the conversation of onboarding and whatever they need to do or direction they need can be discussed over there, the channel is created now. It is on ECH Discord.

Pooja to create an issue for EIP bot to get updated. Okay, so we have this issue created. Anyone who is willing to get more engaged and help out with the kind of development of this new bot, this new script to identify the proposals which needs to go into the right status. The issue is available on EIPIP GitHub repository.

Alita to work with Micah to close EIP bot development issue. And this does seem to be closed now. So we are all good. That's all from the items listed on the agenda today. Anyone want to bring up anything?

**Trenton Van Epps**
Yeah, I just wanted to mention, I brought this up maybe a month ago to Jamie. But it looks like it's come up again in the Cat Herders about people going into Gitter, and nobody's really there. So I'm going to try and get those deprecated if we can and just direct people into the Ethereum R&D Discord instead. But it's cool. It looks like somebody is already finding where they're linked in documentation. Does anybody have any thoughts on this?

**ECH - Pooja** 53:06
Right? So someone pointed it out, but he specifically pointed out that wherever the Cat Herders Gitter was mentioned. So we are trying to fix it for Discord channel over there.

**Trenton Van Epps**
Gotcha. Yeah, just just generally, I think it's probably a larger problem outside of Cat Herders documentation. Right. So it seems like Jamie is the person to contact for this, but I'll try to reach out to him.

**ECH - Pooja**
Right. So yeah, we will continue discussing in different channels that we have mentioned today about the EIP process and the JSON RPC API processes and other stuff. Thank you all for joining today. You all have a good one.

# Attendees

* Alita Moore
* Brent Allsop
* ECH - Pooja (Host)
* Edson Ayllon
* Hudson Jameson
* Jared Doro
* Jim Bennett
* Micah Zoltu
* Tim Beiko
* Trenton Van Epps




# Date for Next Meeting: June 30 at 1500 UTC
