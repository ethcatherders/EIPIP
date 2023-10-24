# EIPIP Meeting 88 Notes
### Meeting Date/Time: Aug 23, 2023 at 14:00 UTC
### Meeting Duration: 1:01:10 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/257)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=i03o5JMQ-zY&list=PL4cwHXAawZxpLrRIkDlBjDUUrGgF91pQw&index=1)
### Moderator: Pooja Ranjan
### Notes: Metago

## [Summary](https://github.com/ethereum-cat-herders/EIPIP/issues/257#issuecomment-1690850073) 

## Introduction

**Pooja**
Welcome to EIPIP meeting 88. We have shared agenda in chat, which is
issue number 257 on EIPIP GitHub repository. Thank you everyone for joining. We will go ahead and start with our agenda item.

And the first one here is to discuss open issues and ?. We will also discuss issues from the past that are ongoing discussion, will have a look at the Monthly Insight, a brief of EIP editing office hour, and anything else
anyone would like to share or discuss today. 

## Discuss Open Issues/PRs, and other topics
### [Placing a warning on ERC-20]( https://github.com/ethereum-cat-herders/EIPIP/issues/255#issuecomment-1671818828) [0:50](https://youtu.be/i03o5JMQ-zY?si=UkFwr8Sj4nm4nbvY&t=50)

So starting with the very first item
under which we have, the first one listed here is placing a warning on ERC 20. 

I know this was recommended by Sam Wilson. Sam, if you would like to provide an overview on what this is all about?

**Sam**
Sure. I wouldn't say I'm recommending this, but I'm the one who put it on the agenda. So there is a developer, dexaran, that is annoyed that people keep losing money with ERC 20s and they're asking us to put a warning on ERC 20 to tell people that it doesn't require that the destination of a transfer can actually accept ERC 20 tokens. So this is fixed in a bunch of newer proposals but people keep deploying ERC 20s and people keep losing money. My personal view on this is that we shouldn't modify ERC 20 and if people want to use a better standard, they can, but I wanted to bring it up here because I said I would. 

**Gcolvin**
I noticed he was also like trying to get in touch with the foundation through us and things like that, and yeah I think you sort of let him know that he was talking to the wrong people, but he should be talking to core devs and
contacting the foundation directly with some of these issues, and of course ERC 20 and anything final is immutable, so I think that's that. We don't, I guess he could open a new EIP at the informative level to tell people about this.

**Victor**
All right. So my view on this is that the ERC 20 is definitely has that caveat and that is by design. Finding the right place to show the warning is something that I felt slightly leaning towards in favor of but I also think in a larger scope,
in a larger context, we should start to think about how do we allow proceeds allow, supersedes or how do we allow newer best practice for example like the internet standards like rfcs they will say this RFC is superseded by the other one and also they will have a number for best practices so they will actually refer to best practices in those cases and for standards that's important like the ERC 20, maybe it's a play a good place and good example for us to discuss EIP editors and ERC editors group as a whole, how do we harness and QA this practice of continuing to improve. We've seen this we also seen the caveats in the how the approval was made right. 
Initially ERC 20 was designed to set up specific approval limit however most of the exchanges these decks require a very high or almost unlimited approval when they actually use that, like Uniswap, Permit 2. Those are what we see in practice and then I think of a good starting point for us to discuss how do we talk about improvement of standards and how do we direct people to use newer and better backward compatible versions. So that's my view yeah. I'm done talking.

**Danno**
Yeah thanks for that. I tend to agree that some form of update or errata should coexist with the immutability of a final one. I think one I can't remember where but I think I offhandedly said like underneath but just instead of something that and maybe when something goes final an author should be able to say like please see this later informational EIP that some of us also wrote that wrote this EIP sort of like best practices like you mentioned like linking to a later document that nuances that are caveat that or give the implementation guidance or something because like supercession sort of implies a technical thing being replaced by an a newer technical thing with legacy support for whether to proceeding but like just a newer document that just describes problems not foreseen at the time it went final, is a different speed you know it's not a superceession it's just sort of a please see this later document as well from the author. 

**Pooja**
Danno?

**Danno**
 I think there's like two issues here should these be allowed in general and in this one a particular should it be allowed I think there needs to be some sort of standards I think I'm personally opposed to putting a warning on ERC 20 for this because it amounts to user error and I think that should be considered part of the warning one that I could get behind was let's say hypothetically there's a break for the Blake too for the Blake 2 hash function that you know something is cryptographically broken that's worthy of a warning on an ERC or an EIP but something that is you know practiced and used, I don't think raises to the level of putting a warning sticker on there.

