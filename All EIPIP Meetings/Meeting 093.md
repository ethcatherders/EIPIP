# EIPIP Meeting 93 Notes
### Meeting Date/Time: Nov 01, 2023 at 14:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/285)
### [Audio/Video of the meeting](https://youtu.be/ib9xInX3nkk)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
93.1 | **Topic Group - Should new topic groups be independent of EIP/ERC or peer within the same structure?**: Sam mentioned It hasn't been set in stone, The way it has been envisioned, they will be peers. ERC | Core-EIPs could become topic / working group.
93.2 | **Topic Group - Start-up: what is needed? an XIP-1 document? Initial editors/stewards?**: Most of the documentation is written.Sam will introduce it.
93.3 | **Topic Group - RIP numbering? even/odd won't work. Start from a different number?**: The current process uses a spreadsheet for numbering. It will be replaced with automated number allocation.
93.4 | **Topic Group - "Boundaries" - how do we determine what group a proposal goes to initially? Is that "portfolio/jurisdiction" baked into the XIP-1 document?**: Each topic group has sections that describe the area the topic group is interested in reviewing. New proposals will go into the most matching specific topic group.
93.5 | **Topic Group - How do we deal with specs that feel like they belong to multiple groups? Have one group have initial jurisdiction? Multiple specs? Joint specs?**: Will be determined case by case. The general advice is to go with the closest category.  @SamWilsn will be publishing the document as soon as possible. [Early version here.](https://hackmd.io/@SamWilsn/BJTdMfA0n)
93.6 | **EIP-ERC repo split**: Token received and will be shared with PandaPip to run eth-bot on ERC repo. Working on updating ERC references at multiple places
93.7 | **Web Page Rendering for EIP & ERC**: Lightclient is in favor of two separate websites.
93.8 | **Web Page Rendering for EIP & ERC**: Pandapip1 who is working on the website could not be heard on the call due to a technical issue.
93.10 | **Web Page Rendering for EIP & ERC**: Consensus on Markdown rule - ERC-x and EIP-x for EIPs website (or separate websites, if agreed)
93.11 | **Web Page Rendering for EIP & ERC**: Change in the preamble of ERCs or both (EIPs & ERCs to keep it number only)
93.12 | **Web Page Rendering for EIP & ERC - Decision**: Keep ercs.ethereum.org & eips.ethereum.org working as today
93.13 | **Web Page Rendering for EIP & ERC - Decision**: will fix the markdown rules for authors & Rename EIPs or ERCs in the preamble to just the number.
93.14 | **ERC-1**: SamWilsn and most of the people on the call think that having a separate ERC Meta document does make sense rather than updating EIP-1 with ERC-related processes
93.15 | **ERC-1**: Poojaranjan proposed to have another special number instead of ERC-1 as ERC/EIP numbering is unified and we can avoid duplicate number.
93.16 | **ERC-1 - Next step**: Document ERC process, make a pull request and it will follow the normal numbering process but the proposal can be redirected from ERC-1 to that number.
93.17 | **EIP-7539: ERC Extensions discussion**: SamWilsn thinks it's better to discuss this after the Working group charter is proposed.
93.18 | **EIP-7539: ethereum/ERCs#8**: We couldn't discuss it as we ran out of time.
93.19 | **#284**: SamWilsn responded, the issue could be closed
93.20 | **#Call for Input**: SamWilsn walked us through the open issues & Editors are requested to respond to them as soon as possible
93.21 | **#Fix a Security related change to a Final EIP**: SamWilsn will create a Call For Input.

## Intro
**Pooja Ranjan**
* Welcome to EIPIP meeting 93. This is issue number 285. On agenda we have a lot to discuss today. So starting with the EIP-ERC repo split we will get some updates from editors meeting that happened last week. There are pending task list which is added as an issue in the new repository.
* Will take a look at that. There are a few suggestions for ERC governance and other area of improvement. We will learn where we are on rendering of EIPs and ERCs Looks like there were a few editors who could not join the last meeting, and we may would like to revisit where we are. On that additional topic for discussion, here is the topic of groups.
* Those can be created after the split to help this move smoothly. There are a list of questions suggested by Dano will take a look into that. We have listed call for inputs and then we will have some discussions from the past meeting. We also have added a monthly update the  EIP editing, office hours and some announcement to go.

## EIP-ERC repo split [1:39](https://youtu.be/ib9xInX3nkk?t=99)
**Pooja Ranjan**
* So starting with the first item which is EIP ERC repo split. I do not see Sam or Panda on the call. I wonder if anyone else has any update from the last editors meeting that happened, and that led to the split here. 

**Sam**
* Matt said he'd be a little late, but the really short version of it is the split happened and ERCs are on their own thing. It's a bit rough around the edges, but they do get merged onto EIP.ethereum.org. But yeah, I'll let Matt go into more detail on it when he gets here. 

**Pooja Ranjan**
* Sounds good. So kind of next. But related is like the list of pending tasks for EFC migration, which Lightclient has already created. Do we want to talk about this now, or do we want to straightaway jump into the topic group discussion and we'll come back when Matt is around? 

**Sam**
* Yeah, I can definitely talk about topic groups for a few minutes. 

## Topic Group [2:27](https://youtu.be/ib9xInX3nkk?t=147)
**Pooja Ranjan**
* That makes sense. So we'll skip this section. Please go ahead with topic Group. 

**Sam**
* Sure. So I just haven't had a chance to make any progress on it yet. The ERC EIP split has taken up a bit of time. Going through Dano's questions here. Should new topic groups be independent of EIP, ERC or peer within the same structure? The way I've kind of envisioned it, and this isn't like set in stone or anything, but they'd be like a peer.
* So ERCs would become a topic group. Core EIP would become topic groups. Or working groups, I guess, is the name we're going with right now. What's needed? So we have most of the documentation written. I just have to actually put it up and introduce it. So ROP numbering, even it won't work.
* Start from a different number. So we have a spreadsheet that we use for numbering. And we're going to use that for now. And then eventually we'll move to something automated. Our boundaries. How do we determine what group a proposal goes to initially? Is that portfolio jurisdiction baked into the zip1 document.
* And yeah. So each each topic group has a section that describes what areas that they're interested in reviewing. And EIPs or new proposals go into the most specific matching topic group. Bnd how do we feel with sorry? How do we deal with specs that feel like they belong in multiple groups? Does one group have initial jurisdiction, multiple specs, joint specs? And I think that's going to be determined mostly on a case by case basis.
* How we do today with ERCs and interface and stuff like that. The general advice is probably going to be to split things or to just pick one and go with it. I mean, we're all people. We can we can work out conflicts. 
* That's about it. And really, we're just waiting on me to publish some documents and get approval on them. So, yeah, I'll be getting to that as soon as I can. And that's about it for the topic group. Update. 

**Pooja Ranjan**
* Well, thank you so much, Sam, for covering this. I wonder if anyone has any immediate question that Sam may answer on this particular topic. 

**Joey Santoro**
* Yeah, just a quick one. What is XIP and RIP designate. 

**Sam**
* I think oh go ahead. 

**Danno Ferrin**
* XIP used as a generic what is your name that you're going to be. So it'd be and let's say there's a wallet. So just used to say whatever the letter is. So XIP means their founding document of whatever their initials are. 

**Joey Santoro**
* Got it and RIP for roll ups. 

**Danno Ferrin**
* That's what's been floated. 

**Joey Santoro**
* Okay. Cool. Yeah. 

**Pooja Ranjan**
* All right. Any other question. 

**Danno Ferrin**
* Mostly. I'm happy to hear that there's work going on behind the scenes. I just haven't seen any of it, and I knew it was kind of a big deal. And the RIP call last week. So I just want to make sure that the the wheels are greased and things will happen. Well. 

**Pooja Ranjan**
* No I think you are right on time. 

**Sam**
* So I posted a link in the chat to my current draft of what? Like the working group that defines the governance EIPs. This is what I think their charter will be. It's a very early draft, but feel free to take a look. 

## EIP-ERC repo split [7:16](https://youtu.be/ib9xInX3nkk?t=436)
**Pooja Ranjan**
* All right. So see now we are joined by Matt Light client. So if we do not have any further questions on topic group, we can perhaps go back to EIP ERC repo split discussion. So Matthew did not miss much. We just have covered the topic groups and tried to get answers to some of the questions shared by Daniel here. I'll be trying to summarize it in the agenda as a comment at the end of the call.
* So going back to EIP ERC split, I was wondering if we have updates to be shared from the last editors meeting already. Sam has shared a shorter version of it that the repo has been split. I wonder if you would like to, walk us through the pending task or for ERC migration or anything else specific coming from that meeting would like to share with the group. 

**Lightclient**
* You have something to share, Sam? 

**Sam**
* Oh, no. Not really. I did it earlier. 

**Lightclient**
* Let's look at the pending tasks. There's a lot of them. Okay, so I got the token from Jamie last night. I will send that to Panda after this call. And that should get us the EIP bot on the ERC. I know that he's got the EIP, some EIPs review bot running. I don't know if that's actually a merging things. Let's see. Yeah. I'm not sure if it's merging things. We'll have to figure that out. But yeah, we're still trying to get the EIP bot running.
* That's pretty critical because every PR just stacks up and needs somebody to merge it in the meantime. And then like more generally, we have a problem where there's still this EIP reference in a lot of places on the ERC repo, and I'm trying to replace it with ERC. So for example, in the preamble EIPs colon, the ERC number. And I want to change that to ERC. But there's a lot of problems. And also importantly in the in the relative links. But the problem is, is that because we're building the website on the website.
* We sort of need this these values to be EIPs. So the Jekyll builds correctly. We could. Translate those values on the fly in the repo, but I really don't want to add a bunch of additional logic that is processing ERCs outside the ERCs repo. It's brittle. It's not really clean. It can break and we won't really notice. So I would like to find a resolution for that. And I propose resolution is what I thought we agreed upon a couple meetings ago, which was to just split the EIPs website and the ERC's website.
* And that's why I got ERC's ethereum.org set up. I don't know, it might even be available right now. 
* ERCs's ethereum.org. Yeah I mean ERC.ethereum.org is live. It has been really publicized, but it's available and. I think that just makes things much simpler to deal with. The all of the issues that we're talking about, because we can just update everything to be EIPs for the ERC repo is for the ERC repo, and then have a link at the top in the top bar to go to EIPs or to go to ERC, and it also allows for some different things to surface on the different groups.
* So I think like as we go forward, some things will change a bit between EIPs and ERCs and we will want to expose that for ERCs. And I want the ERC editors and folks involved with that to be able to modify their website. Like, I think Panda's website looks nice. I don't want it for core EIPs. I want core EIPs to be like very light to download, but if they want to ship that website for ERC, like they should be able to do that. And so that was the intention and I would like to move forward with that.
* But I know that you guys talked about it last week, and some people were more in favor of having another repository to hold the website. 

**Sam**
* Yeah, it really depends how we end up going with the working groups. If we do one website per working group, I think it'll get a little messy. So. Yeah. 

**Sam**
* Because you'll end up with, like, I don't know, wallets.ethereum.org. And then you'll have like rip.ethereum.org, and you'll just have a bunch of these separate websites. And there might, there might be a lot of them. So I'm not sure if that's the approach we want to have. 

**Lightclient**
* I mean, look what other ones are going to be, because I don't see a lot of them coming out of the woodworks. 

**Sam**
* Yeah, it's pretty much just wallets. Layer two and core and ERCs. 

**Lightclient**
* The problem is, is that they're just not EIPs or we haven't really come up with a definition of those two things that makes sense to people. And so it's just confusing to eip.ethereum.org have ERCs. But tell everyone, oh no, these aren't EIPs, these are ERC. And same with reps, same with wallet stuff. 

**Sam**
* We created the distinction between ERCs and EIP, so I think we're partly to blame for that. 

**Lightclient**
* I mean, I don't think that we were the ones who did that. That sort of just happened by the community. Like we had this ERC category and they decided to refer to things as ERC 20, ERC 721. And so that distinction evolved naturally, and we at times have tried to push them closer together. But at this point, like, I don't really understand the relation. Like I know that you're describing these things as like they're still an EIPs, but to me that doesn't like that doesn't mean anything.
* Like I can see on a high level that it's an Ethereum improvement proposal that's like ERC focused, application focused, but this is like extreme nuance that someone really involved with this process doesn't quite understand. And there's no way we can ask the community to deal with that type of nuance. So I would rather just lean towards having a much clearer boundary between the two things. 

**Sam**
* Sure. Okay, I'll try to consider that a bit more when I'm working on the working group stuff. 

**E**
* Hi, everyone. I'm Anamika. I go by on ETh magician's website. I'm just about, like, something around ERC, like naming convention around. So for a while now. And I know this is, like, ERC are sticky in the sense that a lot of people like, use it, a lot of but I don't see the need for it to change. That's like a practical, you know, person usage level. But I was wondering if we could, you know, we can have EIPs. And I thought in my mind as EIPs or like Ethereum app standards, whereby, you know, the overall umbrella is an EAS and an EAS is you have ERCs.
* So, you know, words can just be like an Ethereum improvement proposal.
* So can even fall under like Ethereum core standards, if you will. But then fundamentally for ERCs, you kind of give them the overall umbrella term if they're Ethereum app standards, and then ERCs can just be like the code words or the code names for Ethereum app standards. So it's a thought I had a while ago. I never mentioned on the magicians for But simply because I feel like ERC is still very sticky.
* But then if there is like an interest or a need or want to like be a bit more defined between the two, that I think we could start with Ethereum app standards, and then ERC has just become like the code names in every app standard. So when someone's like, oh, what's an ERC? We're like, oh yeah, it's an Ethereum app standard. That's what it is. that kind of thing. So just some thoughts I wanted to put out. 

**Sam**
* So you're suggesting, like a new name for ERC category. 

**E**
* A new umbrella? Exactly. A new umbrella name or a new overall term for the category. Like we can still call them ERCs when we're kind of talking about them, because those are like the code names. But then overall was the name we could know them as if they're on app standards. So gradually. Eventually you're going to have to be able to talk about ease and then, you know, oh, what's an ease? It's like it's just standard. It's like like you're actually 20, like 20, 21,. But that way we can kind of have a path to delineating between an EIP and an ERC. You know, in a more social way. 

**Joey Santoro**
* Spiritually. I like the idea of reorganizing the naming conventions to make things clearer. I want to be really careful of, like introducing even more cognitive overload. Kind of like what Matt was saying earlier, where we have more acronyms that people need to get straight of their relationships. So I think whatever we come out with at the end should be as sort of simple as possible, even on the naming level. 

**Lightclient**
* Yeah, I think this is originally what I hoped would happen with this split, and I was kind of overruled a bit because originally I hoped that we would completely separate EIPs from application standards and let application standards be their own thing, govern themselves. And now we're kind of in a different world where the expectation is that they'll still always be a part of this working group. Ethereum improvement proposal world. And. We're still figuring out exactly how that's going to work out.
* But I think as long as we are unwilling to let ERCs sever their ties completely with this governance group, then yeah, I don't think that we can adopt another umbrella name around the ERCs. 

**Joey Santoro**
* I think we can still have them sever ties completely, at least from like. I like the whole referring to things exclusively as ERcs versus EIPs, and that they're now conceptually separate things in my mind is the direction that we're heading with the repo split, and I feel like that's good enough. And then, yeah, that's I think we should have, like, new. Let me just for the thought, like, I don't like the idea of having things called RIP and EIPS, and I think that's going to be really confusing.
* I think it should be like a wallet ERC, and, Roll up ERC in a DeFi ERC. And like, those are just ERCs. And that's the name for the ease that I was talking about. Bhat would be my preference. 

**Sam**
* So I don't have any strong preference about what they're called. I really don't give a shit what the abbreviation is. I'd prefer if they were all EIPs, I guess, but like. At the end of the day, we're not governance really. We just hold documents for people. So I don't I don't see why we need to completely sever the governance stuff. But this is opening an older discussion. So I don't really think we need to go down that road again until we have a concrete proposal on the table which is waiting on me. So I'm sorry about that. 

**Lightclient**
* Yeah, I agree with that. Let's not reopen the discussion. I think it's something to discuss in the future, but for now, let's just focus on I mean, we've got a lot of fires to put out with respect to just making the split, you know, work out correctly. So I don't know where that leaves us with respect to the websites. I feel like it's much more straightforward to have separate websites, and we can think about this problem more as we go forward. And if later in the future we're dealing with 3 or 4 websites and we're like, damn, it would be easier if these things were all put together, then maybe we can do it.
* But I don't like the idea that we're early optimizing for something that doesn't exist yet. 

**Pooja Ranjan**
* E see your hands are raised. Do you have anything else to add? Or is it from the last time

**E**
* Yeah, just just a few last thoughts on this particular topic. Best around like how we can even socially navigate EIPs. Bo I had after the, after the split happened, I had this thought where I said, okay, I the other day, we're going to be doing an and, but even at the paper level, we're still going to be looking at an for an ERCs. Bo what about you know, the key thing is if we're able to indicate to people what things are and particularly I thought, oh, why don't we consider like so for example, you know, how in the optimism Collective they have like two houses, that kind of thing.
* I was wondering in, you know, at least from the magician's perspective, starting from magicians and maybe we can proliferate from there.
* We can have two camps where it's like, okay, we have camps the name? Camp core and camp application or camp EIP and Camp ERCn that way, in the documents, even people are able to see that, oh, this is a core. This is an application that whether they see some kind of even if they still see EIP like the paper somewhere, they look at a class or the camp and they see, oh, this is a core EIP or this is an application or like would want to see an application. I shared a post in the chats to kind of give more light to that.
* But then also I think on the agenda for today, there's like a topic on the preamble. So I think we'll ERCs back on to just sort of this delineation.

**Pooja Ranjan**
* Thank you. Thank you everyone for sharing all thoughts here like from this discussion. I think I'm getting that we are still not clear on website side. I checked with Panda. He mentioned that he would be joining later today. Maybe in in a few more minutes he would be joining. So if he has changed perspective or I'm assuming that because he is the one working more on the website side, and if he's recommending at this point that we can continue with one website, we'll try to listen his thought as well and see if it is very difficult or relatively easier to maybe having separate website in future.
* So just for people documenting notes, we do not have any concrete decision as of yet.
* We are hoping to have one website to go ahead with and look into other questions that we need to answer today. One other thing that I wanted to mention from this conversation here. I really like the idea of division of ERCs, like ERC wallet and ERC RIP or whatever else. I'm saying this because, you know, we have one structure as of now that is documented in EIP one, which is all about the standard track EIP. We can perhaps have, whatever. Like we want to have multiple ERC categories. We can have some certain standard track, not standard track ERC but divided into different categories.
* That is a separate discussion that Sam mentioned. That would be clarified after the working group or the topic groups are created. We can revisit that question, but as we have on the agenda today, there is a proposal of having a separate ERC 1. I'm a little shaken by this because as of now, we are still having a unified numbering number allocation system. We are maintaining it with a with a Google sheet in which we are trying to make sure that one number that has been allocated to an EIP should not be allocated to an ERC.
* So I'm wondering like what people think about having this separate ERC one, or is there anything that we can do to add information in the present EIP one and let EIP one be the standard document for reference for any category or type of EIP? 

**Sam**
* I think we just need to give up ERC 1 you know, one being special and just pick whatever we want and put the rules for ERCs in there, and it'll just be some random number. 

**Joey Santoro**
* I disagree. I think we should either do EIP one /  ERC one as separate things, or put all of the content EIP one for describing the ERC split and how ERCs are going to be managed in the future. But I think that like how ERCs are governed is as important to ERCs as EIP one is to core EIPS, and we should keep an elevated status and not give it some random arbitrary number, because I think that the category is that important or the document is that important. But that's my take. 

**Sam**
* We encourage for authors, or the philosophy we try to promote for authors is that numbers don't matter. And I think we need to adopt that philosophy ourselves, just like there's nothing special about it being ERC 1, except for the fact that it's the first one in the repository. 

**Joey Santoro**
* But it's the living document that describes the whole process. I feel like if anything's going to be special, it's that. 

**E**
* Yeah, that's like the number one thing that guides every contributor, developer and even third party observer who's, like, looking to wonder how to navigate this particular side of Ethereum development. I feel like that is very critical. So yeah, I'm with the other gentlemen. That is a valuable area to focus on and to get right. Most importantly, lest you know, new comers and even existing folks have like major issues just trying to find their bearings with. 

**Pooja Ranjan**
* Do we see any downside in updating EIP one? I'm suggesting this because when we initially started with this ERC EIP repo split, there were a lot of proposals and we tried to have that accommodated in the existing meta EIPs that we have. For example, the charter concept that was updated to EIP-5069, if I remember the number correctly and part of it was going into EIP-1. What are the downsides of documenting ERC related changes? Because we do have a meta that describes that EIP repo has been split. And yeah, people can find details over there. 

**Sam**
* Well, if we put all of the, like, formatting rules and everything into EIP one, It'll get really, really messy if the process is diverge. So I think it's valuable to have separate documents describing each group, whatever we want to call them. 

**E**
* Yeah. Agree with with Sam. This let me see if I can share this page, but you probably have the link to already with regards to even like the changes for that.  

**Pooja Ranjan**
* If you have something to share, screen and talk about it, you can perhaps do that. 

**E**
* Oh, okay. I'll wait first. Are we strictly discussing the ERC one document now? I can probably switch to my laptop and, Well, then just give me a second switch to my laptop. Sorry. 

**Pooja Ranjan**
* Okay, perfect. No problem. So I was just wondering, like, if ERC specifications or the documentation process needs to be documented separately, do we really need to have the same number like as ERC ? I know we are somewhere around 7500 plus. Can we give a bigger number? Allocate a number which is different from one? Like any standard number, let's say ERC 10,000 or 8000, 9000, whatever, it works out. But what I'm trying to advocate here is let's not have duplicate number for one for ERC, and till we have a number allocation process split as well. 

**Joey Santoro**
* I don't think that's an important hill to die on. I think that it's so much more important that everyone knows immediately where to go. Look for the process for how to govern an ERC or EIP, and having number one be kind of a special number that is allowed to be duplicate only to describe the process itself, is a willing and useful exception for the entire community of authors and editors etc. I feel pretty strongly about that. But, you know, obviously that's just my take again. 

**Pooja Ranjan**
* Wonder what editors think about this number allocation. And then definitely we can dive into the details of it. 

**Lightclient**
* Can you repeat it? Sorry. 

**Pooja Ranjan**
* So I'm wondering, like what editors think about the documentation or go to document for ERC. Do we want to keep it ERC1. Or can we come up with any other number which hasn't been allocated but kind of special in a way. 

**Lightclient**
* I really don't have that much preference, to be honest. So if Sam has a preference, we can go with it. 

**Sam**
* My preferences. We just write a document for ERC and follow the normal rules for assigning numbers. 

**Lightclient**
* That is the EFC way it seems. If you look at newer ways of doing things in RFCs, they just write an RFC. That's the number and it says, this is how we do this. So I think it's okay. I do understand. 

**Sam**
* Having a redirect from  ERC one to that number, but yeah, I'd rather not. 

**Lightclient**
* It's not a bad idea. 

**Joey Santoro**
* Yeah. If it's like an alias, that's good enough. Like, to me, as long as people can find it really easily. The actual number to everyone's point isn't the important part. It's that everyone's mental model of where to find this thing and what it means is elevated or special in some way, but that can be an alias or a redirect. That's totally fine by me. 

**Sam**
* Okay, yeah, I'm fine with that. So I guess the decision is we put it at the assign, like the number from the spreadsheet, and then we redirect from one to that number. 

**E**
* Sounds perfect. Sounds good. 

**Pooja Ranjan**
* All right. Wondering. He is ready to share the dock. 

**E**
* Yeah. Bo for those wondering, I've put the dock in the chat, but I'm going to share my screen right now. So I believe you guys have a access to my screen now. 

**Pooja Ranjan**
* Yes we do. 

**E**
* Okay, perfect. So this started off as a as a PR from Joakim. I'm not sure if he's on a call right now. Joakim. LeBron. But then I saw then I started to kind of add in like polish it up a bit, flesh out a bit into into this. So pretty much like what's an ERC? It defines the whole process. But the key thing that catches,  the what they call the potatoes and meat or chicken, I think they call it is what belongs in a, in ERC structure and particularly in its preamble.
* So in the preamble, I decided to kind of build out a taxonomy. So naturally you have an like the field sort instead of the field saying it would say ERC, EIP. And then you have the number two it title. And as you go down what you will see are two new fields or two new fields and one existing one. I think fields that people are familiar with usually type and category. Now with, what's the name? With EIP, normally you see the usual standards, method and information, but the categories you see network, ERC, consensus for ERCs. So to take a different turn on that, a more dedicated turn into the app ecosystem or app standards ecosystem.
* So your your types remain the same. Standards track meta informational but your categories improve. So categories such as token wallets, wallet  metadata standards, Joaquim include package formats for libraries and interface formats as well for smart contracts and APIs. Stuff and registry for I think struct like stuff such as like ENS I don't know, like stuff and everything. Baturally this is all these particular categories are in the realm of like discussion and kind of further improvements. 
* But then the category is supposed to give a given contributor, developer or observer or researcher a top level, view of where they are going to explore. So if you talk about ERC tokens, you definitely want to be looking at token category. Yours pertain to wallets. You definitely want to look in the wallet category. And then from there you can further add in more precision based on sub categories. So this can be NFT feet like so fungible semi fungible. So bound tokens was hardware wallet software wallet user ops.
* Those who are familiar with like the intent based systems, account abstraction and so on and so forth. Also in the realm of  improvements, by the way, sub categories are optional, but the key thing is that the better you can introduce a sub category to your to your ERC proposal document, your proposal documents. The clearer it is for people to understand what exactly you're touching on what exactly you are looking to improve. So those are three key parts. I ended up building a bit of a taxonomy. So an ERC into a type which has standards track meta information.
* Also one thing to note, in terms of the categories for meta ERCs, it is optional for standards and informational. It is, you know, required that you kind of state a category and subcategory. But for meta ERCs it's optional, such as the first ERC itself that doesn't have a category. But yeah, moving down into like the visual aid itself. So you'd be able to know that, okay, every ERC should have a type standards, meta information, and every type should have its categories and every category should have a sub. So naturally every every type can have sub same categories as the other type. 
* So yeah standards track meta informational. I have added more information in terms of like how do you define these categories. And then you have like interface, you have wallets and a subcategories and so on. So the  key idea is that besides that nothing else really changes. Like the the process flow in terms of statuses are the same. Bnd I noticed, Joakim used like the old, Bow do you call it? Like the link into external repos. And. Yeah, he used, like, the client specifications. I felt like a lot of these parts we could get rid of or we could kind of improve on.
* But I didn't touch them because I was like, okay, you know, they might be valuable, but that's up to the room to really decide if, like, okay, we should be, Booking at these as like consensus specifications and everything. I thought we could get rid of it. But the, the crux of everything is pretty much like the new taxonomy, which is geared towards application standards. So, Bou know, if tomorrow. B. The sites or, you know, while it decides to add in. 

**Lightclient**
* Hello. I think someone came off mute. Go ahead. Okay. 

**E**
* Yeah. So if someone tries to come in and build like a wallet, they have every opportunity to decide, oh, do we want to handle ERC tokens differently or do we want to handle I don't know, account abstraction matters differently. They can always find that, B have to I actually have to improve this this supposed to say subcategory.
*  I apologize for that. But this way they're able to have like, this precision to it. And that way, Everyone knows what is what to the, you know, closer to the, to the needle itself. B think this is like one of the valuable aspects of the entire ERC. Bas the name guideline document. And  I yeah, I'm going to put a cap on that. I'm open to any questions or thoughts or suggestions around that. 

**Sam**
* This to pandas tagging proposal. So every EIP could be tagged with with one or more tags, the links in the chat. And then you could build a taxonomy out of those. 

**E**
* Links in the chat. Hang on. So this the one Sam posted? 

**Sam**
* Yes, that's the one I posted. 

**E**
* Okay. I love tags so users can filter by topic. Yes. No. So I think this is. So how do I call it if? ERC-1 is the blueprint. The tags are kind of like how you can even implement them. I think the tags would even work phenomenally for subcategories, especially because in the document I make it clear that wait, hang on, where are you? Yeah, in the documents I make it clear that we would like for proposers. So let me suggest, uh. Other values can be suggested in proposal and reviewed by ERC, so they can be suggested in the proposal.
* So I guess the tags are like a great way to kind of propose them. And then the ERC editors can then look at them and say, oh, it looks like you're trying to talk about this, or yeah, this looks like a good enough tag to kind of have its own subcategory, that kind of thing. That way, those who come in are also able to kind of see what's already being used and also kind of suggest newer ones.
* So I think the tagging system is kind of like a how you apply onto the blueprint that is this particular document. All right. So yeah, they work hand in hand I think. 

**Sam**
* Yeah. So I'll take a good look at this. This is in a pull request on the ERC repository. Right. 

**E**
* I like to think so because I did a PR on. Yeah. Is is. Yeah. 

**Sam**
* Okay. 

**E**
* So in. 

**Sam**
* Great. Awesome. 

**Gavin John**
* I'm wondering if it makes sense for. Every ERC to get its own tag automatically. Like, if like if you. 

**Sam**
* Wouldn't that just be the requires header? 

**Joey Santoro**
* Yeah, that would be the required header, I think. 

**Sam**
* We last panda. All right. 

**E**
* I should improve. That requires her to. I definitely miss that. Let me. I'll improve that. Apologize for that. That way it's a bit more clear. Like just from the document itself. 

**Sam**
* All right. So I know we have a lot of other topics today. So I want to make sure that we get through them all. Who was up next? Was this the EIP 5000? Um. 

**Lightclient**
* What was the outcome for this? Sorry. 

**Sam**
* Oh, it's I'm going to read the pull request and then we can talk about it. Yeah. 

**Gavin John**
* Yeah. 

**Lightclient**
* Thanks for presenting this. This was a lot of really nice content. Yeah. Appreciate it. 

# EIP-5000: Renumber to EIP-5159 (PR #5270) – Call for Transparency and Clean Rules #284 [39:31](https://youtu.be/ib9xInX3nkk?t=2371)
**Pooja Ranjan**
* Right. All right. Yeah. So next thing was like okay, we had this number 5000. And then we'll get back, On the web page rendering if there is anything else to be added here. So yeah, the pull request number here is. Oh sorry. It's an issue number 284. 

**Sam**
* Yeah. So this is a profit ZX. They're kind of a very adversarial participant in the EIP's process. And they are or were asking for transparency on the renumbering of I think everybody remembers that pull request. And I posted a summary. If nobody objects, I'm going to close the issue. 

**Pooja Ranjan**
* Perfect. That was the idea of adding it over here. I think the response that you have added here kind of satisfies the question, but it would be really nice to see if anyone else would like to add anything to that issue. Yes. Number 284. All right. There is one other thing. Before we move on quickly. Want to hear your take, Panda? As of now, we heard that you are in favor of having one website eip.etherum.org, for rendering all the EIPs.
* Do you by any chance have any other thoughts or change your mind and and want to go ahead with separate repository, separate websites at this point of time? I'm not sure I can hear you.

# Call for Input [41:17](https://youtu.be/ib9xInX3nkk?t=2477)
**Pooja Ranjan**
* We'll get back. Moving ahead. We have multiple call for inputs. Have added all those issues here. The issue is still open till November 19th, 14 and 16, but editors are requested to maybe take a look. These are the last day where we can, like, you know, close the issue with whatever responses we have collected. But it would be really nice to get responses beforehand. Anything. Sam, if you would like to add on these, call for inputs. 

**Sam**
* Oh sure, I can run through them. 

**Joey Santoro**
* So yeah, before we get onto too many new topics, I just wanted to call out, I think that we skipped the discussion for ERC 7539, which was related to the EIP ERC split and ERC 1. I don't think it'll be a super long discussion if we can talk about that now. Or I can wait if other things are higher priority. 

**Pooja Ranjan**
* He okay, fine. If it would not take long. Let's go ahead and quickly wrap that up. That will actually conclude all the items listed there for discussion. 

# EIP-7539: ERC Extensions discussion @Joeysantoro [42:22](https://youtu.be/ib9xInX3nkk?t=2542)
**Joey Santoro**
* Yeah. So the quick Tldr is 7539 is primarily useful for defining an extension, which basically extends the functionality of a pre-existing ERC in sort of a more strict sense, with some definitions of what that means. I made it simpler from Sam's comment and from discussions with the rest of the editors. I think that we can even make it even simpler and include it in ERC one.
* So most of those discussions can happen relatively asynchronously, but I think it's really important. The most important aspect of it is really a subset of the requires header, which would be an extends header or extensions depending on which direction we go from. And that would allow for very explicit forward and back linking between arcs which extend each other like ERC 4626 extends ERC 20, ERC 7540 extends 4626, whatever. We can talk about the details, on other times, but if there's any major points that anyone wants to call out, I think that. The most important place to land is having some form of an extension header, even if it's not super formal. How extensions are defined.
* That's basically my position with why I made the ERC in the first place. 

**Pooja Ranjan**
* Well, thank you for sharing. As I can see here in the comment, like it is something that may be of more relevance. Post a working group is implemented and there are a lot of things that needs to be clarified with respect to ERC especially when we are trying to have it with tags and having a different categories. So it's good to have the proposal on the table. We can perhaps have it discussed in future when we get clarity on the specification of ERC1, if that helps. 

**Joey Santoro**
* Yeah that helps. I can even pull requests from initial ideas. But yeah, that's a good place to end for for now. 

**Pooja Ranjan**
* Thank you so much. And E if there isn't anything further, we can perhaps stop sharing. 

**E**
* Oh, sorry. Yeah. 

**Pooja Ranjan**
* No worries at all. And now we can move on to call for input. Back to you, Sam. 

## Call for inputs [44:53](https://youtu.be/ib9xInX3nkk?t=2693)
**Sam**
* Sure. So the first one up here is withdraw EIP 7199. Just reminding everybody about it. It's a rule that should have been in EIP one and it's not. So this is just to remove to withdraw that pull request. The next one is remove external implementations from ERC 20. This one probably has a bit more debate on it.. There are links in ERC 20 to particular reference implementations, specifically Consensuses and Open Zeppelins and Dexron raised the concern that that unfairly privileges those implementations. There's some question of neutrality whether we remove them because it's final or not. So this is issue 287 and the deadline is November 19th for comment on that.
* So another one that came up is ratifying the editors listed in Eth one. So right now we don't really distinguish between editors and subtypes of editors in our governance documents. So Gajendar and Ben, there's been some question as to whether they're full editors or not. And I would like to settle those questions once and for all. So I have a call for input open on that. Deadline is November 19th for comment. And then finally we have there's an accidental function that was included incorrectly in ERC 223, Before it was finalized. It's pretty clear that it was like a git merge error, at least in my opinion. Deadline for comment is November 16th on that one.
* Yeah, I think that's all of the current calls for input. Yeah. Awesome. Thanks. 

**Pooja Ranjan**
* Thank you Sam. And one point on that one of the call for inputs was between distinctions of editors have added here a EIP link of editors and associates. So as of now there are two sets of people who are contributing as editors. Editors are editors. And there are a few associates who are trying to support the editing  EIP process, but they haven't been added as full editors. Can we take a look at this Google Sheet? I have tried to add all individuals who have came forward to support  ERC editing as well. So people who are looking into both side of EIP and governance or supporting with documentation have been listed here based on editor or associate.
* If there is any change, please do. Please do let me know. I can update it, but I think this will give us a very good visibility of how many peoples do we have around in order to support the reviewing of ERCs and EIPs. 

**Lightclient**
* Can you add me to your ERC editor please? 

**Pooja Ranjan**
* Okay. I will go ahead and do that. 

**Sam**
* Yeah. So there's the distinction between like EIP editor as a governance entity or role. So like and then there's the people who only look at ERCs and the people who only look at EIPs.. And that's kind of what that call for input was meant for clearing up. It's like, who is actually a governing editor? 

**Pooja Ranjan**
* All right. Yeah. Got it. 

**Gajinder**
* I can also act as an associate for the ERC. 

**Pooja Ranjan**
* Did you mean you are already an editor? You mentioned associate as an ERC By the way, this is open for comment, so please feel free to leave your comments if there is any mistake I Think. Joe, you mentioned that there is a mistake in the name spelling. I will fix it later on. 

**Gajinder**
* Just a comment. 

**Pooja Ranjan**
* Yeah. Gajendra Singh, sorry I missed that part. Do you mean to be added as an editor? For a ERC as well. 

**Gajinder**
* Associate for ERCs. He is better because. 

**Pooja Ranjan**
* Okay. then we may get a little bit more clarity on that part. As of now, we have added editors and associates, because those are the tags we are using in discord for people to know, but editors are people who are already listed in EIP one. I hope when we get clarity on call for input, as mentioned earlier, we'll be able to add it over there. But understand the intent is like you may not be actively reviewing, but open to help and extend your support, if that's my correct understanding here. 

**Gajinder**
* Yep. Got it. 

**Pooja Ranjan**
* All right, let's move on to changes to final proposals. We have a bunch of. 

**Lightclient**
* Can we go back to this website question because we got to figure this out. 

**Pooja Ranjan**
* Do we have Panda back on call? 

**Lightclient**
* I don't know where he is, but we got to figure this out. Guys,  we split the repos on Friday, and it's a tire fire out there. 

**Sam**
* So, I mean, does it matter what we do with the websites right now? As long as we get the rules for the markdown files consistent? 

**Lightclient**
* Yeah. I mean, I don't think it really matters so long as. Yeah, I mean, I guess it doesn't really matter too much. I think it's a lot simpler to just go with the separate websites and have a link between the two, because we just have to make the changes to the documents. And if later on we're like, we really just need this to be a single website, then we can write like, I think that's a lot more development work. You need to update the website to support the different formats, or you need to have some sort of software that translates the URL to the ERC EIP format.
* Like, I think that there's a lot more work to do there than just having separate websites. 

**Gavin John**
* Yeah. 

**Sam**
* My concern is that, like some of the rules we have in EPW right now do depend on the content. Like, are we still going to have the rule that like a course? Well, maybe the other way around. An ERC can only reference core EIPs that are in a more advanced status, like. 

**Gajinder**
* I can always seamlessly redirect. I mean, we don't really need to have a merge website as soon as long as the look and feel sort of gives a unified view to the user. 

**Sam**
* Yeah, that's true too. 

**Lightclient**
* So I don't know. I mean, there's a lot of things that can be checked in the ERCs. There's I have no I don't know, I don't really have a lot of thought on exactly how we want to deal with that. But I think that, like, right now, we're not in really a good place where we're kind of asking them to put things that don't actually link to anything. So it works in the back end with some translation we have, and I want to resolve that ASAP. I know more things will break along the way, but to me, the fastest and simplest thing is to have separate websites and we can go from there. 

**Pooja Ranjan**
* So the one person who is actively working on it and is not in favor isn't on the call. Matt, I'm not sure if we would be able to make any decision without that, because in the last meeting, we made decision in your absence, and that was different from what we are coming to a conclusion today. 

**Lightclient**
* Yeah. I mean, I don't know. 

**Pooja Ranjan**
* Lets take it on the discord and see, because there we will get. 

**Lightclient**
* Yeah. I mean, this is just. This is terrible. 

**Sam**
* Open a call for input, and then we can put all of our shit on there. 

**Lightclient**
* Oh my God. 

**Sam**
* Got 1 or 2 websites, and then we get to wait 30 days for access to not answer. Yay! 

**Francisco**
* Is there a list of what's broken? I don't really understand. 

**Gavin John**
* You can. 

**Sam**
* It's even if it's not broken what we want to decide. Like, let's assume everything works perfectly, right? So whatever we decide, let's assume everything works. Do we want ERC start ethereum.org and eip.ethereum.org? Or do we just want eip.Ethereum.org? 

**Francisco**
* Yeah, but that seems like that can wait. But what's broken right now should not wait. 

**Sam**
* Yeah, that's what I was talking about. We should come up with whatever markdown rules we want and then worry about which website organization later. 

**Gavin John**
* I mean, is. 

**Lightclient**
* There any disagreements about the markdown rules? 

**Sam**
* So is the markdown rule we use ERC- whatever. VMD in Ugcs and then EIP- whatever MD in in everything else. Yes. Okay. We can make that work. 

**Lightclient**
* Are there other markdown rules that are problematic? The other main thing I think that I would like to change is to change the EIP and the preamble of ERCs to ERC. 

**Sam**
* Yeah, I mean, that would be fine. Or we just change it to number that way. It's not different depending on what type of file you're looking at. 

**Lightclient**
* Yeah, either of those are fine if you have a preference. I really don't care. But I think that. Yeah, we need to make a decision. 

**Pooja Ranjan**
* So any final statement, any from anyone on this one? Do we have a decision or. We are still working with the unified website? We'll continue discussing on discord and maybe come back with a decision for the next meeting. Okay, so. 

**Sam**
* So right now it's we'll keep ERC.ethereum.org working and we'll keep eips.ethereum.org working as they are today. So both on Eips, we'll fix the markdown rules so that it's same for authors. And we're going to rename EIP in the preamble to just number. 

**Lightclient**
* The problem is we're getting to. The thing that I don't want to do is write these translations to convert them back to EIP whenever they get to the EIP website to build the full website. 

**Sam**
* Well, we don't. I'm not saying that's how we're going to end up implementing it. Right. I'm just saying. Like in the short term, we might need to do that. And then in the long term we might have something better. 

**Joey Santoro**
* How much crosslinking is there between EIPs and ERC? In the split nomenclature. 

**Sam**
* That's a good piece of data we should get. 

**Lightclient**
* I think relatively little. 

**Sam**
* Yeah, it's probably something. 

**Joey Santoro**
* Yeah. If it was. 

**Sam**
* We need to store or we need create to. And that's about it. 

**Joey Santoro**
* If it was close to zero, then we could probably just like clean, split everything and like kind of edit out those references or something, I don't know. But yeah, that's good data to get so well, I mean. 

**Lightclient**
* The cross link I think are going to have to use absolute links. Like, I'm not really sure there's another way around that. 

**Sam**
* Yeah, exactly. 

**Lightclient**
* So if you want to link to an EIP from an ERC, you would just link to the Eth website. 

**Joey Santoro**
* The website or the GitHub. 

**Lightclient**
* To the website because if you link to the GitHub, then when it goes on to the website it will link to the GitHub. And we mostly don't want people browsing the GitHub unless they're looking at the history of the EIP or something. 

**Sam**
* Yeah, it's like if you're on GitHub you should probably like ideally, if you're on GitHub and you click a link, you stay on GitHub. But I'd rather, you know, if you're on the website, you stay on the website. 

**Joey Santoro**
* Yeah, that makes sense. 

**Pooja Ranjan**
* You know, you have to add something here. 

**Danno Ferrin**
* Yeah. So when your last call, if anyone had anything to say, this whole process that we went through of splitting the repos, I thought that two separate websites was part of the process and always part of the end goal to have erc.ethereum and eip.ethereum. So feel like, you know, changing this last week. So it's all going to one website is a very material change in the opposite direction inside of one week. So I was always under the impression it was going to be two separate top level domains. And that is always what was operating on these past six months.  

**E**
* I think I stand with we should have these two separate top level domains. I think it's it's very valuable. 

**Pooja Ranjan**
* Okay, we'll get there. I know this is an hour here, and I just quickly want to check on the next meeting time. We know that, uh, due to daylight shifting, there would be a different time zone here in the United States. Not different time zone, but the timing will be different. Do we still want to keep it at 1400 UTC? And there is another reason is the roll up meetings that is going to be on exactly the same time. Editors have any thoughts, want to keep it or have any other proposal? 

**Lightclient**
* I'm not going to be able to make it if it's going to be during the roll call. 

**E**
* So yeah. 

**Sam**
* I'm fine shifting it to after the rollout call. That would work for me. 

**E**
* That's actually. 

**Pooja Ranjan**
* But after the roll up call is the EOF call. 

**Lightclient**
* Somebody's going to have to look after the EOF call then.  I mean, yeah, we're going to have some conflict I can do before roll call, but I know that's starting to get pretty early for some people. I could do after the roll call. 

**Sam**
* I don't mind. 

**Lightclient**
* Or we could skip next one. 

**Sam**
* Oh, is it just a one time? Oh, I mean roll call. 

**Lightclient**
* Yeah. Roll call connects every month. 

**Danno Ferrin**
* So every month on the same week of the month. So sometimes it's going to conflict. Sometimes it's not. Well for the call. 

**Lightclient**
* So here that we're going to make bigger changes to the number of calls and days of calls. Maybe the beginning of next year. So we don't need to go overboard on. Figuring something out right now. 

**Sam**
* So this next call, let's do it after. And if Pooja, if you're running the EOF call, I can I can run this one. 

**Pooja Ranjan**
* No, I'm not running. Actually, it is Matt who is running. I'm just recording it. I'm just saying that because Matt again will not be able to make it. 

**Sam**
* I think that's fine for one call. 

**Lightclient**
* Yeah, I got to go to the call now, by the way. But we need to figure this website out thing before this end of this week. We can't wait till the next call. So let's talk about it on discord. All right, I'm going to drop. All right. 

**Pooja Ranjan**
* Thanks guys. So thank you Matt. So finally we are going to be at the same time at 1400 UTC. Is that the decision for the meeting on November 15th? 

**Sam**
* I think we were saying after call. So that would be what? 1330 15 UTC. Yeah. 

**Pooja Ranjan**
* Oh, yeah. Yeah. No, no, you are right. 1330 I don't know, on my calendar. No no no. EOF And roll call are also conflicting. So yeah that. No, no you're right. Figured out. 

**Sam**
* It's 1530. 

**Pooja Ranjan**
* Okay. Perfect. Yeah. All right. So let's go ahead and do that. Francisco, I know we are over time, but please go ahead and add if you have to add something over here. 

**Francisco**
* Yeah. Sorry I had one of the items in changes to final proposals. I don't know if we can cover it now or I can make it super quick, but basically ERC 1271 there is a small security concern and we want to I'm one of the authors. We want to update the security considerations and the reference implementation, but not the spec. So since this is a final ERC, it requires would require an exception. How do we proceed with this? 

**Pooja Ranjan**
* So generally we discussed this kind of exceptions. As you can see it is listed on the agenda for EIPIP meeting. Unfortunately we could not get to attend those today. I hope those are being attended by editors async. If not, then we'll be happy to bring it up in the next meeting. Generally, we try to get all editors on board for making any changes to any of the final proposals. So even if it is security related, we need to get all editors on board for that. 

**Francisco**
* So what's the next step that I should do? 

**Sam**
* Do you have a link to the changes you want to propose? 

**Francisco**
* Since it's since it's a security thing, we're not making it fully public yet. Yeah, but I think you're in the telegram group. Yeah. 

**Sam**
* Yeah. I just wanted to ask you here. So I will make a call for input, which is like our formal way of making a decision with a with a date. And. Okay, we'll let you know where it goes. 

**Francisco**
* Yeah, sure. Please tag me in on that. 

**Sam**
* Sure. What's your GitHub username? 

**Francisco**
* It's ffrangio. I'm also there on the agenda. 

**Sam**
* Oh, perfect. Okay. Yep. 

**Pooja Ranjan**
* All right. Well thank you everyone for joining us today. See you all on November 15th at 1530 UTC. Have a great day. 


---------

## Date and Time for the next meeting

Nov 15, 2023 at 15:30 UTC


---------
## Attendees

* Pooja Ranjan
* Sam
* Gajinder
* Lightclient
* Francisco
* Joey Santoro
* Danno Ferrin
* E




