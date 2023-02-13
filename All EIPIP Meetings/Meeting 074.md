# EIPIP Meeting 74 Notes
### Meeting Date/Time: Feb 08, 2023 at 16:00 UTC
### Meeting Duration: 1:11:02
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/210)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=JyQw6ZWuZkY)
### Moderator: Pooja Ranjan
### Notes: Metago

## Summary

Summary | Description
-|-
74.1 | [CI: Upgrade EIP-Bot to eip-review-bot ethereum/EIPs#5508](https://github.com/ethereum/EIPs/pull/5508). Editors approve merge of eip review bot.  
74.2 | [New contract interface and EIPs should be required to include a privacy considerations section ethereum/EIPs#5682](https://github.com/ethereum/EIPs/issues/5682). Participants have divided opinions. Discussion can continue in the issue section to garner more feedback. It may be added to next meeting's agenda.  
74.3 | [Separate EIPs and ERCs repo - A proposal](https://ethereum-magicians.org/t/proposal-forking-ercs-from-eips-repository/12804) CL team will be asked to add EIP editors and the issue may be discussed again at the next meeting.
74.4 | [Adds @xinbenlv as an EIP Editor (#5502) ethereum/EIPs#5703](https://github.com/ethereum/EIPs/pull/5703). It will be posted in the pr that @xinbenlv is added as ERC editor after agreement from Sam. 

# Introduction [0:00](https://www.youtube.com/watch?v=JyQw6ZWuZkY)
**Pooja**
Welcome to EIPIP meeting 74. I have shared the agenda in chat. We have a few open issues and pull request as usual to be discussed on this call as well as we have another important topic which is EIP and ERC repo separation. There is a proposal that we will look into and will cover some of the discussion continued from earlier meetings. 

## [CI: Upgrade EIP-Bot to eip-review-bot ethereum/EIPs#5508](https://github.com/ethereum/EIPs/pull/5508) 
So let's get going. The first item listed here is a CI upgrade EIP bot to EIP review bot. I think it was suggested by Sam. Sam, if you would like to provide info and we can discuss this one first. 

**Sam**
This is Panda’s actually.

**Pandapip**
Yes, my, it's my PR. Sam is the one that suggested it for the meeting. So currently EIP bot has quite a few bugs and the code is not easy to maintain. In fact, I'm still not entirely sure where some of the stuff that needs to be fixed even is. I have tried multiple times to fix particularly the bug. That means that PRs that delete files can't be merged, multiple times unsuccessfully. So I really don't even know how to fix that one. I also, so what I did was I made a complete rewrite of the EIP bot. I think the only reason that it's not merged is concerns over if there's some oversight we made that allows PRs to be merged when they shouldn't be. So basically concerns about make like I have fully tested it, tested every part of it manually and have automated tests too. But there is still a chance that some things slip through and I think that's what's blocking it. At some point it would probably be useful to merge it and maybe try it for a, take a snapshot of the repository and force push it backwards if need be. But I really don't think that there's any bug. I have thoroughly tested it and there are automated tests. 

**Sam**
And as somebody who's refuted it does seem fairly understandable. Yeah.

**Pooja**
Matt and Victor, if you guys have any thoughts on merging this one? 

**Pandapip**
Well, I think we probably definitely want to at least probably have a local clone of it so that we can force push if the worst comes to worse and someone does find a way to absolutely break it. But I think it's almost certainly fine. 

**Lightclient**
I mean, it sounds like it's really ready to merge if there's test, you manually tested it and Sam is taking a look and it looks good.

**Sam**
All right, so consensus is to make the switch.

**Pandapip**
...inconsistent.

**Lightclient**
What is happening in your audio? 

**Sam**
Me? Damn. Yeah, sorry, it's a 3D printer. 

**Pandapip**
Cool.

**Pooja**
All right. So let's go ahead and merge that. Any of the editors may merge it during the call. It would be nice. Or we can do it after the call as well. 

## [New contract interface and EIPs should be required to include a privacy considerations section ethereum/EIPs#5682](https://github.com/ethereum/EIPs/issues/5682) [03:37](https://youtu.be/JyQw6ZWuZkY?t=217)

Moving on to the next one, which is an issue. I think it's a new contract interface and EIPIP should require to include a privacy consideration section. Anyone has thoughts on this? 

**Sam**
I don't think we need another section for it. I'm feel pretty strongly that if there are privacy considerations for an EIP, they should go in the security consideration section. 

**Pandapip**
I propose an alternative thing, which is that we rename the security consideration section to just considerations and allow subsections. Such as a mandatory security subsection and I guess we could also make it a mandatory privacy subsection. 

**Sam**
I just don't think that there are that many EIPs that require privacy. Like it's on a blockchain. 

**Pandapip**
I don't think there are that many EIPs that require security considerations. Either nonetheless, it still requires section. 

**Tim Bieko**
Core EIP should definitely have it. Even if it says there's a thing. 

**Pandapip**
Yeah, I think we should, the privacy considerations at the very least should be mandatory for core EIPs. 

**Tim Bieko**
Even if there are, oh, sorry, I meant security considerations not privacy. Core EIP should have security, even if…

**Pandapip**
Well, yeah, we'll just say there's that. The security considerations are mandatory now, right now for all the EIPs, regardless of type or category. 

**Pooja**
Are we clear on this part like why do we need privacy? I mean, I can understand it. That is something related to, specifically related to ERC, but again, we are talking about standards. So, do we need to have the privacy part like we are trying to make it open source, adaptable by everything? So as much as transparency, it can be. 

**Pandapip**
Yeah, I think it's primarily for like, as you said, transparency purposes. Like if something's going to like somehow need some information, just by the nature of whatever algorithm it uses, that should probably be the end user. It also makes, but as someone who has done application development, being able to know what, what affects the tools you depend on, create, allows for things like GDPR compliance to be a little bit easier. So that would be my rationale for why it would be a good idea to at the very least rename the security considerations to considerations. 

**Sam**
So my problem with having just considerations…is my audio any better? 

**Pandapip**
Your audio is great.

**Sam**
Okay, so it would just considerations is that people are going to try stuffing whatever the hell they want in there that isn't even related to security or privacy. They'll have like one monetary considerations and…

**Pandapip**
I think that's absolutely fine. If there are any considerations, they should be listed. In fact, there might even like for example, the…my EIP that's the Ethereum notary interface, that I'd like to put a legal consideration in there, if possible, but like that's just like not and there's no good place to put that. Sorry, Trains. 

**Victor**
How about we add a new other considerations and as optional so that if someone want to bring in privacy, they can bring in there and if the other things comes up, they can put it there and we can still keep security consideration separate and mandatory. 

**Pandapip**
I was thinking just subsections of the consideration section. So you have two second level considerations, third level privacy, third level security, third level on other. 

**Sam**
I don't think we're going to get very far talking about this on the call. Maybe we can make a thread on or I should discuss this in the issue. 

**Pandapip**
There is discussion on that proposal. That's in fact the proposal I put there.

**Pooja**
So to summarize, the proposal here is to have a renaming of the section security consideration and just consideration and there could be the different types of consideration depending upon the proposal. 

**Sam**
I am fairly against giving people more flexibility. I'd like to not have another considerations or just a vague consideration section. 

**Lightclient**
I'm also generally against, I do like the idea of people being more cognizant about how they are ERC and I'm saying ERC because I think that there's not many cases or EIPs come into play with respect to privacy, but I do think there are a lot of ERC protocols that should consider how their application deals with user information. 

**Pandapip**
The thing that prompted this was actually an interface EIP. So yes, there are in fact EIPs that would definitely deal with this. 

**Sam**
I just want to understand why privacy isn't security. Like, aren't they the same? Like, isn't privacy a subset of security? 

**Pandapip**
Yeah, that was actually me. But like, I definitely still believe in that, but the public perception of them is different. Right? Especially since there's a trade-off, like privacy and security, there is often times the trade-off there. And so I think it might be meaningful to distinguish that. 

**Pooja**
Okay, it definitely looks like we have divided opinion here on the call of the dependent participants. So maybe we can have more discussion going on in the issue section and we get more feedbacks there. Probably we'll bring it up to the next meeting. Does that sound reasonable? 

**Pandapip**
Sounds good.

**Pooja**
Awesome.

## [Separate EIPs and ERCs repo - A proposal](https://ethereum-magicians.org/t/proposal-forking-ercs-from-eips-repository/12804) [10:28](https://youtu.be/JyQw6ZWuZkY?t=628)

So we know that we have another topic for discussion today, and that is a proposal, a proposal to separate EIP and ERC repo. The proposal is proposed by Tim Beiko. We have him on the call. So Tim, if you would like to maybe provide a brief overview, so we can start this question on the top. 

**Tim Bieko**
Yeah, sure. Thank you for having me. Also, thank you for all of you. I think almost everyone on this call has replied on the thread. So I appreciate the engagement there. I guess it's probably worth starting from where this came from and then we can get to this specifics. But high level, the thing I like, the number one thing I've been focused on and sort of care about is figuring out how we get to a point where there's a single sort of pretty straightforward process to propose consensus changes to Ethereum. 

And by consensus, I mean, not just consensus layer, but just like a changes to the consensus rules of the protocol. And today, I think pretty much everyone here knows, which is for clarity, like on the execution side, we use this weird thing where we have a yellow paper that's now out of date. We have EIPs that act as like layers. We apply on top of the yellow paper. And this is more or less what we call our spec. And at least historically, that was the case. And then on the CL side, they have a Python spec where they just make PRs to analyze basically the actual spec of the network. 

On the technical side, yeah, we, I mean, Sam and his team, you spent a bunch of time over the past year getting an EL spec up to mainnet, which is great. So I think this gives us like a much better sort of technical base on which to like specify changes to Ethereum, especially in a post-merge context. And so we've, I think we've done like really good work rectifying that part of the process. But the bit that's still quite separate is that we basically use EIPs to specify changes on the execution layer. They don't do that on the consensus layer. 

And it would be nice that this would be the same thing. And a few reasons why this would be nice is like one, you can think of like the changes of the consensus layer now matter like much more given that like we've merged, you know, the beacon chain is live and it's all one system. 

And you know, you can take one very like strong an example, you could say, look, the consensus layer can literally just double issuance on the network, do this to like some random PR to the specs. And there's not really a great place where like it gets, it gets like documented in a way that's as easy for people to understand. As like EIP1234 is the place where the changes propose. The other bit that's quite hard is when you have changes that affect both layers. So we have two examples of this right now, like withdrawals and 4844. And both are like pretty awkward. So like withdrawals has like a HackMD that acts as a sort of meta spec. And then that basically points to the CL repo and the EL repo for the CLIP and the CL specs sort of the EIP to like describe the changes. 

4844 is this weird sort of EIP where the EL changes are describing the EIP and then the sort of references without linking the CL specs for the rest. So I think, you know, the ideal insight would be something like, you know, these core EIPs or these core changes get specified in like a common way and then can link out to their respective specs. And talking to client teams, I think people are, you know, generally on board with this vision. 

But one, I think the biggest challenge is how do we get people on the consensus layer side to want to interact with the EIP process to like specify their changes and kind of add this extra degree of like formality to their process, which they don't currently have. I think they're, you know, I spent a bunch of time talking to them. 

They fear that like the EIP process is pretty rigid and bureaucratic and that the sort of friction created from it won't be worth it, you know, and just sort of slows them down. And they would also like they feel like they can, like they don't, they aren't only the ones that have to comply with the EIP process, but maybe you know the EIP process and can kind of adapt to how they do things because, you know, they might do things better than we do as well. And so, you know, this is kind of a long intro, but the idea is like, I think the main problem I've been thinking about is how do we like create a process for specifying changes to the core consensus rules that is like very, I don't know, like enticing for people on the consensus layer to start contributing to and ideally that has like the lower friction than the fully EIP processes that exist today. 

And then, you know, the sort of second order effect from there is I think based on that, you can imagine core EIP starting to like evolve in a way that's different than the rest of the EIP process. And I think this is kind of where the idea of like splitting ERCs and EIPs came out of, where, you know, this would be a way to kind of signal like, look, these processes will diverge. This is like the first step in that divergence. And, you know, we can kind of then both take them, take them forward in different directions. 

I appreciate all the arguments that's, you know, like there's some high technical overhead to do that. So, I don't want to like, you know, incur all this work just for the sake of it. Like, I think it's sort of considering the, like those drawbacks as well. But I think, you know, the sort of meta proposal I have here is like, how do we include CL people and give them a way that's like much more flexible where like they can start to iterate on the process. Even if it doesn't meet, you know, whatever bar the current EIP process has, I think it's like, we're in a much better spot if we have like, full on quote, bad CLEIPs that like don't fit our templates don't, you know, work quite well than if we have the current status quo, which is nothing and like them being sort of scared to engage. 

So yeah, I'll pause here, but that's kind of all sort of like high level why I wanted to bring this up and then kind of the rationale behind it. 

**Pandapip**
Yeah. Here's my thought. First of all, we need more, we need more editors period. If that's all or some other system so that more PRs can get reviewed. Once that, once that's done, the EIP process will be a lot less bureaucratic. 

Secondly, I think that there's no reason why we can't have a, for example, my proposal to just automatically merge all the drafts. That would make it very easy to get started. I don't, I don't, and we could even possibly disable make the validator due warnings for draft EIPs instead of fall blocks. So that's my thought. And that I think would definitely help people get on board and not require splitting the repo, which it's easier for everything's in one place. 

**Sam**
So to echo Pooja's argument against auto-merging draft prs is that a lot of EIPs get abandoned in draft. So the only time editors interact with them is in the first PR and to pull into the repository. So I think that's probably the strongest argument against just automatically merging drafts. 

**Pandapip**
I don't get it. Why is that a downside? 

Because they'll be terrible. Yeah, I think if they're terrible, nobody uses them. If we serve terrible EIPs from our domain, then it looks bad on us. And I think there is, I hate to say, but I think there is some amount of like reputation that we want to maintain. We want to have a minimum bar of equality for what we publish. 

**Pandapip**
Okay, then we just lowered the stagnant threshold for draft EIPs and allow deleting them if they stagnate. 

**Pooja**
I mean, that is increasing our work. The first thing that we can do at the entry level is like make sure that we are adding only good proposals even in the draft status. There is nothing wrong in staying as long as they are not ready to be merged as draft considering that we have now so many channels open. We do arrange this biweekly meeting for EIP editing office hour. All authors are welcome to come and talk to us to move the proposal to make them better and then add it as a draft. If we start auto merging them, we are practically losing there's a space of giving this opportunity to learn. 

**Zainan Victor Zhou**
If I may chime in, I think Tim comes in and raise the problem that's because of EIP editing has, of too many frictions. They want to kind of propose a fork. And I can resonate a lot with that. I'm actually a big fan of reducing the frictions and respect adopters, including allowing much more linking to useful sources. What I feel that we were going into debate is about whether in micros area, whether we want to accept draft merging or not. 

That's a more practical but in a high level, do we want to have a forked version? I want to bring to the attention to this group also that there's nothing stopping EL and EL and CL, applying developers to continue just ignoring EIP fully, which is what they do. And out of respect for this program, Tim come to us and I believe that if we could think of how we can reduce the friction for them, that's the only way we can keep the core or other EIP type inside of EIP. 

I personally feel that I'm totally in support of having core EIP and maybe network EIP and even interface EIP have different rules and different layouts and different merging frictions by different people. What I felt reserved is to have different repository and different domain names to serve them, which has both technical problem as well as it creates confusion for people to understand where to go to look at Ethereum proposals. So what I propose to the team and the group is that we allow a group of core contributors to quickly become EIP editors and for them to make decision about their merging rule, their editing rules. In that way, we can keep this as in one single repository. Yeah, that would be my proposal in this. 

**Pandapip**
I agree with that. We could just fast track quite a few core developers into being core EIP editors. And actually, with the new EIP review box, it wouldn't be that hard to make it like a core only like no website changes. Like a slimmed down editor thing that only works for EIP and doesn't give general editor stuff. 

**Sam**
Before diving into solutions too much here, I want to understand a little bit more about what the problem is. So what is friction? What about our process is difficult for people to work with? 

**Pandapip**
I can answer that. It's the…we spend that it to a lot of people, it appears that we spend a lot of time on nitpicking stuff. And I can actually somewhat agree with that…that it's just that the reason why we spend so much time on nitpicking stuff is that we want all EIPs to look good, right? That goes back to the kind of the like, the like reputation like thing. But I think that we are actually a little bit too nitpicking with too nitpicking in some cases, particularly with draft EIPs that aren't even going to see the life of day. A lot of the time. But yeah, I think it's maybe time to over…it…that needs to be... 

**Tim Bieko**
So I think like I follow the process more closely than like the average consensus layer dev. And I do think it has improved quite a lot over the past, I don't know, sixish, maybe 12 months. I do think that those incremental improvements are perceived against like four years of basically stagnation from the CL teams. And I think this is why there's a bunch of small tweaks that cause friction. Like I mean, and whether this is like the syntax rules, whether this is, yeah, just I don't know, the templates or stuff like that. 

I mean, I think like the, for example, the SSEAP right now, you could imagine a world where like you just merged the first draft of that and then still kind of have the discussion about like, you know, the improvements after it. But I do think like talking with CL folks is like they just view this as like something that if they sign up for will like slow them down immensely and they might not be able to control. 

And they sort of add this dependency in their process that like they, I don't know, they're sort of fearful of to some extent. And something that like signals to them that like, you know, they'll be able to like use this process in a way that's like useful for them, even if it's not like completely following sort of current rules. I think that's the thing they would like to see. 

And whether this is, you know, spilling it out in a separate process in repo, I think that that sense that's it. No, I think the other option of like, yeah, adding some like, you know, potentially even just CLEIP editors or something that that can merge stuff, you know, like even if it's not, if it's not perfect, that might be good enough to get them to use it. 

And I think if we went down that route, you know, for example, like it would be worth looking then at like, okay, I don't know, over the past two months, like we sort of forced merge these four EIPs, you know, what like, what's like the check that they weren't passing? Like what is the thing we overrode in the bot? And that might be like the most useful way to understand like what's, what's like, what, what a friction comes from. 

But I do think like, you know, there's definitely like a quote unquote irrational fear from the CL side, the participate in this. That's based on just like the accumulated perception over a long time, rather than like having spent a ton of time sort of, yeah, actually engaging in the process. And I guess most people is just, you know, most people don't have a ton of time to engage in the EIP process. And yeah. 

**Pandapip**
Well, once you actually know what the processes and what the formatting and stuff is, then it's actually quite simple. But there is a, but there's definitely on…

**Lightclient**
I think beyond just this like question about being fearful of the process, there's also this problem that the process for getting, you know, core EIPs over the line and the process for doing ERCs are different. And we're spending a lot of time trying to come up with rules that work for both of these systems. And we are, you know, just coming up with something that sort of muddled in the middle. And I think that to me is the biggest argument why it used to be just separate. 

**Sam**
So what would you say is like…

**Lightclient**
…going for two totally different. 

**Sam**
Yeah, so what would you say is an example of something that's very different between EIP, like core EIPs and ERCs? 

**Lightclient**
I mean, core EIPs is a very specific small group of people that are actively working all the time to try and make these things happen. And we have very specific ideas about, you know, trying to come up with certain test cases, or writing security considerations on all these things. And for ERCs, it's like a completely wide open world, like anything is possible. We have people who are writing completely new protocols. We have people who are writing additions to protocols. Like we should be thinking a lot more about how can they make the process more amenable to what these types of things that they're doing. You know, we don't really have as much of this extension of EIPs, usually in core EIPs. But that's like super common thing for ERCs. All the time they want to add new things to the NFTs standards. 

And it's something that they just keep adding more and more ERCs rather than coming with a more appreciable top down approach about how can we just like continue moving the NFTs standard forward. And this is to me is just a problem because nobody is really engaged on that side. Because we don't want to, I mean, it's hard to have them engaged in this process because this is a very important process to core EIPs as well. And so we don't want to just let application developers come in and start defining tons and different like procedural things. 

And so I think if we make it separate, give them a room to experiment and try different things. Then they'll end up with a much better process to see their needs. We'll end up with a much better process to start needs. Because we'll be able to bring people in who are involved with the core process who don't have to ever look at any of these things. We are seeing something that often has these discussions about. You know, we want to make this change. I was just working for ERC, especially our specialists. 

**Tim Bieko**
Great. And I think then the question is like, I think there's two levels. So that one is like the technical coupling of the repos and two is like the quote-unquote management of it. So you can imagine in the world where like, you know, we keep it on one repot to like lower technical overhead. But then we, the process sort of evolve independently or what not. And I think there it's like, yeah, maybe you need like, you just need time and over time you see, yeah, over time you see the divergence maybe that leads to a split. 

I do think like even if you read the EIP 1 today, there are like all these awkward things around like, you know, core EIPs. And I think there's also this weird question with core EIPs that's different is like, how do they fit with the network upgrade process. And that's always been like a very sort of awkward thing. And potentially having a separate process there. Potentially having a separate process there helps like, converge to something that's like not only a specs process, but it's like a specs plus like statuses map the hard fork status or whatever process. 

**Lightclient**
Yeah, we're doing a huge total different…

**Zainan Victor Zhou**
I resonate. I resonate and recognize what team says that or you have already had a different treatment at least when it needs to move to final. And we just allow more diverging of the rules, but not forking the repository, allowing more editors from the core team to merge. 

**Lightclient**
What is the ultimate fork in the repository? 

**Pandapip**
Having everything in one place, having allowing a core by nobody, one core EIPs, one another. There's a lot of arguments for having…

**Lightclient**
When before the reference in ERC or vice versa?

**Pandapip**
Sorry?

**Lightclient**
When do core EIPs need to reference ERC? 

**Pandapip**
Well, say that something relies on an output being available such as say, good-like proxies rely on delegate call. 

**Zainan Victor Zhou**
Also chain ID proposed by 55 was being referenced in, I believe, ERCs 112 uh 712 to which is both, I personally perceive as both interface and ERCs. 

**Lightclient**
These are extremely simple things to resolve once they're split up. You can say requires that the EIP requires this fork of Ethereum. 

**Zainan Victor Zhou**
I think William and Trigen provide a good argument about not forking mainly because of the technical…the wholeness of the technical side. Like a stack, people can go to and then see everything together. It is definitely nothing preventing them. You can even break down core EIP into two different repositories for execution and consensus. But what we have right now, and 

**Lightclient**
…we're trying to unify these things. 

**Zainan Victor Zhou**
So why do you, the reason the rational arguing for unifying them is and be also leveraged to you to argue for unifying many of the other stacks? 

**Lightclient**
The people who are working on these core things, this is one specific group. But they're working on the EL, they care about what the CL is doing, if you want to CL, care what the EL is doing. This is like a known group of people. Whereas the application side like, this is also a known group of people. 

But if they're completely disjointed, there's almost no overlap in point of view of or building application stuff. There are very, very few people can follow two things about.

**Tim Bieko**
I do think there is a separation of concerns between what's built on Ethereum versus like the specification of the protocol. I think some, yeah. 

**Pandapip**
Doesn't the protocol just fails on itself? 

**Lightclient**
Absolutely not. Well, I mean protocol is it is it causally being moved forward with upgrades and adding features, but these are like, so it's being done with its application developers to use. But this is totally different. Right. So the applications are on the platform. 

**Pandapip**
And adding features on top of the platform to the platform, I don't see much difference at all. 

**Tim Bieko**
Well, there is because, for example, the most obvious feature is that a consensus change requires the entire network to adopt it or the network is going to fork. Right? And it has to be bug free, otherwise the network can try to bug. I think the sort of bar in terms of consensus building that we require for core EIPs is much, much higher than an ERC, which is an opt-in feature. 

And then I agree, I think Sam, you were the person at this point on Ethereum magicians, then this is like sort of a spectrum. Right. If imagine Core EIPs are on one side of it, ERCs are on the other side. Something like an interface EIP is kind of weird because maybe like, sure, not all the clients need to add E68, but then if they don't gossip these transactions the right way, it kind of messes up with the network. 

**Lightclient**
Well, I would say that I will not be in the networking, the DEP report, I shouldn't be in the EIP. I was in the EIP really any more. 

**Tim Bieko**
Right. But yeah, but I do. Yeah, so I think it's like there's two clear spots. There's like a standard for a new NFT royalty thing, which is opt-in, it has like, you know, there's no sort of, if I never know that it exists, I can use Ethereum and like my experience has not changed. But then there's something like, oh, we're going to double the issuance. And then it's like, wow, everybody who like has a say in like Ethereum should probably be aware of this thing. And this is where like I think Core EIPs are different. 

We're like, even when we add an upcode, it's like we're asking all the nodes to like update at the same time. And it's really valuable that like this information is like clear. And this is, I guess, that to my point, it's like the fact that we don't have this for the CL today, I see this as like a really terrible sort of failure of the process because, you know, you go to the CL specs, you see like a diff on the specs with like a couple comments, but it's really hard to make out like what are like each feature. 

So like, you know, this fork introduced one, two or three things. You don't have something like a security consideration section. You don't have something like a rationale. And I think it's just like the process is much less like legible than the EIP process. And like, yeah rectifying that is like basically the number one thing I care about. Like if we can get to a spot where when we have changes happen on the consensus layer, there's like a handful of EIPs we can point to that say, hey, you know, we've changed validator rewards. We've like updated the fork choice rule, you know, whatever else like added withdrawals. Like that's extremely valuable because then the community can review those changes, understand them, which is much harder to do today. 

**Pooja**
I think we are talking about maybe two different processes here. So when we are talking about separating repo, am I understanding is that we are trying to follow the same process that was followed that was being followed so far. And it's just that we are having two different fork for ERCs and EIPs. They both followed separately. 

But then we are trying to follow the process which is already being followed by the CL specs that are going to be a different process than the one that currently being followed at EIP. So if we happen to follow what CL is doing, then it's better to which I think…

**Zainan Victor Zhou**
The proposal was to have a fork and then the core EIPs doesn't follow any of the existing rule if I understand it correctly to reduce the pressure. 

**Pooja**
Yeah, that's exactly what I want to clarify. Like are we proposing that EIP will not be following anything that is being followed so far? We are trying to move towards the different process of the core proposal which was earlier execution specs for the EIP process. 

**Lightclient**
So proposing to split the EIPs and ERCs apart and then separately develop a process for both of them independently that's useful in the needs in a thus way. And part of that is like figuring out how to engage CL in the EIP process. 

**Pandapip**
Yeah, but I think I'm weakly opinionated on the order of those two things. Like if you know if you all think that like having the ability to like have CL folks sort of update the process of the core stuff as part of the EIP process as it exists is the right first step until you know potentially like there's enough friction that like separating the repos makes sense and maybe that never happens. 

Like I'm fine with that but I think like the yeah the most important thing is like how do we get CL people to feel like they can come and contribute and that is very low friction for them to do that. And regardless of the way you do it it's going to assume that like a sort of higher error bar or like a lower quality bar for CL stuff. And I think we should be very okay with that because our current style of school is that we don't have an error bar or an error rate or quality rate for like CL stuff because like they just don't have the EIPs right. So it's almost like we don't see them but yeah. Yeah. I think that's that's bad. Yeah. 

**Pandapip**
How about this compromise? We introduced a new type of EIP basically attract EIP and it's basically a redone, it's a different EIP one. It describes an entirely different process but everything's still on the same repo. So it can all in so track EIPs of different tracks can still interact with one another while still having different processes. 

**Tim Bieko**
I don't think we need a new EIP 1. This is sort of what I liked with forking the repos is like you know most of the stuff actually stays the same right like so I don't think you need a separate EIP 1. I think I don't know where the EIP rules are written or the EIP 1 are on like the homepage of the website. Okay but yeah so I think um yeah I guess and maybe I don't know the other way I would frame this is like I would rather lower the friction and then rebuild the process than to try and like proactively come up with the right process because I think that's sort of the thing that it's like if we add a bunch of new process rules to make this work then we don't know that they're right and this is sort of the other problem it's like if we can just you know try out a bunch of CLEIPs see how they differ and then sort of go from there I think that gives us a better like starting ground and say like oh we're going to try and think of the right way to accommodate them in a new process and then add a bunch more constraints around that. 

So I think yeah…

**Pandapip**
I'm thinking that an EIP one could be changed to a track EIP and then what you what we do it basically create a new EIP depends on EIP one and just says these conditions don't apply to these EIPs which would allow for a fast track. 

**Lightclient**
…

**Pandapip**
Sorry didn't catch that. 

**Lightclient**
I think you're just adding more than two different things that you can do to your homestoppers work it's like okay I want to make a change I usually make a core EIP oh wait the EIP 1, just to go look at the other EIPs so like if you're on the time you get to that you can make it and so it's okay. 

**Pandapip**
We just document it very clearly. 

**Lightclient**
Yeah I know how clearly documented I mean this is like their full time job they don't want to put in or reading about how to like make a change whenever they've been making changes for years a month. 

**Tim Bieko**
And I think this is yeah this is kind of back to what I was saying earlier is like to me if we had you know someone who can like force merge CLEIPs you know these people are not stupid either right, like they do care about their work they do generally like do high quality stuff so it's like you start by force merging their stuff in, even though it breaks the rules then you sort of retroactively look at, like okay what's like what rules did it break how did this thing differ, you know and you can even imagine a world where like aside from asking for a title with like a number that you know they don't need anything else right, like maybe they don't even use the same section, it's maybe they don't use that and then it's like, maybe you like, over time sure you build the separate EIP 1 that documents this but I think your odds of like success are much better if you start from allowing them to use it as they would want to use it and from there you know potentially enshrining some things or maybe you know after six months you tell them you know you guys never put in a security consideration sections that's really bad we're gonna force you to start doing it but at that point they're already sort of like engaged enough that they can maybe understand like the value of this. 

**Sam**
Yeah well then maybe the path forward is we you know find somebody from the consensus teams this is for the hardest part that wants to be an EIP editor, we tell them you know you can force merge and override whatever you want for CLEIPs, that way they get exposure to the process. Oh no it's got to be, it's got to be one of them directly it's got to be a CL developer because they need to learn the process and that's it. We don't change the process at all, because I don't think, like it's just a perception of frustration right? 

Like the reason why it takes so long is because like for ERCs at least we have myself and Panda that do it right, like that's and it's 90% Panda, so like for core EIPs we have like Matt and Greg and everybody and they go through a lot faster there's a hell of a lot less friction than there is for ERCs, so if they added develop like if they add a core EIP editor they can go as fast as they want, they won't be blocked on anything because they can just approve their own EIPs and they can force merge if they want…

**Pandapip**
They can approve their own EIPs.

**Sam**
Sure but I'm talking about like as a group 

**Pandapip**
Okay.

**Tim Bieko**
So like anybody in that…?...write the EIP…yeah yeah yeah okay sure. 

**Sam**
So hell we can add two but it doesn't matter right it like yeah and they'll only get notifications about core EIPs maybe a few random ones but it's really not that bad as long as you're not on the ERC track and that way they control exactly how much friction there is 

**Lightclient**
And I think some app devs are like what the heck is they get to just merge their EIPs without doing this and I have to go all the day all the time…

**Pandapip**
We would be willing to accept that. 

**Sam**
Yeah, so they can double that. 

**Lightclient**
I don't want to have to deal with like the angry app devs like I want to put them in their own box and let them flourish in their own realm…

**Pandapip**
Just pin the blame on me. 

**Sam**
EIPW is not that bad 

**?**
yeah I agree with that I would like to stop that as our cannot if we contain…

**Pooja**
I would like to share an example of consensus layer a proposal which was considered to be a standing in the process for way too long that was for proposal for it to be moved to the review status so Sam had this discussion in the call we had yesterday the EIP editing office hour there was dependency on one proposal to another so they wanted to have like EIP 68 to be a part of required section if they allow people to just keep on force merging and do not follow any process then it may end up creating chaos so the simple thing was there to have EIP 68 in review and to get EIP 68 in review we needed to have EIP 67 in review so I talked to Marius, we created a pull request and it was solved so I think it is a simple process that we are following here…

**Tim Bieko**
I wanted I think this is exactly the type of thing that you want to like shield CL people from as they start.

**Pooja**
Like right so for shielding them we have group we have process and we have people like Marius did not have to come and make the pull request, I did it for him so when we know what is the problem we are here to help them out. Sam explicitly mentioned in the comment that what we need is to move this into review and proto made a PR to make it into review process so it's not that it is dependent on anybody it's just that awareness that is lacking in the CL team and it's the comfort that we have to provide them that if you're following the right thing and if you're even if you don't know what is the right thing we are here to help you out so let us know what challenges you are facing and we are here to help you out move it smoothly.

**?**
But you're sure yeah I think you want that to be developed for the people 

**Tim Bieko**
…don't think it's the right thing they'll be like it's just stupid why should I like why is this rule there like I just want my spec and I sympathize with like you know the reason why the process is there but I think if you start by like forcing them to follow and like sort of wade through this like this labyrinth of like exceptions and networking EIPs I think are like every time I don't know for some reason they're sort of and that being the worst ones 

**Lightclient**
…but like I mean I think part of it is that the guest team absolutely EIP process and refuse to engage with it and so as the people who are making the network EIPs they make the draft just to get the number and tell the people to implement it and then they don't have to do anything else with it. 

**Sam**
Yeah right so I think interface EIPs 

**Pandapip**
…and as you've seen I've actually gone ahead and tried tried to get the ball rolling on a few of those interface EIPs…

**Pooja**
Sam, you were saying something I think we missed you. 

**Sam**
Yeah sorry I just it completely slipped out of my mind. 

**Tim Bieko**
But maybe okay so Sam, I think the your like your previous proposal was like okay we add a couple we add a couple CL folks as EIP editors for core they can force merge stuff it's important that they're actually CL people and not just like random people because this acts as a way to pull them into the process. Does that generally make sense because there's a CL call tomorrow I think it would be reason you know if people here agree with that then we can just go on a CL call tomorrow and ask if one or two people want to be sort of tributes for this and kind of go from there?

I think the thing is like yeah they need to have force merge access for core EIPs and feel that like you know they can sort of own that part of the process and then through social means we can hopefully align them with the rest of the process but technically they should have sort of free reign on that small section. 

**Pandapip**
I don't know how to do that 

**Tim Bieko**
Okay, so I'm happy to go on the CL call tomorrow and share that and I can come back I mean you're obviously I welcome on the CL call as well but yeah I can go and let them know and we can go from there.

**Pooja**
Yeah and just to add like getting access is not a big challenge here we just want to make sure that people having access are really responsible I mean I don't mean to say that EIP editors are not responsible we just want to make a few bullet points to be covered over there and getting that… should not be a problem and we are happy to provide all the support to just go through the basics of it and yeah it would be great to have more people in.

**Tim Bieko**
And I think one thing also that like we can in terms of being responsible maybe one soft requirement we can do is we can tell them look you can for force merge stuff but like try and keep that for CL things right? so like you know because I don't think we should add a separation in core EIPs but like I think it's fine to say that like you know EVM changes like shouldn't be forced merged by some CL dev who just is best off at the EIP process like technically they would be able to do that but to tell them like you know please refrain from that and use this as a way to help CL folks onboard I think that's a reasonable ask. 

**Pandapip**
Speaking of editors can we make a Zainan one? 

**Sam**
Okay wait before we jump topics here I have something else to throw in just a heads up that the merge to EIP 1 that makes ERCs use ERC dashes to prefix and everything else use EIP dashes of prefix was merged so I'm in the process of updating EIPW, be ready for a lot of very angry people being very confused.

**Pooja**
I was the one who 

**Lightclient**
…was talking about what it now yeah 

**Pooja**
I was the one I think was the one biggest fan of referring them as EIP considering there was no ERC written in the repository but now that it is actually reflecting ERC 20 I think I will pull myself from that, being a roadblocker there, 

**Pandapip**
But yeah are there any objections to Zainian being editor?

**Lightclient**
Honestly we haven't finished talking about the topic.

**Pandapip**
Sorry

**Lightclient**
It it's great that we decided that we can get some CL editors on and I don't think it's going to be an endorsement of CL stuff but I still want to get ERCs out of this repository. I don't think it's the right place for them and I really haven't heard any compelling arguments that they should be in here.

**Pandapip**
Well I think that the purpose of the EIP's repository is literally any standard relating to Ethereum I think that is the scope of it. Quite frankly I don't think that the special rules for core EIPs make sense like, having it make it having it turn to final only when it's merged into the quote unquote canonical Ethereum, that doesn't make sense to me right? Because the standard is final long before that. I think the status of the standard should be planned. 

**Lightclient**
…there's been a rubber band but I think that is just super contract 
…like core EIPs the whole goal and we're focused on Ethereum we don't care about other chains I don't really care if I have a way to make some EIP to update their EVM and we're only going to move in Ethereum so going forward and so we're very much tied to the hardcore schedule of Ethereum. 

**Pandapip**
Yeah but nonetheless I don't think that the EIP's repository should be the place to make government governance decisions I think that the proposal should all be final even competing ones and then the best one is selected to be part of the meta. 

**Lightclient**
I mean I think this is I think it is just like not understanding the process very well because there's no way that we can make something final before it reaches the testnet, if we make it final before it reaches the test net and we realize that there's like a small thing and it's been changed in the last moment we have to go create a whole new EIP and that's a great a huge you know cause and confusion about what is the actual thing that's going in and so like we have to leave it at last call until we actually start forking test net and probably before forking mainnet. 

**Pandapip**
Yeah and that would be the risk of moving it to final before the testnet is made but nonetheless I don't think it needs to be the EIP editors’s responsibility or anything related to the EIP process’s responsibility to care about what has or has not been implemented where.

**Lightclient**
I'm not really saying that's what's all really what I'm asking for I'm trying to say that I think that the proposal for EIP and the EIPs are different and that they should be completely separate.

Yes the original scope of the EIP repository was to define all of the standards related to Ethereum but that was done in 2016 and over the years we realized that things that are happening on application layer are very different than the things that are happening at the core layer and so I'm saying that the scope should be changed at this point.

**Pandapip**
What changes would you propose would be made…what divergences would you like to see in the processes?

**Lightclient**
I mean it's not really up for me to say like I think the process that we have right now is been mostly dictated by the needs of the core protocol with some occasional input from what application developers want in a process and so it's not really my place to say how the application developers should modify their process to support their workflows. I think the process that we have right now is reasonable for doing core protocol changes but it's not very good for the application developers and how do I know it's not very good for the application developers? because they don't even follow the process you just walked watch this big permits to contract a few months ago and they just didn't go through the editing process at all they were like why would we do that like let's just ship it and this is like the risk they were having because people don't want to do this process it doesn't work very well for them. 

**Pandapip**
Well then we just fix it and like oh 

**Lightclient**
We can't fix everyone we don't work at Uniswap 

**Pandapip**
If everyone is camplaining about the same thing both ELCL and application devs then that suggests that there's something wrong that should be fixed everywhere and not by forking.

**Lightclient**
But there's just all people from different perspectives like we need to let the people with those perspectives come then and play a role and find an area of the changes, we can't just like sit here at the top of this pyramid and ask for feedback and then make all of the changes top down. I'm not involved in absolutely high level applications developers…

**Tim Bieko**
Right they might not they might not be the same disagreements.

**Pandapip**
Yeah well then why don't they just make a PR modifying EIP 1? I mean that's entire point of like that that we get to almost like crowdsource the process.

**Lightclient**
I mean I know they should be more involved with the process. I don't disagree like I am frustrated they're not more involved with the process but I think the right way to get involved with the process is to sandbox this process away from the core process and let them be the captains of that thing, let them have ownership and responsibility over the full end process, if we add them and involve them in this process I agree we have to I just 

**Pandapip**
I agree with letting the core people do the core stuff and not having to care about the ERC stuff nonetheless I think that they should still remain one repository.

**Lightclient**
At this point was like it's just a pointless semantic and I'm saying that I've like had a lot of quite a bit of feedback about it's too much noise for people to just follow this repository because it's pushing grab bag of different things that are happening…

**Zainan Victor Zhou**
I think what Tim has proposed in two steps, the first step is inviting the CL team core to become editors and see if they can still fit in…

**Lightclient**
This is separate and this is separate than the CL editors is we're separating the ERCs and the EIP repository we already said that we'll add the CL people as editors and they'll have forced merge abilities, I'm saying that we need to get ERCs out of this process as well and let the app developers take the reign and really you know manifests the process that they want to have.

**Pandapip**
I still I still think that this should be done without separating them

**Lightclient**
I think they can be have different why like what is the argument for not separating…

**Pandapip**
Again so that they can interact with one another so that…

**Lightclient**
They're not there's no need to interact with that one another you can go with time that you need to interact as if you're just saying this relies on this core change and I don't think like core ever needs to interact back to ERC like there there would be no point. 

I would not accept the EIP a core EIP that refers to an ERC.

**Zainan Victor Zhou**
I think Greg has some strong opinion on this shall we wait for him to come on and have a say on this? We already make some good progress in compromising and we can also see how he plays out.

**Lightclient**
He should be here and I'm sure we'll talk about this many more times but let's keep going on for a couple more minutes.

**Pooja**
Right and we are almost out of time for like to have this discussion continued maybe we can bring it back in the next meeting, for today is from what we got as a conclusion that maybe on the tomorrow's CL site CL meeting will try to look talk to CL Dev and see if they are interested to be a part of the process and maybe if Matt if you would like we can bring it back again to hear your arguments of having it separated 

**Lightclient**
though I feel like when this is going on for three years and I just want to make it happen and I don't think that there are any compelling reasons to keep these things together other than this idea of unity and I'm saying that there is no need for this thing of unity because they are actually not a singular, like it designs things anymore we are very well aware that these are two totally different areas of development and we should respect that by getting in their own places to define their processes. 

**Pooja**
Right as much as I agree but I think that you know this thing coming from more from the ERC authors that I don't want to be a part of EIP repository we want to be having a separate repository than core or EIP repository would make more sense to me but so far I think we have not received any negative feedback in terms of complaints like ERC authors. 

**Lightclient**
Why would they have negative feedback? They don't care, they don’t have to go through this process but they do have issues they don't use the process so they just don't use it and then they go on with their lives and they launch their projects and their standards and they just say you should use it because we're Uniswap you should use it because we're open seas. 

**Pooja**
Right I would I would tell maybe slightly it's for here because I have seen in according to EIP’s Insight, I have seen them more of ERC proposal more as final so they are definitely moving ahead they are definitely following the process and limitation. 

But how many of these ERCs are coming from like top tier teams things like openseas or Uniswap the people who should be the most involved with where this base is going in terms of creating standards. 

**Sam**
Unfortunately unless it's required for inter-op you're not going to see people writing standards like I don't understand why you just want whatever want to write a standard for anything they may do. 

**Lightclient**
Well I mean if you look into Permit 2. Perman 2 is totally something that should be a standard like Perman 2 is this idea that you have this single 10 per miscontract where you give an allowance like a max allowance to and then Uniswap is able to across all of their different token pairs rather than even the allowance of that token pair contract across all the token pair contracts it can basically do some sort of like authorization via this global permit contract. And they don't have this. 

**Sam**
Why do they need a standard or does it only work for Uniswap? 

**Lightclient**
Well it doesn't work for anybody but the point of having a standard is that this is like an interface that anybody can interoperate with. 

**Sam**
Yeah but no like the contract is there the interface is published so it's done there is no standard required you just use the contract like a regular contract right?

**Pandapip**
Except I think you would absolutely be worth it to be for it to be a standard take EIP1820 which is basically that the exact same thing except with except basically EIP it's basically EIP165 on steroids and with the registry contract instead of each contract implementing a function. 

**Lightclient**
If you're less about having the artifact of the standard interface being defined and more about the process of getting set artifact I think was missed on Permit 2 other projects 

**Sam**
But what I'm saying or they aren't building something that warrants a standard there aren't going to be…

?

**Lightclient**
But everybody should use this permit contract and so in the interest of doing things in like an open way that is amenable to everybody's needs it would have been a lot better you know it's not like an open thing what do you think about this permit 2 contract is this something that you're going to be able to use too, because if everybody implement their own permit 2 contract then the gain is not that large 

**Sam**
No for sure but for private for-profit companies

**Lightclient**
I agree I agree like if they don't standardize 

**Pandapip**
Except Google for example Google has tons of standards with the IETF like they do have an invested interest in interoperability there's no difference here. 

**Lightclient**
There's nothing I would do to force the private companies to have these types of standards other than the social pressure and I think it's like really important that we try and have the social pressure that people are building standards for things that can be you do a lot of many different people that they have to build it in the open.

**Pandapip**
I agree with you here and I do agree that we should make the process easier but I don't think we should do it by splitting the repo. 

**Pooja**
I'm sorry to like interrupt here we must have to wrap up now, we are like beyond the time we can definitely bring it back in the next meeting. I just want to make one small point before we when I'm like what we are doing here is helping people to build a standard. We cannot force people to come and build a standard with us so it is totally up to people who want to contribute who want to help other people out what we can ensure 

**Pandapip**
By making the process easier and that's 

**Pooja**
Yeah but what we can do is just by making the process easier so we can rather focus on what are the challenges, what are the friction that people are feeling here and try to resolve that. 

I think this would be a good point to maybe wrap up and have if people would like we can have it to discuss in the next meeting anyway we have to see the result that is coming up from the CL team or more EIP editors if they are willing to join. Any final comment thoughts anybody would like to add before we just close for today?

## [Adds @xinbenlv as an EIP Editor (#5502) ethereum/EIPs#5703](https://github.com/ethereum/EIPs/pull/5703)[01:06:22](https://youtu.be/JyQw6ZWuZkY?t=3982)

**Zainan Victor Zhou**
Yeah just want to quickly check if what the temperature check for adding me as an editor. 

**Lightclient**
I think Lightclient was the only objection?

**Lightclient**
I mean I haven't really seen a whole lot of editing in the last month and a half? frankly 

**Zainan Victor Zhou**
I can I can find a help I think 

**Pandapip**
I think he is more I think he is more than capable as an editor and I think that's primarily because right now his suggested edits have basically no weight because he's not an editor yet. 

**Lightclient**
Now ultimately I think that we need to be bringing people into the process who are involved with client teams and that's like my main focus, I think if you wanted to come on in an ERC editor then that would be great but I am like worried about adding more people to have the power of controlling what the like standardization processes for core EIPs who aren't involved with the core process at all. 

**Zainan Victor Zhou**
I'm okay yeah…totally okay serving as ERC editor.

**Pooja**
And then to begin with we're going to start like a like a really difficult yeah please go ahead.

**Lightclient**
Now we have this really difficult problem know where it's like and this is why I want to separate these repositories because how do we like have this conversation about changing the process and I am saying like I don't feel super comfortable about adding more people who have the ability to change the EIP core process who aren’t invovled with these client teams and so what like you're just supposed both to not participate when we start talking about changing the core process? like this is a very confusing way and we haven't had an editor added in this manner before. 

**Zainan Victor Zhou**
Yeah I'm in favor of letting CL and EL and core devs to make the whole decision about the core EIP editing rules I can refrain from participating at all. Yeah that's totally okay and then I actually don't have a strong opinion there.

**Lightclient**
The EICY this makes much more sense if these are two separate things where we don't even have to have this it's like oh we're not talking about core standard change Victor is not going to participate in this specific discussion blah blah blah. We already have different editors right? In our bot metadata? they know…

**Lightclient**
I'm talking about any types of meetings I'm I we have great tooling for dealing with this on the PR level I'm talking about at this meeting level when we start talking about you know we want to have this change like Mickey what if we want to change the statuses or something for core EIP that a new status like about to go in a hardcore right like having these discussions I'm saying that I don't want to be adding more editors into these conversations who don't have contacts about what is actually like feeling the process as a client and owner.

**Zainan Victor Zhou**
Yeah I can totally reframe from commenting on the core EIP process as an as an ERC editor for sure. Yeah I totally understand that you need more contacts on that side to comment on that. Would that resolve your concern?

**Lightclient**
Yeah I mean this is this resolves my concern on at front I still think that this is like a muddy situation of having the ERC and EIP together to meet is a very clear reason to have them separate but we're not going to resolve that for a while so I'm happy to move forward with this agreement.

**Zainan Victor Zhou**
Sounds good. Thank you.

**Pooja**
All right I'm not sure like Sam has already dropped off so do we have a consensus here? we're like what are we trying to conclude out of this?

**Lightclient**
If I were to summarize yeah I would just post it on the PR and make sure that Sam acts in agreement 

**Pooja**
Okay that makes sense 

**Zainan Victor Zhou**
Thanks Matt

**Lightclient**
Absolutely.

**Pooja**
All right thank you guys. Thank you for joining us today I hope to see you in two weeks have a good one everyone.

## Attendees

* Pooja Ranjan
* Pandapip
* Sam
* Tim Bieko
* Zainan Victor Zhou(@xinbenlv)
* Lightclient 
* JA
