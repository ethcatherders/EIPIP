# EIP Improvement Process Call #1 Notes

### Meeting Date/Time: Wednesday 15 January 2020, 15:00 UTC
### Meeting Duration: 1 hr 
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=ZW3AWJD6cmI)
### Agenda
* Introduction of participating members
* Previous discussion
* Tools to be used
* Next steps 
### Moderator: Hudson Jameson
### Notes: Pooja Ranjan


----
	
# Summary
* We need more understanding of how to update an EIP in general and document.
* The current process does not need an overhaul, certain documentation, and increase in communication may add value.
* Mentorship program
* Document best practices
* Define processes for different categories of EIPs
* Have a different groups of editors as assistants and administrators. Define the scope of what an EIP editor should be doing.
* Order those list of problems in the [document](https://docs.google.com/document/d/1KzEMD21Joqn7IWk4WnocwraRuo66y7r2w8R9Wml4BN0/edit) and vote up and down to prioritize issues.

### Concerns
* Plenty of unattended EIPs with no clarity of to be or not to be addressed.
* Earlier EIPs were more of a good idea now, its just documenting specifications.
* No one really does the decline option if EIP is not of use anymore.
* There are very few people who actually want to push things
* Struggle with the process
* Async selection of EIPs for an upgrade. EIPs which is not being pushed/championed by anyone is being pushed over the EIPs of people who are actually currently working
* Delay in accepting useful EIP 
* What kind of process you have for revising the EIP?
* EIP1 is a specification versus a guideline


### Suggestions
* EIPs should have the 'Scope' section.
* Document what is needed in an EIP.
* Clear the backlog of PRs and issues.
* Define the 'archive' timeline.
* Add expiration dates on the EIP.
* Have a good policy to close the PRs.
* Reach out to Bitcoin, Zcash and Ethereum classic to understand their process
* Reduce frictions for the individuals that want to participate 
* Bring a mentor program
* Have a different group of editors as assistant and administrator.



----


**Hudson**: Welcome everyone to the first EIP Improvement Process meeting. For today's meeting, it's not going to be super long but we do want to go over 
* some of what we discussed in the telegram group 
* maybe give some intros for everybody 
* figure out some solid next steps with a Cadence of the meeting should be 
* what tools will be using cuz I had a few in mind mostly Google Docs related tools coming up with a group discussion in certain documents. So yeah I'm going to pull up the EIP Improvement processes meeting doc from Telegram and look through that a little bit while we go through that so then we can talk about some of what's been discussed in there. We'll start with Anett.

**Anett**: Hi! I am Anett from Magicians group, just to see where Magicians can help out with EIPIP process. I'm just to see what we can help, thank you!

**Hudson**: Thanks Anett, next we'll talk to Brent.

**Brent**: This is Brent. I'm with Canonizar the consensus-building in the tracking system.

**Hudson**: Okay, next we have Bruno. 

**Bruno**: Yep I'm with the Web3 foundation, I am here to learn from you guys and maybe contribute something, but mainly as an outside observer and commentator.

**Hudson**: Okay great, Charles?

**Charles**: Hey everyone! I'm with Maker DAO and part of Ethereum Cat Herders. I like the idea of improvement process and am here to see where does it go.

**Hudson**: Okay, next we have James.

**James**: James Hancock, I do a lot of work with the all core devs, a part of hardfork coordination and stuff like that so I am pretty excited to be a part of this improvement. 

**Hudson**: Okay, Louis? Okay, will come back to him. Pooja?

**Pooja**: I am Pooja from Ethereum Cat Herders and I'm here to help out with the improvement process.

**Hudson**: All right Wei?

**Wei**: Hi! I am Wei from Parity, pretty excited to be here. 

**Hudson**: William Entriken?

**William**: I'm Will. I've been running some EIPs  also involved in Solidity and magicians.

**Hudson**: Thank you, William Schwab?

**William**: Hi, I'm also William and I'm here with the Cat Herders and I'm also here basically to see what I might be able to offer the EIP process. 

**Hudson**: Excellent! I think that's everybody has people come in we can also just get them intro but for now let's move on to the next step, which is carefully defining what scope we want to actually tackle using these meetings and using these Github issues, we are going to be opening. **Just to be clear this isn't a dictatorship of meetings to change everything it's basically a way for discussion to happen more quickly and then that discussion to be transferred onto something like GitHub issues or Ethereum Magicians Forums** or something like that so the broader community can participate if they're not able to participate through these calls like at the time doesn't line up or they don't have telegram or things like that. We want this to be very open and accessible to everyone who wants to be involved. 

I think there's a lot of issues that we have with the EIPs. So, let's go ahead and start voicing some of those and then from that we will just go around and start saying the kind of things we think can we improve something like and then from there we can identify the most urgent places to address. 
Examples of this could be 
* I'm confused what the EIP 1 has to do with anything or like 
* this process is an EIP 1.  
* I think it's too hard to get an ERC or any EIP of other type of the EIP approved 
* there's not enough editors and things like that.  So, who wants to go first?

**Will**: I want. I'd like to see a **project scope** for EIPs in general, like why are we doing this? what is the goal of this EIP not to the proposal but the project?

**Hudson**: So, can you define Project scope a little bit better for people who haven't really ever done a project scope?

**Will**: The purpose of project scope is that you can quickly close issues that are out of scope. A lot of people that want to contribute and rather than having sad discussions on, someone thinks if they want to make a change and someone thinks this is not a part of the project. If you've scope you can point to it and you say the reason why we can't do this is because it's out of the scope. There is a lot of discussion on EIP 1, out of this meeting and we'd like to know why are we doing EIPs at all? how's it fit into changes in general? for example when the scope is not clear for this project; such as one where we should not have any state changes that there was like the protest EIP, I think. 

Do we want to have that in our discussion here? is that out of scope? that help us define what are we doing this to track the ideas that are out there or it is just purely technical? I think this has changed, so **in the past, EIPs were about, what changes are good ideas? Now EIPs are more like let's just document specifications**. I think that's more where we are today. I think there's no understanding of that, but I don't think it's written down. so I'd like it to be written down in the clear way that if everybody agrees on it.

**Hudson**: That kind of made me think earlier on in the EIP process in the beginning there was this need and this extends the **vagueness around the EIP process, to make it flexible** and to make it so that there wasn't like this really harsh handed this is how things are going to be and be nice about it. We do want to keep some of that spirit with the fact that there can be multiple people who can make multiple token standards and even though one of them is Final if someone else is in draft you can definitely use that standard and stuff like that. So making sure to avoid words and statements and things within the written procedures and written scope of work for an EIP that would dictate it to be like end-all-be-all for all of the different EIPs that could be submitted is probably not what we should be going for, in my opinion. But it's something that I think people expect out of the process, so I agree that writing down a project scope would be a good idea.
Who's next? Who wants to say something else?

**Pooja**: I can talk about it. When we started this discussion about the improvement process, we drafted something here in the telegram group about the layout of how we should be going ahead. It says like when we are talking about the improvement process we need to consider the issues that we are facing at the time, the problems that we need to identify first in order to actually be able to solve it with the improvement process. We kind of tried to list the existing problems and one of the most important things, it suggests that we need to do is on-boarding of EIP Editors. I think that is going to be an important aspect for this group to be taking care of.

**Hudson**: Excellent! I love that [document](https://docs.google.com/document/d/1KzEMD21Joqn7IWk4WnocwraRuo66y7r2w8R9Wml4BN0/edit) we should look at that and see what we can do about contributing to that. Before we go further, Bob, we did quick intro with everyone. So we can do a quick intro with you as well. you can just say, who you are and why you're excited to be here or what you do or whatever.


**Bob**: Hey guys! My name is Bob Summerwill. I was previously at the Foundation, EEA and ConsenSys. Have been working for the Ethereum community for 4.5 years now. I am now the Executive Director at the ETC cooperative as well. Very interested in EIP process, backing standards, how that fits together? How EEA, EIP, ECIP fits together. This whole process is of lot of interest to me. 

**Hudson**: Okay, thank you. And what we're doing right now Bob is just going around and if you and coming up with things like the ones listed on the sheet that Pooja put in chat. 
**Problems** that they think are **with the EIPs** from like 
* a Meta perspective, an overview perspective, specific issues,
* there's not enough editors, 
* EIP 1's confusing, stuff like that. And we're just voicing those cuz there is some one note taking and we can go back and we can kind of shuffle through those between now and the next meeting and organize them in a document using telegram as a kind of way to organize participation and then the next meeting have like a clear list of priorities or at least something we can finalize as a list of priorities for this subgroup.

So, who else has anything that they want to discuss about? Like if you could have something as a cool angle to all of this whole initiative, what would it be or what's the problem?

**James**: Do you want me to put up the document, like screen share it?

**Hudson**: thank you, that would be great.

**Will**: So practical goal, we could endeavor to **clear the backlog of PRs and issues**.

**Hudson**: Yes that's a good one.

**Charles**: I just have a suggestion, under the existing EIPs which are stale, having a **defined archive** kind of **timeline** for which EIPs within the time line will be archives and the whole mess cleaned up eventually, would be cool. Like six months or nine months, if EIPs is there and has no progress then it gets archived.

**Will**: I agree it's a lot easier to bulldoze through when you have a bulldozer. 

**Hudson**: yeah. next anybody?

**Brent**: I have just a comment. It was mentioned about defining skull, for making rules or anything like that. Just my belief is that consensus can override everything including blockchain State. If you can demonstrate and prove that everyone agrees, that we should do something, that should be done. So anyway just a comment.

**Hudson**: I think that's an important point to bring up is that how much is this group going to define, what it means for something to be under consensus or approved. What generally has been the rule of thumb is that **we leave it up to the "community" and then the EIP editors being more of the judges of when something comes to consensus** more or less is how it's happening right now. I'm not finding huge problems in that except for the fact there's too many EIPs for the EIP editors to go through and the EIP address to go through and approve or decline or things like that and there's also **no expiration dates on the EIP**, that might be something we want. I don't know how much we should focus as a priority on what is defined as consensus but that doesn't mean we shouldn't put the tools out there to make sure that people know about them and can utilize them and maybe give new suggestions and the template to say hey here's some things that are available for you like reach out to Twitter to Reddit use different tools to like assess your community consensus of who's using the tools and things like that.

**Bob**: About how many active EIP are there in the moment? Obviously like  numbers must be a real big problem now.

**Hudson**: yes, I don't have the numbers. When you say active, define active.

**Bob**: well, listed and not resolved. 

**Hudson**: Because of the fact like, **no one really does the decline option** very much, we just kind of lose track or lose sight of wherein there's any EIP. Then there's no archive mode that we would probably want to create. I mean there's in the hundreds if not a thousand or more if someone has to page pulled up they can answer cuz I have my full-screen recording on so I can't pull it up.

**Will**: We've 100 'draft' and then 'defacto draft', pretty specified initially but then not created as a file as a draft. So we're looking at thousands history from years ago but are still getting comments but actually specifying the past few months are about 100s in past few months.

**Bob**: Because I know, in ECIP, we've same kind of process. In some cases we know that the stuff is never going to go through, it's not sufficient quality or it's just a stupid idea but you've got this balance between not wanting to like throwaway people's work but also knowing that it's not helpful to have it. I guess it's a problem like in general in some kind of project like **rejecting pull requests**. Just thinking, not wanting to throw out valuable contributions away but also you have to manage the load and sometime say no. But how do you say no in a consensus process of an open network?

**Will**: I've had two comments on that. We are starting as a community project and we're working into an Enterprise size project. To benchmark against some other projects out there. I just want to put this out so if you're interested, you can look into. 
1. VSCode which is the most popular project on GitHub. If anybody ever opened an issue of VS Code, you know if your issue is not top quality, it will be closed automatically and with and you won't be sad about it. Because it will tell you why it's closed and there's a policy and that's done. **The solution when you have too much is to have good policy**,  so feelings don't get hurt. 
2. we have a second one and maybe this is an issue that for our brainstorming here, is the **Swift Evolution project**. This is where **the idea for last call came from**. Swift evolution is made by Apple and a very innovative language. They have specifications and proposals to change it. I think it's a very good process, it gets a lot of active reviews. So whenever there's a new idea there's a lot of review that's why **we have RSS feeds for all of our ideas**. On how do you solve these problems when you've got a lot coming in and you don't want to hurt people's feelings. 

**Hudson**: That's some good comments. I would also say that I think we need to probably **reach out to Bitcoin, zcash and Ethereum classic** to see how their policies and their structures are different than ours. Since the EIP is initially coming from the Bitcoin Improvement proposals which initially came from the python environment proposals or PEP, I forgot what it stood for. but it has a history of itself and each group I think iterates differently on doing it with different ideas. So getting an understanding of what they're doing differently, I think would be very helpful. ZCash, I know that they do really well organizing there's.

**Brent**: Kind of red taping, what's in and what's out of scope. Something what really needs to happen is everything needs to be prioritized. what are the top 10 things on the list and we work on those and so if you can find the entire Community for example we could create a topic where you rank all the EIPs and everyone can say this is my top most important EIP, top 10 and so on and then you can find out the entire communities ease of the top 10 and then someone has an issue that's real old it's been hanging around, that in any new technology that makes that possible, than they can start recruiting and it can rise up and popular and you lower down. It's all about prioritizing thing and all large communities fail miserably at that kind of thing. The best they get is making rules saying that we've got whole bunch of sensors, trying to make people mad by saying we're shutting your project down but if you find out what everyone wants and do concise and quantitatively get. If you can know what everyone wants that by definition of consensus. If everyone can prioritize things and if you can measure consensus by what does the people holding their ether think,  what are the pure rank core developers, what do they all think, what do the miners think. If you can canonize things in different ways that allows you to prioritize all your work and problems like that become much easier solved.

**Will**: So what you say is you want to encourage, make it easier for this good ideas to finding encouragement they deserve? 

**Brent**: You measure the good ideas by finding how many people are supporting them. And also you have to have a way for people that don't want particular things to happen to also have a competing camp and you find out what both camps want and then you have negotiation to find out where the agreement is you focus on the agreement and you push the disagreement to lower-level supporting sub camps and it's all about finding out and getting everyone everything they want and not sensor anyone, any good at anytime. 

**Louis**: So if I may, I think I'm going to be a bit harsh on this one. I think it believe that people will get more involved into as they are today. What actually happens are there are few people who actually wants to push things and those are the one who actually wants to do things. I don't expect the community to you rise now in say I'm against this or I'm favor of this. The problem right now with the EIP is that we don't have the support and we don't have people coming and saying that I'm interested. 

We don't have people coming forward that are sufficiently interested to do the due diligence or do the work of sorting things out.

**James**: I would really agree with that. Louis if you can just introduce yourself so people can know.

**Louis**: I am Louis from Starkware. I got involved with the EIP process for the case of EIP 2028 which was a reduction of transaction cost in Istanbul.
From my experience, I am very late and do not come from the Ethereum Foundation and any such organization that is part of it for a while. There are two things that I found very challenging at first when I was trying to get involved. 
1. The GitHub, there's like many code that are very hard to understand from the outside and you need you to prove your point and provide it to the rest of the core dev. 
Also the things from my perspective and from what I saw in the Istanbul process, there is a list of EIPs that went through including that no one was pushing it. I got upset from the perspective of the future of the network because we end up with like proposal that get accepted but end up being barely used for many many reasons or the specification were not appropriate because there is only one out of group of people who worked on it.

**Pooja**: Louis to summarize the issue that you faced, I am assuming that people who are not coming directly from the Ethereum foundation or maybe development work on a regular basis to the challenges that they are facing at the initial level is how to proceed from proposing the proposal EIP from draft to accepted and how we can steer like taking help from the all core dev and the reviewer, is it what you're trying to communicate?

**Louis**: What I am trying to say here is the core dev should be the safe keeper and not political. Need to focus on only technical. What I'd like today is to know, what do I need, from a process perspective to show that I'm serious when I'm working.
I have an example that I open the EIP and may not be making it public on what's going on, we keep pushing it although it's not ready or good enough at this stage. If I am clear?

**James**: My experience has been along that as well is the **reducing frictions for the individuals that already want to participate** will solve a lot of these, what should bubble up to the top or not. I pretty strongly feel that we don't need to put what is or aren't considered from substantiation state or from ideological state or whatever because there isn't really many people willing to get in there in the first place and though they making the individuals who want to participate have less friction to beat to participate and then **give them clear guidance on what to do** when you want to, I think will kind of ease out a lot of these things on its own.


**Charles**: Another good example of someone that struggled with the process, who was actually trying to contribute was security consideration in EIP1. There is no defined process to make any of changes to the EIP process of getting dragged on for 9 months and I am not sure it is included yet formally. He kept voices of governance session and Nick Johnson just agreed that we need to define process for EIP1 process changes etc.

**Hudson**:   yeah I think security considerations were added to the EIP1 in the last 4 months.

**Bob**: Something which is a little unclear to me as well in general is **what kind of process you have for revising the EIP?** I saw recently that there was a proposal to do with a mechanism for Metadata or EIP another update? There is this discussion that we have on ETC as well, if you update EIP1, should there be an EIP for update? EIPs like this are kind of changeless. If you revise an existing one, it only processes one which will be really sensible. I don't know there have been update to others. I guess, you can do it for ERC 20. But just the genaral question is what's the model of EIPs and what are specs. Because if specs are a bunch of decks, that itself makes it very hard to understand what the overall protocol is. So, if you make changes to EIP1, should that itself be an EIP? Can we also use a canonical document to hold this together because yellow paper is designed only for the part of the spec but the broader spec itself makes it very hard to understand? if you make changes to EIP 1 because there isn't a canonical thing that would be building all these. So how does that work? 

**Hudson**: **How it currently works for EIP1** is EIP1 is consistently an active status and because it's an active status, it is able to be updated and then any significant changes are documented through the pull request. You can look through the pull request history of the EIP1, the changes to the file or you can look at the bottom of the EIP1 and there's a list of significant changes and the date they were performed on and that has been at how it's done since 2017 roughly. There hasn't been a major problem with that. As far as the problem of **updating ERC20 if there's a major security concern**, the general answer has been making a whole new EIP and you can call ERC20 version 2 if you want but it will have a different EIP number. Yeah basically just make a whole new EIP if you want a change in there that's not something that's like spelling grammar or gross overlooked like part of it you misspelled the word Ethereum, kind of like that.

**Will**: I agree that this discussion should be apart of the. I have updated a whole bunch of EIPs because of various reasons. **Normative changes require a new EIP**, non-normative changes I've been filling around and they are fairly getting merged. Also, the EIP 1 is not an EIP at all, the fact that we call EIP 1 to call Active is just a particularity this project. Other projects like Swift Evolution don't, they wouldn't call it standard. It's not a standard, it's a governance document. 

**Louis**: I think in the case of Bitcoin they didn't change a bit when they used the process.

**Hudson**: So do you mean that they did that just for BIP1?

**BoB**: They actually made a BIP2. Luke made a replacement.

**Hudson**:  That sounds like Luke. I think we won't be able to solve that one today, anyway. But basically the summary would be, **we need more understanding of how to update an EIP in general** regardless of this if its EIP1  in this case or if it's an EIP that needs small changes or the big changes, putting that on paper, I guess is the best way to describe the problems we have.

**Bob**: I mean something that I thought about a lot when we were starting the EEA was what does good look like? I really like the thought but you got something in the form of the yellow paper that's covering really the EVM but you haven't really got great canonical specs around everything else. My thought really was EIP are changeless, and they're looking like JAVA programming language book. As new changes are made, that book is updated. So I kind of like thinking that EIP are really the process, the change management but they don't necessarily the best final form of documentation. 

**Hudson**: Yeah so there needs to be a delineation. From what I'm hearing from you Bob is there used to be a delineation between if an **EIP is a specification versus if an EIP is a guideline**, or abstract. Like more of an idea or something that people can implement. I don't know if we wanted to find that or not that might be something we think about and just having our list of things that would be priorities are not. 
So, yeah anybody have the last couple of things?  Again Pooja post a link to a Google doc and that Google doc has a list of stuff already so we can address that or if you want to have more detailed any of those points as well.

**William**: I'm listening to the whole conversation over here one thing that I find myself sort of asking myself is maybe perhaps in terms of **defining the scope** of what we're trying to do here, are we looking at maybe to clarify an existing process or maybe to Define process or is this may be a question that even needs to address the possibility of creating a specific platform? as in it sounds like **there's a number of things along the way** so to speak of EIP process. 
* Whether it's the amount of stale EIPs, 
* the EIPs can even go stale, 
* whether it's the difficulty of understanding exactly how to get the support, 
* whether for low levels of participation and 
* lower friction along all of this different sort of point of pressure, are we looking at the possibility of creating an entirely new platform form for the EIP process in general or we just looking to augment the currently extant process?

**Louis**: I've a question, out of this group of people talking right now, I'm asking, how many of us have actually pushed an EIP through the process or try to push. I am asking not being snarky, I just want to know because I have very different experience. I think there are three of us.

**Hudson**: I can count six people. 

**Louis**: From my perspective, the EIP process is not broken, it actually could work. Issues I was  facing are, two things:
1. It's unclear from outside to whom we need to reach to get the validation, that what I am proposing will make sense? It's pretty hard to say that in the core dev chat and say, here is my thing. So what should I do?
2.  there is a lot of things in my feeling that were just not said out loud because of the fear to be perceived as against someone or against the project, and I just didn't speak out. That is more that I would try to fix by providing peer guidelines than trying to reform the process that somehow works.

**Will**: I have a quick note here, yes I think **this phone call is the EIP IP and not EIP replacement**.
I heard some descent on how much we want to encourage new people? one of the ways to solve this problem which I have committed in the KTE project, which is a Linux is **bring a mentor program**. Yes there's a lot of rules and honestly I got involved in 2018 and none of the things were specified in EIP 1, that were my experience. So, I've to go find out actually how it works that's why I'm here to document some of that stuff but with KDE it is much harder to get involved and what we did is we said, here is the group of people you can call that can just help you from idea to what you want to do. I will volunteer to do that, I know other people would too. We don't just write the stuff down and agree on it we can just put a couple of names of people that have done this stuff and want to help.

**Hudson**: yep that's a good simple solution.

**Louis**: I agree 100%.
**Hudson**: William Schwab that answer your question about if we're going to kind of redo a lot of the stuff?

**William**: yeah, I think so. I mean if I'm understanding you and also you William, it sounds like **the process seems to be at least a process that can work. There's a certain level or certain lack of communication about what needs to be done, a certain lack documentation maybe.** Does that address your second point though Louis? you were saying before that there's also sort of this bizarre process that certain EIPs seem to have some level of Brownian motion, they got sent to motion and they somehow get included.

**Louis**: They don't get included. They keep being referred to, although everyone in the sort of know that there is a big problem with it. My second comment was more like, the core dev claims to be non-political. Political not as having an ideology, political as having a public place where people  describe whether to lobby for it. And because it's you don't recognize this aspect of it then it's very hard from the outside, when you don't know the dynamics of it, to push efficiently to the process. it's more of the second point and maybe standardized a way. For instance, when EIP can be implemented at the client end, the people who should say about the spec should be the client. When EIP is not implemented by the client, then there could be multiple condition referred to by the client.  These could be standardized which I think is solution to the problem we're facing.  

**William**: So, you're saying that you think that also could be handled by better documentation and communication?

**Louis**: It would be pretty end up better we talked about the mentorship program proposed by Will. And also sort of an agreement on what are the best practice we should have?
I can talk what we did. In our case the EIP could have been very litigious, because it involved ideology in blockchain. What we did, we thought that by providing objective that everyone could check and when we finished, really seems like yesterday; we publish the first EIP and it's saying that what you said was correct, the methodology works. The reason we wanted to push it mostly because we believe it's the right and should be in place. Maybe when someone refer a new EIP, we need to define what people or core dev feel comfortable with.

**Hudson**: I think that something to take note of though, your EIP process that you went through is the core EIP and part of the challenge we're going to have is addressing the fact that there are **four types of EIPs - Core EIP, Networking EIP, ERC and Meta EIP**.  I think, I got those right. But anyways, each one of them seem to have very different process which doesn't mean we should break out the EIP repo into different other repos necessarily but that we should better define and like cement some of the processes behind getting those through, and the core devs meeting have already started doing that with things like eligible for inclusion EIPs and other rules like that that aren't written we need to write this down this year, pretty much. 
Then real quick Alex B (Axic), if you want to do a quick intro, we gave intros earlier so, just feel free to give a quick intro for yourself.

**Alex**: I just joined like 5 minutes ago. I was in another meeting and I need to leave shortly. I hope there's a recording or something so I can listen to recording and notes. Briefly about me, I've been involved with the EIP process for quite a bit and I guess been since probably 2016 and I be in volunteering to review stuff for quite a bit and as of the past couple of months, I've been doing reviews as an editor and I submitted a lot of different proposals to improve the process and a lot of those are still in pending state.

**Hudson**: Well thanks for joining the telegram and the call and I'll be pushing out the recording of this on the telegram and on Twitter and stuff after I get it uploaded.
Anyways that was a lot of good that sentiment, Louis and I agree with that I think it's going to be something that will need to work with the core developers as we overhaul a lot of the EIP wording and processes that will need to get them involved for their part of the Core  EIPs because that only touches like less than 200 people a year. The core EIPs track and maybe not even that many cuz there's not that many core developers and there's not like the average person writing a core EIP. it's like the same 30 people with the exception of people like Starkware who want to get involved in they had to go down that bumpy path to start doing an EIP other than  some people who want to do the low-level stuff, it's very rare that we get the average person going through that process. 

**Bob**: Just a quick thought, the list of editors that is effectively the same listed as being since 2016.

**Hudson**: That's an accurate, that list is accurate.

**Bob**: My thought was just that, for that different threads, you can **have different group of editors**. The core developers don't necessarily have to be gating or involved for standards to do with higher level things. If it's the case that many of the proposals are of very very high level, you will see standards built on the top of the core protocol. A completely  different set of people could come on board as editors calling it with an understanding of that  we're not going to focus on the core thing. I don't know about core things but I  know about small contract that happens and can help for those things.

**Hudson**: Yeah, I think that's an interesting idea. I think we need to **define the scope of what an EIP editor should be doing** beyond what the EIP1 says and like figuring out if we need to add or delete anything and then we should figure out if there needs to be subgroups of the EIP editors, like variant groups of the EIP editors, that's a good idea though.

**Bob**: Something that we want to see at ETC side, we have not done it yet but maybe would do it. It is kind of **having another role as** well as added to which is coming my **assistant or administrator** who are basically volunteers who're keeping things up to date, fixing broken links, enable helping things. I guess it's kind of role for a little bit like the Cat Herders to be honest. It is also acknowledging that there are a lot of stuff that doesn't need core protocol developer skillset.

**Hudson**: that's not a bad idea either. I think that's all really good. we have a few minutes left, I said, I thought it was going to be a short call.

**James**: I thought, getting a group of people that can do a lot of the things of the editors don't need to do a defining what editors do or don't do and also having a group of people that can do stuff that they don't need to do, is same is something that had seemed very valuable for me  and just getting that would allow more people to be active in the process. I have had a lot of thoughts about this for a long time about a year ago when I first started getting into EIPs. At some point, I got proposal to rewrite the entire thing of how everything works, some big brand vision and then since I realized, I would strongly support or suggest that we look at small incremental changes that been are made over time rather than zooming out and having this big overhaul. I am assuming that things would work like we think they will and instead make a small change to see how that works and then continue to iterate on those things. 

**Hudson**: I think that's really good and sorry we crushed your hopes and dreams of a giant overhaul last year.

**James**: I didn't propose, I was just my way of thinking about it was like oh yeah let's do all this stuff and then I realize wait this is actually like a moving system and we can just incrementally make it better.

**Will**: You think globally and you act locally.

**Hudson**: That's a good line, I 'm gonna steal that. It's just a few more minutes and so I don't anymore tangents to a couple of end announcements and then wrap up the call. The first end announcement, after discussion with the Ethereum Cat Herders this EIPIP initiative is going to fall under the Cat Herders and that the note-taking will be funded the videos will be hosted on the Ethereum Cat Herders YouTube page and they will help with other pieces of support as needed, such as advertising on Twitter and Reddit and stuff like that. so that's one thing. so if people ask like who's doing this you can say it's the Ethereum Cat Herders and then I am taking a lead role in facilitating it, technically but there's most of the people in this call can take over what I'm doing if I'm not able to make a meeting so it's really a group effort. Was there any other final like things anyone wants to say as far as like announcements or ideas or things like that?

**Will**: For the next call, will we approve these minutes? does this become an official? like is the outcome of this phone call we just had that now we have a scope?

**Hudson**: The biggest outcome of this phone call, I believe is that we have a list,  the note taking Pooja has been doing, the [document](https://docs.google.com/document/d/1KzEMD21Joqn7IWk4WnocwraRuo66y7r2w8R9Wml4BN0/edit) that she created has a list of problems that we found with the EIP process, between now and the next meeting what I want to do is **try to order those** maybe it might require a spoken meeting but hopefully it won't require that and we can just do whatever Telegram and a Google doc and just like **vote up and down on which issues** are the like the issues that people think are the worst issues that we need to address first. Does that makes sense or do you think there's a better way to do it?

**Will**: I think that's great unless it doesn't work, it means it is not great. And related you as a technical leader here, do we have authority the people in this call, to do the things that we want to do?

**Hudson**: Myself and Axic are the EIP editors. I know other EIP editors want to get involved and if we basically take our ideas from this meeting and put them in an EIP, it's kind of cheating because I am the EIP editor and I can absolutely at a fair and honest way push this along community Support.

**Will**: That's one of the fears of me ever wanting to be an editor is that I'm going to other side and I don't want to have superuser power, you got to compartmentalize that. 

**Hudson**: you got to do the best you can.

**Will**: Is our goal here is to come up with a proposal? What is the threshold here? Do we need the unanimous consensus of all EIP editors to change the EIP1? or is that the part of this discussion too. I want to know the steps to these ideas to PR to merged?

**Hudson**: It would be like 
1. ideas 
2. to ordering the ideas 
3. coming up with Solutions in different documents that we can apply slowly and 
4. then finding out the best way should this be a big PR that has like six different changes or should we do it little by little, once we decide that then we produce those PR's. I am leaning for it being a big one and we just kind of discussed within a GitHub issue and just say this has the backing of a lot of people that we do want 
5. to discuss this over the next month or however long and then get a lot more opinions, 
6. edit it a little bit more and 
7. then eventually once there is consensus and the last call issued, that it goes in; that's my dream ideal for it, although a little might not work that way.

**Will**: Got it!

**Hudson**: Cool! the next meeting, will two weeks from now work?

**Pooja**: Sounds good.

**Hudson**: Yeah, I can do 2 weeks from now.

**January 29th at 1500 UTC** and Bob has a final comment on the group chat.

**Bob**: In the doc, there is a proposal for a separate EIP call rather than not being bundled with the core devs call, I think it's a great idea. Because, I think the part of that 'political process', how do we push things through kind of things stems from that. They are deeply political and economically impactful. Whether things go in or not has really has real impacts to the network participants. I know a number of the core developers say that I don't want to be political and this is just a technical specification process. This could be true for the work of the core devs but is not true with whether these EIPs go through or not. I think dividing those two would be very useful also because the sets of work are different. The core developers are developing clients, the EIP editors are doing the technical specification process and then having these political decisions of what goes through or not. It's many of the same people doing those two roles and they are different. so I think it would be very useful.
 
**Louis**: I tend to disagree with this one because there is no one except the client developer that really know the protocol at the core. Separating one from the other is the recipe for technical disaster in my opinion.

**BoB** All I mean is the technical discussions on the EIP, of all things which the core devs would be involved with but the actual process of deciding what goes through or not is these EIP process and yes many of those are the same individuals, all filling both roles. And they obviously are not going to do something that core devs would not support to but ultimately these are two different things. These EIP process and dev process are different, that's what I am saying.

**Louis**: I agree there are two different things. But it's kind of delaying, it's very easy for the client to say, it is not my problem anymore and we end up in a situation where decision is not made. So, that's why I'm saying, separating the two, theoretically seems like a reasonable thing but could end up where decision don't end up making much sense. 

**James**: I would agree also with Louis. We get a lot from having the all core devs call, having decisions being made on the all core devs call and then being reflected through the EIP editors or through EIP administrators process. I think it was some really good separation and allows a lot of things to work.

**Bob**: I think what might work best as, the Cat Herders didn't use to exist and they do now and there is value in that, Magicians didn't exist and they do and they obviously value that. I see EIP call in the same kind of context. It's like a wrap around the core devs saying how can we help to move the thing forward. Some decisions will obviously go back to the all core devs to make the call but you don't want to burden them up with all the details, but have to sync some times. 

**Louis**: The place where I would object is that you don't see the Geth developer is coming to Twitter and debate you don't see Nethermind coming to Twitter and debate, you don't see those guys. If you think it's a political road, then I think it's a political road in my opinion. You just shed the responsibility off the shoulder, people will be happy but the internal security of the network, in my opinion will be a disaster. 

**Hudson**: We're after time. So let's definitely pick it up the next time and we can bring this up again. Feel free to write down and send me the gist of what was being discussed. I can definitely bring it up again next time. So thanks everyone for coming and we will talk to you on telegram.
Thank you very much!

**Date for Next Meeting**: Wednesday, January 29th at 1500 UTC.
	
# Attendees

* Anett Rolikova
* Alex Beregszaszi (axic)
* Bob Summerwill
* Brent Allsop
* Bruno Skvorc
* Charles St. Louis
* Hudson Jameson
* James Hancock
* Louis Guthmann
* Pooja Ranjan
* William Entriken
* William Schwab
* Wei Tang

## Links discussed in call:

* EIP improvement process [document](https://docs.google.com/document/d/1KzEMD21Joqn7IWk4WnocwraRuo66y7r2w8R9Wml4BN0/edit)
* [EIP 1 ](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-1.md)
