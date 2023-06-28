# EIPIP Meeting 83 Notes
### Meeting Date/Time: June 14, 2023 at 14:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/241)
### [Audio/Video of the meeting](https://youtu.be/UHqkpwt_3XM)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
83.1 | **PR-6907** - No objection from EIP Editors present in the meeting. It will be merged.
83.2 | **PR-7111** - No objection from EIP Editors present in the meeting. It will be merged.
83.3 | **PR-7113** - No objection from EIP Editors present in the meeting. It will be merged.
83.4 | **PR- 7117** - No objection from EIP Editors present in the meeting. It will be merged.
83.5 | **PR-6834** - No consensus achieved. It was planned to get back if we get time at the end, but did not get enough time to discuss.
83.6 | **PR-6813** - @SamWilsn will take a look offline
83.7 | **Reopen EIP draft** - EIP Editors not in favor of reopening.
83.8 | **PR-5682** - @SamWilsn proposed to rename "Security Consideration" to "Security & Privacy Consideration". | @xinbenlv @gcolvin are in favor. @g11tech is neutral @lightclient not in favor. No consensus yet.
83.9 | **Splitting ERCs and Core EIPs** - @timbeiko shared that now we have EIP & ERC Editors to better manage processes separately.
83.10| **Splitting ERCs and Core EIPs** - There are entirely different users of both processes & Perhaps separating them will provide a better opportunity for evolving processes separately.
83.11| **Splitting ERCs and Core EIPs: Problems identified** - Numbering of EIPs & Placeholder
83.12| **Splitting ERCs and Core EIPs: Proposed solution** - Odd-Even EIP numbers & Have a separate repo as https://github.com/ethereum/ERCs
83.13| **Splitting ERCs and Core EIPs: Open question** - What about Interface, Networking, Informational, Meta EIP? & Will that be a part of EIPs or ERCs repo?
83.14| **Splitting ERCs and Core EIPs: Next step** - @timbeiko will add an item to collect client teams' thoughts on the split of the rep & Depending on how the ACDE call goes about this, further action will be taken. Recommend watching the recording for specifics.

# Intro
**Pooja Ranjan**
* Welcome to EIPIP meeting 83. I have shared agenda in chat. This  issue number 241 at EIPIP GitHub repository. we have a bunch of pull requests and issues added, from the EIPs repository to be discussed today and probably to make some decisions towards the merging. The first set of pull requests are the list of PR proposed by Sam Wilson to update EIP-1. 

# Update EIP-1: Update EIP-1 to allow link to BIPs ethereum/EIPs#6907 [0.58](https://youtu.be/UHqkpwt_3XM?t=58)
**Pooja Ranjan**
* Anyone having strong feeling to merge these and not probably we can discuss one by one. So the first PR here is 6907. It is to update EIP-1 to allow link to BIPs any part objection support. 

**Sam**
* So I think the only person with an objection was, Gavin and I don't think they're here. yeah. 

**Pooja Ranjan**
* All right. we still have I think three, four more EIP editors, so anyone from the editor's community other than Gavin having strong opposition to that. 

**Sam**
* All right. So I think we can probably go ahead with this and then we can resolve Gavin's, Concern on the pull request. Yeah, exactly. Well, we can resolve it after, as long as everybody else is on board with this. 

# Update EIP-1: Add W3C as a permissible origin ethereum/EIPs#7111 [2.04](https://youtu.be/UHqkpwt_3XM?t=124)
**Pooja Ranjan**
* Sounds good. So we can move on to the next number. And that is #7111. It's add W3C as a permissible origin. All of them are proposed by Sam. so I'd be curious to hear, thoughts from other editors. yeah, if you have any objection or anything you would like to add or in support or not in support, I think it favor, I can see no reason at all not to allow it. 

**Sam**
* Perfect. 

**Pooja Ranjan**
* And we're okay with the, the wording as written or Any changes we would like to see in the PR in wordings or we are good. Probably we can start with the same wordings if we do not have any, anyone opposing to that. Very well. We are just joined by light client. Matt, we were discussing issue number, sorry, the pull request number #7111.
* So it is about to Add W3C as a permissible origin. Seems like most of the editors are on board. Just checking in case you have any thoughts, concern with this one, especially with respect to the wordings, as is. 

**Sam**
* There's actually still some discussion on the Add W3C as a permissible origin, so we'll have to, I, I'll go over it again to make sure everything's good, but as long as nobody objects, I can, I can merge it. 

**Lightclient**
* Yeah, I haven't looked at it closely, but it seems fine. 

**Sam**
* Yeah, we can probably just deal with these all as one big group. So like, bips, anybody object to linking to Bitcoin improvement proposals? Speak now or hold your silence. All right. W3C. All right. ITF RFCs. Are we allowed to link to those? Anybody? Object. Cool. And then, the what? Working group? Any objections? 
* Cool. the yellow paper. I know you object, Matt. So, I will let you make your case again. 

**Lightclient**
* The yellow paper is not up to date and it's deprecated in terms of the using the execution spec. So I don't think we should allow authors to continue linking to it. 

**Juan Caballero**
* Would it make sense to link to, I dunno, like the execution APIs repo instead or something like what's the equivalently authoritative stable link that replaces the yellow paper Execution specs. Oh, okay. 

**Sam**
* Yeah, so we'll just leave the yellow paper off as that, as that's contentious, but yeah. all the other ones, I didn't hear any objections, so I will merge all of those. 

