# EIP Improvement Process Call #6 Notes

### Meeting Date/Time: Wednesday, March 25, 2020, at 15:00 UTC
### Meeting Duration: 1 hr 
### [Audio/Video of the meeting](https://youtu.be/ZPy1x2clAqk)
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/10)
### Moderator: Hudson Jameson
### Notes: Pooja Ranjan


----
	
# Summary


### Action Items

* **Action Item 6.1**: Hudson, Sam and James to work together about how the bot update stuff in the blockers now. Before the next meeting create a new notion document with 
    * a proposed plan for what changes need to be made and 
    * a time line of when to make and also 
    * get some ideas early on about funding.


### Decisions

* **Decision 6.1.1**:  To have a deep understanding of the Bots and the inner workings of the application for *Migrating EIP content to ethereum.org*, a separate call will be organized and notes will be taken, might even be streamed for transparency reasons. 

* **Decision 6.1.2**:Hudson will lead the EIP migration group and will get help with whoever wants to attend meetings and brainstorm and maybe a separate telegram group will be created.

* **Decision 6.2.1**: Store history or the process of an upgrade in an Informational EIP that is a post-mortem on hardfork.

* **Decision 6.2.2**: For EFI, we can create an Informational EIP, which just link back at EIP 1, where you say here's the process for the core EIP and you linked to Informational EIP that describes the EIP centric process.

* **Decision 6.2.3**: There is not a way to upgrade active EIP such as EIP 1, so the way to upgrade EIP 1 to specifically set on precedence alone and not on a process that's recorded and the precedents for upgrading EIP 1 or other active EIPs of which EIP 1 is the only active EIP, is to do a pull request for that EIP and have a go to last call and have people agree on it.


----


**Hudson**: This is meeting number 6 of the EIPIP meetings. 

### 1. Migrating EIP content to ethereum.org - [proposal discussion](https://github.com/ethereum/ethereum-org-website/issues/343#issuecomment-575446111) and [draft proposal](https://www.notion.so/efdn/Migrate-EIP-content-to-ethereum-org-b50f198d8c254e2eb89790658e9079a8)

**Hudson**: Okay so the first one is one we've been talking a lot about on the telegram chat, which is migrating EIP content to a different Ethereum.org address. Sam made a proposal document, so I think that's on notion, right Sam?  

**Sam**: Correct,  and I shared it with this telegram group and the EIP gitter Channel happy to like turn this into an issue on their respective GitHub repositories if that's easier. I think, that'll be one of those things, I'm looking for feedback on, today.

**Hudson**: Okay, sounds good and that actually is the first agenda item, so if you want to take it up. I think our Agenda is pretty light today. We can spend a good amount of time on this if you want to just walk us through that and a lot of it we've already heard before but those we haven't on the call is some of the proposed solution and the skepticism criticism section specifically. So I'll let you take it away and then the people have questions along the way and discussion will go through that.

**Sam**: Sure, sounds good. So good morning everybody if you guys weren't on the call 2 weeks ago, my name is Sam I work as a web developer at the Ethereum Foundation primarily on Ethereum.Org. so you can imagine how this idea popped into my head but what this **proposal** essential is - *it's really an effort to make the EIP content on the GitHub and EIP sub-domain, just more discoverable and more accessible*. What are ways that we can increase exposure and awareness from people inside and outside of the Ethereum ecosystem, and  just like educate them get them engage with the EIP process. So, *this proposal isn't to change anything about the process itself, it's really just a change to the public website that would display these existing EIPs*.

The proposal is in agenda, we can walk through it and its entirely if people would like or we could kind of leave at to asynchronous feedback and  I'd encourage anyone who has input to go ahead and comment in this [notion document](https://www.notion.so/Migrate-EIP-content-to-ethereum-org-b50f198d8c254e2eb89790658e9079a8). It should be publicly accessible to comment but essentially a high-level what I tried the layout was here is the problem statement which hopefully like everyone agrees upon as like a it would be beneficial thing to get more exposure and increase discoverability of this great content and these standards of the community has developed from the people I've spoken to, within the EIP editing process and we have managed the repo in the past; it does seem like they're just has a bit much capacity to focus on this or like making General improvements to the site so the opportunity I saw was how can we  make that better and I outline some of the things we've tried up to this point I such as adding links from Ethereum.Org, doing some on-site optimization of the existing EIP site and starting to build out at the additional content on Ethereum.Org that talks about EIPs and links to additional content there. So what this proposal essentially out there is like hey one option could be if the main goal is to improve like the search rankings of this Yeti contest to actually migrate all that content from the existing sub-domain to a subdirectory on Ethereum.Org and I layout some of the reasons like why I and some others think that would be beneficial, some of the risk we think involved and some of like the skepticism we've received from a lot of folks in the community. So at this point I just like open it up to questions if there are any, otherwise yeah if we have time and people are interested we can definitely dig into specific aspects of the Proposal.

