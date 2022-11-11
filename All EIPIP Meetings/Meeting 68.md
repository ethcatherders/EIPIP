# EIPIP Meeting 68 Notes
### Meeting Date/Time: Wednesday, Nov 02, 2022, at 15:00 UTC
### Meeting Duration: 1:01:03 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/187)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=-UDyjJy1ULg)
### Moderator: Pooja Ranjan
### Notes: Metago

----

# ACTION ITEM

1. Sam is going to remove the EIP per origin section in EIP 5757, and it'll just be a pr into EIP 1. The EIP editors will figure out a way to specify free links for DOI objects and Sam will remove the non-redistribution requirement. 

2. The EIP editors will revisit the issue in the next EIPIP meeting, and continue discussions on ECH Discord and Ethereum Discord. 
# AGENDA


## 1. Discussion: 
### a. Process Issues that haven't reached consensus:
#### External link policy, perennial external references, ACD Discord, Victor's proposal, Sam's proposal, Create an EIP External Link Archive ethereum/EIPs#5408, Allow external links when archived link provided  ethereum/EIPs#5733, Add EIP-5757: Propose process for allowing external links ethereum/EIPs#5757

**Pooja**
Welcome to EIPIP meeting 68. I have shared agenda in the chat. Today we have a small number of agenda items but I think the discussion is going to be relatively bigger. So the biggest point of discussion today here is external link policy. So I have tried collecting all the related documents, proposals, issues, and pull requests here in agenda. I see a discussion started by Greg on Cat Herder’s Discord about perennial external references. Later on there are some questions by Sam Wilson on ACD Discord. There are two Hackmd, one by Victor one by Sam for some general solution and also issues and pull requests here. 

So I know Sam you have tried to summarize that and put it into a question format. If you would like to give a high level overview of the dispute like people we are not having consensus on what kind of external link policy should be there and then we can start probably discussing from there. 

