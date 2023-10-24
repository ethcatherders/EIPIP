# EIPIP Meeting 89 Notes
### Meeting Date/Time: Sep 06, 2023 at 14:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/260)
### [Audio/Video of the meeting](https://youtu.be/7lqT8vpm7M4?si=aotx94VnmuAasPMB)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
89.1 | **EIPs:7549** - Revaluate the proposal in the next meeting. Simplify and get rid of the complexities which are there now.
89.2 | **EIPs:7541** - Shemnon has some concerns. According to him, it is great for history but wondering if it is put in as a part of the presented specification, as it might bend room for arguments. | @g11tech suggested the option of having a side pane to improve the EIP reading experience.
89.3 | **EIPs:7541** - A/B testing was also proposed
89.4 | **EIPs:7482** - It's a very lightweight IP protection. At the moment, CC0 does not protect against patents.
89.5 | **EIPs:7482** - Victor will also collect thoughts from ERC authors at AllERCDev meeting.
89.6 | **EIPs:7554** - Most of the editors on the call were in favor of having different rendering websites for EIPs and ERCs. The split will proceed as decided in the earlier EIPIP meeting.
89.7 | **EIP:721:** - Having a policy in place to update Final EIPs will be good to have.

# Intro
**Pooja Ranjan**
* Welcome to EIPIP meeting 89 and have shared agenda on chat. This is issue number 260 on EIPIP GitHub repository. So we have added a few issues to be discussed here today. There would be discussion from past meetings will go over EIPIP Insight and an overview of EIPIP editing Office Hour.

## Dark mode for eips webfront ethereum/EIPs#7549
**Pooja Ranjan**
* So starting with the first item added here, which is an issue added to EIPIP GitHub repository, it is about dark mode for EIPIP web front. I see there are conversation happening. I just wonder if we have any PR for that or anyone would like to. Yeah. Okay. So we already have a PR for it. Sweet. Awesome.
* I don't think anything else on this to be discussed, but. But if there is, please feel free to share. Very well. We can quickly move over to the next one, which is the. 

**Gajinder**
* PR is for which PR is this? 

**Pooja Ranjan**
* 7554. 

**Gajinder**
* I think that is something else. Oh, I think that Lightclient is saying that we. He's bringing it to the agenda. 

**Pooja Ranjan**
* Okay, never mind. We can go ahead and add that. To the agenda, which could be added as the default item for today's discussion. Wonder people have thoughts on the first one. I know there has been a lot of discussion. And it was pulled up by Gajendra Singh. So if you would like to add anything or maybe we are just waiting for. 

**Gajinder**
* Yeah. So basically Panda sort of provided an alternate site that he has been building eip.info, which basically has JavaScript capability and supports dark mode. So. Mean that looks good to me.
* But if you want to add this to our main eip web front for that, I think Sam had a few suggestions regarding enabling it through media queries and CSS, but I think that those are not working, so I'm not sure. 

**Sam**
* Yeah, I can take another stab at adding it. I'm just not super familiar with. The Ruby thing we use for building our website. So. 

**Gajinder**
* But I mean, can we sort of have this that, you know,  we have a website which basically if we do server side rendering with React or some other thing, basically that website can probably also work in links or any other, known JavaScript. 

**Sam**
* Yeah. I love the, the press site that Pandas put together. I'm pretty sure that's all rendered server side. So. 

**Gajinder**
* So I mean, maybe we want to transition to that site at some point if the server side rendering can be enabled and sort of, you know. 

**Pooja Ranjan**
* Now I feel like if we can maybe go ahead and add the dark mode in the present website eips.ethereum.org. That would be really nice to have.  I don't know. I really do not want to put you on the spot, Joshua, but because you are from that team, maybe if you have any thoughts, if this is something that we can request ethereum.org team to have it considered. At some point, maybe. 

**Joshua**
* Yeah, we could chat about it. I don't think it would be too difficult based on the current setup. Just a quick glance. 

**Pooja Ranjan**
* All right, That would be great. So we have an issue opened that is 7549 where we are discussing of having a the dark mode for this. I have also shared the link of eips.Inside.com that also has dark mode. It seems it is something which is like, you know, people like a lot.
* So having that integrated on the original side, Ethereum ethereum.org would be great to have.  anything more before we move on? 

**Sam**
 * Yeah, just following up on this, I think Matt was the one who objected strongly to the week press migration, so I wanted to see if your opinions have changed on that at all. 

**Lightclient**
* I mean, I'd have to look at it again, but I still don't really want to have a complicated site. 

**Sam**
* No.

**Lightclient**
* So it was. 

**Sam**
* The. It's all rendered on the server. It's the same way is so.

**Lightclient**
 * I mean, when you say rendered on the server, do you mean it's rendered whenever you compile it and it's available or is it different? 

**Sam**
* That's my understanding. 

**Lightclient**
* Okay. It's not like rendered server side, is it? It's rendered on demand at request. 

