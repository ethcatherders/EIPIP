# EIPIP Meeting 71 Notes
### Meeting Date/Time: 2022 Dec 14, 2022 , 15:00 UTC
### Meeting Duration: 1:00:56 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/198)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=ylDXaR31gYg)
### Moderator: Pooja Ranjan
### Notes: HenryJK4

## Summary
1. Discuss Issues/PRs, topics
* Propose Policy: Last Call changes shall be separate from the PR to move to Final
* Decision: Big changes in Last Call will restart the "Review ends" date
* Hide Stagnant and Withdrawn EIPs from the EIP list
* General consensus: Not very useful feature to hide

1.5. Changes to Final EIP
* PR-6104: Sam will merge it
* PR-6038: General consensus - PR should not be merged. Sam will create an issue for concern regarding updating Solidity to old EIPs.
* PR-6012: Author needs to list normative changes and non-normative changes. We should avoid adding change to big EIPs like this. Closed.
* PR-5877: Shouldn't change older EIPs for updating table. Anyway, an EIP isn't a best place to maintain a table.
2. Discussion continued from earlier meetings
* A Straw-man Proposal: Continue collecting feedback here
3. EIP Bot
* Group seems to be in favor. Will keep the issue to collect if anyone opposes to the proposal

## Intro
**Pooja Ranjan**
* Good morning everybody and welcome to EIPIP meeting 70 I have shared a gender in chat And we've added a few topics for discussion. The first few sub issues are taken from the EIP GitHub repository. Let's start from there.

## 1. Discuss Issues/PRs, topics[0:13](https://youtu.be/ylDXaR31gYg?t=13)
**Pooja Ranjan**
* Propose Policy: Last Call changes shall be separate from the PR to move to Final ethereum/EIPs#6129 I think this was submitted by Victor but I don't see Victor right now. 

**Sam**
* I think this already is policy maybe we just need to write it down.

**Pooja Ranjan**
* Part of this was suggested by you in the EIP editing hour last week. A person needs to make a new PR to make it final. Is that correct?

**Sam**
* It's not necessarily a secret PR. If you make a large change in the EIP in last call it should restart the last call timer.

**Pooja Ranjan**
* Ok

**Sam**
* You have to let it sit for another two weeks kind of thing.

**Pooja Ranjan**
* OK so we can probably set this as an outcome for this issue and close this issue right?

**Sam**
* Yes 


**Pooja Ranjan**
* Hide Stagnant and Withdrawn EIPs from the EIP list ethereum/EIPs#6027 thoughts from people here.

**Gcolvin**
* It's a bad idea.

**Pooja Ranjan** 
* It's a bad idea. Why do we want to hide stagnant and withdrawals?

**Gcolvin**
* Stagnant especially the author, Google doesn't have anything to do with that.  Just wind up with EIPs that have gone to stagnant. They're in Google they're still historically interesting. Google says here it is go to that page’s,  where is it? Or Google stops indexing it, and it disappears from history.

**Pooja Ranjan** 
* Any other thoughts?

**Sam**
* I don't think it's to hide the EIP itself. I just a list but I can see how that would make it harder to exit. I'd be OK with displaying them separately I think we might already do that, yes we do. Yes, we don't need to make this change.

**Gcolvin**
* This is the reason I always prefer the ITF policy. Things to draft and then it has a status But we already lost that. No point going back.

**Pooja Ranjan** 
* There's already a pool request on this particular issue. I'm sharing in chat if people would like to read more. It looks like the proposal is also in favor of creating a toggle button instead of hiding it off from the dashboard.

**Gcolvin**
* That's just a UI issue.

**Sam**
* Yes 

**Pooja Ranjan** 
* Ok so is it safe to presume that…

**Gcolvin**
* It's a real point the table of contacts. I'm to the end. 

**Pooja Ranjan** 
* All right looks like we're generally not in favor of this proposal. To hide stagnant and withdrawal VIPs from the EIP list, so we can leave a comment here. 

## Changes to Final EIP [5:20](https://youtu.be/ylDXaR31gYg?t=321)

