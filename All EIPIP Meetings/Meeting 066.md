
### EIPIP Meeting 66 Notes
### Meeting Date/Time: Wednesday, Oct 05, 2022, at 14:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/181)
### [Audio/Video of the meeting](https://youtu.be/tMe14UC5DkA)
### Moderator: Pooja Ranjan
### Notes: Alen (Santhosh)

## DECISION ITEMS
**DECISION 66.1**: So we have to create an issue to change the date of creation of merged EIP as draft and the date will be the date of merge by Eth bot. 

**DECISION 66.2**: EIP 5517 will be closed and Victor will come up with a new PR.  

**DECISION 66.3**: Change in the EIPIP meeting call - Pooja to reach out to individul find an time which works for all, and publish it.


## Intro
**Pooja Ranjan**
* Welcome to EIPIP meeting 66. shared agenda and chat. We have a few items listed from the open pull request and issue side. the first item here is open items from the past meeting, but I think that most of them have been added by Sam already as the issues where we haven't reached consensus. So maybe we can start with the, with the items. So those were partially discussed and are listed here again.

## Website: Add MathJax ethereum/EIPs#5596   [0.31](https://youtu.be/tMe14UC5DkA?t=31)
**Pooja Ranjan**
* Website: Add MathJax. I believe it was discussed in the meeting last meeting as well, but I don't know, like Lightclint was not there at the time. under it was only Greg and Sam, which seems to be on board. Anything specific we would like to discuss about this proposal? 

**Lightclient**
* Yeah, that's all I remember about, about it. 

**Pooja Ranjan**
* And if I remember correctly, it wasn't tested at the time, like we were not sure of that. 

**Lightclient**
* Right, Right, right. 

**Pooja Ranjan**
* So I can't see Panda on the call. I'm not sure if we have any further updates on that, so maybe we can skip this one unless, anyone else on the call has anything to add or share. 

**Sam**
* I think we should just turn it on. I mean the risk is it doesn't work and we don't like it and we turn it off again. I think it's pretty low, low impact side of 

**Pooja Ranjan**
* Sounds okay to me. Okay. Anyone has objection? 

**Lightclient**
* Go for it. 

**Pooja Ranjan**
* Thanks for support. 

## CI: Disable certain labels from becoming stale ethereum/EIPs#5655 [1.58](https://youtu.be/tMe14UC5DkA?t=118)
**Pooja Ranjan**
* The next one CI: Disable certain labels from becoming stale ethereum

**Sam**
* Yeah, I think we just haven't really agreed on which, label should, we could scale or not. I think we have been discussing in the PR. able to make this possible meeting. So think got missed the last two. No. Trying to make a time that can Agreed. 

**Pooja Ranjan**
* I have actually added that in the item number two as a change in EIPIP meeting time, though we recently have changed from 1500 to 1400, but obviously we are open to thoughts. Yeah, I dunno, I can't see Panda or Victor mentioned in the chat that he may be fine with somewhere around 1500 UTC. Do you have any preference? 

**Lightclient**
* Maybe We can figure it out A huge problem right now, but just wanted to mention it. I think there's a lot of things, things that he's so hard to make a decision now. 

**Pooja Ranjan**
* Yeah, I agree too. maybe I can start on, reach out to a address individually and try to collect it and submit it before the next meeting. Okay. sorry, just to, be sure again, Sam, what are your thoughts on like, number two CA disabled certain levels from becoming, we continue discussing this in the PR itself. Exactly. Yeah. Okay, cool. V

## Update EIP-1: Fix Backward Compatibility Typos ethereum/EIPs#5680 [4.09](https://youtu.be/tMe14UC5DkA?t=249)
**Pooja Ranjan**
* The third one here is update on Backward Compatibility Typos. Again, it is with Panda. 

**Sam**
* Oh, I think backward compatibility and backwards compatibility are both acceptable and I don't think we should change it.

**Lightclient**
* I agree. 

**Pooja Ranjan**
* Okay. I'm just making a note of it that it agreed on the card. 

