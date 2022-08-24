## EIPIP Meeting 61 Notes
## Meeting Date/Time: Wednesday, July 27, 2022, at 14:00 UTC
## Meeting Duration: 1 hour 30minutes
## [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/161)
## [Audio/Video of the meeting](https://youtu.be/VpL4bwu6_sc)
## Moderator: Pooja Ranjan
## Notes: Alen (Santhosh)

## Decisions Made / Action items
| Decision Item | Description | Video ref |
| ------------- | ----------- | --------- |
|61.1 | EIP w has been added as a required check. And if there is a problem, if there is something very difficult to do, Sam, perhaps you could assist them in making it easier. So we're not stuck, and the bot isn't stopping things. And we can discuss it further at the next meeting. | [8:45](https://youtu.be/VpL4bwu6_sc?t=528)|
|61.2 | For the non-normative texts in the EIPs, action would be to just change editor behavior and maybe change EIP one, decision to be taken in the next meeting| [19:00](https://youtu.be/VpL4bwu6_sc?t=1144) |


## Intro [0.13](https://youtu.be/VpL4bwu6_sc?t=13)
**Pooja Rajan**
* Welcome everyone to EIPIP meeting 61. I have added agenda in chat. The first item listed here is removing eipv as a required check, and adding eipw as a required check, Sam, we have managed to move it to a Ethereum depository and currently both are working or was there action needed? 

## Removing eipv as a required check, and adding eipw as a required check [2.15](https://youtu.be/VpL4bwu6_sc?t=136)

**Sam**
* Yeah. So, so right now, eipv is the required check. It is running. and I I'm just proposing that. We remove that and switched to EWS are required. Anybody object? No. 

**Pooja Rajan**
* Okay. And Gavin does not have a microphone in the chat mentioned I'm in favor of that. Okay. As next steps we supposed to do what it is just to be. Okay. Thank you. So that is done. Moving on to the biggest section of this meeting today, there are some, GitHub issues and pull requests that I have collected and added here for discussion. Some of them were suggested as a comment to this agenda and some, I found it in the repository and I have tried to order them based on their number. The first one is ethereum/EIPs#5265. It is to include superseded status and superseded by any thoughts. 

**Sam**
* The, the superseded discussion is interesting. because right now we have withdrawal reason and I think that that can cover it, pretty well, but, I'm open to other people's opinions too. 

**Pooja Rajan**
* If I remember correctly, sometimes a good, it was decided that superseded should not be there anymore, but is it just a change preamble section? Okay, fine. I got it. Okay. there is an update that eipv is removed and EIP w has been added as a required check. Thank you, Matt, for that? Any other thoughts from any? Yeah, please go ahead. 

**Micah Zoltu**
* Is he EIPw ready for being a required check? 

**Sam**
* I think it is, but that's kind of why I brought it up on the meeting instead of just changing it. So if anybody has any objections, we don't have to do it yet. 

**Micah Zoltu**
* It's pretty strict. which I generally like, I'm a big fan of it overall. I'm just a little concerned that we may end up having to override it frequently compared the EIPW. I don't, I don't have a good answer for this because either we have a very strict, so it's super useful, but we have to override it more often or we loosen it. So it's not particularly not as useful, but it means we don't have to override as frequently. 

**Sam**
* I can downgrade some of the particularly strict checks to warnings. that way they still show up, but they don't block the merge if we'd like, if we want something like that. 

**Micah Zoltu**
* Yeah, that, that may help, the other option. And I don't know, this may be nontrivial and if so, feel free to tell me to go pound sand. but it would be cool if we editors could like somehow comment on a particular check and say, this is okay, or accept or go away. But just for this one thing, Yeah. 

**Sam**
* I can look into that Overall though. 

**Micah Zoltu**
* I'm quite happy with it. Like it does check a lot of things that I was previously manually checking. And now I just tell people, go all the bot, come back when you're done. I kind of on the topic of the bot commenting so much, I kind of almost wished the bot would comment after the person has managed to clear all of the things, rather than because like every single person has errors, like a hundred percent of time. And so it's useful to have the bot, tell the person, Hey, by errors, go look. But for me personally, I would like it to receive notification when the boss says, Hey, this person finally fixed all the errors. It's time for you to go look at their PR at the moment. I basically just every single time I see someone comment, if I don't see the bot reply to that, then I go check. But oftentimes it's just, I'm faster than the bot. And so they still have a bunch of errors. I don't know how other people feel. I know, Kevin prefers less bot comments. 

**Sam**
* Yeah. I think it'd be like, I want to figure out a way to signal on an EIP generally, what an editor is required. so that might be like putting a label on it when all of the checks are passing or something like that. So, I'll add an issue for figuring that out too. 

**Pooja Rajan**
* There is a comment by Gavin here. How about EIPW get ordered in by multiple editorial approval. And the other one is how about only running EIP bot when all other checks have passed? Okay. So are we, sounds, commentaries? Yes, that could work. So are we going to make it mandatory right now? And the condition that it will only be running when all of the checks have passed, like deciding the level of precedence. 

**Micah Zoltu**
* If I understand Matt's comments, it's already marked as required. 

**Pooja Rajan**
8 Right.Is that any precedents, like, even if it is marked as required, will it go, does it it's like, there will be bot number one, going first, bot two going next, and then we can decide, and this EIP part will go.

**Micah Zoltu**
* Oh, I see.no, currently they all run simultaneously in parallel. and really we only, we have, so we have the auto merge bot that basically just checks and comments on who needs to approve a thing. And then we have the EIPW, which does everything else. the EIP bot does do a handful of other things, but, it doesn't actually come up so much, very often. So I think having them in parallel, I think is probably the best bet. Oh yeah. Happy bot is the one that requests editors. Jen, I think having them in parallel is appropriate here. It makes it, so it gets people get the information they need as fast as possible. 

**Pooja Rajan**
* Right. so, just for it, clarity offer the decision here related to this particular issue. Are we okay to have it enabled? Although it has already been enabled by Mac and whatever issues will come up, Sam may be able to help them fix it. And we can revisit this in the next meeting. 

**Micah Zoltu**
* Oh, wait, maybe I, maybe I misunderstood what Matt said. I'm looking, it doesn't appear the EIPW is required right now. EIPw still is. Did you set it somewhere different than I'm looking at? 

**lightclient**
* I said it in branch protection. 

**Micah Zoltu**
* Yeah. Branch protection rule for the new one. Oh, sorry. I saw EThW validator and I just ignored the Bellevue about, Yeah. 

**lightclient**
* I mean, it looks like a V 

**Micah Zoltu**
* EIPw elevator as what I saw. 

**Pooja Rajan**
* Okay. So yeah. people documenting notes, EIP w has now been added as a mandatory check. And if there is any issue, if there is any very strict to do, Sam, maybe helping them make them easy. So we do not stuck and bot does not stop things. And we can revisit this in the next meeting, moving on as we were discussing 2.1 that was proposal to include superseded status by superseded by is that anyone in this group of presently? I think that, it is, it is something that can be considered and that has to be changed in EIP1, I believe. Right. I mean, is there any significant use of making this change?Is that I'm trying to put this question

**Micah Zoltu**
* As I mentioned in the issue, I'm not a fan of it, Personally.

**Pooja Rajan**
* Anyone from the editor's group is strongly in favor of this proposal. I don't see the proposal in this meeting. Yeah. There's not a hearing this meeting so I can let it be there. And maybe we can expect some more feedback and comments from other EIP editors if they have there any strong feelings, either in favor or in against. So we'll keep this issue open. 

**lightclient**
* It relates to, sorry, Serious. Oh, sorry. Okay. 

**Pooja Rajan**
* Yeah, no, no relates to will, will be the next one. Yeah. So I was just talking about superseded by superseded by so yeah. there, there is a request to change in the name of, one of the headers in PMBOK section. That issue number is 5265, 

## Ethereum/EIPs#5274 [10.39](https://youtu.be/VpL4bwu6_sc?t=638)
**Pooja Rajan**
* Moving on to the next sub-item. That is issue number 5274. It is the proposal, for EIP preamble include, relates to as an optional feed. This is by again, by the same user. I don't see him on the call, but any strong favor or any discussion needed 

**Micah Zoltu**
* I don't feel super strongly on this one.my personal general preferences is that in my experience, people who referenced EIPs, gratuitously, generally would have a better EIP. Like the quality of would be better if they just didn't reference so many ifs and the act of requiring that they add them to the required field forces people to really think about the EIP they want to depend on, and it causes them to drastically limit and constrain the set of EIP. They depend on it makes their EIP overall better. that being said, like there's probably other ways to solve that problem. we could just, you know, editors can just spend more time coaching people and, trying to work through them and say, do you really want this one? Do you really need this one? You really need this one. it's a little bit more effort than just saying, Hey, you can include as many as you want, but be where you have a hard dependency on all of them. So your call, yeah, like I said, I'd like to solve that problem. This is the currently the way it's being solved. It's a poor solution, but it's really easy to implement. And, I always liked those. 

**Sam**
* I'm a fan of adding more context than less context. like I, I don't see a problem with referring to other EIPs that aren't mandatory. even if they're just interested or interesting reading. so I think you and I have different opinions there, but I also don't think we need to relate to field because like we have marked down, we can just link to things if we're related to them. 

**Micah Zoltu**
* So, Yeah. And for what it's worth, I was editing one of my EIPs today and I added a link to, if you want EIP 165. And I was like, oh, but I don't have to edit to the required section. And so I removed it, but I will admit to the texts was slightly worse because of it. I'm like, yeah, if you want in 65 would have been like a perfect example. Like I was saying, you know, I was suggesting in my EIP that authors should also implement some kind of introspection or, err face detection mechanism such as the EIP165. And so I do recognize the value and any sort of links. It's not lost on me. 

**Greg Celvin**
* The ITF for RFCs insists on a proper reference section with proper citations at the end, not just mysterious numbers in the header. So you can actually see what something refers to. And especially if an external leg has problems, you ever proper citation. So you can find other copies,even in the library. 

**Micah Zoltu**
* I don't think you have either in any libraries. 

**Greg Celvin**
* No, but they can refer to documents that if they're not online are available in professional journals and in, university libraries. 

**Sam**
* Yeah. If we were like referring to something. So just because we have geth and we have like markdown rich links, I think internal EIP references are always like fully qualified. It's, it's very difficult to have a more accurate reference section then, you know, the file name and the get commit hash. But if we did allow external references, I'm fully on board with like fully qualified references and just like you're describing 

**Greg Celvin**
* Even, even internally, it provides, it provides a title and authors, to, to put things in context.It's just a professional way to do things is to have readable. The header is a convenience for the bots. 

**Micah Zoltu**
* I feel like we could. So in the, if this was something that is heavy demand, I feel like we could achieve it in the rendered version of the page by making it so the EIP internal links turned into something that has like a little additional info on hover or something. 

**Greg Celvin**
* Oh yeah. Yeah. The same for Matt as it's used, in the published version, it says, please cite this as user our own proper citation format, but also it makes it easy to distinguish. Non-normative likes to sections. 

**Micah Zoltu**
* Again, a little off topic, I believe for the question at hand, which is the relates to field. I'd say that because we have a very long list and I believe this,

**Greg Celvin**
* I think it's a good idea. 

**Micah Zoltu**
* Like you think that we should have the requires field and the release. I think someone's mic is live, excuse me. 

**Greg Celvin**
* Yes, I do. 

**Micah Zoltu**
* Why do you think that we should have the relates to field rather than just like, it's just, it's just going to be a list of EIP numbers. Why not just have links in the document itself, which is what Sam was suggesting, 

**Greg Celvin**
* Because the specification section should have nothing but normative references, but to Mount, a reasonable motivation and rationale can, can have you're referring to non-normative references that are part of your argument, but not part of your specifications. 

**Micah Zoltu**
* I see. So would you, would you be okay with allowing, allowing non-required links to non-required EIPs in the non-normative sections? Just freeform. So like, I can just say my motivation, blah, blah, blah. 

**Greg Celvin**
* See, Yeah. Often your motivation is that this is an alternative. if you can't talk about what you're an alternative to you're floundering, making statements of fact with nothing to back them up. 

**Micah Zoltu**
* Right. I mean, I think I can probably be convinced, by Sam suggestion, that we just, and what Greg described, you know, we just, for the non-normative texts, you can link to any other EIP. I would like to retain the requirement that the status be further along than your EIP or, immutable in some way. just because we, even for the non-normative sections, I really don't want people to Lincoln DAPs that are going to change drastically and then therefore change the non-normative content. And in theory, we could have a bot check all that for us. 

**Pooja Rajan**
* So, is, is there, action needed? 

**Micah Zoltu**
* Like I see this as in the issue form, I think the action would be to just change editor behavior and maybe change EIP one. I don't know if the EIP one said anything about it right now. 

**Pooja Rajan**
* Okay. 

**Micah Zoltu**
* I would like to, can we, before we make it official, can we continue the dialogue in the issue maybe for one more week and then if no one else voices concerns or if, and after we all think about this particular solution and we can agree that it's done. 

**Pooja Rajan**
* That sounds good to me because I see the opinon are divided here. Like some of them are in favor and some of them out in against, so let's continue discussing in that issue. If we make a concrete decision on that in the issue itself, it's bad enough. If not, then I can bring it back in the next meeting and see where we are. 

**Micah Zoltu**
* Okay. And I still do feel worry that well in the ideal scenario where all the editors are good editors, the solution will be fine. I'm concerned because I see a lot of EIPs is the word where people just link to, you know, a dozen different things. And it makes the standard incredibly hard to follow and read and understand. because as Gavin said, people like to write history books and their motivation section and motivation section should be, you know, a succinct, pithy description of why this is a useful thing, not here's the history of the world and how we got here and how we're going to fix it. 

**Greg Celvin**
* That's why you put one link to the, most important textbook tells reader, go study, go study this textbook. And you will be qualified to understand this document. I kid you not there's RFCs that have a single non-normative reference. That is a, like, to a text. 

**Pooja Rajan**
* Okay. So yeah,let's keep it in the issue. We continue discussing. Let's have more feedback collected from EIP editors, and if they choose not to resolve, we'll bring it up in the next meeting. I hope the proposer also joins the next meeting because I don't find him on the call 

## ethereum/EIPs#5294 [20.43](https://youtu.be/VpL4bwu6_sc?t=1243)
* Moving on to the next, number that is five to 9, 4 8 is how should we pick EIP number? This looks like particularly interesting because there is a proposal. 

**Micah Zoltu**
* Can we come back to this one? We've got a very long list and I think this one's gonna take the rest of the meeting. 

**Pooja Rajan**
* Oh, okay. Okay. 

**Micah Zoltu**
* Number five. 

**Pooja Rajan**
* Okay. If that is, if there is any preference, I can probably go on there. Do we want to go on any particular number five? 

**Micah Zoltu**
* I saw a note skipped three and five for now, and let's come back to them. I think those are going to be very long conversations. 

**Pooja Rajan**
* Okay. So number four, Everything else. Yeah. I mean, the list is very long today. 11 sub items let's see how much we can cover. So I suggested number four is about fixed SPGX license identifier. I have added the link here. It is Three And five. 

**Micah Zoltu**
* You said, I thought I said three and five. He said, escape for Skip three, four, and five. 
* So we're skipping four entirely and we're doing three and five at the end. 

**Pooja Rajan**
* Okay. Let's move on to number six. I hope that is fine. Okay. I'm going to share the link here. Oh, skip a field. Sit still. 

**Sam**
* Oh, don't worry about it. It's just a, it's a rhyme. 

## ethereum/EIPs#5272 [22.00](https://youtu.be/VpL4bwu6_sc?t=1336)
**Pooja Rajan**
* Children's Okay. Number six is about, no, I think I, I mistakenly have added the wrong number. The number is 5, 2 7 2. It is about add RSA information information to him. 

**Micah Zoltu**
* Yeah. so the, the TLDR, my position at the moment is that I don't have any problem with Lincoln to RFCs. my problem is the door that it has potential to open, because we actually do get quite a few people who want to link to their new standards, repository. It's got like free standards in it and they call it a standard repository. I mean, every standard report positive, it has to start small. And so I get it. but like some of these repositories I doubt will survive the year. Like they do not have the longevity that RFCs have, for example. And so my concern is that if we open the door to, okay, these standards repositories are allowed, these are not, we're opening the door to people to argue that, oh, my center's repository should be allowed as well. And we do get people suggesting this, like, they're like, well, you referenced RFC 2, 109. So that's a standard repository thing, which wanting to reference mine as well. And so if we had like a strong mechanism, like a good shelling fence for saying, you know, preventing this from happening, then I would feel a little better about RFCs. In which case I wouldn't care whether we linked to them or included them or whatever. The one, the reason I do like the current suggestion of including the RFC as wholesale is because this allows anyone to include any standard from any other place, as long as they're willing to copy it over, we'll sail into the repository and they're allowed to, whereas if we link to it, now we have to get into the fight over, you know, what external resources are people allowed to link to and what aren't right now, the very simple, none is the answer. And, we can give that answer out very quickly, very easily, and we can stick to it and we don't have to fight with people. Whereas if we start saying some, then things get much harder Given you have, oh, sorry. He's not having microphone Require that any standards that we link to must be around for three years and Matt suggested 30. I think I'd be okay with 30. Like if you've got a standard repository and still around for 30 years, I mean, that, that's like what, RFCs maybe a couple other from the I, the ITF and not much else. And so it does give us a pretty nice, thing. And to Sam's question, what does a shelling fence, a shelling fence is a, yeah, a line in the sand. It's, it's more specifically, it's a thing that you can reasonably believe that once you cross some blurry line, when you get to this thing, it's very clear that you have a new line that you will not cross. And so it's, it's basically, if you imagine a slippery slope, a shelling fence is some fence that everybody can agree on where everybody is, everybody involved in this process, that it will be very clear when you cross that layer. 

**Pooja Rajan**
* So, is there a general consensus of letting it task for like, let's go ahead with this proposal and if the information and keep it there for a few years. 

**Micah Zoltu**
* So I think the disagreement right now is there's three options. One, we continue with the current policy, which is, do not allow any external links whatsoever to allow external links to some subset of things. And then if we go to, we have to define what that subset of things are. Option three is we allow people to import external standards into the repository as assets, and then we don't care where they came from as long as they are important in the repository. So that way we can be sure it's I mean, has anybody actually done it?  Me?Okay. So Sam has allowed himself to do it. So yes, I guess we do collectively. yeah, I mean, this is why this is coming up because you know, people are wanting something here and Sam's is one such person, 

**lightclient**
* I guess I'm on board with allowing RFCs and for the other standard standards, just importing them. Because I think that the amount of standards people want important are extremely low. 

**Micah Zoltu**
* Really. I find, like, I feel like it's once every couple of weeks, I guess someone that will spend like an hour arguing as me over why their standard is acceptable to include in the eip link to Outside the chain agnostic standards. Maybe I'm, maybe that's a bias making me think it happens more freely. 

**lightclient**
* I feel like that one does come up somewhat frequently, but beyond that, I haven't personally seen many. 

**Micah Zoltu**
* So regarding, Greg's suggestion of just common law or precedent based law. my two problems with that are one, and we'll discuss this more later, but the whole credible neutrality thing, it's really hard to like when you have just say editors decide, if the editors are all totally honest and on the same page and agreement, and they align with the ethos of the broader community and that works great. The problem is, is there's no way to guarantee that as is the case in any given point in time and from a credible neutrality standpoint, it's hard to maintain that over time because eventually you get, you know,some editor will join and they're an honest person and they want to help, and they are being helpful, but they just don't agree on what is acceptable. And, when that happens, now we have like, a change in the ethos and that change may go in the direction of the community as a whole, or it may go against the direction of the community. And so now, if it goes in the direction against the community, now you have lost some incredible neutrality with, with the community because of that. And well, and just, this is something that, whereas if you have hard and fast rules that are just written down and they're just applied uniformly to everybody, then it's much harder to go down that route of no. Okay. Why is this allowed, but not that allowed. And then the second reason I'm not a huge fan of it is just because we historically have been very short and editors. And I will admit lately there's been a lot more active editors. And so maybe this is not as big an issue as it used to be. but we have also gone through times of lots of editors and then they'll disappear.but we have also gone through times of lots of editors and then they'll disappear. And so hopefully you'll forgive me if I assume that some subset of the people in this room right now will be gone by the end of the year. And I will be back to the only active editor. And once again, having to do all the work myself and in that scenario, I do not want to be getting engaging in debates and discussions with every single author that wants their thing. 

**Pooja Rajan**
* So currently this is in the form of pull request. There is a request to make some changes over there. Is it fair to understand like, this merge will take place if we have like, all a disapproval or maybe in favor of three or four? 

**Micah Zoltu**
* So if we can get all the editors to agree, then yes, it will. It'll happen. as soon as we all disagree, I'm at the moment, I don't think we have full agreements across the board. Everybody has kind of a slightly different version of what they want. And so we're trying to hammer that out and resolve it. 

**Sam**
* So, so my understanding is that right now we can put whatever we want in the assets directory, as long as it's allowed to be redistributed. Is that correct? 

**Micah Zoltu**
* I mean, my, my personal policy, which I don't think is written down is everything must be CC zero licensed, which basically forbids external standards. I know that it's not everybody follows the same policy. I'm more of it. And it was one of the many things that we don't all agree on as editors. 

**Pooja Rajan**
* There is this question in the chat 

**Micah Zoltu**
* Gavin's suggesting and merge as is changed later. My general preference is, is when there's disagreement amongst editors to prefer to go with the status quo or previous rules rather than change them just as they kind of default rule. I mean, I know that prefers conservatism versus liberalism, but the opinion that's valuable in cases of disagreement. 

**Pooja Rajan**
* Yeah. This is an interesting comment, merge if something as much as they likely to stick around. So let's, let's keep it open and, we'll collect some more feedback from other EIP editors and you can see, we can have an anonymous deficient. That would be the best case scenario. If not, then we can try to maybe make some changes in that request and come to a general agreement. Anything else anyone like to add before we move on? 

## Reference ERCs by ERC-X #5273 [32.00](https://youtu.be/VpL4bwu6_sc?t=1975)
**Pooja Rajan**
* All right, moving on to the next item listed here. This is, this particularly is very interested because we have been, planning to discuss this for past few meetings now that we have at informa pull request. I believe it, it will be easier to maybe discuss and, come on a decision. It is about how do we write ERC and EIP, especially for documentation purposes. We did make one change on EIP. One that wherever it was written as ERC for documentation, we did drive it as EIP. but this pull request is to suggest that it should be written as ERC, any thoughts people would l ike to share. 

**Sam**
* So I guess the only thing I'd like to mention here is that it is harder to enforce that ERCs are written as ERC and EIPs are in a eth, like in, in EDW. I'm not opposed to doing it, but that is just a point against it. 

**Micah Zoltu**
* Do we not currently, does the EIPW not currently have code to follow the link and parse the text with the other side? 

**Sam**
* Yeah, It, it does. It's, it's just more complicated than the regex that it has now. 

**Micah Zoltu**
* Sure. But it may, it's not like a, if you already have the code for following links and parsing the metadata, then it's not as big of a jump as if you didn't have that already. 

**Sam**
* Correct? Yeah. 

**Micah Zoltu**
* Okay. But, but I can appreciate that. It's still notably more work than a regex I'm in the winter. I'll go with whatever direction anybody else wants. 

**Pooja Rajan**
* I think one important, feature change that we discussed earlier as well, like if this has to be done, they might want to like change the header that is generated for every EIP, because currently it is written as EIP, no ERC, no code, no networking, no interface. It is just EIP followed by the number. 

**Micah Zoltu**
* So I think that at least for this initial change, if I understand correctly,it would just be changing the links, relative links people put in their EIPs, it would not be changing anything else. And that being said, if we did the change, I could definitely see wanting to do a follow up change that also maybe edited the rendered page and, whatnot. And then I do not think we should change the file names though, because that would be a huge headache. 

**Sam**
* Yeah, definitely no changing the file names. And I think we should keep EIP, colon as EIP colon in the preamble. 

**Micah Zoltu**
* Yeah. 

**Pooja Rajan**
* I may be wrong here, but for some reason it feels to me, if we are not changing the head and we are making this change in documentation, we are inviting confusion in terms of EIPs. And ERCs again, like earlier, we agreed that the ERCs are standard track proposals are standard deck EIPs. And that's why like all other standard track EIP is it is also documented at least a documented as the EIP and people are free to call whatever they want to call it. They want to call it that ERC 20. It's fine. But it is documented as EIP 20. 

**Micah Zoltu**
* I think that's fair. I can see the argument that if we're going to do this, we should do it all at once. Meaning I still don't think we should rename the files and I don't think we should change the, the number adopt. but I can appreciate simultaneously updating the rendered page to render them differently, Matt and choosing to be proponent. And you have microphone. 

**lightclient**
* I think that we've been referring to ERCs for a long time. And I don't think that we should unilaterally decide now that everybody needs to start calling them EIPs. 

**Micah Zoltu**
* So I believe haven't, we always required them to be EIP dash, blah.And in the texts, 

**lightclient**
* I've always required ERCs to be ERC dash, but I don't think it was codafide in EIP 1. 

**Micah Zoltu**
* So your belief is there is some, some volume of ERCs have relative links that are to ERC, yada, yada, 

**lightclient**
* They say ERC dash number, and then they linked to eip-number.md. 

**Micah Zoltu**
* I keep missing the first half of what you're saying. I think your Mike's cutting into late. 

**lightclient**
* Maybe the zoom is bugging. there are a lot of ERC links and there ERC, the different EIP in the ERC category that start ERC dash number and then link to eip-number.md. 

**Micah Zoltu**
* I see. So the link itself is to EIP, but the text, the all text is ERC in much VRCs The policy has generally been strongly prefer ERC dash number, but I wouldn't die on the hill of someone's to calling it EIP dash number, 

**Pooja Rajan**
* Generally speaking, I feel like this would be an easy, convincing point for people who are calling.I it's. I know the community is very big, very strong, and they have their own mind or decide and call whatever they want to call. But when an author is documenting a proposal and he or she is trying to refer to an ERC category proposal, he is, writing ERC dash 20 and directing it towards EIP dash 20 dot M D. He knows that it is called as EIP 20. So it may be way easier to convince that you see it is the AP 20. Let's call it EIP 20, and let's start educating people. ERCs are started track EIB is category ERC, but that's, again, my argument, my thought, is there any suggestion how we can collect more feedback and how can we come up with the solution that we can start educating people? 

**Micah Zoltu**
* I propose the last man standing gladiatorial and gladiator match between Pooja salmon, Matt and Gavin, who else seemed to care? 

**lightclient**
* Will you host it All hosts? 

**Micah Zoltu**
* It sounds like Tim wants to join the ring. 

**Pooja Rajan**
* One thing that we can do is like, we can start sharing this pull request and ask more people to comment and feedback how they would like to see it be it's about community. So maybe it's beyond editors only, and we can provide in more community though. I don't know how much is the reach, but does that sound like a reasonable solution for now? 

**Micah Zoltu**
* I mean, I'm okay with the punchiness till later. I'm always hesitant with inviting the community because the very amiable amorphous set of people and, it can very easily lead to brigading like, you know, someone, that's got a lot of Twitter followers tweet, Hey, everybody go comment on this. And now all of a sudden you have a hundred people agreeing with that person. but none of them post posing, you know, new arguments, they're all just parroting what their thought leader has told them to pair it. 

**Pooja Rajan**
* It looks like an attentional debate.It has been there for a very long time 

**Micah Zoltu**
* As we move on and potentially skip some of these other ones. We have time for those two big ones. 

**Pooja Rajan**
* Okay. You can move on any particular number that we want to pick today, next floor, because I know we have only Does. 

**Micah Zoltu**
* So I think several of these are yours. Gavin, remove old EIP, 20 file disallowed smart in the EIP title and description, centralized discussions to, and last call addition with changes in standard. So I think for, we can skip number 10, the person who wrote that I don't believe is here. And so we would just be agreeing with ourselves. 

**Pooja Rajan**
* Number eight, I think that's what the Gavin is suggesting here. Yeah. 

## Remove old EIP-20 file #5302 [40.49](https://youtu.be/VpL4bwu6_sc?t=2449)

**Sam**
* Oh, plus one on removing the, the EIP 20 file. 

**Micah Zoltu**
* I'm fine with it. Anyone want to keep the formerly named EIP 20 file? That's just currently redirect.It's been there for like four years now. Okay. Let's, let's get rid of it. That was easy. so yeah. Does anyone passionate about talking about the word smart and titles and descriptions today? If not,I propose we skip it until next week.

**lightclient**
* I propose we close it. 

**Sam**
* Yeah. I don't see it enough to think it's a concern. Like we look through quickly on the apprenticeship meeting, where smart was entitled and it was almost always paired with smart contract except for one. And that one was just a bad title, so I I'm okay with allowing it, but we should just be more careful and forcing people to have a descriptive titles. 

**Micah Zoltu**
* Okay. I'm fine with that. for the record though, I do think that if you're saying the smart contract,you should just say contract, I think that that's redundant to say smart contract when There are at least three EIPs that also have legal contracts in them. So, Okay.We can talk about smart time, but I'm fine with, not standardizing on that. 

**Pooja Rajan**
* At least not making an official, There can be some exception for that and they discuss it. Maybe as I mentioned that in the EIP of condition meeting, weekend, I mean, it can be in it's it is like not good at all. Probably it can be documented. 

**Micah Zoltu**
* Yeah, that's fine. Like I'll probably still tell people, please don't use smart, but I'm fine with this not being a rule that we actively enforce. And if other editors want to allow smart and the title IX smart contract,I'm fine with that. Oh God. That was fighting words mad. So I propose, we move on to number, I'd say number five, number three and five are more or less the same conversation, but I think five is one that we need to resolve sooner rather than later. Whereas three is when we can delay,if we need to. 

## Renumber EIP-5000 to eip-5159. #5270 [44.30](https://youtu.be/VpL4bwu6_sc?t=2666)
**Pooja Rajan**
* Alright, I'm going to share the link here. And we did have a little bit down on agenda, so I know there had been discussion going on on this discord. 

**Micah Zoltu**
* I'm surprised it hasn't spilled over into glitter yet, or maybe it hasn't. I just don't follow the right people. So for those listening in, I will try to describe the situation, as fairly as I can, feel free after I'm done to correct me on all the ways that I am. My biases are showing. the, I think the crux of the issue to skip all of the, what led to this. I think the crux of the issue from my perspective is that there's a disagreement on whether editors should be, whether editors should be given special privileges to repeat contributors and well known members of the theory of development community, or if we should be treating the random stranger who shows up off the street and submits an EIP exactly the same as long time core devs like metallic. basically everything that we discussed has led me to inclusion. I think that's the, the core disagreement. I'm in the camp of, I think we treat everybody equally. if metallic shows up, I'm probably gonna treat him more strictly or when he shows up, I treat him more strictly than I treat other editors, specifically, because I want to make it clear that no one gets special treatment.I don't care how important you are. Things if you're in community, you get treated exactly the same as the Rondo with a brand new GitHub account that shows up as long as you're not a spammer. I believe, and I'll let Matt jump in here in a second. but I believe Matt holds a position that we should be kind of rewarding and favoring and, giving nicer treatment or better treatment to the, longtime attributors, you know, like, and this is before like I've conflicted with Peter on a number of occasions on this cause Peter hates the EIP process and he hates it. When I tell him to do, you know, the busy work that every EIP author has to do. and I keep telling him, no, you have to do this busy work and eventually handed off to Tim. And that worked, worked great because Tim just did the busy work and we got it through pretty quickly. but this isn't the first time this conflict has come up where longtime contributors want preferential treatment or special treatment or, you know, to, for things to go a little smoother for them than it has been everybody else then not have to, you don't have to follow the rules like everybody else does. and I'm pretty strongly against that. And, finish the reason I'm against that is because I do think the EIP process is part of if your team's governance process. I think it's very, very important that if your team's governance process remains as credibly neutral as possible, and one way to remain credibly neutral is to make it very, very obvious that there is no favoritism. There is no old boys club. There's no insider deals. There's no because everybody is treated exactly the same.We can be confident that there's nothing underhanded going on. There's no one trading favors behind the scenes because everybody follows the exact same set of rules. 

**Greg Celvin**
* Let's, let's flip. The bot is for the bottom is science the number, and it doesn't matter how we feel about it. 

**Micah Zoltu**
* Are you sure? So like there are essentially the second, the second thing that's issue, number three on our agenda here is how can we resolve this very specific problem of EIP number assignment? But I think the broader problem is that the editors currently don't all agree on whether we should be giving preferential treatment to the core devs and longtime contributors, or should we treat everybody the same? And I think even if we solve the numbering problem, we're still going to have this problem crop up somewhere else. And I think we should resolve that. 

**Greg Celvin**
* We can't resolve everything with a policy upfront. If we have a discussion later, we have a discussion later. 

**Micah Zoltu**
* Well, I mean, so th this is the discussion later. Like that's what I'm saying. 

**Greg Celvin**
* We need to have In the past, in the past, when we run into these walls of credible neutrality, we've simply let the bot do it. So we simply get out of the argument. It's just the way it's done. 

**Tim Beiko**
* Right. I think, I think because point though is like, people have like abused, you just kind of a strong term, the bot, right. And not that's like, and then the question is like, does that matter if like, okay, the bot has said you get the next issue number. Well, if I opened a thousand issues, they get the next round, but you know, a thousand number,like what do you do in that case? 

**Greg Celvin**
* The person, It was that big.You block them Every block, Alex, I don't want to talk about what already happened. It's gone, it's done. We have a leg inside numbers. 

**Micah Zoltu**
* Every time it happens, we have to actually address it or it's going to happen. This will happen again. 

**Greg Celvin**
* If we do nothing, We've already addressed it, we've gone over and over and over it's addressed. 

**Micah Zoltu**
* No, we still have the, is still open. Alex still has the number. If, if anybody does this again, they will face the wrath of that's reasonable enough. Okay. 

**Micah Zoltu**
* So I said that the last time, and now is the time for the wrath and Alex, because he's facing the wrath. I don't think, but I Think We can't just keep kicking the can down the road every time it happens. 

**Greg Celvin**
* Yes, we can. 

**Micah Zoltu**
* I mean, okay. So yes, we can keep kicking the can down the road. I don't think we should keep kicking the can down the road. 

**Greg Celvin**
* It's the lightweight cam is steel toed boots. 

**Micah Zoltu**
* So I would like to know, do you believe that I represented your, our disagreements? Well-matched like, do you feel like that's accurately represents kind of, where are our misalignment is? 

**lightclient**
* I guess I, I didn't, I don't really see it as preferential treatment because to me it, their contributions more weighed into like my editor, editorial judgment of whether or not they were standing, the repo, everything else was followed according to EIP one, and it's not like they were breaking any kind of rules. And I was allowing them to break rules. There's no rule against sniping and the IP number. And, you know, if somebody else came in with that number, maybe it would have been more likely that they created that spam. But I just feel like given my experience, working with them in the past, that's not something they would do. And so I felt that, you know, they have followed all the, the standard procedures. And so I don't think it's the same as like Peter wanting to just move something to final, which I like. I agree. I, I, I think that everybody should follow the same process. I just think the authors of 5,000 deadfall the correct process. 

**Micah Zoltu**
* So I think what, what you described there, I think is I think what you described aligns with my feelings situation, because my feeling is is that if your, familiarity with a particular author comes into play in our decision-making, then it by definition is not incredibly neutral process any longer. like if you're saying, well, you know, I know Alex, I know him personally. I we're friends, you know, I work with them.I have a history of, 

**Tim Beiko**
* If you can know them as a contributor, to a Ethereum them, right? Like I'm not friends with Alex. Like, I mean, we've met a few times, but like, I know who he is. Cause I know he was the guy who works on all these EVM EIP's and like, he does really good work and I'm not an editor, but if I was, I would be like willing. It's not even to like accommodate him. Cause it's like, I think I agree with Matt that like, he, he generally followed the process, but it's like, I don't know. I wouldn't be willing to like, not make the process explicitly worse for them because they just do good work. And this is not like, yeah, it's not because I like Alex particularly, or don't like him. It's just like, he's like a valuable contributor and Right. 

**Micah Zoltu**
* And so I agree that he is valuable contributor. my concern is, is that for an outside observer, what they see is a different set of rules being applied to different. 

**Tim Beiko**
* If you already have like 10 EIP's since like 2016, which I think, I think it's reasonable. 

**Micah Zoltu**
* Sure. And so that's why, that's why I think we have an ethos misalignment like you and Matt think that's reasonable. And I don't want to claim that. I believe that mine, my view on the credible neutrality here is necessarily right. I think that the disagreement is, is that you guys think that is an acceptable behavior. And I think that is unacceptable behavior. And we need to come up with a cohesive vision on what is acceptable behavior for me, I get it. Or should we be looking at the contribution history? And you know, there's a few authors who have submitted 10 EIPs in the past and I really would rather not give them any for a fun stream. I think their EIP are terrible. And this now it comes down to like, am I preferring this? Is it just, if you have, then you get treated better, but do or this

**Tim Beiko**
* Any rough consensus system is going to end up like that.It's like the same thing. He has All core devs, you know, like another way to like frame, this would be like, why do we let you make us speak on All core devs? Right. Like people could just say like, oh, you know, he's not part of a client team. He doesn't like, he shouldn't be here and we don't have like a soft rule for that. You know, it's like, generally you make good contributions. And people kind of recognize that then like, you know, you get like preferential treatment relative to, I don't know, some random person on the discord who shows up. and like, I, I don't know that we could draw a line there. And I think if we drew a line, it would just be bad because it becomes like, I don't know, you, you just can't like manage just as like a pure bureaucracy, because like people's idiosyncrasies kind of end up, I don't know, in different places. And if they're good contributors, you need to accommodate that to some extent. And some people want the nice EIP number. So I don't know, especially for something like for something like that, where it's like, you know, I like very soft abuse of the bot. You could say, I that's kind of why I see it as a non issue.I guess if Alex had like spammed a thousand issues, you know, 

**Micah Zoltu**
* And then Alex immediately sniped the problem is, is we can not, the only reason we don't believe Alex family issues is because we trust Alex. And I really don't like the idea of saying, I trust that guy, even though all the symptoms looked like he did something very bad that would have, should have, we should have gotten them banned, even though it looks like that I trust him. Whereas that other guy who did the exact same thing, I don't trust him because, you know, I don't have a history of them. That's where I get very uncomfortable. Okay. 

**Tim Beiko**
* But we trust people to be EIP editors, right. It's like, it's kind of the same thing. Like I trust that you're not going to come and like mess up the entire process tomorrow. Right? 

**Micah Zoltu**
* Sure. So I have the ability to mess up the process, but my hope would be that if I did mess up the process, I would get kicked out and everything would be re re reverted. And so in this case, you know, someone came in and mess with the process potentially. And so the, you know, should we allow that? Should we let it stand? And this is where I don't think we should. 

**lightclient**
* So I mean, what are you afraid of happening? Because in my perspective, like the EIP numbering is not very high on the list of important things related to the Ethereum. 

**Micah Zoltu**
* I agree. I agree with that. when I brought this issue up in initially, the, the number was not actually the big deal. the, the bigger issue was that I saw that Sam told an author to remember their EIP, and then they refused to read number the EIP and they merged it. I'd actually noticed that Alex was a co-author at the time. And when I initially saw the issue and then you merged it, and I assumed initially that you just didn't notice Sam's comment and you merged it without realizing that the author didn't respect, Sam's comment or respond to it or anything like that. So I was like, Hey, this is just a mistake. You know, this author is, is maybe, maybe they missed the comment from Sam or they forgot about it or something. But then the more I dug, the more, it was like, oh, wait, that was all there. I definitely saw the comment from Sam because I sat there for three months and then I dug some more. And it turns out that, you know, the author reached out to you privately and now, so now things are not happening in public, which is what has happened every other time that this has occurred. It's been brought up in public. And so like this, the issue that triggered this all was the EIP number sniping. But by itself, that was not that big of a deal. And I probably wouldn't have even, I would have pushed a little bit to renumber it, after the fact. But if that was the only issue someone got away with this night, people have gotten away of Snipes before we know of several. I probably would have let it slide. my bigger, far bigger issue is how the situation was handled and, who was involved with it. again, the private discussions, it feels like it's not how we have historically handled any of this. we have, we had an author, an editor who specifically told the author to change the number and there's no public discussion after that. It just like these are the things that are, the issue is because to an outside observer. And this is to answer your question. My mind, my problem here is to an, until observer, it looks like you have a couple of EIP editors. You have an EIP editor, who's an author and the IP editor who, you know, follow the normal procedure of renumbering Snipes. And then yet another EIP editor who just merged it blindly, like without respecting that first editors, comments and at best, you know, it looks it's sketchy looking. And so from a credible neutrality point of view, not arguing that anyone's non neutral here just from appearing neutral to the public, this is not a pure, like a neutral process. Listen appears very much like our traditional governance institutions where backroom deals happen and people engage outside of the public view, make decisions, and then just apply them without any public discussion or public discourse or anything like that. And so that is kind of the bigger issue that end again, th this ethos misalignment, where I think that, I guess there's really two issues here. There's the ethos misalignment where some of us think that we should be giving preferential treatment like Tim and Matt to longtime editors or long time authors and contributors. And there's a separate issue of this, you know, that the whole thing occurred behind closed doors. We don't know what to the average external person, we don't know what happened. What was in that conversation who was in that conversation? Where did the conversation occur? You know, what, what was exchanged? Was it just, a request to an, a, an okay. Or was it like some deal was made? And this is stuff that no one can know because it wasn't done in the public. And so these are the issues that the numbering really doesn't matter. I do think we should solve it to kind of avoid this class of problems. Cause we've been getting more and more, sniping attempts lately. but those that the numbering is really not the issue in my opinion. And that's not what I'm worried about. 

**lightclient**
* I think a lot of the conflict arises from the fact that I treated the situation pretty nonchalantly because it was about something that I felt was extremely unimportant, like the number of an EIP. And so I, you know, wasn't thinking as seriously about like, what are the implications of doing this or this or that. And I do agree that, you know, to me, like the biggest mistake was just not saying, Hey, yeah, I see Sam renumbered it, but I think it's okay to keep it like this. If I would have posted that on the issue, then I don't really think that there would have been an issue, you know, a really a problem because I feel as an editor, I have the agency to override another editor. And maybe in the past, we've been like a little bit more explicit about, you know, how, or when, but we have on many times in the past, you know, overwritten other decisions. And typically it's like followed by. I'm not going to stop you or like, I'm not gonna improve this myself. So somebody else can improve. It that's happened like many times in the past. And it just happens that Sam and I have worked together in the past and we talk somewhat frequently and I hop in to ask him, Hey, is this going to be something that you want to stop me over? And he said that it wasn't, he didn't want to fight about it. And if I would have posted that on the issue, which would have been the right thing to do that, I don't really think there's a problem with the situation. 

**Micah Zoltu**
* So I,personally agree with that. So I think if you would've posted on the issue and Sam would have pushed the response to the issue. and I think it would have been less of a problem though. most likely if you were to post it on the issue, I would have replied and say, I'm definitely not okay with this. And then we would've had to have a discussion and, you know, engaged and have a longer, this longer debate that we need to have about numbering. I still feel though that's so that would, that would resolve the half of the issue, which is the, the, the decision was made in private. So, so that is one problem. I don't think we should, as editors should ever be making decisions in private, like everything should be done in the public to maintain our credible and reality. And you're right. What you described would have addressed that half of it. I still don't think it addresses the issue of it's Alex. So it's okay. I don't think that should ever be an answer to anything that comes up in the EIPs repo that it's so-and-so so therefore it's okay. Like, or it's so-and-so so therefore we can trust them. I don't think that's how we should be doing business for any big issues or small issues. Like they should be. Did this person follow the rules? Would I apply this rule evenly, even handled lead to everybody? And I think this is where, you know, Tim and Matt disagree with me on, should we be treating everybody equally or should we be giving preferential treatment to long time contributors? And so I still think even if what you described happened, we would still need to resolve that problem. 

**lightclient**
* Because I do think that's going to come up again and again, I mean, I personally don't think I've renumbered any EIPs, so I'm not really the biggest fan of the renumbering. It, to me makes it feel like the editors have to go on some sort of investigative journey to determine what is their span before, like who did the spam and it's, I don't know, just not really a side quest that I want to engage in. If it's like extremely egregious, like 25, 5100 spam pull requests or issues beforehand, then maybe we can start talking about that. Or if it starts becoming a problem where we're seeing, you know, again, like hundreds of issues then maybe, but I just don't think this is that big of a problem. If there's a few spam issues beforehand, obviously we want to discourage that. But I think it's like more the, you know, I think it's more telling that our system is kind of broken for figuring out the numbering, if you know, we're, dossing ourselves over four or five issues of spam before number. 

**Micah Zoltu**
* Yeah. I agree that we should address the number issue. there's a,this is, so if we re very briefly switch over, agenda item number three,there's several options that I think would completely mitigate this entirely. So numbers are essentially randomly assigned and don't have any control over them anymore. And then if you happen to get 5,000, you got lucky. but like I said, I, I still would like to resolve the issue of, whether editors should be treating core devs different from, I mean,how is this going to manifest? 

**lightclient**
* Like, what other ways can we treat core developers differently? Because I think that the EIP number is like a small area of a very small amount of editorial ability up as an EIP editor. I don't really know what else is out there. 

**Micah Zoltu**
* So, some examples of have been in the past and some of these, I think you and I agree on some of them, I suspect we don't, there's, Peter has repeatedly requested that he doesn't have to follow the process, so that There's no editorial Wanting to look different than us. If we don't agree on this broadly, then some editor may decide, you know, it's Peter it's okay. He doesn't need to go through the draft to review to the last call to finally, he can just skip the final, the there's one, that's much more subtle that I, again, I just want, I suspect suspected. We disagree on, I have noticed that when a Corp dev submits an EIP, it gets reviewed with like within two days and not by me, like someone else actually beats me. It's like the one time I get beaten, two reviews on the IPS is when a Cordova summits, and this is a subtle one. It's nothing that, you know, you can say, Hey, you're, you're obviously going to say bad here, but it's noticeable.I think, to repeat EIP authors who get frustrated when they see, you know, every time Alex submit something or his name's on something, it gets reviewed like within 24 hours and it gets merged like almost right away. And not just because they're there. I mean, he does do a pretty good job writing yet piece, but, it's not always it, like, there are other people who write very good at EIPs, and they take a long time to get reviewed just because we don't have the staff. And so said another small example of us giving preferential treatment to a inside group versus an outside group. 

**lightclient**
* I just don't think that these degrees of freedom affect Ethereum in any material way though. 

**Micah Zoltu**
* So they, like I said, it's all about the credible neutrality. Like I think that it's very important and perhaps this is the real core disagreement between us perhaps is whether credible neutrality for the EIP process actually matters. I believe in matters and we should be as credibly neutral as possible. Like it should be as plain as day. Like if someone goes and really digs, they should be able to find absolutely nothing that suggests that we're giving better treatment to one particular group or similar particular group. and if someone dig dig today, they'll find a number of cases, you know, where we are potentially giving better treatment to one group versus another group. And I believe that it should be impossible to find such examples of things. And so, like my process just coming from, as an example, I go through the EIPs in the order that they show up, I ignore who the authors are. I treat everybody exactly the same and that includes sometimes telling theater to go away, because, and he has followed the same process, but he else is sometimes means that I leave, you know, metallics PR to much later than because I'm backlogged for other people's stuff. but these are things that give us credible neutrality, that I think is very important. 

**lightclient**
* I think we should probably wrap up soon. We're 10 minutes over. I don't know if we're going to come to a conclusion here, but we can talk about, so on the, the very immediate issue though, maybe we can resolve this one. 

**Micah Zoltu**
* We do need to decide what to do about EIP 5000. I would like to at least renumber it to something else. there's a PR out that does that. I believe we have a few editors that have agreed to it. I think if, if you're willing to move forward with that, we can at least close out that issue and move, move on. if you were pretty strong that we should not read a number, maybe 5,000, then we definitely should continue to discussing that specific issue, which may require resolving this bigger issue. 

**lightclient**
* I mean, you have the ability to override me, but I don't think that we need to do anything about this. 

**Micah Zoltu**
* I mean, sure. We have three, three editors, but my general preferences, I don't, I don't think we should, like, if we don't have unanimous or at least no one arguing against it, then we should wait quite awhile. and so the question is, is do we continue to discussing and over the next month or so, and eventually maybe renumber, maybe not EIP 5,000 at the end of the month. or would you rather just us remember it now? And you agree that, you know, your, I don't wanna say you agree, but like, I don't see an option where it's, we don't remember it ever. I think the options are, we decide we continue discussing, and then we decide Whether Or not, you know, after a month of further discussion or we decided today to we number it. If you're willing to budge, I'm not willing to budge on this at the moment, maybe with further discussion, I will. but at the moment I'm not. And so if you're also not, then I think that we should leave this in limbo until we can make progress. 

**lightclient**
* Let's, let's leave it in limbo. 

**Micah Zoltu**
* I saw your mic light up, but no sound. 

**lightclient**
* I don't know. Why can you hear me? Okay. 

**Micah Zoltu**
* I can, but I keep getting like the first half of your statements cut off. 

**lightclient**
* I said, I think you're, How about if I turn off automatically adjust microphone? 

**Micah Zoltu**
* Oh, you got louder. It's something changed. 

**lightclient**
* Can you hear me now? 

**Micah Zoltu**
* Yes. I heard you say, can you hear now? 

**lightclient**
* Okay. I think we should just keep it in limbo. 

**Micah Zoltu**
* Okay. So we can keep in limbo, continue discussing them. probably the on the PR is probably the best place I think. 

**Pooja Rajan**
* Well, yeah, we can probably take it for a few more days a week. Whatever's needed to get this decided and people are free to leave their comments on the pull request number that is added here in the agenda. I believe one of the important question that we were discussing idea was like this clotting issue also for squatting. If I have to like put it in the vote for the new try, we generally agree that, if we find some not so useful issues or requests created before dropping on good numbers, then we can particularly refer to them as a squatting. However, this is not exactly that issue, but it is, about the authority or the governance process that can be particularly considered as one time issue and could be discussed in the pull request here. 

**Micah Zoltu**
* I think the summary is we have lots of problems. the one we didn't talk about was the EIP number in unfortunately, I suspect that was actually one of the easier topics, despite it getting a lot of discussion

**Pooja Rajan**
* Right?Maybe we can have it on like top of our agenda and for the next meeting, we could not touch on item number two only, and then even more so we'll try to collect and put it on priority. So we get to address most of important things that we can maybe able to get a resolution faster. 

**Micah Zoltu**
* The there may be value. I don't, I don't know. I'm not sure how to proceed on these topics. in order to come closer to agreement, I think there's just like a, a fundamental, fundamental ethos difference between the parties involved. And those are very, very hard to come to rapid agreement on. one option would be to, you know, schedule this meeting to be weekly until we resolve it. kind of as punishment to us, recurring punishment until we fix our problems. we have to suffer through more frequent meetings. but I'm not sure that would actually help. Like, I think that when you have ethos disagreements like this, it just requires a lot of dialogue and that dialogue needs to be spaced out enough that people have time to go home cool down, think, restructure their world model,ecetera.And that is not a fast process like that can take weeks, months, years, depending on the topic. And so I don't know if we're going to get this resolved anytime soon. I do think we need to keep talking about it. but yeah, I don't, I don't have any quick and easy paths to resolution here. 

**Pooja Rajan**
* Right? Definitely more discussions are required here on this topic and many other similar problems. We'll try to bring it up and see where we go. I think we have, like, we have reached to a better place where we were about two years ago in January, 2020 when the EIP  meetings started. So I hope that this is going to help and future as well for the weekly. Do you have a proposal that we propose to have it next week? I can check it on the discord channel to get more feedback from people. Yeah. Yes. 

**Micah Zoltu**
* Feedback from other people, if they're willing to continue engaging on a more frequent basis, like all the parties involved I think are passionate about it, but I think also I suspect most of the people would rather not discuss it because an uncomfortable topic. anytime you have political or ethos disagreements like this, it's not fun to discuss them. And oftentimes it's not, you don't make progress either. Like it's, you don't get anywhere. And so on the one hand, you know, scheduling more meetings would give us more opportunity to discuss, but that opportunity may just be wasted if no one actually wants to engage. And so, and I don't, I don't know. So it's probably worth at least talking to the other people involved and seeing if they want to engage in a voice call more frequently until we get this resolved, or if they think that would not, that would not help. I'm really quick to answer Jay's question. so I think the EIP bot, still exists. It still has a purpose. It is still being used. And at the moment, basically we have a long list of things we want bots to do for the repository, whether they go into EIP w or the EIP bot. it doesn't really matter to me at least. and so it's really just, you know, who gets to it first, if someone as the EIP, great. If someone adds it to the EIP bot, great. we just want things to get improved and fixed and better. And so I don't think the EIP bots dead, it still has a large number of things that, EIP doesn't do. And I don't believe there's any intention to have EIP do many of those things. And so, so bots not dead. And if you, or someone else's interested in adding features to it, I'm certainly fine. It's probably good to coordinate with the people working on the EIP just to make sure you're not both working the same thing at the same time. but yeah, I think we continue iterating. 

**JA**
* Thank you briefly. That's fine. But if we don't manage to get the, that this, the cold test for the EIP board II, we will never progress. I mean, I have to try everything, sorry for my ignorance, because I need to do, to really confirm and conclude from my side that it is no way that I can set a test environment for, for the code in the boat. So, and we can do a lot of products because I have the code for, for these pull requests that are already there and find more issues. But I know the EIP wish already I read the code and it's good, but yeah, there are things that there is not going to do. We never do you, there is no way to, I mean, there is no way to test it. Well, at least I can, I can do the call and I can do the debug and I can try and, I cannot get there and sorry for the frustration, but I'm really frustrated. 

**Micah Zoltu**
* Yeah. Feel free to, let's talk in the, one of the EIP editing channels. and let me know in there, what's, you're running into, you definitely should be able to test it. I know Lita was able to test it and it should just be a matter of working in the Ethereum repo and, attaching the bot to it. but I can maybe try to help you a little bit more on getting through whatever roadblocks run into let's do that in one of the editing channels. 

**Pooja Rajan**
* Thank you, Jay sharing, a concern and the Micah for resolution. I think it would be a good idea in general to, put any question, common concern and the aviators channel. I'm sure someone on the channel, if they find issue and they are aware how to resolve it, they will be there to help out with, so thank you on that. And for the next meeting, I am currently considering that I will be definitely making, making an outreach to EIP editors and see if they are interested in having next week a meeting. But because most of them are already gone. Probably we can have the next meeting two weeks from now, but we can definitely share this word in the channel to collect feedback. And if they are interested going forward, we can have weekly cadence for sometimes, at least till we get some resolution. Well, thank you everyone for staying a bit longer. I know they could not touch on most of the things, but they hope to get it, get on it in the next meeting. Have a good rest of your day on a few. 


# Attendees

* Pooja Ranjan (Host)
* Micah Zoltu
* Chris huges
* Daniel Tedesco
* Gavin John
* Greg Colvin
* JA
* Lightclient
* Sam


# Date for Next Meeting: 10 August 2022 at 1500 UTC.


