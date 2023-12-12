# EIPIP Meeting 94
### Meeting Date/Time: November 15, 2023 at 15:30 UTC
### Meeting Duration: 68 mins
### [GitHub Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/292) 
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=uaYvYugYLOE)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

# Agenda
## 1. Discuss Open Issues/PRs, and other topics

**Pooja** [0:00](https://www.youtube.com/watch?v=uaYvYugYLOE&t=0s): Welcome to EIPIP meeting 94. This is issue number #292 on Ethereum Cat Herders GitHub repository. So we have items to be discussed which are some of them are open issues and Pull request, a handful of open call for inputs that we would like to know where we are on that. And then we will take a look at EIPs Insight plus ERCs insight for the month of November. A few updates from EIP editing office hour. And we'll take a look at review action items from the earlier meeting. 

## EIP-ERC repo split

**Pooja** [0:40](https://www.youtube.com/watch?v=uaYvYugYLOE&t=40s): So starting with the first one, discuss open issues, PRs and other topics. I believe the burning topic here is the update on EIP ERC repo split and we are joined by Gavin. So Gavin if you have any update on that to be shared please feel free.

**Gavin** [0:59](https://www.youtube.com/watch?v=uaYvYugYLOE&t=59s): Okay so recently upgraded my SSZ and also switched from winners to Linux. So I am still kind of getting my new development environment set up but I will be able to resume work on the tooling’s soon. 

**Pooja** [01:18](https://www.youtube.com/watch?v=uaYvYugYLOE&t=78s): That is awesome. I believe a few of the authors have shared some concern with respect to HTML proofers. Is it resolved? Where we are on that?

**Gavin** [01:31](https://www.youtube.com/watch?v=uaYvYugYLOE&t=91s): So the issues have primarily been that users are doing the or rather authors are doing the expected thing and updating their links to the new files. The problem is they can't do that yet because the tooling isn't smart enough to be able to rewrite the links yet. And this is also because the system we have currently is a very temporary solution. And we are planning on kind of taking out all the website code from both of the projects and putting it in the new repository. But to all EIP or  ERC, well specifically to all ERC authors, don't update your links use “EIP- EIP number or ERC number” even for ERCs. And I guess also for EIP authors if you're linking to an ERC use EIP Number.

**Pooja** [01:38](https://www.youtube.com/watch?v=uaYvYugYLOE&t=98s): That is helpful. I believe there were some authors with this kind of concern in yesterday's EIP editing office hour. So it's a good piece of advice that all ERC authors even if you are creating a new pull request at ERC repository. Please keep the name of the file which you are referring within your document as “EIP - whatever the number was”. 

**Gavin** [03:12](https://www.youtube.com/watch?v=uaYvYugYLOE&t=192s): Also the link Checker will complain so and unfortunately that's one that gets kind of priority for check annotations because HTML doesn't have check annotations. So I'm considering just removing the link or disabling the link check CI for the time being. Because I think it might be misleading authors.

**Pooja** [3:41](https://www.youtube.com/watch?v=uaYvYugYLOE&t=221s): Right. I believe as of now on ERC repository Issue Number #8 is kind of guideline for ERC authors to follow and make their PRs on the ERC repository. Do you believe if we add any additional information with respect to this HTML proofer or what they are supposed to do specifically here. Would it be helpful? If it is not there. 

**Gavin** [4:05](https://www.youtube.com/watch?v=uaYvYugYLOE&t=245s): We should absolutely do that.

**Pooja** [4:08](https://www.youtube.com/watch?v=uaYvYugYLOE&t=248s): Okay you mind taking care of that?

**Gavin** [4:12](https://www.youtube.com/watch?v=uaYvYugYLOE&t=252s): I cannot, it's a lightclient’s issue. Oh wait no I can edit other people's issues sorry yes I can do that.

**Pooja** [4:20](https://www.youtube.com/watch?v=uaYvYugYLOE&t=260s): Okay perfect. I hope this temporary solution will be answering the burning question from ERC authors as of now. But in case you guys feel any other question feel free to drop by Ethereum Cat Herders Discord Channel. We have EIP editors Channel especially for all these sort of discussion if you have any questions there.

## Web Page Rendering for EIP & ERC

**Pooja** [4:47]( https://www.youtube.com/watch?v=uaYvYugYLOE&t=287s ): Next item here is web page rendering for EIP and ERC. I believe we could not get to any solution last time in your absence. Well lightclient was on the call and he was in the favour of having a separate web page but unfortunately you weren't there. Sorry I'm referring to Gavin here Gavin wasn't there. So we were not able to make any decision wondering again if you have any new stance that you would like to share where we are on that. My question is with respect to web page rendering for EIP and ERC do we consider two different pages or is it going to be the one page.

**Gavin** [5:37](https://www.youtube.com/watch?v=uaYvYugYLOE&t=337s):  So I think it's probably going to be still be one website but with two very different like. Basically, my plan is one website but each repository gets to control how its portion of the website is kind of rendered and all that stuff so the EIPs can have EIP specific data information on their Pages like for. Basically I want it all to be one website so that users don't have to worry about which website I go on to. And also so that EIPs can all kind of just share one place. But I also agree that each kind of I guess its working groups now each working group should get to decide what stuff is displayed on the EIP page. And what kind of stuff is searchable it allows EIP to be searched for.

**Pooja** [6:39](https://www.youtube.com/watch?v=uaYvYugYLOE&t=399s): Right. So I believe we are going to maybe talk about the working group if this is something that we should decide after getting Clarity on working group. Perhaps we'll come back at it. And I don't see Mat on the call today. So, it would be fine when we have some more clarity and then we come back to that issue. 

## Topic Group

**Pooja** [7:03](https://www.youtube.com/watch?v=uaYvYugYLOE&t=423s): Very well the next topic is topic group and I see Sam joining the call Sam if you would like to maybe share a high level structure of topic group or working group or what is the plan to take it forward.


**Sam** [7:20](https://www.youtube.com/watch?v=uaYvYugYLOE&t=440s): Sure. So I'm kind of working on like a prototype of how I think it should work. Essentially there's one repo per group. And that's pretty much the only change. It looks very similar to the ERC EIP split. But I'm going to get all the tooling working ahead of time and then I'll shop it around for people's approval. Nothing's hugely different from today. Biggest changes are removing the EIP - prefix and the ERC - prefix. So it's just numbers. I've already sent it to Pandapip and to light client and yeah I'll keep you updated as I work on that.

**Pooja** [8:13](https://www.youtube.com/watch?v=uaYvYugYLOE&t=493s): Very well. Thank you for the update Sam. So there was this question with respect to EIP editors and Associates about who are Associates? or is the role associate defined anywhere? Just to make it clear editor associate is not a formal position and it is not listed on EIP-1. This is just to indicate whoever are interested in contributing as reviewer and may aspire to become an EIP / ERC editor one day and this is also being used as a tag on ECH Discord. So they get the required permission and if editors have to make any announcement which may engage Associates as well like they should be informed they can perhaps make use of it. And the sheet that we have added here on the agenda is just an official documentation of which all are available here. So we get a good hang of how many people are with us for this purpose. And people may be able to tag if they know whom to be tagged here for reviewing of their respective EIPs and ERCs. With that perhaps we can move on to the call for input. I see five inputs Call for Inputs are there out of which one should be closed. Sam if you would like to maybe take on each one of them.

**Sam** [9:47](https://www.youtube.com/watch?v=uaYvYugYLOE&t=587s): Yeah I can run through these just open all these up here. All right so starting off with The Accidental function in ERC-223. Right now it looks like everybody's who's commented is in favour of this. This ends tomorrow and this will merge pull request removing an Accidental function then we have ratify editors listed in EIP-1. The deadline for this one is November 19th and this is basically to formally welcome Gajinder and Ben as Victor sorry as official editors so there's no more question about that. So far it looks like we have two votes in favour. Then we have removed external implementations from ERC #20. The deadline is November 19th. There's been quite a bit of discussion on here. My preferred option I think at this point would be to move the reference implementations into the assets directory and otherwise make no change. 

**Gavibn**[10:56](https://www.youtube.com/watch?v=uaYvYugYLOE&t=656s): Well that's that might be a bit tricky with. I'm not sure. I'm pretty sure one of them is unlicensed.

**Sam** [11:06](https://www.youtube.com/watch?v=uaYvYugYLOE&t=666s): They're both in repositories with an MIT license file at that commit.

**Gavin** [11:11](https://www.youtube.com/watch?v=uaYvYugYLOE&t=671s): Okay good then there's no issue with that well I mean except for the fact that I would rather everything in the EIPs or ERCs repository be CC0. But I guess that's hard to do even when even EIPW isn't CC0.

**Sam** [11:27](https://www.youtube.com/watch?v=uaYvYugYLOE&t=687s): So would you be okay with moving them in?

**Gavin** [11:34](https://www.youtube.com/watch?v=uaYvYugYLOE&t=694s): That would be vastly preferable to what we have right now.

**Sam** [11:38](https://www.youtube.com/watch?v=uaYvYugYLOE&t=698s): All right okay. Okay so I'll make a note for that. So we have the withdraw EIP 7199 and we have two votes in favour of that and that ended yesterday. So that looks like we will be merging that pull request. We have November 30th deadline for add security consideration to ERC 1271. So if anybody listening can go and leave your comments on there. It's kind of an important one. and then we have an informational EIP that is created describing apparent flaws in the ERC 20 standard again kind of an important one to leave comments on. So please go and do so. And yeah, I think that's it for Calls for Input. 

**Pooja** [12:44](https://www.youtube.com/watch?v=uaYvYugYLOE&t=764s): Awesome I am confident that this will help us get to a decision sooner rather than later. And with the deadline we must have a decision by the end of the deadline. So yeah this is helpful thank you Sam. 

**Gavin** [13:01](https://www.youtube.com/watch?v=uaYvYugYLOE&t=781s): Well the deadline very specifically anyone that hasn't responded by them basically then doesn't get to have a say that's what the deadline means. Ideally everything should be a we should have input from everyone by the deadlines. But that has well even Alex just I'm pretty sure Alex actually hasn't responded to. I think there's one or two that he's responded to. But yeah so far that's not what the deadline has turned out to me. 

**Pooja** [13:36](https://www.youtube.com/watch?v=uaYvYugYLOE&t=816s): Whenever we are creating this Call for Input I know,  the link is always shared on respective Discord for editors to follow and maybe leave a comment whenever they get a chance. Do we think if we add them in the call for input may be helpful to grab their attention sooner rather than later?

**Gavin** [14:01](https://www.youtube.com/watch?v=uaYvYugYLOE&t=841s): I think that right now the problem is just that Alex is currently working on other stuff. And well for example I'm also working on other stuff specifically getting my development environment ready on this new operating system. But that also means that oftentimes there's a few like there's a few of us that just aren't keeping track of everything that's going on. So I'm wondering if it might make sense to reduce the amount of time needed before. Basically if it might make sense to reduce the four weeks down to three weeks. 

**Sam** [14:52](https://www.youtube.com/watch?v=uaYvYugYLOE&t=892s): oh just like making them faster.

**Gavin** [14:55](https://www.youtube.com/watch?v=uaYvYugYLOE&t=895s): Making them slightly faster. 

**Sam** [14:57](https://www.youtube.com/watch?v=uaYvYugYLOE&t=897s): I like the long period period and I kind of picked it long to encourage people to remove inactive editors but that didn't go very well. So yeah.


**Pooja** [15:10](https://www.youtube.com/watch?v=uaYvYugYLOE&t=910s): I think this four-week period also give us the opportunity of that particular call for input being mentioned at least twice in EIPIP meeting.

**Gavin** [15:21](https://www.youtube.com/watch?v=uaYvYugYLOE&t=921s): That is true. The annoying thing right now is that this basically anytime a somewhat major decision needs to get made it the current system means that it can't actually happen on a single call. If there is a clear consensus because we actually have to. Well I guess we don't have to I guess Sam can just decide okay consensus has been met but like.

**Sam** [16:00](https://www.youtube.com/watch?v=uaYvYugYLOE&t=960s): No there's a line that says every editor is entitled to be heard before the keeper makes the determination.

**Gavin** [16:06](https://www.youtube.com/watch?v=uaYvYugYLOE&t=966s): Except that hasn't happened for several of them now because Alex just hasn't shown up.

**Sam** [16:12](https://www.youtube.com/watch?v=uaYvYugYLOE&t=972s): Yeah. So it goes like you have 30 days and you can't make the decision until everybody's expressed their opinion and then after that it's the Quorum is reduced to the people who have responded. 

**Gavin** [16:25](https://www.youtube.com/watch?v=uaYvYugYLOE&t=985s): Yeah that I remember now.

**Sam** [16:27](https://www.youtube.com/watch?v=uaYvYugYLOE&t=987s): Yeah. No, I made it to be very very annoying because I think it would be much better if everybody would answer as soon as the Call for Input went up or as soon as we were on the call but you know that's not how this works so.

**Gavin** [16:46](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1006s): Yeah I think it really does seem like there should probably be some system. Well I guess we do have a system that makes lots of smaller changes faster and that's like I guess EIPs are just an example of that. But like we I think we need kind of more Pathways to make more minor changes Faster.

**Gavin** [17:16](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1036s): Yeah I think that's
Fair.

**Pooja** [17:25](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1045s): All right. We can perhaps update the Proposal of the EIP as we get to a point where we need to have a smaller duration for call for input. Maybe specifying that under a criteria that is time sensitive. it could be done in future if needed.

**Gavin** [17:46](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1066s): Maybe like for example change that can be easily reverted. Only requires two weeks and then there's an additional four weeks after it's merged where any editor can object and then bring it back to a call for Input.


**Joey** [18:03](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1083s): Yeah I like that it could even be like by the next EIPIP meeting or something as long as there's a couple days of grace if it's something really so reversible or small. Just an idea.


**Gavin** [18:18](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1098s): Like for example say up like a rather during a final EIP like that's pretty minor change in Grand SCH of things and can be easily reverted. And so I think that would be a good category for like we only need two weeks of deadline. And then an additional four weeks after that where basically an editor can object and bring it back to a call from. Sam? 



**Sam** [18:54](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1134s): My only concern with that is like for things like assigning an EIP number or like irrevocable changes like that.


**Gavin** [19:03](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1143s): That's what I'm saying. This would only be applicable for easily revertible changes and changes that don't leave a side Effect.


**Sam** [19:11](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1151s): Yeah. I think that'd be okay um I think we could work something out like that and put it in the EIP. 

**Pooja** [19:21](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1161s): Sounds good.


**Vladimir** [19:23](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1163s): By the way I think it will be a little bit in line in what  what we will try to say later in the call so this is great direction.


**Pooja** [19:35](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1175s): Right and I think we are almost there I just wanted to make one final comment before we move on to the next topic. Gavin, if you have any specific example of this use case that you are talking about. It would be really helpful to be added in the EIP. I mean like for some event to maybe come up with the idea. And we will have a reference like why we want to have this thing included in the EIP thing.

**Gavin** [19:59](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1199s): So for example there's a few of them like one the creating of the informational describing the issues with the ERC 20, the create, the withdrawing, of one of those EIPs. These are things that can be easily reversed. And also there and also don't leave a side effect. And therefore I think can be merged a bit quicker. And then if it turn and then that kind of I forces editors to actually pay like forces editors that don't agree with it to.  Then say that but it also means that we can make the changes faster. 

## security-related EIP modifications Ref. comment and here

**Pooja** [20:43](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1243s): Sounds good. Well thank you. And with that I think we are good for call for input topic today. And the next one is security related EIP modifications. There is this comment by Dex and I have added the link to the comment as well as a response by another user, Andrew. I know that we are joined by team to maybe talk about this particular topic. So if someone from the team may be like to summarize what they are proposing and then we can get it for discussion for EIP editors here.

**Vladmir** [21:25](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1285s): Okay. So I'm Vladimir,  I will most likely represent the, let's say, business or like main overall direction position and Yuriy and Dexaran, can be more from technical perspective. So the main idea is basically coming from experience and from where we see everything is heading this is more security. And more definitely more Cyber security implementation. So from this perspective I come from the country that is part of European Union. And it's visible that there is basically movement for every company in Europe to start Implement more and more security implementation to be in line with guidelines that are provided by EU or the state where you are based. So why I'm saying that is that there is possibility. And we can see it more often a good example is Microsoft. Imagine that Ethereum is in a position as Microsoft. I think it's not far-fetched because you are providing a platform to developers. the developers are doing their products on top of your platform and are also working in line of your guideline or your processes.  Right now we don't see a reasonable way how to affect already known security issues in the EIPs. Because they are final if they are final there is basically no way to reopen them or it's extremely hard to show to the users that this has known security vulnerabilities. So the main idea is basically be able to have this information to be shown to end users or other developers because from what we saw quite often is if you have final EIP. People usually will take it as a template and they will use it in their projects later on and if there is no information on revealed already known security issues with the code that is in EIP. Then basically nobody knows and the actual developers will use the already known security issue. And they will continue basically spreading the already known problem. Because for what we can say quite certain is that always there is a good analysis of all these hacks or issues security issues so we know what are the issues is we cannot say like we don't know or who can know that like it's known that the EIP has security issue. The problem is nobody kind of knows about it or it's extremely hard for people to see it. So this is the main Direction why we are trying to propose. It has many possible benefits and it has also some risk involved if the platform will not do it one of the main risks.


**Gavin** [25:11](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1511s): Just a sec what is the solution you are proposing? You were talking about what kind benefits the solution would propose would you mind actually going into what your solution is first.


**Vladmir** [25:28](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1528s): So, okay, I can go into the solution. So I thought it's quite clear. So if I understand it correctly after EIP is final there is basically limited way or almost no way how to adjust or put.  Yeah so this is process that is simply either incorrect or or wrongly designed because it doesn't respect the fact that the EIPs and any program or anything will change in the time and if we know already that the code is faulty and is imply wrong. Because we know that it is as I said then there needs to be a way how to reopen it and possibly comment it.

**Gavin** [26:13](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1573s): So I would say what is the solution I prefer to see. So first of all I need to establish what EIPs for EIPs are basically a way of making sure that basically once you implement something then it's almost like a label as long as your smart contract implements an EIP correctly. Then other contracts can expect that that well that contract will implement the EIP. So in terms of actually modifying final EIP I don't quite like that. In term but I do agree that there are now multiple instances where an EIP has had flaws. That means that it shouldn't be used. So I'm wondering if what we want to do is make another working group but that working group is unlike any other working group in that it is explicitly like it does issue recommendations. So as a whole the EIP project does not issue recommendations. The existence of an EIP does not mean that basically it's a good idea to use It. The existence of an EIP is just a way that you can ensure our operability. However people have been I will fully admit people have been using EIPs as almost a way of oh if this is published then it's safe. And so we need, I think at this point we do need a way to communicate to readers that there are probably better options available. And so possibly an opinionated working group might be a good idea. 

**Vladmir** [28:16](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1696s): So as you said there are many quite complex how to do it obviously what we are trying to achieve is to start this discussion and most likely the implementation can be more complex because as you said either we can put a label there so this doesn't touch actual EIP finalization. But there is information provided to the people hey there is something wrong here maybe you should take a look on the updated version of the EIP or ERC. And so there are many ways how to tackle it I don't think we can give you straight away all the possible solutions but one of the solutions is obviously ability to reopen. I do understand why this is not liked idea because obviously if you can reopen something you can change it then you need to have then you are basically ending with the question who is guarding the police. Yeah, so, I know it's a really difficult discussion but there are many solutions one of the solution is basically being able to put some label or some note that is on top of let's say this EIPs or things basically to say we in this in this particular EIP.  We know that is this security vulnerability and please be aware of that. The reason why I said the example with Microsoft is that it's actually quite good comparison because you are providing the platform. And in the end who if the users are damaged and the money is lost or or stolen in the end who will be responsible obviously. What we think right now is that the responsibility lies solely on the developers. And they are responsible for them what they write but in the end the platform needs also to be able to explain why and how they did everything possible to to help the people to at least take in consideration that these risks are there.  

**Gavin** [30:39](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1839s): So again the purpose of EIPs is not to endorse specific standards it's simply to provide labels that allow things to interact with each other no matter how bad those interactions like like no matter how like not like no matter how flawed those interactions are. 

**Sam** [31:03](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1863s): Yeah you're kind of saying like if you implement ERC 20, even if ERC 20 turns out to be completely broken and horrible somebody can come along and know how to use your ERC 20. You know 30 years.

**Gavin** [31:15](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1875s): So that is what the goal that is kind of what the EIP project is. In terms but I will not deny that people have been arguably Miss using it as an endorsement of a specific standard. And in that regards I think that we can do better to communicate to readers that something is flawed. And a few things that I can think of doing off the top of my head that would require almost no effort on our part is make the security considerations. And always editable post final any modifications to the security considerations are Rob. No matter what they are as long as they are true. Second thing is move that security considerations way up if they are important. So if there is a really glaring issue then we should move the security considerations above. Even the abstract, so those are kind of two things that I can think of that wouldn't require much work at all. And I think it would definitely be a good benefit.


**Sam** [32:26](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1946s): So I'm definitely starting to come around and I think that we do need something. You and Dexaran have convinced me for sure but is just how to implement it. And I think in a way that keeps the EIPs process. You know true to its goals and I think right now my concern with what you suggested panda is that if we edit the security considerations like who is supposed to decide whether an edit is allowable or not like if it's the author and the author doesn't want to reveal the security vulnerability because it will you know hurt their NFT Marketplace like stock and they they keep blocking the Pull request are they allowed to do that do EIP editors need to make that choice. 

**Gavin** [33:15](https://www.youtube.com/watch?v=uaYvYugYLOE&t=1995s):Let the EIP editors make that choice make it clear that EIP editors are making that choice.


**Sam** [33:22](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2002s): Then that puts us in a place where we have to make decisions that we could like we some of our credible neutrality if we do that.

**Vladmir** [33:29](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2009s): So I think I don't agree that you will lose any credibility. Obviously that you need to have a little bit credibility.

**Gavin** [33:39](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2019s): Credible neutrality it's slightly different basically the pro the process is designed so that EIPs again are just label that can effectively be applied to compliant smart contracts. Something is compliant or it is not. What what the problem is that this kind of is that what I'm suggesting does admittedly go outside of the scope of what the project is for. The project is not for kind of determining what is good practices no matter how obvious those good practices may appear to be. I do think that we can so again what I've suggested is making another working group that is explicitly not credibly Neutral. 

**Sam** [34:30](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2070s): Yeah and I think that'd be acceptable.

**Vladmir** [34:35](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2075s): I will just give you some notes from let's say outside perspective because I'm a little bit less involved with the on-going process but from my perspective like I see EIPs as a template basically to be used obviously what you are saying makes sense. I don't know if anyone is actually aware of what you are saying it makes sense. It's basically repository that needs to basically track so in 10 years you know how it was done but the question is if basically everybody sees it differently. If it's better to basically adjust and do what is let's say expected how to do it as you said is, I think the options that you can do obviously. You can see I think a little bit better than for example me but I think that there needs to be done something how it's done. I think you are right it's extremely difficult to have a process where basically you only store information how things were done. And that's it and something that is updatable or comment able where you need to have some judge basically to decide if I push this button and then announce that this nft marketplace has a security issue. Therefore possibly damaging and if it will happen that this Marketplace didn't have security issue. And it was just false alarm then this can be quite big issue obviously. So yes there are many things that  you that needs to be considered I think the main thing was to basically bring up the topic  and open it discussion because we do believe we have experience to basically be part of the discussion and possibly give you some good proposal that obviously you will adjust as you as see it.

**Gavin** [36:44](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2204s): So I think we can probably model a bit of this on what the ITF does so the ITf's working groups are literally working groups so kind of there is a working group responsible for for example the ACT specification part of The Proposal. One for the security considerations part of part of Proposal etc. I think we can start doing that and taking effectively the security considerations out of the EIP and into its own working group and I think the security considerations working group should not be explicitly credibly neutral. I think the security considerations the working groups don't necessarily need to be credibly neutral right just the editors do. So I think that works. So if we create a security a working group with the only goal of determining what should be done with any given EIP security consideration whether or not it should be moved to the top or left its current situation what changes should be made to it post final. And let's be perfectly honest. I don't think that the process should for adding is or editing the security considerations like editing the security consideration section should not depend like the process should not depend on what stage the proposal is at except maybe in draft. So because if it's if there's a security consideration it doesn't matter if it's in review last call final or even a living it should have the same process except maybe other should have an easier time disclosing vulnerabilities.

**Yuriy** [38:36](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2316s): Maybe we can add a section like security reference it not will be so strictly like consideration. We will public in the reference links to the security company or Security Experts who describe issue in some EIP. If they found or insecurity reference can be public audit information that this EIP was checked by security company and was confirmed that this EIP is have no big issues for example. 

**Sam** [39:12](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2352s): So something like that would probably go on a Wiki like I think that kind of a format would be great for collecting security considerations.

**Gavin** [39:21](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2361s): So I'm wondering if what we want to do is basically take make EIPs literally like the actual EIP part of the EIP literally just the abstract. And the security considerations and maybe also the test cases so we take so that is what the EIP itself is and then we take all the other sections the security considerations motivation rationale, reference implementation, against copyright section goes in the regular EIP bit and then we take all of that and we make that a Wiki. 

**Vladmir** [39:59](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2399s): Also like if you will consider the the actual solution. I think it's extremely good if there will be a place where different in like. I will give you good example something was hacked we know usually one day after why it was hacked. And we usually know what vulnerability was used maximum in a few days there is no doubt about that about that because there are many companies working on Ethereum doing different analysis of these hacks Etc. So that is definitely a good thing in this. But the question is how this information will be provided to users  or specially developers. So, for example if I used ERC 20. And I know it's a part of my code how I will receive notification or how I will receive the information that something  changed. And that because in if it's part of a then obvious if the EIP status will change I will receive notification straight away from the GitHub no so this is basically kind of semi-automatic. 

**Gavin** [41:14](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2474s): So I think what the easiest solution to that would be is have an RSS feed that is updates to security consideration sections. What do you think Sam? 

**Sam** [41:25](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2485s): I'm thinking what we should probably do is time box this conversation for now. Make maybe a Discord Channel or a thread or something to keep our thoughts on. We'll use the discussion thread that we already have and we list out like what the possible solutions to this are like whether we have a Wiki. Whether we allow modifications to the security consideration section and we kind of sketch out all the different like options. And we we try to decide on that because I think right now we're kind of just brainstorming on a on a an hour long call and I think that's.

**Gavin** [41:59](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2519s): Yeah I think not  Efficient.

**Vladmir** [42:02](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2522s): Yeah, you are correct I think what we wanted to do is mainly to open the discussion. If you are open to the discussion I think it's exactly what you said the solution most likely can be completely different from what we discuss right now. And needs to be discussed in some open format. so if we can join the group and put the ideas there. We are happy to do so.

**Gavin** [42:26](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2546s): You guys are in the Etherum capitals Discord right. Okay. Great.

## Changes to Final proposals

**Pooja** [42:35](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2555s): All right. So I see here in the chat Dex has also shared the link to the fellowship of ethereum magician where this proposal is active. People may find the link in the agenda today and may perhaps leave their comment and thoughts on this on any possible solution to this proposal for security consideration. With that I think we can perhaps move on to some of the open PRs which are with respect to final proposals. I see a bunch of proposals added here and most of them are from the earlier call. So I wonder if any editor has any thought on any like any proposals to be allowed or not. The number one is ERC # 49 which is for ERC 223 remove standard Function.

**Gavinr** [43:33](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2613s): I'm pretty sure the deadline for that is tomorrow. If that if and so far I think we've got two approvals and let's See.

**Pooja** [43:47](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2627s): Yeah.

**Gavin** [43:48](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2628s): This is an example of where I would like that two week deadline that can feed.

**Pooja** [43:54](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2643s): Okay so just for the summary of this call do we want to keep it on hold because there is one more day left or is there anything that we can answer it as a solution to this PR or maybe next Step.

**Gavin** [44:10](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2650s): We should. Sam are you willing to merge this tomorrow if nobody objects.

**Sam** [44:17](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2657s): Yeah I'll do that.

**Pooja** [44:19](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2659s): Merge It,  tomorrow if nobody objects.  Okay the next one here is update ERC 2612 which is which seems to be like a small typo and the PR number is ERC #57.

**Gavin** [44:40](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2680s): Yeah this is I'm pretty sure this is correct.

**Pooja** [44:45](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2685s): So we can allow Merging.

**Gavin** [44:49](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2689s): Yes. so annoyingly this is in the spec but this is fine I think. Actually hold on.  So I'm pretty sure that there's so it first of all I think it's pretty clear what the original intent was. Second I actually you know what I think that this is actually incorrect wait is it hold on. I need to actually check the when he's back here.

**Pooja** [45:31](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2731s): I think Joey is on the call who is the author of this. Joey if you have to add anything here?

**Joey** [45:39](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2739s): Yeah sorry what was the question for ERC 262?

**Gavin** [45:43](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2743s): I'm just double checking that the function name is correct?

**Joey** [45:49](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2749s): Yeah. I believe the function name is called allowance not approval for the mapping that I mean it's not even it's kind of weird because in ERC 20 it's defined as a function not a mapping. 

**Gavin** [46:10](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2770s): So the fact that It's, So the a mapping become functions with two parameters. I'm pretty sure. 

**Joey** [46:18](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2778s): Right. Yeah. But it was just like you know the way that he wrote.

**Gavin** [46:24](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2784s): Style choice but yes this can be merged. This is a very obvious.

**Joey** [46:31](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2791s):  Cool. Yeah thanks.

**Gavin** [47:07](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2827s): Okay Sam, do we have any more. 

**Sam** [47:23](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2843s): Yeah the next one is ERC 1363 fix created date.

**Vladmir** [47:36](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2856s): I think from my perspective if it's all and if anything I will be obviously on Discord or Forum to be reached something it's needed thank you for consideration and bye-bye.

**Pooja** [47:50](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2870s): Thank you. All right so the next one is a 1363 which has actually 4 open PRs number are 66, 74, 75 and 76. All with respect to one proposal which is ERC 1363.

**Gavin** [48:11](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2891s): I'm not sure about the Creator date. I don't think there's any precedent for what the Creator date is. And therefore I don't think it should be changed since it's Final. 

**Sam** [48:21](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2901s):  Oh I mean they created date like it was it was an issue before so.

**Gavin** [48:25](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2905s): Yes I know it's issue we don't I will fully admit here the created date in EIP-1 is just completely underspecified since EIP 1363 is final I don't think we should be changing it the Created Date. 

**Pooja** [48:42](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2922s): So it's a field in Preamble. We should use that right why do we want to change it.

**Sam** [48:49](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2929s): Oh so the created date was set to when it was upgraded to an a markdown file as opposed to like it was a draft issue created long before that so.

**Gavin** [49:01](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2941s): I guess you can see what 223. ERC 223 okay they used 20 the issue created date okay yeah sure this is good.

**Sam** [49:14](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2954s): Yeah ERC20 is you know 2015 which is well before the using markdown. So sure.

**Gavin** [49:23](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2963s): I'm still not a fan of of updating finals just to change the created date to something different but you know what since this is what most of them are doing I'm fine with it. 

**Pooja** [49:36](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2976s): So I'm just trying to understand here like a created date is a field which is added when the draft was added why was that not updated at the time of making draft.  It could have been easily updated.

**Sam** [49:49](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2989s):  So the draft was created as an issue that's in 2018.

**Pooja** [49:57](https://www.youtube.com/watch?v=uaYvYugYLOE&t=2997s): Why I mean there must have been there must have been a draft in markdown and in that they can add any date if they want to keep the issue date. 

**Sam** [50:07](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3007s): As they just put the wrong date when they made the markdown file.

**Pooja** [50:11](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3011s): Okay I don't see any as of now I don't see any advantage of changing that date any significance why they want to change it except for history purposes if they want to keep it there.

**Sam** [50:25](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3025s):  I think it's just a like it was one of many modifications they're making to the EIP and this is the only one I thought was reasonable. But yeah.

**Gavin** [50:38](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3038s): So I think also this kind of ties into that that created date it's just like completely arbitrary like EIP-1 says it's the date at which the proposal was created like this unclear is it the date at which it was merged when it was first conceived when it became an original issue or a Pull request like it's just arbitrary. And I think yeah it most of them have been the issue creation date.

**Sam** [51:14](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3074s): Yeah. It's the earliest date a relatively complete document has appeared on the EIP repository. I think is the rule we go with about magicians.

**Pooja** [51:27](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3087s): I think that would create a lot of confusion. We should be clear here and created a date is a field which is to be filled by the author if they want to keep the created date as the initial date of when it comes to their mind they can add that date. We should not go ahead and change it like let's keep what author propose it when they are creating the markdown for the first time and whatever date they enter we respect that that is is what I'm thinking it would be the right thing to do here is because I know the confusion about the created date because I was trying to create a chart where we are trying to find how much time did it take from one proposal to move from draft to final. And there are two created date here one is the date what what is added in the Preamble field. And one is the date when it was actually merged and there could be a month of difference between these two. But what we are trying to do here is like whatever created date they have added as in the field of Preamble should be considered as a created date. 

**Gavin** [52:31](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3151s): Okay how about  first like the date at which the the EIP editors were first made aware of it.

**Pooja** [52:45](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3165s): That's making the PR date.

**Gavin** [52:48](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3168s):  Well except it also is work for things where there's not actually a PR which was the kind of previous way of doings.

**Pooja** [52:57](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3177s): But that could be very confusing many editors could not get notification of that right. So first time they get notification.

**Gavin** [53:05](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3185s):  Specifically like like when when a notification is kind of the date at which the notification was send basically like so this this doesn't whether or not the editors actually check it does not have an effect on when it was actually sent.

**Pooja** [53:24](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3204s): So if we try to collect this piece of information with respect to GitHub I think GitHub action Bots provides US history when the PR is merged. Yeah when it is merged or when it is created. 

**Gavin** [53:38](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3218s): Also think we should try to avoid depending too much on actually GitHub as the flow for what we do I think that whatever we have in the EIP-1 should not depend on there actually being such a thing as a pull request that is required to submit any EIP. I think it should be I think Pull requests and all this should just be implementation details.

**Pooja** [54:05](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3245s): Right and while creating pull request this is the opportunity with author they can input whatever created date they want to add their I don't Ihave never noticed any EIP editor creating an objection on the date of creation based on like why is it different from.

**Gavin** [54:21](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3261s): But this is completely arbitrary. 

**Pooja** [54:24](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3264s): Yeah they can did Arbitrary.

**Gavin** [54:28](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3268s): Like I'm pretty sure that my that my first EIP 4834 has a created date that it's two days before the actual date I submitted it because I made a typo.

**Pooja** [54:46](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3286s): Alll right let's get back to the this PR here do we want to add it update it I see there are bunch of other updates considered for this particular EIP. So if you want to make it a part of it can be done but I Just Want to Be watchful of creating this as an example that anybody in the future can come back and say that my issue was originally created, whether it was not with respect to the PR.

**Gavin** [55:16](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3316s): You know what I'm in favour of changing the Created date on this proposal. And I also think that the authors if they strongly agree with it should be to change it back because.

**Sam** [55:32](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3332s):  I think the authors were the ones who originally proposes change. 

**Gavin** [55:35](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3335s): So okay then yeah this is a no-brainer then.

**Pooja** [55:39](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3339s): Right yeah if the author himself wants to do it we can perhaps allow it but yeah we should be mindful of this kind of situation.

**Sam** [55:46](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3346s):  Yeah the authors approve the Pull request. 

**Gavin** [55:48](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3348s): Okay then yeah absolutely let's do it. 

**Sam** [55:52](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3352s): Yeah I don't yeah I'm just going to pretend this is not controversial and we're going to go for a merge on that. 

**Pooja** [56:02](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3362s):  I think there are 2 or 3 other open PRs with respect to this EIP so if we can make decision on that perhaps we can mark this item as completed. So the next PR is 74.

**Gavin** [56:22](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3382s): This is how much of this is actually Rewritten I'd say that the Rewritten version is actually just way better stylistically but unfortunately it is also Rewritten. Yeah like the description and the simple summary don't actually match up although that's partially because you can't have markdown and because the simple summary was just bad. Oh gosh what was their former abstract okay I'm in favor of this just because how just because of how poor the original content is that's appalling and being hyperbolic but like. 

**Sam** [57:19](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3439s): Yeah this is just better writing anyway yeah but that that's kind of goes against the spirit of changing a final EIP right like. 

**Gavin** [57:26](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3446s):  This one's Tough.

**Pooja** [57:33](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3453s):  All right so.

**Gavin** [57:35](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3455s): You know what I  don't think it creates any incompatibilities here is just a rather larger. It fixes some bad style Choices. Sam, what do you think?

**Sam** [58:01](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3481s): It's final so I'm generally against editing it and if they want to publish a new version with you know updated text they absolutely can.

**Gavin** [58:18](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3498s):  Okay how about we recommend to the authors to the author of PR number 74 that they split this into first of all split it into things that are actually necessary like moving the simple summary to the description updating the discussions to URL. These are things that I think are good and should be merged. Do you agree Sam?

**Sam** [58:48](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3528s): I don't know if changing the discussions too is necessary but I mean. 


**Gavin** [58:53](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3533s): it's just not the correct link any anymore.

**Sam** [58:57](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3537s): That if people want to see the historical discussion for this EIP it is the correct link.

**Gavin** [59:01](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3541s): Well except the historical discussion oh is there actually anything on the updated Ethereum magicians link or is it just stub.

**Sam** [59:10](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3550s):  Well that's what I mean like I think the old.

**Gavin** [59:13](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3553s): No there's actual  historical discussion that's of is there no there's not okay considering there's not actually any discussion on the new link that's not on the original link. So I'm against updating it to the new ethereum magicians link because that wasn't actually where the discussion took place in terms of moving the simple summary to the description as long as no changes are made apart from removing the markdown because there is no mark down in Preamble that I think is okay in terms of any other obvious fixes as long as it's an obvious fix. That's fine I would also like them to submit another PR that actually not does of this changing and ideally section by section so updating the abstract and updating the modification. Because I do think that the writing of IRC 1363 is not the strongest. And I would like to see it changed especially since it look let's be again I'd say the purpose of the EIP project is to kind of create specifications that can be applied to different programs to enable interoperability if modifying a final EIP does not conflict with this Mission and in fact makes it easier for potential implement to kind of understand what the proposal is all about I think we should be allowed to modify a final EIP.

**Pooja** [1:01:05](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3665s): That's kind of vague statement like people can interpret it differently. We need to be explicit about what are the conditions under which it can be allowed because if the like you know if the potential user should understand it better then we may have to end up updating a lot of EIPs.

**Gavin** [1:01:27](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3687s): I do agree here. So we do need to be explicit about it I'm just throwing this out here should we be allowed to modify final EIPs to make the content easier to read because it will help implementers in the primary objective of the EIP project which is to enable operability.

**Sam** [1:01:48](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3708s): No I don't think we should I think if somebody wants to take the spirit of this EIP like the same like if somebody wants to specify the same thing as this EIP with different words they can just make a new EIP for it.

**Gavin** [1:02:05](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3725s): So arguably it's just the same label though right because I'd say all EIP is just a label that can be kind of applied to something that's compli.

**Joey** [1:02:17](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3737s): Yeah I'd like to understand the thought process Sam behind your no just so that we understand the principles that we're discussing this under.

**Sam** [1:02:28](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3748s): Oh sure. So the EIP is supposed to be immutable and whether the wording is exactly the same.

**Gavin** [1:02:36](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3756s): Understanding quickly why you feel like the entire EIP should be immutable.

**Joey** [1:02:41](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3761s): Mutable of content or immutable like immutable of text or immutable of the actual spiritual content right.

**Sam** [1:02:49](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3769s): It's like of the law yeah so absolutely immutable sorry go ahead panda.

**Gavin** [1:02:54](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3774s): Because again I do agree that the actual EIP the like the main part of the EIP itself. What the EIP is and even it's like the details in the specification. The specification not the text itself but the specification should be immutable what should not be immutable is the actual text itself because the EIP can still be the same EIP but with different text.  And one of these ways is kind of just the EIP in my mind is what is trying to be conveyed by the document itself not the actual document itself.


**Pooja** [1:03:39](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3819s): Well I think we should try to wrap this up here. I am sure we are not going to get a solution until we have some more thoughts collected from editors who may not be able to make it today. Would it be okay to have it added to the next meeting agenda. And like a specify conditions under which a final EIP can be considered for changing. 

**Gavin** [1:04:01](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3841s): Yes and I think we should also kind of create almost like a more general thing of like what constitutes the EIP itself. Because I think we should all agree that EIPs themselves once they are final are mutable but what the actual EIP like what are the parts of the EIP, that are essentially the EIP and what are the parts that are just kind of helping the reader to understand the EIP and by the way Sam, at some point I'd actually like to just have like a one-on-one conversation. So that we can try to find some consensus here.

**Sam** [1:04:45](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3885s): Yeah sure.

**Pooja** [1:04:49](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3889s): Very well. So I will go ahead and add that for discussion in the next meeting and I would request EIP editors to maybe take a look at the other open final proposals if they have any thoughts they can perhaps add it. If we get a consensus on the pull request itself we can make a decision on merging it on the next call otherwise we can definitely bring it up for further discussion. I'm trying to just look over other items if there is anything of higher importance that we might want to discuss. I think there are a couple of other items with respect to renaming of ERC office hour and things but we don't have time. How about we decide on the next meeting time this was not our usual meeting time our usual meeting is 1400 UTC but this day for today we made it 1530 UTC. As I can look into the time for the next meeting which could be on November 29th. I see it is in conflict with execution layer P2P breakout what is a our stand on that. Where do we want to have it? Do we want to have it after that meeting ends? Or yeah any suggestion here.

**Gavin** [1:06:02](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3962s): So in terms of moving it forward that would be less convenient for me but I could do it in terms of moving it backward I cannot actually I can't do it any earlier than the normal time.

**Sam** [1:06:17](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3977s): I'm not attending the execution layer P2P meeting. So I don't really care if it.

**Gavin** [1:06:21](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3981s): I'm not attending it either but I imagine that problem if there is a person here that we do need to have on the meeting it's Light client and I imagine that Light client will likely be attending that meeting. I don't want to assume but.

**Pooja** [1:06:37](https://www.youtube.com/watch?v=uaYvYugYLOE&t=3997s): And I see that after that there is EUF meeting so both, 1400 and 1500 slots are booked by other calls so if you want to make it, 1600 I can perhaps do that if it is not inconvenient for anyone present today. 

**Gavin** [1:06:52](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4012s): Hold on let me check time zone.

**Gajinder** [1:06:59](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4019s):  1600 works fine for me.

**Pooja** [1:07:03](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4023s):  I was concerned for you specifically Gajinder singh but thanks for giving a green check there.

**Gavin** [1:07:08](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4028s): So this is 1600 UTC.

**Pooja** [1:07:11](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4031s): Yeah 1600 UTC will be 11:00 a.m. eastern time. 

**Gavin** [1:07:15](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4035s):  I am no longer Eastern time I'm central time but yes I'm that is good for me.

**Pooja** [1:07:24](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4044s): Perfect Sam does that work for you also?

**Sam** [1:07:28](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4048s): Yeah that is pretty open for me so.

**Pooja** [1:07:32](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4052s): Okay so let's try to avoid the conflict. Hopefully we get to join by Matt as well. So we can decide future meetings. But for the meeting scheduled on 29th let's keep it at 1600 UTC sounds good to me thank you everyone for joining us today and staying a bit longer. I know this is not the usual of the call but yeah thanks everyone see you around have a good one.

**Gavin** [1:07:59](https://www.youtube.com/watch?v=uaYvYugYLOE&t=4079s): Thank you very much have a good day thanks everyone.

-------------------------------------------------------------------------------------------------------------------------------------

#Attendees
* Yuriy K
* Pooja Ranjan
* Tio
* Vladmir Venca
* Dex
* Gavin John
* Gajinder
* Joey Santore

### Next Meeting Date/Time: November 29, 2023 at 16:00 UTC