## c. Process issues that haven't reached consensus: [4.49](https://youtu.be/tMe14UC5DkA?t=289)
**Pooja Ranjan**
* Okay, cool. I'm moving on. the next one is a list for process issues that we haven't reached consensus yet. 

##  Update EIP-1: Reference ERCs by ERC-X ethereum/EIPs#5273 [4.52](https://youtu.be/tMe14UC5DkA?t=294)
**Pooja Ranjan**
* The first one is, Update EIP-1: Reference ERCs by ERC-X 

**Sam**
* I don't think we have enough people here. 

**Pooja Ranjan**
* Okay, all right. I think we have been discussing this for quite some time. I'm just trying to pull again. Yeah, sure. We can keep it. 

**Sam**
* I just think Matt and I have all good opinions on this and I don't think anybody's gonna be here to, you know, break a tie. 

**Pooja Ranjan**
* Fair enough. Maybe I can bring it up in the next meeting if, assumingly we have more editors and reviewers joining in with the new change in time. So I'll make sure to bring it up again. 5273. 

## Update EIP-1: Clarify when to use requires ethereum/EIPs#5614 [5.54](https://youtu.be/tMe14UC5DkA?t=345)
**Pooja Ranjan**
* Next one is, 5614 Update EIP-1: Clarify when to use requires. I like we did discuss a in the past, anyone having foreign against like when to have it, so if Yeah, please. So if I remember correctly from the past, like it was mentioned that requires is a section that is there. it's not applicable to all EIP, but for particular EIPs where someone is trying to reference something from the past or existing EIPs, they must mention it hasn't request section the number and we generally recommend to have that proposal, which is under the required section must be having status of final. Please correct me if I missed anything. 

**Sam**
* Yeah, so, so that last part is true. It's just whether or not we want to, require every little EIP that  to be in required center or just certain ones. 

**Pooja Ranjan**
* Yeah, that's a good point. Okay, sure. Yeah. as per my understanding, requires where generally used when it is, maybe either the extended version of an existing EIP or using some part of any other EIP like this, this standard won't work if, the project hasn't implemented the earlier EIP, so that was the thing based on my understanding. I don't know, like kind if you have any particular thoughts on when to mention EIP here. 

**Lightclient**
* Yeah, I mean that's my thought too. I don't think that we should change that. 

**Pooja Ranjan**
* Cool. 

**Pooja Ranjan**
* Okay. Then maybe we will keep it open for a few more times to see if any editor has different thought to add there. All right. We are also joined by Victor now. before we move ahead, let me try to, bring this item again. So if he has any thoughts, probably we can capture that. So Victor, we were talking about, the request section in an EIP number is 5614. it is clarify when to use requests. So, looks like the general agreement is when we are using an EIPs extension or sending a proposal for an EIP extension or the present proposal, which is using any other EIP in final status must be mentioned there. 

**Victor**
* Okay. I thought the original, consensus that we near we are, we were near was that if it's mentioned in specification section, we will require that to be required and then elsewhere would be authored at discretion. Is that, if this meeting reach a different consensus? 

**Lightclient**
* I think that's just the trail ends indicator of what we actually want. Like I don't think that you should mention an EIP in the specification section unless it's required as part of the specification, but that's like a separate thing. Like if I happen mention, oh, this is similar to this EIP shouldn't include it in requires, I should just not have that statement and the specification. So the thing that we actually want is we want required to only be, you know, required if you have to have, you have to implement that EIP to implement the, one it described.

**Victor**
* Yeah, that argument I agree with you. like plan, I actually don't know what you go by, but so, my understanding about our view on, specification is that specification, that particular section should be as brief as possible, not mention anything necessary. In your very example, it's like the other one that it is like the other EIP should actually go to rationale, in that particular example. Is that a good understanding?

**Lightclient**
* Yes, I definitely agree with you. I'm just saying that I think that if we say, if you describe an EIP in the specific section, it must be required is not getting to the underlying thing that we're like, that we once here, we want the EIP to only be described and required if it is actually required to the EIP. That's like the fundamental goal of that section. And if we say it has to only like only if it's in the specification section, then I think, you know, we're just sort of like touching the surface of what we want. 