**Gcolvin**
* The execution specs are not useful for that purpose. They're, they're code, you can't, they're not useful for the purpose that the yellow paper is. You can't, you can't express concepts. You can't say, this is a concept that I'm using that you, you can't just include blocks of Python code, to explain. I'm sorry, we've been here before, 

**Pooja Ranjan**
* So We can probably go ahead and merge the first four and, we'll leave that open for any further discussion. 

**Gcolvin**
* I greatly object to disallowing the yellow paper. It has limitations, but it's the original fundamental specification of the protocol. 

**Zainan Victor Zhou**
* If you're, I agree with, you know, Greg. 

**Sam**
* Yeah, I mean, I'm, I don't mind linking to the yellow paper, like to a specific commit of the yellow paper because even though it's not up to date, like if you're linking to it at a specific commit should be fine. 

**Pooja Ranjan**
* In the last meeting we discussed about, giving permission to specific commit. so, I'm assuming that it is being proposed with the allowing link to yellow paper with respect to having specific commit. And, it seems like, we just need to get Matt on board and everybody else seems to be on, on board. Matt, would you be fine with commits? 

**Lightclient**
* I mean, we had to do it by commit already, so it's not any different and I still don't think we should be linking to the yellow paper. 

**Gcolvin**
* Okay. So if you want in a proposal to state the exceptional halting conditions on the execution, how do you state them? 

**Sam**
* Like you're asking for how you would state them with the execution spec, you would say any, location where a subclass of, exceptional halt is thrown. 

**Gcolvin**
* And how would, how would you make a reference to that? 

**Sam**
* Like a link to a list of them or like, is that what you're asking? You're asking how you would link to a list of the exceptional halting conditions? 

**Gcolvin**
* Yeah, I'm thinking of proposals I've written and how the hell would I write them, by referring to, by making, I guess I would have to understand that piece of code, and the reader would have to understand the piece of code well enough to even understand what you just said. 

**Lightclient**
* I mean, the same is true for the yellow paper, but I think this is why we shouldn't allow it. Like, we don't want to have new specs coming through trying to describe things the way the yellow paper described it, because it's not maintained. 

**Gcolvin**
* Okay. That's a different fight I'm trying to make, but if the community decides that they do not want to have a specification, then I can't stop that. 

**Lightclient**
* I think if someone is maintaining it and it's like staying up to date, I don't really have that much of an objection to including it. 

**Sam**
* I still like generally prefer Well, That's, I think that's the problem though, right? Like we aren't linking to the live version of the yellow paper, so I don't see harm in linking to an old version of it. 

**Gcolvin**
* You link to it for concepts, it lays out the concepts. An execution spec is not conceptual, and many, the Execution spec does lead the concepts out. 

**Lightclient**
* It influence the whole protocol. 

**Gcolvin**
* That's the Yeah, but it's code. 

**Lightclient**
* It's the same way that we do the consensus layer. It works fine for them. I think that it's better to try and unify the approach that we take to specify the consensus protocol, both consensus and execution. And because the yellow paper isn't maintained, I don't think that we should be making room for it. We should focus on unification of all these things. 

**Gcolvin**
* Okay. there are thousands of references to the yellow paper in, just go to Google Scholar and search for it. Thousands of references and the, the execution spec. It is great to have it, but it doesn't serve the purpose. Programmers can read it. Mathematicians can't necessarily read it. Logicians can't necessarily read it. 

**Victor**
* We don't have a lot of mathematicians writing eip, But a lot of people read eip, so even though they might write, they might read it. And the fact that one question I have is that one reason we restrict, we put so much restriction, which I object on linking, is because some link can change. 
* I'm a little bit curious why at this moment we're rejecting linking to yellow paper because it didn't change, and get updated. This seems like conflicting with the principle why we restrict linking to it in the first place and, can expect, execution spec can in the future, stop working as well. Can be like if it happens to yellow paper that it stops being maintained. 

**Lightclient**
* Yeah. But we have three or four full-time people working on the execution specs and it's being funded by the foundation. So I have like high confidence that it's going to continue  to be maintained. Of course that can change, but that's just what we are today. 

**Victor**
* Yeah. I believe that you, you can have high, high confidence in it. so it can change just like yellow paper can stop being maintained. and I don't see the reason why that's, a paper of paper, yellow paper cannot erase, yellow paper, still have a lot of concepts that still valid, in the EVM instructions and, and, and the costs, etc, and how it works.
* The transition of states that has not changed. It does need to be updated, and I feel that we should put the resources to updating it, but it doesn't reject us from seeing yellow paper. And it's got, and, and academia and many other, group of people think it's super helpful in their view. And the fact that we stopped making to it actually reduces, the chance that it gets no notice and support. And we just, excluding mathematicians and other people from even joining this conversation

**Gcolvin**
* Anyway, there's just a long history  of computer languages, other systems that started out with reference implementations and then wrote actual specifications. EVM went from a reference implementation to a real specification. Somebody found the money and paid some experts to do that, and they did it. and reference implementations are not specifications. 
* They're not readable by anybody but programmers in the language in which they're written. And to ask people to learn Python, simply in order to participate in understanding and working with Ethereum is a big mistake. And I don't think we should contribute to it. And, I just don't see the problem, of course, in the link.  as part of the editing, it is a question of does this link to the yellow paper, is it something that's likely to change to be a big problem? 

**Gajinder**
* Maybe we allow references to yellow paper in some particular section when, where a person is giving some background or rationale. 