**James**: I have one thing or one question. In the problem section, I don't know if it's worth putting this explicitly or not at this site itself is also very difficult to discover EIPs within. I see that you said that there is low bandwidth from EIPs to make improvements but it doesn't, it might be helpful to say there is a problem with the site that needs improving and then the sub-problem of that is that there aren't people working on it. Coz I don't know how many people really are at the Forefront of their mind that there isn't search functionality on the site it's very hard to find a single EIP unless you have back information about where it would be beforehand and even then you have to scroll through the site all the way to the bottom. If it's in draft or active and you have to know that in advance there's not a way to navigate EIP easily from withing the site itself. 

**Sam**: Got it, yeah just made a note of that. Yeah and you know I think like with this problem statement and proposed Solutions like there's definitely alternative ways to try to address this which as of now yeah I haven't really outlined in the proposal and I'd be happy to. For me it's like **two main pieces**, James you just touch on **one** *is like okay maybe the existing like site interface and UI is suboptimal and there's just general like UX improvements we could make to like make the EIP content easier to navigate, easier to comprehend and share and somehow engage with* and then the **second** *main piece is just like the exposure of the content itself, primarily from an SEO stand point*. Like the keyword research I've done around EIPs and like Ethereum token standards, there's not a ton and this is just using like say like Google AdWords, keyword research tools to get an estimate of like overall impression volume. As you can imagine there's really not a time other than like the most popular EIP you such as like erc20 and that erc721 token standards but my hunch is that there is a decent amount of just like long tail search for specific EIPs that in aggregate like do make a pretty significant amount of interest. Right now the EIP sub-domain just doesn't seem to rank very well. **Google does tend to treat sub-domains as like independent entities** which as we've discussed like can be good for certain things and bad for others. In my mind it's bad for SEO rankings where we have this incredibly old and authoritative powerful domain at Ethereum.Org, that we could leverage to help like you have this content of boost in a sense of like having those pages on the site being able to link to those internally and  index those as part of the main domain, I think could potentially like really boost this content in search results. So those are the two main things I think that we could potentially separate as like UX/UI improvements to the site itself and then just like improving exposure and awareness of the content primarily through like SEO benefits.

**Hudson**: Great, I completely agree with that. James do you have any other parts of your question or comment?

**James**: Another, this is may or may not need to be included but just so everybody on the call can here this part is that the **other problem** is that *the actual Improvement of the EIP process is blocked by improvements to to the site and because there are changes we can't make unless someone makes changes on the interface, that  represents it and so then some of those things you just hold there*. Like I've made a proposal last year to do an inactive status and then the feedback was well there's no one to make the bot and the other things and the site renders it then that way it's just frustrating to hear from both sides at what we can't change it but then also the proposals can go through at the same time, anyway.

**Hudson**: Yeah, I agree with that heavily. I think that I'm starting to get really strong feelings that moving the site and with moving the site improving the bot and the website are top priorities because like you just mentioned James, without doing that we can't make iterative changes to EIP 1 or the structure of the documents because they can't be updated on the side and there's not search functionality and a few other things. So it's kind of like, it's exactly what you said and I looked through the solution and the skepticism criticism and I mean if you look at it really **all we're doing is moving the EIP before Ethereum.org  to moving it after Ethereum.Org with the benefit of a lot of SEO,**  and also oh it's mainly the SEO I'm focused on; because I think we do need more visibility for looking up EIPs on something like Ethereum.Org and it's not a case of like trying to separate the two entities because we already have eips.ethereum.org and I think the only people who have these illusions of if it's a (blank).etherum.org being completely separate or people who are really in the ecosystem and what what this is for is for people in and outside of the ecosystem. So, doing etherum.org/eips is not going to make a huge difference. I don't think as far as like making an illegitimate so I don't like that argument very much, even if other sites like seem to turned away from that for standards, like very big professional standard site, this is a blockchain standard site and it's like Bitcoins bips or you know python, it's like made after the bitcoin standards and python standards in which the python URL is python.org/peps  I think. So all that to say, I think we should do it and the only other thing would be yeah they're just going through each criticism I guess, I can just do that real quick for my opinion on it and then Sam, I'm just stop me if you have a different one. I think you've already written down here.