**Victor**
* Yeah, I respect that. if there's the expenses to the team, I just feel that, require making specification minimum plus required when appear require the EIP would appear in specification is the probably the easiest for arguments to be for debate. I can see these examples when you, when we vaguely describe it as like when it's depending on something. for example, yes, EIP 1191, adding the new check on. Does, do we think it's depending on the EIP 55 the original check on without considering, chain EIP, I think argument can be made both ways and then I think that way we do our, productivity in terms of reaching consensus whether one or not, I just wanna put that into consideration. But I do the accept consensus. 

**Pooja Ranjan**
* So I'm just trying to understand here from where I'm hearing looks like both of you are saying the same thing. It is that I'm trying to understand what is that difference of opinion or thought here. So the idea is like if someone is mentioning any proposal in specifications, that means the new proposal which is on the table cannot be implemented unless the earlier proposal, which is being mentioned in the specification is already implemented. that's my understanding. And if that is the case, that proposal, the earlier proposal must go into the required section. I'm looking into EIP 1191 one that you just shared. So here, we have 2 EIPs in require section 55 and 1055. So, they have mentioned EIP 1055 in specification as well as EIP 55 . Yes, they did mention both. So both had in required sections. So if you can help me understand what's the difference here. 

**Victor**
* EIP 1155 didn't mention EIP  155 specification section. It only mentioned that EIP 55 because they used the same algorithm. So in that particular case, 1155 was not required. 1191 was not required. So when we say 1191 adding chain ID to mix tape it achieves, protection on, on we play attack, but it actually didn't require 155, which, at least I think based on the specification, if it says however that chain ID of chain ID is a requirement, then definitely this one is, it is depending on 1155, but since the specification didn't mention it, we can just ask to remove it. so I'm just using the example project provide to the, to see, to provide an, an a demo of editorial feedback for author. And I think that that's actually a simple rule to remember to propagate between editor and author also to help offer . All Right, the judgment here is that whether chain ID is a taken for granted things, if people think in the EIP in a development of the later EIP a chain ID is a taking for granted things, then people should assume that I, that chain ID as defined by 155 should be, configured, non required because it's already taken for granted. But if we do, but if we don't think they're taken for granted many other things like half merge should actually be required, then that goes on and on and it, it's a very honest about in. So that would be my, my take. But  I do respect that if we want just keep it a little bit vagued for giving me way of more, discretion by I'm okay that, so yeah, depending on the word, Right. 

**Pooja Ranjan**
* So, it looks like, there is no strong recommendation of changing of the wording, existing wording in EIP 1. So we can probably let it live like that. And if we come across any new proposal in the future where, we might need more clarification, then probably we can bring up this discussion at again, because all these EIP that we discussed so far are like already in the final status. And EIP 1191 one is actually having both the EIPs in required section, if that's okay. 

**Victor**
* Sure. 

**Pooja Ranjan**
* Cool. So no, we can, we don't need to change the wording over there and we can let it be as it is. All right. Yeah, thank you. And, we can probably move ahead. 

## Update EIP-1: Add finalized date to the preamble ethereum/EIPs#5517 [17.09](https://youtu.be/tMe14UC5DkA?t=1029)
* The next number is 5517, that is update EIP 1 add finaled date to the preamble. we discussed about it in the past, if I remember correctly, right now, the templates just only created date, however, the created date is, is not the date when it is merged. So having the date, finalized date when the EIP gets into final status, I guess that's the proposal here. Thoughts, if any, if we need this field to be added, 

**Lightclient**
* I really don't wanna add this field, but I would absolutely to have an EIP upgrade field.

**Sam**
* Yes. Like I would love to have some kind of a field that describes the state on Ethereum block number it was activated in, like that kind of thing. and yeah, I don't think finalized state is probably the, like it's not a good proxy for that information. 