**Gajinder**
* No server side rendering is a concept where the website is sort of the entire Dom is prepared on the server depending upon the path link that the user is requesting. 

**Sam**
* So this one. 

**Lightclient**
* But that's different. 

**Sam**
* Than what. 

**Lightclient**
* Jekyll is. A static site I think is. 

**Sam**
* Yeah, it's statically compiled. Okay. That's what I thought too. 

**Lightclient**
* Yeah. 

**Sam**
* It produces so it's not. 

**Lightclient**
* Server, it's not server side rendered. 

**Sam**
* Correct. Yeah. It's pre rendered and then stored on the server. Yeah

**Lightclient**
* Yeah. We need to look at it again. But like when I looked at it there was a lot of JavaScript code to do the rendering and it didn't look so straightforward. And I mean it's just generally that's not really the direction that I was hoping for the website to go. Like I would like the website to just be very simple. 

**Lightclient**
* The pipeline to be very simple. 

**Sam**
* Yeah, that's fair. Okay, we can we can talk about this a little bit more, I think. I don't want to take up too much time on this call. 

**Lightclient**
* I mean, ultimately, like, if we have people who want this to be maintained and who have experience maintaining it and that we're confident are going to be around for a long time to do this, then okay, I'm okay with it. But I yeah, I mean, right now it feels like Panda is kind of the only person who is really pushing to have this and is willing to maintain it or.
* You know, has that experience. I'm sure that a lot of us could figure it out, but that's not like what my job is. And I yeah, I just don't really have time to mess around too much with like configuring some like JavaScript,  build pipeline on this. Like, you know, enough of the EIP tooling in its JavaScript form has been. Yeah. Figuring that stuff out. 

**Gajinder**
* I can also help. And I'm maintaining because I do have TypeScript JavaScript as well as a React experience. And but yeah, it's, I mean, I can't really commit to so many hours to it, but yes, I can be there to assist. 

**Sam**
* I think there are just more of us familiar with JavaScript now than Ruby. 

**Lightclient**
* I mean, for sure. Yeah, we're not in a great place with, like. I would like to move away from it totally. But yeah, I just want to move to something simpler and not embellished. And that was my take with Cypress. And guess now it's out of beta also, which is positive. But originally when it was proposed, there was a lot of stuff happening and it was like alpha or beta software with a thousand stars on GitHub. 

**Sam**
* So I guess maybe for the next call we can reevaluate whether we want to do this and see if we can simplify it and get rid of all the. Complexity that's currently there. 

**Pooja Ranjan**
* That sounds like a good summary. Maybe we can have it on on the next meeting as well. It seems that there are quite a few people. I see one also mentioned on the chat.  may be able to extend the support to Panda and we have Gajendra Singh as well so we can have more thoughts collected on the issue and we'll bring it back on the next meeting. 

## Embed discussions-to threads on the EIP itself ethereum/EIPs#7541 [9.30](https://youtu.be/7lqT8vpm7M4?t=570)
**Pooja Ranjan**
* Moving on. The next one is embed discussion to thread on itself EIPs. I think the suggestion is coming from Gajendra Singh and Sam also has a added some reference sources by which it can be done, but I do not see any PII yet. Just out of curiosity. Anyone here is opposed to this because as of now how discussion to is is added is just a link provided which is taking to that page. Yes, please go ahead. Now. 

**Danno Ferrin**
* Would that result in possibly some people looking at the discussions and thinking those are normative as opposed to the text of the EIP itself? Because the discussion doesn't talk about the normative. It's the back and forth to figure out what's going on. And it's great for history.
* But my concern, if it's put in as part of the presented specification, it might lend room for arguments like, well, they discussed possibly doing it. Why is it not in there? Versus when you have to go to another website cognitively you're not thinking this is normative now. 

**Gajinder**
* I think the major intent for sort of embedding discussion inside the EIP is that, you know, so when somebody is presenting the EIP or writing the EIP, the summary is generally started from over there. And if somebody is reading the EIP, it's it's basically a good point to actually understand the summary itself so that the rest of the EIP can be followed. So with that regard, I think that that was my original intention that when I propose this.
* But I mean we can have a site pane that basically renders this particular discussion to link EIP inside the web front itself so that the person really doesn't have to move out of the EIP experience of the experience. 

**Danno Ferrin**
* But if you have to refer to other sources, my argument is EIP does not stand on its own and EIP is a document should include the rationale and the motivation without having to go to other sites. And if you need to go to other sites, I would think you should summarize that and update EIP to add the motivation and the rationale rather than saying go read it here. 

**Gajinder**
* I get the point. Basically, we need to also sort of formulate a guideline to how to summarize an EIP, because when I was, for example, asking Lion to summarize any EIP mean this happened on a particular EIP and they said that, okay, you know, this is already being discussed in discussion to this already has been said in discussion to link and that's where the real summary is and mean they are. So again, the question was asked what is the best way to summarize or how it should be done? So that is basically the problem that should be solved. 