**Sam**: So yeah one quick point I'd make Hudson, just to change your comment on like actual changes to the EIP process being blocked by the current EIP site is like once again this specific proposal at least like really isn't making any changes to like the processes itself or really even to like the structure of the application itself it would just be like to start mirroring one page to etherum.org. So I think what I'm trying to say is like maybe those two things could be solved independently, like if there is something about the current structure that's blocking changes to the EIP process, like we might be able to address that and try to solve that without this entire proposal or maybe it will make sense to change as part of this proposal. It would help me to understand like what the specific issues are about the current site that are blocking you but just to say that there was this changes may be able to be made in isolation. 

**Hudson**: I consider the more together and the only reason for that is usually things aren't usually you can do things in isolation that's good to separate but the bot actually talks to or I should say the web server looks at the EIPs repo and does updates based on that; so the bot is in a way communication with the web server even though it's not bot to server, it's server to bot. When we do the new one, we're going to have to make sure that it's set up in the same way as the old bot and while we're doing that we might as well update the bot because it's going to be a waste of time to it would be a waste of time overall to change the bot to just literally all it does is go to the ethereum.org/eips site, when they were going to want to do more to the bot afterwards, does that make sense? It's better to do the bot upgrades, not all of them but like a set up one or two or three priorities one of them being documentation and then get a few people helping on it and then move it over after a couple of those priorities are set, so that we have something we can work with very fresh on the other side when we move it so this is this also helps because this could kind of be an efforts that combines to do separate things until 1 and that's a little stronger when we say this is relaunching the new EIPs and this is what we're changing and etc.

**Sam**: Got it. Okay yeah! I like at this point I don't have a deep understanding of the Bots and the inner workings of the application so whenever the time comes probably just worth touching base with you and James till I get some specifics on that.

**Hudson**: Yeah let's have a separate call for sure and take notes, we might even stream it, just so that  people have an understanding of what we changed before and after for transparency reasons. And then William said "couldn't we just modify the existing sub-domain? I'm not sure why we need a new domain specifically if we just put in the work on the existing EIP sub-domain, what wouldn't work?"  So I think you might have missed it while you were logged off William, but it's the SEO it's not returning as many hits and I'm not an SEO guy, Sam is. So you can explain it better Sam if you want to just in a few sentences. 

**Sam**: Yeah, it's a good point and worth reiterating and like what I tried to outline at the beginning is like what this proposal really tries to address is like two separate things is like 
1. is like potential UI and UX improvements on the site 
2. is exposure of the content primarily through SEO.
For number 2 to happen, to get the SEO benefits, from my understanding and you know I've been out of like the hardcore SEO game for a couple years now but it was my career for a few different years and I don't think it's changed too much but I think to get to the SEO benefits like we would need to migrate this content to re-domain.  William, to your point to get the like UI/UX and just like General site improvements that is not require migrating this content at all. Like we could try to find a way to get resources allocated either my time spent improving it or you know funding Gitcoin bounties to use to get fixes to the site, like it's not at all requirement to do this migration to get those site improvements. I think one of the reasons I mentioned in my proposal, as like a reason or like an additional benefit of migrating is that on ethereum.org we already have a lot of like functionality in place that we could leverage in essentially reuse such as **Site Search**. So that we wouldn't have to re implement it in a separate code base, we would just move the content onto ethereum.org and then we would just get site search and like table of content features out of the box if you will. It would definitely come with that upfront cost of like actually executing on this migration now.

**James**: Echoing Hudson thoughts,  I'd see value putting. Well technically you could separate the things into developing the EIP sub-domain and having in /EIP that it's much, keeping them together makes a lot more sense to me and mostly from a resources and also like the people involved, the people who are going to be making the changes should be able to do the changes where they want, at the end of the day, cuz we're grateful that you guys are.

**Hudson**: Yeah, that's very intertwined both the Bots and the website migration. It's not so intertwined that it couldn't be done separately but like I said earlier it it's a waste of time if it's done separately. 

**James**: Definitely.

**Hudson**: so William said, "In other words, sub-domains have a harder time in SEO?"
yeah if it's blank.ethereum.org that's worse than ethereum.org/(blank). 

**Sam**: An easy way of thinking about that is like you know the Blogspot days are probably over but if you do remember when like anyone could essentially spin up a sub-domain on blogspot.com, like Google recognizes that distinct sub-domain can be under control of distinct groups. So they tend to the treat them as separate website and the other pieces that just like the ethereum.org core domain itself just has massively more inbound links to it compared to the EIP sub-domain.

**Hudson**: So we don't have to spend the whole meeting on this but I do you want to give everyone else an opportunity to speak. Who else has opinions on this or comments?

**Brent**: Just a small one, when I first started in that's like six months ago I was trying to learn my way around that EIPs in the SEO it was really hard so any anything that want to improve that is good, just in my view.