**Pooja Ranjan**
* I think the state on Ethereum and block number is only applicable to one particular category that is core, and it may not be there for any other, including, interface and networking because they can be implemented on client level at different point of time. So we may want to look into something which is common for, all types and categories. 

**Sam**
* That's some pretty, we can, we can add finalized date, but it really is not useful to core. 

**Pooja Ranjan**
* Yeah, right. 

**Sam**
* I mean, Victor, if you're opposed to it, 

**Victor**
* I am okay with dropping it. I think this was originally requested by Mikhail, and like materialized that he request, but if, yeah, if editors are like not in favor, this, I'm happy to be withdraw this.

**Lightclient**
* Probably Useful for some EIPs. I think that's fine, but I really don't think it's something that we need for.

**Pooja Ranjan**
* Actually, I have a couple of thoughts I would like to share here. As I mentioned in one of the meetings that I'm also looking into automating the process of EIPs insight that we are working on currently. So in that we came across this field, I'm try, I was trying to collect data for the past EIP. So when it was introduced, as of now as of date, what we do is like whenever an EIP is merged for the first time as draft to EIPs Github repository, then we added as EIP added in that particular month. But we were having hard time finding, this information for old EIPs because we have to actually go by every commit number. So we have to go to every, I go to its first commit and then collect the date from there. One of my resources, what they, what he tried to do is like collect the created date, but obviously the date it was created and the date it was merged was not in the sync. So I was also thinking of having one date in which we can be finding it like everywhere. So if it is useful when that proposal is merged as draft for the first time, that could be the first time when it entered into the, EIP repo, if we can have that date instead of created date or finalized, because finalization can be there there for core EIP, we can track when an upgrade is activated and that particular EIP was considered for that upgrade. So we can definitely  have the final date, we can collect the final date from there. Yeah, any thoughts or suggestions, solution?

**Lightclient**
* Sorry, I don't understand why do we once the date that it was first added to the repository. 

**Pooja Ranjan**
* So, for creating this EIPs insight dashboard, we are collecting information of how many EIP were merged as draft or as final or change of a status in a particular month. So, draft is the first status when, and EIP is added to Github repository. So I was hoping if we can have that field, definitely it's something that we can collecting data from Github as well. But if we can have it as well. 

**Victor**
* I think you are coming from, like  a collecting that kind of, reasoning and that that makes, the time to merge, helpful. I wonder if we can kind of reach to a simpler, version. One is the, the created, which should actually be the first day it was merged, and also the, also a finalized day for non-core to be the date that, it's announced to be finalized. This because ERCs and other things, other EIPs are using final status to declare the, that they're ready to be implemented, but core is actually going as de facto, de facto adoption mechanism, which means only client adopted means it final. So, or may maybe we can just say for core, we will use that final day to match with the last part if it happen. Would that be helpful? 

**Pooja Ranjan**
* Sorry, I could not catch the last part of you. 

**Victor**
* Like, yeah, for core, you mentioned something I'm proposing for final, the noncore, use of date that it was, final for core use the date of the merge. Yeah, Sorry, not, Not upgrade, not The merge of,the Yeah, use the, the date of the, of the upgrade or half work. Would that be helpful? I, I would defer to core editors. 

**Lightclient**
* I mean it's better, but it's still the wrong data type or what's happening there.

**Victor**
* We, I'm okay with, adding data type like block number or a name of update. Do you think that would be helpful?

**Lightclient**
* Yeah, I mean those two values are more what we're looking for cores EIPs, but I'm just trying to think how to deal with this and like fairway across EIPs now we're like starting to purpose how many fields there are for EIPs like what fields there are for core EIP and just making the process more confusing 

**Victor**
* Or maybe that's the weight until we find it more urgently necessary than like we're basic. I heard what you say is basically making tradeoff between adding new ones creates more complexity for preamble versus not having the few reviewability in some of the cases. And it seems like in your mind, knowing the finalized phase is not super helpful to justify the more value introduced in,

**Lightclient**
* I mean, I don't know if I would say it Like it's not valuable. I think that right now it's very valuable to know what upgraded Corey idea is. I just don't know if it's all built out that valuable to have time, live date for your, 