**Danno Ferrin**
* I mean, there's a link to the discussion too, in the EIP already.  my concern is that bringing in the text into the EIP, the boundary between the needing to stand on its own and getting the history on it. You can still navigate there from the data, but it's clear that it's meant to stand alone when we don't render the discussion forum in the EIP.

**Gajinder**
* I think if we have the link, then I don't really see what really how exactly it's different if we are just making somebody's EIP reading experience better only. But yeah, so I'm not. 

**Justin**
* Sure that's the case and it feels like we've consciously exercise history from the piece, like the same way that we're not, we're not really big on examples and pseudocode in there because, you know, it needs to be it needs to stand alone. It needs to be implementation agnostic, right? So I think one of the first things that we should decide is, you know, do we need to expand an EIP to include the history and rationale for how we got there?
* I have gotten the sense that we've made an intentional decision not to do that. If that's not the case, then sure, maybe we go down this path. But I think as it stands right now, I'm kind of concurring with Dana. 

**Pooja Ranjan**
* So that is the case. Like we are intentionally not inclusive, including the history, how we reached over there. But just to clarify here, we are not trying to add the text of MEV on the EIP. It's just that the rendering of the page right now, it is it is opening a separate tab and taking us to a FEM page. But if I understand it correctly, what Gajendra Singh is proposing is like we can have it rendered on the EIP page itself.
* People can scroll people if they want. They can click on and get into it to add comments and everything else. It's just that the proper rendering is not there on eips.ethereum.org page. 

**Justin**
* Yeah, I think that's a feature, not a bug but happy to be persuaded. 

**Danno Ferrin**
* Yeah. Feel the rendering it in the is what I object to. So. 

**Victor**
* Is multi-site a option like we can have two competing sites, one with the EIP.Ethereum.org and then other ones could be there providing different features so people can choose their preference preferred one. 

**Justin**
* How do you see that being different than having the link to Eth magicians at the top? 

**Victor**
* It's perpendicular to that decision. So for example, eip.info can have the one that renders it and the renders the one that renders for discussion and eip.ethereum.org can choose not to. And then we can see how people like them. 

**Justin**
* Okay. Thank you. 

**Gajinder**
* I'm good with the suggestion. 

**Pooja Ranjan**
* Maybe. Danno, if you could add your thoughts, because that is against the motion here. So if you can maybe add your thoughts and if that helps any other developer come up with a solution by which they can address the issue and come up with a possible solution to have it. You know, rendered on the website another way that would be nice. Otherwise this could be another discussion point. Yeah. 

**Danno Ferrin**
* There's nothing stopping other random people from forking the repo and rendering it themselves with their own information. I mean, that's the point of it being cc0. You can take the information, you can render yourself.  if we do an A/B test on the official one, you know, we're basing it. It seems like the compromise is, Well, let's just do it anyway.
* You know, when you get the test on without thinking about the purposes of why we're putting it in there is the link is sufficient.
* I mean, it's sure, we can go ahead and do this, but it's it seems like you're just whatever. 

**Gajinder**
* How much traffic do we actually have on the EIP repo to actually have A/B testing? 

**Sam**
* I think the argument against A/B testing is that we're not looking for user feedback here. We're looking for like whether we want to imply that adding comments to the page is makes it normal, appear normative or not. So it's not like we can show this to 50% of our users and then ask them, Oh, is the discussion now? Do you feel the discussion is normative now, or do you still feel like it's not normative?
* Like that we don't have a feedback system that can capture that kind of information. So I think like, I don't think AB testing is going to solve anything here. 

**Gajinder**
* Yeah, but that can easily be solved by a small banner that says that, you know, for the real discussion, you should. Follow the link. Like how we show the banner right now that, okay, you know, go to this particular link for discussion to. 

**Victor**
* So just to clear, I didn't say a AB testing. I think a AB, testing one. Put in test a, AB, testing. My intention is to keep them two separate competing sites. If you're not discussing this, I don't have preference or comments between whether we want to do a AB testing on the EIP stuff.
* But I'm in favor of having allowing people to have different sites just in such as eip.info and then so people can choose to go to eip.info more often when they see the feature there is more helpful. 

**Danno Ferrin**
* That's that's something that would be fine. Entirely separate site not from the the main rendering but a secondary one that people can start using without, you know, it's not be AB tested on the site. We don't force it on them. It's a different way to render the website.
* I mean that's that's fine because you're you're bringing into a separate with context option rather than keeping the normative reference and adding on these possibly non-normative texts with it. If the website is up front that says this is not normative, we're adding other features to help you understand it, then I think that's an entirely different situation than an AB testing. So it's an entirely different website URL, adding this context. And that's fine. 

**Victor**
* Yes, I agree. 

