# EIPIP Meeting 77 Notes
### Meeting Date/Time: March 22, 2023 at 14:00 UTC
### Meeting Duration: 54:01
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/219)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=NQTjeuM4T2Q&list=PL4cwHXAawZxpLrRIkDlBjDUUrGgF91pQw&index=1)
### Moderator: Pooja Ranjan
### Notes: Metago

## Summary

Summary | Description
-|-
77.1 | [New contract interface and EIPs should be required to include a privacy considerations section ethereum/EIPs#5682](https://github.com/ethereum/EIPs/issues/5682). No consensus reached. Issues will be discussed further in the issue section and Discord. 
77.2 | [Website: more rss feeds ethereum/EIPs#6579](https://github.com/ethereum/EIPs/pull/6579). Approved.
77.3 | [https://ethereum-magicians.org/t/discussion-of-criteria-for-advancing-eip-status-a-straw-man-proposal/11995](https://ethereum-magicians.org/t/discussion-of-criteria-for-advancing-eip-status-a-straw-man-proposal/11995). Continue the discussion on how to create a guideline and its content. 

# Introduction [0:00](https://www.youtube.com/watch?v=NQTjeuM4T2Q&list=PL4cwHXAawZxpLrRIkDlBjDUUrGgF91pQw&index=1)

## [New contract interface and EIPs should be required to include a privacy considerations section ethereum/EIPs#5682](https://github.com/ethereum/EIPs/issues/5682)

**Pooja**
Welcome to EIPIP meeting 77 I have shared agenda in the chat the first item listed here is new contract interface. An EIP should be required to include a privacy consideration section. I believe we discussed this in the past I should have mentioned it in the section too, but recently it was requested by Victor to maybe have more discussion on that. Victor, if you would like to maybe quickly recap and why do we want to have it here for discussion today?

**Victor**
Yeah so I think last time I was not there and the question here is that if we have something other than privacy consideration where do they go. It seems like current status, current layout is quite rigid. I'm proposing that we have several options, either have a privacy section, independent ones or have an other considerations by itself as an section as a fallback catch-all. So that's generally the idea. 

**Pooja**
All right. I don't see Sam on the call but if I remember correctly I guess he wasn't in favor of having a privacy consideration as a part of EIP. I wonder what are other thoughts that the present editors today 

**Lightclient**
Yeah I'd also rather not have the section. I thought we'd discussed this a couple calls ago so I don't know why we're like rehashing old things. 

**Victor**
My proposal is to have a other considerations as a catch-all. 

**Lightclient**
I think the sections are adequate right now.

**Victor**
You mean others consideration is added now?

**Lightclient**
No. I'm saying the sections that we have currently are adequate at the moment.

**Victor**
So we know that it's on…it's not all EIP need a consideration for privacy but if someone needs a privacy consideration in some of the case what's the best section to go in.

**Lightclient**
The security considerations.

**Victor**
That is what I know is not the right thing to do because a lot of non-technical and people consider security the same as complete security and privacy and we as a standard body, especially in the crypto space, I feel that is not a good example to set up that we would probably ask people to put privacy into security section. 

**Lightclient**
I mean ultimately this is a Blockchain and there's not much privacy at all, so I think that anytime there is, you know extraordinary scenario of breaches of privacy, this would fit perfectly in the security consideration section. 

**Victor**
What do you think if we increasingly see incoming protocols or bystanders addressing ZK privacy preserving scenarios, in that case do you still consider that as security space?

**Lightclient**
I mean we'll see if that happens but I don't think that most Proto most ZK protocols need to make EIPs about their ZK protocol and describe what the privacy is are of their protocol 

**Victor**
My question is what is preventing us from having other consideration as a fallback. What is the argument against that, like, are we predicting that our section will never be needed and in a first one that needs to miss it and will never appear.

**Lightclient**
I mean for first like I don't want to have a section that's just extremely generic that people can use to mean privacy that people can mean to use to some other type of consideration. Like so I don't think that having just a catch-all is a good idea and second so I don't think that we should be changing the EIP format right now, it's like something that again and again editors wants to change this process but it's not being requested really by users of the process. Whenever we start seeing tons of EIPs putting privacy considerations in the security section and they're telling us this doesn't make that much sense then we should consider changing it, but like I don't think that this is a good idea to just keep proactively changing this process.

**Victor**
So this was from authors. This was a request from the author. That’s for one and second what are other possible considerations that you will worry people…

**Lightclient**
This person isn’t involved in the EIP process, this person is involved in the IETF process, yeah he might also be an author but it's you know something that somebody who's already involved in processes is trying to change.

**Gcolvin**
Once upon a time and not that long ago, people keep telling me things have changed and really has not been that long authors were allowed to put an appendix, more perhaps possibly more than one appendix on our proposal so there was a place to put things that were important to discuss but did not exactly fit one of our predefined procrustean backup. People know what a procrustian bed is? 

**Victor**
I don’t know

**Lightclient**
I don’t remember. When we had an appendix so I'm guessing it's been at least two or three years…

**Gclovin**
Gee and that's like a century right? Haha! It's a pretty common thing in documents to just let there be an appendix it's you know other considerations call it what you want but it's an appendix and then the author can lay out important material that doesn't fit our procrustean bed that's it was a Greek myth about somebody who ran a roadside something and I forget all the details but it was sort of this bed of nails I think that he you had to lay in the bed and if you didn't fit you would be scrunched or  scratched until you did fit.

So somewhere in the format it's good to have it come all out rather than get a bad EIP where someone scrunched something into a section it didn't really belong in and then later say oh well we've got this stuff put in security systems, it really isn't a security issue and now we have these fat EIPs where is it we have oh some of our EIPs are showing up with appendices about privacy um and maybe we do need a privacy section I didn't think we really did until I saw it a long list of EIPs and particular considerations I hadn't thought of so clearly there are EIPs for which there are privacy considerations and for for some of them they actually are security as well so yes for the ZK for the ZK stuff it's a lot of it's all about maintaining privacy and if they fail to maintain privacy in a ways that they're supposed to it's a security problem but it's not exactly the kind of security problem that we're usually dealing with so it is confusing I wouldn't bind a non-normative privacy section I'm not quite sure where to go with that and so I'm really happy to just say that yes there can be an appendix but in general when we put this process together just a few years ago over and over and I can't find the logs because we did it on Skype and it evaporated but over and over it was, these are strong suggestions, as the EIPs come in yeah we can loosen up the format for any given the EIP to fit that EIP better and that eliminates a whole bunch of arguments about changing the format in anticipation of stuff that hasn't happened yet but anyway I'm rambling. 

**Victor**
Yeah thank you Greg and then I agree which correct in that I've seen at EIP consideration comes up in some of the cases I'm I felt resonate with a lot of other editors that's it's not generally needed so I okay for it to be it a optional ones I also pasted the Google search as well as in our Discord channel for you to see that EIP ERCs and EIP that has mentioned privacy in their text. Examples includes restricted Ethereum provider API and just injection for EIP for privacy consideration um app keys and application specific quality contracts including author by Dan Finley and also steals addresses that is recently a topic as well so this scenario has increasingly seen that uh some of our EIP especially ERC side has touched has changed some of the perspective about potential use cases for privacy professional considerations about quite privacy and once that back for me is that we as editors provide an uh format in order to make it more consistent and useful for the authors to use but we are not there to dictate what information is should be included and what information should not be included by the format itself. 

The format serves a purpose and so that's why I'm arguing that one consideration could be useful to give authors more leeway because I still experience carry a lot of memory when I'm authoring a lot and the rigid format has make it very hard for us to provide the full information about this. Something like adoptions existence adoptions are also considered can be put in that other considerations.  

**Pooja**
Okay I think I mean like what I'm getting from the whole conversation is obviously there is a strong recommendation of having a section for other consideration at this point of time however people think that it would be a good idea to have a particular example in mind like if we are struggling with any proposal if we have a proposal to be like struggling with adding the information, I think that way it would be better for editors to weigh if we really need this thing and making the policy change in advance that can be abused if not properly explained to people, can be a threat. So uh what do you think Victor in in this case like uh as we kind of are discussing that there could be a proposal let's wait for a proposal to be like that and have it discussed maybe on issue section and then probably in the future meeting?

**Victor**
I shared in a Discord there are more than 10 existing ones date back to ERC 1385 mentioning about privacy and privacy is a strong it's important consideration I don't know what our other new EIP ERCs or are we just ignoring that this has been unless a need from a from EIP all together back but for such a long time.

**Sam**
So my biggest argument against this still is can someone give me an example of a  privacy concern that isn't also a security concern?

**Victor**
So privacy is usually depending on security so when asking that question it is very hard to kind of get you out of context answering. Okay but uh it's important that we don't conflate them that's why I think me and then a bunch of other authors could thinking 

**Sam**
My argument is and I wouldn't be all privacy concerns are a subset of security concerns and should be a subsection of the security consideration section…yeah.

**Gcolvin**
All right, it's not that simple it that is some cases on a blockchain the fact that everything is visible is the whole point. It's not the check is in the mail it's the transaction is on the
blockchain and there's no arguing about it everybody involved can look and this is a feature. Other times it's a problem and people are inventing technology to do a better job of that and people are inventing whole blockchains and other technology that is much more and sometimes almost completely private, so it just seems for some EIPs it
actually is a security concern and needs to be handled there and I think that would then show up in the motivation that that these privacy concerns are part of the point and if
they fail it's a security issue. Then then there's this middle ground where things have privacy implications that nobody thought about but they really are important and
so an optional privacy section does uh yes motivate people to look at that. In those cases where it matters in other cases it doesn't even the security section sometimes yep I just sort of scratch my head and go um there are no implications here except
the usual ones of, you know, there better not be bugs here. Sso I kind of go I kind of go on circles on this, I see the points but I just keep coming back to the appendix, further discussion not just an optional privacy but just some sort of optional section that people can use for these sorts of things that come up that sometimes are important, only one EIP where people can put discussions of things that are important that don't fit our very rigid format and really the entire item, yeah the ietf going all the way back and the IETF was very much a model for what we were doing their formats are nothing like as rigid
as what we're trying to do. There's just a lot more freedom given to the author to present their material in the way that the author and the working group believe is best so if we're going to have such a rigid format we need a little bit about if we if if we feel the dependencies should be forbidden then something you know just optional optional further or discussion section something like that privacy is just one one such aspect that comes up…

**Lightclient**
I would love to have a less yeah you know rigid set of sections. I think that the way the
IETF does it is a you know ideal in a lot of ways the reality is that we have a lot of people who are able to and wants to permissionlessly create EIPs and so that ends up creating a lot of noise for people to you know search through and try and edit and if we were having the type of quality and the type of contributors of the IETF is having, I think that it would be okay but we we don't and so…

**Victor**
Can we have an example of what could go horribly wrong when we fallbacks given currently we're very rigid in blocking links what are other concerns that could be abused in in this section. People can still put things in specification right like they can put some random things there what could be worse…

**Lightclient**
It's also about frustration and fatigue of process change, like at this point I don't know there isn't really anybody who still enjoys being a part of this process because of how much it changes under their feet and just adding more and more things like this is not for the vast majority of people who need to create EIPs it's not something that they're happy with.

**Victor**
I think people so speaking of myself as an author what I and other authors that I see frustrated is adding restrictions and I haven't heard any authors complaining about having flexibility more flexibility was as what they complained. Maybe I don't have the historical context and maybe editors will be very trained for new flexibilities but I would love to hear what could be very bad in this case from an editor's perspective.

**Lightclient**
I mean we've already gone over it's confusing it should be part of the security considerations it's not something that's super important for most EIPs and erases so it just doesn't need to be a section we don't need to change this aspect of it and I feel like
we just keep debating in there's no progress but it seems like Sam and I have both said that this probably doesn't need to be a section we talked about it on another call and that was the outcome we didn't feel like it should be a section and I don't understand why we just every EIPIP call go over rehash old arguments. I think uh Greg and I are here today providing more of the author's side of the um of the of the feedback uh and
then our general concept idea is to have flexibility and you mentioned that you want to have more flexibility and you haven't I haven't heard by the way the arguments about
what this flexibility more flexible section could help could could bring wrong with it the only argument I currently heard is that we don't want change and it's uh I think Greg also answered already about the argument that privacy is not always security sometimes privacy, the the features it's just a it's a feature so sometimes it's a problem then just by secure design but it could have a privacy implications. These are examples that why we feel that security section considering section is not enough and I haven't heard about a counter argument about having other consideration works here further discussions other than we are tired of have seen changes and which I think…

**Lightclient**
I've already gone into the other arguments like it doesn't make sense as a separate section from Sam and I’s point of view it's something that should live under the security consideration section.

**Victor**
And I guess in that case is that…

**Lightclient**
Most EIPs don't need this section.

**Victor**
Well what about having other considerations because just like diversity not all of the eips need this particular consideration…

**Lightclient**
I don't think that other considerations make sense because I don't think it makes sense to have just a catch-all section to put whatever authors want to put in.

**Sam**
Yeah 

**Gcolvin**
I think I strongly I strongly think authors need a little bit of an out. If you're going to have a really rigid format yeah it's instead people stuff stuff into motivation and rationale that doesn't really belong there but you got to put it somewhere or else you wind up, macaw is gone unfortunately but we went through this with a long-running EIP where you know the rules kept getting tighter and so my EIP kept not yeah I had to keep rewriting the editing to beat the new rules which yeah 

**Lightclient**
I mean that's extremely frustrating like having to update your EIP as the rules change but and I look I mostly agree that we should have an out. I don't think we know how to do it properly and I don't think that having a generic out called other considerations is the right approach. If we were to do an out I would rather it be some sort of ad hoc
situation where someone says I need to have a top level section that says this and we approve that as something that is added to the EIP. Right now it doesn't feel like we have the manpower to like actually make that happen the way that we have this continuous integration setup it's not easy and we have a lot of junk just coming in from authors where they don't really care about the readability of their EIP and so they'll just do whatever they feel like doing so I just think that like the rigid system we have is kind of the best the worst best thing that we've come up with right now. 

**Gcolvin**
Wait a minute for centuries in the publishing world you have appendices that that's where you put stuff that doesn't, you know it doesn't fully fit the flow of the document, it's not the usual format it's definitely…

**Lightclient**
…don't think they're privacy considerations should be something in an appendix like if it's important…

**Victor**
Then it should be the main body but…

**Gcolvin**
The point is that should be it's a place it's a place you put things that don't fit the current format. 

**Lightclient**
Right now we use…

**Gcolvin**
…time pardon?

**Lightclient**
I feel like we use we use link we try to link to things that don't fit the format like generally my experience appendices have things like something that fits outside of like the narrative of that document so it might be oh you refer to some hash function here in the appendix you can read exactly how that hash function is implemented or something of that sort and for that or just use hyperlinks.

**Gcolvin**
But our link you can't link to almost anything. Where are you supposed to put what you linked to? Plus…

**Lightclient**
 You have a process for adding links.

**Gcolvin**
That's a of a lot of work.

**Lightclient**
 I think it is I'm not saying that this is process is great but this is the process that we're kind of ended up at and we can't just change it every three months.

**Gcolvin**
No it's easy to lose…tightening it up is a pain loose you know relaxing a restriction that got put on…

**Victor**
Right.

**Gcolvin**
…is is easy…

**Lightclient**
…optional manage all of the Bots 

**Gcolvin**
…an optional further discussion section just any sort of optional thing at the end, where the author can put stuff that…

**Lightclient**
I strongly disagree with having a catch-all section whatever its name is I think if they're going to have additional sections that aren't part of the like ordained set then they should be named and they should be specific to what the author is trying to convey.

**Victor**
And then I think you're proposing that this section will be one-off exception what ad hoc approved if I do I understand it correctly?

**Lightclient**
I'm saying I don't think that right now we have the ability to actually pull it off.

**Gcolvin**
Okay I think I’m partly reacting to my experience of the death of 2315, which was probably the right decision given that it motivated EOF but was personally very painful and part of the pain was that appeared that a lot of people on that call some of them had never read the EIP and a lot of them apparently had read nothing but the EIP despite the links to other things to do so to the extent that you can't get everything important in the EIP you're really making it difficult. You know we've got a hard link policy and then a hard format and then it's like we'll put it somewhere else but where do I put it that I can link to it and will people bother following the link. If you have an appendix you give it a name, you just say you can add some name sections at the end
um I just I'm not I'm not I'm not seeing that the huge objection here yeah it yeah dot I'm not seeing it creates a whole lot of extra work I think it's easier to have a section at the end than to have people squeeze these things into sections they don't belong in and then you're going well this isn't really motivation, this isn't really rationale, and then it's like well okay but where do I put it…

**Sam**
I think the uh the opposite is probably the bigger problem where you end up with motivation and rationale in this third section and we have to tell people to move it into where it's supposed to be but I mean, it I guess I'm not as opposed to a generic
section as I am to a privacy consideration section but I don't want to give authors more freedom because like it's already hard enough keeping them consistent like as it is.

**Gcolvin**
We're driving authors away because it's too much trouble so I people wind up putting
out hackmds and then it's like will somebody please tell me where the latest hackmd is for this proposal you know and it's like…

**Lightclient**
I mean the people who have to make EIPs are going to continue making EIPs and the people who don't have to make EIPs it's a little bit harder for them to convert what they're trying to explain into the format that's probably a win at that stage 

**Victor**
I think I think that's uh that's I that's not the case we have seen Nick Johnson move to eip-e-n-s-i-p we have seen uh fallbian uh moving to use um locksco uh IPS without updating 71725 we've seen 

**Lightclient**
…started this chain a long time ago like, he's not involved with Ethereum really
to change its protocol.

**Victor**
We have seen Dan Finley and uh and Rick Mall complaining about EIP process that make it very hard to drop the EIPs and giving people more freedom gives us more authors basically. It's very hard there's always a spectrum of authors who are here to contribute to EIPs who are not here to contribute to you who have to do EIP here anyway but uh as a standard body I feel that um we're here to serve the authors and and not there to kind of think that how to make it only easier for the formats and that's why it's I'm proposing to give this more flexibility and I do understand that you personally don't want to give to add this that are the considerations and Sam doesn't and then Greg and I are in favor I think we can we might not have consensus today but we can see how the consensus can move forward and obviously EIP is not only done by authors. I strongly believe that the stake the major stakeholders are actually authors and adopters so how about we summarize what our each believe individual beliefs are and then put it out there for authors and other stakeholders to come in. I don't think we should be dictators or dictator groups in this space and if no one starts authoring EIP or adopting EIPs then basically rendering EIP programs worthless so how how do you like that we just put down what we believed so far and see in the don't active with other people's inputs can we kind of converge into consensus and it's okay to take a longer discussion maybe three months, a year from now to see how this evolved into?

**Pooja** 
Sorry to interrupt here I think we are completely moving into a different direction we need to come back on the track so we can probably take a look on to the other issues or the topics that we have we are here to discuss but just for this particular topic it is obviously clear that we do not have a consensus, we do have four or four editors on call and half of them are in favor and half of them are strongly not in favor, but the proposal I mean we do have option of appendices here people are thinking of what can be in section that can probably provide authors this option to write this but I believe when we are talking about standard, the flexibility should also have a limit to it. And we cannot say that we are like distracting authors because the number of proposals every month we get is a way more than it was earlier and the numbers of proposals that dies in stagnant status is like a really huge number so we really do not have to have a lot of proposals just getting in for the purposes of editors to keep on reviewing with a lot of sections added, and if needed on case to case basis this can be like you know addressed. I would highly recommend uh discussing this issue further in the issue itself because we do not have a clear consensus on this call, and uh yeah any final comment? Anybody would like to like suggest or say just to wrap up on this topic so we can move ahead with the rest of the other discussion issue?

**Gcolvin** 
I better not start or I'll go on for 10 more minutes.

## [Customizable editors ethereum/EIPs#6650](https://github.com/ethereum/EIPs/issues/6650)

**Pooja** [32:30](https://youtu.be/NQTjeuM4T2Q?t=1949)
Okay in that case let's move on to the next one I think that is the best option to move on here. I think the next topic that we have is about customizable editors. It's proposed by Pandapip and it's a proposal for enhancement. It says that in EIP review bot currently there are predefined editors group depending on the type and category and he is trying to propose a stopgap solution before implementing tags that we have a slightly more customizable editor list for peer reviewers wonder what people think about it.

**Lightclient**
…understand what the what the goal is.

**Sam**
Yeah same I don't know what like if you don't have tags how do you narrow down the list more so that's why I posted my comment.

**Pooja**
I think the next number I mean like the next not exactly the next one. There is another proposal that is coming up for ABC so the number is 6575. If we can probably take a look there, I think both are kind of interrelated and it's also suggesting of an intermediary EIP role here, not exactly what bot would be doing but kind of a role that can be useful if they are not completely editor. I'm sorry if I have mixed two things please correct me over here.

**Gcolvin**
Stopgap… is this really needed? I thought GitHub already made it possible for any given EIP to you know market that that you know any particular person's approval was needed to to move it forward in the system.

**Sam**
So unfortunately only people with the write access to the repository can be requested as reviewers um so that's what so the EP review bot kind of handles that for us. Yeah it's dumb.  You can't like you can't request Greg as a reviewer because you're I don't think you have write access to the repository?

**Gcolvin**
No that's just that's a sore point but that's a different one yeah 

**Sam**
Yeah that'd be great if we could do that but we we kind of work around it but this…

**Gcolvin**
…is my write access was taken away accidentally then it was never given back you know which actually sort of demotivated me demotivated me from…

**Sam**
I completely understand that, yeah…

**Gcolvin**
…but I can't get when something's broken then I have to wait a day or two for some other editor to will you please force this in? Anyway um I'm still not sure it still takes one of us with write permission to finally get things like from one stage to the next so I don't does this need to be so formalized? 

**Pooja**
Maybe we can wait we can wait for the proposal to provide more context of the proposal, I see comment from couple of editors saying like what this exactly would look like and what is the proposal, sorry um Greg if I interrupted please go ahead.

**Gcolvin**
No problem. All right so it sounds like there's just technical issues with how the GitHub process works and I'll leave it at that.

**Pooja**
Yeah probably uh panda is uh looking into a lot of changes around bots so yeah it's related to GitHub processes my understanding as well. 

**Gcolvin**
So the important thing is just making it possible to get reviewers for particular proposals in, so we don't have to be trying to bringing in more editors in general when for any given ERC there might be very few people who are actually interested and for any given person who might want to edit, there might be very few ERC's that they're actually interested in.

## [Upgrade to Mend/Renovate from Dependabot ethereum/EIPs#6588](https://github.com/ethereum/EIPs/issues/6588) [37:20]( https://youtu.be/NQTjeuM4T2Q?t=2240)
Right all right moving ahead with the next one which is Upgrade to Mend/Renovate from Dependabot. I already see some comments here from one of the editor. The proposal here is to allow opening PRS to upgrade CI components and provide some more information on what changed. Anyone particularly have strong opinion about it, looks like it's another enhancement proposal?

**Sam**
Yeah, these are just technical bot changes so I don't think most of the editors will care.

**Gcolvin**
Yeah.

**Pooja**
You know I mean it's good that these issues are mentioned here and we are also bringing it up in the meeting so people who may have concern who may have thoughts or maybe even some suggestions for a better enhancement, they can come forward and probably add their thoughts here so yeah I think it's a good one that it is being created as an issue to be discussed in the meeting.

## [Website: more rss feeds ethereum/EIPs#6579](https://github.com/ethereum/EIPs/pull/6579) [38:23](https://youtu.be/NQTjeuM4T2Q?t=2303)

All right moving on to the next section discussion continued from the earlier meeting. Okay, in the last meeting we discussed about RSS feed. Looks like a lot of conversation happened after that and currently when I checked last, it was approved by Panda. I wonder any editor has any strong opinion on this one or can we go ahead and merge this PR.

**Lightclient**
Seems fine.

**Victor**
No objections. 

**Pooja**
All right I think I don't know Sam, Matt, either of you can may be able to merge it, like whenever you get a chance it's not needed to be done right now, yeah if you don't have objection on that.

**Victor**
I have a question I didn't ask like well can we or what happened to Greg's write access and who is the right person to talk to to get to fix that.

**Gcolvin**
It doesn't matter anymore, not immediately but over the next over the next month or so I'll probably need to be backing out of this because a startup I've been working on has has gotten funding and…

**Everyone**
Congratulations!

**Gcolvin**
I was talking to Pooja before we came on. It's a project involving a dam in Paraguay. It's the second biggest hydro facility in the world and it makes more electricity than anybody knows what to do with and so we're probably going to use the Ethereum blockchain plus some new blockchain like technology we've added to set up a computational  marketplace to usefully suck up that power because their legislature doesn't want the power used for Bitcoin mining and it's so it's going to be really cool but you know how startups go, it'll it's basically going to be every waking hour for quite a while.

**Pooja**
Well congratulations Greg and just to answer Victor's question, Victor I think this is the like the access is attributed whenever a written needs that that is there whoever is actively editing they have these accesses so probably it's better managed right now and as Greg mentioned that he is totally fine with it so yeah I think we can move on.

## [Config: Add @abcoathup as ERC/Meta/Informational editor ethereum/EIPs#6575 (comment)](https://github.com/ethereum/EIPs/pull/6575#issuecomment-1461055801) [41:10](https://youtu.be/NQTjeuM4T2Q?t=2470)

The next one here is again yeah the contributor, he cannot join the meeting because he lives in Australia he said that unfortunately it's not possible for me to join but he requested to take a look at comment 6575 and he is keen to give this a trial ERC editor run. I wonder what people think about this proposal.

**Lightclient**
I'm generally in favor.

**Sam**
 I'm fine with doing a trial period getting them to do like maybe let's say 30 days of editing and then when they run into other editors just get them to note the comments and make sure they're doing good work and then if they are then we can add them as an editor 

**Pooja**
I think so but uh curious to do this trial period other than notification that he or she is engaged in this trial editing does the individual need any kind of special permission access or anything in general?

**Sam**
Nope just leave comments as if you were an editor and that's about it. 

**Pooja**
All right. So…

**Victor**
What's our well I think the app that's the name I guess mentioned that he's only interested in signing numbers and not kind of generally editing the content, is that the case or do I understand…

**Lightclient**
I think we talked about it at the last call that if all he wants to do is assign numbers that's not really something we would be open to accepting right now but if he wants to   generally edit and it's only like 30 minutes an hour a week then that's something that we would be interested in trialing.

**Sam**
He said about 30 minutes a day and could do you know number assignment guidance on how to comply with the automation typos but not technical stuff which sounds right.

**Pooja**
Yeah.

**Lightclient**
That's what I thought.

**Victor**
Yeah generally you can you can start editing and then and you can read to your review um feedback and uh I would love to see the work and work for more with him to be able to comment on this as from the reviewing side. Yeah it's not I don't think we need a
official kind of trial kind of thing you can we can we should promote a idea that anyone can come in and provide a review help will provide editorial support like this this should not be feel that they have to ask for permission for us to do that, so long as they are providing useful feedback they can always contribute that and then yeah, so I don't think they actually need any program or approval from this group, and then obviously which it's our job to kind of identify those who are doing really good and active and to invite them onto the editor groups and to be an official and bear some duty after like the responsibility yeah afterwards.

**Pooja**
Generally I agree what you are suggesting here Victor, like anybody can do these things but I really appreciate this individual notifying us because when someone is making a special notification of that, then there are more eyes to what's there you know review
comments and everything else probably he has in mind I don't know for sure, like maybe he wanted to be an editor in future, which is which would be good for us and having this notification is helpful, but definitely it is open for anyone to come and provide feedback.

**Victor**
Yep.

**Pooja**
So all right I and I think from this meeting we can obviously communicate it to the individual that he should be good to go and let's start this 30 days trial period from here on.

## [https://ethereum-magicians.org/t/discussion-of-criteria-for-advancing-eip-status-a-straw-man-proposal/11995](https://ethereum-magicians.org/t/discussion-of-criteria-for-advancing-eip-status-a-straw-man-proposal/11995) [45:27](https://youtu.be/NQTjeuM4T2Q?t=2727) 

All right thank you. The next one here is Ethereum magician discussion of criteria of advanced EIP status - a straw man proposal. I think we also discussed this in the past but I guess it was requested again for today's discussion by Victor. Yeah Victor we have 10 minutes if we can quickly like have a small intro for the past and what changed since then to have it discussed in the in this meeting. 


**Victor**
Yeah I just want to share a light on this strawman discussion. Maybe people are not like fully agreed but I just want to kick off some discussion about questions I usually I get asked by authors is that what is needed for advancing to the next status of the EIPs and it's pretty subjective up until this point and we see people saying like oh we need to wait more time or we need to have more good quality but like what is an or good activities on using on on forums that it might be helpful for us to kind of formalize what is like and so that's why I put down this proposal to kick off the discussion and just want to get it out of the temperature in the room and see if it's either something that we couldn't explore or not in favor at all, or like maybe not so soon and we should discuss it like, come back six months later. Pooja, do you have link in in that and you put it in so it's easier for people to click?

**Pooja**
Yeah I just shared. 

**Lightclient**
So what is the outcome of this thread that you're hoping to see happen?

**Victor**
So the outcome is that we identify the specific need for ERC’s interface Network and core, like core already have a very defined way to finalize right? But what about other things, do we just let people move it to final or can we say that you will have to have this discussion and implementations to move to final, if we want to have any quality control that is not arbitrary by subjective matter in editor’s heart but also a kind of but uh but have a concrete bar of quality control, that's basically the idea.

**Lightclient**
I generally want to avoid concrete bars of quality control, like some rigid guidelines about when things should move. I'd rather it be generally something that we can, you know just do as we feel is best as editors, but I like having guidelines so that authors can have an idea of what is necessary and what is expected, like that seems useful, but I wouldn't want to frame this as if you do this then you're barely over the bar and you get to move to the next level.

**Victor**
Hmm, I'm in favor of having guideline too and it's fully okay that is, does not become a mandatory thing but a guideline. Is that a good understanding and good consensus?

**Lightclient**
I think so.

**Victor**
Cool then the next step is what type of guidelines that we, that we think in and this one is like strawman proposal to see if you have suggestions to advise to change.

**Sam**
So I think the my biggest problem with this particular proposal is that we can't really verify that implementations are independent right?

**Victor**
That’s true.

**Sam**
…so I don't know like the author could just make three accounts implemented three times and then there you go it's done and setting barriers like that doesn't really help very much.

**Victor**
That's true, that's totally true and then I think that's why I feel that Matt's comments on, that's make it a guideline, not just like this is how you do and then you advance um so we, there's still we can still give them like visually, or we should still review them anyway right? But uh I'm in favor of and if you don't have implementations like it's not
useful like, I think last call or finals should pretty much kind of guideline that you should at least have yourself and then one other which we might not be able to verify, but at least implementations, like we both agree that it's possible to do civil attack by creating implementation by themselves, multiple ones but when I'm, if I'm not clear is that well I think that if no one's if no implementation or no two implementations that is that is not seeing a good use, a good place for a standard to be in.

**Sam**
Yeah like I think if we had a guideline like that, I would have a much easier time telling people no you can't standardize this because you have no one interested in it and like I would like to do that more often. I'm just not entirely sure that this is a strong enough
like rule to stand those decisions on. But yeah we can definitely talk about it some more just remind me to take a look at Discord at some point and I'll write up my thoughts on it.

**Victor**
Cool yeah thanks. We I think the conclusion is in favor of continue the discussion and creating a guideline, content to be decided. Is that an understanding?

**Sam**
I think so yeah.

## [Special case markdown-rel-links to help when linking to eips.ethereum.org ethereum/eipw#5](https://github.com/ethereum/eipw/issues/5)[52:01](https://youtu.be/NQTjeuM4T2Q?t=3121)

All right, let's move on. I just wanted to make a quick mention of this PR 6575. I think that needs to be merged. This is already in proposal form to just get that editor added. And we have like a three four minutes left. I don't know, Jose if you would like to quickly give a update about the issue that as mentioned here, do we have any progress or we have merged it? where we are at?

**Jose**
Hey hi thank you. Now just to remind Sam whenever you have the time Mr Sanjos take a look on the pr that's it.

**Sam**
Yeah of course. It looks like it's still failing CI but uh yeah I can take another look.

## [EIPs Insight - Monthly EIPs status reporting.](https://eipsinsight.com/march-2023)[52:50](https://youtu.be/NQTjeuM4T2Q?t=3175)

**Pooja**
Right and that's great thank you and I think that’s mostly all except for this EIPs insight. For EIP’s Insight, I have added all details in the hackmd as well as the website is showing all correct data. We do have five final EIPs. There are 8 proposals in last call for in review and there are 21 stagnant proposals and 9 proposals are added as draft. Please take a look on either on the website or on the hackmd to follow the details proposals in last call. If you have any thoughts on those proposals please go ahead and make sure that you add your comment in the discussion thread so author can maybe take a look before it is moved towards a final PR. So that's all for today's discussion and I know many people have to jump off this call for the next meeting, thank you everyone for joining us today, hope to see you again in two weeks at 14:00 UTC have a good one everyone.

Everyone thanks Pooja. Call ends.

## Attendees

* Pooja Ranjan
* Gcolvin
* Sam
* Zainan Victor Zhou(@xinbenlv)
* Lightclient 
* JA


