**Pooja Ranjan** 
* The next sub item is changes to final EIPs. I have found a bunch of EIPs that are already into final status. Authors have requested certain changes sometimes the original author or someone contributing from the community. I have listed all of them here the first one for example is  Update EIP-5375: Fix typo in JSON ethereum/EIPs#6104 share this in chat. Generally speaking we are not in favor of final proposal getting updated but these are available in form of pool requests. Any thoughts on what to do with the EIP’s?

**Sam**
* Yes so I think this one is an author that approved it. So it's probably just waiting on me to merge it.

**Pooja Ranjan** 
* OK so the next one is a change for EIP 20. Obviously there's some strong opinions about it. If anyone from this group would like to add your thoughts. So the EIP 20 is a very old IP. Which has been widely accepted so the main concern is have these changes attitude EIP 20 all together or maybe have a new proposal altogether?

**Sam**
* I haven't looked through the PR yet but if it's just formatting then I'm fine with making them I think that's OK.

**Pooja Ranjan** 
* I think Matt you had a strong opinion on that, maybe you'd like to add why you think it's not a good idea. To have new recommendations fit in to this proposal. 

**Lightclient**
* I'm sorry new recommendation for which proposal?

**Pooja Ranjan** 
* The pool request is # 6038 for updating EIP 20. 

**Lightclient**
* Yes I don’t think we should be updating old EIPs in the ?? 

**Sam**
* I'm fine with that too. 

**Lightclient**
* Occasionally I like smaller changes but this is a very widely read EIP. It would be weird to make large changes to it.

**Gcolvin**
* Which EIP are we talking about?

**Pooja Ranjan** 
* #6038 you can find the link in the chat.

**Gcolvin**
* Yes found it. There was a few other links so I wasn't sure. Let me look at those changes.

**Pooja Ranjan** 
* It's about the use of license changes with the proposal that has been recently merged.

**Gcolvin**
* Yes we sure not to mess with the PIP 20 more than necessary.

**Sam**
* Yes these changes go beyond the minimal requirement to meet the current standards. As written I wouldn't approve this.

**Pooja Ranjan** 
* So do we want to have further edits in the pool request? Or do we not want to include these changes in the EIP 20 altogether? 

**Sam**
* I think it's fairly nuanced I can make some comments on the actual PR. I think by moving simple summary to description is a perfectly fine thing to do. Changing it from solidity 0.4.17 to 0.8.17 is way out of line for what we should be doing. What's everybody else's opinion? 

**Gcolvin**
* I agree. 

**Pooja Ranjan** 
* OK it seems like most of the editors are in agreement that we should not make changes to Final EIP.  So we can close the school request with a comment.

**Gcolvin**
* Slow down this does bring up an interesting issue. The solidity code is out of date. People use this to build on and we're giving them a version of solidity that won't compile anymore. Possibly. But I don't know in general how we wanna handle that or should we just leave it to the user. 

**Lightclient**
* I want it compile?

**Gcolvin**
* I don't know yet overtime solidity versions are not backwards compatible. 

**Sam**
* Call data memory thing. 

**Lightclient**
* Right but, oh, I guess because they picked that version there. But there's no need to update it. Like you should compile.

**Gcolvin**
* You have to tag the version or you don't know what version you're looking at with solidity. It's generally unfortunate that we use solidity for this type of specifications. Just don't know if we should have a way to update these things once they get grotesquely out of date.

**Sam**
* I also agree with that. I don't know what to do?

**Gcolvin**
* I guess I could take a new PR. But that seems silly when nothing changed. I guess it's a question of if solidity gets to a point where it just won't compile. Really obvious changes. And I don't know solidity well enough to judge. If this is still going to compile OK.

**Pooja Ranjan** 
* Is it safe to summarize that the current PR or in the current form we may not be able to merge. We do not have consensus on that, However if we are changing the solidity version. It may require a new pull request to be sent out for consideration. 

**Gcolvin**
* It's just a dangerous thing. Making sure the new solidity does specify the same thing as the old solidity. When things are not backwards compatible and there is no formal specificity. The alternative argument is to just leave it be that you can figure out from that what the authors intent was.

**Pooja Ranjan** 
* Ok I'm trying to summarize it and also it will be in the notes. But this pool request we did not get a general consensus here. However we are soldering updating solidity in old proposals not in the EIP 20 but in general.