**Victor**
* Okay, how about this? Let's, pause the request to add finalized. Say let's prioritize adding what is, adding the, the upgrade available  to the core so that you don't have to think about it every time when talking about finalized day. And then we can decide whether finalize day is helpful at all for all. 

**Lightclient**
* I lean towards not having one date. That is seems to be common, but people can say common ask, Hey, why do core doesn't have things like that. I just wanted consistent across different types for that particular, 

**Victor**
* Yeah, so, okay, this here is my proposal. I will create a new PR, add a final add a new field says this is the upgrade for the core. And because people are easily understand only applies, the core people will not have impression. See if editors are happy with that, include that and then we talk about where the finalized should be, Will be useful or not. How about that? 

**Sam**
* The, my proposal, I think there are reasons why we don't have, upgrade and block number generally in EIP template. and you know, might in, but I think the idea is that, you know, if we, so were to fork the chain or start a new Ethereum embedding the, the kind of governance information, the EIP might be a bad thing. because like it makes the difference to our chain as opposed to any for of criteria. I'm not sure if that matters so much now with stake and all that, but yeah, I dunno. That's a good argument. That's a good reports.

**Lightclient**
* I'm sorry. You can for our, if you can't for our repository and figure out how to remove that, then I don't know what to tell you. We shouldn't make, we shouldn't make it easy for and then make our lives worse cause of it like be easy to just 

**Victor**
* I think.  I think that is, that hasn't philosophical assumption that I agree a lot. also I have, I don't know, if I really that my, I think I find you mentioned somewhere that you are thinking that EIP is trying to  govern the Ethereum and particularly mainnet, which I think, at least in my intuition, I agree. And in that argument we should not, it's not very helpful to assume that other for who need to have a different block and different block number that we upgrade with labels. I maybe people agree, but I also in  a very small voice in my heart that I think is Ethereum, movement is decentralized. And then when we say Ethereum movement, it also applies to anything that you see. So if they want adopt, they can use it. So that's a small voice. Now coming back, I have another like, more practical question for you guys is let's assume we are going to have sharding very soon. What happens is some sharding allowed the block, allow some of the upgrade to defer while other upgrade happens. Is that possible?

**Lightclient**
* No, We'll always have one, global block or slot number to refer to. We'll never get into a scenario where  I mean sharding like this idea has changed a lot over the last several years, but like the shards are now layer two. So if a layer two upgrade to a different point, that's not a concern of the four that you call,

**Victor**
* I can see in the old one in out sharding mechanism, it is possible. 
* I can see that in Dan sharding is much unlikely that they will have a different, they will follow different validated rule. But I, yeah, maybe that's, that, that's thinking too much because that's a very , that's  the scenario that T happened. So if you are all in favor of, of having a upgrade, I will create a new field and, and you can comment. Would that be helpful? 

**Sam**
Yeah, I mean I'm okay with At least three proposal for it. 

**Lightclient**
* I'd be great. 

**Victor**
* Oh, cool. Let me create a new, new field and put on how the old one. 

**Pooja Ranjan**
* Sounds good. Thank you. but one last question before we move ahead right now. the created field is there in the EIP template and that is for the date of creation. When author originally created or maybe some, sent for pull request, is it possible to have that replaced, have that date replaced with the date off merge? I'm checking if that can be done with the help of bot, or existing bot

**Lightclient**
* Yes, it can done by the bot. Someone recently implemented.

**Pooja Ranjan**
* Okay. So we can maybe create a pull request for the, an issue for that, like implementing that in bot, but before we do that, any objection on that and what do people think about it? Like changing the created date as the date of merge as draft in  EIP repo? Is that okay? 

**Sam**
* Yeah, I think you know Eth Bot. 

**Pooja Ranjan**
* Okay, so we have to create an issue to change the date of creation of merged EIP as draft and the date will be the date of merge. I'm saying this for record, so people who is documenting notes may able to capture it as action item. Oh, it's already there. Okay. Then I will try to follow if he's working on it or not. Fair enough. And about this, I think, the final decision here is that 5517 will be closed and Victor will come up with a new proposal. 