**Hudson**: So what I want is an **action item** *I want to work directly with Sam and James* but mostly with Sam James only for the necessary explanations to Sam about how the bot update stuff in the blockers we have, but before the next meeting I want to get a new notion document going which is up a plan a proposed plan for what changes need to be made and a timeline of when to make them that's real rough that we can change, nothing official but and then also like get some ideas early on about funding and just getting this done. Cuz if we get this done in the next couple months, while we're making decisions in the on the back end of how to change the EIP 1 and other stuff in there, then we can quickly just do all those changes we can quickly do all these changes later after the merge in the migration is done or even you know right at the end of the same time so that we have this huge package to present the community.  Here's the updated here's what the update of EIPs that we are the updated EIP 1 plus the updated domain plus the updated bot plus the updated Site.
So yeah I think something like that would be really valuable and maybe not all those things at once maybe it needs to be more iterative that I'm talking about, so what will need help brainstorming but *put me as lead on that and then I'll get help around me*,  whoever wants to attend those meetings and brainstorm with me and get a maybe a separate telegram chat and yeah so that's all I have about this topic any last words, Sam, that sounded threatening :) anyone else have any comment?

**Sam**: I guess one question I have is just like in terms of gathering additional Community input like would you recommend, I open this up as an issue on the repo, is there any other groups you'd recommend like sharing this proposal?

**Hudson**: So you have the proposal to do it; once we make a proposal for how we're doing it we, can put both proposals in an issue and also elaborate on that issue on Twitter on the Ethereum.org account and across some communities like the AllCoreDev Gitters and just say we're wanting to do this, or some of us are wanting to do this and we've been talking a few meetings about this, here are the notes, here are the two proposals we want feedback or opposition, if there is any.

**Sam**: That sounds good to me.

**Hudson**: Anyone else?

**James**: I'm sure I can do that call. 

**Hudson**: What was that again, that you cut out?

**James**: For sure, add that the conversation with me, you and Sam about the blockers for the process.

**Hudson**: Okay, perfect. 

### 2. Adding 'Motivation' in MetaEIP of an upgrade 

**Hudson**: So next up is adding motivation to the Meta EIP of an upgrade. I don't know who this that was.

**Pooja**: This is in continuation to discussion in our last meeting. At the end of the meeting, we were discussing. It was my  proposal initially that we should be adding motivation section in the Meta EIP of an upgrade. The initial thought was, the process that we follow for an upgrade is like kind of changing. From past two of the upgrades at least, we've seen that the process keeps on changing and I was looking for a place to store this process that we used for a particular upgrade.
If we keep it updating on the EIP 1, the next time the process change and we edit EIP 1, the process for the last upgrade will get lost. So I was thinking if we can add it into the Meta EIP of that particular upgrade, people can always find and this thing will be stored forever.

**James**: Do you mean the process of the process for doing upgrades or the specific process that was taken at that time. Like there's a standard that we're going to we're trying to follow when the there's what actually happened at that time.

**Pooja**: At that time, I meant. Like for example in Istanbul, we did the 'schedule based' upgrade. The process that we followed, it can be a case study for people coming up in future and trying to understand how we did that thing. So my idea was to save the information about that. This time we are including EFI into into the process and doing an EIP Centric upgrade, so I was hoping to have this mentioned at least in the Meta EIP for Berlin. So that people would know that that is process that we followed for Berlin or maybe if we are not changing it any further, it's fine and it can we moved to EIP 1 but if we're changing to some other upgrade process for next upgrade it should be mentioned in the next Meta EIP.

**James**: And the reason for having that is for people to be to learn from the process or what does that add for you for you to come?

**Pooja**: I was thinking, at this point of time we are doing a lot of experiments so there may be a point when we would like to analyze all these data and see which one was the most successful upgrade for us or the process for the upgrade that we should be following. So if we have this kind of data available to get analyzed at one point of time, that would be helpful but if we keep on losing it it would be difficult to collect back.

**Hudson**: I think it's a great a great idea to collect that data that that historical perspective so that we can improve upon it. I'm skeptical that should be in the Eip1 in any capacity because what EIP 1 is, the purpose of the EIP 1 in my opinion and how it's kind of been described in the readme is if you are someone who wants to make a change to Ethereum and you want a succint guide on how to do that, what the different types are, what you have to do to accomplish that and who reviews them you go to EIP 1.  If we start putting stuff about hard Forks in there specifically I think that would be make it bulkier it would also detract from the purpose of the EIP 1, which is just for people who are writing EIPs cuz if you're writing EIP, you don't care how Core EIPs are processed. I think it's a good idea to have it in the meta EIP potentially but that also introduces some opinion and non-technical material, so those are my two comments so far.