**Gcolvin**
* I'm not saying we should I'm saying. There is an issue here to keep in mind. There's no way we can go back through all the EIP's and update their solidity. But it is an issue especially if the authors EIP the need but it doesn't feel right to alter a final EIP. I'm just pointing out there's an issue and it may take a new IP to do it. We may in the future want to separate that out. This is a fairly unusual EIP in that way.

**Pooja Ranjan** 
* Right, maybe we can create an issue on EIP get hub to discuss updating solidity in earlier proposals. 

**Sam**
* Yes I am doing that right now. 

**Pooja Ranjan** 
* OK thank you Sam. 

**Gcolvin**
* I don't know if the author of this one wants to take that on? As trimming this one back somehow, keeping the discussion going. It's our panda here anyway is he on the call? NO he’s not so we should kick this down the road and he's here to talk about it. 

**Pooja Ranjan**
* Very well, and Sam is already creating an issue for updating solidity concerns. Moving onto the next pool request which is  Update EIP-721: Update link ethereum/EIPs#6012 thoughts or comments on this? This pull request is by the original author. It looks like some people are entry and some people are not. We don't have any thoughts right now I'm also trying to share these PR's so we can take a look after the call. And the last one here is.

**Gcolvin**
* I'm just still trying to figure out this, is another final one we don't wanna touch. I'm just trying to figure out why he really wants to touch it.

**Sam**
* It's a broken link that's what it comes down to.

**Gcolvin**
* There's a lot of changes here for a broken link.

**Sam**
* We're looking at 6012 or? 

**Gcolvin**
* Yes 

**Sam**
* He hit the three dots at the top you can turn off the annotations it's just the bad complaining because it's a really old EIP.

**Gcolvin**
* Oh ya cleans it up thank you.

**Sam**
* No problem. The only change is the link down at the bottom.

**Gcolvin**
* Is this a normative link?

**Sam**
* It is a link to another project that implements save EIP 20, it doesn't look like it's part of the spec.

**Gcolvin**
* I don't care.

**Sam**
* We could just remove the link.

**Gcolvin**
* It's fine I don't wanna touch it. 

**Sam**
* OK

**Gcolvin**
* It's not normative it's not required to understand it if someone's really motivated to understand it they can find it. And this is why we want to severely limit outside links.

**Sam**
* If Greg is saying to not apply a PR, I think I’m in powered to say we’ll just close this PR.

**Gcolvin**
* Gone around this is an example of where they go wrong but it's also an example it's not normative so it's not really a problem. It would be much better it doesn't look like there's much of anything except the link to get to this anyway. It's a link to some code, that's no good the master keeps changing, should be a link to some particular commit. He still hasn't fix that anyways. Oh yeah he has a link to a particular commit. OK I see what he's trying to do. He's trying to fix an old mistake. OK this is slightly more on the edge. I mean this is 721 we've got a whole fucking industry Built on this. OK I'm sorry I didn't review this sooner but let me go look at this. Where is that referenced in text. We have a concept of Arata but we have no process for it. It's long past due to just get our act together on Arata. Then we can handle these things. This is an old one and stands with references. Yes this is harder than I think.

**Pooja Ranjan** 
* It's all right we don't have to decide on it right away I just wanted to bring it to your attention. But you can leave comments and feedback so it's not missed and to see if we could quickly come up with a decision with anything listed here.

**Gcolvin**
* There's also an example of why outside links are useful. In motivations and rationales because he's going through existing prior art in the rational and it's generally a good idea to take a count of standard art. When standardizing some thing without the links he's just going to be making bold assertions based on prior Art and thanks at all. Really inclined to take this as an opportunity to find a process for Arata, and then these can be handled as Errors. Without actually modifying the final text.

**Sam**
* I'm down to have some thoughts about Arata. What were allowed to change.

**Gcolvin**
* It's old so things are broken out but he's got standards he's referencing some of that's probably normative, some issues and various discussions. The other is clearly not normative. A lot of the prior art that he's trying to incorporate either directly, he's referring to ERC 165 that looks to be normative. I'm really inclined to throw it back to the author's once we've got the Arata process and fix this. This is a very important ERP and it's important that people can understand it and it's worth trying to figure out those links that are going to cause a problem understanding it and which ones can rot without it being an issue. At least how I've discussed it everything needs to be normative. And what's not in a specification is not normative. And the EIP are mixed together.