**Victor**
* It's not, Yeah, it's putting on the hold I close it. but yeah, I will come up with a PR for sure. 

## Update EIP Template: Add EIP patent waiver ethereum/EIPs#5696 [32.49](https://youtu.be/tMe14UC5DkA?t=1969)
**Pooja Ranjan**
* Okay, cool. Looks like, the next is 5723 we already discussed a bit earlier, so move 5696. That is update EIP Templates Here. Looks like it was proposed by Panda. Fair enough. We can bring it back in the next meeting when Panda is around. I'm making a note of all of those. 

## Add EIP-5617: Non-transferable Token Standard ethereum/EIPs#5617 [33.37](https://youtu.be/tMe14UC5DkA?t=2017)
**Pooja Ranjan**
* Let's move on to the last one here Add MathJax is already merged. The number is EIP-5617, Non-transferable Token Standard why is that listed here as a for discussion?  so here EIP number was an issue. looks like, this proposal was created and editor has some concern. Yeah. Are we  on board there that we can use the earlier number? 

**Sam**
* Yeah, so it looks like the original author approved. yeah. so I'm fine using original number. 

**Pooja Ranjan**
## 2. Past meeting discussion continued
* It just looked like for the Cool, So let's, item number two is discussion. The discuss about change in the meeting time. I know we are short off editors on this call. I will try to reach out to them individually, however, Victor proposes 1500 or 1530 UTC, so if people are in support of either of those, they can signal that on the discord channel. 

**Lightclient**
* And 15 30, 15 30, is it 1530 UTC right now? 

**Pooja Ranjan**
* No, it is 1400 currently. 

**Lightclient**
* Oh, so 15. So this would be one hour later. 

**Pooja Ranjan**
* Yeah, So yeah, earlier we used to have it at 1500, but in the last survey probably six months ago, Editor is a shared signal that they would be interested into having it at 1400. So it was moved to 1400, but if people are fine moving it back to 1500, we can do that. Just that we want be having more attendance here on the call. So yeah, whatever. 

**Lightclient**
* I have a conflict right now. 1500 don't know how long running be, but I probably Do the next I'm For Okay. 

**Pooja Ranjan**
I will up with simple form so we can collect available best. Alteast I haven't . I mean at least I have not seen him for over a year. 

**Victor**
* Maybe We In that case, yeah, I have a PR that I read from manual. 

**Pooja Ranjan**
* Okay. And the other item from the past was, about GitPOAP, so, we were joined by one of the team members of GitPOAP in one of the earlier meetings, recently they have reached us, stating that the GitPOAP for EIP editors are almost ready. They are working with Panda on that. So they mentioned that we have created a bot, GitPOAP bot on Github that Panda will tag with the list of authors of each finalized EIP and if someone was an author of a given EIP in the given year, they will be awarded that year. GitPOAP. I wanted to check here with the team, like, people present here if anyone has any strong objection or thoughts or suggestion on this, like this can be managed differently or should not be done at As you don't reference it, Right? So Yeah, please go ahead. 

**Lightclient**
* They can do whatever they want, we don't have any preference for the GitPOAP

**Victor**
* GitPOAP? That's right. Yeah, I don't have thoughts, I can do night. 

**Sam**
* So I think, so if there's that tags, in the comment of PR, is that linked to GitPOAP? 

**Pooja Ranjan**
* Yes. 

**Lightclient**
* Why would they have a bot posting on every PR? 

**Sam**
* So the architecture that has things was discussed a while ago and it's been a while so I'm a little fuzzy on it, is, GitPOAP has a bot already that, you can arbitrarily like GitPOAP to people, by taking in a comment. And then hand tip was going to write a bot for our repository that tag GitPOAP. 

**Lightclient**
* Yeah, I'm to be able to issue the collapse without interfering with the repository. 

**Sam**
* Yeah, that I think it'd be kind of annoying having it posting on every PR I already get enough notifications. 