**Pooja Ranjan**
* All right. It is pretty obvious that we have different opinion here. We do not have any PR. And we would like to further discuss this issue on the issue section, GitHub.EIPS so we can discuss this issue on eips.gitHub website. And the number is 7541. Let's move on to the next item added here for the discussion today. 

## Consider adopting a Community Specification License terms for the new ERC repo  ethereum/EIPs#7482 [20.30](https://youtu.be/7lqT8vpm7M4?t=1230)
**Pooja Ranjan**
* That is issue number 7482. It is a consider adopting a community specification license term for new ERC repo. So some here has provided the description of the issue and I found a few comments by people were there, but there is no significant direction. If we are going to have this thing adopted. Wonder what people think about this particular proposal.
* I know this is for ERC people. We have not divided the people yet, but that is again, work in progress. So any thoughts would be welcome here? 

**Sam**
* What's the main difference with this license? Why do we want it to change? 

**Juan**
* I can speak to that. It's like a very lightweight IP protection like you. It's sort of a a lightweight affidavit of each person who contributes through a GitHub account that whoever controls this GitHub account doesn't hold any patents or they're going to exert against a contribution via GitHub.
* So since these, since this all happens via PRs, it's like a, it's like three quarters of the way to a or 9/10 of the way to a CL without  lawyers and translation and you know, like DocuSign and all of that. It's like just using a GitHub account insead of a DocuSign account to promise you won't sue people,  or patent trolls or something. And I've, I've set up.
* Community specification and the CLA bot on some repos where the participating companies felt it requested it . You know, coming from diff like Linux foundation orgs where it's sort of co-development and quote unquote corporate.  corporate open source. It's common to be worried about these things. And it's,  when you mean it's sort of like the, it's the specification equivalent of Apache two. It's like,  just enough licensing that makes people 80% more comfortable with 20% of the inconvenience.
* If that answers the question. I'm not sure that was exactly your question, though. 

**Sam**
* I just wanted to know mostly what the difference is between this and Cc0. 

**Juan**
* Oh, yeah. Cc0 is Doesn't protect us. Protect against patents. 

**Sam**
* Okay, so this explicitly includes a patent grant. 

**Juan**
* Sorry, I'm blanking on the details. 

**Sam**
* That's fine. But yeah, so we can. We can definitely look into this, I think. 

**Juan**
* To be totally transparent. Like, I'm not a lawyer. I don't have a law background. I tend to just do what people demand of me in collaboration contexts. And like, if no one is complaining, if no one is saying I'm not going to contribute to EIPS until you have a more,  defensive license,  you know, maybe isn't a homework we need to add to our plate.
* It's more like if you know the besu team or if I don't know if, if people are feel like they're hearing of people holding back from contributing or documenting things as EIPS because of this, we should we should move on this. I'm sorry, Victor. 

**Victor**
* Yeah, I think this is a worthy of discussion thing. It's from me. I have,  I previously worked at a company and for that company purpose perspective like this would not be able to be signed, which means that it had. I had we adopt that and then if I were still employed in that company,  I wouldn't be able to contribute to EIPs. So this one data source.
* So this is a double edged sword. Some company require it to be a patent grant to be comfortable allowing their, team to contribute some, on the other side. Cannot grant a patent grant and promise they wouldn't sue other people. And so if they add the CLS, they wouldn't be able to let the people, the team contribute to that.
* It's kind of like the debate between the two kind of license either you keep it open and what people can do whatever to it and or you keep it at like open and require people to be open continuously kind of free license debate. 

**Sam**
* We don't want people who might patent sue to contribute to the EIP repository. I think we're okay excluding those people from. 

**Victor**
* It's very different. For example, like I know that we're currently doing Cc0, which don't grant a patent. And on the other side I think the go eth choose to use the GPL, which is the the reverse. Are we saying that we all are going to the GPL side for it's not about patent, but copyright has similar issue here. Regardless. 

**Sam**
* It's very different, right? GPL imposes downstream restrictions on implementations where a patent grant would explicitly like a patent grant would explicitly remove restrictions on implementations. So like we're currently GPL and we'd be going to MIT to put that in like a copyright analogy. 

**Victor**
* But it is very widely adopted and even MIT doesn't have a GPL or even doesn't have a patent grant. 

**Juan**
* Or to put it another way, a patent grant is a defensive thing. Like you make people swear they're not withholding a patent when they contribute because then they could exert that patent against things downstream. So like what? When we when we talk about a patent grant, it's like a protecting implement future implementations from owing someone money they didn't know how to patent on a on a PR you know sorry Danno think your next. 