**Lightclient**
* I don't know why we talk about this every call. Like we need to bring the yellow paper up to spec and then discuss it. Like we just talk about the same things we talked about last call every single time. Nothing's changed in the last two weeks. 

**Sam**
* Well, sorry,  I just added to this agenda because I added all the other ones that wanted to add permissible sources. I kind of figured we'd just be like, we're at a stalemate, we can't decide, we'll just move on to something else. and I'm sorry for putting it on the agenda again. Okay. 

**Lightclient**
* It's Okay. I'm just saying we do this a lot. 

**Sam**
* I just, okay. maybe we table this. 

**Lightclient**
* I love talking to back, love talking to You guys. 

**Sam**
* Come back to it at the end of the meeting so we can get through the other stuff. is that all right with everybody? Just because I think this is gonna be the longest discussion and we can get through the other stuff quickly. 

**Pooja Ranjan**
* Yeah. Okay. Sounds good. So, just for note takers, so far we have reached consensus for the first pull request that could be merged. And for the fifth one, if we get the time today, we will come back to the discussion. And I'm sorry, Mac, if we do not get time, we probably would like to discuss it, further or whatever is decided.
* Depending upon if there is any request to get it discussed in the future meeting, we may be adding. All right. moving on to the next one. 

# CI: Bump rakefile deps ethereum/EIPs#6813 [17:17](https://youtu.be/UHqkpwt_3XM?t=1037)
**Pooja Ranjan**
* The next one  is, not, for any proposal, but it's, for about CI: Bump. Seems like it has received a thumbs up from Victor and waiting for review by Sam and Mac. Anyone has, thoughts or would like to maybe take a look at pull request number 6813 CI-bump. 

**Sam**
* Yeah, I'll take a look through it. It's if it's just dependencies, it'll be fine to do offline. 

# Reopen EIP draft Ref comment [17.36](https://youtu.be/UHqkpwt_3XM?t=1056)
**Pooja Ranjan**
* Sounds good. The next one is here, about an EIP draft, which is, now closed. And it is requested by author in the comment to the agenda that, he thinks that this proposal could be reconsidered and, this PR can be allowed to merge. I wonder what the editors think about it. 

**Sam**
* If anybody merges a PR to set a definition for EVM equivalents, I will submit a different definition of EVM equivalents. Just just to make that clear. 

**Victor**
* Oh, I think I'm on that one. Originally, I think it was, trivial that, it doesn't seem like a EIP would be BIPs. It seems like I'm slightly convinced and neutral now with the author proposing the context where some of the, evm, solutions trying to market them as EVM compatible, but in some of the behaviors, they actually did not. 
* And so that's the background of the EIP. And with that, I'm leaning towards neutral because, it seems to be, to me some value to clarify that if you really are EVM compatible, there is certain rule that you have, you can't market anything that is not, fully compatible with using capacity. I see value in that, and I just wanna hear other EIP editors about, 

**Sam**
* There is absolutely value in doing it.  It's just we are not an authority, right? Like no one here has the power to stop the Ethereum community from advertising fully EVM compatibility or compliance, like adding this EIP will change nothing in the marketing world, It's also okay, or  it's also okay that people will argue that they're not EVM mean here is one of the way that they make this argument. 

**Victor**
* I don't see the reason if there's value there, I don't see a strong reason not to included or at least as an information to show some opinion. But I'm open to hear things as well. 

**Sam**
* So, like I said, when we first brought this topic up, if anybody merges an EIP defining like VM compliance, I will make a differentEIP with different EIP EVM compliance and there will be no clarity So there like, like as a thought experiment that shows that there's no reason to merge this EIP because it doesn't change anything. 

**Pooja Ranjan**
* What's the category here? Is it informational or any other, because if it's informational, probably, it would not make much of a difference if someone wants to go ahead with this cause it's not changing the protocol or it's not even suggesting to follow it. 

**Victor**
* Yeah,  I think it's, it's a suggestion. It's more or less than a suggestion. And then, I don't know  if there's a reason in our label to officially reject this as  informational e p. So I would love to hear, like what, what's our official reason put down there? Says, Hey, be, just because, we don't think matches this criteria, we're rejecting it. 
* And then in the future, if this criteria is not met, we'll go by that as well. yeah, but I also don't wanna spend too much time on this. yeah. 

**Pooja Ranjan**
* Maybe anyone would like to comment to or maybe respond to this proposal, in the agenda itself. That would be great to have. So at least author who cannot join this meeting may get a clear response, or if we are open to have a discuss some other time, we can do that either. 

**Juan Caballero**
* I just had a question. If, isn't,  I can see the argument that the EIP group or the EIP corpus isn't where this gets decided. I feel like it's kind of a meta question is that an execution APIs question or a future iteration of the yellow paper question? Like, is there some authority, some community that would be qualified to say, you know, for interop purposes, this is the, you know, like for the sake of bridge safety and bridge interoperability, this is what we're, we're defining EVM as complete, I don't know, RPC equivalent or something. Like who, is there another group that sh would be in a position to, to define that? 

**Lightclient**
* I don't think there's really a group right now, but I think there probably should be some sort of coordination amongst L2  to describe what their standards are and the interoperability amongst them. Like we have defined the Ethereum protocol and the word equivalent has a definition and people are free to call things equivalent if they want to, but if it doesn't follow the execution specs, it's not Ethereum and that's fine. 
* But once you start opening the door for having some flexibility on that definition, I think it's like really difficult to actually describe like, what are they implementing, what are the deviations they're making? So I think that the layer two should be doing this. 