**Sam**
* I'm tempted for this one to say it doesn't hurt the understanding of the EIP to this link rot. So we'll just leave it but we mentioned that we might have a more formal Arata process. And we can revisit the issue at that time.

**Gcolvin**
* yes 

**Sam**
* Ok are you all right with that Matt?

**Lightclient**
* Sounds good to me.

**Gcolvin**
* I would Kick back to William how to sort out which of these links are normative and which ones are not. Because the ones that are normative we have to keep an eye on. 

**Pooja Ranjan** 
* OK I think we can have an issue for one of the upcoming meetings for the process of Arata. And we can have more discussion on how to define the process. If you can leave feedback for this PR to distinguish between normative and a normative links that would be nice. If the author would like to respond to that and if not we can let it be there for some more time.

**Gcolvin**
* That makes since. 

**Pooja Ranjan**
* OK there's one last discussion needed for Include Ganache private chains (5777) in EIP-155 ethereum/EIPs#5877. This is a word proposal offered by Vitalic. Replay attack protection. So the proposal is to add an additional line to Ganache GUI private chains. Yeah there's a comment in the chat but that should not go in.

**Sam**
* This is a list of the existing chains at the time right? 

**Pooja Ranjan** 
* Yes 

**Sam**
* No we're not going to do this there's no way we're modifying EIP 155. It probably shouldn't have had a list in it in the first place. And EIPs are not the best place to maintain lists. So I’m just going to close this unless somebody objects.

**Pooja Ranjan** 
* Any present objections from any EIP editors? For closing the PR. OK it looks like we have no objections. We have a heard consensus that they are not interested in changing the existing a EIPs. As you said this is not a good place for maintaining lists and so we will go ahead and close this one.

## 2. Discussion continued from earlier meetings [30:06](https://youtu.be/ylDXaR31gYg?t=1806)

**Pooja Ranjan** 
* This proposal has been discussed before.  A Straw-man Proposal https://github.com/ethereum/EIPs/commits/master/EIPS/eip-6049.md Update EIP-3475: Changing comments ethereum/EIPs#5789 Victor if you'd like to summarize your proposal? And people can share their thoughts and opinions.

**Victor Zhou(@xinbenlv)**
* The idea that I've heard from various authors and editors is that there's no clear criteria. So in advancing status some would like, a very easy way to get to final. Some Think going to status is too fast. Some think that going to final the EIP didn't have enough consensus or demonstrated interest to go to final. This is an attempt to formalize what he means for each status. And the highlight is what we already know at core is, obviously require client implementation. I understand what he means by client implementation and getting it applied in their platform. But when it comes to ERC network and interface there's no hard requirement and this race concerns that EIP is going to final too fast. We also saw things like EIP 712 and that was going into final status prematurely. It has a lot of interest it's being widely adopted. Also recently discovered 3475 and that's had a lot of editorial issues even after it passes the final. I just want to propose some thing that people can agree on. One of the contentious ideas to attack is require also implementations for net work interface and ERC just as we require for the core. I'm personally in favor of that because I think a standard without multiple limitations is now counted as a standard and it doesn't make sense to finalize them if no one really cares to implement and deploy it. The other thing that people propose is that lower bound, which I think Pooja approves of? And recently in the same thread another author proposed an upper bound which is proposed to move to next step. I just wanna put it on the table and bring it up to this group to see what you think. The current proposal is that for all the standard tracks in that discussion and implementation, to advance to final. And for meta and informal wait for consensus even longer. I'll just pause here to see what you think.

**Sam**
* I don't want to add any more requirements to make it even more difficult to get an EIP finalized. And I think we make it very clear Final is not an indicator of adoption. Or use or quality of the EIP's technical merits it's just a statement of whether it's going to change or not. And I think that adding multiple requirements for implementation or having certain levels of adoption before moving to final. I think that will be too taxing on the EIP process and what benefit is it going to bring us? It's going to bring even more standards just sitting in the process, draft, or review for even longer it's of time and I don't think it's going to help anything. And on the minimal length of time between changing statuses I think it seems like adding delays for no reason. Maybe we need to do a better job as editors of making sure that sufficient discussions has taken place but I don't think a time bound is going to change anything. EIP 712 was sitting in stagnant for years and it's still ended up a mess. I don't think a time limit is going to improve anything if more people aren't looking at it.