**Sam**
So one of the big problems with these kind of warnings and additional notices and I think that's one of the reasons we don't have them so far is that who has the  authority to make these claims so like let's say that I don't know, Blake two is broken. How do we verify that it's broken and how do we verify that adding that information is, you know, correct, and maybe for less black and white things like this ERC 20, there are, you know, fungible token standards that don't let you send tokens to contracts that don't support it so they fix that whole class of user errors but you know I say I'm with you on this one Danno, I know where I don't think we should put a warning on it because you know it's like mailing money to an address that doesn't exist and you don't put that warning on the postal service right? Like so yeah basically I just don't want EIP editors to have the power to determine whether or not something is worthy of a warning so I'm, you know, we should just not have them at all it's kind of my thought.

**Victor**
I think you bring up a good point and a center of it is who has the authority and I think I'm with you on that in that ERC editors on probably not the best one to have that authority whether to put that consideration somewhere to allow readers to be more cautious or have an added educated approach to it is I think a separate story about where the authority, who the authority who has the authority maybe also as the Authority or maybe we can have a social consensus to allow that to happen and even if it's a warning I'm not saying like on top of it there should be a warning I'm more in my mental model I'm more thinking of maybe it should happens in the consideration.

I don't know if it's a security consideration but this is something pretty new to a lot of people the metaphor of mailing an envelope to an empty address is a good metaphor but a lot of people doesn't yet have established that kind of mindset yet so my view on that is if people will be writing ERC from day one and if there is a consideration section, maybe in the consideration section they just mentioned that not all addresses by Ethereum design, has the ability to send back or to resend another ERC 20.

That's different from the address that doesn't exist. The USPS will rebond address or if it's an empty house some people can go in there and and claim it and by the design of Ethereum at the moment right now, an address is by generated by a lot of the actions and then if it doesn't exist then it  doesn't exist right the contract is a hashes or EOS is it's the public key so that's the difference between the empty address metaphor versus these and the skin scenario I'm done I'm done talking.

**Danno**
I mean I think there's, I agree that a general purpose warning put there by some big collective is not good. I was kind of assuming that you ever did the same controllers have changed ideally after it becomes final as well and whoever sort of like speaks whoever can could still updated if it wasn't final could theoretically add some kind of Errata or booth a generally useful thing the Blake 2 example is good because if you for instance if you wrote an EIP that was like a pre-compiled for a specific signing function or you know cryptography is sort of always supersedable or unforeseen complications other event practices come up later after something goes final the author should be able to say please see this later EIP and so it isn't really appropriate for that author to say like two is definitively we can't use it anymore they could only say look at this other document and in that other document it could argue that maybe it's bad according to some criteria but it's like just pointing to a later document not you know anything more substantive. That was sort of like my idea of the Errata thing and in that sense also coming back to the specific case um if this guy this person seems like they're maybe on something of a crusade and like it seems like they're trying to prove a point about the governance or the documentation or something, so like in a way it's a politest thing to do if there was an errata option available to authors of final EIPs, we can tell the person hey you don't keep bothering us don't keep bothering Ethereum Foundation, the only person who could point to updated guidance would be the authors of ERC 20.

Like For Better or For Worse maybe this mean to them but I don't know just on 

**Sam**
So I think something that we could probably do today would be PR against ERC 20 updating the security considerations section with a note getting it approved by the author I think that would be um doable? I think they could fall under Errata or clarifications. 

**Danno**
So this I just assumed that adding any even non-normative text to it to a final EIP was breaking the immutability I didn't even know that was an option I was assuming you could only Point towards a later EIP you have to ask the authors to make another EIP. 

**Pooja**
Greg you were saying something? 

**Victor**
Greg, you are muted 

**Greg**
Okay there's the button. A final is final and Errata are for the case where the EIP actually fails to describe the actual intended normative behavior so that this is this is what ERC 20 does normatively. For all I know there's applications out there that actually use this behavior for a purpose. So there's just there's no there's no point to going in and changing these things. There are other token standards you can use if you don't like this behavior and this person is quite free to write an informative EIP describing this problem and making these warnings and he's free in a bigger sense to create his own group to start some process of going through things and starting a process for finding these problems and creating EIP to report them maybe a living EIP we just don't have a process for this and it's not clear that it's the editor's problem to start keeping track of ways that you can get in trouble using various standards there's any number of ways to get in trouble with Ethereum and lose lots of money.

