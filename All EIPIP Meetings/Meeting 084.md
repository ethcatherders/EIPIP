# EIPIP Meeting 84 Notes
### Meeting Date/Time: June 28, 2023 at 14:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/245)
### [Audio/Video of the meeting](https://youtu.be/kgNGfCrOPfI)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
84.1 | **Issue 7198** - Responded with EIP-7199
84.2 | **PR-7222** - @xinbenlv mentioned it is blocking many changes and he is fine with whatever editors agree on.
84.3 | **PR-7225** - @lightclient @SamWilsn supports this. Will be moved to Withdrawn. @xinbenlv will make a PR to EIP-1
84.4 | **PR-7240** - got approved to Final but not merged. @Samwlsn: waiting on updates on the bot situation from @Pandapip1
84.5 | **EIP-ERC GitHub repo split** - Juan pulled up the [Task list for ERC/EIP Split hackmd](https://hackmd.io/A1zfRkO7RKKV6BIaSXpcbw) and mentioned that he added some action points
84.6 | **EIP-ERC GitHub repo split** - Juan is willing to volunteer on the Editorial boards post-split
84.7 | **EIP-ERC GitHub repo split** - @gcolvin shared some process improvements [Update EIP-1: EIP pain relief](https://github.com/ethereum/EIPs/pull/7230) ethereum/EIPs#7230
84.8 | **EIP-ERC GitHub repo split** - @xinbenlv suggested discussing points mentioned in Greg's PR (The PR is in "Draft")
84.9 | **EIP-ERC GitHub repo split** - @SamWilsn is open to discus Greg's proposal
84.10 | **EIP-ERC GitHub repo split** - Danno Ferrin (Besu) brought CFI valid only for Core as an example of the requirement of Core process change
84.11 | **EIP-ERC GitHub repo split** - Marius (Geth) indicated to be more active in editing post-split.
84.12 | **EIP-ERC GitHub repo split** - The group discussed tooling. @SamWilsn will look into the EIPW bot and connect with @Pandapip1 for the eth-bot. Hopefully, both repos. will be managed by bots as it is now.
84.13 | **EIP-ERC GitHub repo split** - @xinbenlv wants to collect feedback from ERC devs and share it by the next meeting.
84.14 | **EIP-ERC GitHub repo split** - @lightclient will hold merging the PR (7206) and wait till bots are in place
84.15 | **EIP-ERC GitHub repo split** - A lot of back and forth. It's worth watching the [recording](https://youtu.be/kgNGfCrOPfI).
84.16 | **EIP-ERC GitHub repo split** - The group will revisit progress in all directions and discuss merging PR-7206 in the next [meeting](https://github.com/ethereum-cat-herders/EIPIP/issues/248).

# Intro
**Pooja Ranjan**
* Welcome to EIPIP meeting 84. This is issue number 245 on Ethereum Cat Herders GitHub repository. Have shared agenda link in the chat. we have few items, to be discussed today. The first one is, open issues, new open issues and pull requests. Then we will have discussion continued or updates from the past meetings, followed by some updates on EIP is insight and, editing office hour, 

# Proposal: Make EIPW only check changed lines except for changing status ethereum/EIPs#7198 [0.42](https://youtu.be/kgNGfCrOPfI?t=42)
**Pooja Ranjan**
* Starting with the first, item here. that is with respect to a meta proposal, 7198. The first one added here is an issue. It suggests that make EIP W only check change line except for changing status. looking into the issue, it looks like this has already been responded with the PR, 7199. Just wondering, do we still need to discuss anything? 
* We would like to, you know, come to a discussion any further, or is it good and can be closed? I see this was proposed by Victor. Victor, if you have to add anything on this one. 

**Victor**
* No 

**Pooja Ranjan**
* Very well. so it looks like the other two PRs are also related to this. The two PRs are 7222 and 7225. The 7222 suggests that propose 7199 should be moved to review. And, there is another PR opened by Sam Wilson, which suggests that it should be moved to withdrawn. first one is by Victor. 
* Victor, if you would like to share your thoughts on that, and then we can look into the proposal for Sam. Proposal by Sam. 

**Victor**
* I'm open either way, so as there is a update, it can be in Eth1 and I can move it to withdraw if there, if we modify the EIP-1

**Sam**
* Yeah, my objection to this is, I mean, both procedural and content, but my procedural objection is that if we have every policy decision in its own EIP, we're gonna have a ton of little scattered EIPs with policy decisions, and I'd rather keep them all on EIP-1. 

**Pooja Ranjan**
* What do other tests think of it or, yeah, 

**Victor**
* I think this has been blocked many updates.  So ideally it would be, it would be spell out. I don't think this is every small policy because, it just happens so often. So ideally it would be spell out. 

**Pooja Ranjan**
* I wonder, Matt or Greg, do you guys have any thought on this, which PR should be moved forward? 

**Lightclient**
* Are you still talking about 7199? 

**Pooja Ranjan**
* That's right. 

**Lightclient**
* Yeah. I mean, I think it should be withdrawn. 

**Sam**
* Is that for a, like you, you disagree with the content or you disagree with having a meta Eth for it? 

**Lightclient**
* I, yeah, I disagree with having a meta Eth for it. 

**Gcolvin**
* Yeah, I'd rather it go any EIP-1

**Sam**
* All right. So if you wouldn't mind, Victor, could you make it as a Eth-1 and then we can discuss on there? 

**Victor**
* Okay. 

**Sam**
* Much appreciated. 

**Pooja Ranjan**
* Thank you. All right. we do not have any changes to final proposal as the next item. However, I'm still wondering, if, we have the bot issue got resolved. Looks like there was this, PR 7240, which was approved yesterday in the EIP editing office hour, to be moved to final. But, that hasn't been marked yet. 

**Sam**
* I haven't heard any updates on, on the bot situation from Panda. 

**Pooja Ranjan**
* Cool. so the authors, so they were, inquisitive about if anything has to be done and our general recommendation was to wait till the bot gets activated and it meds all by itself. I hope you stand good there. 

#2. Discussion continued or updates from past meetings [5.35](https://youtu.be/kgNGfCrOPfI?t=335)
#  Discuss the EIP-ERC GitHub repo split Ref: PR
**Pooja Ranjan**
* Moving on on to item number two, which is discussion continued or updates from the past meeting. so one big item that has been listed here is EIP ERCD post split, for people to have some context. We have been discussing this topic for a few years, and, there has been significant progress in the past two weeks. Matt opened up PR for repo split, and it was also discussed in, in the last all core dev execution meeting from the ACD meeting.
* It looks like most of the client devs are in favor of the repo splits. So if that's the way forward, we must discuss next steps. there is a HackMD proposed by Victor, which is also added to the agenda here. we can take a look into that and, yeah, opening the floor for people to discuss this topic and, propose next steps for us. Juan, if you are speaking, we are not able to hear. 

**Juan**
* We can just, oh, no, Sorry, I was just screen sharing for people that aren't, for whom it's more convenient than opening the heck empty right? I, oh, sorry. I should probably introduce myself. 
* I'm just a random guy who, is trying to help I don't have, a strong opinion on this other than I would be more active after the split in one of the two editorial boards. That's all Cool. 

**Pooja Ranjan**
* I don't know, Victor, if you would like to walk us through the document and let's, talk about the major points that, you propose here That would, that's more than come up with. 

**Victor**
* So I guess whoever added that, can comment. I just list a few tasks. Feel free to add more. 

**Juan**
* I just indented suggestions under each of your top level points so that, here maybe it's more visible in this view. The numbered points were victors and I just gathered comments from various places and threw them in there. so maybe it's work going over the high level ones and ignoring all the stuff and then zooming in on them one at a time. If people wanna add anything or subtract anything, does that work as a workflow? 

**Pooja Ranjan**
* So Juan, if I understand correctly, you mentioned that you would be interested in contributing to the both side of it. yeah. Anything specific you would like to add here? You mean you would be helping out with EIP, coreeip? Of course. Yeah, please go ahead and share that. 

**Juan**
* Yeah, sorry. I mentioned in one of the GitHub threads, I can't even remember which that like, if these were distinct editorial boards, I would love to be an editor and volunteer, whatever the minimum hourly time commitment is to be on the board for the non core ones, like, I really don't understand how clients work. I'm not, you know, a rust or a go wizard. 
* But  I think that, like, to put it another way, what I'm most interested in is having the real world processes around like the editorial processes split. the specifics of like the repo or the, the documents themselves to me is like a secondary concern. So like if there's consensus that's splitting the, editorial duties between two editorial boards, if there's consensus there, like I think everything else is detailed, then  I'd love to champion whatever details get consensus. Right. 

**Pooja Ranjan**
* Sounds good. Thank you. 

**Gcolvin**
* Yeah, there's, there's, there's not consensus and then never has been. 

**Juan**
* Yeah, maybe that's a good place to start. Sorry, I'm coming in apparently years late. I dunno the backstory. So please help me, understand what the sort of blockers are to consensus. Other, other than your most recent comments, which I read. 

**Gcolvin**
* I've never been in favor of splitting the process.  I submitted changes to EIP-1, I thought they were on the agenda. 
* I don't see the point of splitting until we've actually looked at what the pain points are, and I simply haven't seen that the split actually helps the pain points and the pain points I can identify, I've suggested how we can address those without any split. 

**Juan**
* Gotcha. 

**Lightclient**
* At this point, we're kind of overwhelmingly in favor of the split. It's basically, okay, you and Victor and Sam who are against, I haven't seen anyone from the community opposed to the split. 
* So I think at this point we just need to go forward with it and solve the problems on the way We operate by consensus, not by vote. And the community has come to consensus that they want these processes split. 

**Gcolvin**
* The editors have not the community, the editors have not come to consensus. It will do damage to our process to split these. I'm convinced of that. 

**Lightclient**
* Okay. We're, we're gonna go forward with this split because the community has already said that this is what they want to happen. 

**Gcolvin**
* If you want to Continue no longer an editor, then I am no longer an editor. That's the price you're paying for not getting consensus from the editors. 

**Danno Ferrin**
* So one thing I'd like to point out is that we're already starting to move core EIP processes outside of the e EIP process. There is no EIP for the en execution engine API. I, the mid EIP for, the hard forks are no longer kept as eip. They're kept in a separate repo. a lot of the JSON RPC stuff is done outside of the EIP. and a lot of these is the community just doesn't, they don't, some of them don't respect the EIP process. some of them find that cumbersome, some of them refuse to interact with it. 
* And this is a step that would help, adjust the rules for the core just contributors versus the application layer contributors so that we could change the rules that have slightly, they have very different audiences towards what a core process needs from an EIP than what an ERC needs from an EIP and splitting. It'll make it very crystal clear that these follow under different rules rather than having, different views within the editors and different processes. But I think the big problem that we need to address is that this split is already starting to happen. 
* And if we don't take action soon, it will continue in a way that will fundamentally change EIP in general. So we should try and direct it to a net positive solution rather than have coordination failure and let it move away from it and destroy an existing institution. I think we need to come to a consensus to try and make things better, but just refusing to acknowledge that that half of the half of the, the client base that is using the EIP process wants the separation, I think and is, is not a net positive solution. 

**Gcolvin**
* I've, I've suggested a series of changes to handle a number of the problems I'm aware of.
* I haven't seen, I've seen we want to split them, but then what I haven't seen, if we split them, these are the ways in which they're actually going to differ. I haven't seen any ways that they need to be different in order to solve the problems, cuz the problems are affecting both sides in the same way. 

**Lightclient**
* I mean, for one, the things you've proposed are things that have been proposed for years and years that we haven't actually been able to integrate into the processes. 
* So I'm not really optimistic that this time is different. We're going to be able to change these things, but I think ultimately we need to show that the community that we're willing to make drastic changes and help bring some people back into the fold by showing them with this process split, even if there isn't something that's like materializes immediately off after the split. Right now they're so disengaged with everything that they're not even willing to interact with the processes with, you know, minor modifications to things. 

**Gcolvin**
* Well, a big one is if we're not willing to change our link policy, we're not, we're not gonna get people to stop complaining about our link policy, which they hate. 

**Lightclient**
* I don't think it's worth like going into these complaints right now. We've already kind of decided to move forward with this. 

**Gcolvin**
* No, we have not. And if we have not decided, We have decided, have a consensus of the editors. If the community so-called can simply tell us what to do, I'm out of here. 

**Lightclient**
* Okay. 

**Carlbeek**
* What is the point of being an editor and of these things, if it's not to serve the community, if it's not to be a place to improve Eth through the community's like needs. 

**Gcolvin**
* I'm trying to, I've written a PR against EIP-1 that goes through the things I think are wrong and ways to fix them. 

**Lightclient**
* We've had three or four years to do this and we haven't been able to do it. So I think it's time to try something different. 

**Gcolvin**
* So we split them and then what, how does the split actually help a damn thing? What are we gonna do? 

**Danno Ferrin**
* One, Four developers that wanna keep an eye on just core changes have a shorter list or review, rather than reading every random, application layer business model that thinks they need an EIP. So that's one material advantage that splitting the repos will have to core developers 

**Gcolvin**
* In the user interface for GitHub, you simply pick a label and filter out that label. As far as the emails, we, the bot sets the titles so the bot can put a label in the title to make it easy to filter. 

**Lightclient**
* We Can create all kinds of fancy ways for people to better differentiate the different types of EIPs, but at the end of the day, this is not how people interact with the GitHub repos. They're used to their repos having all of the things that they care about, and they just use the standard notification tool. 
* They don't use labels, they don't use email. And we've seen for years we've had these RSS feeds. Nobody uses them. This is the only way that we're gonna get people to interact with the repo. That's just the end of the story. 

**Gcolvin**
* They can't be bothered to hit the label button in the Github user interface. 

**Lightclient**
* You can't get no notifications by label. 

**Gcolvin**
* Yes, you can. You go up and you hit the label and Only not for notifications. No, we, we need to simply fix that. So your email filter pulls out what you want. 

**Lightclient**
* I don't use email for GitHub. Most people don't use email for GitHub. We just go to the GitHub notifications tab and review what's there. 

**Victor**
* This thing complaining into very specific points of notification pain. I know that's Lightclient, you use notification. I don't know if other people, I don't, I personally, that's not my experience. And also I haven't come to know a handful of people, near me who doesn't. So I don't know how representative that is. 
* I think it's worthy that, we go through some of the policy proposal, that, list out and see if that is where you wanna go. It's, it's worthy discussion even if after the splits, and for the record, I personally have reservation on this, and then I don't wanna, I'm not saying that I'm going to block consensus, but I do think that, what's, Greg has listed out as a proposal deserves a chance to be seen here. And you can see how much, improvements, or agreement you have in the future of policy. And if you don't even, the good, the the positive thing is that if you see that you will agree together. 
* I mean, that's, the policy where it will go then split makes sense. But if you cannot agree on a lot of policy, maybe that's time for discussing it. So, maybe we don't see what, Greg proposed in I at edit of EIP-1 as directly respond related to the split. But maybe it's just de deserve a read.

**Lightclient**
* I've read it. And these are just a lot of things that we've talked about in the past and we haven't been able to make this process useful enough for people. So I think that we just need to move forward with the split and discuss policy changes after 

**Gcolvin**
* None of these changes require a split. 

**Lightclient**
* Where were they in the last three years? 

**Gcolvin**
* They, I've been discussing them for years. I put them out there. 

**Lightclient**
* Exactly. So this is another PR that's gonna sit here for years while we debate like what, how it should go in, how we should change it. 

**Gcolvin**
* No,  I put it on the agenda for today. That's why. 

**Lightclient**
* Yeah. We've had on the agenda many times how to improve, like getting EIP into draft. Like what should that look like? Should they be numbers, should they be letters? Should they be EIP, EIPD? 
* Like we've had these debates. Debates have gone nowhere and it's time to just throw the white flag up and split these processes and then try and resolve should these things settle. 

**Gcolvin**
* I remain convinced that splitting them will do real harm and will not help. 

**Tim Beiko**
* I'm curious in understand like what harm do you see coming from this because, and like I understand Sam's point that like, look the repos like a collective documents, you can treat different documents a different way, but obviously we have different types of documents in different repos today. Like the yellow paper ELs, Jason RPC live in different places. 
* So like what's the, what's the harm that you see from splitting aside from like, sure, it's gonna be a bunch of work to do it the first time. but yeah, beyond that, like assume the split is done, you know, what is the pain we're experiencing after on like an ongoing basis? 

**Gcolvin**
* Are we going to create two organizations to go with the split or is it just two different file cabinets to deal with? 

**Tim Beiko**
* What do you mean organizations? 

**Gcolvin**
* I'd like to, under the split is just seems to be creating two file cabinets for some purpose. 

**Tim Beiko**
* What do you mean by organizations? Do you mean specifically EIP editors or something else? Are there gonna be Yeah, so yes, I, suspect the process to add and remove EIP editors, it might be the same process, but the people might end up being different and potentially overlapping. So maybe, you know, if you stay,

**Lightclient**
* But this is no different than today. 

**Tim Beiko**
* Right. Yeah, but yes, I think or organization is maybe like implies too much overhead. Like it's not like there's like a, a company or like a, a literal organization for those things. 

**Gcolvin**
* What are we actually going to do differently after we've created these two file cabinets and gone to all this effort? 

**Lightclient**
* But what is the thing that you're worried about happening? Like, you keep saying that this is going to create something bad for these processes, but you're not really enumerating the issue. 

**Gcolvin**
* Nobody's told me what good is going to come of it. 

**Lightclient**
* I mean we did, we told you a very specific good thing that we'll come up with that the court developers are asking for, which is that they can actually use the notifications for the EIPs. Whether or not you think this is reasonable, like I can't make you believe that that's something that's useful, but that's like a very small specific thing. 

**Danno Ferrin**
* The good that's gonna come from it is, it's gonna be a lot easier to get people who have disengaged from the process to re-engage with the process, like has been mentioned in chat. We have been losing specs that should be EIP to other repos that are skipping the EIP process that should have EIP numbers posted for these changes. 
* But rather than engage with the EIP process that create their own repo and do their own thing, that's the big win I see is by splitting the focuses of these two filing cabinets, these two organizations or however you wanna view it, people are gonna be able to laser focus on the area they care about and not have to worry about the other things that are outside of their scope of concern. 
* ERCs and application layer EIP have a broadly different scope than protocol level changes and there's very little overlap. And when they do overlap, it's worth an EIP in both repos because there's gonna be different aspects that impact how the protocol interacts with it and how the clients interact with it. 
* So that's the big change I see is making these two layers much clearer and more distinct in development and test development and process and uses. So it's gonna make it more crystal clear that this happens on the application layer and this happens in the protocol that is the single biggest game I see from splitting this, and I think alone is sufficient to split it. 

**Gcolvin**
* Okay. Well I'm sorry if we do this, I'll leave. I'm free to leave. You're free to let me leave and I've gone through the changes I actually think will help. I think the same changes need to be made to the ERC see the same problems with the process. So splitting the repos still leaves all those problems. 

**Carlbeek**
* I don't think many people disagree with you there. There are many common issues and there are many things that need to be addressed, but this is an orthogonal issue  we're trying to address here. and very much would like to to to fix many of the things you brought up and in many of the ways that you're, going after here. But this is something else that we desperately need to be like,  would EIP V process get more used? 

**Gcolvin**
* I still don't see how it helps you still write an EIP and submit it to the process and having two processes over time. Why have them diver? 

**Carlbeek**
* So because to people who aren't actively involved in both processes and don't actively all of the exact weird rules you have to learn to interact with those repo. it is a nightmare to come over to this repo. I see it and they are, like,it just seems like a very confusing place to exist.
* And we can do this thing where it like dramatically simplifies things with, for the average person, you just have to go to the repo and look at the things that are probably relevant to you, and you can then start filtering by topic instead of figuring out what the metafilter mechanism is that, happens to, to interact with the repo. 

**Gcolvin***  
* This, this PR doesn't suggest changing anything about the process that people are complaining about except getting a smaller set of notifications

**Carlbeek**
* And making the repo itself easier to interact with.  But like, again, no one here is pushing back against the other, the other changes you're proposing. Those should also be discussed and implemented. I think people desperately want more changes. So let's just do the But we haven't for, for years and years. 

**Gcolvin**
* So I'm gonna have, I said there're gonna be two EIP-1. What are we actually splitting here? 

**Carlbeek**
* The places where these, EIP exist and potentially the processes slightly over time, if that's what the demands are from the two different communities largely that are interacting with this process. 

**Gcolvin**
* It's only one community, but that's another that Communities In one finally cabinet. 

**Lightclient**
* I feel like we should try and time box this. I think we're just starting to go in circles now. 

**Gcolvin**
* Okay. 

**Victor**
* Yeah. Can I, can I ask A question? 

**Gcolvin**
* I question, I put something on the agenda that's, that's not getting discussed, so We did discuss it Hardly. 

**Victor**
* But,  can I propose to also ask that I, we've seen, a group all core devs and you are definitely welcome here, but, I have heard your voice. can I ask other than, lightclient who in the editor group is strongly in favor of the splitting, The Gordon in the chat says he's strongly in favor, Gordon. Sorry, maybe I, we didn't over, but, I've, not worked with you. maybe you put three times mine. 

**Pooja Ranjan**
* No, I don't think, this name was ever in the editor's list. If this question was specific to editors, no, I don't think it was there. And, we are not joined by all the editors today in the meeting. That is another point to be considered. So I'm not sure if we can get a proper response over here. I see, Panda and, saying not in the meeting 

**Victor**
* Yeah, I think we, we don't have all the editors just like we don't have, all core dev team as well, but I've seen that currently it seems to me only like Lightclient in favor. and, so it seems your gender is in favor still. yeah. It seems like there's, a bunch of people  who are reserved and I do believe that's,the problem that called back and Daniel and Mary has said is real problem, that people were disengaged and notification was not, was inconvenient.
* For me, the notification is more is inconvenient, but the more problem is it's so hard to edit. And what's, I think, what's, EIP-1 updates by, Greg is about making it convenient. And if you discuss, you will realize that a lot of things that you believe is natural are actually not, like some people in the editor group are actually trying to say that, oh, let's make it harder.
* And that's what I think, we are trying to repeatedly, Greg and I and and a bunch of folks are trying to make the process easier for people to engage. And we are frustrated as much as you are. 
* We feel that the discussion has not been made to make the progress and most of the All core devs are not as closely follow the debate of policy as we have been. And we don't know how to surface those  but those debate to you of the better way, if a lot of that all core devs like individually come to us and say, Hey, this policy is really dumb, we should fix it. And whenever we take it to the editor group, it gets blocked. 
* I, the frustration I've seen is that those are from both sides. People just don't want that to be so restrictive and we haven't been able to resolve it. And I'm not, I'm unlike Greg, I'm not planning to block the split. I just felt that, we really, really should discuss and take the input from the all core dev and EIP authors that how how to make is easier for us to edit. And, until now I'll say other than a notification, I hadn't seen very convincing things that a clear direction of why, or how or can, can benefit a policy that ERC can't in the point. And yeah, so can we at least take a look at, the EIP edit up, updates of the, of Greg's and then, hi, have Greg maybe walk through the, the over overview of it and, and see, because we, it is a valuable time where a lot of eyes here are, today you can see the, the proposal that we make and see if it makes sense for you. 

**Pooja Ranjan**
* Yeah, I see, Danno has some points to make on protocol specific policies. Please go ahead, Danno. 

**Danno Ferrin**
* So there's a couple of things that would benefit if we could split the repo that we could even have the discussion about starting if EIP and ERCs were different. Some, there's some, workflows that the core devs have adopted, such as eligible for inclusion included in the hard fork that that kind of used to be in the EVM process. But we pulled out, and these are steps that are completely inappropriate for an ERC to be considered as gatekeeping. 
* We shouldn't be have to gatekeep the diamond standard because clients don't have it implemented for, for Cancun or Prague or whatever. So that's one policy change that I think would go on pretty early is we would bring back in our signaling for which EIP s are actually viable in which ones aren't for inclusion. The withdrawn suspended just really isn't doing it for us. We need something that has feedback that is more tightly integrated with the ACD process. and the second thing is I think we need to add another step for EIP that are core protocols that reflect the  readiness for testing development. Do we have reference tests written for these that should be a separate lifecycle step that should block final acceptance of these tests? And we should also integrate in the process whether it's ready for testnet, if it's been deployed on main net. 
* These are things that are very, very peculiar to core protocol and aren't worth discussing. While we are still merged with, the  ERC process that has completely different goals and completely different agendas than what core developers have is these vastly diverging policies, vastly diverging needs that come from what people want from the ERC process.
* That is really what's freezing the gears in all EIPs  one discussions on the thought that it needs to serve all possible use cases. If we split the repost based on use cases, we can go, we can have more reasonable discussions about specifically forming and changing these policies that we just can't have when it is an all comers type filing cabinet. Just as little as two different filing cabinets will make it easier to even have these discussions that we just can't have today because people say, well, I don't understand it and don't call into the meeting. 

**Sam**
* So I definitely understand a lot of the frustration with having the EIP process not attached to the like the core development process. Like, well, I was working on ELs the amount of times that it's like, okay, which hard fork is this EIP is in? And, you know, what block number does this EIP activate on?  I understand a lot of those frustrations and, you know, switching from my ELS hat to my editor hat, the statuses of documents and Els are of the documents themselves. 
* And I think the reason, and this is from before my time as an editor unfortunately, but I think the big reason why, we aren't more tightly integrated with the release cycle of main net is that EIPs are meant to be, like agnostic to the chain that they're deployed on. So you can point to an EIP and say like, you know, on Ethereum Classic we have these EIP and on on main net Ethereum or a testnet Ethereum have those EIPs and like that's kind of why they're, they're so separated from how core development works. Maybe it's time we reexamine that link, but we can do that without splitting the repo. I think like having a different process for core EIP is completely doable. 

**Pooja Ranjan**
* I would also like to add a few points here. I think there is some, misunderstanding. I would like to clarify. The existing EIP process is somehow different for CORE and the rest of the proposals, rest of the category in time. So, for core EIPs we do have the process of CFI, which was never a part of ERC, 

**Lightclient**
* It's not part of EIP though, it's outside of the EIP process.

**Pooja Ranjan**
* That is a part of network upgrade process, which is only applicable for core EIPs. So we do have a way to follow it. It just that is it an EIP one? it is on the execution specs. It's added there. Okay. 

**Lightclient**
* That's outside the EIP process, Right? 

**Pooja Ranjan**
* What I'm suggesting here is like we can still follow that and it is not affecting core EIPs to follow it. And it is, I mean like ERCs are not a blocker here. The process, what is being suggested can be followed. We have ways to follow and I don't think ERCs are stopping that ERC and core EIP process.
* In fact, core EIP is only category where, where it is a little bit different than any other process. For example, core EIP should not be moved into a review status unless it is into CI dev net, phase like client have started testing into it. We cannot move it to, last call unless it is on public testnet. 
* And these are not the restrictions for ERC or any other category. For any other category. We say last call is only for 14 days, but in case of core EIPs, it can be seven days to a end number of days till we put it on the main net. So we already have different things in place for core EIPs. 
* We are already making it an exceptional category where we are providing special privileges. So what I understand from this discussion, what Vector and Greg are trying to communicate is let's try to point out the pain points which are not accepted by the ERC category and which we want to implement because we want to support core EIP here in this repository. 
* I do agree that de noise point is very much valid. The notification point is very much valid and  I perhaps do not have any perfect solution for that. But if that's the only consideration for the split, I don't have much to add. 
* But if we have other pain points that can, that we can address, I think it is not only going to help core EIPs process, but to all EIP process for that split may not be required. We need to understand the issues here. 

**Danno Ferrin**
* So let's look at the CFI process. that's something that does not really managed by the, by the EIP process. That's something entirely managed by the ACD. So now what we would have to do is if we want change that we would then have to post an EIP to EIP-1, let a bunch of editors who don't always call into this meeting, then we have to represent what the needs of the core devs are. And that just increases in a lot of friction to an already slow process of, of shipping core protocol changes. and as we've seen when you do a proposal that someone doesn't like, they will jump up and say, I'll block consensus or I'll resign and make big drama outta something that should have been a simple change. That is my concern of keeping it together already making all of these exceptions. But the number of the exceptions that we're getting is to me a signal that it needs to be a separate process. The filing cabinet should be generally all comers to all and have all the same rules. If you have more and more exceptional processes for subgroup, then I think that's very strong signal that that subgroup is not being served and is not appropriate for this particular filing cabinet. 

**Gcolvin**
* Some history here, we started out with nothing but drafts, and how the all core devs organized their own process was not an EIP concern. Once something went on the mainnet, we labeled it final because once it was on the mainnet, it couldn't really be changed. whatever was on the main net was what was on the main net, and that's what the EIP needed to describe. 
* We added a last call process for ERCs just so there was some way to get them final for people to say, okay, this is what we're going to implement. over time we wound up adding more categories in process and sort of mixing up the core dev process and the EIP process from my, from my perspective as an OG it got more complicated, it got more mixed up together. 
* So yeah, the core devs are having to fight with EIP process when really they shouldn't have much to do with each other. The core devs could organize where a draft is in their process pretty independently. 

**Tim Beiko**
* And, but you can't this and, and I mean the fact that like Eth2 launched without using the EIP process shows you that like this doesn't work in practice, right? Like, and the fact that you have to create a process out of the band just like adds way more friction. Like when I have to send someone the CFI definition and it's some random thing in a repo somewhere, like it, it just feels like it's terrible. Like when we have to use each Eth-magicians, to like signal which like EIPs we may want to include in the hard forks, it's like we're creating all these random things that the only people who can actually track are folks like basically me whose job it is to do that. But if you're a random person who wants to figure out, hey, which EIP are being proposed for Cancun, you can't go to like Eth ethereum.org and have any in insight on that. 
* And similarly, you know, on the ERC side, if you're a random person and you want to figure out which, you know, what, what are the implementations of like the last NFT standard? You can't do that. and you can imagine like that would be a much healthier version of both those processes. like yeah, like Peter from Geth asks me for these random documents, you know, from time to time. And it's kind of insane to me that like, you know, with the context he has, he's not able to like intuit where the right thing is. 
* And I think this is because the things have to be standard and I understand that like it, you know, you don't want the EIP statuses to be focused on hard forks because not all of them need hard forks. 
* But if we do split the reposts, then you can say, look, on the EIP side, there's an extra tag that says, you know, hard fork status or something like that. And you know, maybe for networking EIP it's just not set, but for like a core protocol change, then, you know, it gets set and then you can just click on like the proposed tag or the included tag or the London tag and you just get a full list of all the EIP and that fork. And like, I think there's, there's some aspect where like, how do we make this easy for people who have very little context about the whole thing? Because like even with folks that are, you know, on quite literally the Geth team that work at Ethereum Foundation, they can't figure out how to find stuff. And this means that like if you're a random contributor who just wants to come and like write their first EIP and make sure it gets seen by the right people and you don't necessarily know, you know, Peter or me or Marus or someone that can like, help you through the process, then it's, it's like really bad and it puts those people at a disadvantage. 
* So I think the more we can do to keep the processes encapsulated in one thing, the less context people have to learn. And because there are some differences with EIP and ERCs, it makes sense to split them so that, you know, both processes can eventually reflect like the reality of the whole life cycle of not just like writing the spec, but like writing the spec and getting it live and deployed and stuff like that. 

**Pooja Ranjan**
* I mean, strongly in favor of like keeping both process encapsulated and keep on working. It looks like the ship before, stopping the, repo split has already been sealed and I think it'll be interesting to, follow on what on the next steps. yeah, please, Marius, if you have to add something over here. 

**Marius**
* Yes. So one thing that I would really like to talk about, is, so as core devs, I feel our duty is with the community. And if the community wants, something or doesn't want something, we have to respect that wish, even if, the community, want something that we are not in favor of. So for example, I was really in favor of it and I thought it was the, the right thing to do and at some point the community decided that this is not the right thing to do, and so I had to accept it. 
* And, I think the idea of the EIP editors overruling the, the community is something that is so foreign to me, that I think it's incredibly undemocratic. Why, why should these eight people have a vote on, how this process that should serve the community and doesn't, why should they have the vote to block the, the, the view of the entire community? There's, I haven't seen anyone except for, people from the EIP editing team speak out in favor of keeping the repositories together. That's, that's it. Thank you. 

**Sam**
* Well, so like I said in Chad, the community would rather have, you know, way higher gas limits that would cause, you know, database problems in a few years, right? The community doesn't always know that, you know, the technical reasons behind why things are the way they are. 
* I'm not saying that there are technical reasons to keep the repositories together, don't get me wrong. I'm just using that as an example of why the community might not always be correct and experts might be, you know, have a different opinion and, you know, a lot of the times with the process around EIPs, I think they have very logical reasons. and I think a lot of the hate the EIP process gets is from, you know, the previous era of EIP editing and that we're a lot more, like, we're a lot easier to follow now than we used to be. 

**Pooja Ranjan**
* Yeah, there has been a lot of process change. I do not deny that. I think it's time to accept this as one of the process change and, one reason why I feel like EIP editors  have been strongly supporting or opposing whatever their point of view they are sharing, because ultimately process management is something that they are heavily engaged with. So yeah, considering that, the split will bring as, as I mentioned, that there would be a fixed cost of having this split done.
* Let's start looking into this cost and, if I understand correctly, it, was mentioned in the all code execution call that if this thing does not work out, we can perhaps come back and fix, make things back as it was. I think that there would be some te tooling needed. I was having a conversation with, someone and, he mentioned that we can, we do need to duplicate some of the work. Let's start looking into that. I don't know, Sam, you have been managing most of the bots related thing. You think that there would be some challenges that we should perhaps discuss here and try to find out this solution to that in case we need to, move forward with this split? 

**Sam**
* As far as EIP W, the, the validating bot goes, it would maybe be like a couple days worth of work, probably a little less to, make it like configurable. for a split. it shouldn't really be a problem. for Eth review bot. I'm a lot less familiar, but I don't see it being more than a few configuration changes. 

**Pooja Ranjan**
* All right. So just imagining this as like a cabinet, changing for ERC and EIP, we do not see a lot of tooling issue. Is that a correct understanding? You can perhaps manage it? 

**Sam**
* Yeah, so the, the tooling should be easy. the governance overhead might be a little bit worse, but I don't think I, like, I don't think there's any like having to do a ton of work objections to splitting the repos. 

**Pooja Ranjan**
* All right. I do understand that there are people who are still not in favor of having this, split and I heard, Greg mentioning that he may be willing to resign at this point of time. I would sincerely request to every editor, please do not resign. 
* We need you understand there can be objection and that can be solved and that can be help only if we have you, we only have six editors on board and we need more people to join in to help out with this process. 
* Split whatever time you have got, if you can divide it for both repositories, that is good to have. If not, then please support one repository and we'll try to have more editor on onboard on the other repository. As of now, this seems like, what people are requesting for looking for. 
* Let's give it a try, see if this helps and if it helps the core EIP process to evolve better, ERC can always learn from core EIP and have the process adjusted. other than the filing, cabinet filing issues, I hope that ERC group, ERC community does not feel a lot of, you know, pressure because they are less with editors or they do not have people to support. 
* We are here to support. We will try to support both groups. Having said that, yeah, Greg, yeah, I was hoping for you and Victor to jump in and say, some concluding words for the start. 

**Gcolvin**
* I have put a proposal on the agenda. We have not really discussed it. I've been told, well, we've already discussed those things and yes, we've already discussed splitting and we haven't really gotten to a consensus on either one. I'm simply not. 

**Lightclient**
* We Have a consensus on splitting or kind of asking if you still want to be a part of it. If we go forward with this. 

**Gcolvin**
* I'm blocking consensus until we have a complete plan, not just really I think at, please hear me for just a sec. 

**Marius**
* I think at this point You might just not be part of this anymore. 

**Victor**
* I have asked to, have an opportunity to surface this to the ERC author group. and  I was hoping that to get a chance, when I heard that the ERC authors are not part of the community, I was a little bit confused. So, when, like Lightclient says it's a community consensus, I was quite, confused, because we haven't asked the ERC author and it is totally possible that when we go to ask ERC authors, they want to see split as well. 
* It's totally possible. It's just that, it seems like I Posted it on Twitter Consensus was, well, it seems like the consensus, what you meant is not as mature as I would see it. 

**Lightclient**
* They had an opportunity to say that this is not what they wanted. Tim posted this on ETH magicians in February. This PR has been open for over a week. There's been a lot of opportunity. Not a single ERC developer has said that they don't support this. So at this point, like there's just nothing. Like, there's no point in in continue to drag this out. 

**Victor**
* Do you? 

**Gcolvin**
* What is the object? Please. What's the objection to simply saying, I want to see a complete plan, not just we're going to split them, but we are going to 

**Lightclient**
* Have you read the hackmd? Yes, There's the, there's the plan. We're not going to enumerate every possible permutation of this plan because then it's never gonna get done. We just need to go ahead and do it. This is like the rough outline of how it's going to happen. 

**Sam**
* What is the first rule change that's going to happen in the core EIPs repository and the first rule change that's gonna happen in the ERC's rules? 

**Lightclient**
* I don't wanna, I don't think we should be going into like the specific rule changes. Like we, no, I already, Just one example, it doesn't really matter what We don't, I mean we, we have six minutes left. I think that we need to like sort out how this is going to go down because we need to come out of this call saying, yes, we're going to do the split because we can't continue to drag this on forever. 

**Gcolvin**
* I have a PR out. I would like it be considered. Seriously, 

**Lightclient**
* It's Not going to be considered before the split That I'm not just Greg, Greg, just, just How dare, sorry.

**Gcolvin**
* If you're not going to consider my EIP that I'm not being retreated respectfully and I'm gone. Okay. 

**Pooja Ranjan**
* Greg, I really want to be respectful over here. I really want to be respectful over here and I would request you to move the PR in from draft. I mean like it is still in the draft and we don't know if it is ready yet. If we can change, change that, make it like, you know, the PR is ready to be discussed. I think we can perhaps have more discussion on that. And as Victor also mentioned that he would like an opportunity to have it discussed with the all ERC dev meeting. 
* We can, listen to, what people over there have to say, what we want to do here right now to get prepared for both sides. Like if the split is happening, then we should be ready with tooling. We don't want things to break down. So we should be, ready with toolings, which I suppose isn't, moving in the right direction. We should do not have to work too much. It can be done. I also manage a website called EIPs insights. For now we are already taking care of like, you know, every data coming up from this EIP is repository. 
* If we have to go with the split, then we perhaps will have to have another set of tooling done for that thing. Definitely. We have to do a lot of work. What we are, I think concluding here is we should be ready for going in both ways. We would be discussing the changes that you are suggesting for EIP one, if it is valid for core EIP, what we need to do is like suggest it for both parties and see if we can discuss it over there.
* But let's keep that, pain points that you have mentioned, separate from this, repost plan. I do agree, about, you know, the ideas to learn how we want to make changes, what are the proposed changes. It would be really interesting to learn. but in the meantime, my only request to you would be please do not take any decision and,in rush. Let's give it some more time and let's see that, we, how do we evolve with it? Let's be ready for both sides. 

**Lightclient**
* Like I'm going to continue forward, down this path of executing the split because this is what the community has said that they wanted, right? But I don't want to lose any EIP editors in this process. But we can't just sit here and debate this every call for the next six months. we;ve been talked about for years and years. 

**Pooja Ranjan**
* Matt. Matt, my only request is to not merge the PR just as now as, Victor requested for some more time. We give them the time to come back with, whatever decision they have as we gave it to core dev. Let's give it to core, ERC Dev as well. 

**Lightclient**
* They had their time. They had since February, they have had years. We'll, no, I'm not going to merge this PR until we have the bots ready, but yes, we need to start working on the bots. 

**Pooja Ranjan**
* Yes, of course. 

**Lightclient**
* And I'm, we're not going to listen to more debate about whether or not to do this. 

**Pooja Ranjan**
* No. I totally understand your point here. So let's move that. Let's get the bot ready. Let's prepare our repository to be ready for whatever case we go. 

**Lightclient**
* We're going to do the split. 

**Pooja Ranjan**
* We can go ahead and merge that, but please don't do it in rush. Let's give it two more weeks. I'm not discussing it any further, but what I'm saying is let's, let's be prepared for this flight. Give us some time to get prepared. maybe by next meeting we'll try to collect some asing feedback from Panda on EIP bot for EIP W. 
* Sam already mentioned that there are some work to be done and that should be, that should be good. and I hope that by next meeting we would have everything in place and we can smoothly merge it. I am not saying Greg, we are trying to disrespect you here. It just that, there are some times we go by the majority of what people say. 
* Even if we do not have an absolute consensus, we go by the rough consensus. And if that's what people are looking for, even if we are having a different opinion, let's give it a try. 

**Gcolvin**
* So we're, we're not willing to consider my draft before we make a decision on splitting the repos. Is that what I'm been told? 

**Sam**
* I'm willing to absolutely And, and ok. 

**Pooja Ranjan**
* You what you need to do is like make it out of the draft. Like your PR is currently in draft, so if you make it out the draft Yeah,

**Gcolvin**
* I'm sorry.  I put it in draft so that the bot didn't accidentally merge it, which is

**Pooja Ranjan**
* No, it would not. Yeah, it would not. So if you make it out of the draft, then perhaps we'll start getting more comment on it because then we consider that as ready to be discussed. Right. 

**Gcolvin**
* Okay. I've had them. 

**Lightclient**
* These Are orthogonal things though, like going through the proposals that you're making, Greg and doing the split. We can do these in parallel. Like I appreciate the proposals for changing the process, but this is not something that we're going to block Splitting the repos

**Gcolvin**
* It makes a difference to my block. A big difference. 

**Lightclient**
* We're going to go forward with the split even if you're blocking this. 

**Pooja Ranjan**
* All right. 

**Gcolvin**
* I'm saying it could change my block and that makes a difference to me. I put many years into this. Into this. Okay. 

**Pooja Ranjan**
* No, no, that's absolutely true. We are really, thankful for all the time that you have given up. Perhaps you are one of the oldest editor that we have on board and we would not like to lose you. But I think it's time to wrap up and let's have this conversation, like giving it a beautiful rest. 
* We wait for another two weeks. In the meantime, we will try to work on the bot side, get our EIP GitHub repository and ERC GitHub repository ready for the split. And in the meantime, Victor will also take some feedback and come back and share it with us. Matt, sincere request, please do not get that, PR merged before we have the next meeting. See you later.
* Alright, thank you everyone for joining us today. Have a good one, everyone. Thanks everyone. 


---------

## Date and Time for the next meeting

July 12, 2023 at 14:00 UTC

---------
## Attendees

* Pooja Ranjan
* Victor
* Gcolvin
* Lightclient
* Tim
* Carlbeek
* Danno Ferrin
* Sam
* Anaphant
* Marius
* Gajinder
* Gordon Wright
* Juan CaballeroSam