**Sam** [01:14](https://youtu.be/-UDyjJy1ULg?t=74)
Sure so I guess I put up EIP 5757 which I'm just now realizing is a pretty big number, sorry about that but yeah so it kind of contains a framework for doing external sources and some of the requirements in that EIP are a little contentious, the first one being like no paid research, like no linking to things behind a paywall, and Greg is of a mind that if the EIP depends on a paid resource then we have no choice but to link to it and myself Matt and Panda I think are all an agreement that we do not want any paid resources to be linkable. That's probably the most contentious item. I think there's a few other questions around like wording and like particular details but I haven't heard any criticisms of like the overall process. So yeah the questions you were talking about are, I asked in the All Core Dev Discord were specifically about whether all core devs would pay to access resources and a few questions about like the durability and immutability of linked sources so like whether or not you can link to a blog post or a Twitter post or a Reddit post and whether an archive.org link of the same is also acceptable. So we're just trying to figure some stuff out like that but I think the details are all in 5757 if anybody wants to read it.

**Pooja** [03:03](https://youtu.be/-UDyjJy1ULg?t=184)
Nice summary, thank you. I see that only we have received one response from Matt. So Matt if you would like to share that here?

**Lightclient** [03:14](https://youtu.be/-UDyjJy1ULg?t=193)
Against the ? content for each I think basically everybody is except for Greg. 

**Pooja** [03:27](https://youtu.be/-UDyjJy1ULg?t=205)
Okay so if I get this correct most of the people are against the paid content. Is that correct? So oh good thing we are having Greg on the call, welcome Greg. Greg can you hear us?

**Greg** 
Yeah Im here

**Pooja**
Morning Greg, so we were discussing the first item that is the external link policy, based on the questions those are shared on all core dev discord by Sam Wilson we were discussing about thoughts it looks like there is some disagreement with that if you would like to share it with us here?

**Greg** [04:07](https://youtu.be/-UDyjJy1ULg?t=247)
Yeah. Well I noticed I'm late because over on all core devs, the topic just exploded. 

**Sam**
Yeah, I know, I posted in advance of the call and during the call people started talking about it.  

**Greg**
I'm again mostly thinking we're making hard policy in advance of choices we don't need to make yet, but there's, obviously you go for the highest quality source you can find and when you get down to normative stuff you, at some point you have to reference what you have to reference. 

**Lightclient** [05:05](https://youtu.be/-UDyjJy1ULg?t=299)
I don't know if people are against referencing like a published piece, I'm just against like it being like a requirement for understanding like I think that we should like you know kind of rewrite the portion that is a requirement for even a specification and say this was first derived in this work and cite it.

**Greg** [05:28](https://youtu.be/-UDyjJy1ULg?t=319)
You want to write the proofs of how EOS works?

**Lightclient**
I don't think that we need to write the proofs I think we've already accepted the EOS works.

**Sam** [05:33](https://youtu.be/-UDyjJy1ULg?t=333)
Well if we were to generalize that to let's say a new crypto algorithm like do you need the proofs of how that crypto algorithm works in an EIP and I would say the answer is no because you don't need to know how it works to implement it but that's just my opinion.

**Greg** [05:52](https://youtu.be/-UDyjJy1ULg?t=346)
But you need you need a reference for the reader to find out how does this work, it if you're trying to implement something you need references to how to implement everything.

**Lightclient** [06:06](https://youtu.be/-UDyjJy1ULg?t=359)
The specifications should describe how to implement it in my opinion, fully and if that requires...

**Greg**
...possible. If you I mean that just goes layer by layer all the way down to the hardware. At some point you draw a line and say go look here or you just refer to the term and assume that the reader can figure it out. Sometimes that's what you do.

**Lightclient** [06:32](https://youtu.be/-UDyjJy1ULg?t=389)
But right and we've generally like set that boundary at cryptography and I think that that's okay.

**Greg**
Yeah I don't know why we're trying to be bigger hard asses than any other standards organization that I've dealt with. 

**Lightclient** [06:41](https://youtu.be/-UDyjJy1ULg?t=401)
I'm really not trying to be I mean this is an incredibly painful process for me too. 

**Greg**
Well we're making it painful it's just a reference is a reference and occasionally they rocked and it's not it's not like the end of the world.

**Lightclient**
I agree.

**Pooja** [07:07](https://youtu.be/-UDyjJy1ULg?t=425)
Greg what do you think about referencing these additional resources in the Fellowship of Ethereum Magician page? I feel like we definitely need to set a boundary what can go into the specification in EIP and what can be left out for any educational resources that are currently not allowed and we think that it is not directly related to Specs maybe it is only for references purposes can we not have it on FEM thread sharing, these are the additional resources to follow along? 

**Greg** [07:45](https://youtu.be/-UDyjJy1ULg?t=455)
All right I guess I'm just not seeing why this became such a big problem. The IETF has been dealing with this for many years and I suggest their policy is a good place to start. We can keep bringing up examples of bad lengths and for the most part they should simply not be should not be needed. 

**Lightclient** [08:07](https://youtu.be/-UDyjJy1ULg?t=479)
I mean I think that the IETF is has a bit of a different angle because it tends to have a lot more of an academic footprint and so there's a lot of citations that are academic journals that maybe do cost money if you're not part of that community and I don't think like for crypto most people have access to that stuff, there's like free ways of accessing it and yeah not super against like linking to academic pieces because it's pretty much commonly accepted, is okay.

**Greg** [08:48](https://youtu.be/-UDyjJy1ULg?t=524)
Well things a reference is a reference. They actually consider links to be optional but what's needed is a reference you know the author of the title enough information to find it.

**Lightclient**
Right but all of the references most the references in the IETF RFCs are to quote unquote published documents which are retrievable via those mechanisms and we link to a lot of things that are like URL native. I think our general policy should be linked first and that includes you know references to academic pieces. 

**Sam** [09:25](https://youtu.be/-UDyjJy1ULg?t=559)
So to be clear in 5757 it doesn't specify whether it's a URL or like an APA or whatever citation, it's anything that refers to an external document is a link it's just to clear up the terminology there.

**Greg**
Yeah I'm suggesting we have a reference section as the most straightforward way to do it, is there's a reference section and anything external there's a citation, and the citation gives the information someone needs to find this thing. So…

**Sam** [10:05](https://youtu.be/-UDyjJy1ULg?t=601)
I agree with that entirely...

**Greg**
I don't whatever and as far as links sometimes there is no link, usually there's one or more links and they should be the highest quality you can find. So the Journal of publication is a good link even though it's locked up, it's the Publisher's link so it's a place to start if there's a DOI identifier that's a good link the author the author of the editor the reviewer someone could do a little work to try to find high quality links that aren't paywalled and last resort whoever's implementing it has to get the information somehow but you've given them a big leg up on finding the information and if it's information that's necessary to implement it that seems to be a much bigger favor to the author than concentrating on whether a link might go dead in the future that if it goes dead in the future it can be fixed in the future.

**Sam** [11:20](https://youtu.be/-UDyjJy1ULg?t=673)
So I mean I it's kind of a crazy counter example , would you be all right if I started to replace like any core EIP I write, is going to be a link to my website in the specification section where they have to pay me a hundred dollars to read it, would that be an acceptable way of publishing EIPs?

**Greg** [11:39](https://youtu.be/-UDyjJy1ULg?t=697)
It would certainly be a very low quality link and I'd be looking for isn't there a better way to do this and if it's your own website you would have the rights to it and wouldn't we say let's put that in the assets? 

**Sam**
Sure sure I'm just saying like as an EIP author I can refuse to do that and force people to pay to access it.

**Greg** [12:05](https://youtu.be/-UDyjJy1ULg?t=720)
But these are decisions we can make when the EIPs in front of us rather than trying to make a policy to cover all possible futures.

**Lightclient**
Okay I think we just need to be using more common sense.

**Greg** [12:22](https://youtu.be/-UDyjJy1ULg?t=739)
Yeah it's just not that hard it's easy to come up with obviously counter encounter examples but mostly authors aren't going to do silly things like that. 

**Sam**
Uh I'm not sure about that but yeah I don't know I think like I really don't think there's much of a problem with having like a list of places that we allow like I don't know why like why there's a lot of opposition to that particular idea. 

**Greg** [12:49](https://youtu.be/-UDyjJy1ULg?t=768)
A few of them um yeah it can become a long list. 

**Sam**
It can be checked automatically though right like that's the point.

**Greg** [12:58](https://youtu.be/-UDyjJy1ULg?t=773)
I may have misread but I've checked to making the author go through the work of making their Source beyond that list just because we've said that's a cool link for this article doesn't mean this is a cool source for all possible links you know it could be as a last resort this is the source we use for this link we don't recommend it in general it really is I could see a small list of things that just are obviously fine and after that it gets case by case and the academic literature is hard because so much of it is paywalled that's that's just an unfortunate fact there's a story that when Reagan came in one of his people in charge of PubMed I think the NIH director was going to insist that anything listed on PubMed would have to have a publicly accessible copy online to be listed and uh that guy got fired so this is the world we're stuck with but...

**Pooja** [14:16](https://youtu.be/-UDyjJy1ULg?t=856)
So Greg I would like to share a couple of thoughts from my end here I am I don't know how much it is relevant in terms of IETF standard and for Ethereum I understand that it could be a good practice to follow something that is coming from a reputable organization but I believe that with Ethereum we are not only trying to create this educational resources and other things but why we are trying to make it a policy instead of case by case is something that we want to standardize the process for like being watchful for future proposals that are coming in.

**Sam** [14:56](https://youtu.be/-UDyjJy1ULg?t=889)
So we don't have to argue against every single EIP author that they're like linked to a tweet is not good enough. I want to avoid the situation where we get into arguments with authors every single time and we don't have a clear policy that we can just point to and say like this is how we approve links, follow this process because like otherwise we're going to get into so many arguments with people and we see it all the time already and it's like once we automated the process with EIPW, a lot of those arguments just went away and it's a lot easier now, so I'm on the fence of automating as much as possible and having a clear policy for external links I think. 

**Greg** [15:38](https://youtu.be/-UDyjJy1ULg?t=935)
I don't have a big problem there.

**Pooja**
Yeah I think in in fact what we should try here is like have a standard agreement from all EIP editors or I can say them like most of the people being in favor of any decision either to go this way or that way but that should be as a policy that we people who are trying to help out other authors we are not EIP editors but trying to let them know where to go and find what to do next. We will be like having some documentation or some reference to cite to people and I believe that will help us like a lot of discussion in future and this EIPIP meeting is especially for streamlining the process so if we can come upon any agreement on what is the best middle ground from where we can let other EIP authors know that beyond this line you are not allowed to put anything into the proposal, that means into the dot MD file of that EIP, you are very welcome to have it on Fellowship of Ethereum magician and people can go and refer it over there.

**Greg** [16:45](https://youtu.be/-UDyjJy1ULg?t=1004)
How stable a link is that really?

**Pooja**
No here in this case like we are not taking guarantee of a stability of the link whatever is there in Fellowship of Ethereum magician but what we are providing them is the discussion tool link which is added in EIP and we are sharing that this is a place where you can go and add your thoughts, so when we are providing a platform that can be relevant and that cannot be relevant after a few period of time but that is not a part of a standard right?

**Greg** [17:24](https://youtu.be/-UDyjJy1ULg?t=1044)
Yeah well that's what the discussions to link is for in the header.

**Pooja**
Yeah right so that's what I'm suggesting here let's start making use of that link and only where we think is directly related to Specs should be put into the dot MD file any additional information or the link which may or may not have paid like money involved there or copyrights involved there should be a part of like you know the discussion to thread not the part of the dot MD file.

**Greg** [18:00](https://youtu.be/-UDyjJy1ULg?t=1074)
Yeah but I think I've been clear enough here and I'm not it's not important enough to me to dig down into the details of these but…

**Pooja**
So considering that I mean I would like to understand how people think about the 5757 proposal like is it something good that can be moved forward we can have it merged because I don't see that is merged in repository yet so yeah any thoughts on that one or probably people who have objections yeah? 

**Victor Zhou** [18:41](https://youtu.be/-UDyjJy1ULg?t=1122)
I need to open up the link is that the one that Sam Wilson is having to add external link policy?

**Pooja**
That's right I have shared it in the chat.

**Victor Zhou**
I think my feedback would be first of all it's I appreciate that effort I think I want the general concept I agree with but I think we need to make it easier to add source shall be necessary to add something in a list and also I object to the requirement for a source to be create access two of the main asset and we should also have a broader extension for example like Ethereum projects should be like it shouldn't be very hard for Ethereum projects to be linked especially it should be easier for yellow paper to be linked I think it's a little bit kind of surprise to people that they can even not link to the consensus spec or the yellow paper. 

**Sam** [19:58](https://youtu.be/-UDyjJy1ULg?t=1195)
Yeah yeah I think those so if we go ahead with like a trial run of 5757 I can put up a like EIPs to do like the execution specs, consensus specs, the yellow paper, and I can take care of all those.

**Victor Zhou** [20:13](https://youtu.be/-UDyjJy1ULg?t=1207)
I don't like to have a requirement for a new EIP in order to add a source.

**Sam**
Yeah so I wanted to say yeah I'm a little torn about that too. I think my the reason why I specified that originally is because then each EIP gets its own discussions to thread and I think that's somewhat useful.

**Victor Zhou** [20:43](https://youtu.be/-UDyjJy1ULg?t=1234)
…And people to have a discussion we can have a centralized discussion for all the list of you know extensions…

**Sam**
Right yeah yeah but like then if a source comes up again like we can't…sorry you're cutting out a little bit…I thought you were done talking… sorry to cut you off there but so like if the source comes up again and we have the discussion on Discord then it's very difficult to point somebody at the existing discussion and be like here we've already talked about it so we'll end up having the same discussions over and over again so that that's my concern with not having an EIP per source. 

**Victor Zhou** [21:24](https://youtu.be/-UDyjJy1ULg?t=1282)
Yeah the EIP itself has a full workflow from to last call to final and if the only thing you want is…I think I'm okay to make that as a requirement and have…let's say two weeks of wait time I think I can…if that is like I can make that kind of trade-off. I don't think the full four-step shall be required and I don't know if that is a good thing to add to the process.

**Pooja** [22:11](https://youtu.be/-UDyjJy1ULg?t=1326)
I think the general idea of having the meta EIP is to define the process that we would like to follow so if we are defining a process of acceptance of external resources meta EIP sounds reasonable for this.

**Victor Zhou** [22:20](https://youtu.be/-UDyjJy1ULg?t=1340)
The thing is that no matter he takes too long I'd rather have one EIP being alive rather than have if it requires like it doesn't have to be an EIP either we can we can add something to the EIP 1 if you want or anything like require a high bar for it to be merged in but I think asking it to be a formal EIP can take too long for people if they want to contribute and add things. Yeah in general I think the allow listed approach is too restrictive even if you want 5751 is going into run I really hope that we can restrict the timelines let's say just run it for us in three months but it's only in effect for three months or six months and then see how it goes rather than...

**Sam** [23:16](https://youtu.be/-UDyjJy1ULg?t=1391)
I'm so down with that...

**Victor Zhou**
With unlimited time you're okay with...

**Sam**
Yeah yeah if you guys want to try like 5757 for three months, I am totally on board with that and then we can revisit it and like see how well it worked. I'm totally okay with that kind of a plan.

**Lightclient** [23:35](https://youtu.be/-UDyjJy1ULg?t=1411)
I mean aren't we just trying everything? we're always trying things like but I don't know I mean nothing is set in stone that is the proposal…

**Pooja**
That is true.

**Victor Zhou**
…is what I'm proposing is that trial but by default if there's no additional approval in three months, it just loses its effect. 

**Lightclient** [24:01](https://youtu.be/-UDyjJy1ULg?t=1434)
I just don't want to debate this again in three months I want to make a decision I wanted to fix this problem we've been talking about it for like six months or more.

**Sam** [24:08](https://youtu.be/-UDyjJy1ULg?t=1446)
I think I think it's a year now at least…So I'm firmly in the camp of still no external links like I like that way easier and simpler but because it comes up so much I I'm willing to you know meet in the middle a little bit and have some kind of external links.

**Lightclient**
I mean we always have external links. 

**Victor Zhou** [24:27](https://youtu.be/-UDyjJy1ULg?t=1467)
Sorry, oh yeah go ahead, sorry, I started to cut you off go ahead like you're fine.

**Lightclient**
I'm done.

**Victor Zhou** [24:41](https://youtu.be/-UDyjJy1ULg?t=1479)
Yeah, I'm so like in in favor of well external link, I feel that we lose our ability to make…it's a implement proposal right, it's you're trying to articulate and convince people to do something and you need to let people put them into context and the fact is that a lot of contexts needs to come in the format of link or otherwise we will need to have a full Wikipedia on the…that's what I the assets being put on to the repository it just get bigger and bigger and it's still a thing…okay they're…

**Lightclient** [25:26](https://youtu.be/-UDyjJy1ULg?t=1526)
You are cutting out a lot it's hard to understand what you're saying…what is blocking us from moving forward with 5757 at this point.

**Victor Zhou** 
Prohibiting free non-free access non-free access content and EIP dot requiring an EIP to add new sources what I would be happy with to move forward… 

**Lightclient** [26:11](https://youtu.be/-UDyjJy1ULg?t=1565)
So practically how do we link to academic journal articles I mean I think that BLS is a good example you know insert new cryptography we don't want to write the proofs and EIP we should link to it, how do we do it?

**Greg** [26:16](https://youtu.be/-UDyjJy1ULg?t=1576)
We just do it what what's so hard about this?

**Lightclient** 
I'm asking you how to do it in the 5757 framework. 

**Sam** [26:25](https://youtu.be/-UDyjJy1ULg?t=1585)
Oh sure, so in the 5757 framework you'd pick say DOI right so say you want to link to it as a DOI so we'd have an EIP that defines the format of a DOI reference so it'd probably have like title, authors, the DOI number, the publication date, and that would be just like a blob of markdown that you copy and paste into your EIP and then fill it out and then that's it that's how you reference an academic paper in 5757.

**Lightclient** [27:03](https://youtu.be/-UDyjJy1ULg?t=1622)
Who assigns the DOI? 

**Sam**
The DOI.

**Lightclient**
Okay I mean this is great like can we just merge it this seems like it resolves our problems. 

**Victor Zhou** [27:19](https://youtu.be/-UDyjJy1ULg?t=1641)
One question I have with Sam is that I linked I actually put down some of the trend deployed contract on Goerli as a reference the I wonder if what it would play out in 5757 with the situation.

**Sam** [27:32](https://youtu.be/-UDyjJy1ULg?t=1652)
So I don't know like etherscan probably wouldn't be a valid external source like maybe like I don't know maybe you guys would disagree but I don't think etherscan is, so linking to a reference implementation would just be linking to the byte code on the chain so I don't know how useful that would be, but like sure I mean you can make a 5757 source for linking to an Ethereum address if you want and then you could link to it, I don't really care as long as we all agree that that's a valid source. We can add it…like 5757 doesn't make any statements about what sources are allowed, it just says these are the things that have to be met and then we can argue about any individual source on the discussions thread or sorry I've renamed them origins now because source was confusing so you can…you can argue about any individual origin of documents on the discussion to thread. 

**Greg** [28:32](https://youtu.be/-UDyjJy1ULg?t=1712)
I guess I'm just not really understanding this then are you saying that in order for an author to get an origin approved, they have to submit a separate EIP for the approval of that origin?

**Sam**
So yeah so for each, so like Pandapip is calling them like categories, I call them origins. Right now I still haven't settled on a term that everybody understands but like DOI like the digital object identifier mix system would be one origin and then anything that has a DOI number would be from the same EIP like the same so like 5757 would have one EIP that defines all DOI identifiers and then anybody who wants to use a document described by DOI would just use that one EIP, they don't need a separate EIP for every document they want to reference. 

**Greg** [29:25](https://youtu.be/-UDyjJy1ULg?t=1765)
Now I'm really confused. 

**Sam** [29:28](https://youtu.be/-UDyjJy1ULg?t=1768)
Hang on I have I sent Panda a message that kind of explains this. Let me see if I can find it, here we go…

**Victor Zhou** 
I'm also confused.

**Sam** [29:36](https://youtu.be/-UDyjJy1ULg?t=1776)
Okay here let me let me just read you this it's not too bad, so we have an author let's call her Alice right and she wants to link to the w3c.org media capture streams specification right I think we can all agree that that is a specification that we want to allow people to link to, so Alice includes this in her EIP EIPW sees the external Link and complaints it says this is not an improved external Source you can't link to it so Allison reads 5757 and sees oh okay I need to open an EIP allowing w3c links. So she creates EIP X whatever the number happens to be it doesn't matter and she describes like w3c has existed for 10 years, w3c has like a history of providing documents, we can't include w3c specifications because they're not licensed appropriately for whatever reason doesn't matter and she creates this proposal then editors look at this proposal and they say okay yeah we like w3c we'll approve it as a source now. Alice can use her link to Media capture streams in her EIP that's it. Now Bob comes along and he wants to use say the geolocation API the w3c specifies he includes the link, EIPW sees the link and because Alice already made the proposal allowing w3c links now Bob can link to the geolocation API without any other like extra work, it's just approved.

**Greg** [31:05](https://youtu.be/-UDyjJy1ULg?t=1865)
Okay I'm objecting to putting that load of work onto Alice, she's already doing the work of writing her proposal. That's a lot of work and just because in that example that's probably a good source but the hard cases come down to the source just isn't a very good source and we have to decide in that case okay we can't find better sources so we'll use it like I'd say in general links into authors home pages at universities aren't the best links because they retire and they change universities and those links go away but often it's the best free link you have so it makes sense to give more than one link, here's the here's the link to the publisher I'm sorry it's paywalled, here's a DOI the DOI organization maintains where that goes to it's a good resource, here's a link to the author's copy yeah it might go away but it's free, if it goes away in the future that's an errata that can be fixed and you just the point is to give the reader access to information not to maintain the purity of our repository.

**Lightclient** [32:34](https://youtu.be/-UDyjJy1ULg?t=1954)
I mean do you have an alternative proposal, because what you're describing is how things were previously done on the repository and it doesn't seem like people want to do it that way anymore, so I think if we want to do something other than 5757 we need a different proposal than what we were previously doing. 

**Greg** [32:51](https://youtu.be/-UDyjJy1ULg?t=1971)
Well I'm I wasn't paying attention for a while and so I don't know where the no external links policy came from, it didn't used to be there. 

**Lightclient** [33:02](https://youtu.be/-UDyjJy1ULg?t=1982)
Micah is the one who like really instantiated it but I think like you know Sam and Panda are generally against external links and if we want to move to a place where we can allow external links we have to you know negotiate amongst ourselves and compromise and to me 5757 is a compromise that's not perfect but it is going to resolve many of the issues that we're having and I think we should do it.

**Greg** [33:31](https://youtu.be/-UDyjJy1ULg?t=2011)
Does EIP-1 currently forbid them?

**Lightclient**
It doesn't

**Greg**
Okay. I'm happy to have I'm happy I think we should have a reference section very much along the lines what the ITF recommends and I think the general policy laid out here is fine things like 10 years since Dutch we're just being too specific, I see the point of the editors maintaining a list of sources that we don't even have to think about. If you're using these sources um no problem um and then it does come down to judgment calls.

**Lightclient** [34:15](https://youtu.be/-UDyjJy1ULg?t=2055)
The point of the 5757 is the compromise of we're not going to make the judgment calls per EIP we're going to make the judgment calls per source and if you want to…

**Greg**
That's what doesn't work yeah...

**Lightclient**
But this is the compromise that we're trying to make like what you're proposing is how things were previously done and many of the editors are against it I'm like personally not against it like I think common sense makes sense to me and I would be happy to do it but I've been trying to make that happen for over one year and it hasn't and the only like reasonable solution that's like really been worked out is 5757, and so I would like to move forward with it.

**Sam** [34:53](https://youtu.be/-UDyjJy1ULg?t=2093)
Okay and I'm okay revisiting this in three months like we can just be like did it work?

**Lightclient**
We're gonna revisit it every single meeting.

**Sam**
Okay let's have a moratorium on revisiting it for a little while and then we can come back to it and see if we're happy with it because you know maybe I'm wrong maybe you know this is a horrible process and everybody hates it and it just hurts everybody and I'm totally okay with scrapping it after we give it a trial run so…

**Greg** [35:22](https://youtu.be/-UDyjJy1ULg?t=2122)
My only big objection is putting the author through the work of creating yet another EIP and you know having all these EIPs that don't do anything but say we approve this source yeah because I don't want to approve sources in general just because for particular EIP we decided that this particular low quality link was the best that we could do, it doesn't mean that we're blessing that source for all time, we're just saying in this case this particular low quality length was the best we could do…

**Sam** [36:01](https://youtu.be/-UDyjJy1ULg?t=2161)
I'm giving the wording we have now which is that it says should not and not must not so you know if it still gives us the freedom on a case-by-case basis to approve a link.

**Greg**
So then I have to start really digging in because I'm not quite sure what obviously allow means because I'm not a lawyer that's been a problem with the assets all along, some things are obviously recopyeable and other things you know who's gonna judge there, yeah as soon as you move the assets, you pulled them out of their original context so that's a hard call.

**Sam** [36:42](https://youtu.be/-UDyjJy1ULg?t=2202)
So you're objecting to the like the redistribution like first requirement?

**Greg**
I was just saying who's who's to say you gotta you step into a quagmire right away.

**Sam** [36:58](https://youtu.be/-UDyjJy1ULg?t=2218)
Well I mean I think obviously redistributable is things like RFCs which say the distribution of this memo is unlimited, like some things are very clear-cut allowed to be redistributed.

**Greg**
Right that's where you need a bot that's where you need a policy or a clear judgment that says yes we can put this in assets because then we're acting as a publisher and we have to respect the copyright of what we're publishing it's that's a hassle but there it is.

**Sam** [37:29](https://youtu.be/-UDyjJy1ULg?t=2249)
Okay so if we remove the requirement for redistrict the redistribution requirement would you be okay with 5757?

**Greg** [37:39](https://youtu.be/-UDyjJy1ULg?t=2259)
Yeah I just don't know quite how to state the requirement.

**Sam**
Well that's fine we could just take it out for now and then figure it out I don't mind doing that.

**Victor Zhou** [37:56](https://youtu.be/-UDyjJy1ULg?t=2276)
...the EIPs right...

**Lightclient**
the author doesnt have to submit the EIPs. The editors can do it anybody can do it.

**Victor Zhou** [38:13](https://youtu.be/-UDyjJy1ULg?t=2293)
Okay but is but that's a long process right?

**Lightclient**
...long process...it doesn't I mean it's really only three to five links that I think were like coming up all the time that I mean once we get the ability to link to the consensus specs to DOIs to RFCs I think like most of the problems go away.

**Victor Zhou** [38:31](https://youtu.be/-UDyjJy1ULg?t=2311)
What about Go ETH? what about Ethereum…

**Lightclient**
We shouldn't link to Geth. 

**Victor Zhou** [38:38](https://youtu.be/-UDyjJy1ULg?t=2318)
We shouldn’t link to Geth? why is that when people point that hey this is a working implementation then and wouldn't that be a better version than a reference code that has not been code tested?

**Lightclient** [38:50](https://youtu.be/-UDyjJy1ULg?t=2330)
No we need to be moving to using the execution spec.

**Victor Zhou**
But you can add it as a rapid implementation right? And people have that incline in inclination to add various implementation links there and also it's a stronger argument saying hey these three clients have already implemented…

**Lightclient** [39:10](https://youtu.be/-UDyjJy1ULg?t=2350)
I just don't think that's something that should really be existing in the EIP we can revisit like modifying the EIP template I think these are generally things that should exist in The Magician's thread like here's implementations.

**Victor Zhou** [39:28](https://youtu.be/-UDyjJy1ULg?t=2368)
Okay so you don't you don't think that needs to be at as a as a source.

**Sam**
I don't think we can allow go ethereum as a reference implementation because it is GBL right?

**Lightclient** [39:40](https://youtu.be/-UDyjJy1ULg?t=2380)
I mean traditionally we've like had the list of like here are implementations and people can just like click the link to them…

**Sam**
Yeah but we have the execution specs now so I think…

**Lightclient**
Yeah exactly we should stop doing that.

**Victor Zhou** [40:00](https://youtu.be/-UDyjJy1ULg?t=2400)
What about…?

**Lightclient**
...

**Victor Zhou**
Let's say let's say some of the storage has claim of backward compatibility arguments and that this is because we make this decision kind of compiler has this behavior and that's why we need to be careful of this security consideration or anything. 

**Lightclient** [40:25](https://youtu.be/-UDyjJy1ULg?t=2425)
Is there's a reason to link to something like we can open EIP to add it as a permissible origin…

**Sam**
Like I really don't see there being more than like 10 of these things at the extreme, like how many times like we've gotten by over the past year without external links so I think we can get by allowing some external links without too much trouble. 

**Victor Zhou** [40:52](https://youtu.be/-UDyjJy1ULg?t=2452)
Well if you like force people to not link to things like you have two choice either they would they cannot submit an EIP which is happening or that is it's that becomes segment or they would just remove links and reduce the quality of their articulations that's what's happening too in like web to provide object provider like I don't mean 

**Lightclient** [41:17](https://youtu.be/-UDyjJy1ULg?t=2477)
We generally shouldn't allow everyone to submit an EIP like there needs to be some rigor for what is accepted and I think that having a link policy that is a bit restrictive keeps the quality of the EIPs a bit higher like just letting someone willy-nilly link to Twitter to blog posts and stuff I think creates poor quality use.

**Sam** [41:37](https://youtu.be/-UDyjJy1ULg?t=2497)
So as a great example of that the merge EIP was just awful it had links to like tweets and random blog posts by Vitalik and like at least three of the links were dead and it's just like we need to not do that right like we aren't a normal standards organization because like there are no restrictions on who can publish EIPs so we need to have like a streamlined process for keeping the quality up and that's kind of my argument for 5757

**Greg** [42:10](https://youtu.be/-UDyjJy1ULg?t=2530)
Now we needed to do a lot better job of editing that.

**Victor Zhou**
Yeah that would be my argument like right we can make suggestions say hey they're not like stable they're social media they're not part of the standard that what I agree like the hard cases are for example like GO Eth, like apparently I think always should be and also other client implementation should be allowed to be linked and then you you it's a no-brainer and they should not be…

**Lightclient** [42:41](https://youtu.be/-UDyjJy1ULg?t=2561)
I just don't think this is really related to 175757 like we should debate this at another time but like I honestly don't want to leave this call again without making a decision.

**Victor Zhou** [42:53](https://youtu.be/-UDyjJy1ULg?t=2573)
I think it's uh I think it's an example as that like we are accepting five seven sites like that with the sconces of default and I'm what I'm referring to is if we accept 577 then default is not accepting bill is unless it's approved but I'm looking I'm more inclined to have another version that is more open default is allowed unless it is being spread down like in those cases in those middle grounds I like to be more open I'm I'm using it as an example not to say it's relevant directly but indirectly it is what they thought will play out… 

**Lightclient** [43:28](https://youtu.be/-UDyjJy1ULg?t=2608)
I think we've already seen like the editors are against that we don't want to like curate a list of like non-acceptable sources that's a lot more work than a small list of acceptable sources.

**Pooja**
Yeah I would agree I think the idea of having 5757 is I mean from where I'm seeing is to make it difficult for people to have like external resources added to the EIP, we generally speaking we are not, the group doesn't seem to be in favor of having allowed all the external links so if external link has to be there, there should be certain processes in place and this sounds like a good one I'm in good middle ground from at least we can give it a try for next three months…

**Greg** [44:14](https://youtu.be/-UDyjJy1ULg?t=2654)
Now and as it's written it's not acceptable make… 

**Lightclient**
Which part do you not accept?

**Greg**
There's two aspects to it, what I really don't like is forcing the author to make a separate EIP to allow for a source.

**Lightclient** [44:34](https://youtu.be/-UDyjJy1ULg?t=2674)
You're not forcing the author anybody can make it.

**Greg**
Right but I don't want them, it's just clutter it makes sense for the editors the editors to maintain a small list of sources in the EIP 1 that just says these are acceptable sources don't worry about it.

**Lightclient** [44:53](https://youtu.be/-UDyjJy1ULg?t=2693)
You will also have a list in EIP 1.

**Victor Zhou**
So and so like Ryan I think when you say everyone anyone can make the petition in reality is that the author is being blocked from submitting those links into their EIP and they either have to do it themselves or they have to submit it yeah right that's the reality if we say hey any editor is striking down our games to make one then we can copy saying that that doesn't add the two editors for an alternative work but we don't we all know that's not gonna happen so I think Greg made a valid point this is a hurdle and this will end up in practice making authors submit those EIP or have to give up the links and remove the little things. 

**Lightclient** [45:46](https://youtu.be/-UDyjJy1ULg?t=2746)
That is the point of this EIP it is supposed to be restrictive it is not supposed to be trivial to add links to EIPs. I honestly don't care whether or not it's an EIP or if it's an update to EIP 1 I think it's better than they are EIPs because if we rely on just making a PRT one then we're like further increasing our Reliance on like this GitHub infrastructure and it's not easy for us to like have the history or like the rationale if we're adding things and making decisions, like I get it we already use GitHub for a lot of things in this case I think it's good if we can have this as like a separate artifact, but if this is like the thing that stopping 5757 from happening and I think we should just remove the  concept of having source or origin EIPs and just say you have to open a PR to equal one to change it and we can discuss on the pr thread.

**Greg** [46:41](https://youtu.be/-UDyjJy1ULg?t=2801)
I'm in favor.

**Victor Zhou**
That's better.

**Sam** [46:43](https://youtu.be/-UDyjJy1ULg?t=2803)
All right, I'll make that change.

**Lightclient**
All right what else is blocking 5757?

**Victor Zhou**
Free thoughts and free access distribution that send do you use that when you say remove the requirement for distribution of that that is removed?

**Sam** [47:00](https://youtu.be/-UDyjJy1ULg?t=2820)
So no I'm not ever going to back away from requiring free access to an EIP’s like links but the requirement for redistribution that's the so like if there's a requirement in 5757 that says sources should not allow redistributing in the assets directory and I think Greg had an issue with that because of context like if it's on the is that right? So I can remove that…

**Greg** [47:28](https://youtu.be/-UDyjJy1ULg?t=2848)
I don't really I don't understand what it's saying there just pointing out that on the one hand it's good to have things in assets on the other hand there's both legal aspects as to whether we had a right to put it there um so that's where a list really helps that we've judged as editors that we don't have a problem publishing things there because you don't want the author randomly putting things there it is part of what we publish and when you put things there there is a you have taken them out of context but that's where I keep wanting a reference section with a full citation so that the implementer can find larger context easily enough there doesn't need to be only one link in the reference multiple links are appreciated yeah so in the BLS example the canonical link to the publisher's page was paywalled but the DOI link went to the same page but the ePrint server had a free copy and the eprint server is a pretty stable source I don't think 10 years or I don't think there's any particular definition of stable we can give but it's a judgment call and eprints pretty good…

**Lightclient** [49:05](https://youtu.be/-UDyjJy1ULg?t=2945)
So are we hung up here on the redistribution aspect or on the paywall aspect?

**Greg**
I'm just saying there's decisions the editors are going to have to make and I don't think we can need to set up all this policy in advance just say that you know we can agree that there's a list of sources that we simply approve I think we've got some number already in mind that aren't controversial to us, any other links we do just have to take up as judgment calls that really haven't been that many of them and whether to add whether to add a particular source to the EIP 1 is an editorial editor's decision the author doesn't need to be involved and I can't see creating separate EIPs for every change that we make the EIP 1. 

**Lightclient** [50:00](https://youtu.be/-UDyjJy1ULg?t=3000)
It is still an editor decision and we said we're not going to do the EIPs it's going to be a PR to EIP 1 the reality is that sometimes the author is going to have to make the pr and advocate for that link like if an editor generally reviews the pr and says I don't think this is a good link the author is going to need to advocate like it shouldn't necessarily be our jobs like advocate for every single link but I think not having the EIP makes it simpler for them.

**Greg** [50:26](https://youtu.be/-UDyjJy1ULg?t=3026)
That okay that's the core of our disagreement allowing a particular link for particular EIP should not say that that is a good source for all EIPs.

**Lightclient**
Yeah but we've like already discussed that what you're describing is how we like previously managed the links for EIPs and the editors as a whole are like against this and so we're trying to find a compromise and I think like the compromise that we're like trying to zero in on is creating a list of sources that we think are good for all EIPs. It's not perfect but I don't know if we're going to be able to get agreement on like a per EIP acceptance list.

**Greg** [51:12](https://youtu.be/-UDyjJy1ULg?t=3072)
Well it hit me personally where I wanted to link to a paper by turing it actually wasn't paywalled and there was a strong objection to linking to that paper.

**Lightclient**
Is it DOIed?

**Greg** 
Yeah there was a DOI for it there was a list.

**Lightclient** [51:34](https://youtu.be/-UDyjJy1ULg?t=3094)
So yeah...

**Greg**
I mean it was fine but yeah 

**Lightclient**
So I think we should allow the DOI links

**Sam** [51:41](https://youtu.be/-UDyjJy1ULg?t=3101)
Yeah. Yeah so what I was suggesting what like how I would do the DOI if we were using the old style 5757 where it has its own individual EIP but we're not doing that so let's not open that back up again but if we were, my idea for DOIs was to have like the title author publication date the DOI number and just any arbitrary link to a free copy of the paper that is how I would do the DOI like reference section but then…

**Lightclient** [52:11](https://youtu.be/-UDyjJy1ULg?t=3131)
I don't like I really don't want to go into like these super specific details because like I don't think that we should be linking to any arbitrary link I think we need to like have a you know general link to the DOI object and expect people to go find it.

**Sam**
Okay.

**Lightclient** [52:26](https://youtu.be/-UDyjJy1ULg?t=3146)
Okay because like I don't because I mean lots of professors will like put a paper on their on their like university web page and like I don't want to sit have people like being oh this was the free source or maybe you were linking to stuff that you know is paid content and we shouldn't allow like links like that there's like legal concerns there I think we should just link to the DOI object identifier website.

**Sam** [52:47](https://youtu.be/-UDyjJy1ULg?t=3167)
So then how do you verify that there is a free publication available?

**Lightclient**
I like I mean I think that we need to remove the must for it not being paid have like a very strict requirement of should not, but if it has a DOI identifier it's almost always accessible and some mechanism for free and there's not I just don't think there's really a way around this.

**Victor Zhou** [53:18](https://youtu.be/-UDyjJy1ULg?t=3198)
I have seen a review I think we should not require it to be like completely free like I want it but I don't think that requirement can help improve the things overnight.

**Lightclient**
Question, would you be willing to relax it must not link to a paid content and just have it be extremely strict should not?

**Greg** [53:43](https://youtu.be/-UDyjJy1ULg?t=3223)
That would help a lot yes.

**Sam**
Yeah, sure. Yeah sure I think it's a dumb idea I don't think core devs are ever going to pay for access to something…

**Lightclient**
They're not they're not definitely not.

**Sam** [53:59](https://youtu.be/-UDyjJy1ULg?t=3239)
So I don't think there's any point in allowing non-free resources because…

**Lightclient**
I mean it's just it's not about I mean I don't ever want to allow non-free resources but there is a problem where like how do we uniformly link to DOI objects and also ensure there is a free link without also running into like potential legal concerns like redistributing copyrighted material.

**Sam** [54:19](https://youtu.be/-UDyjJy1ULg?t=3259)
Well because we won't be redistributing it somebody else will that's the point.

**Lightclient**
But I yeah but I also like don't like the idea of just like you know I don't want to put a library genesis link in the EIP repository I don't want to put a link to a professor's website in the EIP repository I would rather just link to the DOI object and just assume that people like know how to like access that information.

**Sam** [54:42](https://youtu.be/-UDyjJy1ULg?t=3282)
I mean I think that's just like it's a really worse than having a link to the free copy and the DOI number.

**Greg**
I can I can live with that if there's a DOI number there's a whole organization that maintains links if there's a full citation google will usually find you free links there's libraries I don't mind I don't mind if we have to resolve this I don't mind pushing onto the implementer a bit of work to go find this I think it's a fantasy that an implementer can just sit down with an EIP and Wham Obama implement it, it's hard work but as long as there's a way to find the information, Google does I would prefer there that they be allowed to include the link but like to avoid the impasse where I was, I simply removed the link and put the citation in line and the bot quit complaining and it merged so.

**Lightclient** [55:53](https://youtu.be/-UDyjJy1ULg?t=3353)
Okay.

**Sam**
Okay say it so I guess in the interest of not holding up this discussion anymore I'll change it to it should not but…

**Lightclient**
I mean I want you to advocate for every single source that there's like a free accessible you know resource and I we can talk about exactly how to format that and I think I would probably be okay if like the default link was to the DOI object but we had like a list of like free links to all of the things that are linked we can figure out the exact yeah exactly the way that that works I'm happy to do that yeah I mean I think that we're good to move forward 577 in that case like we resolved the separate EIP issue we're going to do it as a PR in EIP 1 and we've resolved the like redistribution, I don't know if we have to remove it it's already it should not, to me like it doesn't need to be removed but we can remove it and then for the paid content I think it should not would be profitable and I think that like you know generally editors should always advocate for free resources. 

**Pooja** [57:07](https://youtu.be/-UDyjJy1ULg?t=3427)
Sounds good so if we have to summarize there would be small changes to the current proposal of 5757 but we are as a group looking forward to have that merge. 

**Sam**
So just to enumerate the changes I'm going to make and then if I miss something please speak up now. I am going to remove the EIP per origin section and it'll just be a PR into EIP 1. We will figure out a way to specify free links for DOI objects and I will remove the non-redistribution requirement. Is there anything else that I need to change? 

**Lightclient**[57:46](https://youtu.be/-UDyjJy1ULg?t=3466)
Sounds good to me. 

**Pooja**
Greg, if you have anything to add or you or you're fine with this number of changes that Sam listed?

**Greg** [58:00](https://youtu.be/-UDyjJy1ULg?t=3480)
I think I'm fine and yeah I could I can try to review the document after the changes have happened so I don't quite understand the document as written so once the changes are there I think I'll be able to understand better.

**Sam**
Perfect, okay. 

**Greg**
It's my fault I've been busy trying to find money turn a living so this is this is not uh yeah let me busy inventing the technology that we're trying to sell uh to get the money during a living so this is slipped down the…

**Pooja** [58:38](https://youtu.be/-UDyjJy1ULg?t=3518)
Not a problem one last question to the group do we think that we may need a breakout room for like with the changes Sam will be making some changes and we can discuss that somewhere before the next EIPIP meeting?

**Greg**
I think one already sort of happened on all core devs but um but the answer is probably yes.

**Pooja** [59:09](https://youtu.be/-UDyjJy1ULg?t=3549)
Okay.

**Lightclient**
I don't want to have a breakout room.

**Pooja**
Allright.

**Lightclient**
I honestly think we should merge 5757 as is, it's a draft we need to start moving it to final and…

**Pooja**
Yeah

**Greg**
You are right.

**Lightclient**
...the changes and we can review the changes directly to it.

**Greg**
We're at draft stage.

**Pooja** [59:34](https://youtu.be/-UDyjJy1ULg?t=3574)
Right and I think that would even help with some EIPW changes that Sam has already uh working on so we can have that proposal merged as draft.

**Greg**
Yeah a lot a lot of this a lot of this the community can argue about during review that's what review is for.

**Victor Zhou** [59:46](https://youtu.be/-UDyjJy1ULg?t=3586)
Sam are you going to represent the full source in the format of regular expression is there any formal way that you want to establish?

**Sam**
Yes, I would love regular expression um that makes it really easy in EIPW but uh it's probably going to be more complicated than that.

**Victor Zhou** [1:00:08](https://youtu.be/-UDyjJy1ULg?t=3608)
Okay. Okay yeah just like I I I don't have strong preference but maybe eipw is much easier yeah.

**Sam**
Okay.

**Victor Zhou**
Nothing else. All right thanks for the great efforts.

**Sam** [1:00:24](https://youtu.be/-UDyjJy1ULg?t=3624)
Talk to you all in two weeks.

**Pooja**
Thank you.

**Greg** 
Thank you for the efforts even though I grumble about them.

**Sam** [1:00:36](https://youtu.be/-UDyjJy1ULg?t=3636)
It wouldnt be covered if people didn't grumble so..

**Victor Zhou**
 I hate that proposal but I really appreciate your efforts.
 
 **Pooja** [1:00:45](https://youtu.be/-UDyjJy1ULg?t=3645)
 All right guys see you all in two weeks and we can continue discussing on Cat Herders Discord or Ethereum Discord, wherever possible have a good one everyone.
 
 **Lightclient** 
 Yeah thank you thanks for hoping bye.
 





Okay. 


































































































































































































































































































































































































































