**Sam**
* I think the only way to enforce this is with a trademark. You could have a seal of approval from someone who owns a trademark and then sue people who market it incorrectly. And that is the only thing that would actually make a difference in this. 

**Juan Caballero**
* Or, maybe a test suite if that's imaginable. 

**Lightclient**
* You have a test suite for Ethereum and they can run it and if they pass all the tests, they can say that they're Ethereum equivalent, Right? 

**Juan Caballero**
* So maybe that test suite just needs to be more, have harder tests or something, right? 

**Lightclient**
* Like if they're Pretty hard, there's a lot of tests in there, I promise you no roll passes them. 

**Juan Caballero**
* Oh, okay. So then if there's already a test suite, they're failing at the very least until there's someone who feels litigious. an informational EIP could explain that I dunno, I'm just advocating for the double. 

**Lightclient**
* I mean, they know they're not even equivalent. They're trying to add flexibility to the word, like being equal to Ethereum. There is Yeah, Flexibility on this and that's fine. Like, I get it, they can do what they want to do. I don't think that we should be, you know, trying to approve of any specific definition because are, there are several different definitions about what it means to be equivalent. 

**Tim Beiko**
* One thing I'll add as well for rollups is, they're not all EVM based rollups. So it'd be kind of weird to have like EVM equivalents be like enshrined in a way as something better. Like, it feels like that's not quite the right level of abstraction where if L1 wants to like make a claim about what is or isn't the rollup, it should be something that like also includes ZK rollup, it might be something more of like a bridge standards or some amount of like, I don't know, like, and, and effectively like L2 beats is probably the best we have for doing this. But yeah, there's a risk of like, if you focus on if have EVM equivalent too much, then it's like subtly, like worse for ZK rollups, yeah, Right? 

**Lightclient**
* Like they're trying to come up with 4337, that's equivalent across both optimistic rollups and ZK rollups and it's pretty hard problem. So I think trying to expand that across all of the EVM is even harder and they just need to figure it out themselves. I don't think that we can like enforce anything upon them. 
* There's challenges that they're going to uncover as they implement the stuff and they're gonna need to make their own decisions. I just don't think that the market right now values the interoperability that people are requesting with this, like EVM equivalence standard yet otherwise they would be working together. 

**Pooja Ranjan**
* Well, it seems it's clear enough that most of the EIP editors are not in favor of having it, reopened or maybe even considered for, being a standard at Ethereum repository. So maybe, we can give it a rest. I assume, from Victor's earlier conversation that he is like, from favor is moving towards neutral. 
* So unless we get a strong support editor, we probably will not be able to reopen this proposal and move it forward. Any final comment on this, topic before we move on to the next one? 

# 2. Discussion continued or updates from past meetings
#  New contract interface and EIPs should be required to include a privacy considerations section ethereum/EIPs#5682 [28.15](https://youtu.be/UHqkpwt_3XM?t=1695)
**Pooja Ranjan**
* All right, so moving on to the next, item, which is, discussion continued or updates from the past meeting. The first one here listed is new contract interface and eip, should be required to include a privacy consideration. It's issue number 5682. 
* So initially we discussed this item in October last year, and, this issue has been back and forth on the EIPIP meeting this time it was added by Samuel to today's agenda. And I suppose it is about getting affirmation to the decision made in the earlier meeting and proposing the changes, with a PR. So Sam, if you, would like to maybe briefly go over yes. The issue and reiterate the decision, yeah, that would be great. 

**Sam**
* Yeah. So, some people really want privacy explicitly mentioned for some reason I don't really understand why. and I think I'm the only one blocking that. So I think a reasonable compromise would be to rename the security consideration section to just security and privacy. And that was proposed by Greg on Discord. 

**Pooja Ranjan**
* Are you planning to open up pull request with this, change? 

**Sam**
* I was going to, but it looks like, Matt doesn't want to allow a security and privacy section. I think just to be clear, this would just be renaming the security considerations to security and privacy. and you don't have to talk about privacy if you don't want to. It would just be a name change. 

**Pooja Ranjan**
* So I'm assuming Matt is still not in favor of this renaming. yeah, it would be gathered, you know, consensus from other editors. I know, yeah, in favor for a very long time. Sam, coming to a neutral point with, a little bit of change to the security consideration. Matt, not in favor, Greg, if you would like to add anything. And if you have any thoughts you would like to add to this one. 

**Gcolvin**
* I'm not sure what the objections are unless we just don't want to talk about privacy. 

**Tim Beiko**
* Is there a single example of a core EIPs where this would have been relevant? I can see for ERCs it makes sense. 

**Victor**
* I guess I'm just curious in core, In interface, in, in interface and network, it could also right, be useful. So maybe only core doesn't need it, and then we can exclude core for sure. but I do see value in all other layers. 

**Tim Beiko**
* I mean, I understand that just creates a bunch of like random work. I'm not an editor, but like I'm fine with just a name change. 

**Victor**
* I just wanted to make sure there's no, So one of the, the example I can think of is the, discussion, which is, Ethereum provider in router. So they're trying to allow multiple e human provider and then by allowing Ethereum provider, the involvement would be do you notify user if they should connect it, and if so, does it reveal your And then that is by itself not an EER problem. And also you could get your transaction bundle in, in some bundlers and then go through. 
* And then does that implication of your intention and does that involve possible due mvv activity? So these are, things that can get weird and core. Of course, everything needs to be, changed, but even so, I think there might be other considerations in the future. So I'm okay. The core doesn't include it. I do see, I get convinced  I start off without knowing this could be a possible thing, but I think, I think I get convinced that in other layers there's, very, often, ignorance of privacy. and we, some authors do wanna that reader know that, hey, you should actually,

