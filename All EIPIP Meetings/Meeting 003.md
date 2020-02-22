# EIP Improvement Process Call #3 Notes

### Meeting Date/Time: Wednesday, 12 February 2020 at 15:00 UTC
### Meeting Duration: 1 hr 
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=XpEu8MyPRcc&feature=youtu.be)
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/5)
### Moderator: James Hancock
### Notes: Pooja Ranjan


----
	
# Summary

### Action Items

* James Hancock will follow up with Hudson Jameson on who in the EF would have the Technical Resources to make changes to the Bots for the proposal discussed in the EIPIP meeting #2
* Tim B. to create a PR to replace the 'Ethereum hardfork' with 'Ethereum network upgrade' in EIP1.
* James H. to split the current PR in two - (i) formatting, adding the list of upgrades and merge with Tim's PR and (ii) rest of the content of current PR plus suggestion for a better definition of network upgrades, contentious network upgrades, roadmap upgrade, hotfix upgrade.
* Create a guide for EIP champions, setting expectations in continuation to mentor program that was discussed in the EIPIP meeting #1. 
* Things to reconvene on - Upgrade terminology
* We can take this existing code of conduct available on ECH repo and just change the scope of the impact. Continue the discussion in the next meeting.


----


**James**: Welcome to the third EIPIP meeting. These meetings are every other Wednesday discussing progress we can make to the EIP process. Thank you all for joining today.

We have a couple of things on the agenda. I'll just go over the agenda first. 
1. I made a PR on EIP1 that has some consolidate information. 
2. Flushing out requirements for EIP is related to when something requires a little more work than a normal or the typically EIP that is seen and how we can communicate that effectively.
3. Code of conduct 
4. Process documentation. I am not sure which that one means. Is that one that you added Pooja?

**Pooja**: Yes, if we get time to discuss it, I will shed more light on it.

**James**: OK 

5. Progress on the EIP repo clean up 

6. Any other business and 

7. the next call

Is there anything else out there that would like to be brought to the agenda?

**Tim**: I don't know if this is encompassed in any of the points but this proposal you had a call or two ago around like that sort of DMV office file section on the EIP. I am just curious to know the update on that. Because I don't think the first PR on EIP 1 that you made does cover it.

**James**: It doesn't, but I can give an update on it. I still need to get someone to look at what it would take to change the bot to make it possible and otherwise I heard that it's a good idea. It's a matter of how do we do it in an effective way and implement it technically. It still is like  I can own thing and I didn't follow up with Hudson about who in the EF would have the Technical Resources to make changes to the Bots. Yeah we should take that as an outstanding item to follow up on.

**Tim**: Sounds good.



# 1. [PR](https://github.com/ethereum/EIPs/pull/2508/commits/c56e992586b027e45bca0770b545f3407a838a00) made to EIP 1

**James**: On EIP 1, I don't know if you have had a chance to look at it. I'm on my mobile so don't have an easy way to get to the chat, can someone do that?

**Pooja**: Yeah, I will share that, it's there. 

**James**: Tim and I've gone back and forth a little bit on it.