**Danno Ferrin**
* So I think wherever we go with this, we need to get the opinions of lawyers. Because remember, in a previous job, the licensing of a specification is different from the licensing of an implementation. So you could a specification and you could implement proprietary implementation of that specification. And none of that flows down from a specification to an implementation. You know, not legal advice.
* That's what I remember a previous lawyer telling me. So I think these are some issues that we need to talk about as well. And also, if I recall the Apache license thing, it's not fully so much a grant as much as it is mutually assured destruction. If you enforce patent rights against something that is necessarily,  you know, there is a grant of what's necessary for this. But furthermore, if you enforce patent rights against implementations of, you know, downstream of derivative works on this, you lose all Apache license grants.
*  So there's also a high cost to enforcement.  and nobody comes in thinking that they're going to create a patent trap In these specs you have some startup that gets some cool idea. They get the EIP published and then some large company buys them that is into these patent trolling things. I think if we do get into patent issues, that's the more likely scenario is a small company gets bought up by a patent troll who then starts enforcing things.
*  So, you know, just hoping that, you know, only the good people contribute.
*  It's like today they're good people, Tomorrow they're a problem. So there's if we can get the protections presented by this, that's a good idea. I'm just concerned that what's presented is going to give us what we want out of it. 

**Sam**
* So my takeaway is that we need to go and find a lawyer. 

**Juan**
* More than one. How much do you got? 

**Gajinder**1
* How many are. 

**Juan**
* At consensus these days? Not on fire drills. 

**Danno Ferrin**
* And they won't speak on recorded channel anyway, so I'll have to be offline to get a report from them. 

**Sam**
* Okay. I'll see if I can talk to anybody at the EF again, see if we can maybe get somebody to clear this up, or at least pay for somebody to clear this up for us.  Yeah. 

**Pooja Ranjan**
* Yes, Victor. 

**Victor**
* Yeah I like what I'm very much agree with Daniel.  speaking of whether we add the requirement or patent of patent grants is one thing I do feel realize that there's also something we could do is that we can ask people, if you are contributing, if you are aware of any existing patent that you know you can consider. I'm not proposing, but we can consider whether we want to ask people to require that they declare them.
* So if they enter, they intentionally put a patent secretly there and then declare that it's patented later on.  then they lose some kind of legal ground to sue people. 

**Sam**
* Yeah, that's I think what I'd like to see is at least just like a list of patents you're aware of or a statement saying you aren't aware of any. 

**Victor**
* And maybe this could be a follow up to the legal analysis as well. 

**Pooja Ranjan**
* Right. This doesn't look like an issue that we are going to get the solution right here in this discussion. But I was also wondering, Victor, if it is possible to collect thoughts from other authors on ERC dev meetings, so maybe we can add some thoughts on the issue and. Yeah. 

**Victor**
* Sounds good. I'll add a I'll add an agenda. 

## Update EIP-7329: Fix major website issue ethereum/EIPs#7554 [31:32](https://youtu.be/7lqT8vpm7M4?t=1892)

**Pooja Ranjan**
* On. Moving on to the next item here. This is a pull request number 7554 on it is to update EIP 7329 suggested by Matt and Matt, if you would like to maybe summarize and share the discussion point here. 

**Danno Ferrin**
* Could I jump in and request a docket order change? Could we fold this in after 5669, and do the 721 final and 5069 first, I have concern this might grow to fill time. 

**Lightclient**
* What would make you say. 

**Gajinder**
* Danno? 

**Danno Ferrin**
* Can we finish up the business first? 

**Gajinder**
* Yeah.

**Pooja Ranjan**
* Okay. Before we get. 

**Lightclient**
* To the fun part. 

##  Update EIP-721: Add ERC links ethereum/EIPs#7550 [32:27](https://youtu.be/7lqT8vpm7M4?t=1947)
**Pooja Ranjan**
* Okay. So before we get into 5069, we have one more proposal here that is to be discussed. That is a PR number 7550, which is an update for 7 to 1 proposed by Sam and Sam. If you would like to summarize and what we are trying to do here. 

**Sam**
* Sure. So I didn't propose this, I just finished it. But it's cleaning up some formatting issues in 721, which is a final EIP.  I'm not suggesting that we do this. I'm just bringing it up here because full dissent,  wants to fix some of the formatting issues. 

**Pooja Ranjan**
* Any edited object to it? No. We have like strong feeling that we should not go ahead and edit anything in final. But if it is just about formatting, not in any spec change could we? Do that. 

**Lightclient**
* I haven't had a chance to look at it. The Sam thinks it's good. I'm really good. 

**Sam**
* I'm not saying it's good. I'm saying that I reviewed it. There's one thing that could could maybe be considered a content change, but it's so minor. I'm okay with it. the rest is all all formatting. It just makes it like it's changing. Simple summary to description, that kind of thing.  Yes. 

**Gajinder**1
* What's the change? 

**Sam**
* What is the change?  so it's moving. Simple summary into description. It's replacing EIP 20 with ERC 20. It's adding links to other ERC's where they're required.  it's putting interfaces in backticks to show that their code.  and then it's changing a few of the link formats so that they don't say ERC in them anymore and I think that's about it. Yeah, it's basically just cleaning up a bunch of like ERC and EIP 20 kind of stuff. 