**Pooja**: Basically this motivation section is available in almost every EIP, it is missing in the Meta EIP only. I understand if people have reservation with the word 'motivation' because it is actually not the  motivation but is the process that we're trying to document in that, which is that actually the non-technical part of it, but for the sake of history we can have it and I don't see any downside of that having it in there.  If we would like to change the term, I'm okay with because Meta Eip is the only EIP where motivation section is missing.

**James**: I see one downside from including and as far as having the information available for people who are trying to study the EIP process or improve it, it would be a little bit more digging but there is plenty of blog posts and things that are available about around the time of the fork that would have even more meta information about the decision process. so in my mind if someone is trying to figure that out there is that it would take a little bit more digging but they is available for them to find it even if it isn't on the Meta even if it isn't in the motivational section.

**Tim**: Thing that is odd about the 'motivation' section in the Meta EIP is the motivation is basically the list of EIPs that is included in the hardfork, right? it's like we're saying, you know why do you have this upgrade ? Well to implement these things that are listed here and you can't really have a why that's like more elaborate than that because then people will start disagreeing on it. It just becomes like a place for like political argumentation. I agree it's a bit odd that they are a bit different, the cost of making it similar is high and I'm not sure what the value is. Especially, most of these decisions are like technical upgrades. Look at the Berlin, the motivation is to add the BLS12 pre-compile. I mean, it feels odd to like added motivation for that.

**Pooja**: I get the idea of using the term 'motivation', that's why I mentioned that if we would want to use 'process' or something else. My basic concern here was like we would want to save the information about the process. Because the last time what we did for Istanbul, I saw a lot of effort in a James excel sheet and the process that we followed - it was scheduled base, at what time and how many weeks will be required for this and that, everything was there but we can't see. I mean of course if we keep on digging on that we will be able to find it somewhere or the other but I thought it would be a good idea to keep it somewhere in the Meta EIP maybe with a different heading if motivation is contradicting the thought of 'motivation'. 

**James**: I would say even with a different heading there is a coordination cost to having that information there and that and that is that it would be great if everything that's on the EIP repos agrees and shows the current understanding of what we're doing for the process and if we have certain pieces showing historical information about what did happen if it is a place for people that disagree about what is or shouldn't happen and pointing if they like or well for this last one we did this and then really anyone who is talk talking about the process should be pointing at the current process and so having only that information the one that's easy to find, I think will help with that kind of fragmentation of narrative.

**Hudson**: I think that we need this data somewhere that it was exactly what Pooja is talkin about. I think it needs to be somewhere cuz I don't want we'll have to go digging for it especially as time changing  and we improve and we have to re-explain to people over and over again. but I almost feel like post mortems that the cat herders write, might be a better location and might be something that people can turn to and say oh this is an opinion piece by the cat herders rather than this is something cuz I mean we try to keep non-technical and opinion out of the EIPs except for EIP 1. So EIP should be technical documents with technical  motivation, implementation, security considerations etc and EIPs were created by Alex B. to document what went into a hard Fork at what block and which EIPs went in and it should not to make it too complicated. So that, I think that's the main concern is that it would are the main concerns I should say is that it would complicate it and impose like James said something that could be disagreed on by opinion but we do need to put it somewhere. So I'm thinking maybe somewhere else.

**James**: I just have an idea for a place, having an **Informational EIP that is a post-mortem on hard Forks**.

**Pooja**: Sounds good, that can be a place I mean like it should be related to that particular upgrade.  If not Meta, post-mortem could be a good place because these are the key documents that would be referred when people would try to analyze these data.

**Hudson**: So in doing that we might need to further specify what an Informational EIP is because I don't know they're completely well cuz  an informational EIP according to one is more like a guideline,  it does say information, I thought it would say announcement. So yeah it would fit in the informational EIP.

**Pooja**: Okay,

**Hudson**: That sounds good we can put it in there. Anybody else have comments. 

**James**: And to go backwards and do one on Muir Glacier with you, Pooja. 

**Pooja**: Yeah, I was about to email you for that. I have one more question here before we move on, the process that we are currently following here for the EFI and the EIP Centric, so where we are getting at, should we go ahead and add that to EP1 Or should that be documented as an informational EIP somewhere, for Berlin?

**Hudson**: That's a hard question, I don't have an answer.

**Pooja**: Because this is exactly what I'm trying to achieve here is, like a place for documenting the process. Istanbul is past, so if we will add it in the post-mortem of that, that is quite good, quite okay but Berlin is coming up and we may be seeing more future upgrade so we should have decided place. I'm okay, with keeping it anywhere but that should be the place where we can refer people to go ahead and check what we did. 