**Gcolvin**
* My concern was just that, yes, often privacy considerations are important, but they are often so intertwined with security issues that trying to do them as a separate section can be difficult. And so it just makes more sense to handle them together. 
* If they're fairly separate in a proposal, well you, you do them in separate paragraphs, but forcing them into two sections when they're relevant can just make it too difficult. and, in the discussion, someone linked to the ETF advice on that and specific examples there where really they were the privacy was a concern and it was a security concern for the user if privacy was not maintained. So they just seemed closely related enough to put them in the same section. And, I just, I don't see a big objection there. 

**Pooja Ranjan**
* So I see a comment by, Sam in the chat, like, if CORE and E R C have different rules for adding, I think we should hold off until we split the repo. We do have, this discussion, as our next agenda item. So, if it is fine, we can probably give it a rest and give some time to have, the discussion about splitting ERCs and core EIP and probably not get, yeah. Yep. 

**Victor**
* Can I quickly comment on that? I think there's a part I didn't get talked about, which is the core versus other, all other EIPs, not just E R C. And the, the example I gave is about interface, and then I do think that there's a privacy issue with network as well. So if we are talking about carving out core EIP versus all other EIPs, I think that is a good discussion that we can, hold off to. 
* But if we, if we're only talking about versus and network and, and interface, then to draw, in deciding whether they should include privacy section or not, Right? 

**Pooja Ranjan**
* Yeah, I think that's a good point. But, in case we get the core EIP out of, this like rest of the eip, not only just with E R c, also from interface and networking, I'm not sure what is the proposal here, but if we do, then, probably getting to a consensus about this particular word one will be way easier than it is right now. All right. so let's try to give it a rest, right over here, we have about 20 minutes left on the call. 

# splitting ERCs and Core EIPs [36.32](https://youtu.be/UHqkpwt_3XM?t=2192)
**Pooja Ranjan**
* So let's get into the, the next item, which is kind of one of the biggest can of worms coming our way. So the next item, that we are going to discuss is about splitting ERCs and core EAPs. Most of the people on this call are very much familiar with the discussion point we have been discussing in this meeting as well. I'm curious to hear, what has seen since last and what do we want to discuss for today's meeting? So proposes, please take it away. 

**Tim Beiko**
* Sure. Maybe I can start. yeah, so I guess what changed since the last time? So we now have people who are like reviewing ERCs and like, you know, like thinking about them as like a first class thing as part of EIP editors. And I think that was always like for me, the biggest blocker where if like, I didn't want to like end up in a world where we just like break out the RCS and like this, there's like no one reviewing them. and Matt and Sam have like agreed that they could stay on the editors on both sides if, we were to split things. 
* So, yeah, I think having that, like means we have probably like the capacity to handle both repos, in terms of why we should split them. Like I think high level is just, there's different, there like very different users for each type of like EIPs, whether that's like, ERCs or like protocol changes. And talking with client teams, you know, it's like increasingly, like every, every time we talk with them, basically they say they'd rather have it split and they'd like to see the EIP process sort of evolve in a direction that's like more closely coupled to like protocol development and similarly, you know, just a bunch of things I can imagine from the ERC sites where it would make sense for that to evolve to a world like towards something that's more coupled with like application layer development. 
* Yeah, so I don't think it's like any like huge new reason for like why we want do this. I think it's something that like, at least on the core side, like pretty much all the users or like folks I direct with who like write EIP would rather have this changed. and if we have the resources to do it, I think it, it makes sense to, yeah, I'll pause here, but it's the background. 

**Victor**
* Tim, what's the intention? Which level do we out? Is it just core EIP and network and interface in the, network interface? 

**Tim Beiko**
* I think networking probably makes, so I think core network and networking makes sense together for sure. Interface is a bit of a weird one. I, like, I don't have a strong opinion. I could see it go either way. and maybe it gets duplicated like across both categories. and yeah, honestly like maybe interface meta and information will sort of get duplicated or sent to one side or the other. 
* I don't have a strong view on that. I think, core networking makes sense together. Meta probably makes sense more on the core side, just because of how it's been used historically. informational seems informational and interface seem like maybe they could just be duplicated. and then, yeah, so the, the question okay, of numbering. My, very simple proposal for numbering is like, you use odd numbers on one side, even numbers on the other side. So like we we're moving to the bot and you just have the bot, you know, module one, module zero, depending on which repo you're in. So like you, you, you sort of start from the same number and that means you're gonna have to hard code it, you know, on, on one side. But like, say you, you started from number 8,000 or whatever, then you just like increment using, yeah. even or odd, and better Like Simon twins. 

**Gcolvin**
* Sorry, They're gonna be like Siamese twins. 

**Tim Beiko**
* Yes. 

**Gcolvin**
* Basically, which over time Joined at the hip for life. Well, hopefully over time they can like each walk their own way and like, And they start, they start their numbering system separately and people go, oh, these two numbering systems are independent. Otherwise it's just sorta, I don't know, this, this whole discussion has struck me as so stupid from the very start. 

**Tim Beiko**
* Well Sure, but like literally every client dev I speak with would rather see this, so, and like I get that you object to it. 

**Gcolvin**
* I don't, but it seems like, yeah, it just seems like, yeah, There's, what does they really want splitting them I think is just, it's just an administrative system that we use to file things and give them numbers and run some bots. the conceptual distinction is what matters. 