**Pooja**: I was looking into it and I had a couple of questions there. I'm not sure if this is the appropriate time to discuss it because I was there in the previous call when we discussed it. At that time it did not come to my mind, so I'm just sharing it. 
I like the response of Tim about the usage of 'upgrade' instead of 'hard forks'. In my mind, I was thinking that since we are making changes to EIP1, will it be a good idea to update that as well? 
I see it in your PR, line number 291 / 324 in the [link](https://github.com/ethereum/EIPs/pull/2508/commits/c56e992586b027e45bca0770b545f3407a838a00) that I have shared. There we are writing Ethereum hard forks and updating at what block number.  Can we go ahead and update it over there, instead of Ethereum hardforks' make it 'Ethereum upgrades'? So that would maybe solve future confusion. Any thoughts?

**Tim**: This is a controversial topic. People have strong feelings on that. I almost wonder if this may be a separate PR? Basically takes everything in the EIP 1 right now, switch hard forks with network upgrades, see what people feel about that.

**Pooja**: Yeah, I like the idea. It will give more visibility to what change we are proposing and will get more feedback on it. So, yeah I like the idea.

**Tim**: Yeah!

**Pooja**: The other thing, in the PR you (James) mentioned that we are referring to more on EIP 233 and EIP 2378. Both of these EIP seem to be in the status of 'draft'; so is it the right time to add it into the EIP 1? I mean like when it is not fully accepted? Should we first moved towards making them be accepted first and then work on this PR to be updated in EIP1? What is the general thought over here?

**James**: I thought about it the other way, as when I was talking with Alex B., he wanted the governance information about the process to be in EIP 1 not in the EIP. We moved it to the draft so that people could link to it and it was easy to use, but he would have rather had it not have that information. My compromise was to make it to draft and then when EIP1 is updated then we can remove all of the things that don't need and make it file as just a registry.

**Pooja**: There are a couple of things associated with it. I remember sometimes back the discussion of not having major changes to EIP1 but to the separate EIP. The way we are following, like EIP 233 that defines basically the process of how to create a meta EIP for an upgrade. EIP 2378, at this point in time that describes the core EIP eligible for inclusion. But, I'm not sure about the process that we are going to follow all along. About a year from now we were working for Istanbul and we were considering the model of flight/bus/train, that was an experiment that we were trying to perform for that upgrade. I consider this EIP 2378 again a similar thing. Like this is another experiment with the EIP Centric model and EFI is just an intermediary for this EIP Centric model. So I'm not sure that if this is the right time to include it in EIP1 when we are, I don't know certain are not certain to follow this in the future upgrade. So, I was just wondering like should we keep it separate, for some time, till we decide that we are not going to follow the flight/bus/train model and  we're going to follow the EIP centric model or if something else is proposed in future, so keeping it separate so that EIP 1 is not to be updated again and again, and whatever hardfork process or upgrade process we are going to follow should be kept separately. That was just my general thought process around it, open to discussion.

**James**: Yeah. I have some thoughts but I don't want to dominate the discussion.

**Tim**: The challenge with like having two resources, I get your point Pooja and I agree like EIP1 so far was very conservative in terms of upgrades. The process will change a lot if it wouldn't have changed for a long time that EIP 1 reflects it. So now it's like if we change it then you get to a spot where EIP 1 is suggesting something that is in kind of in-flight. On the other hand, the challenge you get is then it's hard to point people towards the process.
So if it's like we need to point to EIP 2378, it's like how does anyone ever like find that EIP? That's just my concern there, it's like your trade it off like stability vs. like making it accessible to the community.

**Pooja**: I get that part. Because of that, I put one agenda item about the documentation of the process. So if you do not want to do it right now it's fine when we get back to the documentation process then I will bring it again. 
I'm fine with the PR that he (James) made and these were just a couple of concerns:
1. change of terminology - Ethereum hardfork to upgrade. To which Tim proposed that we should have a separate EIP altogether.
2. EIP 233 and 2378 should be converted to accept, because they are still in draft right now. 
Those were my two points here.

**James**: Yeah, in one sense it's in flight. It was in Flight, it was much more in flight when we were discussing whether or not we wanted to try out the EFI model. But then when we had the core devs call and everyone had a consensus for us to try it, I feel like the EIP 1 representing the current consensus of the core devs and then if we need to update it a lot, then cool. People will always know to go to EIP 1. Again another problem would be if we tell everyone to go look at EIP 2378. As soon as the process changes and there is another PR then that like knowledge link is broken and all the people who would go there would go get old information. This goes back to my thought of the proposal, the last call is having one single source of truth for everyone in the community about what is the core devs and what is everything? Like I just was thinking when I was writing out the definition of the hard forks and stuff but there isn't really a place for people to reference to say yeah this is how the core devs are thinking this, it just sort of amorphous everywhere. it just would be nice to get all that documented.

**Pooja**: Yeah, I believe that documentation would help a lot. About a year back I tried that in EIP 1929 which is still again in the draft which was shelved because we were doing some experiments then. I think that this may be the right time to create the documentation about what process All Core Devs are following. Every time it's with the devs  only and it's not documented because we are still in the experimentation phase and have not set something in stone yet. I would recommend to leave it here only and pick up after a couple of weeks and see if we have different thoughts and how would we want to go ahead with it.

**James**: That sounds great. I like to read the ones that you once mentioned in your proposal that are later on the agenda. Because I still have to get my head around the context around it. Any other thoughts on the EIP1?

**Tim**: I have a small PR about the Hardfork network upgrade thing. I just looked in and the hard fork is only mentioned twice in the EIP 1, as it is, so it's a very small change.

**Pooja**: Thank you Tim!

**James**: Great, when I was writing out that section if we call it upgrade then what do we do about the Dow hardfork and where do we put it?

**Tim**: The way I think about it mentally is like the Dow hardfork was a Network upgrade that led to a hardfork. To me a hardfork is a possible outcome of an upgrade, right? The Dow, the EIP implementation is still an upgraded. There was a conversation about if upgrade is the right word, I still feel pretty strongly about that just because the person who is kind of arguing against it was saying upgrade is better but I don't really think that's true I think it's true, I think it's new. The Mac Catalina upgrade is a great example of it, it's new but people don't like it and don't want to upgrade to it. I was saying, we had an upgrade which led to a hard fork or a network split or whatever but all the nodes that are still on the Ethereum chain today did upgrade. So it's just one of the network upgrades but it led to a fork, this is how I would see it. I don't know what everybody else thinks?

**Pooja**: I agree, in fact, I find it more of a reason to use the word 'upgrade', because we had only one hardfork, which was actually an upgrade but that led into a fork. 

**Tim**: There are controversial dynamics around it, that there are hardfork for a fact that there wasn't really a hardfork for a week and then some Exchange started trading ETC and that kind of revived it. So, I am still in favor of calling it a network upgrade.

**Louis**: You're talking about coding the DAO fork as an upgrade?

**Tim**: Yeah, it's basically, the EIP that was patched there was the upgrade and the fork is the process by which the nodes that are still running ETC did not run the upgrade. So, the way I see to it is the **upgrade leads to the fork, you need to have the upgrade to get to the fork**.   

**Louis**: It's linguistic, but I will accept it.

**Tim**: That part is very tricky, but if you put the Dow hardfork aside,  I think everything else can be called the network upgrade, right? The problem with hardfork, I find as it's kind of a loaded term because of Bitcoin. So Bitcoin has this whole thing around like they can't do hardfork, it's like a terrible thing. But Ethereum has done that ever since the beginning. And this was just one upgrade that went pretty bad or good, depending on what you think.

**Louis**: Tim you will be a very good politician, but I agree with you. The current terminology, except the DAO, rest are fairly upgrade. You can definitely argue that the upgrade does not have to be positive, it has to be a modification. 

**Tim**: I think, it's important to state that because I still think it's a really important feature of these upgrades that's like they're not certain to happen and that kind of puts the responsibility on core developers that not put stuff that's like too controversial and not split the network and that is like a really important concern. But also think about that highlight the fact that like Ethereum has this culture where these changes will happen. I think it's kind of moving away from the terminology that Bitcoin uses is good in this regard. But I can see it also as a controversial opinion.

**Louis**: To be honest we are going to get drag by a few crypto bitcoiner twitter doing their jokes and they are trolling and once they are going to get over this and it will be done. To be honest, in my opinion, it is always the upgrades and hardfork is poorly chosen name especially when we think of the people from the older chain like Bitcoin hardfork like Bitcoin cash.

**Tim**:  Yes and that's something I think is likes even more important for Ethereum is like not having that perception for a couple of reasons like 
A. because of the whole, that's how classic started 
B. because it just creates confusion for current users and
C. because of Ethereum 2.0 
Like you don't want to create this perception that like every upgrade is like free coins and has the risk of having two different types of coins. 

**Louis**: I agree. In that case, for the terminology, we can find DOW upgrade as a contentious upgrade which leads to a hard Fork and something that is more understandable for everyday users.

**Tim**: I think that is a really good way to put it. **These are network upgrades, the DAO was a contentious upgrade, which leads to a hardfork, therefore, we want to avoid contentious upgrades because they have a pretty significant toll on the network.** 

**Brent**: That's brilliant!

**James**: As you're saying that I'm realizing it as it would fit as its own section really well and something that just described exactly what you said. And then people can reference that is the definition of when people are yelling about it on Twitter.

**Tim**: Another thing I feel very strongly about is I don't think we should always weigh ETC thoughts on what Ethereum does. I'm sure ETC will not be happy with that definition. but I think we should try to focus on what's best for Ethereum. If ETC wants to say oh we are the original chain... blah blah blah.. that's fine. The ETC repo can say whatever they want.

**Louis**: Yeah, we don't have to compete, we're different.

**James**: I agree. 

**Pooja**: I'd just recommend that whatever we're discussing in the EIP IP and creating PR and everything, whatever is our summary and the action item of this meeting, we share it with the all core dev meetings. So that they don't think that we have started making decisions on my own.

**Tim**: Yeah, for sure. and any change to EIP 1 will need to get approved by people and that's going to be like quite a process. I guess as an action item for this, I don't know James do you want to take a stab at like rewriting some of these as a part of your PR. I feel like your PR is a really good start for all this stuff. Do you think that makes sense? I am happy to help however I can.

**James**: I think it would be removing the parts that I had done that are relevant in and adding language that you did to yours somewhere else so they can be evaluated separately.

**Tim**: I've my tiny PR that is like two-word changes to go for 'Network upgrades', see if that's controversial. Maybe you can **split your PR in two**, where one of this is just basically formatting, adding the list of upgrades in the table of contents and the other part that I did, like a bunch of definitions. Maybe we get the table of content merged to my small hard Fork the network upgrades merge and then once those two are done, you basically haven't changed the EIP 1 much. Then we take the rest of the content of your current PR and push that suggestion for a better definition of Network upgrades Vs. hardfork and what not.

**James**: I like it, so there are network upgrades, contentious network upgrades, this is just so that I can get all my thoughts out into one place. The other kind is like emergency of addressing something critical on the network. 

**Tim**: These are like emergency upgrades. Emergency is kind of alarming, but is kind of the case. Because, they are also upgrades like they literally the same thing but it's just the time component that changes.

**James**: Yeah and then they do feel sort of different then the normal.  So there's the **contentious upgrade** if we just say **upgrade** like the normal it's Istanbul and whatever then there are contentious upgrades which is the DAO fork, the odd man out is the is the ones that when they're facing attacks, were happening. 

**Danno**: Spurious Dragon, those are called **emergency**, maybe we call Muir Glacier a **priority**. 

**James**: Yeah, I don't know, I guess I am not saying let's figure out exactly what it is but finding where that fits, in the narrative, I think then it's completely full. I got up a complete concept.

**Danno**: Roadmap upgrades and another one, not roadmap upgrades. 

**Tim**: They are not unplanned but hotfix.

**James**: They really are hotfix in a way. 

**Tim**: I feel there must be some software terminology for that.

**Louis**: It is a fix.

**Tim**: Hotfix is the actual term?

**James**: If there's a bug in really software and then there's another one that needs to be really tried afterward, it's a **hotfix**. They're usually really small upgrade or deployments and it's just for that one issue.

**William**: Using bug fix can get a bit weird though because if you take a look at things like Muir Glacier for instance, I mean it's sort of implies that difficulty bomb is a sort of bug, which is not what a bug fix would do it.  
**Tim**: The difficulty bomb in itself is not a bug but it's our failure to.

**James**: And I was saying hotfix.

**Louis**: Yeah, hotfix. 

**Tim**: I think hotfix makes sense.

**James**: I will add that is a thing to reconvene on. so then that's we can move on.

**Tim**: I feel like we kind of have this summarizes Network upgrades and then leave subcategories which are probably in the wrong order for comments
Network Upgrades  
Contentious Upgrades
Hotfix upgrades 
Roadmap upgrades

**James**: I will get back into it but it's jelling in my mind, which I like. 


# 2. Fleshing out requirements for EIP

**James**: Moving on, an overview to get people caught up there's an interesting problem that not all EIPs really should have the same requirements of due diligence on both the EIP author and the core devs. I kind of see them as for the three categories that I've observed as we've been going
1. ProgPOW is one of those categories where it was where they even required a software audit before it would be considered and that hasn't been a real requirement that's put on any other EIP has a requirement for software audit 
2. then there is this other level that's kind of exists in which it is currently the elliptic curve precompile one where we don't have a good way of saying hey you need to do this if you're doing this

**Tim**: 3.  I think there's another category of like EIP 1559 where there's both the technical challenge as well as the economics. So it's like do we you know we want to do this big change its assume that it's going to make things better but how do we actually evaluate, so that's another question.

**James**: and so far what it's kind of come up in conversation is in the case of the elliptic curve cryptography one like the core devs don't have domain expertise in the very complicated math, that kind of high-level cryptography but having other members who have the expertise to review those PR, explicitly make that as a if you're doing something beyond normal then having experts come and vouch for the work you're doing, is it important?

**Tim**: yeah I was going to say I think that's generally a good solution and loosely enough define that it works so if you look at like 1962 vs progpow I think ProgPOW because it touches many different parts like the biggest reason you're doing it this delay ASICs and that's like a whole other can of worms in itself with Hardware. Having a  Hardware expert and a software expert sign off and say that this is kind of needed whereas for 1962 you don't have this Hardware component, you just have the crypto, like Louis has proposed in the previous call having specialist sign off, I also think it's kind of sufficient. so maybe it's just about that it sounds like peer review in a way. But what peer and what review means will be very dependent on the context.

**Danno**: I think with the ProgPOW example, one thing to point out is that the algorithm is replacing Eth hash also had an audit covering basically the same things so for Eth hash was being subjected to the same scrutiny and then get replacements was put under, so I think that's what they need to consider, you want to lower the scrutiny standard and maintain the scrutiny standard for these EIPs.

**Louis**: I just want to add on top of the earlier comments. I am with what James would say. But basically, there are three sorts of EIPs today for which the process is not perfectly defined. There is ProgPow where the problem is not technical it's a political one and for which I think, we could have done a bit of work and delegate even before all the technical analysis because I believe the technical analysis was given as a way just to delay it because no one wanted to take the political hit of accepting it. The reason is, I do blame that I know we had a discussion on the core devs about the miners and people coming in defending EIPs. In the case of ProgPOW, we should have waited to accept it, potentially accepted on technical condition and just adding the  narrative of explaining that this is coming as soon as it's ready. The narrative we have for Eth 2.0 today, but applied to ProgPOW. That would have allowed us to avoid this whole technical audit but as of today is useless and we don't know really where it goes. It could have helped and might anyone can say, okay this is going to happen. It's going to happen soon as we have the right auditor and we're happy with it. It is going to be accepted and there is no cost around it or going to be refused in first place. I think this discussion could have. been pushed by one of the core devs and with the miners who came in for EIP when there was discussion about the reward reduction, and keep coming to the core devs to defending it also try and modify the narratives on crypto twitter saying this is it and we've no choice around. That was when we first talk about ProgPOW. 
As of 1962, I think the as you perfectly said, the problem is technical expertise of the core dev and every EIP on the outside of their expertise are needed to be dealing with a lot of thought and lot of auditing and make sure that the core developers are actually comfortable with the way EIP is entered. The problem with 1962 is Alex did a terrific job with coming with talking, coming explaining what they're trying to do. The problem is that there wasn't enough coordination, like the process wasn't clear enough for him to gather the (?) people to come and vouch for his work. I think if you propose to bring like people like this person to (?) crypto need help but might we still need to ask people like you, Danno or Martin to see what to do next.

**James**: yes

**Tim**: I agree with all of that. I think one thing is also worth noting is, it's normal that these things are hard and the change you're proposing, so on one hand, it's like you want to have a smooth process but on the other hand if you're proposing something that's totally new and hasn't been done on Ethereum and this is like something 20 billion network that's live like. I think it's fine but kind of take the time to get to a spot where everybody's comfortable, even if that means that the process, we won't be able to define the process for every type of new things in advance, right? So like this 1962 is different from ProgPOW and that's probably going to be slightly different from something like Ungas. So I think you kind of need a loose high-level guideline probably to be more explicit that if you're coming in with this huge change in Ethereum, be prepared to spend like a year to kind of getting it through and just to set expectations. because I think, it would have been impossible to say 'No' to ProgPOW on Day 1 just because there are so many unknown unknowns. I guess it's just like the setting to write expectations for the people who will pick on this road while also making it clear what they have to do probably better than we do today. 

**Louis**: I just want to comment on top of this there  is one of the things I find disturbing to some extent is to some for some EIP, people pushing it, the champions are not  always the core devs. I think, because we are talking about the 20 billion dollars network, it should be a hrad requirement for some representative of the EIP to be adhered  to come up at any call.

**Tim**: Yes and we should probably just make it clear to them when they should show up. so I can see, I don't know what to take again 1962 as an example if we don't talk about it next week you know it's not great use of a person's time to be on the call being there. They should check the agenda.

**Louis**: To be fair, I don't care. I mean you're talking about grading a system of 20 billion dollars system. For which people are supposed to maintain it for 10 years or more. They should be coming for 6 months for that meaning.

**Tim**: So maybe that's kind of part of **setting the expectations**, that you should be willing to iterate on this thing for a year. You probably need non trivial amount of funding, to get independent implementation and audit. We expect you to be whether it's on every call or to at least check the agenda and if your thing is mentioned, then be there. I think that's reasonable.

**William**: You're probably still going to find some exceptions like reasons why there might be reasonable cause to not be able to make meetings consistently but yeah.

**Tim**: Sure, but like, Danno just delayed its progress and if they are fine with that like that's not the end of the world.

**James**: Yeah, the expectation of moving forward, you show up.

**Louis**: Not only for moving forward, to just be in people's minds. I'm taking example, on the last call there was a new EIP that came in about the requirement for a contract to specific for gas or something, I don't remember the content but the person was very interested but the reason why it is not going to get in is not because I don't think this EIP is not solid but it wasn't known to the core dev people. I think like if you were to come more often, even if something wasn't on the table, if they are out, gather some comment, some agreement that this is made.

**Tim**: So, maybe an action item we could get out of this is kind of a guide for like EIP Champions and I don't know how we split this between small EIPs and big EIPs it's not like you know it when you see it. if we can have like a paragraph or two, on EIP 1 or just on the EIPs website,  like the homepage of like here are couple of examples of very large projects that people have tried to do on Ethereum and see it's kind of what you should assume you'll have to invest in terms of time in terms of like money or just like Technical Resources and timelines, you know it's  not going to happen in three months more like 6-18 months type of things. At least you could set the expectation straight and then we can see if the people agree or disagree with that.

**Pooja**: To be clear here, Tim, are we suggesting this action item is on the EIPIP team to figure out a guideline for EIP Champions or is it something that somebody's owning individually?

**Louis**: I think it's related to the mentor things that was discussed in the first meeting.

**James**: That would fit in there. I split up table contents to have requirements, EIP requirements and EIP recommendations. And recommendations being just tried and summarize on what we've gone over so far if there is something outside of the  expertise of the core devs, you need outside peer review from experts.  if you're implementing some thing or upgrading something having parity with a previous implementation, like ProgPOW got an audit. you should expect if the thing you're doing should maintain the standard of the thing you're replacing. I had them lined up in my mind and then they all falling out. what is one of the ones I've missed?

**Tim**: yeah I think just like the timeline, attending core devs call, peer review.

**James**: And then what I would add is, it came up like what to do if something goes wrong? what is the plan for action of doing it? I mean the elliptic curve cryptography one,  one of the reasons the Geth team was hesitant was if something happens with that EIP on mainnet, that they'll just sit there and look at it and say oh boy! which isn't a good plan. it's like having a plan for it if your EIP needs to have a separate plan that needs to be made in advance. 

**Tim**: Related to that what was said about 1962, I forget his name but the guy who's been pushing it kind of assumed that it is his responsibility to show up if something goes wrong. so I think that if you're a champion of an EIP, you 're a person of contact, but there probably should be two people. Alex seems to take it seriously that's great, but you probably want at least one other person in the world. I don't know if they're like champions for I'm not sure what their title is, like who do you call when there's a problem .

**James**: I'm not sure that's going to be enough though that exclusive. They need to have a plan and that needs to be written out. Because the disconnect that happened was Martin was like oh no what are we going to do, and Alex the whole time was singing oh I'm just going to show up and help. and if he knew Alex's  plan of how to address like a critical something happening on Mainnet and that was written down, it doesn't have to be a dependent. Each EIP  might have a different plan but having that expressed then understood, I think would calm some of the concerns that people had.

**Tim**: It's almost like if you need to ask what are like the potential failure modes and what to do in those failure modes, right? what happened, say with 1962 if two implementations disagree, like how would you debug that? what happens if like I don't know some of those things goes wrong and then I can see a bunch of those with ProgPOW as well, right? What happens if they're still ASICs on the network, if they're still whatever so just thinking how on a high-level you would mitigate them, what kind of difference is the security considerations section which seems very focused on like the implementation in a way but it's almost like the potential risks.

**Louis**: I think you might be turning to 1962, one of my concerns was the quality of the specification not because I'm assuming that they did a bad job but it's probable that when I look at how people are pushing for the upgrade, that is (?) pushing something called as (?). He has been doing workshop like they are ready to explain to people how these things going to work. For EIP that big, and complex, I'd expect not only some of the spots to react, but also just the knowledge to be spread for anyone to  grab it to understand and from zero.

**Tim**: So, does that like a fully comprehensive specification, then need to be requirements cuz I feel if you get an audit for an EIP, you kind of wants that specification anyway. if you get peer review, you probably want the specification. so I'm not sure how to define this but some full complete specification.

**James**:  how is that different than or how does that intersect with saying you need to have peer review from experts in whatever it is. 

**Louis**: I think you're right and the second and the peer review also mean that those peer reviews are coming to core devs, and bring their reputation  on stake and they would say, yes, it's good and we can push forward.  

**Tim**: I'm not sure what I think here, but like the peer review, I assumed is a specification that another expert in the field can read. but maybe average core developers won't be able to grasp  the entire specs whereas I feel like I don't know do we want the requirements above and beyond that any core developer is like comfortable with the specs. I am not sure, if it is even realistic. so I guess 1962 as an example, I can see a case where like somebody from Aztec looks at the spec and he is  like yeah that sounds good to me but I don't know we have Wei and Danno on the call and they don't have like that crypto experience. So maybe they're not as comfortable with the spec. It is like, who should we be aiming for the scope clarity. Is it like the Aztec researcher or is it like Wei and Danno and Martin understand every single spec.

**Louis**: I think that case I would have asked like to be obviously vouching for it and then Danno and Martin and then Wei to have sort of basic understanding of what could go wrong ? and how does it work, I mean like the generic idea. Danno, how do we comfortable the way to share an EIP?

**Danno**: I can speak to what I am familiar with the engineering tasks but you know what it comes out like you said to (?) all those are interesting sorts of questions. It's not something I am trained in. I'd like having someone else come in from the industry of cryptography and say oh no, this particular crypto thing provides what it claims it provides. I think that is something that will be valuable. When I look at these, I look at the engineering perspective and I think people will chime in. Chime in related to their stream to evaluate it is valuable. that's why some of the crypto stuff is it at least a cursory glance is needed. you know maybe Rock Solid, I don't think many of the engineers on the call will satisfy and say well yes, it's rock solid. 

**Tim**: So, someone to validate this spec. so it's like this spec is clear enough that any core dev engineer can implement it but they don't know when they're plugging you know the sort of consent to put the curve, what? like is that the good one and you want to be confident that the sort of assumption in the spec is correct and that's where you get the peer reviews value for.

**Danno**: Right because it we will take it if it presents itself as this is good solid crypto, we don't know any better we might take it. Which is like getting someone who validates those claims that looks like it. Those are the things that are valuable.

**Louis**: Usually understanding the Math are like (?) In any case the bug doesn't come from the Maths, they usually come from the way you write the codes. I am not sure, even if the spec was (?) it will actually save you from any trouble. I think what we actually have are experts in both the cryptographic and then (?) part of the cryptography. 

**James**: I think we are getting a bit trapped in the weeds though, if I can try and pull out for a second. We're using  it as an example to prove that we can't codify exactly what each EIP is going to need if anything there should just be a reference but depending on the scope and just how critical an EIP is, on a case-by-case basis, there may be unique things to each EIP. It seems like everybody was more or less on board with that ProgPOW needed an external full audit because it's ProgPOW. I mean it's the guts of the consensus algorithm to the Ethereum to run on and if anything we don't need to figure out what every kind of change would need right now, I would think that all we need to do is in that big way you were talking about before, Tim. It's just a case-by-case there may be different things needed it may need a more thorough peer review, it might need it credible third parties it might need a full audit. I don't feel like we need like really nail down exactly when we accepted for every kind of EIP right now. 

**Tim**: I agree with that but I think what this conversation was useful because if you go if you assume that like people are satisfied with this kind of expert peer review then what that means if we had that in the process Progpow probably would not have needed an audit because if they could have found somebody to just come on to call and speak that would have been sufficient, right? and I'm not saying maybe finding someone to come on the call and speak about ProgPOW basically cost them the same as an audit. but it was like BoB Rao from Intel, for the hardware audit. But if ProgPOW people were kind of just friendly with Bob and you know got him to come on the call and vouch for it then that would have been like a much more lightweight process that probably would have gotten us the same kind of safety assurance that the audit gives but in a much more efficient way. And like Louis pointed earlier that the audit was an easier way to put it on the road, to define, it makes it then harder for something above and beyond that for political reasons and that's a good thing. Well obviously maintaining like this is a high-stakes thing and you want to be serious about it.

**James**: A part of the nuance is that there's difference between the general requirement of, if you're doing something that's outside of the normal purview of core devs, you should have external peers validate and vouch for it like publicly validate and vouch for it with a reputation like involved. but is there also a need or should there be an expectation of packaging what's going on in such a way that the core devs have a pretty good grasp of it. cuz you could have it all be symbols or whatever and then like okay to have a voucher and as long as you can kind of implement it, maybe that's fine but should there also be an expectation that this is an unknown for me, making a literature or resources are presentations that are designed to give a core dev a sufficient understanding, whatever that means. outside of having someone else come in and say yes this is what it says it is.

**Tim**: yeah that's a good point, cuz that's what Rick was asking about 1559 a couple of calls ago. because what they went ahead and did was like a full implementation as a way to get feedback but you know if they had that type of collateral whatever it is they could have requested feedback on that before going into the full implementation. the hard part is defining what that is.

**James**: In their case that was it was hard to really get a specification without building out some kind of implementation, which is just sort of the nature of how they chose to approach, may be a better way to say. They chose to approach with creating an implementation and then make the spec fit in. 

**Tim**: Maybe that's a question that's worth bringing on The core devs call next week just because we've also only have two minutes left and it feels like something where it would be valuable to get like the Geth team's opinion.

**James**: Yes!

**Pooja**: yeah, I was about to mention that. so yeah in the essence of time if we have anything that we can quickly cover, I am not sure if we can take care of code of conduct, but I saw some conversation from Brent about EIP 3 that he was mentioning?

**Brent**: yeah I forgot just a sec if James could just give me a quick rundown but if it takes longer than a minute or two we can do it offline or something.

**James**: Let's do it offline, the harder part is I am on my mobile phone that means, I can't show or click on things or.

**Brent**: Okay, let's do it later.

# 3. Code of conduct

**James**: Is there stuff you wanted to go over what you're thinking about the code of conduct and things Danno? like you sort of get us prepared to think about it over the next two weeks?

**Danno**: Sure, in general, we need to have some sort of explicit standard of how we treat each other in these environments like all core devs, in the EIPs. I am not concerned about the list of protected classes that seems to like have code of conduct, I think we're all on board with that. but I think we need some sort of standards and boundaries for when certain Behavior is unacceptable and how we treat it. It's just to think about next time but you don't like I said my concern is not about the protected classes on your list and it's about generally conducted.

**James**: okay, like I've  had this on my mind too seeing the ETC like what kind of happened it would it good to get some of this sorted out, in advance, in very amorphous and not very said well.

**Pooja**: I am not sure, but Charles from the Cat Herders team had done on code of conduct for in general, how it should be for participation and ongoing conversation; is it something similar to that you're talking about, Danno or is it something specifically how we proceed with the protocol with core devs and EIp?

**Danno**: It's about basically Charles was talking about and that the scope would be limited to enforcement is the worst, we could do if you could kick people out of all core devs, the worst we could do. that's why I think the EIPIP  is right place for all core devs call discussing an issue like this that has a meta change . 

**Pooja**: I'm sharing a [link](https://github.com/ethereum-cat-herders/PM/blob/master/CODE_OF_CONDUCT.md) of what we have in like the cat herders code of conduct that Charles has created sometimes back. if this could be helpful or if we would want to add something else and place it somewhere else maybe at EIP GitHub or somewhere else. people can give a thought on that. 

**Danno**: Yeah, this is the sort of thing that I want to get bubbled up a but about just the cat herders to have it apply to the all core devs call, all core devs gitter in the EIP process.

**James**: It would be good to have for the EIP, something with the EIP repo.

**Pooja**: We've got this guideline and we can think about what else we would want to add specific to EIP process or core dev; then we can create that and maybe place it somewhere on EIPIP or EIP GitHub itself.

**Danno**: I think **we can take this existing code of conduct** like this one and just change the scope of the impact. What's acceptable with us, be well understood, things like that we just need to get nail down what are scope is who the parties we report to and what actions are to be taken in response to violations.

**Pooja**: Okay!

**Tim**: One comment, I would have, I feel like this can open like a huge can of worms and as we think about the scope thinking how can we like narrow it to be like efficient but kind of reduce the argument surface. because I can really see the feather becoming a massive dumpster fire if it's too broad so just trying to figure out what really essential, what we want to keep and be very clear and concise about that so that it doesn't kind of devolved a huge month-long argument.

**Pooja**: We can **continue this discussion in the next meeting**.

**James**: okay then I believe that is all.


# 7. Next Call

**Pooja**: the next meeting we plan 2 weeks from now?

**James**: yes, 

**Pooja**: Anybody who is not on the calendar invite and they would want to be on the invite please DM me their email address and I would add them to the calendar invite.

**James**: Yeah! I'll do that. This was recorded automatically somehow because Hudson is said a genius and so then that can be made posted somewhere at some point. I think that's all thanks to everyone for coming in.

# 4. Process documentation

Couldn't be discussed. 

# 5. Progress on EIP repo cleanup

Couldn't be discussed. 

# 6. Any Other Business


**Louis**: Anyone will be in Paris?

**James**: I should be there.

**Tim**: I will be there but not the hackathon.

**Louis**: I mean for Eth CC.

**James / Tim**: I will be there.

**Louis**: okay so we could meet you there in French cafe 

**James**: And in-person EIPIP meeting. that's a great idea.

**Louis**: IP EIPIP :)

**James**: Something of that sort :)

**Pooja**: Thank you, James! Thank you, everyone.

### Date for Next Meeting: Wednesday, February 26th at 1500 UTC.

	
# Attendees
* Brent Allsop
* Danno Ferrin
* James Hancock
* Jim Bennett
* Louis Guthmann
* Pooja Ranjan
* Tim Beiko
* Wei Tang
* William Schwab


## Links discussed in call:

* Agenda: https://github.com/ethereum-cat-herders/EIPIP/issues/5

* James's PR: https://github.com/ethereum/EIPs/pull/2508/commits/c56e992586b027e45bca0770b545f3407a838a00

* Tim's PR: EIP-1 “hard fork” PR: https://github.com/ethereum/EIPs/pull/2516

* ECH Code of conduct: https://github.com/ethereum-cat-herders/PM/blob/master/CODE_OF_CONDUCT.md

* EIP 1: https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1.md