So there's nothing wrong with the ERC 20 that needs to be fixed here it's just what it is.

**Pooja**
I would agree to that like there could be proposals which are superseding but supersede is no more uh status for ethereum improvement proposal so perhaps we can as Greg suggested maybe suggest the user to come up with another proposal which may fix an informational proposal, if that helps so they can share more information about that and also Sam suggested to have a PR against ERC 20. I don't know what is the conclusion here like what is the recommended action?

**Sam**
Greg pretty much convinced me that that's a bad idea so I think the recommended action is we do nothing and they can tell people as much as they
want that ERC 20 is bad.

**Pooja**
Right. I suppose the author is also trying to talk about ERC 223 which according to the proposal may be referring to some of the issues that he is claiming to be there with the ERC 20 so if people are interested they can also take a look at proposal ERC 223, which is currently is in the last call and the deadline is September 3rd. 

I think with that the conclusion for this item is editors may not be responsible of keeping track of adding warnings to proposals which are already into the final status and the user can come up with informational EIP and share the information at various levels.

### [Update EIP-1: Remove requires header ethereum/EIPs#7478]( https://github.com/ethereum/EIPs/pull/7478) [18:17](https://youtu.be/i03o5JMQ-zY?si=UkFwr8Sj4nm4nbvY&t=1097) 

Moving on to, thank you Sam, moving on to the next item here, which is update EIP 1 remove requires headers. I suppose this is initially opened by Pandapip but I suppose Sam mentioned that we should be discussing it over here?

**Sam**
Yeah so Panda's been having an effort to cite yeah like to have EIP show up in Google Scholar and one of the things you need to do to have that happen is have like a real bibliography. This is one step towards that where Panda wants to remove the requires header and instead generate the bibliography from links to EIPs in the Proposal itself. So we would no longer have the distinction between like non-normative and normative like EIP references they'd all just be regular links.

**Victor**
Is this a requirement for biography to be generated?

**Sam**
No.

**Victor**
Can we have that and maybe touch the movie requires later down the road? I know that in some places we strictly previously strictly enforces what goes into the requires must uh there's normative links and if we have nothing, I'm not I was not a big fan of that requirement, but if we have mandated that in the past maybe that needs to be taken into consideration when we remove this all together.

**Sam**
So you're saying you'd like to see the bibliography stuff before we remove the required header?

**Victor**
I was  saying that it since the original proposal was to introduce bibliography section it seems to me based on your understanding and my understanding having a request doesn't block generating bibliography, so there's no enough justification to support removing requires at this moment.

**Pooja**
Anyone else has any thought on this one?

**Greg**
Yeah I agree with Victor there we've I've proposed a reference section um and not all of the links in a reference section have to be up to date in the way that the require section does need to track what's normative at a given time so I think they serve independent purposes and I wouldn't I wouldn't want to try to generate require system automatically.

**Pooja**
I would appreciate if either Victor or Greg may add a comment to this pull request that might be helpful, because panda is not on the call although the recording will be made available, but that would help future discussion on this PR.

**Victor**
 I can I can help put down if yeah.

**Pooja**
Very well, anything else on this one? Greg I am wondering if your hand is raised for this one or from the earlier? 

### [Update EIP-1: Add numbering guidelines ethereum/EIPs#7388](https://github.com/ethereum/EIPs/pull/7388)  [22:26](https://youtu.be/i03o5JMQ-zY?si=UkFwr8Sj4nm4nbvY&t=1346) 

Okay cool moving on to the next one is adding numbering guideline. I think this PR is also created by Pandapip last month with respect to how we are changing EIP numbering I suppose. The pr number here is 7388, any comments on that? This seems to be approved by Sam and okay yeah Micah also mentioned it for another PR? yeah any thoughts by editors on this one?

**Sam**
Yeah I think it's good to update this since we did change how we number stuff so. 

**Pooja**
So this just requires merging. Nothing else to be done? Cool so we can consider this as approved and will be merged unless anyone else has any comments to add on the pr directly if not here.

### [Update EIP-1: Semi-stagnation of last call EIPs ethereum/EIPs#7346](https://github.com/ethereum/EIPs/pull/7346) [23:44](https://youtu.be/i03o5JMQ-zY?si=UkFwr8Sj4nm4nbvY&t=1424)  

Moving on to the next one is about semi stagnation of the last call EIPs. This was earlier discussed in one of the EIPIP meetings about proposals standing in last call for a longer duration of time, I believe at the time most of the editors were in agreement that this is fair to move the proposal into the stagnant status. Anyone opposes to this PR?

