# EIP# EIP IP Meeting 28 Notes
## Meeting Date/Time: Wednesday 10 March at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/56)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=fKQVb-s0Tzs)
### Moderator: Pooja Ranjan
### Notes: Jim Bennett

----
## DECISION ITEMS

**DECISION 28.1**: Continue to think about how to deal with suggested changes in Last Call and keep Item #2 on the agenda for the next meeting.[see 20:23](https://youtu.be/fKQVb-s0Tzs?t=1219)

**DECISION 28.2**: Put an item on the next meeting agenda about EIPs for Berlin moving to Last Call. [see 32:39](https://youtu.be/fKQVb-s0Tzs?t=1959)

**DECISION 28.3**: Discuss separating ERCs from the EIP repo in the next call. [see 39:53](https://youtu.be/fKQVb-s0Tzs?t=1959)
----
**Pooja Ranjan**
Welcome to EIPIP meeting 28. I'm Pooja Ranjan.

## AGENDA

## 1. [Progress on EIP GitHub repo action bot](https://youtu.be/fKQVb-s0Tzs?t=4)
The first item on the agenda is progress on EIP GitHub repo action bot. So a little more from the ECH team is working on the EIP GitHub repo. And I suppose she also created a pull requests to share this bot for review with the EIP editors. The pull request number is 3351. If there is any other update on the progress and concern with the bot that anyone would like to share in development of this effort, feel free to share, because I don't see any data here. But I have seen some comments left by the editors on the issue.

**Hudson Jameson**
I heard it's almost done. But I haven't looked at the code myself.

**lightclient**
I haven't got through the code in depth, because we're trying to decide where it should properly live. And I am asking for it to be moved to its own separate repository, and it's just called from EIP repository to do the action. So that's being worked out at the moment.

**Edson Allyon**
Is that how GitHub action works? Because usually you put the script in the repository in a separate folder.

**lightclient**
Most GitHub actions that people use are public actions and a separate repo, and you only add it to your yaml file and the GitHub workflow folder. So I assume that it should be pretty straightforward to just have another repository. At least from what I've seen from the docs for the actions, it seems like it has a pretty straightforward method for referring to an action by a request by a user and a repository name.

**Edson Allyon**
Okay.

**Pooja Ranjan**
Brent, I believe you also have some questions on this.

**Brent Allsop**
Yeah, you guys have been talking about it. It's more related to mine. So I'll just wait till we get to my item, and I'll do it all at once.

**Pooja Ranjan**
Sure, no problem.

## 2. [2. Network upgrade process review](https://youtu.be/fKQVb-s0Tzs?t=135)
The next item on the agenda is network upgrade process review. So there were some questions and comments on the network upgrade process in the AllCoreDev Discord channel last week that surfaced with respect to EIP 2315. Regardless of the decision taken for that proposal, I want to address some comments that were specifically related to the network upgrade process that we came up with recently.

So as per my understanding, it was mainly related to two things. Number one, many people are still not aware of the process. And number two, the network upgrade process could be modified to enforce the review status. That is a fairly new status to be a mandatory status at or before it is CFI approved. So for the first point, people are not aware. I think we need to be a little more vocal about that and create more awareness about the new process and encourage authors of at least core EIPs to follow the process. As far as point number two, I'm proposing some changes to the current process. There is a [link in the agenda](https://github.com/ethereum/pm/issues/264#issuecomment-790929212) that people can follow.  I have been meaning to propose this earlier, but I believe it's not too late to start now as well. I came up with these suggestions based on some conversations with **Micah** at different places regarding the Last Call and the Final status for core EIPs. So I'm proposing this new structure if we can get some feedback on that.

**Hudson Jameson**
So this was the GitHub issue in the comment right?

**Pooja Ranjan**
Yes, I just shared the link.

**Hudson Jameson**
Perfect. Okay. Sorry, I was reading this comment wrong. This diagram that you put into the comment is the proposed changes, not the current state, right?

**Pooja Ranjan**
Right. So in the diagram below, if we see that I'm proposing that Consider for Inclusion could be EIP status could be Draft till Review and DevNet phase that we consider the EIP status has to be Review only. And when it goes to mainnet phase. The first part should be reviewed to Last Call. And as **Micah** was suggesting, we should not put final status on any core EIP unless it is deployed on the mainnet. So if it is on mainnet, then only we provide the status of Final. So this is the proposal.

**Hudson Jameson**
I thought we got rid of Final or changed the definition to separate the upgrade process from the technical process.

**Micah**
Final still exists. I think it's just no longer special for core EIPs.

**Hudson Jameson**
Ah.

**Pooja Ranjan**
What we got rid of was Accepted.

**Hudson Jameson**
That's right. I got those confused. Okay, that sounds good.

**Edson Allyon**
So how I think it'll work out is people will wait to change their EIP to final if it's a core EIP until after it's deployed. So it'll probably stay in Review up until they get confirmation that all right, this is one that we're going to go with.

**Hudson Jameson**
Got it. Okay. That sounds good.

**Micah**
I believe Pooja is suggesting that it goes into Last Call once we once we get a couple of testnets. Once we decide the fork blocks, basically, the EIPs for that upcoming fork all go into Last Call.

**Hudson Jameson**
That seems a little bit weird because if there are changes during Last Call, then we'll have to switch client stuff for the fork blocks that have been created, right?

**Micah**
Yes. By the time you get there, you should not have any changes. If you have changes in Last Call, it means you did not do a good job of reaching out to reviewers ahead of time. So you failed earlier.

**Hudson Jameson**
So that should be in DevNet phase. Because if it's in mainnet phase, it's already so late in the process then we don't want things to change. A lot of people wait until Last Call to actually do any final reviews, and people put it off. So if they're doing that already, then waiting until the mainnet phase seems counterintuitive.

**Micah**
I think people did that because we did not have a Review phase. We only had Draft, Last Call, and Final, basically. And so there was no phase where the author asserted, "I'm done. It's now time for people to look at this before it goes live." There was just, like, "I'm working on this. And then it's going live in two weeks." That was the only step previously. We now added the Review step, which is so we now have, "I've worked and then I'm done working on this. Or at least I think I am. I need feedback." And then I personally think the Last Call is "I'm done with this; I've received feedback; I've iterated. Everybody thinks this is good. This is your last chance to speak up to stop the ship. Like, the ship's already taken off. This is the last chance to stop it" kind of thing.

**Hudson Jameson**
Making it a habit for people to be able to stop the ship in a mainnet phase just seems like the same problems we're facing today.

**Micah**
Well, so the "stop the ship" would be like a security vulnerability. In my opinion, once you go into Last Call, it should really, especially core EIPs, should really be done. Like this shouldn't be the, for lack of better word, it is the Last Call. Everything is done. There's no more changes. This is a last chance for anyone to speak-up-or-forever-hold-your-peace sort of situation. Which to me aligns with the fork block decision.

**Hudson Jameson**
We have a precedent for ERCs that people can do radical changes during Last Call because it's happened.

**Micah**
Yes, ERCs are terrible and shouldn't be a part of the process.

**Hudson Jameson**
So the thing is that because, ideally, that shouldn't be the case. But right now, I feel like unless we really push people to change their definition of Last Call for both ERCs and Core EIPs, we're going to run into this problem, because right now as the definition in EIP 1 stands, it sounds like you can change it during Last Call.

**Micah**
Yes, you can change it, technically.

**Hudson Jameson**
And basically there's nothing in the definition that encourages you to only do security changes.

**Micah**
From your point of view, is this just a kind of historical thing where people are used to Last Call meaning something that perhaps isn't what we intended, but it's what it is, or it's your saying yeah, EIPs should be final before fork blocks.

**Hudson Jameson**
I think EIPs should be... Hmmm. Yeah, that's weird because I don't want to add another status in between there necessarily, because that's adding too many statuses. But yes, I agree that I think the original idea for Last Call, because Nick Johnson put it in. So a lot of people are going off of his definition, which is during Last Call, if there's anyone who has objections, they can raise those objections. And there's not any implication that it has to be a security objection.

**Micah**
Yes, I agree with that. I suspect Nick, if Nick put this in, he was modeling off of like IETF, and RFCs, and all those. And those ones, by the time they hit their last phase, there's almost never any changes. When there is, it's really small. It's like a minor tweak, a constant kind of thing. The problem is, with Ethereum EIPs, we are not nearly as good as those people at making specs. And so, by the time we get to Last Call, like you said, there are a lot of people who haven't even bothered looking yet. Whereas if you look at, say, W3C, you know, when a JavaScript change or a browser change gets to the last phase, there's really no opportunity to make any significant changes at that point. It's already gone through years of iteration, and it's implemented in every browser. And it's all but done. And  that last phase is basically, we're pretty confident this is it. And you better have a really good reason to change it.

**Hudson Jameson**
Yeah, I'd love for it to mean that. I think that people aren't going to use it that way. I think people are going to not know if Review means it's Review day one, or Review day 365.

**Micah**
Is there a solution to get us long term to a place where we actually do have a process that more closely aligns with other standards organizations?

**Edson Allyon**
So I have a question. Say we do put Last Call for DevNet, and then we find something in the dev testnet that should be worth editing an EIP? I think at that point, if we put into Last Call, and it was three weeks after instead of two weeks after, would it be messing up the process to have an EIP that's final, but we have we've found something in the dev testnet that that we should update the EIP?

**Micah**
So for Last Calls, the review end period for the way I've been treating it is not optional, but it's the minimum review. So the earliest this thing will be merged is two weeks later, or whatever date the person puts in. However, it does not have to go to Final exactly at the end of the review period, specifically for 48 days, because it goes Final for the exact reason you said. It does not go to Final until mainnet launch in case there's a last minute change, like a bug popped up in public testnets, for example.

**Hudson Jameson**
Oh, so one way to fix this, then, is to have Final not mean it's in mainnet. Final won't mean mainnet because it won't require a hard fork.

**Micah**
Final means that you can't change the EIP. Remember that from the point of view of the EIP process, it's uncorrelated with the hard fork coordination process. So once your EIP's in Final, you cannot change it. If you want to change it, you create a new EIP with a new number. And you know, maybe it was copy and paste, which is a minor tune, but it's a new thing. You don't get the number anymore. So if 1559 was Final and we need to change a constant, you need to create a new a EIP to change that constant. It makes the most sense for core EIPs to wait until they're on mainnet before they go into that phase, because it would suck to have the EIP go Final and then you're not able to change it because it's already done. Basically, we're trying to avoid that. I don't know if you guys all remember this, but the Keccak-256 vs SHA3 situation where Keccak-256 was standardized. Everybody thought it was done. But it wasn't actually Final in terms of the standards organizations, like, whoever does the crypto standards. And then Ethereum was like, "okay, we're using SHA3," and we launched. And then at the very last minute, the crypto organization, I forget what they're called, was like, "we actually want to change this one little thing." It was a tiny change. But it is totally incompatible with the SHA3 that Ethereum launched with. And so now we have Keccak-256, which is not even a standard. It's just a thing that everybody thought was going to be the SHA3 standard and didn't actually end up being the SHA3 standard. And so we want to avoid that situation. And so one way to do that is to make it so things aren't final until they're live. So we can make those last minute changes and not have to worry about running occlusions and all that.

**Hudson Jameson**
But if we do it the way we're currently doing it, we won't be able to make those last minute changes without breaking testnets along the way, or having to rush client releases. Basically, the intention is good. I think in practice, it's going to be hard to break old habits this quickly.

**Micah**
So I can appreciate that. And so that's why I was asking if people are disagreeing with the ideal long term process, or is the fear that given a Ethereum history and people's historic behavior, we're worried that the current process will not equal the process we want. It sounds like the latter.

**Hudson Jameson**
It is the latter, mostly. There are some ways to tweak this to correct that, I think one of them being to rename Last Call. So basically, because it's been abused so much, just rename Last Call, but then have the real definition be what it is, like what you've described, which is very few changes, except for security vulnerabilities during the Last Call phase. But then that doesn't solve the problem of the Review status being an indeterminate amount of time.

**Edson Allyon**
Is that really an issue?

**Hudson Jameson**
For people who want to review at the last minute. There are some people who look at the RSS feed for Last Call. And that's when they start to look at an EIP.

**Edson Allyon**
I think the solution is just having RSS speak for Review instead of one for Last Call.

**Micah**
Do we know if there's more than one person that uses the RSS feed?

**Hudson Jameson**
Yes, I know two. So that could mean that could mean that there are more than two. So I don't know.

**Micah**
Yeah. I was just wondering if we're optimizing for the right crowd?

**Hudson Jameson**
Well, yeah, I get I guess you're right.

**Micah**
I honestly don't know. Maybe there's thousands of people who subscribe to the RSS feed. I know one.

**Hudson Jameson**
It's just the statuses is the thing. The status does indicate people rushing to review it, and then they start to disagree with it, even though they're not looking because who's looking for a security vulnerability in the last 14 days? I don't think many people are.

**Micah**
So I think the real problem here is this. In my experience, the vast majority of EIPs get a grand total of one to two people looking at it right up until a bunch of people need to implement it. And then you have a thousand people looking at it. And so when a thousand people start looking at it in the Last Call phase, then you get a lot of feedback. And if you somehow get a lot of people looking at in the Review phase, like with 1559, then you get a lot of feedback in the Review phase. Actually, 1559, I got a lot of feedback in the Draft phase. So I feel like we have these statuses that are meant to give people information, but I don't feel like they're particularly functional in achieving that goal. People are not looking at them.

**Hudson Jameson**
I would lean toward this to help with the fact that to basically stick with somewhat of the status quo, but to try to also push best practices would be to keep Last Call's definition as is, pretty much, because it doesn't include all the security vulnerabilities right now and move it to DevNet phase. And then public testnet doesn't include an EIP status beyond... but then that leaves public testnets to not have an EIP status. That's the problem, I guess. Yeah.

**Pooja Ranjan**
One more thing I would like to add here is generally, the definition of Last Call for that is [unclear](https://youtu.be/fKQVb-s0Tzs?t=1128). So one correction there would be a minimum of 14 days would be good. But you know, if they want to keep it in Last Call for over a month, because when it is on testnet, they believe it is like [unclear](https://youtu.be/fKQVb-s0Tzs?t=1139). So I am not very sure that we should put the Last Call status in DevNet phase.

**Micah**
I would be fine with getting rid of that 14 day thing. I've never really liked it personally.

**Hudson Jameson**
That would be okay. But I think the other thing that's messing me up here that makes it harder to find a solution is the fact that the definition for Last Call is the same across ERCs and core EIPs. And if that wasn't the case, then things would be easier.

**Micah**
I mean, just kick ERCs out of the EIP repository. That solves a lot of problems. And a lot of my problems, too.

**Hudson Jameson**
If we can start paying for editors, I'd be okay with that plan. And I actually talked to a project I can't name who said that once they have enough funding, they want to give money for EIP editors. So that's that's kind of part of another piece of this update, I think.

**Micah**
They haven't been watching a food token of some sort, have they?

**Hudson Jameson**
Not quite, no.

**Micah**
It's unfortunate. That would mean they actually have money.

**Hudson Jameson**
Yeah, anyway, I think I need to think about this more personally. So if we don't make a decision today, I'd be happy with that. But to think about this more.

**Pooja Ranjan**
I'm also fine with not making any decision. I just wanted to bring it to your attention. We had this discussion that we are not following the process, or people are not aware of the process, or there are some changes that we should be bringing to the process.

**Hudson Jameson**
Oh, yeah, that sounds okay. I have it on my to do list to make a comment on that issue in the next week.

**Pooja Ranjan**
Okay, so I'm going to keep this item on the agenda for the next meeting as well.

**lightclient**
Thanks. All right. If I can just say one more thing on that. I think a lot of people don't understand the latest EIP process. And I think that was incredibly clear with 2315. A lot of people still thought that the status of the EIP kind of meant how far along it was in the governance process. And people were all like "oh," 2015 was still in Draft. We didn't realize was going into a hard fork." And you know, that's maybe not the best argument in the world. There's probably a lot of documentation that it was going into hard fork. But I think that having this thing separated caused a lot of confusion for people who don't reasonably closely follow CoreDevs.

**Micah**
Yeah, I'm not a hard fork coordinator, so it's not my purview. But I do support the hard fork coordination process requiring that if you want an EIP included, it's got to be in the right phase. You can't include Draft EIPs in an upcoming hard fork.

**lightclient**
I just don't understand what the benefit is of separating these two processes, because for core EIPs, we're kind of saying that they have to be these things to go into these phases. And we separated two processes, but we're still making them forced together.

**Micah**
So two reasons. One, it's a unidirectional connection, instead of a bi-directional. So the hard fork coordination process points at EIPs; EIPS do not point back. And so the EIP process can exist entirely without knowing hard fork coordination process. And that is valuable because of politics. The EIP process, being purely technical, allows us to move forward and ignore politics, and anytime someone brings them up, we can tell them to go away, go to the hard fork coordination process where politics are handled. And that is very valuable, especially given that we are already massively understaffed to actually do anything with EIPs. And being able to tell people this is not the right place for governance discussion is very valuable.

**lightclient**
I really don't see how this is that different. Because in my mind, the only difference would be that if you want to move to a Final state, or we add a new state that says it's going into hard fork, a new status, to me, the only difference in what we're doing is that they need to provide a link to an AllCoreDevs decision that says, "this is going into a hard fork." And then as an editor, we say, "okay, yep, that checks out, I looked at that link, it's going to hard fork, I'll validate the status." And to me, that just makes everybody's life easier and doesn't make our lives harder.

**Micah**
So we ran into this a couple of times with EIPs in the past, I believe, where the governance debate ends up spilling over into the EIP process and being very distracting for the EIP editors. And the reason for that is because at some point someone updates an EIP, and it now says, "going into hard fork x, going into Berlin, going into London," whatever. And as soon as that happens, everybody shows up in the EIP repo and starts commenting and starts to make pull requests to remove that, etc. When that is handled elsewhere, it makes those people go elsewhere when they want to do their debating and their harassing and haranguing.

And so James can deal with that until he quits and hands it over to Tim, who can deal with that until he quits and hands it over to someone else. And the editors, hopefully, can stick around and not be driven away by the massive debating and problems that people cause when they see this stuff. Having a clearly separate spot for them to go to that's not here. Not here. Not these people. Don't distract these people. They are doing real work. Go distract those people whose job it is to deal with that problem. By keeping it very clearly separated, it makes it easier to draw a line in the sand and say, "No, that goes over there." Whereas if the two are intertwined, then it's much harder to stand up and say, "This is not the right place," because they're like, "well, it says right there, it's going to Berlin. So clearly, this is the place, I need to change that. I need to submit a pull request to update this EIP, that's not going to Berlin" or whatever. That's my reasoning. I really like having the shield, basically. So James is able to be a shield for the EIP process, because we have this very clear bucket of responsibility.

**lightclient**
Yeah, I mean, I haven't really experienced that. So obviously my take is going to be different. But I can understand how that is frustrating as an editor. I'll just say my two last points, I think that one, if we design the process in the right way, I feel like we can use the process as a shield. Still, I think that we should be able to say, "This isn't the place to discuss this." We don't choose what goes into hard forks. If an AllCoreDevs decision says that the status gets updated, we update the status. That's it. Go argue about that in AllCoreDevs, wherever else, I don't see why that's that different than just saying this isn't discussed here, because it basically still isn't. And then the other thing is that, I feel like we're optimizing for the 5% of EIPs that have a lot of issues. And by optimizing for those EIPs that have issues and a lot of people fighting for them, we are really degrading the experience for everyone in the community and for the other 95% of EIPs. Because a lot of people just want to go and read about an EIP and know what the status is and do it all that from a single page. And if it's just incredibly frustrating to look at an EIP and not know how far along in the governance process it is from its site. That's why I think I said from the very beginning that at minimum, we should also include as a courtesy, what the hard fork status of EIP is, even if those things are still separate, the specification and everything.

**Micah**
So my opinion on the last point is that I think the real issue here is that people are using the EIP as the center point. And I don't feel like it should be. The EIP should be a technical detail, not the the center point. And unfortunately, this is not how things been handled historically at all. This is very much not how things are actually done. But I do think that it'd be great if instead of when someone wants to ask what is this new fee change, they don't go look up or get linked to EIP 1559. They get linked to the resources page that Tim put up. It has links to some blog posts; it has links to Berlin hard fork; it has descriptions of the EIP designed for certain audiences. It's not just the technical specification. I feel the vast majority of people, the technical specification is not the right place for them to start learning about an EIP or talking about an EIP or anything like that. It's one of those things where there's 10 people who actually read the RFC for email addresses. But no one goes to the email RFC to learn about email or learn about how to send an email or how to use email or anything like that. There are probably a few hundred people in the world who have ever actually read that RFC front to back. I would like if we can get there, but maybe I'm being overly optimistic. Just an optimistic goal.
3
**lightclient**
I totally understand that and definitely agree that that's probably the long term goal. I just don't think that we are close to that. I think that the number of people who are really involved in this process are still, I mean, it's so ingrained that if you're working on a low level of Ethereum, you're gonna go look at the EIP repository to understand changes. And we just don't have the resources to have every single change have a resource page and have write-ups and all of these things. And it's just a lot to ask for every single EIP to have that many resources. So that's why I feel like in the short to medium term, we should keep things small.

**Micah**
That's a very compelling argument. You are right. WWDC and IETF they've got lots of resources when there's a browser change, for example. There's a spec for it, and there's like 10 people who actually read that spec, but it's listed on CanIuse.com and 400 other webpages, and people blog about it. And there's almost no one who goes to the specs repo to learn about upcoming changes to the browser APIs. But you're totally right. It's because they have hundreds of people working on every single change, not two. And so maybe the issue here is we don't have the funding or the resources to actually achieve a goal. And as a result, we're trying to achieve an unachievable goal, which just puts us in an even worse place if we didn't even bother trying.

**lightclient**
I feel like it's gonna happen naturally. Because if you just look at how EIPs have changed over the last 4 years or so, you look at EIP 7, or whatever delegate call is, and it's 50 lines, and there's just nothing there. And now, we're looking at some of these later ones, like 3074, it's really beefy EIP. And if that would have been proposed in 2015, it would have been just like, "Oh, we talked to this was a good idea, let's just throw a couple lines down, and then we'll just talk about it on IRC or Gitter about how to implement it." And in five more years, I'm guessing that maybe every EIP will have a 1559 style resource guide and all that stuff. Maybe it'll be 8 or 10 years. I'm not sure. But I think that'll happen naturally.

**Micah**
I'll think about what you're arguing here. It's very convincing. It's a smaller resource pool.

**Pooja Ranjan**
Okay, so one last question I think I may have on this topic before we move on. Although I know this is not an AllCoreDev meeting, and this is not like we are discussing the Berlin upgrade here. But it's a question to EIP editors. Right now, all the proposals of Berlin are on testnet. And as far as I know, there is only one EIP out of four which is actually in Last Call, and the rest all are in Review. Is it okay to ask the author to change it to Last Call at this point in time?

**Micah**
If they don't want to, I'm also okay with that. It might help if we said that EIP 1 just gets rid of that and makes it more clear the 14 days is a minimum, not a hard requirement. And then maybe in the future, we can talk about removing the Review end period and just have it implicit.

**Pooja Ranjan**
Okay, sounds good.

**Micah**
I think that's the push back here is that 14 days, because people be like, "Oh, we don't know if it's gonna release in 14 days."

**Pooja Ranjan**
So I'm gonna bring it back on the agenda in the next meeting is well.

**Micah**
If we're moving on to the next topic - are we done with this one?

**Pooja Ranjan**
I suppose so.

**Micah**
Since Hudson has to leave in a few minutes, you guys mind if I interject a quick discussion item that I forgot to put on the agenda?

**Pooja Ranjan**
Yeah, sure. Please go ahead.

**Micah**
So for reasons that I don't fully understand, the burden of reviewing EIPs has increased. It is now to the point where I am unable to keep up while also continuing to sleep every night. And so I think starting probably this week, I'll stop reviewing ERCs just because I need to drop something. And it's either drop ERCs, drop sleep, or drop eating. And I've decided ERCs, they drew the short straw. So either someone else needs to pick up reviewing ERCs, or we just need to accept that we're going to go back into a state we used to be in where EIPs were sitting in a waiting for a reviewer for months to years. Unless someone has a very novel solution.
3
**lightclient**
I heard that people want to remove them from the EIP repository.

**Micah**
I've heard that, too.

**Hudson Jameson**
I think while we find a solution, if it goes back to where it was before where we're not completely up to date on it and we have a lag behind, that's not the worst thing in the world, because that's kind of what has to happen. But we should work towards recruiting more editors. I still haven't cracked that code. So yeah.

**lightclient**
I'll definitely keep trying to get those things reviewed. I feel like usually every week or two, I try and carve out a few hours to really go through stuff. It's just generally there aren't things left over because Micah reviews everything within about 30 minutes of it being posted.

**Micah**
Pooja, I promise to stop doing that.

**lightclient**
I mean, yeah, if there's open stuff, I usually will get to them after a week or so. So I don't think we're gonna get back to the place where it's once a month without reviews. But I'm definitely a lot more open to removing ERCs from the EIP repository, probably not something we can decide right now. But I know that in the past I've been against it. I don't know if it's just Micah is really getting in my head and he's starting to control my thoughts, but it's really dawned on me in the last six months.

**Micah**
You're starting to figure it out.

**Edson Ayllon**
I think I think it's fine that ERCs are in the EIP repo.

**Micah**
I haven't gotten in Edson's head yet.

**lightclient**
Yeah, I think the thing that just really pushed me over the edge is that they are so different than core EIPs. And it's just so weird to have the two intermingled. So I would be very okay with having an ERC repository.

**Micah**
And the skillset for reviewing ERCs is very different than EIPs. I happen to have both just because of my history and came up through the dev side and then moved over to CoreDev sort of side later. But I definitely know of people who would be very good at reviewing ERCs and terrible at reviewing EIPs. And I also know people who are very good at reviewing EIPs, and I would not want them reviewing ERCs.

**Hudson Jameson**
So should we recruit before separating or separate then recruit if we decide to do that? Theoretically, not that we're making a decision today.

**Micah**
I would separate then recruit, just for the reason I just said. The skill set is so different that you're going to want to look for different people, and it's much harder to recruit for the core EIPs. The technical knowledge you need needs to be really deep.

**Hudson Jameson**
That's true. Okay. We need to figure out how hard it would be to separate and propose something before we decide, I think.

**lightclient**
I think the biggest issue is going to be that we're going to destroy every permalink to the GitHub repo for ERCs.

**Hudson Jameson**
Yeah, that's a big one.

**Micah**
Well, so, in theory, people should not be linking to the GitHub repo. They should be looking to EIPs at ethereum.org. I've beenn telling them this for a while. Maybe we just say, "Hey, they're all at the other place. Not my fault you went to the wrong one."


**lightclient**
What we could do is we could just replace every ERC with - like I think the ERC 20 token was named differently, and then we've got a placeholder there, we could do that for every ERC and keep that for three to five years. And I don't think that that would really impose much of an issue, because who's actually going through that list of files? Not many people.

**Hudson Jameson**
It's more the discussion links. But we wouldn't be deleting PRs or issues, would we?

**Micah**
No. We don't have the ability to do them.

**Hudson Jameson**
Got it. Okay. Sounds good. I've got to jump off. I'll think about that part more. Thanks, everyone.

**Edson Allyon**
Appreciate it. Alita's here. Did you want to go back to the bot?

**Pooja Ranjan**
Yeah.

**lightclient**
One last thing on that real quick. Theoretically if we did want to do that, does anyone have a theoretical path to making that happen? Who needs to agree to that to make something like that happen?

**Micah**
The benevolent dictator of EIPs.

**lightclient**
So we're gonna do it tomorrow then.

**Micah**
Yeah, I don't know. So it would be people who actually look at ERCs are me and, in theory, more EIP editors that are very few and far between, and then there are the authors of those ERCs themselves. And then once the ERCs get popular, there are the people who are looking at them to implement. Those are the three people I have seen show up in the EIPs repo related to ERCs. These are the three types of people.

**Pooja Ranjan**
I have been looking at it recently just only for one thing - if there is a status review or they are trying to escape it right from Draft the last column. That's my only comment for any ERC that I have logged into so far. Maybe this is something that we could bring it on the next call and as an item itself. Do we want to separate the EIP and ERC, if people are open to discuss that.

**Micah**
Sure. Just so people can chew on it, the reason I want them separated and not just say, Micah reviews core EIPs and someone else reviews ERCs is that GitHub subscriptions. I subscribe to the entire EIPs repository. I to get an email notification for everything. And right now that is about half ERCs. And it'd be nice if I could not subscribe to the ERC half. And I don't believe there's an easy way to do that without splitting out into a separate repository.

**lightclient**
I think that's a general argument for a lot of issues that we have with governance is that a lot of people don't want to contribute because the noise is so loud. But with them separated, I think that there's a lot less happening in terms of core EIPs. And so that may allow a larger number of people to actually review everything that comes through, because they feel comfortable doing that. And then maybe people who want to look at ERCs will feel comfortable. Because this is ERC specific; it's a little more friendly. They don't have to deal with the scary CoreDevs.

**Micah**
That's a very good point.

**Pooja Ranjan**
Okay, in the essence of time, let's move on to quickly go over a few other items. And I will definitely add that on the agenda next time to have a proper discussion on this topic, separation of EIP and ERC. And we are coming back to Alita's item, I think we have discussed it briefly, I want to just give a chance to go ahead with the next items listed for today. And if we have some time, we'll go come back to item number one again to see if there is any progress to be reported.

## 4. [Progress on 'canonical source for EIPs'](https://youtu.be/fKQVb-s0Tzs?t=2512)

**Pooja Ranjan**
So the next item on the agenda is progress on canonical source for EIPs. I believe Brent has something to talk about it.

**Brent Allsop**
Yeah, the meeting's way long, so I just want to mention that we forked the repository, and I'm working with one of our part-time engineers to figure out the bot system that makes the eips.ethereum.org so we can make a mirror of that site. Once we've got that running, we're going to start making the changes we're proposing. And I'm proposing those in the doc. So just wanted to let everyone know I'm pushing in that direction. That's the progress we've made. So that's all I need to mention today. We'll talk about it later.

**lightclient**
Did you have a specific question? Because you were mentioning something earlier.

**Brent Allsop**
well, I just need to get more educated about how the robot system and the EIP GitHub repository works, what robots are involved in it. But I can do that on my own time with my part time engineer, and then do that. So we don't have to do that in here.

**lightclient**
Okay. I was just gonna say that it is mostly Jekll. So Jekyll will basically compile the EIPs into static website files.

**Brent Allsop**
Yeah, my part time engineer and I are looking into that, we're figuring that Jekyll stuff out. So we'll get there, it'll just take it a bit. But thanks for the support. We're working on it. So thanks.

**Pooja Ranjan**
Thank you, Brent, for that. So coming back to item number one now, which was on the progress on EIP GitHub repo, now that Alita has joined, Alita, if you have anything to update on that. And we know that this is already in a pull request on EIP GitHub for editors to review. Do you want to add anything on that?

**Alita**
No, not really. I think that pretty much covers it. It's in review.

**Micah**
Can you ping me once you - I noticed you're making a bunch of changes. And so I kind of stopped checking back. Can you just @ mention me on that once you're to a point where you think you're done with all your next round changes and I can review it again?

**Alita**
Yeah, so actually, that is one thing that I added you on. Did you want tests? I wasn't really clear.

**Micah**
I mean, I always want tests. But I also have been an engineer long enough to know how much of a time sink that can be. And so the question is, is it worth the time? And I don't have a good answer to that one. In your opinion, how easy is it to test GitHub actions? This is one of the things we're gonna have to spend like two weeks just figuring out how to test the GitHub action in an automated fashion or something like that.

**Alita**
So I can build like a custom system that'll just do it like a mock, basically, which is what Gest is for, anyway. And what that means is basically just creating some basic, not necessarily perfect reproduction of a PR, just to test certain behaviors. The biggest thing is there are a lot of edge cases to do. So there are bugs with the current bot, like a lot of them, I think.

**Micah**
Yep. Like it only runs half the time.

**Alita**
Yeah, there are a lot of things that are wrong with it, which admittedly, writing tests would be a really great opportunity to then test and fix those edge cases. But also, the bot seems like a perfect candidate for tests, to require tests, because no one's gonna notice when it tests when something is going wrong. But anyways, it will take me about one to two weeks to get a solid baseline of tests going. So if you all are okay with that, then I think it's fine. And I can do it.

**Micah**
So my feeling is that one, two weeks aligns with where my gut was, just kind of looking over your shoulder. That's what the order of magnitude is. This is almost a question of should you test your test sweep? Because the bot is effectively just a kind of a test runner that is supposed to building an automated CI process? and spending one to two weeks? We can definitely test your tests. It's just a question of is it worth the time. The time be better spent making the bot actually do better, making it do more things. There's a list of things we'd rather have the bot do. We have one or two weeks of engineering time. We can either sink it on making sure that the bot is robust, or we can sink it on making the bot more feature rich, and I'm on the fence as to which is more valuable.
3
**lightclient**
I would like to see just a couple of really basic tests of the EIP-checking functionality just to make sure that, okay, for these simple cases, this makes sense, you know, did they change the status to review? If so, then that means the EIP editor - I don't know what the control flow exactly is, but just a handful of tests. I don't expect every edge case to be tested, but just a few sanity checks would be valuable, and then having the structure for writing other tests in the future would be nice.

**Alita**
Okay, that makes sense as a first as a first go. And then, obviously, I'm happy to continue work on it as well, if you all wanted to keep me on with that. But in regards to building out tests versus - well, first off, for this PR, it would make sense to build out the infrastructure for tests, not necessarily tests themselves, and I can get that done pretty quickly. But I think that the bot itself really needs very comprehensive tests, just because it's going to be really hard to build out things when the bot needs to be on point. Otherwise, it's gonna cause problems, right? Because if we're just auto merging things, because of some bug, then that's going to mess up the repo. So I think that we would be better to be sure than to have problems with this sort of thing.

**Micah**
Yeah, that's a good point. I forgot that with this particular bot, a failure in the bot results in bad things happening. It's not just like, "Oh, I didn't help, so a human can step in." This is "Oh, the bot actually made things worse." That pushes me more towards the Yes, we should test more stuff.

**Alita**
And then also when it comes to the actual code itself, for some reason - I think it's because it was reporting from Python or something like that, the logic was pretty tangled. So there is still some work to do as well to make it expandable. Because right now you can expand it, but it's just gonna cause problems.

**Micah**
Sure, getting the infrastructure up in a place that the rest of us can iterate on is a very valuable first step.

**Brent Allsop**
So you're talking about creating a mirror of the EIP repository on a server, right? And that's exactly what we're building. So, yeah, we could do all that stuff on this repository that I'm working on. And we're going to be tweaking, getting the Jekyll script and everything running on a server. And that'd be a perfect place for Alita to run her tests and develop testing and make sure everything runs on this fork of the EIP repository. And we can keep updating that fork and run the scripts and develop tests and stuff like that. But anyway, yeah, I'd like to get our part time engineer involved and help with some of that. We can do that.

**Alita**
So we don't need a server or anything for these tests. They are straightforward and well-defined for GitHub actions, so it can be done in a single repo. So yeah, wouldn't really be pertinent.

**Brent Allsop**
But is it going to be taking action on live data and stuff like that?

**Alita**
I'm not totally sure what that means. But with the current behavior, it doesn't need anything else. No.

**Brent Allsop**
But is it going to be taking action on live data and stuff like that?

**Micah**
Yeah, you can test infrastructure up at least. And then a few sanity checks on the most egregious things like things that we definitely want to make sure we get blocked, such as, is one of the authors the pull request author, or did they prove it? Like, that's kind of the one thing that it does good. And is it not in the wrong status? If we can get those two things tested, at least on the surface, that would go a long way, I think, and satisfy me.

**Alita**
OK. That's achievable. I'll let you know when it's done. Thank you.

**Micah**
We can't merge this until we're ready to put it live, right?

**Alita**
I mean, you can always disable the action. So you can merge it and then disable it.

**Micah**
Is it possible to manually run the action, disabled like that?

**Alita**
No, because it's triggered based off the pull request itself.

**Micah**
Does the action support some manual triggers?  Like we started out as a manual trigger.

**Alita**
I'm not sure about how to do that.

**Micah**
So if that's possible, if there's a manual trigger, and I want to say there is - I think I saw a repo that had a manual trigger GitHub action. If there's a manual trigger, then we could merge it and then use it manually when the current merge bot fails, which is pretty often because when it fails, I'm currently closing the EIP and reopening it. If instead, I could just go and say, "oh, I'll try Alita's bot" and click the button there. I'm already sitting there watching it. And so if it does something wrong, I'll be there to catch it and fix it. And so that might be a nice way to get kind of tested production, so to speak.

**lightclient**
Theoretically, there's definitely ways where you can tag a bot and give it a command. I know Boris has a lot of functionality like that, where you can tag Boris and say, "Okay, once you know the other people on this approve, go ahead and merge it."" I don't know how hard it is to implement functionality really simply. But it can be done.

**Alita**
Because we're short on time, I wanted to hop on one other thing. Did you all want me to go out and build the botinto a separate repo, and I can just do it, I can set it up, and then Hudson or whoever has permissions, I can just give over control or something like that?
M
**Micah**
I'm on the fence. Lightclient half convinced me. The plus side of having it in the EIPs repo is that it's right there. And the same people who have write access to the EIPs repo would have write access to the bot. So when we, the people who have write access to that repo, notice it doing something wrong, or we want to make a quick patch, we know we have permissions. And so if we add new editors, those editors will automatically get the access rights. Having a separate repo is just like a modularity and keeping separation of concerns. That doesn't make more sense. In that regard, I'm on the fence. If other people have really strong problems, it's definitely one down on either side.
3
**lightclient**
I feel pretty strong that it should be in its own repo. I think it's several thousand lines of code. And I don't really want to mix a bunch of PRs between the two things.

**Alita**
I agree with lightclient. In addition to that, it'll make it a lot easier to do COI for the bot itself.

**Micah**
55:36
Yeah, okay. I'm convinced. Using my own argument against me: tha was smart. I just argued earlier that we should separate ERCs and EIPs so people could subscribe more specifically, and having bot PRs go to the same place that your EIPs PRs go would not help with that. So yeah, it's a separate repo.

**Alita**
Did you want me to do it? Or were you waiting for someone else.I know who it was. But I'm forgetting.

**Micah**
James is the one who has the ability to create a new repo in the Ethereum organization, which ideally is where this would live. In the meantime, if you just want to put it in one of your own repos, it's pretty trivial to move it over once we actually do get a more permanent location. So I would say if if you want to split it out into a separate repo, just under your username in GitHub, we can use that for now. And then once James can create an Ethereum/EIP bot repo, then we can move it there. That'd be what I propose.

**Alita**
All right. Sounds good.

**Pooja Ranjan**
Thank you Alita, Micah, and lightclient discussion, it seems like we are going to see some more actions. And we would want to keep this in the next meeting item as well. So we'll wait for your progress there. I think we are over time. I wanted to quickly cover on the EIP editors onboarding thing. We just have tried to answer most of the questions on the EIP Discord itself. But if you could not get answer, I have created this new role in the ECH Discord as EIP editors aspirants, and if you are not there, you want to be on part of there, if you have any further questions, please reach out to us. You can DM to any of the members of the of the Ethereum Cat Herders or post your question directly in the general section of the ECH Discord. That was the last item on the agenda. Thank you, everyone, for joining us today.

See you all and still on March 24. Thank you.








# Attendees

* Alita
* Brent Allsop
* Edson Ayllon
* Hudson Jameson
* Jim Bennett
* lightclient
* Micah Zoltu
* Pooja Ranjan (Host)



# Date for Next Meeting: November 18 at 1500 UTC
