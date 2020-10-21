# EIPIP Meeting 18 Notes
### Meeting Date/Time: Thursday 8 October at 14:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/34)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=pscnoPt_4ko&t=4s)
### Moderator: Pooja Ranjan
### Notes: Jim Bennett

----

## DECISION ITEMS

**DECISION 18.1**:  Leave EIP-1 as Active and don't change state, but leave arrows.

**DECISION 18.2**: Final EIPs can close their issues if they've marked a discussion to as an issue.

## ACTION ITEMS

**ACTION 18.1**: lightclient has secured @EIPinfo for tweeting EIP updates. Cat Herders, James Hancock, lighclient, and Matt will all work together to start tweeting.

**ACTION 18.2**: Add item to agenda for EIPIP Meeting #19 - "Should the meta and information EIP not be part of the EIP at all?"

**ACTION 18.3** Pooja will reach out to EIP authors to get them to follow the documented network upgrade process.

**ACTION 18.4** Micah reached out to Aragon to tell them they need to put in content to EIP 3000 to discourage squatting.

**ACTION 18.5**: Move agenda items 4-6 from this meeting to the next meeting on October 21, 2020.


## AGENDA

## 1. [EIP standardization process (PR to EIP-1) and Network upgrade process](https://youtu.be/pscnoPt_4ko?t=16)