**Lightclient**
* And that, So we don't want to set the same process down for both. Like it would be nice if we could have some of the process be different for ERCs. And right now it's not easy to do that. 

**Victor**
* What's, it's Already different, right? It is already different that to finalize you need to actually be, going through the hard work. 

**Lightclient**
* That's not, that's not a requirement. 

**Victor**
* I think it, yeah, it's right. 

**Lightclient**
* It's in IP one, It's, I don't think it's in IP one. 

**Pooja Ranjan**
* True. So the present presenter difference between core and you know, any other proposal is like core, generally is when it is with a network upgrade. We keep on waiting the last period, I mean like when it reaches to last call, that also happens when it goes on testnet, not before that. So there are certain criteria which kind of keep it separate from rest of the proposal. 
* So it is different. I think it would be interesting to understand what is this, what is that is blocking, you know, because oh, It doesn't, sure. 

**Tim Beiko**
* Yeah, yeah, yeah. So it doesn't block, it just adds a bunch of random friction and you could imagine, you know, it's like we're, we're always like contrasting what's like this state today, but you could imagine a world that's like, we actually have like a really well coupled process where say to go to last call, there's something like this is actually implemented or has like a series of tests, you know, in like execution tests. And we can just get like more specific around like what are the technical requirements for like core EIP. 
* I think over time as well as we incorporate more of like the CL stuff into it, it just like reduces, having to coordinate between CL and EL is already kind of hard. Having to coordinate between like ERCs and EIP is already kind of hard. 
* So like, you know, just reducing that the like CL and EL gives you, yeah, just like less people to coordinate with. And it doesn't mean again, like, you know, some of the actual people might stay out on both sides and like, I think, but, and, and I think, yeah, it just opens the door as well to like folks in the application. They're like, that feel like this is their space and like that process can evolve more towards like an application standardization process, which is different. 
* EIP are like very, they're like something stronger in a way, in a standard where like you're not forced to use the ERC 20 standard, right? Like you can deploy a contract and create a token that doesn't use it, but like you do have to implement the EIP 1559 if you want to run Ethereum. 
* And there is like a subtle but like important difference there. And yeah, I think just like they're literally different things that we're trying to do and they sort of started out bundled together. But yeah,  it just makes sense to like have them logically separated a bit more. 

**Gcolvin**
* The ETF manages a huge range of documents, some of which are informational, some of which directly affect the internet protocol, others of which define applications that people may or may not run. And they run a single editorial staff, they have a single numbering system. and you know, I've said, we've got issues we need to solve that we keep going, oh, we'll split the repo, but that doesn't actually solve the issues. It creates issues of its own. and it comes down to things like, well, EIP-1 will get a bit more complicated. 
* Well we can, so EIP-1 has two chapters or we decide that we're gonna have a different EIP for these things. It's just, it, it introduces complications and I don't see that it, that it wins us a whole lot. and the odd even numbering thing, I keep coming back to that cuz it simply means we haven't actually separated the processes. We have to like coordinate the numbering forever. 

**Lightclient**
* And repos, I mean, I Don't think there's anything we can do about that. 

**Gcolvin**
* Like we started with them together and yes, I I We don't, I don't like the repos that's then we don't have this problem. 

**Lightclient**
* I mean we just made a mistake in the beginning putting them together. They're like totally separate types of things that we're trying to coordinate around. One is core EIPs that everyone has to implement, they have to agree on otherwise they're left behind than you have the ERCs, which is like way more similar to internet standards where it's like, this is the state of the art, this is how it's specified, you should probably use it, but you don't have to, you can do whatever you want. And I just think like, it doesn't make sense to tie these two things together. 

**Gcolvin**
* So the ETF should actually have two separate editorial things and there's Nothing in the ITEF that everybody has to implement. 

**Lightclient**
* People can do whatever they want. There is no concept of consensus. 

**Victor**
* ERC3 four is a standard, so if you don't use that, you don't get dms. 

**Lightclient**
* That's, I mean, sure, same thing with http. If you don't implement http, you don't get http. But it's like, you don't have to use http. You don't have to use dns. You can implement, you can come up with your own protocol for finding the IP addresses of names, ENS, like we have other ways of doing these things. 

**Sam**
* If you want to implement with that logic or Logic with, with that logic, if you don't want to use Ethere you don't have to use Ethereum. 

**Lightclient**
* But Then again Exactly. And you can go add VIPs to Bitcoin's repository. 

**Sam**
* And that's, that's where I'm going with this. It's like, the I E T F is so general that it standardizes, it can standardize multiple competing protocols like, POP three and imap let's say. whereas we are specifically an Ethereum document repository and there are certain documents that if you don't implement, you can't be on Ethereum right? So there's a slight difference between us and the I etf. 

**Lightclient**
* But for ERCs I think it's a way more similar analogy. Like you don't have to implement ERC twenties in your protocol, you can use a different token standard, Right? 

**Tim Beiko**
* There can be competing parallel implementations of ERCs. There cannot be for EIPs, like at least like that are final, right? Like there can be two, there's, there's been like three withdrawal EIP, but at the end of the day it's like 4895 is the spec, right? And all the other ones are just like, they then drafts and that's like a fundamental difference. 

**Pooja Ranjan**
* But that's the idea with the standardization here, like what I have observed so far, when ERC are being edited, ERC are being reviewed, we generally try to make sure that there is no existing standard which already has the same kind of specification unless there is some improvement or unless that is specifies that it is based on top of an earlier existing ERC standard, then only it is allowed. 