**Lightclient**
* Yeah, and it's also like what happens when you have for their competitors today. We also won't do Those Not scalable. 

**Victor**
* That's a very good argument against, having them. They can do, they can, they can observe an issue I think and and if they just wanna, wanna post it, I know it's also give them the power of advertising them and I be like find that it's, it's not feelable if I a competitor wants to do it as well. 

**Pooja Ranjan**
* All right. I hope this meeting recording will be shared today and probably Panda will get an opportunity to follow the discussion over here. I would also like to share it with the, within the group where they are discussing the progress so far, because we wanted to have, feedbacks collected from EIPs editors if there are any objection or not. so far, if I understand correct, this is to be done by Pandapip. So I'm assuming that it is a work to be done manually. So every time Panda is tagging the bot, then only that will be activated. Maybe we can bring it in the next meeting again with these comments registered as like, not in favor of activation, but let's see if they have other ways to convince editors or come to a consensus whether to go by this or not. 

**Pooja Ranjan**
* Okay. So looks like, Victor has added another number 5466, Victor if you would like to explain this, suggest that EIP use RFP 8174. Yeah, please go ahead. 

**Victor**
* Yeah, the original recommendation we have is RFP 2 11 9, which by I I E P, which that, suggests using mass plus do require and all those keyword words document, the intention when describing a standard, the I F F B EP, 2119  itself says it is upgraded. It is updated by the, the matter 1 8 1 75 4. So I created pull request to upgrade the recommendation for us to use the new one. It requires, all the editors approved except for Alex and these things not, I think I happen to see that, got in Greg. Greg are generally okay, but he didn't issue a formal of three days ago, so I wanna see if I, we should, go ahead and, and merge with it with consensus or do you wanna wait for Alex and go to approve it? 

**Sam**
* So I'm totally fine merging it. but it does add links and those links will be by So, for the time being can't is linked add.

**Victor**
* Oh but, the, is okay to link to itf. I thought that was the intent. That was the agreement he reached to when mentioning I f I asked in all different other, I don't think we like, whether we reach or not, the bot will still, Well It didn't, it didn't like that particularly for problems. It doesn't, it doesn't, it doesn't link each one or the template maybe.

**Victor**
* No, no, it, it doesn't, Right, because you, you all have your eyes. and I'm, I'm okay with reading the link, but I just wanna just for now. 

**Sam**
* Just for now. Okay. Like I'm writing up on how to link. I'll post that the next I have one as well. 

**Victor**
* I'm to generate a concern you wanna add to it or we can, 

**Sam**
* Like you're talking about the, the one three close solutions that the hack be? 

**Victor**
* Yeah, I'm trying to consolidate that. Yeah. Yeah, I'm trying to find, the least 10, the the one that people, the maximum agreement here and then leave everything else to still additional discussion. That was my plan. 

**Sam**
* Okay. I will, if you wanna take a look. Yeah. Oh yeah. 

**Victor**
* Okay. I'll link it there and then I'll, I'll, I'll comment. Yeah, I think this has taken a lot of our editorial cycle for discussing whether Yeah, I'll link it there. Thank you. 

**Sam**
* So let me, okay. You want to be removed just for now, right? I can, I can remove it or do you just for now check it out. Okay. Okay. Yeah, I'm okay with that. 

**Victor**
* Okay. We have more links. We have existing link up to ITF in line one 16, EIP had a preamble already, have RT linked to ITF or you really want it to be moved or do you want to, you think case? 

**Sam**
* Just right now if, if a link is in the EIP like if the link is in an actual EIP1 other than EIP one or if one other one that has reception Eth  W will not let you merge the PR so. Oh, you don't, so just for template, right? Exact template people would copying it would not run into this problem. Exactly. Yeah, I'll, I'll, I'll, That's a good point and I just read and strong pro externally person External links 

**Pooja Ranjan**
* Alright, in essence just 10 minutes left though we don't have many more items. 