**Pooja Ranjan**
* Mostly sounds like a fair ask because we have recently changed the format. Earlier it was written as EIP 20, but for all ERC, now it is ERC. 

**Sam**
* Yeah. So just just request changes or approve the PR. I don't think we need to actively discuss it. I just wanted to mention it here. 

**Danno Ferrin**
* Could this be used as a poster child to set standards? For what? Changing the final changes ERCs allowed and which ones aren't? 

**Sam**
* We've allowed stuff like this before, and we've also said no to stuff like this before, so we don't operate on precedent here. 

**Danno Ferrin**
* But think it would benefit from a policy? Yeah. I don't know. But sometimes cleanup needs to be done. That's the other part of it. 

**Pooja Ranjan**
* All right. Very well, as some of our editors mentioned, they didn't get a chance to maybe take a look at this PR. The PR number is 7550. Please feel free to add your comment. And if in the next two weeks we do not get anyone like stopping the merge, we can perhaps go ahead and merge the PR. 

## Discussion continued or updates from past meetings | EIP-5069's new charter stuff. [35:59](https://youtu.be/7lqT8vpm7M4?t=2159)
**Pooja Ranjan**
* Moving on to item number two, which is discussion continued or updates from the past meeting. The first one listed here is for 5069.  I know the last PR we discussed in the meeting 88 is now merged and from there we discussed it was merged as an informational EIP, but we were supposed to have it changed to meta so we can enforce the changes mentioned in the EIP. Sam if you have thoughts updates on it would like to share with the team. 

**Sam**
* Yeah. So I'm just wondering if we want to ratify the the decision making process and the keeper of consensus role that we proposed in 5069. Last call. 

**Pooja Ranjan**
* People. Please don't take it literally the last call, because this is a living EIP. It's going to be in this. 

**Sam**
* No, Sorry. 

**Sam**
* Yeah. So I think, Victor, you were the one who asked for a comment period on this, so I'd like to get your opinion. 

**Victor**
* I'm sorry. What was the question? 

**Sam**
* So this is the end of the comment period. We had opened last call for EIP 5069, and I'm wondering if you're okay ratifying what's in EIP-5069. 

**Victor**
* I'm in full support now that no more further comment, let's rectify it. 

**Sam**
* All right. And I think everybody else had previously expressed support on the last call. So, we now have a decision making process.  I would like to. Well, I guess there's a few things that I'd like to introduce. We can do that after we're through everything else, I guess. Or we can do it now. I don't know. Anyways, we have to elect a keeper of consensus, so that's probably the first thing to do. I'd like to nominate Gajender. They've been reasonably. I don't know. Neutral on most topics. 

**Gajinder**
* Thank you, Sam. 

**Sam**
* And, yeah, I guess we have to post a formal call for input so we can do that after this call. 

**Pooja Ranjan**
* Sounds fair. So we would also be changing the type of the proposal, right? Currently it is an informational category. 

**Sam**
* Oh, yeah, I can change that. Sure. 

**Pooja Ranjan**
* Okay, perfect.  quick question this,  devoting or whatever we are going to do with the keeper of consensus, where can people go maybe read about it? I remember having a fellowship of Ethereum magician page open for this discussion. Do we want to keep it over there or anywhere else? People can share their thoughts. 

**Sam**
* So this is for comments on.  sorry. I'm not sure I understand the question. So. 

**Pooja Ranjan**
* So my question is, like we proposed in this meeting for having Gajendra Singh as the keeper of consensus.  I know some of the editors are not present in this meeting. We can definitely communicate as an outcome of it, but I'm wondering if we can have a placeholder for it somewhere so people can follow and we can let them know. 

**Sam**
* Yeah. So we have to. So I guess the formal process for making decisions now is we have to post a call for input. So that's actually going to be like a written thing that we put somewhere probably in the GitHub and then we have to post it in the channels frequented by editors. So that would be like discord here.  and then 30 days after we post this written notice is when the decision is made, if we don't get input from all the editors. So because not all the editors are here, we can't make the decision today. 

**Pooja Ranjan**
* That sounds like a very good process for making decisions. Thank you for summarizing that. Anything more on 5069 people would like to discuss here. All right. The other two items. One is GitHub repository split. I think that is work in progress. I don't see Greg on the call, so I'm not sure if there are any update on PR 7230 that people would like to share. Okay.  going back to. 

**Danno Ferrin**
* 7554. Kind of related. 

**Pooja Ranjan**
* Yeah, that's where I was going. Now, I remember the proposal, which is now in the last call. Now, if you would like to share more about it. 

**Danno Ferrin**
* If you want a neutral opinion, someone else should summarize it. But I'm willing to go for it. 

**Sam**
* Is this the like wanting to put things on different domains discussion or. 

**Danno Ferrin**
* Yes. Yeah, I'm only to summarize, but I think a neutral party would be better. 