**Sam**
So let me see this one this so move this will just say that we can move things from last call to stagnant?

**Pooja**
That's right and with the help of bot.

**Sam**
I mean I feel like we should just move them forward for the authors but maybe we shouldn't I don't know.

**Pooja**
So what happens what happens here is like if the pr is not raised, if the pr is sitting then we get a warning to the author but if the author forgets to create a peer there is no warning sent to the author. 

**Sam**
Yeah I think I'm okay with this it'll just move it into stagnant, which I think is fine.

**Pooja**
Okay yeah the idea is the bot will move it to stagnant and the moment the bot will make it to the stagnant it will obviously create a PR and that will automatically generate a message to the author that this proposal, I mean this EIP is being moved to stagnant, if he or she wants to not stagnant that proposal, they can come up with a PR to move it to the final. 

**Sam**
Yeah that makes sense.

**Victor**
 I felt this is another example of problem with EIP ownership the problem happens when authors contribute to the point when they stop getting actively engaged, do they still own the EIP or does the community or in in any group owns this. Community this come up uh in our previous conversation of the remove whether to add a warning to ERC 20 the author was no longer very active in this particular ERCs and then also in that in this case of when at EIP of last call losses authors to move it to final so maybe in the future we can discuss about how do we handle or how do we help in this case, in those cases in an ownership perspective.

**Pooja**
Sounds good.