**Tim Beiko**
* So you can still use, sorry, you can still use ERC 20. Even though ERC 1150 fives exist, you can argue that like 1150 fives are better, but like it doesn't block people from using ERC twenties. Whereas today, like on ethe, like our main net, when we change the gas costs, costs, you can argue that the old gas costs were better, but you, you can't use the old gas costs. like, and, and that's the difference, right? You like force everyone on that change. 

**Victor**
* I actually think that, having EIP and, and I do feel very confusing when people say EIP only to referring to core EIP in some cases. So I like to use Core EIP versus all other eip and I see strong value in keeping them in the same repository and then keeping people so that people can have an eye on both sides. I don't think it's a, it's a bug to begin with. It's actually a good thing. one example is that Metallic himself tried three times to go for account abstraction and two of them were using, were trying to resolve it in a course aspect and then it didn't went very far. 
* And then so, account abstraction, the f4337 is attempting on, on a different layer. So that kind of knowledge does not get propagate very far if you have people working in silo. 
* And, and that's why I think, having four, having four EIP versus other eip, would be, would be a good idea in, in the same, in the same place. But we can definitely, if the problem is about people don't like putting in EIP, and they go to random, I'm fully with you, I think we put too much burden in, in too much restriction in author. 
* And I'm always a big fan of relaxing. Like we don't allow consideration, we don't allow people, we just make this reason that I don't feel very strong and then, over any author who wanna do this, which seems to be in the, in in the way of what and then it would not be changed. Even if the court EIP is I bet that is gonna be the case as well. I don't see very convincing, argument right now. I'll it out and actually let people come over with the current set of rules. Yeah. So unless that is resolved, I don't see this is a, I really wanna see people coming and, use this as, as their way, as a place to drop their EIP, by making it more, more flexible. 

**Lightclient**
* I mean the idea is that we're going to be able to then evolve these processes and slightly separately. Like you have all of these things that you feel are important to do for the process and I have to argue against it because I don't feel it's very important in the core process or it doesn't align with the core process. 
* And we're spending tons of time debating all these things and I think they would be useful if they were just for ERCs. And I want to unlock this so that you and other people involved with ERCs can experiment with it. 

**Victor**
* You mean non-core, right? are you referring non-core? Yeah. 

**Lightclient**
* Or do you refer to, I mean there's so few networking. I mean I think we should deprecate networking. There's not very many ER interface. I'm specifically talking with ERCs. This is the biggest ERC, this is the biggest EIPcategory by far. 

**Victor**
* What do you think about the interface? 

**Lightclient**
* I mean, I think generally we should also deprecate interface because we have execution APIs, which covers the majority of the interface, the types of things that interface standardize. The one place where it's a little bit confusing is around like JavaScript libraries and they're wanting to have standards and I think that, you know, maybe it's painful, but they should probably migrate to interface on ERCs and just like call them ERCs. I don't really care that much though. Like there's so few of them. They could stay EIPs too. Like it doesn't really matter to me Up until now. 

**Victor**
* I feel that ERCs not about anything to be, to be standardized on small contract. So I feel it very confusing to put, when you say that, they should migrate  the JavaScript library onto ERCs and No, 

**Lightclient**
* I'm saying that they should refer to their standards as ERC interface, standard ERC Web three provider standard right now they have, yeah, We're referring to interface  EIP right now, right?  Yeah. I'm saying that we should get rid of Interface EIP also and call them like ERCs and move them to the ERC repository, like things that are related to the application layer. 
* I think that should live and be ERCs and things more related to the core layer, I think should be like EIPs. 

**Sam**
* Yeah. If we divide it by audience, right? So the people who are implementing it, like and generally speaking, like networking and core will be implemented together. so they should be in repository together and like Interface and ERC will likely be in, implemented together. So they should look together. 

**Tim Beiko**
* I guess. Yeah, just cuz to be mindful of time, like I, my suggestion would be like I can bring this up on the next all cord devs and see what clients thinks, but I think if the client teams strongly desire this, like given the core EIP process is effectively there as a way to like standardize what is mostly their work, I would like to move forward with this. but I'm happy to yeah, check in on All cord devs and like be if there's like broad support for this, like client teams. 

**Victor**
* So we, have a list of items that they think it's really bad and hard for you to do in a EIP, in the current EIP with And then  felt like a lot of things is exist in our policy restriction. Like I was involved in, in the complaints that, people cannot even in, linked to execution spac. 
* And that's, that's one of the reason they just stopped proposing that I saw one of the just parted in the draft status because of one of the one one case in that. So I love to see what's the real reason that they don't like to come to EIP and we should fix that. I really feel we should fix our EIP and just relax our restrictions. We can't link to yellow paper, we can't link to a lot of things. 

**Lightclient**
* I don't wanna ask them to come up with a laundry list. Things they don't like about the EIP process, like we've asked them this in the past, they absolutely hate the EIP process more or less like this is not gonna go over 

**Victor**
* Well Wait, but a lot of times it's, I I have to be do respectful, disagree with you that a lot of policy is where's that direction? And I just trying to avoid those policy and keep making those policy. 

**Lightclient**
* I'm just telling you I do record every single day and they do not like the EIP process. We've turned into a joke to them. 