**Sam**
* I haven't followed this at all. So I think you're the most neutral, informed person we have. 

**Danno Ferrin**
* Okay. So full disclosure, I'm very frustrated by this. Panda comes in at the very end of the discussions of the repo split and raises an objection that this is bad for ERC and asks because we're putting it under two different two different top level domains. What frustrates me is that Panda never calls into these calls. We've had lots of discussions and there's lots of back and forth argument that would be great on a voice call to understand what his concerns are and to provide some of the answers.
*  So that's that's my you know, as someone who opposes this, that's my summary. Keep that in full consideration as you consider my words on it. But it's you know, he doesn't want he's basically standing up in opposing the split. And he also another thing that he threw in at the end was saying, great. So as I'm okay with this as long as ERC  and as long as core is getting an entirely different website and don't keep the name EIP. To which my response was.
*  People have been calling ERC forever and telling people to go to EIPs website and go to  what did I call it?  you know, see. cpr.ethereum.com to get your eip information sounds contradictory because the website should be in the name everyone calls EIP. EIPs. I'm just recommending that the names go with what people call them to be. And even in the community I've seen people correct people for non thing saying you don't mean EIP4337. You mean ERC 4337.
*  So I think there's a strong argument to be made that the community already internalizes this change.
*  Maybe I'm wrong on this, maybe it's my perspective fully disclosing that you should consider everything I say with a grain of salt on this because of my position on this. But that's a brief summary of what's being requested on this. 

**Pooja Ranjan**
* Please go ahead , Victor
* If there is any link for this discussion, feel free to share it in the chat. 

**Victor**
* Yeah. Danno,  thanks for that. And just to add context, there was a one time that. Out of consistency that the editor group require all ERCs to be cited within EIPs as EIP. So there's a if you look at it, there were linters that ask the ERC for 337 to be changed back to EIP-4337 back then. And that's a little bit context and I do know that people are confusing or confused by our decision.
* I was opposing to that requirement. But now that we change it back, some people who have been forced to change also were confused in some way.
* So that is the background why potentially Panda was requiring that. And I just want to yeah. Throw in I don't have an opinion on this. 

**Lightclient**
* I find it kind of unreasonable for nine people to be on this call most weeks. And we've discussed this at length, and I thought that we had agreed upon the repository and website split two/ three calls ago. And for him to kind of come in in the last second, I just. I mean, this is just ridiculous. Like, it's not very respectful of everybody's time who's is spending trying to make the process better. So, like, obviously, I think it should be overridden. 

**Sam**
* So this is literally just about deciding what to do with the rendered docs. The there's no debate about splitting the repos, right. 

**Lightclient**
* It's okay to split the repos it seemed. But he doesn't think the website should be split. But that was kind of my impression with the repository split was the repos would then also be split because we're not going to then create a new repo just to generate the website. 

**Sam**
* Yeah. Like I mean I mean I actually prefer keeping them together on one website, but like it's going to be way more complicated to do that. And in the interest of keeping things simple, I'm totally fine. Just splitting the website too. 

**Lightclient**
* Yeah. I mean, think we could have a cool, nice website that had it all integrated, but we just don't have the manpower to do it. 

**Justin**
* Yeah. So like one of the key driving factors of the split was to allow for separate processes. And I think publishing is a really critical part of that process. So I mean, I think I thought it kind of went without saying that one of the intents and results that we expected from separating the repos was that you'd have a different and unrelated publishing schedule means opportunity, all that kind of stuff.
* The suggestion that keeping them together is superior seems to really contradict the whole reason we did this in the first place. So. Yeah, That's going to be a no for me dog. 

**Gajinder**
* I can understand how. Having a single website really affects downstream the processes that are there and, publishing schedules. I mean, these are easy things to figure out as well as how to sort of merge these two repo at the time of publishing by a bot. That is also pretty simplistic. So I'm not really sure where. I mean, the kind of problems that we are trying to solve by splitting the website are actually there. 

**Justin**
* That's fair. But it's also more complicated and more work like. I agree with you, it's possible. But I just don't see the the need. 

**Pooja Ranjan**
* I know Panda is not on this call. And as we have mentioned it multiple times, that in most of the cases he is the one who is updating the website and kind of working on this. The the manpower that we are talking about, it seems like editors on call today not in strong support of having it on the same rendering website. I don't know.
* I mean, I really don't want to say on anyone's behalf here, but it seems like the initial idea of having the repos split will make sense when we have both of the things on different pages to follow to just eips.ethereum.org. There could be erc.ethereum.org and I think that was initially proposed. What do people think about having a having an announcement to get people on board to maybe work on improving the website along with this kind of split?
* And maybe we can invite Panda if not on this call, maybe on a separate call sometimes on the weekend as he has proposed, and see if he would like to own the responsibility of it.
* Plus he may be having the bandwidth of maintaining it in the long term. 