**Hudson**: There are two paths, I can see us taking on this the current because there's a lot of rules that are involved in or there is beginning to a lot of rules what it used to be is you take it to the core devs, they decide it's going in and then we have that complicated, non-document process. Now it's we have EFI and we have Champions with specific edicts and we have you know that  the core devs deals with this stuff and not the other stuff. They deal with Technical and not political and we're working on that problem too and putting that all in EIP 1,  I'm always just trying to I have the protection of the EIP 1 to not make it too much information people are turned off to the process or too much information so that people you know most people who read EIP are going to be reading it for erc's cuz we really get stuck in the core EIP stuff that really most EIPs or ERCs.

**Tim**: Maybe the informational EIP make sense, right? which you just link back at EIP 1, where you say here's the process for the core EIP and you linked to informational EIP that describes the EIP centric process.

**Hudson**: That's a good idea. 

**Pooja**: Yeah, that make sense to me. 

**James**: I'm a little bit, I'm not like stanch on this, and I know I don't have the vision of EIP 1 totally. I've liked the idea of explaining it and making it more usable, like adding it be single-source truth for the Ethereum governance in general and all of those things at and you're right in that I am way too much in the core EIP so then I over do that stuff. I wish there is someone out there that was kind of doing the same thing but for ERC, so we don't exactly have that at the moment but if we, like I added in that a table of contents and I think there's ways of expanding it even if it got large but it could be quickly not navigate available for people. I just start to worry that,  my worry comes in two forms, **one** is finding the right information to the right time can be difficult for people so having having it, oh well to get the information for this you actually have to go over there and have him go over there. If it's linked in the EIP 1, that kind of mitigates that a bit, but it still is a little bit harder to find and then **the other one** is decision-making processes around things like the hard fork stuff  or EFI, should we have the same process for changing the EIP centric model  be the same process for changing EIP 1?

**Hudson**: That last question we need to figure out how to change the EIP 1 before it can be answered. The rest of your question statements, **I would say it works to be an informational EIP** that is set to active status because EIP 1 does say that some information on process EIP such as EIP 1 **may be in active status and they are never meant to be completed**. 

* So we would literally have it be EIP and then whatever number is the one for how champions in EFI and whatever we call that umbrella process is for a core developer decisions, in a core dev meeting etcetera can be that EIP and we can keep that number forever. 
* If we change it we just do a pull request and you know get consensus on the pull request, which we could do easily with the core devs to agree with the process and then it get changed. 
* So it can change as many times or as often as it needs to be.

**James**: I guess if we made an EFI information EIP and then I was an author on it, then pretty much I can write it? I don't know if that's the goal or not the goal? If I was an author on a Meta EIP that described the semi-official EFI process,how that all that works and I really  have like the capacity to do that all on my own, and I don't know if that it becomes a increase in decentralizing the the information part of the community.

**Hudson**: If it's a Meta, maybe, but this would be Informational. So it doesn't have to be followed but it's something to put down. In this case if you're writing it, you're the best person to write it as a hard Fork manager. I mean once we have it put in last call, anyone can come in and have objections and make changes and discuss with you but I just the reality is we can't we can't overly focus on the centralization and decentralization aspect because at the end of the day, if no one's going to argue with you no one's going to argue with you and so we don't need to be taking steps to put the for something in the process. We need to give every opportunity for people to do that but we don't need to like openly solicited hardcore.

**James**: Okay. Then once it is an 'active' status then I sort of been just update it.

**Hudson**: You would have to do a PR that would have to go through last call.

**James**: Okay, if you would want to specify something like that cuz currently, that wouldn't be that. I think, there isn't a way to do what you just said.

**Hudson**: Exactly there isn't a way spoken to upgrade active EIPs, not in EIP 1. This is going to get confusing wording, **there is not a way to upgrade active EIP such as EIP 1, so the way to upgrade EIP 1 to specifically set on precedence alone and not on a process that's recorded and the precedents for upgrading EIP 1 or other active EIPs of which EIP 1 is the only active EIP, is to do a pull request for that EIP and have a go to lastcall and have people agree on it**. I can make that in a rap :)

**James**: That was very well said and articulated. 

**Hudson**: Yay!!!!

**James**: There isn't a way to make a Pull Request be last call.

**Hudson**: Oh, there isn't?

