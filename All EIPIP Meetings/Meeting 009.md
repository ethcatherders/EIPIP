# EIP Improvement Process Call #9 Notes
### Meeting Date/Time: Wednesday, 03 June at 15:00 UTC
### Meeting Duration: 1 hr
### [Audio/Video of the meeting](https://youtu.be/59Bzw9dHIEM?t=10)
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/16)
### Moderator: Hudson Jameson
### Notes: Pooja Ranjan

----

# Summary

## Decisions Made

Decision Item | Description
---|---
**9.1** | EIP process flow will be separate from hardfork coordination.
**9.2.1** | Rename status in EIP-1 _Active_ -> _Living_ 
**9.2.2** | Rename _Inactive_ -> _Stagnant_
**9.2.3** | No change in name for _Final_ status. 
**9.3** | Discussion to be continued on EIP number registry process.
**9.4** | A medium blog to share final EIPIP survey report will be published on Friday. 

---

# Agenda

- [1. Separation of EIP process and hard-fork coordination](#1-Separation-of-EIP-process-and-hard-fork-coordination)
- [2. An EIP number registry process.](#2-an-eip-number-registry-process)
- [3. Discuss EIP-1 Brainstorming Document.](#3-discuss-eip-1-brainstorming-document)
- [4. ZIPs reference](#4-zips-reference)
- [5. EIPIP Survey](#5-EIPIP-Survey)
- [6. Review action items from previous meeting](#6-review-action-items-from-previous-meeting)

---

# 1. Separation of EIP process and hard-fork coordination

Video | [0:10](https://youtu.be/59Bzw9dHIEM?t=10)
-|-

**Hudson**: Welcome everyone! This is EIPIP meeting number 9. It looks like what we got today is the first agenda item ‘Separation of EIP process and hard-fork coordination’.

We made a lot of progress on this last time. I think James worked on editing the model after the last call, right?

**James**: Yeah, I did.

**Hudson**:  Do you want to go over the reviews and edits?

## Discussion on new EIP process flow
Video | [01:10](https://youtu.be/59Bzw9dHIEM?t=70)
-|-

**James**: Yes I will share my screen, thought I had Axic still on this document but I'm not seeing it.  The one I worked on with this top one and I went in and added all of the arrows for all the state transitions to the back and forth. So you can go from idea to draft and then inactive. I left inactive and withdrawn just so we can talk about it, I don't know whether we should still have two or not; but just so that's clear. 
So you can go back you can go forward to an active or back to draft or from an active to withdrawn but then after it's withdrawn you can't go backwards without making like a new one, was the thought for that.  Then you can go from draft to review and you can go from review to forward and that this could go back and forth quite a bit, like between review and last call or however it needs. Between review and active that the the way active should work is that you do a change to active it goes into review and then after certain amount then it goes back to after that the PR is reviewed and edits and stuff go through that it goes back to active status of people know to go when to look at EIP. It's probably going to do is just quick definitions for everyone to be up-to-speed. 
**Idea** is pretty obvious, **draft** is you become a draft when your formatting is correct and you have all of the requirements for an EIP inside of the EIP itself - quality or should it be implemented or not at all. At this stage it's just editors making sure that and at this stage it's viewable by my people in the EIP repository and an author or the champion works on it until they get to a spot where they want to have greater review from the community and this is so then he has he or she has the ability to change its status to review or request for it to be reviewed and then that is a request for the community and for other EIP authors saying that this is at a point where I want other people to chime in on the EIP and get feedback for more any more stable state or it's at least articulated well for people to come in and listen to it. Which after that point, then there's the process of **last call** meaning that this is my the final proposal for this EIP and then it goes through a two-week process of final comments and if there isn't any then it goes to final, and what **final** means in this case that the specification is complete and the author is happy with how it is defined. It doesn't mean that it's going into anything or that it isn't going into anything, the standardization is in a state-of-the-art, it's the final state. And that any changes after that point should be done by making another EIP which **supersedes** the final EIP. That’s how an EIP can be superseded.
The last call, it seems we were pretty agreed on or had consensus about that this is a great way to handle this flow. If anyone wants to go more into that you're welcome to or if someone has a contrary thoughts to that or things that we should have some clarification on some of this.

**Hudson**:  My only comment is between some of the arrows. Maybe we can put “Meta Only” for Active, so the people know that active is not an EIP status for just anything. Same thing for superseded. Superseded could never be used with Meta EIP because those would only be Active or Review.

---
Decision Item | Description
---|---
**9.1** | EIP process flow will be separate from hardfork coordination.

---


**James**: Oh that's a good point, putting it in here in like italics would be really good.

**Hudson**: Yup, that's the only thing I have.

## Rename EIP status 

**Artem**: Again, **what’s Active and Inactive**? I just didn't get the idea.

**James**: I didn’t describe them. Active is a special status, it’s a weird name but it’s related primarily to things like Meta EIP, registries like EFI document, it’s never going to be finalized. It's a rolling document that’s continued to be updated. 
So we could expect that it is something that is updated semi-regularly or when necessary depending on what the registry is. EIP-1 is another example of kind of special kind of EIP where the idea is that it's never finished; it's designed to be editable and to have changes made to it. So having it go through last call and final doesn't make sense because we're not going to make another EIP-1, we're going to continue edit EIP-1. 

 **Artem**: So maybe the better name for it would be rolling. The whole idea is the release is never finished, it continues to update.

**Hudson**:  I think rather than renaming that one, I almost want to rename inactive and the reason is because inactive and active or not related at all. In fact there on totally different EIP tracks but people may conflate them for the fact that they are generally mean opposite to each other. So making inactive like a name like _stagnant_  then seems a little bit more straightforward in my opinion. But Artem can you elaborate on why you would want to rename active?

**Artem**:  Well because for me when I first looked at this diagram today, I thought that active means deployed on the mainnet.  And I guess this is the first thing that many people would  this EIP is active, it’s live on the network.

**Tim**: I guess that cuz it's different from accepted, right? In the past, we had accepted prior to being on the network and then final meant it was live on the network. 

**Artem**:  I guess that's for the newcomer, both accepted and final and in this case active, they're all confusing. 

**Hudson**: I can agree with that.

**James**: That’s been my experience in trying to describe the EIP process usually involves , specifically re-talking about those words in specific. So at the glance, there's just not enough distinction between Active and Final. It’s very much like accepted.

**Hudson**: I'm just Googling synonyms for that and I'm not finding anything for active that's good. I found some stuff for inactive.

**Artem**: We could call it rolling.

**Hudson**:  I like rolling, I think because this is a technical specifications like repository so rolling could be a good one. I'm not like opposed to it yet or anything.

**Tim**: Rolling instead of Active?

 **Hudson**: yes 

**James**: I think the best descriptive term would be ‘living document’ but doesn't fit in status. 

**Artem**: **Living** works too.

**Hudson**:  What do people think of the inactive changing the stagnant?

**Artem**: Stagnant works better. 

**Tim**: Living seems weird, but it’s small chage.

**James**: It does seem weird but it's also weird status 

**Tim**: I think Accepted actually defines it pretty well.  I guess final.

**James**: Accept, it sounds like it's accepted into what? First thought for Ethereum Improvement Proposal, Oh! It’s accepted into Ethereum mainnet which implies a lot of stuff and can be confusing.

**Tim**: Yeah! What are the cases where it goes to active or living your whatever but it doesn't go to final?

**James**: EIP-1, Meta EIPs, they don't go to final.

**Edson**:  I had previously suggested _register_, since this is made for registry?

**James**:  I'm not fully convinced that we're only going to have only Registries yet.

**Hudson**: EIP-1 is a Meta EIP, so it’s not a registry. So EIP-1 wouldn't have a place to live so the chat has some stuff. “Alita : when I heard active as it's running on mainnet and final as the final draft“. 
That’s a good point.
The only other comment was “Active -> Vital”, Pooja’s idea. 

**Artem**: It would give wrong intonation to it. 

**Tim**: ‘Vital’, it seems like you can not take it out of the network. You’re going to break the network. 

**Artem**:  **Let's just just call it a living document**. It would instantly convey the meaning to users and wouldn’t confuse anyone. I mean if you call it something else,  you will still have to explain it. 

**Tim**: Why not something like reference, like it’s a reference implementation. When it gets final that means the kind of can't change any more but I don't know like reference or something that just kind of highlights, rather than maybe the state.

**Hudson**: I don’t think  it’s a good idea to deviate from the fact that these are all statuses and then one of them just being a descriptor, more descriptor than status.

**Tim**: Yeah!

---
Decision Item | Description
---|---
**9.2.1** | Rename status in EIP-1 _Active_ -> _Living_ 

---


**Hudson**: Alita said, “Final to Staged?”

**Artem**: Not necessarily staged. EIPs  in general are the building blocks for the Ethereum ecosystem and if we make any EIP final, we accepted into this tool box, doesn't mean that it is staged for inclusion into the Ethereum mainnet. That applies to things like Clique or ProgPOW.

**Tim**: Yeah I think final like the definition is literally ready,  the spec will not change any more, unless for typos and I think I feel pretty strongly we should keep it as such. Because it's also something that's really distinct from the deployment, right? Because we can say this EIP is final, for example ProgPOW EIP is final, the spec is done; but that's independent of the stage at which it is with regard to like a mainnet deployment. 

**Hudson**: Interesting okay and I think your main points Tim was the status should separate the hardfork process from the EIP process of what statuses they are,  is that kind of what you were saying?

**Tim**: Yeah, I think it should be clear that these are EIP statuses and not hardforks whereas eligible for inclusion sounds way more Hartfork process, right?
If you want to be coherent, you can say included when it gets scheduled for fork and deployed once it's live on Mainnet or something like that.

**Hudson**:  Got it! okay and then inactive to stagnant what would that be something that anyone disagrees on cuz I heard three people say that was better than inactive.

---
Decision Item | Description
---|---
**9.2.2** | No change in name for _Final_ status. 

---

**James**: The  intention for inactive if a certain amount of time has passed in the EIP has been inactive or not or I guess stagnant is another word to use.  It was by the system automatically put into this stage because of inactivity, so it seemed pretty descriptive. I'm more tied to the function than what it's called. 

**Pooja**: About this status, when we mark it inactive and after a certain point of time if somebody would want to activate it again. So, I find stagnant more appropriate like inactive defines that's going to be inactive forever, maybe.

**Hudson**:  And also inactive implies that there is an active State and there isn't.

**James**: Okay!

**Alita**: final locked? just final doesn't clearly convey its immutability (in chat)

**Hudson**: That’s an interesting point.

**James**:  If we were talking about mainnet stuff, I would tend to agree with that. I think leaving it a standard as being final is articulated well enough for it is clear enough.

---
Decision Item | Description
---|---
**9.2.3** | Rename _Inactive_ -> _Stagnant_

---


**Hudson**: Do we have any other comments on any of this? I think we've done a really good job figuring out where things should go.

## Brainstorm more about the withdrawn/stagnant 

**James**: yeah I think the last thing to talk about is do we have is stagnant and withdrawn necessary or do we just have one?

**Edson**: I actually think it's good to have two cuz stagnant implies soft inactivity and then withdrawn assumes finality ? So might be good to add  finality to inactive status?

**Hudson**: Withdrawn is purposefully making the EIP permanently inactive whereas  stagnant is an activity due to defaults and time passed. So we don't want stagnant or withdrawn to be the only one because then the person would know if it's permanent in the person wouldn't know if it just lapsed overtime or not which is important to make a distinction of if you want to resurrect it and  become a new champion of it for instance. Cuz  that happens a lot with EIPs for new Champions to come in.

**Artem**: Can’t withdrawn EIPs get new Champions that's one question and another question do we want to only have withdrawn but not rejected? so what if we declined to move the 80 from to review to last call to final.

**James**:  The first one if I withdrew an EIP and someone wants to be a champion of it. I think they should make a different EIP.

**Tim**:  Yeah I think, also just politically it makes a huge difference to just say you know this is the new proposal for x and this is what you've done in the past as well. Like when we fix like EIP-1283 the other EIP kind of combined both the original one in the fix into one. So I think it's simpler to say this is a new EIP which replace the previous one rather than retaking this old EIP.

**James**:  Here I wrote in from stagnant you can go back to draft. So if someone just dropped it, you can pick it back up, start it back again but if someone purposefully stopped and withdrew then to have to continue that EIP, you would make a new EIP and have it start its draft with a different number.  

**Hudson**: So we're not addressing the fact that you can explicitly reject any EIP within these statuses ?

**James**: Well,  rejecting an EIP really doesn’t come up unless we're talking about mainnet. You can write whatever you want for standard, there is really no reason to reject a standard unless it's malformed and even then it would most likely go stagnant after a while and then disappear.

**Tim**:  But I think in the hardfork process you should have a rejected so it kind of goes from eligible for inclusion ->  included or rejected and then the mainnet, right?

**James**: Last week, I had a very long conversation with with Bryant and I think I've been convinced that it's better to have keeping track of what's on Mainnet be part of the hardfork  process and be kept out of this entirely.

**Hudson**:  So even though it's kept out of this if I'm just a person, reading the EIP repository and I'm like EIP 972, I want to see if that's ever been included in a hard Fork, will I need to go through every meta or will that be in the header or every hard fork Meta,  that I should say? How will I be able to quickly be able to ascertain that a core  EIP has made it into a fork or not. I know there's a separate process but I don't want to have to dig through a separate process necessarily,  if it's not very well-defined what  EIPs went into where?

**James**: I think there are two ways to solve that, I’m not sure which one fits and that’s a big of a question. One  would be at the status level of having a status that says that this is live on mainnet and has been implemented, so that people know this is something that's part of Ethereum. The other one would be to have a document or registry that tracks these are all the EIPs on Mainnet and have that be a registry EIP that's tied to hardfork process. That would be at least my suggestion. I don't know if  we should go over pros and cons of both or an alternate suggestion.

**Tim**: I think the use case would be weird.  People will either care about what's in the hardfork  and then they can I find a hardfork or care about a specific EIP. Say you wanted to see this EIP XYZ included in a hard fork, you just go to the place where the hardfork  process is defined.  Command F to ask for whatever the EIP number is and you should be able to find it there, but I think having a stylus to get it included kind of goes against the whole purpose of separating the EIP process from the hardfork process. 

**Artem**:  yeah so I'm a little bit confused. I assume that this diagram that we’re discussing currently is only about inclusion into the EIP toolbox and not into deployment on any network.

**Tim**: That’s how I see it as well.

**James**: Hudson figuring out what that means and  what do we do about keeping track.

**Hudson**: I think we all agree on that, it’s just that, that was one of the two ways to do it that James said. I like the registry idea better, that also makes it  so that people can look it up every time.  I see the EIP repository as a little bit more than just something that list out specifications it's kind of something that also is used by people to replace the yellow paper at times to look at the latest Network stack of like Eth 65 or whatever I forgot what they're called. So like the networking layer but also like how to how to implement EIPs based on the rules of the EIP. So even though we're not, we don't want to facilitate the EIP process directly saying what's in the main net,  having a registry,  is a good in between.  

**Artem**: That registry would be another EIP, I assume and it would follow the same path that we have been discussing for past half an hour.

**Edson**: It would be a living document, so it would be like EIP-1. 

**James**: It would be similar to EFI and would be tagged as ‘Living’.

**Hudson**: Yeah,  I like that idea a lot. Does anyone has any comments on this,  the graph, the things we've been talking about, stuff like that cuz we can move on to the other agenda items, if not it  sounds like we're slowing down on this and came to a really good decision.

**Brent**:  I have a question about, what about ones that are like recovery of funds like is it EIP 999 which was rejected but (just hypothesizing) had a powerful consensus building tool and they can build it that they could definitively show that say greater than 90% of everyone (Ether, core dev) are on with moving that from withdrawn back to active or or something like that. And in getting something like that approved, simply cuz they could definitively prove that everyone was on board with that; is that something that's we don't want to consider in here ?

**Hudson**: Not to change withdrawn to anything they would just in that case if it's already been withdrawn by the author they would need to create an entirely new one in that situation that scenario you're laying out.

**Brent**: Okay!

**James**:  The part about getting consensus from the network to implement is all on the hard Fork implementation layer not on the standardization layer. You don't need need consensus to define the standard for your EIP, you can just make it and then have it be the best that you can think of and then all of the other stuff happens in the parallel process.

**Brent**: yeah,  I think, I understood that, thanks. 
**Hudson**: Okay,  anything else in, otherwise I'll move on to the next thing.

**Artem**: I have a peculiar question. If we don’t have this EIP process tied to the deployment to the mainnet, will EIPs go through any scrutiny by the core Developers?

**James**:  Yes 

**Hudson**: The reason they would go under scrutiny or not..

**Artem**: Basically what would be the bar for moving the EIP into the last call and into the final. This is an open-ended question but yeah I expect that this bar would be lower. 

**Hudson**: For core EIP specifically,  it would be the first step would be eligible for inclusion and that would be someone has made an idea created a draft and then said my draft is at the point where I want to consider doing things like test implementations that are really rough stuff like that and then from there if core devs say, yes this meets the standards for EFI this is something that could definitely go in then it would go from there to like further implementations and then that would be almost a review picked point depending on how the cord devs want to do it and that's kind of outside the scope of what we're talking about today but it is a really good question, I think because this needs to be decided along with the statuses so that statuses don't impede that process.

**James**:  I think your point Artem is that it's easier to go from review to last call to final,  is definitely the case and I think that's fine. The difficult part previously was the following was the political part/ core dev including the mainnet parts of having that not be a requirement to get to final, means it's easier to get to the final stage.  For if someone wants their EIP to get into Mainnet then there is the whole other process that Hudson was talking about, of getting it through EFI,  getting it through all of these things. You wouldn't be able to get into mainnet without going through this plus doing that extra effort. And here actually the review I think means that they will get better scrutiny earlier cuz it's something we've had previously is an EIPs  goes for quite a long time and development and the others are working on it and then at the tail-end then everyone looked at it or at least their scrutiny is really delved into as when I finally put a Hey we’re thinking about doing this one. So here with review it's a little bit a combination of this will help focussed conversation on EIPs from the core devs and the community as they are ready to be talked about. I think Greg  EIP is a great example. His EIPs for doing subroutine - what he has proposed is a well-thought-out you could say it's standard and we could make it to final one there are some additional concerns that the core devs have related to it like should we have morer estrictions or not? When it comes to point to mainnet, in Greg's case, it would be easier for it to get to final, which is nice for him cuz he has this he has a thing that he's trying to get done and implemented in work and then other people who want to add on and build on it, cann’t do that.  It doesn't mean he has to go back and forth forever trying to make what works for the core devs or for the rest of them. He can get to a finished product and then additional things that need to be done. So it's being implemented into the ephnet that’s coming in and at that staze, we could say - hey, this is good but there's some extra things that need to be done for it to go in the mainnet. I hope that has a bit more pieces that are helpful that answer any of your concerns.

**Edson**: One thing, I wanted to add was that, I think having EIPs be fast track be able to be  in final s kind of features cuz you have any EIP in the final and is rejected by the hardfork coordination process,  then they can make a version 1.1 quickly and try to address any concerns by that. 

**Hudson**: Are they able to do that cuz once it's in final there's not a way to go back to draft or review?

**Edsn**: Yeah, so when I say 1.1, I mean a new EIP the same name as his version 1.1 for  the new EIP number.

**Hudson**:  Got it, okay I'll let Artem answer anything else before I go to my next thing cuz that was his questions initially.

**Artem**: Yeah **that's a bit concerning that you can have a final EIP that will go on a testnet and then suddenly on a testnet you discover issues and then you have to do another EIP to replace it.**

**Tim**: I shared something in chat. (see image in the call [Video | 35:48](https://youtu.be/59Bzw9dHIEM?t=2148)). For last call, the core EIPs should include the testnet period. So it's like you have like last call all the way up to the main net and then it becomes final? 

**Artem**: Some EIPs are never meant to be deployed on the mainnet.

**Tim**: I meant core EIPs. you’re saying that Clique is a core EIP. For those maybe we just still moved into final, you have the standard 2 weeks last call.

**Hudson**: Yeah I mean, I could make something called the Icebreaker format and it like completely redefines how you do account abstraction (or I'm just throwing words around ) and it could go to the last call in final as long as there is like the core devs say yes that can go to final but that doesn't mean it's included in a hard Fork ever.  so Clique for instance it's a good example of that, the networking Protocols are a good example of that because sometimes like that. I think, in the case of Eth  64/65 or some 64 and 65 like some clients actually skipped one of the networking protocols to go to the latest one. That might have been Open Ethereum actually, I forgot.

**Artem**: No, we introduced 64 in 3.0 and we are currently implementing Eth 65.

**Hudson**: I know it's another client that just skipped it so that doesn't mean that either a networking protocol or Core EIP, either one of those could go into a hard Fork but it can still be final and I think we're going to have to drive the point home because that's going to be confusing, especially since final, up till now, including now, means that it went into a hard Fork so we're redefining the term.

**Artem**: Just a note,  EIPs used to networking protocol is a bit orthogonal to the hardforks because it does not affect the chain state, only how the clients talk to each other. so it doesn't require Hartfork deployment and it doesn't affect the change state. So it doesn't require a separate inclusion process. 

**Hudson**: That is a good point and with that's why I'm on EIP-1 right now, networking is actually a separate category within the standard tracks of EIP.
So there's a standard track EIP and networking a separate from core and it's exactly what you said Artem, is because it's separate its consensus critical as core and networking is not critical.
Tim posted a picture in chat that kind of describes a little bit of EFI process.

**Tim**:  Yes I think, **EFI should basically operate,   ideally like in between the EIP stages** right and it's anyways. So you have an EIP that is first a draft and then it can be made like EFI and then when it goes it to review then after that  it can be included and when it  goes into the last call, then we can pull on testnet and when it’s final, it means deployed. I think it  would be good that there a link in-between. **Which stages of EIP process hook into hardfork process.**

**Artem**: I’d rather call it  not included but staged.

**Tim**: I don't have a strong opinion on the name, but mostly on **how these two process interact with each other**. I have to jump though, thanks everybody.

**Hudson**:  Okay this is all really good,  any final stuff before we move on to the next item?


# 2. An EIP number registry process.

Video | [40:27](https://youtu.be/59Bzw9dHIEM?t=2427)
-|-


**Hudson**: Okay so the next time is an ‘EIP number registry process’,  that's a lot better than what we have now does anyone have thoughts on a better process and also I guess we should go over what we currently have. Right now I believe it's by PR number, right?

**James**: There's a little piece of EIP-1 that we don't really follow but it says that after an EIP is put as a PR the EIP editor gives it a number and the number usually references a PR number. What actually happens is you do a PR you go backwards to figure out what number it is then you put the EIP number in and then that's the only way to get it through the edit bot because you have to make sure you have the formatting correct.

**Hudson**:  Is there a better way the people can think of? I  am okay with the pr number thing because it's an unlimited number set and I can't think of an alternative.

**Artem**: It’s awkward, it ties us to the platform GitHub but then there's just no better way.

**Alita**:  Just confirming we talk about the labeling or the numbering ?

**Hudson**: Yes, the numbering, so like if I make a draft the EIP and then I make a pull request for that draft EIP that PR number in GitHub is what is going to define my EIP number within that draft.

**Alita**: The reason that I brought up changing it in the or one of the reasons I brought it up was because at least with the zcash model they use different numbers signify different states at the process and differently purposes of the actual draft. So you can have the same name and -0 number that signifies states. 

**Hudson**:  That's an interesting idea. I love how zcash does it from at least for my review of the numbering. However what they do if I remember correctly is a things like if it is a consensus critical change for instance it's numbers 100 to 199 if it's a networking change its 200-299 and the problem with that is, we have so many that we can't define a preset range that they can because they have many fewer Zips than we do EIPs. But I don't think you were you something that we should do exactly like that but maybe it include dashes indicate some other facts about that EIP like us like a what category it’s in and stuff like that.

**Alita**:  Exactly and I think you can take just like classification, which would be variable as the process and presumably that would help maintain the history of the process.  Say, you have have 0 through 90 be if it's whatever and then each change that they accepted or refused increments that extension by 1.

**Edson**: I think it might add an unnecessary level of complexity especially since we already have statuses defining where it is.

**Alita**: As I recall, the statuses were in the header of the EIP which in my opinion is difficult to comprehend.
**James**: I'm a little hesitant for that and I think it has to do with one way we have better defined statuses. This is pretty comprehensible I'm looking at all the draft EIPs and how they're organized things like having the number be the link is very easy to handle I don't know if we add and I guess I don't see what we get specifically out of having more using the number system to better specify the status.

**Brent**:  Yeah, I agree with that.

**Hudson**:  I see it both ways.

**James**: I don’t think, I have thought about it enough really,  I want to think about that more. 

**Alita**: The reason why I said it would be beneficial is because, we have a lot of EIPs and so it’s easy to sort only certain categories or certain State EIP.

**Brent**:  So you're saying having an extension to the EIP number would make it that people have hard time understanding would make it easier than just having a simple status filled with well-defined values?

**Alita**: That is what I am saying, yeah.

**Brent**: I guess I'm having trouble seeing that.

**James**: If we have the numbers that have more information beyond the status that might add something as far as in like querying status like querying ability. The way that these are organized filtering by their status isn't really difficult. I wouldn't need to have it if I was to write a system to get all of the draft EIPs for networking. I would need any other information to do that pretty sweet like writing a script to do that because this is really strict on what the inputs are. So if I think we would need to think of more things that the numbers signify that are helpful to have but don't deserve their own status then I think that would make more sense that way for my mind so I currently. I don’t want to say  anything definitive.

**Edson**: With regards to the number of being tied to the PR in issue number. Alex in the previous meeting brought up using a smart contract to choose the number. I am not sure if it is too complex than if using PR numbers for the EIP numbers.

**Hudson**:  I don't see what the problem that solves, immediately. 

**James**: That has a lot more complexities. The reason that I think the EIP number process sucks or is unhelpful is the inflation of because it's tied into the GitHub issues we get weird things were one people come in do 10 issues so that they get a good number and then it floods the EIP repository with random issues for no reason other than someone wanted 5 instead of 3. We’ve seen that a bunch of times already in the EIP repo with that which is adding more things into the EIP editor and making it harder to manage the repository. For me I've wanted to go in and make a lot of little changes to update EIPs, like I would have to change the status, it would be nice if I did a lot of changes but I am hesitant to do 100 PRs because it will immediately bumps the number because I wanted to have a couple things change in a lot of ones so they can be decided individually, to have nice packaging things together, which has it’s pulling my thought process into a weird place because of trying to work within them. It's confusing like having a huge gap, say numbers are confusing I think to people like why do we have a EIP 2000 and the EIP 2150? That's like that's like more of a general reason but not like a super hard reason,  I would say not to do it. I would say it's a big deal that we figure out a way to do this, that isn't tied to using GitHub issues as it would free up tissues to be used for a lot of other things. 

**Hudson**: You mean PRs, right, not issues?

**James**: Yeah, you are actually using issue numbers. Because PRs go by the sequential including issues.

**Hudson**: Ah! That’s right.

**Artem**:  Personally, I would just turn off GitHub issues for the EIP repo and put the pull request submission behind some kind of bot.  So people will  have an interface to submit an EIP and the bot will submit a pull request and maybe give that author,  the rights to create a pull request.

**Hudson**: Yeah, that’d be really cool.  I thought of stuff like that a little bit before. 

**James**: Getting a bot will be something amazing. I thought of a proposal for having numbers  and having an EIP registry of the EIP numbers and then when I write an EIP,  I go in and I get the next number and then the editors are the ones that say yep okay because they are the ones who hit the merge button when your EIP is formatted enough for them to merge it and then  they can assign it a number and then just have it be in a list that goes sequentially. 

**Hudson**: Interesting. 

**James**: I get it’s a weird flow for me as an author to write any EIP, put a placeholder tag because, I don’t know what it’s going to be. I have to submit my PR first before I know the number is and so then I go back in after it where they make all the edits and then edit that PR afterwards to be able to get the number. It’d  be a lot easier for me is it from an editor perspectives to sit down, write an EIP, go to the EIP  registries. Oh! this is the next one , write in that number, hit merge and then that’s just ready to go. So, you apply for a number through PR to the registry for an EIP numbers.

**Hudson**:  Yeah, I don't have an opinion on that yet. 

**Alita**: Why don't we currently just use a system where we have ten numbers for each time you request a number, it just increments by one. Is that not a reliable method. 

**James**: The problem is tracking by the increment by one. because without having a way to track the current number and what's the next number then there isn't really a way to increment them. 

**Alita**: Are you saying to use a hub or proxy to manage that?

**James**: So we would have a list year of EIP numbers and the EIP and then the date it was assigned, if you want it to. So then that would be the registry of the EIP numbers and you would part of the process of submitting an EIP is registering for a number.

**Hudson**:  Okay, who  would be responsible for the registry of numbers, the editors, I guess?

**James**: Yes

**Hudson**:  I’ll  think about this more and we have one minute left if there's any final comments on this talking point.

**Artem**:  Yeah I don't know if it's like GitHub is the best solution for EIP management in general but not like I have an alternative right now.

**Hudson**:  Yeah I agree, it has its ups and downs for sure. we need front end like you mentioned to make it more streamlined.

---
Decision Item | Description
---|---
**9.3** | Discussion to be continued on EIP number registry process. 

---

# 3. Discuss EIP-1 Brainstorming Document.

(To be discussed in the next meeting)

# 4. [ZIPs reference](https://github.com/zcash/zips/blob/master/zip-0000.rst)

Partly discussed in _EIP number registry process_ discussion above. 

# 5. [EIPIP Survey](https://docs.google.com/forms/d/e/1FAIpQLSeadXscoQgrKznUOAEB_jSzNNFKHWDEFJxKH1LpDsDsC6mXpw/viewform)

Video | [55:32](https://youtu.be/59Bzw9dHIEM?t=3332)
-|-
**Hudson**: Okay I think we should wrap up then little less than a minute left if not even that so what so let's get to the other topics next time by moving them up the list. Oh the EIPIP survey, we have a new document on that. Edson, do you want to run through that. 

**Edson**:  Yeah so this is probably going to be published on this Friday.  It's in the telegram I can post it in the [chat](https://medium.com/ethereum-cat-herders/the-eipip-roadmap-cabe41fdb908) it just summarizes the results in the form of questions. We’re almost done with creating EIP process status separate from the hardfork process. We could start formalizing the hardfork process and then after we finish that then we go to questions in part 1 and then we could just choose which questions to go for as topics for these discussions. Go through the article if you’ve not already. It will be public on Friday.

---
Decision Item | Description
---|---
**9.4** | A medium blog to share final EIPIP survey report will be published on Friday. 

---

# 6. Review action items from [previous meeting](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20008.md)
(Not enough time to discuss)

**Hudson**:  I thought this was a really good meeting. I'm really excited about the progress we've made and the next meeting is going to be June 17th,  I believe. Everyone have a great day or evening. Thank you !!

---

# Annex

## Attendees

- Brent Allsop
- Edson Ayllon
- Hudson Jameson
- James Hancock
- Jim Bennett
- Joseph C
- Pooja Ranjan


## Next Call

Wednesday, June 17, 2020, 15:00 UTC.