**Tim Beiko**
* Slightly, nuanced this, like, I do think people have appreciated like the small, like there's been like a bunch of small chains at the margin in like the past year or two. Like I think it, and, and like having new editors actually work on stuff has been helpful. 
* So I don't want to like, like completely dismiss the changes, but I think it's,  I would agree though it's like almost, I asking them about like what they don't like, like people feel very checked out from the EIP process in a way where like they just feel like it's like this thing that they don't really have control over or like every time they engage with it's like not the best experience and like splitting the process basically gives them like ownership over the thing where it's like, yeah this can now be the process that's focused with like core development and like we can just not have any other considerations beyond that as we're doing changes to it. I do need to hop as well though, unfortunately. but is it helpful to put this on the All core dev as agenda for next week or do people feel like there's not any value there? 

**Pooja Ranjan**
* I would also love to hear more thoughts about like what specific changes like  client teams are looking to have in the new process that is going to make it different from the present process. And that's why it would be useful for them to have a new process altogether. 

**Tim Beiko**
* Yeah, I think we Should know, like if the core team say that they want to get rid. 

**Lightclient**
* Yeah, I think we Should know, like if the core team say that they want to get rid.  Use from the core repository. Are we going to do it or are we just gonna come back to this call and block it? 

**Gajinder**
* Like I said in chat, we don't need consensus on this. 

**Pooja Ranjan**
* We do kind of need consensus though. Like, yeah, we do not, I mean, of course we can de fork the repository and do whatever we want, but that's just like we, we want to have a subdomain on ethereum.org that says ERCs and EIP, and somebody has to decide who, you know, picks the repository that appoints to. And those people are kind of us right now. 

**Victor**
* Yeah, I mean domain, I'm happy to sit in a core group and ask what kinda and then we can make that, list and see if it's, it's doable. And maybe they'll come up with a ideal state that it's achievable and then either it's by forking, that's fine. Either it's not. 

**Lightclient**
* The core devs are not going to babysit the EIP process. They don't want to sit and engage. They have so many breakout rooms and other things to do. They're not going to try and talk about the process. That's they, that's their least favorite thing to do. They don't even want to go to the calls where they talk about the technical things. They're not going to engage with us. 

**Victor**
* And, and then they will have recovery, they lose control of, and then they'll feel bad and then they'll go to random place. 

**Lightclient**
* Just like They don't have control of this repository. I'm trying to provide some sort of viewpoint to you guys about how they feel about the repository and they don't wanna deal with ERCs. 

**Victor**
* I have never blocked a updates in a in, they don't have to, they don't even have to look at or write. But, I don't see, A lot of us have not blocked any blocked any of their edits. 

**Lightclient**
* This is, this is why whenever we added you originate as an ERC editor that I didn't want to like add you as a full editor because then we would have to debate like the merits of doing things at core and comparing them with ERCs. 
* And again, here, like we're just debating about, you're saying that it's okay for core developers and I'm saying as a core developer and as someone who's working with them on a day-to-day basis that it's not okay and now we're in the stalemate and you're going to block the ability to like remove ERCs. 

**Gcolvin**
* I'll block it too. It doesn't solve the problem. It's just, it's a bookkeeping system. It's a filing cabinet. And we're arguing about, well, if we put things in different filing cabinets, it'll solve a problem. It won't solve the problem. 

**Lightclient**
* When is the last time that you utilized the GitHub notifications to interact with the Eth repository? 

**Victor**
* I can use, I use a different way. And then on the other hand, I'm here to provide aspect of their authors. I feel it's not very well represented, even though the majority of the, a vast portion of it is from ERC. And then I do feel that when you, use that comment, I feel a little bit personal. I don't wanna go that go down that route, but I do believe that, there's a lot of value in having people look at, both side of the category as well. And then my argument is that splitting it doesn't solve the problem. just like you. 
* And you are still going to go off and make it very hard in the, in the future for all the new core EIP repo three for, for them to edit and then they'll be unhappy. so that's, that's will be my argument, whether that you believe it or not, I'm not sure. but yeah, that's, that's my opinion. 

**Pooja Ranjan**
* Yeah, I think we are over time we will be probably listening to more from directly from the core devs in the next all core dev meeting. It would be really interesting to hear their thoughts, like what they are trying to introduce as a core EIP process, that is going to help them. If that is something really good, I would, hope that ERC or any other category process should also implement those changes. It would be nice to have changes which are going to make life simple of new authors. If that's okay, we can probably wrap it at this point and we'll, look forward to the decision or suggestions coming up from the all code meeting.
* So I know we had a couple of more items. Those are real quick. one is EIPs insight. I have already added the list of proposals here. We, we received one EIP in, final status and that is, of course E R C category We did receive eight drafts out of those eight. One is core and rest seven are ERC drafts. We have only one proposal in last call with deadline 15th August. The proposal is 6093. For rest of the details, people may refer to the Hack MD or the EIPs insight.com. We did have a EIP editing office hour yesterday. Recording from the past meeting is added. And also the agenda where authors can add their pull request to be discussed in the next meeting if it is not merged before the next one. I have also added the summary from the last meeting, also shared by Samuel on the Eth R&D discord. 
* Please check it out and, yeah, thank you everyone for joining us today.  Hope to see some good reference point, point from the next, meeting to have it discussed in this meeting. Have a good one everyone. Thank you for joining. 

---------

## Date and Time for the next meeting

Jue=ne 28, 2023 at 14:00 UTC

---------
## Attendees

* Pooja Ranjan
* Sam
* Gajinder
* Victor Zhou(@xinbenlv)
* Lightclient
* Justin florentine
* Tim
* Marcus
* Juan Caballero
* Gary Thung

---------