**Edson**: On that, I actually, I created an EIP to document possible process for updating Active EIPs, I think about in December, I could [link](https://ethereum-magicians.org/t/eip-2458-add-updates-and-updated-by-eip-header-options-for-active-eips/4113) that below.

**Hudson**: Oh please do, yeah we can definitely use that.

**James**: And this actually goes into a piece of something I wanted to talk about today, so maybe we can go ahead.

**Hudson**: So Edson, you go ahead. 

**Edson**: The idea was, we already have a process for putting things into last call, so the Proposal was any change would be made inside an EIP, so any EIP didn't go through the EIP process and once it's accepted then that change can be put into the active EIPs referencing, that's  what's the simplified version of it.

**James**: I would argue for a simpler version. You're on the right track, but I'd do it just a little bit differently and this is something I've been wanting to talk about today.  So as far as editing active EIPs including EIP 1, getting public feedback and making sure any changes are known by the community which currently has been the last call, RSS feed, but I think it would be you I wanted to ask the group here, if we had some kind of communication channel, whether it be like a Twitter bot or an RSS feed for specifically changes to active EIPs that then has its own subscription list for last call for them, something like that.

**Hudson**: Why would it be only for Active EIPs?

**James**: If we made an EIP to change the EIP 1, every time, on everything,  I think that is way too much more overhead and there's a certain loyalty to process that happens among people that I've seen in the ETC community where they're arguing something but from without actually arguing the change itself but arguing the process of the change and then that just spiraled into its own weirdness. So I would buy changes to active EIPs and I like this including the EIP Centric model as an it as an Active EIP as part of that same group that those changes if I was to change the definition for what it means to be EFI I don't think I should make an EIP to make that edit but I do think that the community should be aware of that and be able to respond as of its kind of a last call thing.

**Hudson**: Yes so you don't need to make an EIP for that edit, you do need to make a pull request for that edit to upgrade that active EIP and that last call should go into some kind of Twitter bot or something like that's what you're proposing?

**James**: Yeah some Twitter bot or RSS feed. As of now, the only way to trigger the RSS feed is for the status of EIP to go into last call, which if I made a pull request that wasn't adding an EIP, it was editing one of these active EIPs,  it wouldn't have that. So then I can't trigger the RSS feed.

**Hudson**: No, you could, you just change the status from the last call and then it would go back to active after it's either confirmed or denied that the new changes are going in. That would still trigger the RSS feed and it wouldn't decouple any other last calls from active cuz that would complicate things, in my opinion.

**James**:  You  would have to accept the pull request to trigger the bot.

**Hudson**: Yeah, you'd have to accept the last call status, yes. 

**James**: So, I'd make a PR that would make it last call and then make a PR that makes edits on that ?

**Hudson**: That's how it works with the ERCs, currently, yes. However, the discussion all happens in magicians forums, hopefully.

**James**: I just want to make sure, I understand this part, I'd make a PR to EIP 1 that makes no changes but moves it to last call?

**Hudson**: No, so **how it works in the ERC**, which would be similar to act 2 an active EIP is, you have a PR that initially puts your data out there your EIP and it's in draft mode as long as it's well formed. Then you have a last call status, so it goes from draft to last call and then to final, and then from there I must have changing a spelling error it's it's superseded after that if you want to superceed it. So that's how an ERC would work for an active EIP, it's actually less steps because the first step for making it at all is to make it a draft and then active or no draft last call and then active and if you want to do changes to it, you would do last call if it's approved and then active again.

**James**: But you couldn't trigger the last call without it being approved, without merging the EIP.

**Hudson**: Yeah, you'd merge it with the header file, just saying last call instead of active. So then EIP would be reflected as a last call status which is helpful for people visiting that EIP out of the blue, to say oh this is changing soon or not changing.

**James**: For that you would only within the changes. So then I would need to have a PR that changes at the last call but doesn't have the contents of the change? 

**Hudson**: Yes.

James**: But then having a PR that has contents of the change ?

**James**: Yes, exactly. The PR with the content of the change would be the one that goes to active again.

**James**: Okay that's a little kind of confusing.

**Hudson**: Yeah we should make it with number one we should make a graph for the current process and number two we should change it maybe. 

**James**: I like the idea of a Twitter bot or something. It makes sense this has it's own process and its own subscription feed.

**Hudson**: Cool we spent way too much time on this we should time box :) I don't know  if there's anything else on that. We need to take a lot of that off-line or in the telegram. 

### 3. Update on proposed changes to EIP 1

**Hudson**:  So we only have a few minutes left but Update on proposed changes to EIP 1. I think we can skip that because we've been going over that off and on today and we'll need to recollect our thoughts and go through the notes and kind of you know list them out before we talk about them again.

### 4. Survey on the [EIP process](https://forms.gle/WCPRoLKUnmA5YaBL6) (target audience - core devs)

**Hudson**: Survey on the EIP process, that is oh we already have a form, cool!  We made this before, I remember this now. Has anyone replied to that or are we not send it out , I forgot where we are on that?

**Edson**: So we haven't sent it out yet. I think, Tim posted in the Cat Herders newsletter.

**Pooja**: Yeah we did add it in the biweekly newsletter this week, but since it is with you, so I've no visibility of if we received any response to that or not.