### [Update EIP-1: Add adoptable field ethereum/EIPs#5533 ]( https://github.com/ethereum/EIPs/pull/5533)
[26:53](https://youtu.be/i03o5JMQ-zY?si=UkFwr8Sj4nm4nbvY&t=1613)  

Moving on to the next one here on the agenda is ADD adaptable field, the pr number is 5533. I think it was added by Sam Wilson.

**Sam**
Yeah I thought we had decided that we weren't doing this.

**Victor**
Ownership problem?

**Sam**
Yes yeah.

**Pooja**
 so we need to close this PR?

**Victor**
I think Panda actually bumped it up and we've opened it so Panda was not here.

**Pooja**
Okay in that case maybe if we can drop a comment that we decided to close this one and we can take any further discussion on the Discord.

**Victor**
Yeah and Sam already commented.

### [Add NIST as a permitted origin for external links ref](https://github.com/ethereum-cat-herders/EIPIP/issues/257#issuecomment-1688478926) [27:50](https://youtu.be/i03o5JMQ-zY?si=UkFwr8Sj4nm4nbvY&t=1670) 

**Pooja**
Perfect. The next one here is add NIST as permitted origin for a reference for external link.

**Sam**
So this would allow linking to cves which I think might be kind of nice and we have an author asking for it. I just wanted to know if anybody had objections to that before I wrote up the EIP for it or the the pr rather?

**Victor**
Yes we should be able to link to cve so I'm in favor of that.

**Sam**
All  right I'm not hearing any objections so I'll put it on my to-do list.

**Pooja**
Just to clarify so for this particular item people think that it would be a good idea to come up with an EIP and Sam would be taking care of that.

**Sam**
Yep.

**Pooja**
Perfect.

### [Update EIP-5069: Replace handbook with charter ethereum/EIPs#7468 Ref Discord](https://github.com/ethereum/EIPs/pull/7468) [28:48]( https://youtu.be/i03o5JMQ-zY?si=Ik1XrvWmr6uwMrPM&t=1728)

The last one under this section is update EIP 5069, replace handbook with charter. So in the last meeting of EIPIP we discussed that the proposal, the charter shared by Sam should be in two parts, some updates goes to EIP 1 and some updates goes to EIP 5069. I see a big overhaul here. The proposal is being moved from informational to meta and a lot of things are being changed. The pull request number is 7468. I think Sam is looking for some last feedback if people have any, before this could be merged. 

**Victor**
I'm generally in favor of that direction proceduralize them. What do you think if we change the content and teach them informational at least for a amount of time like a few months for the general public, editors, authors and everyone to get familiar with them before moving them to the meta? The reason being that moving to Mata is enforceable and for important document like this is since we need more, like if we are imposing a review last call final for a technical document, I think we should also have a way for people to know that something is coming up, it's important, and if we want to adopt them there is a time for you to voice your feedback in general public property in general public this is because the editing itself is still in draft, and it has not been published to be viewed by a lot of people, it's currently only editors are involved.

**Sam**
Well this is a governance decision for ourselves so I don't know if it needs to be like open to everybody, but 

**Victor**
I think ourselves if we're refer to editors and authors I'm under that impression because it impacted how authors like being treated in the future, down the road 

**Sam**
So what would be the externally visible changes that authors would see if we adopted this?

**Victor**
I think we should I think at least a better way is to publish it as an informational and then have a PR standing there to say hey in a few, a long number of weeks that were moving into meta enforcing it and you better respond by this and then also I think it's worthy of bumping up the FEM threads that this is turning from informational to meta.

**Sam**
I can do it as a different EIP if that makes it better, like and just go through the the process. 

**Victor**
Like well that yeah that will work currently no one is engaging in the EIP editor handbook thread and if we're turning it into charter which is I think I'm in favor of that it makes enforceable and then then people should really care.

**Sam**
I'm just really not seeing what other people need to care about for this it's not going to make any differences for people outside the EIP editor group, like there's no topic groups in here anymore it's literally just like writing down our decision making process.

**Victor**
Okay I hear that you said there's no point notifying outside of the EIP editor groups because you think this is a decision make among ourselves.

**Sam**
Yeah exactly. I just don't understand what like why do we need input from people who are not editors on this? 

**Victor**
I don't know Danno, what's your view? I guess maybe providing a perspective.

**Danno**
So when you're working with a system it's nice to know how you expect it to work although this would be law and how these readings actually work as case law and they are quite different so that is a point of frustration is that it's a random number generator when someone who is not an editor interacts with the system. 

I'm kind of disappointed now to hear the topic groups you're out of this are they out in general are they just out of the specific ERC?

**Sam**
They're just out of it until we like there's still some finer points that we want to work on so we're just getting this in first and then we're going to add topic groups or working groups.

**Danno**
I mean from an outside perspective when The outsiders don't have any input and they watch what should have been an agreed-upon thing that was agreed in principle three weeks ago get spinned over and over they lose a lot of faith so that's a perspective as an outsider.

**Victor**
I think what I hear Daniel says is that it will if we let outsider give us the back on this and give them some time it will allow us to accumulate more faith or credit from them, if we don't then we lose the chance to get their credit and to improve our credibility by soliciting outside feedback. Is that a good understanding of your perspective?

**Danno**
Well even if you get the outside feedback, will it speed up the process of actually coming to a decision and consensus? Because anything that slows down that process is going to cost credibility. 

**Greg**
I'm sorry which do you want, did things go really fast or that the community has time to let us know that this is a charter for a group that they actually want to serve them in the ways that we want to serve them well?

**Danno**
We want certainty, it's like a court of law you want certainty you don't want you don't want unpredictability.

**Greg**
But we also I do think we want feedback from the community so that they understand we are the editors and this is what we are proposing to do. We can reject the feedback but it would be good to have that feedback and we've been around long enough that taking a bit of time to try and get things right is I don't think a big problem. 

**Sam**
All right so I'm hearing that you guys want me to have a last call type period for this, where we can get feedback from the community? And I'm also hearing that Danno is upset that it's taking a very long time and that we aren't making any decisions. Is that a reasonable summary of everybody's stances?

**Danno**
It's not that it's taking a long time is that three weeks ago there's one decision and then all of a sudden it's just thrown up in the air like 52 card pickup, so that's my personal perspective, I'm not speaking for all core devs in this regard.

**Sam**
Yeah okay 

**Pooja**
Just to I traded here a proposal which are moved as living there are very limited proposals which are in living status that already provides this flexibility to make changes in future. That's the reason why we do not have this last call thing added for proposals which are in living statuses, however I find it as a good idea to have it publicized, reliving the FEM discussion thread is good suggestion. We can perhaps make use of that but as per my understanding we do not necessarily wait for another 14 days for this to be settled down. So if people are okay we can perhaps keep this PR open for another seven days or so, and maybe we can have discussion thread ignited again on FEM about this change coming up. Would that be a fair resolution that we are coming to a decision, we are going towards getting this certainty and we are not waiting for a very long time?

**Danno**
I think I'm just more disappointed that it was communicated to me that there was a consensus and they were going forward in that all of a sudden everything's on the table again so that's where a lot of my frustrations come from.

**Pooja**
Yeah I understand that but I don't think we'll be moving in that direction we are not going back. The decision is still there we are just trying to make sure the decision is added and being reflected in the document, so people can follow and refer it in future, so I see a couple of hands up by the editors here. Just as a summary we can have this pull request open for next seven days and after that if Sam will change from, you know draft to a real PR that would be merged by bot, so anyone having any thoughts try to come up before that.

**Victor**
So I think I would personally suggest that we publish it at as opposed to merged as a SL post of keeping it as a draft PR because not many people will be able to see that and also publishing it allows search engine to pick it up, allows much more notification to kick off. So what I would suggest alternatively we introduce all the change, publish it, except for the type being informational rather than meta, and in a few weeks we make another pull request to move it from informational to meta, just start enforcing it.

I want to know what people think about of this approach instead.

**Pooja**
My quick question here. I know the original author is Sam. Panda and me and Sam has created the pr. What can be done that bot does not merge it. If Sam moves it to draft.

**Sam**
Well as long as I keep in draft it won't merge it that's why I keep it in draft.

**Pooja**
Yeah but I think Victor is suggesting that we should make it like as a normal PR so people can see it and it should be publicized.

**Victor**
Yeah I actually should merge it and publish it as an informational before we start enforcing it in the meta and maybe we should drop a line in the document says this is going into meta, if no objection like in a time that we agree in a timeline that we agree upon.

**Pooja**
Yes Greg. 

**Greg**
I'm confused wouldn't this be better as a living document?

**Sam**
Yeah it'll be living in the meta category.

**Greg**
Yeah, okay. So yeah, if we go ahead and publish it and it will have a discussions-to link so any discussion on it can continue and as it moves to living changes can be made on the basis of the discussion and I think that that takes care of what I'm hearing. 

**Pooja**
So the idea here is the status is going to be living. It is not changing. That one thing that is changing is category and type. Earlier it was informational and now we are talking about moving it to meta.

**Sam**
All right, so just to reiterate one final time my understanding of the plan is change the pr from a meta to informational so that there will no longer be a status update, then merge the pr and then in two weeks from today on the next EIPIP call, we can ratify, like make this our government's process. Do I understand that correctly? 

**Victor**
Yeah except for two weeks maybe too short for people to give this kind of feedback but I'm okay if it's too weak. I'm just yeah.

**Pooja**
Two weeks is generally the last call period even if we are not following it formally the last call period informally it is being followed here 

**Sam**
And this will be I think I don't know week five or week six that the proposal has been circulating at least semi-publicly so yeah okay I'll do that perfect.

**Pooja**
 so 7468 with the status with the type change back to informational the pr should be good to be merged and in the next meeting we can discuss further changing from informational to meta.

## [Changes to Final proposals]
[Update EIP-1820: Remove superfluous pre tag ethereum/EIPs#7506](https://github.com/ethereum/EIPs/pull/7506)  
[Update EIP-820: Remove superfluous pre tag ethereum/EIPs#7505](https://github.com/ethereum/EIPs/pull/7505) [44:03]( https://youtu.be/i03o5JMQ-zY?si=Ik1XrvWmr6uwMrPM&t=2643) 

The next one here is a set of proposals which are already into final status number one is 1820, the pr is 7506. I think all of them are created by Sam, if I am not mistaken. Maybe you can share the purpose of having this changes to already finall proposals?

**Sam**
So these are 7506 and 7505. Yeah okay so these two are, somebody put raw HTML in their proposal. They just look like, it's just not necessary HTML tag so I just want to remove it for formatting purposes. 

**Pooja**
Anyone has any objection? So the other PR 7505 is also same or similar, right?

**Sam**
Exactly it's just removing okay pre-tags.

**Pooja**
Okay so maybe editors can take a look and if anyone has any objection drop a comment over there otherwise this PR should be good to be merged in next two weeks if not before that. 

**Victor**
Hey Sam, did you put in like how long does electing keeper how often do we elect a keeper?

**Sam**
It's whenever anybody asks for it so any editor can be like I would like to elect a keeper and then an election starts. 

**Victor**
Oh okay oh anyone at any time can call for a keeper? Okay agree upon okay yeah that's good. 

### [Update EIP-4804: Add more details for the examples for EIP-4804 ethereum/EIPs#6860](https://github.com/ethereum/EIPs/pull/6860) [46:07]( https://youtu.be/i03o5JMQ-zY?si=Ik1XrvWmr6uwMrPM&t=2767) 

The next one here is a PR number 6860. It is about a proposal which is already in final, number is 4804. I think there were some review suggestions by Sam and author has responded to that. I do not see any change in the code here, but yeah I wonder if people are generally okay to get this PR merged because it's been a while it is sitting over there.

**Sam**
Oh so I'm still I think in the camp of not updating this but yeah I guess we can read this and comment on it.

**Pooja**
Yeah that would be helpful. 

[Discussion continued or updates from past meetings] 
[EIP-ERC GitHub repositories]
[Update EIP-1: EIP pain relief ethereum/EIPs#7230](https://github.com/ethereum/EIPs/pull/7230) [47:08]( https://youtu.be/i03o5JMQ-zY?si=Ik1XrvWmr6uwMrPM&t=2828) 

Moving on to the item number two okay we have eight minutes left and let's try to move as fast as possible, discussion continued or updates from the past meeting it is about EIP ERC github repositories split. I think we discussed part of it in fact more of it in the earlier discussion, yes Danno, if you have to add anything on this topic?

**Danno**
The EIP 7329 you asked me to put a review with all core devs, should it be moved to last call now? It's really it's the pr informational meta giving the ration office split. 

**Pooja**
Yeah, that could be done anytime. 

**Danno**
Okay, I'll move it in last call for two weeks from today. 

**Pooja**
Perfect thank you and I think we are good with all other decisions that the decisions were to move part of it in one and part of it and the EIP editors Charter book.

Yes Greg please go ahead.

**Greg**
Yeah, Sam and I discussed this and there's just an editing merge issue as EIP 1 has changed enough that the merge can't happen and what we want to happen is to be sure that the core devs can keep track of their own statuses. We don't want to force them into that there must be a review period, there must be a last call period. They had their own workflow and they need to put that in the document and I think Sam may remember better the choice was whether to just let the core devs use the existing status field for that purpose or whether to introduce basically a working group preamble that the working groups and initially the only working group we have is the core devs, that the core devs can use that preamble in any way that they want, tracking status tracking anything else that they want to track in the document.

And so that's that was the one thing we needed to settle and the other was a reference section. What we needed to go in there, distinctions on informative and normative links. I don't think that all got settled, but the first one I know Danno had a strong interest in and I'd like to hear back from Danno on that sort of choice. 

**Danno**
So my understanding was, we split this entirely in two, the split is separate from all other governance issues, whether we use headers or not, and those moved into the discussion of what's going on with the new topic groups and with the EIP editor preamble, I was hoping we could talk about topic groups this week because I was hoping that the new charter would have been resolved by now and I think that we can't really talk about those details until after the charter is complete and set those standards and because the agreement that I remember from all core devs from two weeks ago, was the split is completely separate from governance issues.

**Greg**
The splits happening yeah, that's where the files go in the repo that the question is we still currently have a status field and a defined workflow for what goes in the status field.

**Danno**
Well those are governance issues and those can be resolved once the charter's done. 

**Greg**
We pretty much are done with the charter, that we're going to put it up for some comments but I don't expect any substantive changes there. so what's what we broke out of that was the working groups, because the question the question Sam and I ran into was simply do we give the core devs the status field itself or do we give the core devs their own preamble to keep track of their own governance.

**Danno**
 I'm in favor of reducing the scope of core governance so letting the topic groups decide their own status thing is in line with that general principle that the central groups are doing less and less is giving more and more power to the topic groups, so I would prefer that core devs get to do what we want with the status groups you could say like well you need to categorize these in some mutable and immutable states that would be fine, and propose a process for resurrecting abandoned and rejected stuff, but I would very much prefer that topic groups get full control of their status.

**Sam**
Yeah I think Greg's proposal is whether so if let me set this up Greg and correct me if I'm wrong but you wanted to have two fields one that was for editorial status and one that's for whatever the working group wants to use for their their progress tracking right?

**Danno**
And The Proposal I recall sing at one point had the mutable and enemy of the fields and you would just map the topic group ones to an editorial figures from that and that would be the task for the topic groups it's establish what that mapping is. The real concern about editorial status is is it mutable or not.

**Greg**
Not really, I don't think. The it's up to the working groups of mutable and immutable is even a concept for them, from the from the editor's point of view the statuses that really matter are draft, final and final doesn't really matter to us until after an upgrade really, if the editors want to make it go final before an upgrade fine but we're not concerned, we 

**Danno**
Okay so if it's providing a list of states that map to immutable and immutable if the topic groups map their statuses to draft a draft status in the final status then we don't need the editor status because we can map it into the topic group's workflow brought 

**Greg**
Everything in between draft and final is up to the core devs and the question is simply do we let the core devs use the existing status field or do we give the core devs their own preamble, in the header of the document there's an extra preamble that a working group can use to put any fields whatsoever that they need.

**Danno**
Yeah and I just want the one status field I don’t want two status fields so let the topic groups control status.

**Greg**
and if you want to add other headers then what?

**Danno**
You can add other headers for topic group um but to have like a header that means two different things between core governance and topic of governance I think is sort of friction that'll result in problems.

**Sam**
Yeah I think um so the way I had originally written this up is the first seven Fields I think were fixed and that was like the data was created the authors who can edit the document what topic group it belongs to there's a few of these fixed ones but then anything after those first n number of them uh would be totally up to the topic group

**Greg**
Okay what I was seeing on the status field is that from the editor's point of view it goes to draft and it stays draft until it's final. From our point of view it's a draft and it's subject to change all along from the core dev's point of view it's going through a sequence of changes that the editors don't need to care about and while things are so I don't know it at that so that is very confusing and it's I think helpful for the editors to know that and it's pretty much just a tooling issue as to how that gets displayed on you know on what is it eip.etherium. It just creates a separation of responsibilities um so we're not having to oordinate it all on that 

**Danno**
So what if uh the topic groups had a naming requirement to say that if they had if that the last word in their status needs to be one of draft or finals so they could distinguish at the glance, so we have proposed draft on CFI draft EFI draft test net draft uh main net final so that way from one field you can get
both informations or you could require that they have every topic group  have a final state and their final state is final and it might be final Dash rejected final Dash implemented final Dash mainnet and everything else is draft.

I think with with two Fields you're going to get too many conflicting States because the topic group statuses really should map into this is either a draft date or a final state and it's going to reduce it's going to result in people messing it up. So maybe we could even in there is no course data that the editor that the authors put on is something that the regulars put on when they render it onto the main page, so we could put the mapping inside of the logic that there's a sort of EIP logic that Panda's writing.

**Greg**
Yeah I'm not sure if we disagree here I'm tired and and there's lots of details and that's part of why it's not in this document is because there are details some some of the ritualing details some some of them are just my desire to somehow dissociate this as much as possible so that the core devs and the editors do not need to coordinate um on this stuff and also that the ietf pretty much gets by with everything either being a draft or an internet standard. That's that's it from the publication.

**Danno**
But we very significantly from the ietf that's why I want to call these topic groups instead of working groups because we don't do anything close to what an ietf working group does we don't assign an editor um we don't assign a chair we don't make the chair responsible for writing it it's not a large group so it's quite different already from ietf which is why I prefer things like calling in a topic group to make it clear that we're not confused with other processes well 

**Greg**
Google topic group and Google working group under topic group you'll get nothing that makes any sense under working group you'll get all kinds of different working groups and all kinds of organizations. Working groups are people who get together and organize themselves to get some work done topics are just anything you can talk about the core devs are organized to work on a task um how they organize themselves is not the editor's concern. 

The editor's concern is just is this a document that's still subject to change
or is it a document that is no longer subject to change. I think that's the
only thing we care about. This is not a hard it's not like I'm hard and fast on this it's just a detail we sort of need to resolve and mostly I think the editors can resolve it, but I don't want to be in the way of the court of developers or mess up their process with this.

**Danno**
So I think we just provided simple mapping every topic group or working group whatever the call just say this status maps to this data in the core draft final hierarchy and then we can automate it with tools.

**Greg**
Something like that yeah.

**Sam**
Works for me.  All right I'm gonna hop off I have another call um thanks for the good discussion on this I appreciate it.

**Greg**
Sam are you pretty  sure you understood what Danno said? I'm too tired at this point.

**Sam**
 oh sorry go ahead 

**Greg**
I was up working on zkevm stuff with a mathematician in Australia until 4am.

**Sam**
Sounds like a fun evening but uh yeah my understanding is that Danno wants to have a file somewhere that says uh you know on the left hand side the name of the status and on the right hand side a Boolean indicating whether it's a draft or a final and then each working group defines that file 

**Greg**
that they can do what they want yeah 

**Pooja**
Perfect details of it maybe in the future in the few things but for two days I think we are all on the same page we are going ahead with this split and things are being sorted Sam has dropped off I don't know if there is any future call with respect to that uh proposal if there would be I'm hoping that the announcement would be in the Discord Channel thank you everyone for joining us today have a good day thank you.

## Attendees
* Pooja Ranjan
* Sam
* Danno
* gcolvin
* Victor Zhou
* Gajinder
* Juan
  