## 3. EIP Bot [47.46](https://youtu.be/tMe14UC5DkA?t=2866)
**Pooja Ranjan**
* We are good by the time. the next one here is item number 3, EIP bot. I think the main concern that was shared with me earlier in the Ethereum Cat Herders meeting was, that we are not getting a clear, understanding of what all issues to be worked on or not. For example, issue 65 that we just discussed briefly to have the created date. Looks like, Jose wanted to work on it, but Pandapip is also working on a tool which will propobaly cover, this issue. So we may not be able to, we, we don't need to work on this issue separately. That's a good thing to have. I wonder where we can track that. Maybe we can check with Panda to provide updates on the issue there or maybe in the EIPIP meeting. Yeah, none of them are here so I will take, take it offline. Yeah, we'll check with both of them.

## 4. EIPs Insight - Monthly EIPs status reporting. [48.48](https://youtu.be/tMe14UC5DkA?t=2928)
**Pooja Ranjan**
* Next is EIPs Insight for the month of October. Today is the 5th of October. We do not have ton of EIPs, to be discussed for this month. So far we have two EIPs that move to the draft, that move from draft to review status and there are a handful of EIPs added in the repository in the pull of request. We hope to see more coming up as new draft have added information for proposals in the EIPs insight hackmd(https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/) and be added to the agenda. 

## EIP Editing Office Hour [49.34](https://youtu.be/tMe14UC5DkA?t=2974)
**Pooja Ranjan**
* Next is a EIP editing office hour. We organized a office our yesterday, it was fine. We tried to look into the proposals, the pull request and we were also joined by a couple of authors. Thanks Sam for conducting this office. I have a question here, which I actually have added there for the next meeting agenda as well. Like, do we want to have this meeting for 30 minutes giving QnA? Because most of the time it is you are reviewing the proposal live, which is good thing to have. but yes, any task there? 

**Sam**
* I mean I'm, I'm happy to keep it for an hour. Okay. but if we want to like, I don't know, I find it rather tax pain to be viewing on a call. So if we wanna bring it then to half an hour on final. 

**Pooja Ranjan***
* Yeah, I think we can do it for 30 minutes, like for first QnA and if we have any author on the call staying longer because we could not address their problem, then probably it makes sense to extend the call. But generally speaking if we keep it for 30 minutes and address those questions and you do reviewing at your own convenience, does that sound reasonable?

**Sam**
* Yeah. So we can make that change. either Victor you can update the calendar or I can do that. It's fine. 

**Victor**
* I'm not following the new update. I'll update the other calendar please. 

**Pooja Ranjan**
* Okay, I will do that. Cool. that's it. people can follow the recording from the past meeting. A link is added and we also have added agenda for the next meeting, which is about two weeks from now. Last one is review action items from earlier meetings. looks like we had only one action item from the past meeting, which was for Victor to create a peer two for the discuss on the copyright previous section. Do we have the poll request? If we would like to add the number here for discussion maybe in the next one? 

**Victor**
* I don't have it yet. 

**Pooja Ranjan**
* Okay, not a problem. 

**Sam**
* There Was one, there was one that showed up. I'll see if I can find it. I'll post you again one. Okay, yeah, that would be great. Thank you. 

**Pooja Ranjan**
* Cool. And yeah, I think that is all. we do not have the EIP number bot yet. Right? I wonder if, Okay, cool. I wonder if anyone would like to pick up this thing and maybe create a bot to allocate EIP number. We discuss this issue in the past, so if anyone has any question like people following this recording, if you are interested to work on this particular issue and you have questions, feel free to reach out and you can probably post your questions on EIP editors channel on Ethereum Cat Herders discord. So that's all for meeting today. Anyone would like to bring up anything? Cool. So let me collect some more consensus for the next meeting time and I will share the information on, Cat Herder discord as well as the EthRnd discard both places. So people following either of the channel for this EIP meeting may be able to join us in the next meeting based on whatever EIP. Thank you everyone for joining us today. Hope to see you in two weeks. Have a good one. 
* Thank you for all. 

# Attendees list
* Pooja
* Lightclient
* Sam wilson
* Victor
* Shubhangi



