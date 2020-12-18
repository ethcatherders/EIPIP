# EIPIP Meeting  23 Notes
## Meeting Date/Time: Wednesday 16 December at 15:00 UTC
### Meeting Duration: 35 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/44)
### [Audio/Video of the meeting](https://youtu.be/B8uSDIYznuY)
### Moderator: Hudson James
### Notes: Jim Bennett

----
## DECISION ITEMS

**DECISION 23.1**: If you move things to Final, there's not a requirement for the yellow paper to be updated [see](https://youtu.be/B8uSDIYznuY?t=1377)

**DECISION 23.1**: Plan to have someone update the yellow paper or to make another source of truth in bulk in the new year.  [see](https://youtu.be/B8uSDIYznuY?t=1377)

**DECISION 23.5**: Tentative decision to publish EIP status blog & EIP editor roles & responsibilities blog ojn the Cat Herders blog as well as Cat Herders Medium. Waiting for Edson to make a final decision. [see](https://youtu.be/B8uSDIYznuY?t=1860)

## ACTION ITEMS

**ACTION 23.1**: Put on the agenda for the New year the possibility of creating a bounty for an authoritative, single source of truth place that defines the current state of Ethereum. [see](https://youtu.be/B8uSDIYznuY?t=1287)

**ACTION 23.2**: James will do an ETH 1.0 specs repo list of EIPs per fork eventually. [see](https://youtu.be/B8uSDIYznuY?t=1377)

**ACTION 23.3**: **Micah Zoltu** to update the issue on implementation section in EIP and close it. [see](https://youtu.be/B8uSDIYznuY?t=1509)

**ACTION 23.4**: Brent to create a temporary Google doc to help cordinate the clean up and documentation of all duplicate Ether Informaiton. [see](https://youtu.be/B8uSDIYznuY?t=1660).

The Google doc has been started: [EIP Single Source Cleanup](https://docs.google.com/document/d/1hUpMQh9gA5z3WSDvXKqU_CS6g3Y0hugJZHDYQdKxot8/edit?usp=sharing)

----

**Hudson Jameson**  0:00  
## 3. EIP Repo cleanup

All right, I think we're live. Hello, everyone, and welcome to EIPIP meeting number 23. We have a few agenda topics today. The first two were ones that lightclient put in. So instead of us going to those first, until lightclient shows up, we'll skip them. And then we'll have them at the end, regardless of if he's here, for anyone to comment on. So we'll start with [EIP Repo cleanup](https://youtu.be/B8uSDIYznuY?t=33), item number three. What's that one about?

**Pooja Ranjan**  0:41  
So in the previous meeting, we decided that we should continue this task of EIP Repo cleanup that we were doing earlier, now that the new board has already taken care of a major part,  like if an EIP is old or redundant as is mentioned there, it is closed after a certain period of time. But we realize that eips.etherium.org, they have this list of EIPs, and they are still in the same status, even though the issue and PR are closed on GitHub, the status are not getting changed for EIP. And I was doing a quick analysis of what are the EIPs and statuses. I'm going to share a [sheet in the chat](https://docs.google.com/spreadsheets/d/1KnsLDuVr9F7-vE3aEQFhWmmyktZmMIAMxSSh1Snhm8k/edit#gid=1016682054). So it basically lists all the EIPs that are present in eips.etherium.org. And it lists a total of 312 EIPs. So in the sheet, if you can go to tab number two, pivot table two, you may be able to find the list of EIPs divided on categories. And if we give it a look, we see that there are 229 draft status EIPs there out of 312. So it's a major chunk. And we Cat Herders are trying to reach out to authors of these EIPs and see if they are still interested in either pursuing the EIP, if it is valid, and if it is not valid anymore, we would request them to change it to the status of Withdrawn. So in the tab "EIP status change reached December 2020," I have populated with some of the EIPs where we already have reached out to the authors and have requested them to change the status depending upon the conversation that we had. Unfortunately, it's not a very big success so far. Even if we have asked them to change it, it is still in the same status for awhile. So I was wondering what could be the right next step to move forward,  and we should be able to move all the EIPs in the right status.

**Micah Zoltu**  3:29  
My personal strategy has been to wait for the six-month timer to tick through all of them and then just mass-close them all, or mass-stagnant them all, I should say.  That's still like four months away, I think.

**Hudson Jameson**  3:45  
Yeah, we can be proactive if we want or just leave them stagnant. It's kind of whatever. If someone wants to take that initiative upon themselves, they can for sure and contact authors. But whether or not it's really necessary, I'm not sure.

**Micah Zoltu**  4:06  
I would say, if we have author's agreement to mark it as abandoned, I'm personally okay with just doing the the actual PR to do that, as long as we have credible belief that the author actually agrees. Normally, the normal process would be the author sets to abandoned, but I'm okay if you contact the author on Discord, and they're like, "Yeah, yeah, mark it as abandoned." I'm personally okay with using that as agreement. I don't know about others.

**Pooja Ranjan**  4:35  
Yeah, actually, I was coming to that point. We are reaching out to authors, and I have been reaching them for some of the other tasks, and during the discussion for some of the EIPs comes out that it is not valid anymore. I was wondering if it is okay for me or Brent or anybody who is in touch with that author to just create a pull request? By that, we are also giving the opportunity to an author. First of all, we are creating the pull request, because we have data, we have reached out to the author, and we have their permission. But in case of no verification of that, if we create a pull request, we give, say, 14 days time for the author to respond back if he does not want it to be withdrawn, or he has changed his mind, or something like that. Then he can mention that as a comment. And after that, we would like to mark that as withdrawn. The only concern that I found there was if any of the Cat Herders are taking that step, they would be added as a contributor. I'm not sure if it is ethically very much right. But if an EIP editor is willing to take that, I think that should be okay.

**Hudson Jameson**  5:57  
Yeah, or we could just say that you don't have to be a contributor to do a PR for someone else, which really, do you have to be added as a contributor if you do a PR for someone else's EIP? Or is that just more common, that's what commonly happens?

**Micah Zoltu**  6:16  
You do not have to be a contributor to do anything to open any PRs. There's no technical restrictions, I should say. I don't know if there are social ones.

**Pooja Ranjan**  6:26  
Right. So I was thinking, I mean, I'm not sure, maybe you can help me understand this part. If I go ahead and create a PR for any EIP in which I have information that the author has mentioned that he is not willing to pursue it anymore, my understanding is I would be added as contributer to that once that PR is accepted, but that PR is accepted at this state as Withdrawn. So in my mind, that should be fine. Just wanted to raise it as an ethical concern.

**Hudson Jameson**  6:58  
Yeah, go ahead, James.

**James Hancock**  7:00  
If you do a PR, then an editor still is going to be the one that has to merge it, which makes that totally fine. I just want to go through the different cases where I think this would make sense. If an EIP author, if you talk with them, they say, "Yeah, I'd like to withdraw this EIP or make it Withdrawn," then you making the PR for them, and then just mentioning that the author said that it could be, the author could always refute that that happened. So it's not really that big of an issue if if someone was doing it wrongly, because the author could just come back and say, "Wait, no, never mind, that wasn't the case." Or if the author says, like, "Do whatever status that makes sense." But if an author replies and says, "I'm just not really working on this anymore," then I don't really think that counts as Withdrawn. That, to me, sounds more like Stagnant. It should just default to going to Stagnant when the time goes out.

**Hudson Jameson**
Yeah, they could give their opinion, though, and just say I want to withdraw it. And that's all we're giving them the opportunity for.

**James Hancock**
Yeah, yeah. And so if they say that. But if I talk to someone, and then I hear from them,  I don't think that default means that we can withdraw.

**Hudson Jameson**  8:31  
Oh, yeah, of course.

**James Hancock**  8:32  
Like they have to say that they allow us, like explicitly say that they're okay with us moving their EIP to Withdrawn. It shouldn't be assumed or something like that.

**Hudson Jameson**  8:44  
Yeah, that sounds good. And then just to make sure I'm clear on this, Pooja, what you're saying, as far as being a contributor, you would do a PR that would attach your name to the EIP, but not actually write it down as a contributor to the EIP, right? Like as an author or anything?

**Pooja Ranjan**  9:03  
Yes. Yes.

**Hudson Jameson**  9:04  
Okay.

**Micah Zoltu**  9:05  
I think what she's probably referring to is in GitHub, they have a little contributor tag that shows up on people who have successfully gotten a commit somewhere in the commitment stream. That's just a GitHub feature.

**Hudson Jameson**  9:16  
That's fine. Yeah, I'm personally good with all that.

**Pooja Ranjan**  9:22  
So, if if there is a general agreement on this, I will have a list of EIPs for which we have already requested the author to change it or they they have agreed somehow, but maybe in absence of bandwidth or higher priority job or something like that, the DPS has not been created yet. So now I can go ahead and do that and adding a note to the author. So if you have a disagreement with this, please respond back within 14 days or something. Is that fair?

**Micah Zoltu**  9:55  
I think that's reasonable. So for a lot of these authors, having worked with some of them before, I suspect if you just create the PR and send them a link and say, "Hey, do you mind, can we get an approve on this," they will be more likely to do that and go and create the PR themselves, because you clicking approve is marginally easier than actually going through the effort of creating the PR itself. And so if you just create the PR for them, and then send them a link on Discord or Gitter or wherever you're contacting them and say, "Hey, do you mind clicking approve on this," I suspect most of them will be willing to do that, since it takes like 10 seconds.

**Pooja Ranjan**  10:34  
Sounds good to me. I will try to do that.

**Micah Zoltu**  10:39  
That lets us speed things up a bit, so we don't have to wait two weeks for them to decline. Because they'll probably do it right away, and then we can just merge it immediately. So that's easier.

**Hudson Jameson**  10:56  
Okay. Let's see. Do we go on to the next one? Or do we have any other comments?

**Micah Zoltu**  11:06  
Lightclient said he's not gonna be able to make the meeting. So we can go back to one and two, if you want.

**Hudson Jameson**  11:10  
Okay, let's do one and two.

## 1. [Handling Retroactive Changes.] (https://github.com/ethereum/eth1.0-specs/issues/12)

Let's do [Item Number One: Handling Retroactive Changes.](https://youtu.be/B8uSDIYznuY?t=678) If you [click on that] (https://github.com/ethereum/eth1.0-specs/issues/12) it goes to an issue in the Eth 1.0 specs where you said there was no dissent in moving EIP 26814 during AllCoreDevs number 101. The problem is, what does that mean? With the separation of EIPs and network upgrades, Final doesn't mean mainnet. Typically, this isn't a major issue, because we can use the upgrade tracker, and once it's scheduled and upgraded, it  is recorded during that transition, the EIP 2681 sets a limit on account nonces retroactively from genesis. Hmm. My guess is that a modification should be made to the yellow paper.

**Micah Zoltu**  12:00  
My feeling on this is that there's a whole set of EIPs that lightclient and Axcic would like to push through and I fully support. I don't think that we need a super formal process for this set at least. And I tend to be hesitant to generate super-formalized processes until they're needed. In this case, I'd say we just mark the EIP as final, and we're done. Updating the yellow paper,  we should probably do as well. And anyone can submit a PR to the yellow paper to do that. And I don't think that would get anyone into any trouble. But I don't know if we need a formal process here. I say just merge to final just like any other EIP, update the yellow paper like any other core EIP, and that's it. We're done.

**James Hancock**  12:58  
It might be as easy as just having a list of the active EIPs on mainnet in a table on the Eth 1.0 specs repo. So you merge it, you add it to that list, anyone who wants to make a client can just look through all of the EIPs and say "Oh, yeah, that's one."

**Micah Zoltu**  13:12  
Yes, a caveat there is that you cannot actually write a client from the EIPs alone because we do not have the original set of spec on anywhere other than the yellow paper. The yellow paper should already have the whole list integrated into it, in theory. If you have the yellow paper, you don't need the EIPs. And if you don't have yellow paper, the EIPs don't do you any good. Which is an unfortunate situation. In theory, the yellow paper is supposed to be updated every time there's a corporator call change. I don't honestly know how good we as a community have been at that. I don't know if anyone else does?

**James Hancock**  14:05  
Oh, pretty much all the precompiles that have been added since I don't think are in the yellow paper. You'd have to go to EIPs for those.

**Hudson Jameson**  14:12  
No, some of them have been added.

**Micah Zoltu**  14:14  
Really?

**Hudson Jameson**  14:14  
Yeah, there's been someone keeping up with it. Community members been adding them and they are getting merged every once in a while. I can't say it's completely up to date, but it does have a good number of the precompiles.

**Micah Zoltu**  14:27  
Okay.

**Hudson Jameson**  14:29  
My take as it shouldn't be required to update the yellow paper for it to go to Final, if that's anything being suggested, which I'm not sure if it is. But it should be encouraged if someone's willing to do that, I guess. And then Final doesn't mean mainnet. Have we changed that rule yet, or have we just said that?

**Micah Zoltu**  14:59  
"The final standard Final EIP exists in state of finality and should only be updated correct or added." That's what Final means. So it's nothing to do with mainnet anything anymore.

**Hudson Jameson**  15:08  
Okay, then yeah.  I see the concern now, more so. Yeah. For now. I like **Micah Zoltu**'s idea, what he originally said, I think we should go with that.

**Micah Zoltu**  15:35  
But it does lead into another discussion, possibly better suited elsewhere. But it would be nice if we had some team or group or something that makes sure there is one canonical source of the Eth 1.0 spec. I personally am one of the people in the medium-sized group who hates the yellow paper. But at least it is a single consolidated place that has the current Ethereum definition. It'd be nice if there was confidence that that was actually true, I guess, "Here is the current state of Ethereum defined" somewhere. Again, whether that's the yellow paper or purple paper or green paper, fuchsia paper or some specs repo like EIP 1 specs, two dozen maybe within a wiki or something, any of these be fine with me. But it would be nice if there was a single source of truth that defines what it means to be a client. That being said, I am way overworked. I think all of us are, so I did not volunteer.

**Pooja Ranjan**  16:42  
Just to add here, in the last meeting, even lightclient also mentioned that in the discussion. Like we have backup Eth 2 and Eth 2.0 spec repo, the current spec of our client. Could we have something listed here in at Eth 1.0 spec for Eth 1.0 chain?

**Hudson Jameson**  17:06  
This sounds like a really interesting thing to do, starting with this next Berlin hard fork and working backwards. So that would fall into the Eth 1.0 specs repo, which generally falls under James's stuff. But James, what's your load like right now?

**James Hancock**  17:24  
Oh, no, that makes sense. Putting all the hard forks up and retroactively, putting in Berlin and then putting in all the other hard forks and these are the EIPs and the block numbers when they came in, that stuff I was already planning on. What I don't really understand yet is what's the best version of how to keep, if we did keep something like **Micah Zoltu**'s saying on Eth 1.0 specs, what's the best way to do that that would allow it to be most likely kept up to date and easiest to be used?

**Micah Zoltu**  18:02  
I do not have an answer to that.

**Hudson Jameson**  18:04  
Yeah, that's another whole thing, I think.

**Micah Zoltu**  18:06  
The canonical problem. I mean, a sufficiently specific specification is called code. And so, by definition, just the Geth repo is arguably the Eth 1.0 specs.

**James Hancock**  18:29  
That's what I just don't know yet, is like, what would a list of EIPs that are supposed to be on mainnet be sort of enough? The yellow paper should stay probably where the yellow paper is, because people expect it to be there. There's some other things that probably [crosstalk] the networking protocol stuff like the EIP 64, EIP 65, EIP 67. Those things could probably fit, to0.

**Micah Zoltu**  19:07  
I think, as a user who has unhappily had to read the yellow paper many times over, the thing that I want that I always end up going to the yellow paper for and then when I get there, I'm like, "Oh, I wonder if this is actually up to date,"  and it makes me nervous,  is I want a reference. For example, gas costs. How much do things cost in gas today? I don't actually know if the yellow paper reflects reality right now. It might be close, maybe it's mostly right, I don't know. And there's no place I can go to get an authoritative answer to that, other than digging through the Geth and Nethermind repo and trying to find their gas accounting methods and maybe hoping they have a constants list somewhere in the repository. Those are the types of things that I really would like to see. Similarly, data structures for the structure of a block.  I can go to the yellow paper and try to parse that out of the mathematical notation. Or I can try to go on Stack Exchange and try to find someone who has defined what a block is.  But that's probably out of date by now, and so I've got try and find another other one. And so I end up trying to put together all these pieces of sources of truth where, okay, here's the yellow paper, but it's out of date, the Stack Overflow has slightly more updated and easier to read information, but it's out of date. And then the Nethermind repo defines blocks, but they're kind of spread out over 17 different files. And so all I wanted to do is figure out what is the shape of a block, like an RLP-encoded block. Show me that. There's currently nowhere to go that's authoritative. It would be nice, if there was an authoritative place that I felt like I could trust that is a) up-to-date and b) human readable. Yellow paper kind of half meets up-to-date and does not meet human readable in my opinion. And then all the other sources don't make the up-to-date, or don't make human readable. Again, I do not have time for this, I recognize this as potentially a very large task. And so I do not want to put it on anybody. One potential place is the Eth wiki. It is the third place that I go to look. And I don't know who's maintaining that, but it has some good info, but it's not always accurate. It's not updated.

**Hudson Jameson**  21:16  
Maintainership is up in the air right now.

**James Hancock**  21:24  
I could certainly coordinate and help make sure everything stays consistent. But I would need someone to help do a lot of the heavy lifting of actually getting all the work and the information written in.

**Hudson Jameson**  21:36  
I see this as a good bounty project. So we pay someone.

**Micah Zoltu**  21:39  
It's a lot of work.

**Hudson Jameson**  21:40  
Yeah. So we pay somebody to do it. And James is the project manager of it, kind of.

**James Hancock**  21:49  
Because I have enough knowledge of all the little pieces that I could keep them together, as far as what's supposed to get done and how it's supposed to fit together. And we could bounty off the rest of it or find someone who wants to spend three months.

**Hudson Jameson**  22:03  
Let's add that to the agenda for the new year. Or maybe even for next meeting to flesh it out just a tiny bit more, but maybe for the new year to figure out funding and maybe have an EIP editor fund that the Cat Herders control.

**James Hancock**  22:18  
Yeah, because that sounds like a good resource for developers.

**Micah Zoltu**  22:28  
I know I've personally needed this class of information dozens of times. And it's surprisingly hard to come by reliable info. So I would love it.

**Hudson Jameson**  22:43  
Okay, sounds good. In that case, if we are we done with this topic? That got a little bit off on a tangent, but that's good, because we're gonna bring it back in the next few meetings about this. But the decision made was basically that you move things to Final and that there's not a requirement for the yellow paper to be updated. But there's gplans for both James to do an Eth 1.0 specs repo list of EIPs per fork eventually. And there's also a potential plan to have someone update the yellow paper or to make another source of truth in bulk in the new year. Does that sound right, everybody?

## 2. [Implementation section in EIP](https://youtu.be/B8uSDIYznuY?t=1414)

Okay, next agenda item: [Implementation section in the EIP repo](https://github.com/ethereum/EIPs/issues/2940)

**Micah Zoltu**  23:40  
So this week, we can maybe speed through this one, if you don't mind. So Axcic took a politically correct approach to this problem and started with an issue and filed it and fast responses. And then I forgot about it. And then I went and took a more, let's say bold approach to this exact same problem. And I just submitted a PR to make this change. No one said no to it after two weeks, and lightclient said okay, and so I merged it. I later realized it just now that I had forgotten this issue was created. I probably should have let lightcleint do it the politically correct way rather than the bold way. But yeah, so it's already done, basically.

**Hudson Jameson**  24:30  
Oh, okay.

**Micah Zoltu**  24:31  
We can revert it if there's discussion prior to.

**Hudson Jameson**  24:35  
I'm fine that it went through, personally. Yeah, just let him know.

**James Hancock**  24:41  
It should go through. And I remember we talked about it a while ago as well. It's still the same. It shouldn't be there. And in general, I'm in favor of removing a lot of the stuff that was kind of put in to assuage people into trying to do something that doesn't make sense anymore.

**Hudson Jameson**  25:05  
That sounds good. Okay.

**Micah Zoltu**  25:07  
Oh, I'll update that issue and close it.

**Hudson Jameson**  25:10  
Okay, sounds good. Oh man, item number four is missing. Everything is broken. The world's over.

## 5. [Single source of truth for EIP](https://youtu.be/B8uSDIYznuY?t=1523)

Never mind, we're gonna go to number five. single source of truth for EIP. What was this one about?

**Micah Zoltu**  25:31  
(laughing) Can't handle this chaos.

**Pooja Ranjan**  25:32  
Sorry about that.

**Hudson Jameson**  25:34  
That's okay. I'm just playing.

**Pooja Ranjan**  25:38  
Okay, so a few meetings back, we discussed that there are too many sources for EIPs. Like we have EIP readme, GitHub, and then eips.ethereum.org and then medium.org/EIP. So Brent volunteered to get this information at one place. I think he left some messages on Discord. He was proposing to have a Google Doc to list all of the following sources of EIP truth where we find duplicate parallelism. I'm not sure he is in the meeting today to explain that further.

**Brent Allsop**  26:24  
I'm here.

**Pooja Ranjan**  26:27  
Thanks for joining, Brent.

Sorry I'm late. So are we talking about the single source of truth for EIPs?

**Hudson Jameson**  26:46  
Yes. That's it.

**Brent Allsop**  26:47  
Okay, cool. Yeah. I posted on the Peep an EIP the proposal to create a Google Doc to to coordinate and list all of the single sources of all the nonce, all the sources of truth that have lots of duplicates, and then some proposed solutions and list of issues and build consensus, make sure there's consensus around the fixes. And then once we have that set out, then we can push forward to making that happen. But anyway, if everyone's on board with that, then I'll go ahead and push forward with that and get involved listing all the issues and proposing solutions and stuff like that. So if anyone has any other additional sources of truth or any other ideas, yeah. So that's the plan.

**Hudson Jameson**  27:32  
That sounds good to me.

**Brent Allsop**  27:35  
Okay, yeah, I'll be creating that document and start listing the issues and proposing solutions. And we'll see if we can pull everyone involved on board. One question I did have - is it Jason, the guy that works with the foundation that's responsible for that site, what's his name?  

**Hudson Jameson**  27:58  
Is it Sam?

**Brent Allsop**  27:59  
Sam. Sam Richards. Can someone contact me his Skype ID or something like that? Because I'd like to make sure he's on board with that and I think he's one of the key figures.

**Hudson Jameson**  28:20  
Yeah, sure. I have his Telegram. Let me give you his Telegram.

**Pooja Ranjan**  28:25  
Sam also joined our Cat Herders Discord so possibly can get his contact there .

**James Hancock**  28:31  
He's pretty active on Discord.

**Hudson Jameson**  28:33  
Yeah, let's just do Discord, actually. I won't even send the Telegram because he's more active on Discord, I think.

**Brent Allsop**  28:38  
Yeah, yeah. Discord should work.

**Hudson Jameson**  28:42  
Perfect. All right. Anything else on that?

**Brent Allsop**  28:44  
Nope. That's all. Thanks so much.

**Hudson Jameson**  28:48  
## 6. [EIP status blog & EIP editor roles, responsibilities blog](https://youtu.be/B8uSDIYznuY?t=1727)

Alright, EIP status blog and EIP editor roles and responsibilities blog. Sorry, I wasn't here last time. So I'm out of the loop on this item.

**Pooja Ranjan**  28:58  
So this is coming from a few meetings back when we were discussing about the EIP onboarding. I guess Edson supposed to submit a blog on what are the roles and responsibilities that were agreed upon here. And the other blog was the EIP status blog. So I haven't heard about the first part, but EIP editors roles and responsibilities, but Edson submitted the second blog that is for EIP status. The question that we were trying to get answered to last time was is Cat Herder Medium the best place to publish that blog, or should it go to somewhere else? And he was supposed to reach out to James because James was not there in the earlier meeting, but today, I'm not sure, Edson is not here. So yeah, that was the question. Should we publish it on Cat Herders Medium blog or somewhere else?

**Hudson Jameson**  30:07  
My perspective is we should do Cat Herders blog, because we've been doing all the EIPIP stuff. So we're kind of associated with it in that way. And I don't know of a better blog for that.

**James Hancock**  30:18  
Yeah, I agree with that. It may make sense to some day, take that  and distill it into some place on like the EIP repo or something, too.

**Pooja Ranjan**  30:31  
write, I just have shared the [blog in chat and the link that is submitted to the Cat Herders Medium.](https://medium.com/p/928c628b306e/edit) It is not published here. It was just a thought suggested by lightclient that because this is might be higher visibility or something. So we should first check out with James, because he's the hard fork network coordinator right now. So yeah, if we are fine, then we can go ahead and publish it in Cat Herders blog. And if people have any thoughts and suggestions on any correction  that is needed to know, leave a comment.

**James Hancock**  31:06  
And we can we can get more visibility on it, like through a tweet or something like that, too, right? Make sure to bring stuff like that up, and we can see if there are other ways to get better visibility.

**Hudson Jameson**  31:22  
Okay, great.

## 7. [Review action items from the previous meeting.](https://youtu.be/B8uSDIYznuY?t=1886)

Number seven is review action items from the previous meeting. Oh, did we have anything else on the blog stuff? I guess we should wait for Edson to make a final decision.

**Pooja Ranjan**  31:34  
Yeah, I'm fine with that. Yep.

**Hudson Jameson**  31:38  
Okay. So the decision items, we're going over action items. Yeah, action items. The only one is Edson will contact James to decide where to publish the EIP status blog. So that's just one we're waiting on. So that'll be rolled over to the next meeting. Okay, was there any other stuff for the EIPIP meetings? Also, what's two weeks from now? Is that a holiday? No, it's not technically a holiday. Is there anyone who won't be here for that?

**Micah Zoltu**  32:19  
You get holidays?

**Pooja Ranjan**  32:22  
It's 30th of December.

**Hudson Jameson**  32:25  
It's the end December, so everyone's off randomly. But I guess people are traveling less depending on where in the world you are.

**Pooja Ranjan**  32:36  
I mean, I'm fine to make it next if it happens on December 30.

**Hudson Jameson**  32:45  
Yeah, I can make it.

**Micah Zoltu**  32:49  
I don't have a personal life. So I can do that.

**James Hancock**  32:54  
Echoes sentiments.

**Hudson Jameson**  32:56  
Okay. Three or four is a quorum for these kinds of meetings. So we'll go ahead and have that in two weeks on December 30 at 1500 UTC. Anything else from anybody before we close the meeting?

**Brent Allsop**  33:18  
Did someone have the Sam Richards contact? I'm not seeing that yet. Did I miss that?

**Hudson Jameson**  33:22  
It's on Discord in the Cat Herders Discord

**Pooja Ranjan**  33:31  
I messaged you.

**Brent Allsop**  33:32  
Cool, thanks.

**Hudson Jameson**  33:34  
Okay, if there's nothing else -  what was that, **Micah Zoltu**?

**Micah Zoltu**  33:38  
Hey, congratulations to us. We're down to 28 open pull request in the EIPs repo. Down from like 500. Down to two pages. Very manageable.

**Hudson Jameson**  33:50  
That is awesome. Great job. Especially to you, **Micah Zoltu**, you kind of did the bulk of that. I feel like if not lightclient, too.

**Micah Zoltu**  33:58  
All credit goes to the bot.

**Hudson Jameson**  34:01  
The bot did it. All right. Well, good. Good job, bot.

**Micah Zoltu**  34:05  
The robot did all the hard work here.

**Pooja Ranjan**  34:09  
Okay, this bot, I just got one question. In my mind. I know I'm in it's not a new question for people. The bot has already closed my earlier hard fork or retrospective that we did as Informational. So I think it would be a good time to move it to Eth 1.0 spec repository now.

**James Hancock**  34:31  
Yeah, I agree.

**Pooja Ranjan**  34:34  
I'll do that.

**James Hancock**  34:37  
You can make a folder for them. Yeah.

**Hudson Jameson**  34:43  
All right. Sounds great. All right. Thanks, everybody. See all in two weeks. Bye. Have a good day.

**Brent Allsop**  34:49  
Yep. Thank you.

**Pooja Ranjan**  34:49  
Thank you, everyone. Bye.

Transcribed by https://otter.ai


# Attendees

* Brent Allsop
* Jim Bennett
* Chandrawinata
* Hudson Jameson (Host)
* James Hancock
* Lenova K6 POWER
* Micah Zoltu Zoltu
* Pooja Ranjan



# Date for Next Meeting: December 30 at 1500 UTC
