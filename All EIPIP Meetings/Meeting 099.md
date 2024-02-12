# EIPIP Meeting 99 Notes
### Meeting Date/Time: Jan 31, 2024 at 17:30 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethcatherders/EIPIP/issues/310)
### [Audio/Video of the meeting](https://youtu.be/qd5E-4TbbXs)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
99.1 | **RIP process documentation**: Juan Caballero got a chance [to talk to the author of RIP-7212](https://ethereum-magicians.org/t/eip-7212-precompiled-for-secp256r1-curve-support/14789). The author is active in the community, but not part of the RIP working group.
99.2 | **RIP process documentation** The community may use some RIP process documentation.
99.3 | **Web Page Rendering to include EIPs, ERCs, RIPs**: @SamWilsn updated that @Pandapip1 has stepped down from the EIP Editors role.
99.4 | **Web Page Rendering to include EIPs, ERCs, RIPs**: @SamWilsn mentioned that he had a chat with Ansgar and they seem pretty interested in seeing RIP as a working group rendering. @gcolvin shared his support for the working group rendering.
99.5 | **Web Page Rendering to include EIPs, ERCs, RIPs**: Juan mentioned that Ullas (author of RIP-7212) at the time, didn't seem to know about the roles and responsibilities of the working group. People are already committing to other conversations.
99.6 | **Discuss Open Issues/PRs, and other topics**: ethereum/ERCs#213: @SamWilsn & @g11tech are okay to merge it.
99.7 | **Web Page Rendering to include EIPs, ERCs, RIPs**: Allow links to the Yellow Paper #275 - Decision: Yes
99.8 | **Call for Input #306**: Deadline Feb 07, 2024. @g11tech it can become a spam vector or maybe an issue to allow a new EIP to say that it supersedes or updates a particular EIPs
99.9 | **Call for Input #306**: Juan mentioned that there are multiple extensions of ERC-20 already. @g11tech will hesitate to pop these links on ERC-20 page.
99.10 | **Call for Input #306**: @SamWilsn suggested having a UI to showcase how the forward links will look like.
99.11 | **Call for Input #306**: Update EIP-6963: @poojaranjan thinks of proceeding with another proposal similar to ERC-233, to update the security vulnerability found in 1271 and educate the community about that. Updating a Final EIP may not be needed. Lot of back-and-forth argument, no decision - Editors please add your comments to come up with a decision by the end of the deadline.
99.12 | **Call for Input #308**: @gcolvin perhaps the authorship wasn't acknowledged when it should have been, if so - errata
99.13 | **Call for Input #308**: @g11tech thinks that EIP authorship is not a credit-giving system. The Final EIP does not require any further editing, so no need to update.
99.14 | **Call for Input #308**: @gcolvin thinks it adds value to individual resumes. However, @g11tech thinks it may open a Pandora's box of such cases of updating authors later on - No decision, editors may add their comments.
99.15 | **Call For Input #291 & #293**: Can be closed

**Pooja Ranjan**
* Welcome to EIPIP meeting 99. This is issue number #310 on Ethereum Cat Herders GitHub repository. This seems to be pretty short agenda. In fact, we have a few items to be discussed with respect to process. Then we will discuss any open issues in PR, call for input and any other discussion continued from the past meetings. We'll quickly take a look at the EIPs insight for the report of, January 2024.
* And, we'll get to know about editing Office Hour to begin with. the first item. And I see a comment here in the chat by Sam. No, Sam, we did not hear you. Maybe if you would like to rejoin or check your microphone. Very well. So the first item listed here is RFP process documentation.
* It was on the suggestion of RFP working Group, but I don't see any of the member on the call today. I wonder if anyone has any update to be shared. But I have got one update. 

# RIP process documentation [1:04](https://youtu.be/qd5E-4TbbXs?t=64)
**Pooja Ranjan**
* There is one RIP, which is RIP number 7212 has now been moved to final. So it will be really interesting to learn about the process they would like to follow. And what are the type categories they would like to consider. Because I can see here the category mentioned is good.
* Yeah. If anyone has any update or any thought about R.I.P. process. Feel free to share. 

**Juan Caballero**
* I briefly talked to, Dugan. sorry. who is the, guy who opened this one? and he, made it sound like, the roll up, like a lot of the decisions. It's sort of, in, you know, sync, like meeting based, and that they're doing something sort of on the a all core devs model. but it sounded like, he couldn't tell me who to talk to about the more horrible stuff. I didn't, I couldn't understand if it was. Who was the person who wanted.
* To be harassed about process per se. Like, maybe maybe Lightclient knows. Oh, sorry. I was putting them on the spot. Maybe we should start over. 

**Pooja Ranjan**
* All right, just for some context here, we were discussing the RIP process documentation, and it seems one, get an opportunity to talk to the author of RIP 7212. But we are still unclear about, the the decision making and process part. We were hoping to have someone from the working group to join this EIPIP meeting to maybe share about the process, but yeah. Anyone else on the call if you have.
* Thoughts, ideas or any information collected, please feel free to share. I have also left a few comments on one of the All core dev agenda, and after that we were reached out by the team. But I will try to follow up with the team again and try to get them in the next meeting if possible. 

#  Web Page Rendering to include EIPs, ERCs, RIPs [4.37](https://youtu.be/qd5E-4TbbXs?t=277)
**Pooja Ranjan**
* So if there's nothing further on this one, perhaps we can move on to a web page rendering to include EIPs, ERCs, RIPs. I am not sure what is the progress on that side, but yeah, if there are any. Okay. 

**Sam**
* Yes, I'm working now. Okay, cool. so I've been making a little bit of progress on the,. Keeps working group stuff. So EIP review bot is now running on my, repositories and the rendering is done, for that. also, I'm not sure if anybody else is aware, but, Panda PIP has stepped down as an editor for the time being.
* Just wanted to make an announcement about that. but yeah. So, I'm working on EIP review bot for, working groups and, yeah, you can follow along my development.

**Pooja Ranjan**
* That is wonderful. Thank you, Sam, for that. Sam, whenever you think we are in a position to maybe have a small demo and we can publicly announce that that would be really nice to have. 

**Sam**
* Yeah. I mean, eventually we're going to have to decide if we want to adopt, that structure. So I think that's probably something we should do before, we announce publicly. how do people feel about that in general? Do we want to go down the working groups road? 

**Pooja Ranjan**
* Yeah, I feel like this could be a good time to discuss that, because we do not have a ton of items on the agenda, and we probably have most of the editors on the call. 

**Gcolvin**
* Can you put a link in the chat to. Any document that I can skim quickly. 

**Sam**
* Yeah. It's the same one that we've been discussing, with the, working groups having their own, like, members and everything. I'll find the hackmd. 

**Pooja Ranjan**
* I have a question here. If I understand correctly, the present eip.ethereum.org also, rendered the ERCs. I mean, I had someone working on rendering of our RIPs, but I do not see any success over there. I'm wondering if people still want to go that route, or if we want to switch and move altogether to the working group part. 

**Sam**
* So I'm in favor of having our RIPs be a working group so they'd inherit the same rendering stack. But I don't know how everybody else feels. 

**Gcolvin**
* How do they feel about it? 

**Sam**
* I've talked briefly to Ansgar about it, and he's pretty, pretty interested in making it a a working group. 

**Gcolvin**
* Which case, I'm all for it. 

**Juan Caballero**
* Yeah, that's all. I seem to like the general idea, but it seemed like I was. He was hearing about it for the first time. I don't think he had, like, a clear, definition of what being a working group meant and didn't know how to, you know, check if I was asking him to commit to more than he was already committing to another conversation. So I think my action item was to, send him links to what becoming a working group meant. maybe.
* I don't know if that's. Similar to the vibe you got from Önskar. Blushes I think just an active member. I don't think he signed up for any sort of formal duties. He's just the guy who wrote the RIP mentioned above. 

**Sam**
* As far as like formal responsibilities for where like what is like quick summary of what it means to be a working group. It means you're kind of subject to the similar rules that we have for EIPs now. So like, you know, formal external link policy, you have to use markdown, a few other things, and, you'll have to use our repository structure.
* And then on the governance side, you have to like write a document describing your policies. But other than that, there's not too much overhead. 

**Juan Caballero**
* Yeah. The the first thing les told me was, I said, hey, do you guys want to be a working group the way is? And and he was like, oh, you mean like getting a repo like they have? Yeah, I think we're planning to do that. So on that level, I don't think there's any conflict. I think they're okay with that. 

**Sam**
* Yeah, I guess reviewing PRS would be the other thing. People would have to review PR. 

**Juan Caballero**
* They'd have to review PRS, but they already have their regular, calls. So I think it's very it's sort of logical to be like at each call we just review, you know, check in on our repo. It seems like they are fine with it. It's the same compatible with their structure. 

**Gcolvin**
* I can predict that there'll be conflicts over external link policy. 

**Sam**
* Yeah, I think that's probably true. And, you know, obviously working groups can define their own kind of. Exceptions and however they want to approach it. There's a lot of freedom. So. 

**Gcolvin**
* So pretty much if an author of an RIP wants to do a link that we wouldn't like, it's more up to the working group. Is that what. 

**Sam**
* I think so, yeah. like, our goal, like our mission as EIP editors, is to make sure things are, you know, durable for the lifetime of Ethereum. and I think we can probably come to reasonable compromises with working groups on the specific, like, rules they want to use. 

**Gcolvin**
* An easy one is is simply to, Push it as far down the pipeline as we can. so it doesn't prevent drafts from going in. But by the time you get to final, these things have been resolved. It also gives the author time to find a better source for the length, but still have something to link to now so that people reading the proposal, you know, have something that they can read.
* So. E.g. you might you might have a link that's only to the author's web page, and it might take some doing, to find a better link.
*  But during draft phase even review, the author could want the link there because that's the only link that he has to explain the the concept that needs explaining or to back up the motivation or anything like that. 

**Sam**
* Yeah, that makes sense. 

**Pooja Ranjan**
* Absolutely. And I would really appreciate, the users and whoever involved with the RIP process right now, like on definitely it's being discussed in the meeting and being pushed. Peers are being merged one off. One or more of the members may either document those things.
* So community may be able to refer to or maybe join our meeting and share their thoughts, and we can be aware of it and kind of help whoever are new and would like to document a new RIP, we can definitely send them towards the RIP discord channel that is available on the Eth R&D, but generally speaking.
* It will be a good idea to have proper documentation around because I know at this point the GitHub repository is also like really a very early stages, and we do not even have the name of editors listed over there. So it will be really nice to have something documented there.
* All right. Sam, just to be sure. Like, would it be possible for you to maybe provide a demo by the next meeting, even if we are not formally announcing that? that will perhaps give people to have a better look of it and maybe compare and see, if we would like. 

**Sam**
* So to to be clear, everything is working except for Eth review bot. And if you can actually see it all live right now. like the web page rendering and all of that. 

**Pooja Ranjan**
* Would it be possible for you to maybe collab? Sure. Yeah. On your screen? Yeah. Thank you. 

**Sam**
* Yeah, yeah, I can do that. 

**Sam**
* Here we go. So it's pretty much the same as before. I don't have RIPs just because they don't have, a repo yet, but, you know, web page is here, and it's all rendered from separate repositories. Rendered using Zola instead 

**Pooja Ranjan**
* What is this governance mean here? Like, I can understand Core wallet and. 

**Sam**
* Yeah. So this is, the working group for, defining the EIPs process itself. So this has things like our external links, the EIP, ERC repository split, our handbook. yeah. So this is kind of like the meta category. 

**Pooja Ranjan**
* Right. But if I understand correctly, it's not collecting all meta but some of them. So how do we pick it? Like is there any code defined for it, or do we need to select these proposals manually? 

**Sam**
* So all EIPs that exist today are moved into core, except here written list, because most surprisingly, most meta apes are, hard fork descriptions and not, governance documents. 

**Pooja Ranjan**
* That's right. And I'm wondering why we are ERC EIP split here and not in the core. 

**Sam**
* Oh, because this is a governance related like splitting the repositories is a governance thing. 

**Juan Caballero**
* So hard fork sort of project management coordination documents be informational technically, or was meta the right way to designate those in the first place? 

**Sam**
* So meta was originally like, a category describing other EIPs, and it was meta because it was just a list of the other EIPs that were in the hardfork. But now there is no meta because it's kind of ambiguous. So there's, there's governance, which is for the EIP process itself. And then there's Core, for You know, hard fork organization and stuff. So. Yeah. 

**Pooja Ranjan**
* So just to understand it better, we are not going by the type and category, but we are going by selecting which will be the best suited for the working group. 

**Sam**
* Exactly. So instead of it being like a type and category, you'll have a working group and then each working group, if they want, can have categories like, core. 
* Yeah. So, so for example, the core, working group has both core EIP and networking EIP as subcategories, but that would be up to the working groups to define how they want to organize stuff. 

**Pooja Ranjan**
* And maybe one other related question. I'm sorry. I'm asking so many questions. One other related question here, like do we have a list of or should we maintain this list somewhere? But who are the participants of respective working group? Can we maybe, provide some placeholder in this website so people can know that if I have question with respect to this particular working group, I can perhaps reach out to these editors or users. 

**Sam**
* Until we officially launch it. Like, this is just my playground. there's nothing here that's permanent. I regularly erase it and start over. So I don't know if it would be worthwhile, but there are, There are. If we go into the actual repositories. There is like the, same kind of Yaml file that lists the members of the working group and EIP editors. so that's going to be very similar to what we have today. 

**Pooja Ranjan**
* All right. Yeah, I mean, I find it good. I mean, I feel like it is really good. If we can add perhaps a little bit more information about the people whom we should be reaching out to, for example, to understand what are their thoughts about just they want to categorize core networking and how they want to put it. Otherwise it looks good, and it would be a good way to share proposals. With respect to working group, I wonder if anyone else has any other questions. 

**Juan Caballero**
* I was just going to plus one and say that the. the working group breakdown as opposed to category or type breakdown. Like it like adds another category that loosely maps to category and type. But like, there's very good reasons for needing a certain category. It would it would be more legible.
If it was part of a bigger socialization of the concept of the working group. And one way of doing that, like Pooja mentioned, like if when you click on a working group, the color of the site changes or you know, a contact name appears or like it sort of, some sort of UX feature flagging that you're like, entering a different zone of authority and there's like a different contact person.
Right. Like that could be that could be at the level of display that could be hidden from the level of display, but obvious in other contexts.
 Maybe when you go to the repo, it's in the at the top of the first Readme and the root directory, maybe wherever, like, wherever it happens. I do think it's good to have some sort of nudge that like, you know, this is a, this is a.. A different zone, a different something. 

**Sam**
* Okay. So, You'd like to see more of an indication of like that, you're in a different part of the website or kind of. 

**Juan Caballero**
* Yeah, like I do think I mean, I think Pooja's, instincts are right here, that the average user won't care much about differences of governance, but they'll be very thankful if they know there's a different person to tag on GitHub or a different sort of, you know, contact endpoint, whether that's an email or a GitHub name or what. But, something that sort of signals it's a different department or a different workflow, something like that.. 
* I'm trying to yeah, I'm trying to agree, but also generalize at the same time. Like maybe, first idea, probably best idea, but but thinking more generally, the, the working group as a concept is sort of only known to the people on this call or the people involved with moving repos. So it might be good to think of the socialization of the concept as a project worth coordinating, like pin, a message on ETH magicians.
* Maybe I was thinking about maybe working groups could each have categories on ETH magicians, and whoever curates that category might be the same person you contact if there. See what I'm saying? Like a front door for each working group might be good. 

**Gajinder**
* Or I mean, there is another way one can sort of allow them the freedom to render any way they want, while adhering to the checks that we would want is in terms of social web tags. So they can basically, right now, our, lenders expect a certain format and we can basically throw all away all of that and allow them to have any rendering format they want. And then basically with the social tags, they would have to match the categories that we have in our internal rules.
* And using that, maybe, you know, it is possible to give the freedom to working groups to render in any way they want. 

**Sam**
* Is it something? Potential working groups want. Like they said, they don't want to necessarily use markdown and they don't want to use like our pull request bot. They want to do their own thing entirely. 

**Gajinder**
* I'm not sure. I'm just thinking if this is a real issue, that they want their own rendering formats, and maybe this is a way to allow them. 

**Sam**
* Yeah, that makes sense. Yeah. I think at first we should probably provide just like an out of the box solution, and if somebody wants to do something crazy, then I don't see why we couldn't let them. 

**Gajinder**
* Yep. Makes sense. 

**Sam**
* Cool

**Gajinder**
* Intent of allowing them the freedom to do that will solve a lot of the edges that people get, when they are restricted. So if you just say that you are allowed and we will be able to, again, we will be able to assess your page based upon, for example, social tags. Then, I mean, most of the issues that they would have for fitting into a certain format, we want them to those would go away.
* I mean, even if they don't end up doing anything. But still the illusion of the freedom basically takes away a lot of resistance. 

**Pooja Ranjan**
* I find this generally is a very good idea. To be very honest. From my side, I would love to see no change in header or maybe a unified header across all working groups. Data analytics could be easier for individual projects, infrastructure projects around EIP, but obviously it would depend on working groups. So yeah. 

**Gajinder**
* That could still happen. Pooja, in the sense that when we process the markdowns and we look for our, social tags, then we can basically process and format those tags on the top of the page. So it would still be possible. and we still can sort of allow them the rendering format they want. 

**Pooja Ranjan**
* That would be awesome. Great. Well thank you Sam. This seems like a good progress towards a including all proposals, including our apps as well, along with Ercs and other working group, that we can see here. Hopefully we'll get to collect some input from other editors as well who are not here on the call today to maybe decide on if we want to go ahead with the, this format and merge it as a part of, EIPs.ethereum.org any final comments before we move on to the next one? 

**Juan Caballero**
* My only thought would be. Could we ask Ansgar or someone involved with our EIPs, to come to the next meeting? 

**Pooja Ranjan**
* I mean, we can definitely tag members, on EIP editors channel on R&D and let them know about the next meeting date in advance, and perhaps hope for one of the representatives to join. 

**Juan Caballero**
* Cool. Yeah, I think it might just help because then it would double as the walkthrough on the next meeting would also double as onboarding if they want to do it right. Like it would be a. Absolutely like sort of a subtle way of nudging them, tricking them into saying yes on the call. 

**Pooja Ranjan**
* All right, moving ahead to the next item, which is about to discuss open issues and PRs and other topics I see in the chat. Sam has already given a thumbs up to the PR #213, which is about EIPs updating an ERC 1363. This was also requested by one of the users in the comment I wonder any editor has any different thought. Or if all of them are okay to get it. So I see one more thumbs up. Very well.
* We can perhaps merge this PR unless that any editor may add any further comment suggesting they are not open to merge this one. The next one. 

# Call for Input [29:15](https://youtu.be/qd5E-4TbbXs?t=1755)
* Here is the call for inputs I have listed two new call for input number is 306 and 308. Sam, if you would like to maybe take a few minutes and talk about these, call for inputs. The deadlines for both of them are February 7th and February 8th, respectively. 

**Sam**
* Sure I can talk a little. So 306 is a back link kind of proposal. So, let's say I'm working on an extension for ERC 20. in my document I'd be able to say extends 20 in the preamble, kind of giving an official symbol or, like back link to the thing I'm extending. And then on ERC 20, there would be a list of, all of the proposals that claim to extend ERC 20 and that would be handled by the rendering infrastructure. So there'd be no change to the actual text of the ERC 20 to make that work. 

**Pooja Ranjan**
* Editors. If you have not added your input for this particular issue, please feel free to add it on or before February 7th so we can have a discussion. And yeah, may be able to move forward or just close it. 

**Gajinder**
* I added the input and my apprehension is the same that I did over there, that it can become as a spam vector or another vector, where we have to judge whether we can allow a new EIP to say that it supersedes or updates a particular old EIP. 

**Juan Caballero**
* Maybe. Maybe the 6000 ERC for ERC 20 extensions is a good concrete case for discussing that, because without having a way to without marking each as an extension of ERC 20, we still get a lot of them. Do you think there would be more of them if they could mark themselves as an extension of ERC 20? 

**Gajinder**
* I mean, if on that particular EIP or ERC page we show that it extends, for example, ERC 20, then it's fine. I mean, because those tags are not getting into ERC 20 EIP page and a person who is looking at that particular EIP page for that, it is a relevant information and a back to back link to ERC 20 is useful. but yeah, I would basically hesitate to sort of pop these links on ERC 20 page.

**Juan Caballero**
* I mean, I guess  my thought was in the case of. Extension. Later documents extending. That's a pretty good argument against forward lengths, but in the case of an informational updates, hey, I want to rewrite the security considerations. Same author updating a final EIP with a new X section or more examples or something there. A forward link is really helpful because you want everyone who sees the original to see the update.
* And for me, the utility of having update EIP being more satisfactory to the cranky people trying to update their final EIPS, is, a good that outweighs the bad of ERC 20 having a spammy forward link section.
* You know, like I think I think it's a pretty minor. Nuisance to have ERC 20 have a, you know, 200 forward links. Whereas I think it's a pretty major benefit to have updates be seen more. I think in all the threads where people are trying to, patch final EIPs. the recommendation is we'll just open a new informational and every time they're like, but no one sees it. To me, that's the big thing in. 

**Gajinder**
* The structured in the structured groups like, you know, core devs, right, where the core devs adopt an EIP which supersedes a previous EIP. It's very easy to make a decision, right, that yes, this has been adopted, but for example, for ERC where the standard is more decentralized and there is no community, which is basically saying that, you know, also a community can't definitively say that, okay, this ERC is interfaces better, right?
* So in that manner, how will you do that? Maybe you can just have a link that says that okay, you know this, they are extensions to this particular ERC.
* And you click and then it does a search kind of a thing shows you a list. Maybe that can work. 

**Juan Caballero**
* Right. I think listing everything that claims to supersede. Isn't that harmful? A harm like if there's too many links in that section? Oh, well, there's too many links in that section. 

**Sam**
* So maybe what we need to move this forward is like showing a UI of what it might look like to have these forward links in the case that they're very spammy. So like, how bad would it look to have 400 forward links off ERC 20? 

**Juan Caballero**
* Yes. And that's also an argument for you know the precedent from ETF a is structured working groups like you're saying. So that it applies better in some categories than others because there's some external curation. and B there's two categories. There's replaces supersedes and there's extends. Here the extension category of ERC 20 would have 400 in it because the all the ERC with NFT in the title are assuming the basic ERC 20 interface and adding more functions or whatever. so. 

**Sam**
* That's kind of like.  Our requires header now. 

**Juan Caballero**
* Yeah, even just displaying requires if people are using requires properly already. If the corpus of documents already has a lot of them filling out requires, then you could just, maybe to your point that it might help to have a sort of preview. You could just do this with requires because requires and requires extends is sort of the permissionless version already the supersession part is probably the spicier part. 
* And there I was, trying to think of the permissionless semantics, and all that could come up with was like forks, because a fork is assumed to be a permissionless upgrade. Like, you can join us or not join us, but there's no sort of authority calling this the one upgrade. But maybe that's a. 

**Sam**
* It's an interesting choice of words. 

**Juan Caballero**
* Inflammatory choice of words, perhaps. But like the hard fork schedules. Right. Like there. It's an upgrade cycle. I don't know. Super session only really works in like an ETF case where there's an external authority saying. This definitively supersedes this. But a fork is sort of like it could be superseding or it could not. It depends on the it's decentralized. 

**Sam**
* Yeah, I think the prime example here is like  223 and ERC 20. . The dachshund who wants to, like, rip out approvals. I think, you know, he considers that to be a superseding  EIP where I would consider it not to be superseding and it to be like competing, I guess. so I'm not exactly sure what. 

**Juan Caballero**
* We have a word for that already. It's a hard fork. 

**Pooja Ranjan**
* I mean, I would suggest that we should not complicate things any further than it is actually required at, if we give a look at the present list of EIP, even on the simplest website, EIP.ethereum.org. It is not difficult to find ERC 20 related proposal. If people want to have extension, they can go ahead and do that. But is it really necessary to? The new proposal could be considered as superseding. So we really think there is. There is any advantage of doing it. Yeah. 

**Gajinder**
* So it could be useful for example in core EIP I mean because yes, there's there is some superseding that does happen and it is very, you know, clear that, okay, this proposal supersedes and has been accepted and has moved into final. So. 

**Pooja Ranjan**
* I agree, it totally makes sense over there. 

**Gajinder**
* Yeah. Maybe we can by a working group, have these tags. Whether it's superseded is acceptable in this working group or not. I mean, maybe we can do that. 

**Pooja Ranjan**
* I feel like in the case of application standard, it is not for, like, the governance member to decide on that because application proposals are for different application. Some may need the older version and some may need the newer version of them. It could be on their organization if they want to have like a upgrade their proposal and they can say, okay, fine, we have upgraded. And now new proposal is superseding that.
* In my mind, it is not adding too much value to the list of standards, especially for application. I can totally understand it makes sense for the code proposals. 

**Juan Caballero**
* I think, I mean. 

**Sam**
* Those are the ones that need it the least, though, because. Core proposals don't go final until they're on main net. So you can just update the proposal until it's. Published, whereas irks somebody will finalize it. And then like in the case of what is it, 1271 they find a security problem and then they want to update their EIP. Well, like they don't want to come up with a new number because it's going to be mostly compatible except for a little note they want to add. So I think core EIPS don't need supersedes nearly as much as ERCs do. 

**Pooja Ranjan**
* And in certain cases we have seen examples of like, you know, one proposal, I think, which was in the past upgrade now get a better version, I mean, like the better proposal and we move on that on the core. We just know by the latest list of proposal for the latest upgrade and we move forward from there. Yeah. 

**Juan Caballero**
* But we just know is exactly the thing that's a problem for casual observers or first timers, or if there's sort of an information asymmetry there. I think that the distinction here is like all core devs just know because they're there's an external authority to marking things as archived elsewhere. And once an ERCs goes final, there's no way to know or notice that it's archived, like you can only withdraw something if it didn't go to final.
* When something goes to final, it can only be forked, permissionless only because there is no mainnet runtime to tell you that a final ERC is no longer relevant, or that the momentum has moved to another fork.
* I don't know. I feel like I feel like that. I feel like the arguments I'm hearing actually sort of cut both ways. And in a way, the just linking the things that claim to fork something permissionless is almost like the most you can do without changing the rules for final status. Like if you don't want to change status, but you do want to give final ERCs a way to be. Somehow marked as archival externally. I don't know, just my thought. 

**Gajinder**
* I mean we so superseding is something that for example can be part of the base. IRC which is being superseded. I mean, if that author is agreeing that this is being superseded by some particular other standard, then we can actually allow a superseding tag directly in the that particular ERCs which basically author is agreeing to. So there is a definitive authority who has earlier authored a particular ERCs and is now conceding that. This is being superseded, or it has security issues or whatever and should be superseded by this particular ERC. So maybe I. 

**Juan Caballero**
* Actually proposed that earlier, but I was told that front matter can't change after something goes final. 

**Sam**
* Yeah that's my position. So once once the document goes final you can't change it. Well it's not that you can't change it. It's that. I mean, we don't want to defer to the author as the authority of deciding whether or not we can change it. 

**Gajinder**
* Now, instead of allowing basically the author to change segments to it, he can just add that this is superseded by this particular ERC, for example. I mean, that is the only change we can allow. 

**Sam**
* So my problem with that is once a proposal becomes final, it's kind of gifted to the community. Right. So the the entire ecosystem decides whether or not it's been superseded, not just the author. Like sure, the author has, you know, permission to change it all the way up until final. well, I guess last call technically, but, then once it goes final, it's like this is done. Anybody can use it. and then Okay, maybe an example is better.
* It's kind of hard to explain my feelings on this. So, imagine, you know, a malicious author writes, an EIP that contains a security vulnerability, and they write it all out.
* They know about the security vulnerability or maybe even not a security vulnerability, let's say a inefficiency or a bad API design. And, you know, they convince the rest of the ecosystem to implement their standard, while secretly they're implementing the next version of their standard. That's significantly better. and then they release that, after everybody's wasted a whole bunch of time implementing the first version of their standard. So they have this leg up on the rest of the competition because, you know, they convinced everybody.
* Think badly and then they release, you know, the better version later on. and I mean, you know, supersedes and labeling it in the EIP doesn't really stop them from doing that. But I'd rather not give authors the ultimate power to modify their EIP. 

**Gcolvin**
* In the and internet standards superseded. Makes sense, because it basically means this is the way we did it in the past, and you should stop doing it that way. Because if you do, you're going to fall off the network. everyone's going to do it this new way now. but for the typical ERC, that doesn't make any sense. people can do whatever they want. So in the absence, I think in the absence of a working group, that's actually taking responsibility for these things so that they can make such recommendations.
* No, there's no one thing can't supersede another, except that the community can recognize that, oh, ERC 20 is broken in certain ways. And here's a new proposal that's better. And so the community sort of on its own, either keeps using ERC 20 anyway or uses the better one. 

**Juan Caballero**
* But but sorry, but I completely agree, but the distinction there is between a centralized protocol and a decentralized protocol. Because if you can only be on one version or the other, like you say, if you fall off the network doing it the other way, then that's a fork. 
* Be a supersession because there isn't one network that decided unilaterally that we're all going to fork. So there can only be a sort of opt in, opt out fork. But if you want to signal, you either do the older way or the new way, we need some semantic other than supersession, and I lead more and more towards fork because the new EIP is telling someone do it this way instead of that way to switch from that network to this network. 

**Gcolvin**
* Another tirm is deprecated in the case of core the criteria. 
* The, the criteria used to be that it's, it's basically final once it's on the main net. and the core developers are they can set up their workflow however they like, and they're even when they didn't have their own workflow, they were we can't prevent the core developers from grabbing something from any stage of the EIP process, or even something that's not an EIP, and deciding that they are going to include it in an upgrade.
* And then then ex post facto would be really good to have an EIP describing what happened. but typically there is an EIP. and it will need to describe what's actually on main net. And that becomes the final EIP.
* And if any discrepancies show up. the discrepancies are that the EIP does not, describe the main net because the main net is running the the main net is the source of truth, not the EIP. And at that point, at that point, I think you need errata to the original EIP. rather than new. I way confusing to have a new EIP that supersedes the old EIP. that people, implemented onto the main net. This would happen if everybody made the same. If everybody did it differently than EIP, and it's running on the network and it's, you know, there's consensus and,
* And I'll stop talking, because I'm trying to say something simple and I'm going on and on. 

**Pooja Ranjan**
* Actually, it's slide number 21. so I have just shared a presentation that we had a few years ago, wanted to let people know here that superseded was actually a status a few years ago. But when we tried to kind of simplify the process or unify the process for all core and non core proposal, this was dropped. I am aware that there was at least one proposal which was into final, and in the next upgrade it was superseded by another core proposal. So we use this status. But it was dropped and we decided to move on with final only. So if you want to bring it back.
* Like considering there are use cases of that that can be definitely be under consideration and we can start discussing that. But about this particular, call for input, do we really have a case to back it up? Why are we proposing this at this point of time except for 7020? 

**Sam**
* 1271. Okay, so there's a security problem in it. And it is a like inarguable, legitimate security problem. And. they want to, update it with that security consideration. 

**Pooja Ranjan**
* I mean, I'm just trying to understand why are we treating it different than ERC 20? The author of ERC 223 also claimed that there was some issue with ERC 20 that led to a lot of hacks. Then the author potentially went ahead and wrote another proposal. Can we do the similar thing with 1271? 

**Sam**
* Sorry. Could you ask the question again? 

**Pooja Ranjan**
* So my question here is like, the solution that we shared, with respect to ERC 20 and the author went ahead with the new proposal and kind of educating the community that this new proposal is going to overcome the issue, which were there with ERC 20 that may have led to certain loss of funds. 

**Sam**
* You're talking about like 223, right? Yeah. 

**Pooja Ranjan**
* Yes. So can't we suggest the same thing for 1271? I mean, if an organization, if a project found that this, this particular, proposal has some security issue, they can perhaps come up with a new proposal and upgrade their project to that proposal. Is there any specific reason that we need to stick with 1271 as the number that has been implemented in that project? 

**Sam**
* Not that they want to stick with 1270. I mean, they do want to stick with 1271. Their preferred solution is updating it. But I think what they're willing to accept as like a compromise is if we have a link on 1271 to the replacement. 

**Pooja Ranjan**
* I mean, that is an additional ask. And that's really kind of them that they want the community to know about it. But I understand there are other ways that can help that particular project and perhaps the community, without making a lot of changes in the current process. I think we already have. 1 or 2 calls for input on 1271 K specifically, or do we want to have. Maybe one final round of call for input to decide on this, this particular issue that can or cannot we include the superseded part in a final proposal.
* I think at this point, we can definitely wait till 7th of February to see what other people think about it and based on the response that we collect. It it can be decided. All right. Is there any other final comment or thought that people would like to add for this particular call for input? 

**Sam**
* I think we're good to move on, I think. 

**Pooja Ranjan**
* Yeah. So there's another one. 308. 

**Sam**
* So, this is, a final EIP where the existing authors want to add a new author to the author list after it's been finalized. 

**Gcolvin**
* Sorry. They would probably do that if that person was an author all along. But, wasn't their authorship was not acknowledged when it should have been. 

**Gajinder**
* I mean, as I have commented on the issue as well, I mean, authorship is not same as the credits for the EIP. So I don't see why we should allow any change over there now since it doesn't need any maintenance. 

**Gcolvin**
* I'm not understanding. for us, I think authorship is just literally that you you contributed. You contributed to the EIP. either. 

**Sam**
* So it's both permission to modify the EIP and a list of people who contributed. 

**Gajinder**
* So in my understanding it is does not reflect credit to the EIPs in the sense that the people who contributed to the EIP, because, I mean, I don't know the crediting and saying that. Okay, you know, we picked our idea from here. These are the inspirations. All that is a messy stuff, I see. Author of the EIP. As a people who would want to make edits to it or edit it or basically maintain it, but since it's final and it doesn't need any maintenance,
* I don't see whether why should there be another author to it in the sense that it is also a retrospective step. Right?
* If the contribution was meaningful at that particular time at which the EIP was written, we would definitely they would definitely be a mention. So in retrospect, editing of the authorship, I actually don't see what basically the benefit to the community is and why it should be allowed, because it doesn't serve any purpose. 

**Gcolvin**
* If nothing else, it serves a purpose in the resume of the person who should have been recognized as an author and wasn't. 

**Gajinder**
* But it opens up a door box to other people who will say that. Okay, you know, people who might bribe other well-known EIPs to get their name inside and to pump up their resume. I mean, we are not there for people to pump their resume, right? So,  I actually feel that, I mean, I strongly feel, but I think that we shouldn't do it. 

**Gcolvin**
* Yeah, of course we're worrying about something that's never happened. What? What has happened? 

**Pooja Ranjan**
* This is the first case where we have received this request to maybe update an author after it is being finalized. Otherwise, historically, we have seen authors being added, whoever may have implemented those proposals and respective client, or may have contributed significantly as co-author of the proposal. 

**Gcolvin**
* But what has happened is proposals, where one of the authors no longer supports the proposal. and currently that that person remains an author, because of their contribution. And in one case, did not want to be removed as an author, even though they were very much against the proposal. So, um. Mm. 

**Pooja Ranjan**
* Very well read, and any other editor who may not have added their comment. If you would like to maybe add your comment towards this issue, it would be really helpful making decision by the end of the, deadline here. And we are four minutes past time. I quickly wanted to maybe mention about the issue number 291 and 293. I think the deadline for these two call for inputs have already passed. do we plan to extend that deadline or are we good to close them? 

**Sam**
* I think they've been open long enough. 

**Pooja Ranjan**
* Okay. Perfect. And, I think I have repeated item number three. My bad. So we can perhaps skip that part quickly getting into the EIPs insight, because today is also the 31st of January, which is the last day for this month. So if we, take a quick look at the EIPs insight, we have two final proposals on, EIPs repository, one in ERC  and one in EIP. So this is the first proposal which moved to the final status for RIP.
* And we have nine proposal added to the ERC repository in the month of January. And two proposal on EIPs repository have been moved to the stagnant status. The detailed list can be found on the links added to the agenda, and people can also refer to EIP insights.com. One other question that I want to ask this group quickly before concluding the meeting for today is the time for the next meeting, it seemed in the another group chat, the discord channel, that there could be further discussion of the alternate time.
* Do we want to stick with this 1730 UTC, or we want to go back to 1400 or 1500 because us and each JS team meeting are at 1600 till 1730. Okay. Yeah. Please go ahead. Sam. 

**Gajinder**
* Ask Matt what his preferred time slots are. 

**Pooja Ranjan**
* Sam, I think I over spoke you. You were saying something. 

**Sam**
* I was just going to ask, my audio cut out for a second. I didn't hear the times. 

**Pooja Ranjan**
* Okay. I was mentioning about going back to the original time 1400 or 1500 because, the later half is, like, filled with other meetings. One is EOF meeting at 1600, and, each meeting is there from 16 to 1730. So we can either start at 1730 or we can go back to 14 or 1500. 

**Sam**
* I'm okay with any of those. 

**Pooja Ranjan**
* It seems most of the participants of this call are definitely okay with 1730 UTC, but as I have mentioned in the discord channel of Eth R&D, let's hear from people if they would like to maybe change it to 14 or 1500. But if we do not receive much of the response in support of either of time slot, then we will continue to have it at 1730 UTC. All right. I think we have covered to most of the agenda item today. Is there anything else people would like to quickly mention? In that case, Thank you everyone for joining us today.
* And thank you, Sam and Gajendra for running the last meeting. It was a quick one.
* I really hope that you guys run the meeting so it becomes a way quicker. All right. I hope to see you all in two weeks. Have a good rest of the day. 

---------

## Date and Time for the next meeting

Feb 14, 2024 at 17:30 UTC

---------
## Attendees

* Pooja Ranjan
* Sam
* Gcolvin
* Gajinder
* Juan