**Edson**: There hasn't actually been a response yet. But I'll [link](https://docs.google.com/forms/d/e/1FAIpQLSeadXscoQgrKznUOAEB_jSzNNFKHWDEFJxKH1LpDsDsC6mXpw/viewform?usp=sf_link) the latest form, if it's final okay, we start sending it out. 

**Tim**: I like the latest form, I like how simple it is. I would say that at the very top we need to talk about the EIPIP process and say this is where you can go for more info and it's happening right now because as many opportunities as we can take to say join us we need to do that because otherwise there's going to be this just implicit just stigma around, oh you did this without the community and all this other stuff, that can very easily happen if we don't push this everywhere.

**Edson**: All right, sounds good. I think that links don't show up in the description.

**Hudson**: You can put the URL, that's real short. 

**Pooja**: Would it be a good idea to share that in ALl Core Devs call, because that is watched by most of the people in Ethereum and most of the developers are there. So we can share with them and ask them to give their feedback?

**Hudson**: Yeah, we can do that.

**Edson**: Sounds good. Any other final comments on the form?

**Hudson**: I like how simple it is.  We might do follow-up forms with people leaving their contact information. If we need more specifics, I should say, we might not.

**Edson**: Sounds good.

### 5. Review action items from [EIPIP meeting 5](https://github.com/BrentAllsop/EIPIP/blob/3535e41826792234244d0ba912ad2acde4720681/All%20EIPIP%20Meetings/Meeting%20005.md) 

**Hudson**: Review the action items from EIPIP meeting 5. I forgot where the action items are. Are they at the bottom or was it just..

**Pooja**: No actually it was supposed to be here only in the Summary section, but in the last meeting we discussed about two major topics that was one migration of EIP content that we actually covered and the second was the motivation. So, I don't think we do have much action item over there, from the last meeting.

**Hudson**: Okay, will have some for this time. So, you're taking notes, so just put as the Action Items, if we've any left off from previous EIP meeting, would you add those please?

**Pooja**: Of course, I'll do that.


### 6. Any Other Business


**Hudson**: Okay, any other final business ?

**Brent**: Yes, if we got a sec just one question for Sam Richards. Thanks for putting together that, what was it a notion.so, summary of your proposal, that whole conversation and it was nice to see that summary. I noticed, somewhere you're asking for comments, if I want to say that I am for this, can I add that as a comment somewhere? is there anything like that?

**Sam**: Yeah so you should have the ability in the notion document to essentially like if you highlight any piece of text you should be able to input a comment.

**Brent**: Oh that's how we do that.

**Sam**: Let me know if you have an issue. I know the tool fatigue, another new documentation tool. I personally like notion but again happy to change the format and it sounds like once we do have a more firm, like how to implementation strategy, we do plan to open it up a as a GitHub issue in the EIP repo and that should be like a friendly and familiar place for people that add input.

**Breant**: Cool, thanks! Yeah yeah and just a plug for Canonizar here, if you want us to help because if if you put something like this in Canonizer that everyone who supports that could like it's like a petition that people can sign it. And there's also a place for people with different point of view can create a competing camp and sign that so you keep track of that what they want and what's required to get them on board, and track when they jump camp and get on board and all that kind of stuff. But, anyway, I'll shut up now, thanks. 

**Sam**: I'll check that out. 

### 7. Next Call

**Hudson**: Sounds good and I think it's been some color changes on here. That's about it. Thanks everyone will me meet in 2 weeks.

**Date for Next Meeting**: Wednesday, April 08, 2020 at 1500 UTC.
	
# Attendees

* Anett Rolikova
* Brent Allsop
* Edson Ayllon
* Hudson Jameson
* James Hancock
* Louis Guthmann
* Pooja Ranjan
* Sam Richards
* Tim Beiko
* William Schwab


### Zoom Chat

Agenda: https://github.com/ethereum-cat-herders/EIPIP/issues/10 

Proposal: https://www.notion.so/Migrate-EIP-content-to-ethereum-org-b50f198d8c254e2eb89790658e9079a8

William: Couldn't we just modify the existing subdomain? I'm not sure why we need a new domain specifically; if we just put in the work on the existing eips.ethereum.org subdomain, what wouldn't work?

William: In other words, subdomains have a harder time in SEO?

Edson: Do you have the link to that Meta EIP?

Edson: Add updates and updated-by EIP Header Options for active EIPs: https://ethereum-magicians.org/t/eip-2458-add-updates-and-updated-by-eip-header-options-for-active-eips/4113

https://docs.google.com/forms/d/e/1FAIpQLSeadXscoQgrKznUOAEB_jSzNNFKHWDEFJxKH1LpDsDsC6mXpw/viewform?usp=sf_link 