**Sam**
* Yeah, I mean, we could do like a couple workshops on improving the website. And I think the decision for today is that rough consensus among editors is to have separate websites. Is there anybody who disagrees with that? All right, cool. 

**Lightclient**
* Yeah, I mean, obviously I would like separate websites, but I don't think that we need volunteers sort of contributing to this because we need like long term contributors. We've kind of been playing over the past few years with people who contribute for on the order of like two to 8 to 12 months and leave and sort of their projects fall by the wayside. So I don't want to switch to a website where we have some people come in, do a bunch of work and then just leave because then we don't have the experience maintaining it or building it or whatever.
* So I would like to get people who are contributing to the process on like long term scales working on it. 

**Juan**
* Sorry. I was just gonna say, with maybe one minor exception, one off gig that does need some manpower is figuring out how to redirect all the links that would be broken if a canonical link is moving, like figuring out how to make the Jekyll.  you know, have that like whatever it is that Json-ld canonical link thing.  I mean, maybe that just takes someone five minutes who knows how to do it, but that's just like one thing that does need to happen,  in the process of breaking out separate sites. 

**Victor**
* Yeah. Redirect. I think it's a must have. I would not be very conscious. Comfortable having redirect broken. Is that a consensus that we will keep we will make sure that the canonical links to ERC will continue to exist and in the format of redirect or non redirect, I really don't care. 

**Juan**
* I'm trying to remember off the top of my head, and I'm not really a specialist, but if I remember correctly,  if you can't do a redirect. Next best thing would be to keep it where it is and have some invisible, you know, like, non displayed annotation in the HTML that tells search engines. The canonical version of this has moved update your index.. Sort of like when you archive a repo on GitHub, it points you to the new one and you know all people who search for it gets the new one. But just just to say that I also agree that it would be ideal to at least have a canonical redirect, if not a dynamic browser redirect. 

**Danno Ferrin**
* So EIP-7329, which is the meta one. Step four in the specification says set up a redirect for ERCs on Ethereum. Org to go to the new website. So getting these is part of the spec. So it's a requirement. 

**Gajinder**1
* Cool. Good point. Sounds good. 

**Pooja Ranjan**
* And just for people to know this proposal 7329 is currently in the last call and it is in metae. We are going to make it enforced that this ERC repository split is going to happen as per the process to explain in this particular EIP. So that's a good place to follow what is being proposed as of now. 
* We have about five minutes left. Danno, if you have any other concern with respect to the split that you would like to share or maybe discuss. Or anyone else. 

**Danno Ferrin**
* I have no more concerns. I'm just happy we're not five minutes over. 

**Pooja Ranjan**
* That is a good one. Very well. So it seems like we are making good progress in the direction of this repository split. We are considering the process of decision making from here on and we are also considering important aspects of different repositories that may help people, users and authors to maybe follow the process, understand how it is, and maybe, you know, share more information because this is something changing in the entire process. We might want to educate more people about it. We might want to share information as much as possible. That's all on the topic. 
* Let's quickly take a look at whatever is left. I think the next one EIPs Insight. Taking a look at the September months insight, we see that there are three EIPs in the last call as of now. The one is 7329 where the deadline is ending on September 12th. 
* Authors, please feel free to make your proposal into final status. Create a pull request after the deadline date. The other two proposals are of ERC category number is 5114 Soul bound batch. The last call deadline is September 19th, ERC 7401, which is also ending on September 19th. And the proposal is about parent governed NFT token nesting. 
* Authors listening to this call, please create a pull request after the deadline to move the proposal in final status. Anyone else interested in sharing their thoughts about this proposal, please reach out to the author before the deadline because we would not encourage having any changes after the proposal is moved to the final status in this month of September, we have received two final proposals. And there are five proposals in draft. One proposal has moved to stagnant status. The proposal number is 5139. Okay. I don't know if this has to be moved to stagnant or do we really want to move it to withdrawn? 
* But that is on the author to decide on it. That's all on EIPs status reporting. We had EIP editing Office Hour yesterday have added the recording for Meeting 24. Agenda for Meeting 25 is up. 
* If you have a pull request that you would like to discuss and ask questions from editors, please add your number to the agenda and that pretty much conclude everything on the agenda today. Anyone has anything to add share, or maybe something to suggest for the next meeting? Very well. Thank you, everyone, for joining us today. Hope to see you in two weeks. Till then, we can have our async discussion continued on Editor channel on Eth R&D and Ethereum cat Herders Discord Channel. Thank you, everyone. Have a good day. 

**Gajinder**
* Thanks. Thanks, Pooja. 

**Pooja Ranjan**
Thank you!

---------

## Date and Time for the next meeting

Sep 20, 2023 at 14:00 UTC

---------
## Attendees

* Pooja Ranjan
* Sam
* Gajinder
* Victor Zhou(@xinbenlv)
* Lightclient
* Justin florentine
* Juan Caballero
* Joshua

---------