**Victor Zhou(@xinbenlv)**
* I heard Sam saying he doesn't want to tax authors more because that will create barriers to advance to final. What do Greg and Matt think?

**Lightclient**
* Would mostly echo what Sam said. We spent a lot of time trying to separate the concept of readiness for EIPs and moving them into a place that is fixed. And then letting the readiness be defined outside the process. 

**Victor Zhou(@xinbenlv)**
* Ya ok how about Greg?

**Sam**
* Greg has Pooja's icon again.

**Pooja Ranjan** 
* That's funny.

**Gcolvin**
* I don't really have a strong opinion on this. Except not too many more obstacles.

**Victor Zhou(@xinbenlv)**
* My intention is not to just react and propose something to add obstacles. Every now and then I hear editors or authors saying, is this EIP even worthy. And then that creates a lot of debate. If we can say that the worthiness is not going to be controlled by entirely by the author or by the editors that would be a good thing. On one side I worry that if we just allow authors to propose EIPs, unless you guys are super open, which I can also lean into, then we would be expecting an order of magnitude of 10,000 more EIPs coming in. I don't know if this is what this repository wants? And the other thing is either we let editors single-handedly or as a group decide wether a EIPs is worthy. This is a burden as well as a lot of single subjective biases to EIP editors. Some may argue how about we look at a thread and see who was on the discussion and that's still very subjective and therefore the worthiness we're trying to look for something that is Objective in determining worthiness. Seen interfaces that are not even compatible in Reddit and it's still made into final. So that's why we wanted to imply some implementation requirements to at least make sure that it works.

**Sam**
* Do we ever determine worthiness?

**Victor Zhou(@xinbenlv)**
* Some implied like one of the EIPs, I interact by being asked buy an editor is it worthy? That is a technical peer feedback that's fine. As an editor asking that it might imply that there's a gap editorially to enter an EIP.

**Sam**
* So I think asking if the EIP is worthy or not it's fine but if the author says yes I don't think any of us would stop it from going through the only time I think we would stop it for EIPs that are not expected to have multiple implementations that have to have interrupt. That I think is the only bar of worthiness that we enforce.

**Victor Zhou(@xinbenlv)**
* That's true. That's pretty subjective right? Like how do you know that there's going to be or not be implementations?

**Sam**
* It's not that there will be or won't be it's about whether the proposal standardizes some thing that would have multiple implementations. Even if there's only ever one implementation by the EIP author that's fine if we standardize it. It's the weather or not there's the expectation that someone else could come along and make another compatible implementation.

**Victor Zhou(@xinbenlv)**
* Well for me I am ok to reduce that down to one implementation. I'm more in favor of having multiple ones. But I think it's OK to require at least one. But we've also seen EIP's go in without showing or without having implementations and finalized…

**Sam**
* Is that a problem?

**Victor Zhou(@xinbenlv)**
* I think the problem is that one EIP did not work and waste editors and future authors time not authors but implementers time.

**Sam**
* That is kind of annoying. If the EIP doesn't work. But that's kind of what the implementation threads are for. Somebody on there probably would've said something and hopefully. Can a final EIP be withdrawn is that allowed?

**Victor Zhou(@xinbenlv)**
* That's why I'm trying to, I do feel the sentiment in this room today. That you don't want to add hurdles to authors. I'd love to have authors be easier for them to propose. And I consider myself mostly an author. I just wanted to put it here and see maybe see if in six months from now this will come back up and we can use that as a basis to discuss what kind of criteria we want to require for our advancing at status. Anytime I hear a complaint about some thing going into status too fast or too slow maybe we can use that thread as a discussion to better improve our to set an expectation of something to be expected for status advancement. 

