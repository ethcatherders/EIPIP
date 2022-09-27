# EIPIP Meeting 63 Notes
## Meeting Date/Time: Wednesday, Wednesday, August 24, 2022, at 14:00 UTC
## Meeting Duration: 1 hour
## [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/170)
## [Audio/Video of the meeting](https://youtu.be/z1nd3R5TaRs)
## Moderator: Pooja Ranjan
## Notes: Alen (Santhosh)

## Decisions Made / Action items
| Decision Item | Description | Video ref |
| ------------- | ----------- | --------- |
|63.1 |  On How "final" is FINAL for the EIPs -- We don't think we want to be fixing the formatting for finally EIPs, unless we're intentionally fixing the formatting for finally EIPs, which is a whole other issue. However, I believe that the author will remain active for in-process or draft EIPs. So, if someone submits a pull request to fix a typo in a non-final EIP, the author will presumably see it. And we'll almost certainly incorporate it into their work. But, yeah, I just think it's better to keep everything as strict as possible, especially while they're developing, so they don't get surprised by something as simple as a status change or when I go to final. | [48:41](https://youtu.be/z1nd3R5TaRs?t=2922)|

## Intro [0.10](https://youtu.be/z1nd3R5TaRs?t=14)
**Pooja Rajan**
* Welcome to EIPIP meetings, 63, we have quite a few items on agenda for today. I see we are joined by Colfax. I am assuming that he is here for one particular topic that is GitPOAP. so maybe we can bump that up and start from there before we get into our usual discussion. Is that okay? 

## GitPOAP Intro 

**Colfax Selby**
* That works for me. Yep. That's the topic I'm here to discuss. 

**Pooja Rajan**
* All right. so yeah, Colfax, maybe you can share about GitPOAP that you wanted to discuss, and then we will get back to item number one or whatever items are listed here for today's discussion. 

**Colfax Selby**
* Absolutely. It sounds great. thank you all for having me here today. my name is Colfax and I am working on a project called GitPOAP and essentially what is, is what we're doing is we're working on issuing perhaps that represents contributions central to the Ethereum ecosystem.So here I'll just share my screen quickly. we've been working our way through the central projects to the Ethereum ecosystem and awarding POAP for software contributions, as well as other types of contributions. 
* We've onboarded about 600, repos here, including like a Ethereum.org on many D5 projects, core tooling projects. and the goal here really is to offer recognition for the work that's happening and, through the issuance of POAP. So you can see here, this is the 2022 Ethereum.org, contributor POAP app. there's 83 people that hold it and so what GitPOAP is doing is we've, integrated prohibitions into github. And specifically, most of the projects that we have onboarded are software projects where they work on the flow of like submitting code through PR and then that PR getting merged. 


* And I opened up an issue,for EIPIP to award GitPOAP to EIP editors and contributors. And through this conversation,it became clear to me that sort of the way that EIPs are developed is a little bit different from just writing software. And so what I want to discuss with you guys today is, one we're excited to award, GitPOAP to everybody who's contributed to EIPs or any sort of way.And we would do that sort of by issuing an annual contributor GitPOAP to the EIPS repo. And we've, we're working on onboarding actually a few of these other repos that were suggested. 
* And so today what I wanted to do is talk to you about the tool that we've built that I think will be useful for awarding GitPOAP to EIP editors, given that it doesn't work normally on just like a pull request model where the issue or where the pull request submitter is the most valuable contributor. before I get into sort of the spec of the tool, I wanted to show you guys, this is our working, designed for the EIP GitPOAP.I'm happy to take any feedback offline, but I just wanted to share this with you guys. 


* I can share this, in the, in the zoom chat as well, if anybody would like to take a look.I don't know if anybody has any feedback or any thoughts to share about this right now, if you'd like, and I know it says 2023, we're going to update the dates.That would be annual. Awesome.Thanks.I think it's particularly cool to see sort of like the imagery around the Ethereum and logo and the different components and so we're,there's a couple other repos that are related to EIP editing that we're working on,different GitPOAP, where for example,like EIP w and we're sort of taking sort of components of this sort of Ethereum upgrading process and we're diving into it. So here's just like a little behind the scenes, sort of aspects of like how we're coming up with our designs.and so I'll share with you next, the tool that we're building to hopefully allow the EIP, maintainers to award your GitPOAP EIP editors.Thank you, your Panda PIP for some early feedback. basically what we're planning on doing is building a bot,and we already have some components of this already built and basically would be GitPOAP-bot and you'd be able to tag it on a given issue or pull requests.And so here's like an example of one here. So if you go to an issue, basically what you'd be able to do is say this was a particularly important issue.


* What you could do here is tag in a comment like at. And if you tag GitPOAP-bot, it would award a GitPOAP to the submitter, or you can also like tag it in sentence. If we were a part of another comment, or you could specify like a list of usernames,if you wanted to award it to a specific set of folks, or if you wanted to award the GitPOAP to everybody involved,we can do at everyone.And it would actually go ahead and award the GitPOAP to everybody. And so that's sort of our initial idea for awarding GitPOAP based on not just like merge pull requests.so yeah,I don't know if I was talking to Panda PIP before, in terms of awarding for historical contributions, we can help sort of automate the process and identifying and actually executing the bot for like past ones, but on an ongoing basis, we're hoping to sort of build a tool that can integrate into your existing workflows of reviews and you can award them on the fly for, for meaningful contributions. 

**Pandapip1 (Gavin John)**
* I think Victor has some things to say.Yeah, hi, Colfax, thanks for coming. 

**Victor Zhou(@xinbenlv)**
* Yeah, hi, Colfax, thanks for coming.This is awesome. I really, hear me Kind of, okay. 

**Sam Wilson**
* Just Keep the webcam came off. I think he usually works better. 

**Victor Zhou(@xinbenlv)**
* So is it better that 

**Colfax Selby**
* That's better? Yep. 

**Victor Zhou(@xinbenlv)**
* Okay. Yeah. Love the ideas.That's the question I have is, one is that, how do we avoid, rewarding, spammers? Because we recently seen that some people are issuing spam posting and the other one is how do we, whether we have considered having different milestones that contribute to, for example, like their first EIP or their first silo or things like that. 
* So as opposed to annual contribution or in addition to our annual contribution. So that would be true by feedback, by the way. Thank you for coming.I think this is the perfect venue to discuss this because you have penned up pave and Sam majorly on the automation side.. 

**Colfax Selby**
* Awesome, yeah, two good questions also.Yeah.Thank you for having me here.I think it's a great forum to be a part of. so on the first one, in terms of fighting spam, this is something that's very much on our minds and the initial, like the, the architecture of GitPOAP for code contributions, specifically only awards POAP for merged or requests, which inherently have manual review in them. So like any spammer that tries to from one, they're not going to get it because the code is not visually going to be merged with what's actually meaningful. 
* And it was something that we were definitely like our heightened awareness. we had had no worries about around our launch, which happened back in April and so far, nobody's reported back like an increase in spam, pull requests being sent as a result of GitPOAP perhaps, and track somebody actually was tweeting yesterday saying that it's, too hard to earn GitPOAP apps for spam contribution.There's a lot of, it's kind of funny. so in terms of like fighting spam,I would say that really lies in.So it's going to be only a manual process to award GitPOAP.

**Pandapip1 (Gavin John)**
* But I can make it, but I have the EIP bot tagged the GitPOAP. Right? 

**Colfax Selby**
* You could. And so the other detail here is that they GitPOAP will only trigger if it's tagged by a maintainer. 

**Pandapip1 (Gavin John)**
* Well, the EIP bot actually has handle on the EIP is repo. 

**Colfax Selby**
* I said, I guess we would have to talk about how possibly, like, if the EIP bot, if we want the EIP bot to be able to tag the GitPOAP, we can work out those implementation details. But the idea, at least the way that I'm envisioning it is one of the maintainers. So like either you had to pay for maybe Sam,if a particular issue or pull request for a new EIPIP  is valuable. You guys would go ahead and then manually tag the GitPOAP.

**Sam Wilson**
* So, I I'm concerned about adding extra work for EIP editors. So I'd like to see this be like, as automated as possible. So when an EIP gets moved to final, then a person would become eligible. Is that kind of the process we're thinking here? 

**Pandapip1 (Gavin John)**
* Or when EIP gets merged as final, then tags the GitPOAP bot, to then assing gitpoap, And it would be a central authors of the EIP, or Would it be assigned to all of the authors of the EIP? 

**Sam Wilson**
* Okay. So yeah, as long as we can automate it and it happens for like the trend, like after the transition to finalist merged, I think that works. 

**Pandapip1 (Gavin John)**
* And I think that it's pretty, and I think that it should not be too difficult to do that. And since the EIP, I don't think that it requires any configuration with gitpoap app itself just because the EIP bot itself has admin. So if the, if the GitPOAP does it by pinging the hubs,the guide to see what permissions the, a sender has, well,EIP bot has the permissions. 

**Colfax Selby**
* Awesome. That makes total sense. we can definitely do that. One of our core principles too, is we don't want to add any additional work for maintainers. So I think configuring it with the EIP bot that would automatically trigger upon the mark finals and great solution. 

**Pooja Rajan**
* I do see a couple of things that might need to be addressed here, maybe on the bot side, but I mentioned that Pandapip of people that would be like, if any EIP is finalized, then the bot will tag the person or the set of authors who have contributed to that. But if you are making any changes, post it is finalized or, minor changes edits here and there.In that case, we may have to customize that to, you know, 

**Pandapip1 (Gavin John)**
* It would only be when the EIP has moved from any non final status to final, and then it assigns that to everyone that's has a github handle in the author field. That would be the conditions on which. 

**Pooja Rajan**
* On a high level.And that sounds good to me too. 

**Colfax Selby**
* That sounds good to me too. and the GitPOAP bot as designed can support that, and we just need to figure out how the EIP bot then trigger from the GitPOAP bot , but I could just have it, 

**Pandapip1 (Gavin John)**
* Used to get her API descended comment.It's not that difficult. 

**Colfax Selby**
* Of course. and then let's see to address Victor's second question. So the first question was about spam, and then the second question was about, sort of like repeat contributors or sort of like scaling it up the way that we're handling that right now, for code contributions is we're issuing annual contributor GitPOAP. And so you can actually see if somebody's track record,if they've earned the annual contributor, GitPOAP over the course of a number of years, like 2019, 2020 and 2021. 
* We're also, we haven't released this yet, but we're also working on visualization of depth of contribution within a year. So for example, if I've been an author now of like three different EIP's in 2022, granted I'll only have the one GitPOAP, but we have the, we can, when we basically have the metadata stored on like how you earned it and we're working on different visualization metrics to actually signify that.so that's one aspect of it.And then secondly, specifically for EIP is I think it could be interesting. So I think it's a good start to work on just, issuing this annual contributor, GitPOAP for EIP editors, but going forward, if you guys are interested for particularly impactful EIP,is if there were some specific ones, we can actually create a customized GitPOAP with its own design and award that just to the folks who contributed to a particular EIP. So for example, it could be like the EIP 1559 GitPOAP. so I'm just throwing that out there as an idea of there a particular EIP is that you want to award separately from just like general EIP editing. We can do that too, Kind of all neutrality. 

**Sam Wilson**
* I don't think that will be happening If it's wanting to determine EIP is that you'd like to re award extra GitPOAP to feel free, but we as editors probably won't be doing that, 

**Colfax Selby**
* That makes total sense.I'll discuss with my team and sort of maybe we can discuss with the community or something, but yeah, I'm just throwing it out as an option, but I appreciate that. cool. Well, as some next steps, all sort of draw up, the feedback that you guys have given, Pandapip, I'll continue to coordinate with you on our development of the GitPOAP bot and how you can tag that with the EIP bot. and we'll go forward from there. I just want to say, thank you guys so much for having me here today. 

**Pooja Rajan**
* Thank you. Thanks for joining Colfax and sharing this. I'm sure this is helpful and it would encourage more people to be able to contribute to EIP in a repo and make valuable contributions and people can always leave comment and feedback. I have shared the issue that is on EIP issue number is 134. Thank you. Moving on, let's start from item number one,

## Proposals to include in 'Preamble' [15.18](https://youtu.be/z1nd3R5TaRs?t=918)

**Pooja Rajan**
* Which is proposals to include in preamble. we have collected quite a few proposals, which are there to suggest some edits or updates for preamble, in EIPs. the first one listed here is, are finalized date to EIPs. I see there are already ongoing conversation. Yeah. Anyone has any comment and thoughts to add for this issue? 

**Pandapip1 (Gavin John)**
* You're actually missing, what is the PR, adds an item to the preamble. 

**Pooja Rajan**
* I'm sorry. It has been merged, I know, there was one created by Victor, I guess 

**Pandapip1 (Gavin John)**
* The one I just put in the chat.

**Pooja Rajan**
* Oh, sorry. 

**Pandapip1 (Gavin John)**
* The adoptable, that  one since no one has Anyone have any objections to the adoptable.  That's a good idea. 

**Pooja Rajan**
* Sam if you are talking, Sam, if you're talking you're muted. 

**Sam Wilson**
* No, no. I'm okay with adoptable, I guess. yeah, I can, I can approve it. 

**Victor Zhou(@xinbenlv)**
* I don't have the any. I mean, favor up this. 

## Proposal to include Superseded status and superseded-by: (eip number) preemble section ethereum/EIPs#5265 [17.29](https://youtu.be/z1nd3R5TaRs?t=1049)

**Pooja Rajan**
* Okay. So we could move on to number two. I mean, a sub-item for this one, proposal have to include superseded. I think it is a number 5265 I guess it was added by, oh, sorry, please go ahead. 

**Pandapip1 (Gavin John)**
* Oh, just for the superseded. I'd prefer if it wasn't a status and I would prefer if it was, if, if it was an item in the preamble to say supersedes something, and then it made clear that, Hey, this is not unofficial thing. We're just suggesting that you use this instead of this other thing. 

**Sam Wilson**
* Yeah. I think putting something in the preamble for supersedes probably gives the impression that we like we as editors have allowed us to supersede something else.And I'm not sure I'm okay with that implication, 

**Pandapip1 (Gavin John)**
* But there would be a badge like the one for drafts or things in view. And that sort of badge that basically says, Hey, this is the recommendation of the authors and there's not, and may not reflect best practices. 

**Sam Wilson**
* I'd rather just not include it at all. I think if, if somebody wants to withdraw, any EIP and putting the withdrawal reasons superseded by EIP ex they're perfectly allowed to do that, but I don't think we need a special field for superseded. 

**Pooja Rajan**
* I think that we have precedence of, doing that, like with withdrawal.We generally mentioned that, which is, I mean, if there is the reason that any other EIP is better than the proposed one, we do mention it and reason, 

**Victor Zhou(@xinbenlv)**
* I'm the one that proposed this because it was inspired by IEF RFC and there's the RFC field for a supersead so that the whole community can continue to evolve and notify the future reader that something that's being updated. So as much as I respect and understand the concern of Sam said, I, I think we can, I love to kind of, not try to, propose, approve or not move with those PR in on today's meeting, but to further discuss under what consent condition and, who are able to add such thing. And whether we Preamble field is the best format, or is there other way we can do that signal? I can, I can take that offline and, and, and follow up in the future. 

**Pandapip1 (Gavin John)**
* I think that, yeah, EIP 820 does a good job with us. So I'm just going to quickly send a link to a file in the chat. So what it does is before any of the sections that has like a big thing that says PRC 1820 has superseded EOC 818. So basically, and say, Hey, this, this is the authors here saying that due to some, due to a change in solidity, actually you have to use this other thing instead of and this is currently compatible with what we have. 

**Pooja Rajan**
* We can definitely keep the issue open, for another few weeks, people can add comments and thoughts, and, yeah. is that a good resolution, Victor? 

**Victor Zhou(@xinbenlv)**
* I heard the concern that I would document the concerns and I intend to continue to pursue a proper way to indicate that. So thank you for keeping it Sounds good. 

## Proposal for EIP preamble: include separate relates-to: as an optional field ethereum/EIPs#5274 [21.11](https://youtu.be/z1nd3R5TaRs?t=1271)

**Pooja Rajan**
* Awesome. Moving on. the next one is proposal relates-to preamble key ethereum/EIPs#5274, I guess this was also proposed by Victor. 

**Victor Zhou(@xinbenlv)**
* Yes. I think that different people interpret that requires differently. Some people me included see that requires and thought that it means a, to implement some EIP. It requires some previous pre-existing EIP's to be implemented, to be final and to be, to be final for sure, but to be implemented as well. And that's, that seems not aligned with Pandapip and with Michal. And so I think that requires this a little bit confusing.So I like to see if there's a clarification or do we need to add new fields? Yeah, go ahead. 

**Pandapip1 (Gavin John)**
* So I just had an idea, maybe we don't need a separate requires to feel, but, relates to field, but I wonder if we could just, I mean, I can, I'd be okay if, if an EIP one, we changed it so that it's only EIPS that are referenced in the spec that needed to be included, requires fields. I'd be okay with that change. 

**Victor Zhou(@xinbenlv)**
* So may I ask, under what circumstances do we feel that, we want to have a special call out of EIP being referenced other than the body already have a requirement to link to the, if they mentioned that. 

**Sam Wilson**
* Yeah. That's my thoughts as well. Like why do we need a preamble field if we already require them to be linked? 

**Pandapip1 (Gavin John)**
* Well, I can see Eddie  are useful having at the very top thing. Hey, we, these first.

**Sam Wilson**
* But that's required. Right? You have to read these to understand the EIP. 

**Pandapip1 (Gavin John)**
* Yeah. So I would be okay if any we changed it to be anything that's, anything that's includes in the spec has been requires. 

**Victor Zhou(@xinbenlv)**
* I'm not sure. Sometimes the boundary can be the introduction of create two is a prerequisite in some of our scenes, but that you don't necessarily need that create or read, recreate it to be a reader. You might need it to, to be able to author it. And if someone has handled that for you on the dependence, your SDK,you don't have to understand create too. So what I feel is that if we make a hard requirement or make it clear of what inquired means, for example,if we say that without the required,You didn't catch that you, you kind of like he might die. 

**Pooja Rajan**
* All right. It looks like there is some audio issue, microphone issue with the Victor. So we can move on. 

**Pandapip1 (Gavin John)**
* I guess the last one advanced digit EIP, since, Mike is not here. well, I mean, is there any reason not to have this? 

**Sam Wilson**
* Sorry, I didn't catch the beginning of that. This is the finalized date. Yeah. Okay. So I think this would be reasonable to add.yeah

**Pooja Rajan**
* I think we had a discussion about this in the past, and there was some agreement, disagreement they issue was dropped then. but it's good that we have it back in the form of issue and yes, if we have consensus that I believe we just need a pull request. Okay. You have shared the pull request that needs to be merged. 

**Pandapip1 (Gavin John)**
* Yeah. Sound congested. 

## 2. From GitHub Issue or Pull Request [26.00](https://youtu.be/z1nd3R5TaRs?t=1556)

**Pooja Rajan**
* An Sounds good. Cool. Anything more on preamble topic? Alright. we can move on to number two that is from Github issues and pull requests. The first one that we have considered here from issues is, merge policy discussion. How final is final. The issue is already added in the EIPIP Github repository. So we have seen in the past that there are some improvements, suggestions, minor edits are going into final. EIPs is in this month only we have seen three final EIPs is being edited with small changes. So yeah, this is about discussing. How do we decide final is final?


**Pandapip1 (Gavin John)**
* I'd say backwards compatible. I basically, if it's able, if the EIP is able to be implemented and there's no ambiguity in how it can be implemented, then that's how it has to be.If either of those conditions don't fail, then it is okay to get rid of any ambiguity or to make it so that the EIP can be implemented at all. 

**Sam Wilson**
* But I think we need to, I don't think we can actually write in backwards compatible or backwards incompatible into EIP one, just because I'm like, let's say, the EIP specify a core EIP specifically, specified something and all the clients implemented a different, but the same different way. then when the EIP goes to fi like after the EIP is moved to final, you would have to change the EIP to match clients actually implemented, Only four ERCs. I really just think that we should make it a policy to only allow backwards compatible changes to final EIP,but I don't think we should make it a hard rule because there are times where I'm like,if something is wrong with the EIP,like clearly it is not what the author intended.It's,it's just wrong.Then I think it's fine to fix the EIP.Even if it's backwards, incompatible,I think backwards incapacity or backwards compatibility is a good baseline, but there should be, we should be allowed to make exceptions to that. 

**Pooja Rajan**
* I guess. the, important question here would be to maybe outline it for people to refer to, like, what is the point where, Oh, go ahead. 

**Victor Zhou(@xinbenlv)**
* Go ahead and go-ahead Pooja, sorry about That. 

**Pooja Rajan**
* no, not a problem. So what is the point where we can say that, beyond this, we are not going to make any edits basically to clarify on what kind of edits may or may not be able to get in. If there are any edits which is outside the guideline then we can ask the author to come with the new proposal not edit the existing one, not edit the final proposal 

**Victor Zhou(@xinbenlv)**
* Then you need to add changes to the core EIP to reflect what everyone is implementing.I think given the idea of EIP being if union improvement proposal, if everyone is implemented in a same consensus different way, then the better way is to keep the old one as final and create a new one that reflects the true implementation rather than fixing the old one. Unless they're not final, right? If, if the final has been reached, I think changing things make it essentially be alive. So unless we want to agree that final is still alive, I am. I'm very weekly lean towards making final changeable, other than editorial requirements. I don't consider backward implement backward compatible feature improvements as quantified in this case as well. And that's also why I propose to have a super seed so that if the also do think that this EIP has been final, but no one is implementing it, it's not being adopted. And everyone has a new idea, then it should, they should have a way to signal what is the better way. So that's, that's, that's my, my standpoint. And with respect to 721, I think if the author goes to make a final and realize let's sorry, 712 right? So we went to the type six assigned signature. So 7 1 2 on the ERC side is the same. I think if everyone has been implemented in a different way, it's an all, it's a wrong way. The best way is probably just to start a new one, copy the old one, fix it. And then, and then publish that one as, as new final or revert on in a one-time exception. We've already it back to draft towards to anything that is not final. Then I think we can, we can, we can modify otherwise we have to be undermining our credibility of being final. I, I don't think as a EIP editor, a group, that's the best in the best reputation, best way to hold the reputation of this group. 

**Sam Wilson**
* So we, we can't, I think unless we like completely revamp our process, ever move in EIP of final. I, unless I guess it's also the withdrawn. Maybe we could allow that, but, because of the way the, merge bots are set up once an EIP moves out of like, if any EIP is not final, the editors can change it without a EIP editor approval.So you would, you would basically just lose all immutability immutability guarantees if It would be like, even worse than making a one-time change to final.Yeah.

**Pandapip1 (Gavin John)**
* Yeah. Like it's like saying it's final and now it's like me handing you a gift. And when you open it, suddenly say dropping up the gifts, taking it back and putting a new thing in there and giving it back to you. 

**Sam Wilson**
* So, So I am very strongly against ever moving an EIP out of final. 

**Victor Zhou(@xinbenlv)**
* Okay. Compared to, compared to having a one-time change. 

**Pandapip1 (Gavin John)**
* Yeah. Yeah. Because as long as it's in final, the editors can review every minute change to the a. But if it's taken out a final, then it's carb launched that can do whatever they want. Do it. 

**Pooja Rajan**
* Yeah. I would agree. Agree to Sam like, changing the direction of a process flow. I think we had a long discussion on it about a year ago. This is one way,like when it is moving from last call to final, it is uni-directional, however, from last call to review, it can be done. 

**Victor Zhou(@xinbenlv)**
* So, let me put the 712 as into contexts. I'm not sure if any, one of you have attempted to implement 712. I did at, Sorry. 

**Pandapip1 (Gavin John)**
* I says it's not possible then implemented, there are no implementation. 

**Victor Zhou(@xinbenlv)**
* Then we put it into context. I did. And then for what I know, it's the, the, the EIP is largely is largely, ambiguous and not even ready. I, so I think it's not even ready for one-time change to make it final. That's why I'm suggesting it has to go to some status that is updatable that either start a new one or, or move it back to drop, because I think it will take another several months, several iterations to get to a state that, implementations are agreeing on each other. It's currently, we're seeing different interim. I personally see different implementations of what ethers have been doing and what the mathematics is doing. And so I think that the consensus has not been reached that they're just one convinced to go in. I'm not copied on that is that, that is doable, achievable at the current snapshot of 712. It can take quite long. 

**Pandapip1 (Gavin John)**
* There are two, there are two specification sections, one of which was just straight up copy and pasted from, I think it's EIP 111. and I'm pretty sure all of that needs to be done. Just remove that accidentally copied and paste that specification section and time it's done currently as is it's incompatible with itself. There cannot and will not be any specifications of 7 1 2 in this form, just because it just because it has two mas that say two different things.So as written,it is not possible to implement it. And so therefore it is also not possible. Therefore there are no implementations and therefore there's nothing that can be broken. 

**Victor Zhou(@xinbenlv)**
* And, we're in consensus that at this current snapshot, it doesn't work. No one can implement it that I think we're in consensus.I wonder if I make myself clear that even with one change, it is still not capable of being in the final state, like it's in a stable state.I wonder if I made myself clear that I,I think in my personal experience ignoring one of the specifications, the other specification is not ready to be implemented. 

**Pandapip1 (Gavin John)**
* I think we would need to get the authors on that call.I mean, I guess I'm slightly weekly in favor of moving it back to last call, perhaps just because that last call also requires, editors, different revolve changes.so there's that? 

**Victor Zhou(@xinbenlv)**
* What is your preference on like, have, keep it final out, but let the author start a new one or let someone could start a competing one. 

**Sam Wilson**
* So if there are large problems with 712, like to the point where it is ambiguous and you'd like, you can't implement it well, then I think somebody needs to take EIP 712, and just rewrite it under a new number. That that would probably be the best approach. 

**Victor Zhou(@xinbenlv)**
* Yeah.That would be my, yeah, that would be my standpoint. And we can wait for 712 to see if they want to do so. Or if someone else come in and compete that that would like fully compatible with the current process. and doesn't break any, immutability assumption. Okay. 

**Pooja Rajan**
* I guess I could provide some information about 712. We had tried  to reach out to authors. We did try a lot, obviously be contacted some of them, however, they did not show up for pushing in the proposal and final status.So it was championed by one of the cat herders who do so I believe in this case, we can consider that the authors are Mia and having a new proposal of competing proposal will be good. And the, when it is proven that the new proposal is fixing all the ambiguity of the 7 1 2, probably we can take an attempt to make it, stagnant, sort of a withdraw and have shared the new proposal with the rest of the dap developers  that for adoption? 

**Victor Zhou(@xinbenlv)**
* I agree with every part you said, except for the withdrawn decision has to be made by the author or original author. If the already know author, didn't care enough to read through it, then we pretty much stuck because if we, if we open up a precedent that editors, can we store on behalf of the original author, then I think it can open up another Pandora box. 

**Sam Wilson**
* Yeah, I agree. I don't think editors should be withdrawing with the author. 

**Pooja Rajan**
* No,I didn't mean that editor should be doing that.I guess it was being championed by one of the cat-herders.So probably we will reach out to that individual and see if this can be solved, but that is going to be a later issue for us. We should look into getting up with a new proposal. So app developers who are looking into implementing of this has some solution.They do not stop because this is not implementable. Alright. I think in the essence of time we can provide new wrap up this topic. And if anyone has any other comment or suggestion, the issue number is 171. Yeah. On EIPIP GitHub repository, moving on. 

## EIPW policy: Change EIPW to only check modified lines ethereum/EIPs#5469 [41.00](https://youtu.be/z1nd3R5TaRs?t=2460)

**Pooja Rajan**
* The next one is EIP w policy, I guess, that it's an ongoing conversation and we are waiting on some consensus. Anyone would like to summarize. I think it was again by Victor. 

**Victor Zhou(@xinbenlv)**
* Sorry, can you point me to the, to, to the matter I'm just open up my computer and, Oh, this is only, only checking change lines. I think Which, which, I'm lost 5469. Yeah. Yeah. so is there any, I think the, the Sam, Pandapip penned up probably be most authoritative answer, whether it's technical feasible or not. I personally feel that, based on other linking tools it's possible to do so, but like, depending on how much it is, also like Sam and pandapip, do you have preference of notch checking only the change line? Okay. 

**Pandapip1 (Gavin John)**
* I would say probably I'd be okay with EIP w only, only blocking, only blocking verges when the IP status changes. So that is something I would be okay with now. I much I'd be I am much less happy with it. Only changing, venting changed lines, because then you could have it going from like draft to review the entire, the entire, there are a bunch of new things that need changing and that aren't being changed it's only, requiring EIP w the paths, for status change, PRs, a good compromise, Compromise. 

**Sam Wilson**
* I just don't see the value. Like what's like, what's the point of not providing feedback, like early on in the process to authors. 

**Victor Zhou(@xinbenlv)**
* So Sam, I can give you some examples. I can give you some, go ahead. Sorry. 

**Pandapip1 (Gavin John)**
* Yeah. PDW would still be failing the, it, it wouldn't actually be like, it would still be like giving all the errors and errors and stuff. It just would be that the EIP w would no longer be marked as a required check, but the EIP bot wouldn't merge it unless.

**Sam Wilson**
* No, no, I, I get what you're saying, but no one is going to read it.If it isn't failing, if it doesn't stop them from merging, no, one's going to read it. So like, what is the benefit of being more permissive?I don't see one, but, Well, I am very, I am very much against, linting only changed lines because, like, like I said, my comment, the boy scout rule. So if you edit the file, you should make the file better. and I think that, EDW is probably the best way to do that. and I, I don't think we should only require lens on status changes because then when an author is trying to move something from reviewing to last call, then they're suddenly going to get a bunch of stuff that they have to fix that they weren't forced to fix before. And like, right before going into the last call, that doesn't feel like a great, like a developer experience, I guess. I think we should just have a lint whenever they make a PR, it's not like it's stopping them from making commits. It's just stopping them from merging them. but you know, I don't know, I am not a dictator, so you guys can decide something else if you want. 

**Victor Zhou(@xinbenlv)**
* So can I, can I put something into context and see if that would, change your mind or, like at least make you hesitate? one of the scene we see some contributors,not necessarily author contributors who come across the one EIP realize there's the typo come to fix the typo.I think that's a good spirit, right? And then it's also a good way to get into EIP editorials. And, in that case, the micro contributions, help out a lot. So that's why I am suggesting if we allowed, merging, just checking the line.Like if you touch this line for this scope, maybe it's good idea that you want to fix the whole thing in a line or even per paragraph, but for the whole file, it's scare away people who just want to come in and contribute.I have firsthand experience starting at contributing from Wikipedia.A lot of page,I contribute just fixing typos, and then ultimately I'd become a more regular contributors. So in that spirit, I want you to see if you would reconsider that scenario. And of course it will be approved by author in our current setup,but I think so long as at the time it moves to the next stage.Should I change status? For example, we view or five last call or a final, then someone mostly, they also have to be responsible for what is editorial footie checks.So Sam, does that make a good argument before you It's? 

**Sam Wilson**
* I don't think there's anything wrong with the argument.I just don't agree.I think, I think EIPs Are standards documents.They're not like crowdsourced explanations of things.So I think there's a little bit of a difference from Wikipedia and like, I do appreciate people coming in.And so, so one, I think we should turn off EDW for final EIPs, for sure, because that's just awfully annoying and I don't think we want to be fixing the formatting for finally EIPs, unless we're intentionally fixing the formatting for finally EIPs, but that's a whole other thing. but for, for in process or draft EIPs, I think, generally speaking, the author will still be active. So if somebody puts up a, a pull request, fixing a typo in like a non final EIP, presumably the author will eventually see it. And, we'll probably incorporate it into their work. but yeah, I just think it's better to keep everything as strict as possible, especially while they're developing so that they don't get surprised on like a status change or, or, when I go to final.

**Victor Zhou(@xinbenlv)**
* Fair enough, I didn't convince you, I would come back and try in two year. Yeah, yeah. But I agree that we can keep it as if for now I can close this issue and, or use the pendant.Do you want to pursue the chain the way of bad, it only check when their status change or do we want to, 

**Pandapip1 (Gavin John)**
* You know, I think, I think I'd be okay with it not checking as long as the EIP is final, that I'd be okay with. And I think someone was also okay with that, For sure. So if there's just a random EIP, that's fine. Or that has a typo then I think yeah, that that is probably okay to be merged without having to fully be from reformating. 

**Victor Zhou(@xinbenlv)**
* How about, well, not check for last call. 

**Pandapip1 (Gavin John)**
* Last, last call should be checked just because the changes should be made before it is final. 

**Victor Zhou(@xinbenlv)**
* Oh, I see. Not check at four files at final, right? Yeah. That is consensus for sure. and still keep it on for every other status, every out of the commitment, commits, right. Sorry. 

**Sam Wilson**
* Yeah, exactly. Keep it on for everything Except finally EIPs

**Victor Zhou(@xinbenlv)**
* Keep it on for everything. Every commit, except for final commit. okay. That's a consensus I, as minority disagree with that, but I would document it as the consensus and we can close it. 

**Pooja Rajan**
* Thank you. On the, yeah. So closing the issue and also a Sam & Pandapip for having this as a decision. I hope that they've been noted in the notes for this meeting,

## For a manual merge: EIP-4881: DepositTreeSnapshot Refactor ethereum/EIPs#5443 [51.00](https://youtu.be/z1nd3R5TaRs?t=3008)
* Moving on. the next item for discussion here is a pull request number 5443. It is, there, the last moment is for a manual merge. It is with regards to EIP 4881. Anyone has objection there. Yeah. 

**Sam Wilson**
* The depository snapshot refactor, Right. 

**Victor Zhou(@xinbenlv)**
* Sam, do you have any further concerns? I think they fixed the links per your request. 

**Sam Wilson**
* Yeah, I think it's just good to go. I just wanted to make sure we had an opportunity to talk about it here if Greg were to show up, but I guess it's just the two or three of us, so yeah. 

**Pooja Rajan**
* Last opportunity fund Greg here to miss this one for raising any concern. But anyway, this proposal is in very early stages. I guess I'm the big would have more opportunity to come back on this topic when this is most as review our last one. 

**Victor Zhou(@xinbenlv)**
* I agree so long as they have not been last call. I think it should be safe to merge. 

## EIP-5453: Smart Contract Crypto Endorsement ethereum/EIPs#5453 Endorsement [51.10](https://youtu.be/z1nd3R5TaRs?t=3070)

**Pooja Rajan**
* Cool. The next one here is a pull request number 5453. That is a request, I guess, suggested by Victor. And this is about a new proposal, smart contract crypto endorsement. 

**Victor Zhou(@xinbenlv)**
* Yeah. I wonder if there's any, cause I, my goal is to put it into, let people comment, like have a broader reach, conflict of interest. This is my own proposal, so yeah. whatever you decide. 

**Pandapip1 (Gavin John)**
* Well, currently there is a bunch of comments I put on there that need addressing. So that's currently where the proof of proposals, I see a site notes, Penda. 

**Victor Zhou(@xinbenlv)**
* I saw that you tend to merge lines. Is there any particular reason that you're doing? So, because down actually supports my model and it asks also a help. I will ask you to be pro pro multiline because they allow you to be addressing very precisely what part of the code you want to suggest. 

**Pandapip1 (Gavin John)**
* So the reason why I don't like that is just because tax creditors generally backlines for you. But if you have, for example, but basically I like if it can, if it can all fit on one nine in my tech center, I like, I do quite like it that way.Also a lot of people think that, oh, it'll force a line back there.No, it does not force the line break there and mark down. third, third of all. yes, I do agree that you're being able to target things more specifically is kind of a nice feature, but at the same time, get hub, get smart enough to, do some, yeah. Distill somewhat targeted enough,I guess.I, unless there are two that are exactly the same line, but generally you do all of your changes at one that targets a specific line at one time, as you can see, like oftentimes I have a required at part Y required, part Z recommended, whatever, preferred all. And the last reason I prefer it all on my mind is just because if there is somehow a smaller screen, then what you get is a full line and then a little extra and then a fault line in the middle extra. And that doesn't look good. 

**Victor Zhou(@xinbenlv)**
* Yeah. I heard it. When you say, can I actually make an issue and discuss whether we w we are insuring a style, we would prefer not to enforce such a style because I think the previous consensus I understanding and come out into group is there's no particular markdown style. 

**Pandapip1 (Gavin John)**
* That is Actually the consistency is moving actually towards being a specific cell. there's actually, there's actually an, one of my, PRS is, open right here. Let me figure, add mark down vendor. This one right here. 

**Victor Zhou(@xinbenlv)**
* Oh, okay. let me check. That is still, yeah, we, I think we agreed to have a markdown linter, but I wonder if all the rules and that interest has been agreed upon, especially All of the rules currently have been agreed, that are set currently have been agreed upon. 

**Pandapip1 (Gavin John)**
* I'm not sure if the multi-line one has been agreed upon or not. Speaking of that, some, would you mind, would you mind quickly verging that one? 

**Sam Wilson**
* The markdown linter Yeah.Yeah.I'll take a look at it after the call. I just want to go through all the rules. 

**Pandapip1 (Gavin John)**
* And we enable one rule at a time where like in line that, in fact, Michael went through rule by rule and basically argued why none of the rules should be applied. And we were successfully able to  him from disabling all of them. But yeah, there's only, there's only a few of the rules that are actually applied. And I don't Think my timeline one is one. 

**Victor Zhou(@xinbenlv)**
* I see. Can I propose my, my objection to reinforce a multi-lateral contacted native into one line on record? 

**Pandapip1 (Gavin John)**
* No. What I'm saying is that currently that is not, not an issue. Timothy, according to the conflict we have set in the markdown later, you can do multi-line. I personally need to test it, but I guess, I guess I will no longer force people to, do more, to not do multi-line, even though it hurts my eyes just by looking at it, Me too, when I do my personal journaling, but when I do get commitment, I feel that a lot of tools are assuming the line break.so, that's why I in the EIP, I prefer breaking down then, just because like, get deaf much better with different lines rather than single lines, and also get up as doing that same thing as well. 

**Sam Wilson**
* So that will, Yeah, I think opening an issue to discuss multiline versus single line is probably the right approach here. And, I think Pooja brought up a good point about we're close to time, so we should move on to the next, the next topic 

**Victor Zhou(@xinbenlv)**
* I see. Agreed. 

## EIP Editor #5502 [57.14](https://youtu.be/z1nd3R5TaRs?t=3433)

**Pooja Rajan**
* Thank you. Probably we can continue discussing in that pull request, adding comments there, we are very close to time, but I wanted to quickly bring up one last, item for discussion today. It may not be discussed, but just wanted to share it, but people, the item that has been added by, but it's a last minute addition on the will request number as 5502. It is about adding a new editor, having a new editor added to the repo and getting them access. I know we do not have one, the EIP editors present in this meeting today. So we can probably consider this as an announcement of, this pull request. And we'll try to reach out to more editors. Anyone has any comments, thoughts quickly to add on this? 

**Sam Wilson**
* No objections 

**Pooja Rajan**
* From me Sounds good.I think it is waiting on, reviewers or editors approval. We will try to collect more approvals from datas who are missing here in this meeting today. if we get over three, two or three approval, then probably it can be merged. Now that we have five editors. So 20 some, okay, let me Good. We have quite a lot of pull requests and other agenda items that we could not touch today. I hope that it will be discussed in the issue. Number. People may follow the link added to agenda and lead their common thoughts feedback. They're always welcome to ethereum-cat-herders for the EIP auditor's channel and continue discussing it with creating a separate thread. in the meantime, before we get to the next meeting in two weeks from now, but thank you everyone for joining us today. And I hope to see you in two weeks. Have a good one. Everyone. 

**Sam Wilson**
* Thank you for hosting. 


# Attendees

* Pooja Ranjan (Host)
* Victor Zhou(@xinbenlv)
* Pandapip1 (Gavin John)
* JA
* Sam
* Colfax Selby


# Date for Next Meeting: Wednesday, Sep 07, 2022, at 14:00 UTC



