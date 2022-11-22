# EIPIP Meeting 69 Notes
### Meeting Date/Time: Wednesday, Nov 16, 2022, at 15:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/192)
### [Audio/Video of the meeting](https://youtu.be/az8CYGZL2Ow)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

# Summary <!-- omit in toc -->

## Summary <!-- omit in toc -->
Summary | Description
-|-
69.1 | Update EIP-721: Use latest version of solidity and remove caveats ethereum/EIPs#5887:  **No one wants to accept any more changes to this pull request and is leaning towards closing. We'll talk about it at the next meeting.**
69.2 | Discussion continued from earlier meetings Update EIP-1: **Everyone in the call gave a thumbs up. Ready to Merge**
69.3 | Update EIP-1: Reference ERCs by ERC-X ethereum/EIPs#5273: **To discuss in Discord before merging it Based on the Editor's perspective.**
69.4 | EIP Bot Stale review dismissal loop ethereum/EIPs#5868: **JA will look into it and provide an update.**
69.5 | EIPs Insight - Monthly EIPs status reporting: **i) Six proposals were finalized in the month of November. These are the proposals 5732, 5679, 5528, 5375, 2612, and 5484. ii) We have received 8 drafts and 4 proposals are in the review stage. iii) In the previous call, there were three proposals: 1) 5750 general extensibility for method behavior. 2) A 4519 non-fungible token that is linked to a physical asset. 3) 5757 that is the procedure for approving external resources to be moved to the Final stage.**
69.6 | EIP Editing Office Hour -- **Request you update the pull request in the [Meeting 7](https://github.com/ethereum-cat-herders/EIPIP/issues/194) agenda to discuss in the next office hours.**


## Intro
**Pooja Rajan**
* Welcome to EIPIP meeting 69. We have, agenda and chat. So we have listed a few items, to discuss which are coming from issues and pull request, pull request in which we can make some decision and move forward with decision in terms of merging or not merging. And then we will have, a few other issues related to bot maybe discussed. 

## Update EIP-721: Use latest version of solidity and remove caveats ethereum/EIPs#5887 [1.16](https://youtu.be/az8CYGZL2Ow?t=76)

**Pooja Rajan**
* So maybe we can start with the first item here. That is update EIP-721. the pull request number here is 5887. So this particular item was also discussed yesterday in the EIP editing office hour. It is created by Pandapip one of the editors and I believe Sam also left some comments. We were hoping to get more comments and feedback, to move forward with this. I believe that's what the last comment, Sam,left on this pull request.Wondering if anyone have any thoughts to add here. 

**Zainan Victor Zhou**
* I generally, think that the history  one, including what was adopted or was prior arts were very useful and being left as a record, how that EIP was incorporated and, and finalized removing links, if that's what being talked about,I felt reduces the value of the original documents. 

**Pooja Rajan**
* Okay. 

**Zainan Victor Zhou**
* I kinda, I kind of want to kind of prefer I, keeping it as is cause you can't, like you can have a newer version but I kind of feel that the EIP itself was not meant to be updated over time. we don't do that for EIP-620 and I don't know if that is higher value to do it for 20. So that, that would be my perspective just to avoid touching it if it's finalized and has been widely adopted. Even though I had like for another EIP-112, I have a lot of complaints about how but now that's finalized I wouldn't challenge it much. that would be my position. Yeah. Looking forward to better to other people's thoughts. 

**Pooja Rajan**
* Right. yeah, lately we have been receiving a lot of edits for final EIPs so I wouldn't be surprised if that comes later on with someone. However yeah, if any other people have any thoughts, we are currently discussing pull request number 5887. I have shared link here in the chat. 

**Sam**
* I'm relatively against updating.

**lightclient**
* I'll almost say indifference but lean towards not updating it. 

**Pooja Rajan**
* Okay. So I think one editor has proposed it and we can hear two voices in against and I think Victor is also not very much in favor of changing so maybe we can leave that as a comment over here and yeah, if has for the documents we can have it in the next meeting. 

**lightclient**
* I feel like we should just close it. Like I think we have a lot of people who have already said that don't necessarily think the changes best and there's no reason he can't reopen if he wants to. But I would rather like our default be more towards action rather than in action.Cuz we tend to just like reiterate over arguments many times before something happens. And so if we, whenever there's strong consensus, just enact the consensus I think will spend less time reiterating debates. 

**Pooja Rajan**
* I would love that. I was worried a couple of days ago, by looking into the pull request number of open pull request number, but lately we have been boughted and a number exploded. So yes, as much as we can close for request, that will provide us clarity. 

**Zainan Victor Zhou**
* Very much. 

##  EIP status change
##  EIP-3651: Last Call ethereum/EIPs#5979 Ref: Network Upgrade Process
**Pooja Rajan**
* Thank you. So that's about it.The next item here is, EIP status change. so this is a question that we are receiving generally in EIP editors office. However, and on many other forums like new EIP authors are generally confused about how and when we should move though.
* We try to put more information on EIP one. However, there is one special case that, came into light yesterday.It was about EIP 3651, which is a core proposal. The general understanding is for core proposal we do not exactly follow the process of standardization,though we have,the similar nuances except for we try to sync it with the mainnet upgrade because that is supposed to be updated via, network upgrade.so yeah, if any editor would like to reiterate on the process, about the status change just for clarity and I was wondering if we can have this special case mentioned in EIP one as well. 
* Like I have added the block post that was published by Cat Herders over a year ago in which we mentioned that a core proposal should be moved into last call during the public testnet period, like when it is into the mainnet phase. But that I believe is not clearly mentioned in the EIP one. So yeah, any thoughts And yeah, 

**lightclient**
* I don't think it's necessary to really document too much. Like we're talking on the order of 5 to 8 EIP a year that go through this and most of the authors of those EIPs know and we like just had an instance of the author of 3651 warm Coinbase, try and move his last call and I just mentioned, 
* Hey, we usually only move these last call whenever the test nets are happening just in case there were some that needed to be changed and he was fine with that, close the PR. So I don't think it's something that's necessary to really document beyond that. 

**Pooja Rajan**
* Just to add on on there, I mean I'm really grateful that you left that comment. Just to add on there, this pull request was a reaction to an action that was performed by bot. So the author reached out to me saying that I really do not know when to move to a different status and my, EIP is getting this support comment that it'll be still. And he then went ahead and, created this pull request to change the status. 
* Though I mentioned it to him that this is a special case of core EIP and you should be expecting some something from EIP editors. Thanks to Math. You did mention the same thing, so it made it very clear to him, if we are open for taking it case by case basis, I'm fine by that because as you said that we do not have a big number of, core EIP getting into status change from last call to final or review the last call. So I'm fine. I just wanted to share here. 

**lightclient**
* Sounds good. 

**Zainan Victor Zhou**
* Yeah, I also mentioned there's in the EIP one not, but, briefly talk about the core EIP has different requirement that requires implementations be considered file. So I think that level of valid is enough.  I agree. we don't need add more, but I think that even if it's a new EIP author, I am reading EIP one, they should understand that this is a requirement for cores EIP already documented in EIP one.

**Pooja Rajan**
* Yeah. Okay.And one other point that I wanted to mention, related to this status change only I understand we generally do not have any fixed duration mentioned anywhere except for the last call duration where we specify that the proposal should be there for at least 14 days. while looking into the EIPs for the month of November, it came to my attention that there are a few proposals which moved fast of moving fast is not a bad thing. 
* I just want to highlight that, that, it was observed that there were a few proposals which were into draft a status and is in final a status in less than two months. For some reason, my feeling is like, less than two months could be relatively faster and we may not be providing enough time for community to learn about the proposal and add valuable feedback so that we do not have, iteration of changes post it is finalized. Like when a proposal is done, we want to keep it done. No more changes there. Wonder if there are any thoughts. 

**Sam**
* The ones that I remember going to final very quickly were like single method, yeahs were there, were there more complicated ones that went through quickly or

**Pooja Rajan**
* I can list the number I have it. It's 5732,5679,5750. So these are like, the proposal is started somewhere in September and they are in the 5750 is not on final, it is started on October 15 and it is in last call, which is ending November 19th. So if the author chooses to make a pull request to merge it as final, it will be less than two months. Actually within a month it would be. And similarly for 5679, it started on September 19th and on November 10th it went into the final status. 
* So I feel like it is relatively faster.So if there is any recommendation to keep proposal in review for about a month or so, if there is no rush,like if there is no particularly need to move it faster than that.

**Sam**
* Yeah,we can do that. I don't see a problem with it. 

**lightclient**
* I feel like a way of making that happen most likely. I mean, it's not, I feel like the longer time in review is a trailing indicator of what we really want, but we really want, we want to know that people are reviewing our people are happy with this standard. And so I think like if we make it at the criteria more than just time, because having some time limit to me doesn't necessarily mean whether or not that someone's actually looked at it. And we talked about this in the past, I think that if we just made this requirements for, you know, especially ERCs, a little bit more stringent, like we have this requirement that says before you open a draft,you need to like have, discuss this with the community and it has to, you know, have some sort of support from the community. So if we had that is like part of the draft stage, like to move to review or move from review to last call, like you needs to like show like three independent people who have shared thoughts and are approving of this change.And like,I don't really know the best way to like encode that within the EIP process, but I think having something like that where we put the work onto the community rather than having some arbitrary time limit could be a lot More valuable. 

**Zainan Victor Zhou**
* Yeah, I agree with the Lightclient that, maybe adding arbitrary time period is not the best way. I kind of in favor of, particular way to like, kind of based on the community interest. So one thing that I have been thinking of is that for I offer a lot of EIP, I think ERC should generally also apply similar, standard to get final. for example, like how about having multiple, at least two of the independent implementations to get final? 
* I think it's okay to have something be on dropped and  on review and on last call, but  I kind of generally feel that there's an explosion of the ERC and some of them were kind of really repetitive and hard to prove for debates, the weightiness of them and showing that there's, adoptions or showing their certain limitations just like core could help on one side really start the,further iterations of the specification, right? If you already have adoptions, it's hard for you to any actually make formatic change. 
* But also for clients is their time and energy in,invested into building and implementations shows that, that it's not just support, right? You can easily buy support by pen, hey,on forI support this. But having adoptions shows much better.it's much harder and I kind of want to run this by the editors for us thoughts and making adoptions as a kind, web means for ERC to be final. And I think it can generally apply for any standard track EIPs

**Pooja Rajan**
* One thing I remember discussing with few EIPs authors actually, off ERC category,like having a prototype, even if not fully implementation is ready for a proposal to be a standard, that could be a good place where we can realize, okay, this is being implemented and here the prototype maybe it can be moved towards a standard if that is something you should consider. 

**Zainan Victor Zhou**
* No, I don't think the prototype is sufficient. actually working in deploy a small contract or actually Lightclients, I think should be kind of, I am more leaning towards that level  of clarity because you can easily create prototype that doesn't get tested, doesn't get, like,I'm not sure if s for people who contribute at, editorially would be able to test  just by looking into an asset file of ility. And it's, it's, it takes a lot of other things, for the reference presentation to be kind of, you actually testable. 
* And so seeing a real deployment and a real life one is much stronger, much more solid as they prove of this is being adopted and functional.Well that would be my thought. 

**Sam**
* Yeah, I'm not sure we want adoption as a criteria for publishing an EIP as final. I worry that that would kind of stop people who may not be technically minded,or as technically minded from writing an EIP and I think the process should be open to as many people as possible. That said, I think, maybe the approach that I'd prefer is, actually having a, like resource list that we can send to authors and say like, oh, you're writing a so bound token nft, here are 10 people who deal with so bound token NFTs, who you should talk to about your EIP. 
* And I think that like that and then some kind of ensuring that we have a reasonable amount of discussion on the discussion thread would be sufficient. I just think that an actual implementation or even a reference implementation is, is making it like too onerous for EIP authors. 

**Pooja Rajan**
* That's a fair point. Maybe, obviously we can leave it at the discussion of editors, so like when they would like to move, but having a fair discussion in discussion to thread and some implementation could be right set of information that we can pass along to new authors when they're preparing to move their proposal into different status. 

**Zainan Victor Zhou**
* So Sam, I, if I heard hear correctly, you referring to like, you, you don't think you wanna require it by how out said that it's recommended? I am.I hear you and then I totally agree with you that with me, to let as many people contribute to the idea as possible. And that's one of the reason I really want to be flexible on linking links. I do feel that, there's some way to show strong community support if there's any way to show strong, community support, adoptions would be a good one.
* Like I, we can say, Hey, how about us can be adopted, can be seen as community support,but if you happen also have multiple implementations, that's definitely help that, that definitely helpful.so make it an optional suggestions. Would that be, would you be open to that type of 

**Sam**
* I think that's where we are today, right?So yeah, Agree. 

**Zainan Victor Zhou**
* Don't think we, we mentioned that.Yeah, I don't think we, I think that you can put reference, but we don't say it's recommended to be light. it's recommended to even under some reference policy, that you were advocating, if I understand correctly, people should actually remove them, remove the of adoptions. I think we can, we can put that into context when we talk about 1191, I put agenda, and I think that can be test policy discussion can be tested in real reviewing. 

##  EIP-1191 was in last call since 2019. Should we move EIP-1191 to FINAL or STAGNANT? [21.13](https://youtu.be/az8CYGZL2Ow?t=1273)
**Pooja Rajan**
* Right. And I think that is the next, item listed here about EIP 1191. Victor, which, I believe this was added by you,if you would like to provide some context here. 

**Zainan Victor Zhou**
* Yeah. So this  EIP 1191 has been moved to last call since I think 2019. it states with minimum change for a minimum nomadic change. and there's a big list of adoption table, which makes me feel, this wouldn't, there would not be much change,  in the future as well. But staying in last call for multiple years, I think undermines our sense as a community for what last call means. so I kind of pose this question to editors. Should we move it to final or should we move to stagnant? 
* I lean towards moving to final, but there's a strong push, from Ethers author, we chat more, more. so kind of like to get a gouge of thoughts about you, like how, what direction we go here and what the policy thinking process. 

**Sam**
* I think it's like our policy is that if an author wants to open PR and push it through, they can, otherwise we don't touch it, right? 

**Pooja Rajan**
* So just to add some more context here, this proposal, was also under discussion about, about, 6 months ago. And, that point also, we were stuck at a place where author, where are the Ether GS author requested some changes and the proposal author is, not willing to maybe comply with that or,is there only, so the other option is if author wants to maybe withdraw the proposal or someone else wants to come up with a competitive proposal with whatever changes they are suggesting, like I believe it is a note on backward compatibility. 
* So if they would do either the proposal will be moved forward, otherwise bot will definitely move it into stagnent status if nothing happens there for a longer time. 

**Zainan Victor Zhou**
* I do know that, if untouched for six months thought we'll do that. I think my question is, given the current status that some of the community has stopped some of the community being towards and siteing backward compatibility, are they a Eth author once, are they allowed to move this final given this current status? So, sorry, am I?

**Pooja Rajan**
* Oh no, I think, we can hear you. Yes. I think, we will differ there on EIP editors, decision. And it looks like the decision is if there is no request by the author, yeah, to move it to the final and unless all the issues mentioned in the discussion thread are addressed, it should not be moved into the final is if I'm reading correct. 

**Sam**
* Well, like, I don't think we'll stop it from moving to final, if the author wants to move it to final, but like there are a lot of concerns and either like somebody should open an EIP that addresses them at some point.But yeah,

**Pooja Rajan**
* I am not sure if this is the resolution we were hoping to get for this particular item, Victor. But yeah, if you have anything more to add or no

**Zainan Victor Zhou**
* Yeah, I agree.I lean towards that author allow to move it to final. I do also agree that if they can also resolve any concern that would be better. But, my stance, personal opinion here is that once they get large number of adoptions, that the is powerful enough to that EIP generates powerfully enough community consensus and it should be warned,to Yep. 

**Pooja Rajan**
* I think at this point we are leaving it to the author if, the author is willing to maybe make up a pull-request and then we can bring it back to discussion or see where we are at that time. If we, if pull request and the proposal is supported by more adoption, probably there would be cases of getting it merged too far.

## Discussion continued from earlier meetings Update EIP-1: Clarify when to use requires ethereum/EIPs#5614 [27.16](https://youtu.be/az8CYGZL2Ow?t=1636)
**Pooja Rajan**
* All right, moving ahead, we thank you Moving ahead, we have item number two, which is discussion continued from earlier meeting. First one is, EIP one, clarify when to use request. I think we discussed this and Sam Vincent opened a pull request for that. So I believe this is to decide on merging. the pull request number is 5614. Any thoughts, comments or 

**Sam**
* Maybe I mean if it hasn't been merged at this point, I'm, I'm okay with just closing this. I mean we, we have two approvals and, and Victor as well. I don't think anybody's opposed. I'll merge it unless somebody objects right now. 

**Pooja Rajan**
* I think it has received a fair approval here. Cool. And receive comment from Greg also, but it does not seem to be in negative direction, so it should be fine. 

**Sam**
* Yeah. Okay. I'll just merge this then. 

**Pooja Rajan**
* And the other one also, we have already discussed this and I believe, the EIP W bot, sorry, EIP W bot has also been, updated according to it. The pull request number is 5273. Matt, I believe this issue was brought up by you, you have to add anything. I mean this, since we were in agreement, like the majority were in agreement, I am still against it, but majority were in agreement. So yeah,let's go ahead with that. 

**lightclient**
* Yeah, I just wanna press the green button and so I was gonna make sure that that was ok. I'm still against merging it, But I can press the green button. 

**Sam**
* I mean, you have that privilege on Github, Yes. 

**Pooja Rajan**
* It's a good thing. I don't have any privilege on that side. 

**Zainan Victor Zhou**
* I mean, right now basically Pandapip and I are the only people who are pro. You and Sam, 

**Pooja Rajan**
* I think Sam also yes. 

**Zainan Victor Zhou**
* No, Pandapip and I are pro Sam is against, Okay. 

**Pooja Rajan**
* Yeah,Sorry. 

**lightclient**
* But panda PIP is like marginally pro. 

**Zainan Victor Zhou**
* I guess the question is whether Sam are against it to the level that Sam wanted to block it or Sam is just weekly. 

**Sam**
* Oh no,I keep saying I'm opposed because I like, no offense to you guys,I think it's a dumb idea and I don't think we should do this The problem is that this is already the way that everybody does it. 

**lightclient**
* And we are just like, every week I see another person ask why, why is this the case? And this week it's the guy who's working on the warm coinbase,he says,I'm trying to move my EIP last call. Why is it getting mad at me saying I have to refer to ERC 20 as EIP 20. Like, I'm really tired of seeing all these authors confused and the community getting confused. 

**Sam**
* If we flip it, we're gonna have authors confuse the other way. 

**lightclient**
* Like We won't, we will not to all the authors understand that we refer to ERCs is ERCs. I would like to add, I've Never one time seen an author confused by why do I have to call this an ERC? 

**Sam**
* Every author understands this, but I consistently, Because we've never had a rule that enforces calling an ERC is ERC, like there's, there's never been a place where an author would be confused by that. Like when we add the EW implementation that forces ERC, then we're gonna start to see authors confuse the other way. 

**lightclient**
* I'm almost certainly won't because I've almost never seen an ERC referred to as EIP in the like broader context of EIPs, anytime you see an ERC discussed on another form or thread is always ERC except for this more recent time where EIP W has been enforcing EIP. 

**Zainan Victor Zhou**
* I witness, 

**Pooja Rajan**
* I would like to add a small here, people who are referring ERC as ERC, they're generally people who are here in the ecosystem for very long time. And that time ERC was having a special case. Like okay, they were not considered to be, I don't know, people did not even consider it to be a part of EIP standardization, but we spent a decent amount of time in making this thing. And the good news that I want to share here is new authors who are documenting EIP off ERC category, they generally do not have this kind of hesitation and they have a better understanding. 
* Like if we want to document,EIP and ERC category, they have, it has to follow the EIP standardization process because it is a standard track EIP off ERC category. So that, yeah,that is there with the older authors, but obviously we do not want to lose them. They have been a in great contract. 

**lightclient**
* It's Not just with the older authors though. I mean it's with all of the ERC EIP up until 4000, like we're not going to get away from this. There's too much, too many ERC references out there. We can't just change it in the middle of flight. Now even if you're a new, you know, ERC author coming in and you're like naming your things EIP, you still have to like live in this world where all the implementation called ERC 20, all of the references called ERC 21, like no one is calling these things. 

**Zainan Victor Zhou**
* EIP 721 I kind want to see is I agree with, Matt and I kind of want to test with you whether we, we on one principle that, we lean voice call things that is being adopted. 
* Is that a principle that we can, that that we, we agree on or we, we don't, we disagree on this proposed principle, Did catch what the principal was.The principle is that we call ERC or EIP based on what people call it. If we ignore, if we don't care what outside people call about it, then I,like Matt and I, we we agree on we want call EIP.But if we don't, agree on that principle at all, then we don't make a case. But if we, if as in this venue,everyone agrees that, we should call you or ERC based on what people call them,then the next debate is what do people call them? 
* I think we already jumped into the next debate,but we wanna test out whether the first one is actually, the principle is actually,agreed upon by the group. 

**lightclient**
* I mean, if we had a time machine to go back six or seven years, and we could avoid this scenario, we're calling something ERC something EIP probably be great. We don't, and we have to live in the world that we do. And I don't think that we could be trying to erase

**Sam**
* The I mean, how like to, to borrow one of Micah's old arguments, how, how long do you expect Ethereum to last? 

**Zainan Victor Zhou**
* Whatever. that's what I think is like Internet. 

**Sam**
* So the small amount of time that we called them ERC versus EIPs is insignificant and they're very, very long term. So we should probably try to correct the naming now. What was still early? 

**Zainan Victor Zhou**
* That sounds convincing 

**Sam**
* Like it's pretty marginal to me the fact that the community calls it ERC and there's just no, They also c phrases when they own board apes into random websites. Like I, we can't use the community as an indicator of like quality decisions. 

**lightclient**
* Yeah. But we also shouldn't just like pick invasive policy just because we think it's like marginally better. Like if there was, you know, substantial improvement of calling it like this,like the naming change of Eth 2 to the consensus layer and stuff I felt like was a big and important change.And it's a good thing that we did it, but we seeing people who call it EIP rather than ERCs,that's like much less necessary. 

**Sam**
* Yeah, I mean the benefits are mostly just for consistency and like internally within the EIP repository, right? Like we don't name the files ERC 20, we don't, like, we don't do any of that stuff. 

**lightclient**
* Like, I mean, I think that we could do better about creating consistency in the EIP repository by naming it ERC and like working towards that. But right now we're just like upsetting people, Everyone. 

**Sam**
* Oh, okay. So like the consensus or the execution specs are coming along and you know, they're going to be a thing that might be the best time to revisit this discussion because we're gonna be changing everything anyways. 
* So if we do it all at once and we fix the naming,we pick whatever system we want because that, like once we have the execution layer specifications, then there's a very clear difference between ERC and an Eip. And I'm totally fine at that point, calling them ERC. 
* I thought that today is still very clear distinctions. 
* I mean, we followed the same process for both of them. So they're, they're not really that distinct. The only difference is whether you cite one as EIP or as ERC. 

**Zainan Victor Zhou**
* The one the, the route to finalize is different as well, right? 

**Sam**
* Like you need adoptions for, from Have you heard about wireless headphones? 

**lightclient**
* Yeah. Sorry, I'm like losing connection a little bit. 

**Sam**
* Oh, Is that you? I thought I thought that was Victor. What, what have you talked for a second? 

**Zainan Victor Zhou**
* Hello? I also have a crappy, my, my AirPod just very badly. Let me use another. 

**Sam**
* It's not important. It's just every once in a while, like we get a burst of static from someone's smoking And then mine is just like having trouble protect the internet. Oh, Okay. Yeah. So no, not a huge deal. It's just wanted to mention it. 

**lightclient**
* Sorry I missed the last 30 seconds of what you were saying there. Unfortunately. 

**Sam**
* No, no. Nobody said anything. It wasn't you Okay. 

**Pooja Rajan**
* I just will respond to one Vic, one comment from Victor.Generally we speaking at the process of the standardization, is it not very different? We are also looking for implementation for even core proposal,though this implementation is going via a client team. 
* And similarly the expectation is with the ERC also, there should be some kind of implementation or adoption there.So maybe,like in real life, there could be a little bit of difference.The process of a standardization remains the same.And that is not only for this ERC category that is for any other standard track EIP. 

**lightclient**
* I just don't like this thing where we as editors, like make decisions about things and then the community says they don't like that and then we just do it anyways. Like, it just feels, it, it's doesn't feel like we're working with the community to build a good together. 

**Victor Zhou**
* I feel very much the same. I lean towards, using adoptions as a indicator in many places. And then this is one that because, the community has started the ERC names and it's going to be even known better in the future. I felt that, at least  we should consider that a factor into our decisions. 

**lightclient**
* I mean, I would love to just move ERCs farther and farther away from EIP. And honestly, I am like getting tired of waiting. Like, I don't know when that's gonna happen, but I would love to do it more. But I think that like we're just seeing over and over again that people are confused with this. We have ERCs in the wild and now we're like, you know, telling them in an automated way that that's wrong. 

**Sam**
* All right. I will get I will, you know, withdraw my block. but let's have a discussion on discord about it and let's get everybody accept, Cuz I think even Greg might have an opinion on it. And then as long as if I'm the only one that's holding up the process, then we'll, we'll make the change. Okay, That sounds amazing. 

**Pooja Rajan**
* Victor. If you were trying to say something, your voice went robotic, we could not catch what you said. It's no better. So maybe you can type it. So, I will ultimately def it to light client. Do we really want to press a green button right here or continue discussing on this, discord Discuss on this court and wants to hear everyone's opinion. 

**Sam**
* I just don't like if I'm the only one against it, I don't want to be, you know, the person blocking it, but I also wanna make sure that everybody else has a say. 

**lightclient**
* Yep. Sounds good. 

**Pooja Rajan**
* I think, the voice of editors count here and that's why my voice is not counting here. But yeah, I'm also against of it. And one point I also want to mention your, for coming back on this topic again and again, Matt. but here's the thing, like when we decide something for core proposals, there is a lot of things that is coming up for community, but I believe that as a client, developers and people who are in the All Core Dev Meeting, they take this responsibility, they own this responsibility to communicate it to the community. 
* Like what is the right thing to do? Just like you mentioned about in the case of Eth2. Similarly, if on the ERC side,if the EIP editors are trying to make a decision on that, I think it is on them to own this responsibility of communicating the right thing to the community. So I don't think we should be feeling bad about making decisions in the EIP meeting. This is open, people can join and share their thoughts. Yeah, but let's continue discussing this and not the discord side. Right. 


## EIP Bot 
## Stale review dismissal loop ethereum/EIPs#5868 [43.21](https://youtu.be/az8CYGZL2Ow?t=2601)
* The next one is EIP bot. I believe this is an issue created by Matt, for Stale review dismissal .If someone would like to provide an overview of the issue and maybe

**lightclient**
* Yeah, I mean, I'm just on discussion to not have the blog post a bunch of meaningless comments on the Yeah, because there's nothing worse than opening EIP thread. There's like 30, 40 comments, but they're all just like opening, closing the PR stale reviews bugs in the bot, whatever. And this seems to be a Github. Panda says that this is just due to GitHub. I don't know, maybe it's true. It's just annoying to like, I don't know why or how it happens, but for some reason, like you leave a review and the bot will just dismiss it sometimes. 
* Or if someone else's review, they'll just miss your review and it doesn't look very nice on the, the but kinda not here. So I don't think it's anything to discuss on Sam understands Situation. 

**Sam**
* My knowledge ends at the command line interface for EIP

**Pooja Rajan**
* So sorry, I wonder  JAif you have any thoughts on that. I'm not sure if you're completely familiar with the code, which is working behind the scene here, but since you have been looking into the repository, if you may have any thoughts or if you would be willing to maybe look into this issue. 

**JA**
* Yes, thank you. Indeed. I think that we can set a kind of filter. I will take a look on it. I don't think that  we can avoid it, but I think that we can avoid the, the posting, which I believe what is annoying is all that least. And an action of stale review is me or whatever. So I wanna take a look. I feel positive that we can set the kind of filter on that, on that action. 

**Pooja Rajan**
* Sounds good. so maybe you can update it on the issue created the Matt 5868 is the issue number. So if you have any finding you can probably add here, that would be good. Any other thing on EIP bot side that you would like to share or mention today? 

**JA**
* Indeed I choose three more issues to collaborate. I gonna share in the, repo so the can see they're working on it on then or not.

## EIPs Insight - Monthly EIPs status reporting. [46.16](https://youtu.be/az8CYGZL2Ow?t=2774)
**Pooja Rajan**
* Thank you for that. the next one here is EIPs insight for the month of November. I have not added the formal hackmd over here, but I was trying to collect the information with the new EIPs insight.com website that we are working towards it. And we do have a tab of, the latest month, from that, report, I can say that we have six proposals, which reached to final status in the month of November. 
* Those proposals are 5732 5679 5528 5375 2612 5484. So it's kind of good progress that we have so many proposals moving into final. 
* That means they are not waiting in the pull request form for a longer period to be moved to forward. We do have received, 8 drafts and, there are 4 proposals in review status. There are 3 proposals in last call. one is 5750, general extensibility for methods behavior, 4519 non fungible token tied to physical asset. And the last one is 5757. That is process for approving external resources. 
So, Matt, I was wondering like we have this proposal in last call, do we want to move it to final or do we want to live it with the status of living? What is the next step here?

**LightCclient**
* I would like to move it to final. 

**Sam**
* Which ones? 

**Pooja Rajan** 
* The process for approving. Oh, okay. External resources. So we want to have it as a final,not a living. Yeah,I think it's final. Fair enough, fair enough. So yeah, these are the three proposals on, last call. So people, if you have thought comments come forward and share it either on the discussion to thread or on the respective pull request. 
* Better on discussion thread. We don't want to create any confusion. Okay. that's all EIP insights.


## EIP Editing Office Hour [48.30](https://youtu.be/az8CYGZL2Ow?t=2910)
**Pooja Rajan** 
* The next, next item here is EIP editing office hour.Yesterday we had editing office hour meeting number six. Recording is updated on Ethereum Cat Herders YouTube, and this has been going great.I have receiving a lot of positive feedbacks. Thanks, Samuelson for having this meeting.It has helped a lot of new authors, to understand how they can move forward and, people,if you have any, questions or any pull requests and anything that you would like to, check with editors.
* I believe this is the best meeting where you can have one to one interaction. So yeah, agenda for meeting number seven is already added. You can also, leave your pull request number in the agenda so we can include it in the next meeting's discussion. That's all I think. And now we are at the last item, 


## Review action items from earlier meetings
**Pooja Rajan** 
* Which is a review action item from the earlier meeting. And, okay, so there is one action item for Sam.I think he already have worked towards it. It is related to EIP 5757,which is,now in the last call.So that is taken care of and we have revisited issues which we are pending from the last discussion.I think that's all from the items added to the agenda for today's discussion.we have approximately five to seven minutes if anyone has anything to share, discuss.Yeah, please. 

**Sam**
* I think the only other one then that we should discuss is 5874. So that's 5874. That's the two external origins. I think we just need to come up with a, I think I just need to come up with a way to, add the json to a footnote. see if anybody has any suggestions on how to do that, please add it to that PR and then, as long as don't be objects,we can merge it. 

**Zainan Victor Zhou**
* Same,I wonder,it seems like, these, json are very highly structural.I wonder if it's better to be in a separate file as structural or is that intended,

**Sam**
* Like you would have a citations file or something in your assets directory? 

**Zainan Victor Zhou**
* Not necessarily.I thought that the CSL dash Jason file was meant to be used in a EIP W as a way to allow, Citations. 

**Sam**
* Yeah, yeah, yeah. 

**Zainan Victor Zhou**
* And in that way I'm kind of think that,running by, I don't have a strong preference, but, I felt Mark in markdown it's very hard to test whether a structural data is legit and has, been validated. So I wonder what's your thought on making that separate file? Like, ok hson, Like from the, 

**Sam**
* From the validation point of view, it's not a problem. Like Eth W can just grab that block and, and validate it, but, from like a human readable perspective, I can definitely understand wanting to put it into another file. but that would require more work on the other side to get it to render correctly. but maybe that's worth it. 
* I don't know. because like what I have, like, so the, the concern panda PIP has here is that the indented code block that I'm using, doesn't render correctly in common mark. 
* So, that's a problem. So I have to just figure out, yeah, putting in a different file is probably a reasonable solution. I hadn't really even thought of that. 

**Zainan Victor Zhou**
* Cool. 

**Pooja Rajan**
* Okay.so if this is resolved before the next meeting, it's fine. I mean, if it is merge or not. so if we want to bring it up in the next meeting,considering it is still open, we can probably add it to the agenda there. 

**Sam**
* Okay. 

**Zainan Victor Zhou**
* And I also mentioned that I wanna propose, a few other things into this, into our first,accepted,external origins such as if you're in ethereum-dev POP. do you have a thought on adding those? Like I'm hoping this is probably the easiest time to get,origins in, so yeah. 

**Sam**
* Yeah, So I think, just, just because I didn't separate the, like, my PR into like, two parts,like one about the, the rules text and one to add the, the actual origins. So if you can make a PR after this one gets merged, I'd appreciate it. But, if you also wanna make one before and just copy the same like  Eth introduction text, that'd be fine. 

**Zainan Victor Zhou**
* I'm, I love to I don't know where to put that particular file. So yeah, once you need to merge this one or you create a separate PR I'm going to add the, all the list I want to be allows listed to begin with. 

**Sam**
* Okay. Perfect. Yeah. 

**Pooja Rajan**
* Good. Thank you. So I believe that concludes and that is the time we have for today's discussion.Thank you everyone for joining us today.I hope to see you in two weeks. 