**Pooja Ranjan** 
* If I may say here I am not sure of any EIP so far which has been put into final status and it was not working. The idea of standardizing is to have a standardized process in place any implementer or dap developer may pick up that standard and try to add it to the project, they won't want to implement Standard into the project. And adding too many boundaries for people to submit a proposal to become a standard is something I think it's not very fair to them. However I'm open to the idea for example we can probably come up with some other policies just like Sam mentioned we can finally have EIPs withdrawn. So when we come across a proposal that is actually not functioning which I think is not going to happen because we have multiple eyes on every proposal. The moment that it enters into a pool request or goes to a fellowship of Ethereum magicians so that it's rare case that a proposal would get into final status so we should not increase our boundaries. I'm in favor of having more discussion into the discussion thread. If I'm not mistaken this proposal idea may have been fired by a pool request that I found from a meta-EIP which is currently and it's last call. In under 30 days which I really think is not idea for proposals under Meta category cause that is a process related proposal. That should be discussed in the EIPIP meeting so we should think about some thing around how we can increase the length of discussion but not hard coating the length of that discussion in the EIP. 

**Sam**
* We have started the peer review process where we nominate people from the list so that will help a little bit. Not for meta-EIPs obviously but for regular ones. 

**Pooja Ranjan** 
* Meta-type is generally related to process and I think EIP editors must look into it. And any Matache should not get into final status in less than a month or so.

**Victor Zhou(@xinbenlv)**
* Even in favor of setting it for 60 days for Meta. If something is procedural it should take longer and we should let more authors know the editors who look at the EIP repository and discussions so frequently. 

**Pooja Ranjan** 
* This came to my mind that the period of 14 days definitely gives us one EIPIP meeting in between last call to final status. I mean obviously I can bring it up in the meeting but yeah. Any other thoughts on this? 

**Gcolvin**
* Agree that some arbitrary amount of time doesn't help. There's a bigger issue of whether we should really have an implementation before it goes final. With core EIP's by the time it goes final it's on the main net. Mini RC's there is a lot more useful implementations and people will know it works. Four ANSI standards work we wouldn't accept library proposals which are non-core proposals. Strong desire is to have an implementation that would standardize what was already implemented. So it would seem reasonable to to generally not go to last call or at least not come out of it without an implementation that would be the indicator to whether there was enough interest to proceed. If nobody wants to implement it what's the point?

**Victor Zhou(@xinbenlv)**
* Yes that's what I thought too. And by the way this is not to add a hurdle for something to be proposed. This is for adding a bar for something to be finalized. Just wanting to make that distinction clear.

**Pooja Ranjan** 
* General understanding from the time something is proposed and added to get hub repository till the time it is last call it generally takes 3 to 4 weeks in normal cases. And sometimes there are a lot of proposals and it does take time to review them. And on top of that if we had 60 days till last call defining the length of any meta-or informational EIP cannot be less than three months and sometimes if the initial period is one or two months then adding an additional one or two months maze cause the authors to lose interest in pursuing it and it will go stagnant. And even if it's a good proposal the author still may lose interest. So we are not in favor of setting a hard 60 day boundary however what was discussed in the last meeting of peer review and adding even more reviews would be a good idea. For having core EIPs we follow a little different process. So we can just exclude that because it should be implemented by the client team for the ERC. I think we discussed in the last meeting that having a prototype would also be a good idea and having a strong discussion about that would be a good idea. But waiting until the implementation is ready because the proposal may not have time and bandwidth to implement it. He or she may have to find someone else to get it implemented. On a project level

**Victor Zhou(@xinbenlv)**
* I agree to most of those points. The meta-waiting for 60 days you mentioned the author may lose their interest In pursuing. I think if you're proposing a meta-, not an old meta-only recording the hard work but then latest status we only use meta for procedure. Someone proposes a meta-EIP and loses interest in the future after just 60 days I think that shows strong enough interest for. On the other hand if something is really important and we agree has a lot of consensus by this group even if the author lose interest matter in EIP can still advance to final. Or get into the last call sufficiently. Because the group will continue to take on and finalize things we see for other standard EIPs I wouldn't feel too uncomfortable for us to require a longer period for people to give more feedback on meta. For information I really don't care because it's on binding I really think information should only be life and have subject to future changes. That's my opinion. 

**Pooja Ranjan** 
* OK we are very close to time so if anyone would like to give thought final thoughts or feedback here we don't have any pool requests. So we don't have to make any decision. However we do have thread at fellowship of Ethereum magician and you can follow the link found an agenda so people can definitely add their thoughts there. Does anyone want to give anything Final piece of feedback? Ok I think we can continue to collect more feedback. And we will revisit this discussion in future meetings and for this meeting I wanted to bring up one final issue we don't have to finish it here but we can begin.