**Pooja Ranjan**
Welcome, everyone. This is EIPIP meeting 18. I'm sharing [the agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/34) in the chat. So the first topic for today's discussion is the EIP standardization process [(Pr to EIP-1)](https://www.youtube.com/watch?v=pscnoPt_4ko&t=4s)and network upgrade process. So this PR is created by James. Anyone have any update on that? I have also added some comments. I see lightclient and Micah also have added there. So, James, would you like to take over and let us know more about it?

**James Hancock**
It's there. I don't know what the next steps are. I responded to most of them. I guess I haven't, in the last couple days, looked. So there might be ones that I haven't responded to. If there's comments or stuff you all have about, I'd be happy to discuss.

**Micah**
I think the next step is to merge.

**Pooja Ranjan**
Okay, there is just one last comment I added to the pull request there. I just have requested to remove the word "Accepted" there in the comment section. I'm not sure if that is appropriate or not. But if it is, after that. And another thing that I wanted to discuss was on the part of the living status. So for living status, I see some communication on whether it should be one sided or two sided and the status. So it was wondering what would be the ideal situation to consider it, because EIP-1 is going to be under review all the time, but changing the status, is it something that is visible and should be considered or the status should be "living but we will be considering the changes?""

**James Hancock**
My thoughts for that was for EIP-1 going back to review doesn't make sense. Because then we have EIP-1 no longer active looking, which is kind of strange. But I didn't feel too strongly about having the both arrows be possible.

I guess I'll start with the intention of why I had the arrows back and forth. Because I'd like for some way for people to subscribe to changes that are happening to living EIPs. So there are people that are going to want to know what's happening to EIP-1 and aren't going to care about what's happening to many other EIPs or just leaving the EIPS in general. Currently, we have an RSS feed for Last Call. But it would be great to have an RSS feed for all EIPS. So whenever there's a change in state, people can subscribe to that state.

**lightclient**
Are people using the RSS feed?

**James Hancock**
Yes.

**lightclient**
How many people are using the RSS feed?

**James Hancock**
I don't know. I think you can get that from the EIP repo. But you have to have permissions to see it.

**Micah**
I think the answer is like one or two.

**lightclient**
Yeah, seems like a lot of work to improve the experience for one or two people who are using the feed. There are better avenues to alert people with changes of EIPs. I'm not sure optimizing for RSS is the best avenue for that.

**James Hancock**
With an RSS feed, it'd be easy to put a bot, like a Twitter bot or other things. And it's actually easy to implement with GitHub, to have an RSS feed be a thing. We just haven't had someone do it. So yeah, it maybe it's not an RSS feed, that's also fine. I do think we should have some way of people being able to subscribe or see that these changes are happening.

**lightclient**
Agreed.

**James Hancock**
People are gonna care about what's happening to EIP-1. And they shouldn't have to go and look at EIP-1 every week just to see if something's changed and look through all the different PRs. We should make that fairly easy and transparent that stuff is happening there. So whether it's RSS feed or some other way, that's fine. When I had thought about the going back between Review and Active, if it changed state, then the RSS feed would show that. But that's relying on a weird, weird part of the process, a nuance of whatever to achieve a goal rather than just have the goal and then achieve it the best way possible. Which that was brought up by, I think, Micah on the PR.

So I agree with that. But there's probably better ways to do that. And in the case, for EIP-1, moving it into Review would make it look like it's no longer Active. And so that would kind of be strange that there would be no appearance of no EIP-1 Active at a time. And so it should stay. But as far as if there are living EIPs that want to go back and forth, I haven't thought about it enough to really say that they should or shouldn't. And so that's kind of where I got. I didn't feel too strongly we needed to force that there is only one state change here, given that we just don't know a lot about living EIPs. That's something that we can figure out as we go along down the road.

**Pooja Ranjan**
So considering if we have EIP-1 only for now, like as we have only one, do we consider the change of a state, or do we just agree that it has to be living only and we will be doing the reviews? Because as you mentioned, if we change the status, people will have some kind of confusion.

**James Hancock**
Yeah, so for EIP-1, we shouldn't change the status to Review. But I don't know if that means we shouldn't have an arrow. Because before, we were going to have meta EIPs that were in a living state, but a lot of those meta EIPs, the registry ones are kind of moving into the Eth1 specifications repo. So I don't know if there will be another living EIP out of the meta ones that exist.

**lightclient**
Yeah, I would rather see living EIPs be documented in another way. Like, obviously, EIP-1 is special, and it's unlikely that we can change that. But I think that generally when we run into a time where we want to continue updating EIPs, it would make more sense to do those updates out of hand, and maybe define the process for updating and where those updates happen as an EIP. And that can be static. The network upgrades is obviously a good example of that.

**Micah**
Do we have any ideas of what else besides EIP-1 makes sense as living in the EIPs repo, especially now that we've split out the network upgrade stuff?

**James Hancock**
I haven't really deep dove into it since we have done the splitting most things into network upgrades.

**Micah**
My tentative feelings on the matter is until we have another a second example of a living EIP, we don't spend too much time worrying about what the process for EIP-1 is, since it will only affect EIP-1 which only affects the people in this channel right now. As far as I can tell, no users actually read that.

**Pooja Ranjan**
Yeah. So I'm also in favor of having it for EIP-1 at this point of time, because we cannot foresee what is coming up for any other future living documents, but if it will, then maybe considering the status change would matter.

Okay, so talking about the process part. The second part of the first item is the network upgrade process.

**James Hancock**
Let's let's actually just have a decision on that. Is it okay to leave it as arrow goes both ways, and we don't really take time to figure out the nuances until there's a reason to, or do we have the arrow be one way and figure it out?

**Micah**
All I care about is I don't want to see the status of EIP-1 go back to not active, or living, or whatever it is. I don't care what the graphics looks like or anything, since it's just EIP-1. And there's, like, six people that need to care about the status of EIP-1. And it's flow through the process. So I'm not too worried about being super formal about it.

**Pooja Ranjan**
It's my personal opinion here, because we are talking about standardization process. And every time the arrow points, it states that the proposal in that category is going to change the status. So let's have the arrow one way, but while documenting what a living document is, we can mention it clearly that it is a living document, it will be under review all the time, but the status is going to be living. Is it something that is considerable?

**James Hancock**
It seems like we don't really need to necessarily limit it. The arrow in the document literally sits on the diagram.  I can change that. And then if someone was some way to do that later, they'll just have to make an EIP to make it so it can be possible to go do a review again.

**Pooja Ranjan**
Sounds good. Does anyone have objection to this?

**Micah**
Just real quickly, earlier, James, you indicated that the reason you wanted the arrow to go the other direction was so people get notified. You have any idea of who the people that might want to be notified on the EIP-1 changes, or besides the six of us that actually care?

**James Hancock**
For EIP-1, there is a lot. For example, the change that "Accepted" is no longer a status is pretty huge to the community. In the day-to-day stuff, there are people who are working on EIPS, and that's kind of a small group of people. And then there's us who work on the process of EIPs, which is even a smaller group of people. But as far as the definition for how standards work, who are the EIP editors, what and how the EIP repo works and those things, there are a lot of people who care a lot about it. They just don't look at it very much. And changes to those things are quite big.

It'll be easier post (i.e. after) this. So perhaps it's less of a thing moving forward. But previously, it was basically the Constitution of how to do Ethereum stuff. They don't care about it until suddenly everybody does. And changes to it can have pretty far-reaching effects. A good example is the splitting of the network upgrade process. And the standardization process actually has pretty big far-reaching effects for the community and decision makers within them. More people would care about EIP-1 than any other EIP in the EIP repo.

**Micah**
So I suspect that all those people are not subscribed to the RSS feed. Do we know how to reach those people? Is the best mechanism to just tweak? What is the means of actually getting in touch with all these stakeholders?

**James Hancock**
If there was an RSS feed, if there were a Twitter account that tweeted the RSS feed, that'd be the easiest way to get that information to the people who care about it, because then they could just subscribe.

**Micah**
Given this is just EIP-1 and the changes to it are pretty infrequent, I wonder if we can just avoid the automation for now and just have someone here tweet major updates on some well-defined accounts like @EIP.

**Pooja Ranjan**
Yeah, I think that is a good idea since this EIPIP working process improvement part and looking into it, so one of the EIPIP group members can do that, or maybe from the Cat Herders official account. If people would want, we can go ahead and do that, because we do not have any official Twitter for EIPIP. So we can do that, if that's okay with everyone here.

**James Hancock**
Like an @EIPupdates. That'd be a nice Twitter account to have for people to follow.

**Pooja Ranjan**
Yeah, right. So most of the EIPs would be under the process of either standardization or maybe for the network upgrade. I'm not sure if any of the EIP editor would like to volunteer to handle that Twitter account separately? Or is it something that anyone from the group is interested to do that? Because I'm not sure Cat Herders would be qualified to handle the EIP Twitter, because most of them are not EIP editors, so not sure how people are going to receive it.

**James Hancock**
I can just start tweeting them for now until we figure out if there's a better way to do it.

**Pooja Ranjan**
Yeah, I'm perfectly fine with that. Because you being hard fork coordinator, if you start tweeting about EIPs, and especially EIPs, which are related to network upgrade, it's fine. Any other thoughts on that?

**Brent Allsop**
Would that be something that would make sense to have the Cat Herders own that and use the Cat Herders email as the owner of that?

**James Hancock**
Cat Herders can certainly own it, and either they or whoever they want to consult with can help figure out what should be tweeted. I don't know if it should come from the Cat Herders account because people don't know that Cat Herders are EIP updates.

**Brent Allsop**
Makes sense.

**James Hancock**
It may make sense to have its own venue, so people know what they're subscribing for.Oh, @EIPbot is available. Yeah, you should just get that, lightclient. No, let's use it. And then we can coordinate EIPs from it. And with Cat Herders and lightclient, perhaps you can help, too.

**Pooja Ranjan**
Cool, we can note it down as an Action Item. Today, we will be creating a Twitter account for tweeting about EIP status updates and the Cat Herders, the hard fork coordinator, and lightclient, Matt, all of us will be looking forward to start tweeting about it.

**James Hancock**
Yep.

**Pooja Ranjan**
Moving on, the next part was [network upgrade process - process flow.](https://youtu.be/pscnoPt_4ko?t=1109). So the process that we have been discussing, and James and I have tried to work together and document it in a proposal. But the confusion part was, should this proposal be a part of EIP or not? I had some comments there. Going by the current process, I personally feel that it should be a part of meta EIP where we are mentioning the process for network upgrade process. But we would like to hear other thoughts on it.

**Micah**
Broken-Record Micah thinks that EIPs should only be technical standards. For sure you guys all know  my feelings at this point, so I won't go into details, unless someone wants to hear them again.

**Pooja Ranjan**
Right. About that. If people are comfortable, I'm going to put that as a specific agenda item in the next meeting about should the meta and information EIPs not be part of the EIP at all? Because they are clearly defined. They are process, and that is process around Ethereum, but that is not bringing any change to the network itself. So I find that if people are looking for only technical specifications, we have a special category of that standard track EIP. So we can look into that. And I was also looking into the numbers of informational and meta EIPs so far, I think we have very few - under 10 for information as well as for meta. For meta so far, we have only the number of upgrades or the number of metas. Because whatever is going into upgrades, we are just listing all those proposals into one bucket. And we named them as meta up until now. Because for process, we have EIP-1. Now we are separating the process of standardization as well as for networks. So I'm proposing to have another meta proposal for documenting the process. I don't think it's creating a lot of confusion because for technical specifications, we have a clear category.

**James Hancock**
So from the context of metas have a clear category and technical specifications have their own clear category, that those buckets exist with EIPS make sense. What I'd like to avoid is if we have the process for network upgrade processes being within an EIP, then we once again have EIP editors in the politics of what goes into the upgrade process.

**Pooja Ranjan**
I'm not so sure of that. The reason behind having it in an EIP in the first place, my argument was, whenever we change the process, we don't want to go back and change EIP-1 every time. It's just changing one EIP.

**James Hancock**
Yes, so I would say we don't even need it in EIP-1.

**Pooja Ranjan**
Yeah, that's exactly what I'm saying.

**James Hancock**
And we don't need to in the meta EIP either. We just have it in the network upgrade. We have this information in the Eth1 specs repo.

**Pooja Ranjan**
Yes, of course. So the point was when we are trying to reach to Eth1 spec repo, and the readme file there that is limited to this particular repository only. But when we put something on the EIP repo and then eips.ethereum.org, then it is accessible to everybody. But I do not have a super strong opinion on it.

**James Hancock**
Yeah. We can make a file, like in a hack MD file for the process, literally just take this meta EIP and put it on the specs repo, but remove the stuff, the EIP-specific formatting and information and just put it there and make it so it fits in its own file underneath network upgrade specification. As far as formatting and fitting and everything, if the concern is how do we make this visible because there isn't a website that shows the information, then we should figure that out separately and not use that it's convenient that EIPS are shown on EIPS.org. So we could plug into that system by having the network upgrade system use it. It's using what we currently have to do something that we should just do better anyway on its own.

And then we're not again tying the processes together, even indirectly. If someone goes to an EIP and then reads about the network upgrade process, they're getting tied. The worlds are once again coming together into one place, because edits to the process become an edit to an EIP, which then becomes an edit in the EIP repo, which then becomes the domain of EIP editors and then also the people that are there working on it. And that's pulling things together more than I think is appropriate. And any information about network upgrades should exist on the network upgrade spec repo. That's the purpose, to hold the information and the process, the current process and the definition of the process in one place and have it be in its own world. And if visibility of that is an issue, we should then solve that. We can make a website that is Ethereum network upgrades, and then put the information there.

**Pooja Ranjan**
If you have one such website, I think the bot thing that we are talking about would also make sense to have it there. The Twitter bot.

**James Hancock**
Well, the Twitter bot should be for EIPs. But having a Twitter bot for network upgrades also would be nice. But really, that's just me.

**Micah**
You are just a Twitter bot. Pretty advanced.

**James Hancock**
Pretty much I'm just a Twitter bot at this point. My rules have been defined; I just execute them.

**Pooja Ranjan**
Great. Okay.  So I'm gonna leave it just like that. And if it has to be converted into a hack MD file, I'm okay to do that. But again, as I mentioned, my concern would be what would be going into meta and informational? But let's keep it for some other discussion, some other time.

**James Hancock**
Yeah, for the general conversation of should have meta and should we have informational is separate. But I do think anything about network upgrades shouldn't be on the EIP repo. It should be in the network upgrade specification.

**Pooja Ranjan**
So one more thing before we move on from this. The other day, we were talking about different phases of the network upgrade process. So would you like to reiterate on that?

**James Hancock**
Is it something that group wants to go through right now?

**Pooja Ranjan**
There was one concern, which I think should be brought into the consideration for EIP editors. It was about the EIP status. And the network upgrade process is divided into three phases. And I was looking into EIP statuses, but I have seen historically, even if an EIP is deployed on the mainnet, the status does not change from Draft to any other. Sometimes it happens. So I was looking to enforce that.

**Micah**
Yeah, I have strong feelings about this. People very often create an EIP as a draft, and then think they're done, and they just walk away. And then hundreds of other people think, "Oh, this is an EIP, I should go with this,"" and they go implement it. It's not just for core EIPs. This happens to ERCs, basically all of them, which is why we have 3,000 drafts, and, you know, 10 final EIPs or whatever it is.

I don't know how to solve this. But it would be great if we can at least get the core developers to not implement or not put things on the mainnet until they're Final, especially with this new process. An EIP shouldn't be final before it touches mainnet, in my opinion. Or, rather, mainnet should not be putting non-final standards on to mainnet. That's a better way to put it.

**Pooja Ranjan**
Right. So that is what I wanted to specify here. Like when we are changing the category of CFI - CFI Applied, CFI Approved, CFI testnet/devnet waiting room, whenever we are changing the statuses, changing the bucket for any of the proposals, we should also consider the status at that point. Meaning whenever a proposal is getting in the bucket of CFI Applied, they can be in Draft status. And when it changes from CFI Applied to Approved, the status must be between Review to Final.

Okay, I'm just quickly going to [share this screen.](https://youtu.be/pscnoPt_4ko?t=1761)

**James Hancock**
Yeah, share the screen so people can see. And I also agree with Micah that an EIP shouldn't be on mainnet without being Final. I totally agree with that. The nuance to that I kind of want to address is who enforces it and how do we enforce it in a way that EIP and the network upgrade process isn't getting tied again.

**Micah**
Ideally, we can work with the CoreDevs since that's a relatively small group of people. And we can hopefully convince them that this is for the betterment of the ecosystem as a whole if they would stop putting Drafts on to mainnet. Really, all it takes is just someone sitting down and submitting a PR that moves it to Final or Last Call and Final. The champion just needs to do those extra steps. I think for most cases, it's that no one is doing those steps. So my hope would be that we can simply talk to the CoreDevs and convince them that it would really help everything if you guys would set a good example here. And when you're ready to put something on mainnet, take those steps. Have whoever the champion is do the three things they need to do in order to get it on the mainnet. We can avoid anything formal or official, because we're working with just this one group.

**James Hancock**
Yeah, that would be nice. And I would like the decision to be in the hands of the CoreDevs, or the people doing the network upgrade stuff. I wouldn't want the decision to be on EIP editors to enforce that. Or even make it have to do something.

**Micah**
As I said before, I think the the direction of the arrow should be that network upgrade points at EIPS; EIPS effectively don't know that the network upgrade process exists. From a programming standpoint, it would be, have a pointer to from network upgrades to the EIPS repo. The EIPS repo does not have a pointer back to network upgrades.

**James Hancock**
Yep.

**Micah**
Again, as an editor, I don't actually know this exists. But as a user of Ethereum, I think those are fine.

**Pooja Ranjan**
Yeah, as we were mentioning right now, we would want to enforce this. We would like people to adopt it.

**James Hancock**
What we had said earlier is that we don't want to enforce it from the EIP side.

**Pooja Ranjan**
From the network upgrade side, I understand. But I think since we are defining everything... Okay, do you want it to be added as a recommendation?

**Micah**
Who is the network upgrade group? Is there a similar network upgrade group like this one?

**Pooja Ranjan**
Not really, I think James Hancock is pretty much it.

**James Hancock**
Pretty much just me.

**Micah**
James is the group.

**Pooja Ranjan**
Yeah, right.

**Micah**
So, James, the editors would like it if you enforce this over on your side.

**James Hancock**
Yeah, and that's what I mean. I like that it exists as a rule. But I think the enforcement shouldn't exist on the EIP editors, or even defined on the EIP side. It should be in the specifications for the repo and up to the authors and the people like me to make sure that that it's enforced.

It's tempting to make an official EIP standard that only EIPs that are Final go into mainnet and have that exist on the EIP repo, because that would be a sort of easy way to enforce this. But it would put the decision into the EIP editor's hands, and the EIPIP meeting people, or in general, the EIP stuff. The decision is on the other side of the fence. And we want to make sure that that decision is on the network upgrade side of the fence and it stays over there. And so far, because it's just me, and then the CoreDevs, it's easy for me just to tell them, "Hey, this EIP needs to be Final before moving into mainnet." And they say, "Okay."

**Pooja Ranjan**
Cool. In that case, at least we agree to document it. And we'll see in the process how it turns out.

**James Hancock**
Yeah, it can be documented in the network upgrade stuff. And I really just want to be very, very careful about when we decide that something should be done, we should also decide who is it that enforces those decisions, and does it fit with the paradigm that we're moving forward with.

**Pooja Ranjan**
Here's a suggestion. For the network upgrade process, most of the time Cat Herders are helping with some or the other activities reaching out to the authors for some of the other tasks. So if it is appropriate, and if it can be considered under the boundaries of Cat Herders, we can certainly reach out to the authors requesting to change the status, citing this document, that this is the new process, we are trying to follow the process. And according to this process, you're supposed to do that. We are not enforcing; we are just passing information for the first few upgrades, and then maybe eventually people will be in a practice of doing it. So that might help in the long run.

**James Hancock**
Yeah.

**Pooja Ranjan**
Okay, so I'll be happy to reach out to the EIP authors which is considered for this particular upgrade. And we'll let them know. But before that, we have to have it documented in the network upgrade repository or somewhere else wherever.

One thing before we move on, I wanted to clarify here -  the proposals which get into this process but are not moving forward. For example, there was a EIP 2046, which is listed as a CI devnet waiting room. My fear and understanding is that may not go ahead. How are we going to take out those kind of proposals out of this system? Should we have a bucket of rejected or withdrawn? Or what?

**Micah**
Did you say 2046?

**Pooja Ranjan**
Yeah.

**Micah**
Okay. I got it.

**Pooja Ranjan**
Okay. So I was looking for that specific bucket, because that was there in the earlier process when we had network upgrade and EIP standardization together, we had this bucket of rejected EIPs, and that we took off from the standardization, citing that it would be a part of network upgrade. But we don't see it anywhere here. But we certainly need that in the standardization process.

**James Hancock**
Yeah, I don't know. We probably need it at some point. Today, I don't think we need it. Even the EIP you mentioned, we had talked a bit about this last week. The philosophy I've had when designing the system is that, sure, there are many more things to be added or things that could be added. But I want to add them as they come up, so we have a sense of emergent properties that are around the system.

We're building a system that's never really existed before. There isn't really a playbook on how to upgrade a multi-thousand distributed network of computers with lots of different parties. There isn't a project management book that describes how well to do this. So because we're working in new territory, I want to avoid deciding in advance how things should be and then shaping them to that shape. And instead, as we move forward, see the shapes that appear and have the process fit to it. So the CFI and the DevNets and all those things are examples of stuff that arose organically as we were moving forward, as the natural next step in this process. If in the beginning, I sat down and wrote out a network upgrade process, it wouldn't be what this is today. It would have been something else based on my imagination of how things should go, based on who knows what because there isn't anything really to piggyback off. So at some point, there will be a need to have a rejection bucket. But I would not want to define what it is or how it gets there until we have an EIP that needs to have it happen.

**Brent Allsop**
Sounds brilliant.

**James Hancock**
And the EIP you mentioned, it is "technically" superseded by another one going into mainnet, because if that goes in, then we don't need to have that one. But at this state, the EIP that would supersede it also isn't in mainnet. So it hasn't kicked the other one out of the process, because technically at this point, we could switch our decision and have it so the one that's waiting back - 2089, I don't member the numbers - but the gas change costs for that EIP, we could change our mind and do that one instead. And then the other one would be rejected, or whatever happens. So because there hasn't been a decision that kicks it out, I don't think we should build the process for kicking it out yet.It's fine just to sit in the waiting room. Or as EFI.

**Pooja Ranjan**
Yeah, I mean, that's fine. We will come with the more buckets, as you mentioned, for rejection for the proceeding, we'll look into it. And I'm fine with that. Before we move on, thanks to lightclient, we have secured a Twitter for @EIPinfo, Twitter @EIPinfo, that we will be using for a status change of EIPs.

**James Hancock**
Cool.

## 2. [Discussion issues of Final EIP](https://youtu.be/pscnoPt_4ko?t=2473)

**Pooja Ranjan**
Okay, so the next item is [Discussion issues](https://github.com/ethereum-cat-herders/EIPIP/issues/33#issuecomment-699769553) of Final EIP. I think this was mentioned by Micah about a particular EIP. They have created an issue, but after the EIP went into Final, they closed it. Micah?

**Micah**
Yeah. So we encourage people to use either GitHub issues or Ethereum Magicians for discussion to links on EIPs. The question is just should those remain open and active forever? With Ethereum Magicians, it doesn't really matter too much. They kind of just disappear over time, just how forums work. With GitHub issues, though, we have an ever growing list of open issues. That doesn't really hurt anything per se. It just means the search results become harder and harder to get useful results out of. Someone came along and said, "Oh, this EIP is Final, so it makes sense to close the discussion link." And that got me thinking. Historically, we have not done that. And so I reopened the issues, because that is not our general process. But it did get me thinking, is that a good process? Should we do that? Does it make sense to continue discussion on an EIP that's already been marked as Final and the author is now long gone? You can't change it.

**James Hancock**
The discussion, too, was an issue. And it being closed..

**Micah**
Yeah, it was a GitHub issue. And so the author came by and closed the GitHub issue. And again, I said I reopened it, because we normally don't do that. But that was a very reasonable thing to do. And I'm wondering, do we want to do that?

**James Hancock**
That doesn't remove an issue? It doesn't delete it. It's still there. Just not open? So someone could always go back and say, "Hey, we should talk about this again."

**Micah**
Yeah, it just basically removes it from the open list. And it means when you search, it's a little easier to find things because you can filter out Closed. It's pretty minor either way.

**James Hancock**
Would the link still exist? If they clicked on the discussion to link, it would take them to the discussion, and they could read through it all, and then see that it's Closed? But then still see it all?

**Micah**
Yeah.

**Pooja Ranjan**
In my mind, we should encourage people to go and do that with EthMagicians only, because the example that you have cited, I see that that is a recent proposal that was created. But I think if people have done it, if a PR is open for a very long time, the EIP is in process for a very long time, I understand the issue of having it discussion to section the issue, but from here on, we should try to encourage people to get it in at EthMagician, and I think it totally makes sense that we should close it. We want to have the least number of open issues so that it can be addressed and finally closed.

**James Hancock**
I agree. Closing it makes sense. Letting them close the issue, and then as long as it's findable still by the link and the content isn't gone, then it can be reopened if whatever happens. And I feel less strongly about enforcing it being on either one. I think it should be up to authors, but closing it makes sense.

**Micah**
I think the context for why we still allow people to GitHub issues is because EthMagicians does require a second account. And we want to enable people to only need a GitHub account to participate in the EIP process and not have to go create accounts everywhere. Especially since EthMagicians requires an email address, I don't know if GitHub does or not. But if you're trying to remain anonymous, which we want to encourage, it's easier the fewer accounts you have to go create at random places. I believe that was the original attempt with still allowing GitHub issues.

**Pooja Ranjan**
I think that the pull request itself, they are getting a place in the EIP repo to discuss that proposal.

**Micah**
We have a rule that says you cannot use that for you. It has to be an EthMagicians or GitHub issue.

**Pooja Ranjan**
Yeah, I also find EthMagicians to be the best place, because that was originally created to discuss all kinds of proposals.

**Micah**
I agree.

**James Hancock**
Certainly the best place. I don't feel like we should limit authors to only do that. I guess we're kind of getting on a tangent here. As far as should the issue be closed or not? \

**Micah**
I think we're in agreement to close. I'm good with that.

**James Hancock**
Yeah, so then we're okay with closing Final EIPs? And then does anyone else have thoughts on that? So we can make that a decision?

**Pooja Ranjan**
Sounds like we have a decision.

**James Hancock**
Yep. Yeah.

**James Hancock**
Okay, so that one, we can record. Final EIPs can close their issues, if they've marked a discussion to as an issue. So then the next the next part of the conversation started into should we enforce only one or the other or not or the other. So we can get back into that if we'd like.

**Pooja Ranjan**
Yeah, sure.

## 3. [EIP number squatting](https://youtu.be/pscnoPt_4ko?t=2821)

So moving on, the next item is [EIP number squatting](https://github.com/ethereum-cat-herders/EIPIP/issues/34#issuecomment-701148693). So this was brought into attention by Micah.

**James Hancock**
Alex has brought this to attention before, too, I would want to nring that up, too.

**Pooja Ranjan**
I wasn't aware. I just read Micah's comments.

**James Hancock**
Months ago, Alex has brought this up as well.

**Pooja Ranjan**
Okay, so what is the general thought here? Micah, would you like to explain the situation?

**Micah**
So the situation is people know how the editors choose EIP numbers. Technically, the editor chooses whatever number they want, they assign it. But people have figured out our secret formula, which is to just use the PR number. And so when they want to have a particularly cool number, like 3000, or 2000, or 1337, or 777, or whatever it is, they have learned to do one of two things. Either they just set up a bot or something and wait for an EIP number to be next, and then immediately go create new EIP, or worse, they come in and just create a bunch of trash issues just to force the number up until it gets to them when they want, and they squat on that one.

In the past, we have tentatively tried to frown on this, but we haven't actively done anything to stop it. The question here is, we have a situation where someone is doing exactly this. They saw that 3000 was coming up, and they waited until 2999 was used. And then a few minutes later, they created an EIP which, of course, got them 3000. Or at least their PR number was 3000. As editors, we have the authority to just simply give them a different number if we want, since the process is that the editor will assign you a number. And so the question is, should we exercise that power and give them some other number? Or should we allow them to have successfully squatted? My personal feelings is if we allow them to squat, it encourages people to do the same thing in the future. It's one of those things where the situation can escalate. And I would rather nip it in the bud and just say, "Hey, if we even think you're trying to squat, we're gonna give you a different number that you don't like."

**Pooja Ranjan**
I think this is something that most of the editors can answer. But if I have to go by my personal opinion, since we have not done that in past, we could let it go for one time, making it as a note, and then highlighting this issue to be in the future to be lesson learned kind of stuff. And if something is there, we are going to be more strict about it. But that's my personal opinion.

**Micah**
I believe there was one situation in the past where we actually didn't allow the squatting. In this particular situation, if I remember correctly, it was a while ago, someone was actually creating a bunch of issues to bump the number up. And then we closed their PR on them once they got the number they wanted. We said, "no." That that was a little more aggressive. This time around, it's a little more passive. And so I don't know if we want to be as harsh. We do have at least one instance of precedence of shutting down squatting. I don't know if that's enough to do it again.

**James Hancock**
So if someone just waits for a number, and then has an EIP, and they write it... So in this case, did they just get the PR and then write the EIP later?

**Micah**
Yeah, they grabbed the number, and it was TBD on every section. They had had a title, I think, and that was it. If I remember correctly, they might have updated it by now. I'll check. But at the time, they had a title and the frontmatter, and that was it. They had no content yet. And they're like, "Oh, we have a plan." It's actually still there. So yeah, they have title, author, discussion to. Which is actually wrong. Discussion tois actually the pull request. So feedback that if we keep it open, and then TBD for everything else.

**James Hancock**
Yeah, in that case, I would say if someone had an EIP, and they waited, I guess the appropriate cases, if someone wants a number, and they write an EIP, and it has content, and then they just wait, and then they do it, cool, good on them. But if they do this, where it's literally just they have the least amount of work possible to keep the number, then I would agree with just saying sorry, you don't get it.

**lightclient**
Well, it looks like they've got a project with some code and contracts and reference implementation. So it looks like they're progressing towards writing it as a spec. My feeling is that the editor should come in and say, "Hey, we have complete control over the numbers. And so you did this, but that is no [unclear](https://youtu.be/pscnoPt_4ko?t=3139) in the future you're gonna get this. But I mean, this is this is Aragon, this isn't like some random group that has some random EIP. I think of all people to get the 3000th EIP, this is not the worst. I don't know, I don't really think it's that big of a problem. If it becomes a problem, then the editors can start assigning numbers, but no one's upset about this.

**James Hancock**
If they made a bunch of issues, which has happened a couple of times, and then to get to the right number, then for sure, I think that's a far enough that we say sorry, you've just bloated the EIP number issues for no reason, so you're not going to get what you wanted. In this case, it's kind of less clear to me that they're doing that. If they went like a week and nothing had happened, then it would feel more like squatting versus just developing. I don't know.

**Pooja Ranjan**
I'm not sure if they have bumped a number. It's just minutes after that this PR was opened. And they have also populated it with codes now.

**lightclient**
It looks like they legitimately pulled it at 3000, because the one before it, 2999, is legit.

**Micah**
I believe them in this case that they really did just wait. I'm guessing they set up like a GitHub bot to watch and then to just ping somebody when 2999 showed up and then that person and the human came along and just the made a new PR, copied the template, deleted the comments, and hit submit. It's why it took 10 minutes. So I don't think they were doing the malicious bumping. And so maybe it sounds like the general feeling is that if we believe you are causing problems like generating garbage PRs or issues, then we will stop you. If you, on the other hand, just wait and fight with other people for that number and you win, then we'll let you have it. Does that sounds right?

**Pooja Ranjan**
I think that can be recorded as well for future reference.

**Micah**
Okay. I don't know if we want to make this an official policy, I would still like to retain the power to deny numbers in the future.

**lightclient**
Yeah, I agree with that.

**James Hancock**
I also agree.

**Micah**
Unofficial policy I'm okay with. A kind of operating procedure for us internally.

**Pooja Ranjan**
I think would be helpful for usto cite some example mentioning that this is something not acceptable if such a scenario comes in the future, but definitely this is under the purview of editors. So I'm not sure if that can be a policy, just one reference point I was mentioning.

**James Hancock**
Gotcha.

**Micah**
I'm good with this, really. I'm satisfied.

**Pooja Ranjan**
Okay. Anyone has any more comment on it?

**Micah**
Since we're already talking about it, so I don't have to bring this up again, do we have a feeling like if they never actually fill in that EIP? Will there be a point in time where we say, okay, yeah, this is not okay, or are we gonna let them have 3000 forever?

**James Hancock**
Yes, if they didn't within a couple days start doing something with it, then it's then then it was "oh, we just placeholded it to come back to in, like, four weeks or something." And that's also kind of the appropriate time to tell them sorry, you don't get that number. You clearly waited six weeks to do this.

**Micah**
That is currently the situation. It's been about a week and the EIP is still just empty. So the question is how long do we wait before we take away this number from them if we want to do that? Or do we just say, no, take your time. And I'll come back in a year and get your EIP 3000, go for it.

**lightclient**
I think a year is too long. But I think, like, three months, if they don't have an EIP to publish in three months, then...

**James Hancock**
No, no, three months is even too long. It doesn't even need to be an EIP. It could be all they need is a simple summary and the abstract.

**lightclient**
I mean, they have done quite a bit of work. They've registered all these sites around this EIP number, and they've already come up with some implementation of their EIP. If that's the minimum, we should let them know, because I think they'll do it. They have all this information. They're obviously continuing to progress on it. It's not a case where somebody decided they want EIP 3000 and then they just fall off the map. I think that this is definitely going to happen with very little chance it doesn't.

**Pooja Ranjan**
If they don't do it within that time timeframe, it is going to be in stagnant [unclear](https://youtu.be/pscnoPt_4ko?t=3475).

**James Hancock**
Yeah, but thinking about it, just the general case, if it's two to three weeks, and nothing's happened with the EIP, then they didn't have content when they made the EIP. The ideal case is someone sits down, they write some stuff, doesn't need to be everything, but they at least have some of the basic things. And then they hit submit an issue and then boom, they submit, they make a PR, the PR gives them an issue. And then that's their number. Certainly they have the standard and all that stuff already written out or developed. But in the case where they made the number and then came back three weeks later to write those things, that gets further and further from what we want, which is just people to make PRs when they have something to PR. So we should tell them, hey, put stuff in or we're going to give you a new number. Okay. And and the new number probably should be the most recent issue number available kind of a thing.
4
**Micah**
Sure, we can do that. We also have a bunch of numbers that were never used. Like when you get those spammers that come on and create issues in your repo then we immediately delete the issue. Those numbers can be reused if you want. Like any numbers. We've got lots of extras.

**Pooja Ranjan**
So we are out of time here, but I think we made good progress here. And we have few decisions on the topics. There is a tree adding permission if you have anything quickly to go over that, is it something that we need to carry in the next agenda? Or is it something that is done? Lightclient? If you can let us know about it?
2
**James Hancock**
So someone's gonna reach out to the Aragon guys and tell them that if they need to put in content so we can discourage squatting?

**Micah**
I'm doing that right now.

**James Hancock**
Okay, cool.

**Pooja Ranjan**
Okay, so I just wanted to quickly check if the next item should be on the agenda for the next meeting, EIP triaging permission, or is it something that we can remove now? I think we made good progress last meeting.

**lightclient**
Is lightclient in the list and have permissions to do it?

**lightclient**
I don't think I am at the moment.

**lightclient**
Yes. So we're not done yet.

**Pooja Ranjan**
Okay, so we could not even touch comments on that. And I know we are running out of time. So I'm gonna move the items which we could not touch to this meeting to the next meeting. Thank you everyone, for joining us today. I hope you guys have a good day, night, evening. See you all in next two weeks on October 21. Thank you everyone for joining.


# Attendees

* Alita Moore
* Artem Vorotnikov
* Brent Allsop
* Chloethedev.eth
* Edson Ayllon
* James Hancock
* Jim Bennett
* JosephC
* lightclient
* Micah
* Pooja Ranjan (Host)
* SasaWebUp


# Date for Next Meeting: 21 October 2020 at 1400 UTC.