## 3. EIP Bot [53:28](https://youtu.be/ylDXaR31gYg?t=3208)

**Pooja Ranjan** 
* "Requires" section should not accept Withdrawn EIP ethereum/EIPs#6131 the Bot allows final stagnant and withdrawal EIP. My proposal here is that withdrawal EIP they be removed from there because the withdrawal EIP may not have a necessary followed through the steps of a standardized and may not be ready to be an EIP that can be considered for dependency. I have created an issue for that the issue #6131 if anyone has any thoughts or comments they’d like to add?

**Sam**
* So I guess the rule would be with EIP's are allowed to have withdrawal EIP's and that requires a preamble header but the other EIPs are. Is everyone OK with that? 

**Pooja Ranjan** 
* Yes I think that is a better wording for that thank you Sam. Greg or Victor if you have any objections on this or maybe I thought?

**Victor Zhou(@xinbenlv)**
* Sorry I was taking notes on the previous discussion. I will take a look and you can proceed to the next item.

**Pooja Ranjan** 
* this was the last one and we're out of time. I have added the issue #6131 hopefully we can make this change.

**Victor Zhou(@xinbenlv)**
* I think it's very good I am in full support of it. Should we also in void stagnant being referenced as required? 

**Gcolvin**
* My concern here is one author can pull in another EIP as requirement at a stage for example if they're both in draft. Which is not a problem and then and then the one that they're referring to requiring falls into stagnant or gets withdrawn and then what does the original author have to do.

**Pooja Ranjan** 
* One correction that I'd like to mention here is the current EIPW allows for final withdrawals and stagnant actually it's final living and withdrawn stagnant not considered in the first place. So the only status which is under question is  withdrawal. Should allow withdrawal in the required section or should not? 

**Gcolvin**
* Probably not. Maybe this is an old worry but it is a pain if you refer to another draft and the draft slips off to stagnant. Should you have to go over to what slipped off to stagnant and make it a draft again? Order for your proposal to succeed. 

**Pooja Ranjan** 
* At present it's not allowing draft at all it's only final and living proposals. 

**Victor Zhou(@xinbenlv)**
* I am in favor of leading draft and review status be as flexible as possible and reference anything like even if it's stagnant work or I'm OK to band or not band withdraws but I think we give a draft maybe that's OK. I think for getting into last call they want to make sure that the requirements are that the EIP we depend on should be in at least last call. Because somethings going to last call is soon to finalize and should be treated more seriously and if at that point somethings still stagnant or withdrawn the author should remove the requires if it's not a hard dependency or be motivated to pull and take over and then drive that into last call. Depending on if the EIP is a requirement. 

**Pooja Ranjan** 
* I think that would be too much of a hassle for editors if we start allowing drafts in review because as Greg was saying there are chances that they may end up on withdrawal or stagnant and so on the safer side I think it's a good idea for bot to allow only final and living. even withdrawn can be taken out accept for the withdrawn proposal. 

**Victor Zhou(@xinbenlv)**
* I think what I said is that bots to not even complain for drafting and reviews. If this EIP is in draft status. 

**Sam**
* OK for reviews I think we have to have the restriction because it requires header and requires reading it's necessary to understand the current EIP. If the current EIP is ready for review that means all of its dependencies also have to be ready for review. You can't review and EIP if its dependence are still allowed to change freely they have to move in somewhat of a locked step. For draft it's fine like draft can refer to draft. 

**Gcolvin**
* Yes I don't have a problem with draft referring to any state.

**Sam**
* Yes so draft and stagnant can refer to anything. 

**Gcolvin**
* Yeah that just means if you wanna move out of draft and into review yeah I have to somehow resurrect what slipped out of draft. I think I understand. 

**Sam**
* OK I have to drop off thanks for coming everyone.

**Pooja Ranjan** 
* Thank you everyone I'm not sure when the next meeting will be because it is falling on vacation time. So I will take a poll or ask people what they like to do with the next meeting. Thank you everyone for joining. 


## Date and Time for the next meeting

2022 Dec 28, 2022 at 15:00 UTC

## Attendees

* Pooja Ranjan
* Sam
* Gcolvin
* Lightclient
* Victor Zhou(@xinbenlv)

## Links discussed in the call (zoom chat)
* NA
