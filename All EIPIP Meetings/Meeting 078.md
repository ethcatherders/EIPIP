# EIPIP Meeting 78 Notes
### Meeting Date/Time: Apr 05, 2023 at 14:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/224)
### [Audio/Video of the meeting](https://youtu.be/K3IPrhMX-lY)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
78.1 | **PR-6824** - Merged
78.2 | **PR-6813** - Need more testing 
78.3 | **PR-6790** - Closed. The majority of editors are not in favor.
78.4 | **PR-6799** - Closed. It will not be needed because 6790 is closed.
78.5 | **PR-6805** - @SamWilsn will review it.
78.6 | **PR-6269** - Closed. Not a good fit for the EIPs repository.
78.7 | **PR-6306** - Split into two. @SamWilsn created a new [PR](https://github.com/ethereum/EIPs/pull/6834)
78.8 | **Issue-6650** - Not ready with a PR
78.9 | **EIPW bot** - Issue 5 is tested. Hopefully, the PR will be merged soon. JA will work on the next high-priority issue.
78.10 | **Move Shapella EIPs to Last Call** - Pooja will create PR to promote EIPs.

## Intro
**Pooja Ranjan**
* Welcome to EIPIP Meeting #78. I have shared agenda in chat. It's issue number 224 on EIPIP GitHub repository. We have few open issues and prs to be discussed today, and there are a couple of items from the earlier meetings. Discussion continued. We'll get some update on EIP W Bot issues. One of the, Cat Herders are working on it. And we'll go ahead with EIP'S insight for the month of March and April, followed by EIP editing office R. So going ahead with the agenda, 

**Pooja Ranjan**
## Update EIP-1: Update EIP-1 to include wording about The Finalizing Pull Request ethereum/EIPs#6824  [0.49](https://youtu.be/K3IPrhMX-lY?t=49)
* The first item listed here is, an update that is for EIP PR is 6824. It is to update EIP one to include wording about the finalizing poll request. I suppose this is, created by Victor. Victor, if you have, something to share about it. And then probably we'll see what other editors think about merging of this proposal. 

**Victor**
* Sorry, can you put it in the link? 

**Pooja Ranjan**
* Sure. Just give me a second, it's a pull request number 6824. So this is the first item on the agenda pull request number 6824 to include, some word about finalizing. Yeah. 

**Victor**
* Yeah. The, the background is that, in our previous discussion, on EIPIP meetings that people agree, generally, you should not, move a, EIP into final status with other changes. Basically, the last PR pull request to move a status to change an EIP status should only touch the status without other changes. And this is a, reflection of our, the, the meeting's decision. just, oh, it's already merged. Okay. 

**Pooja Ranjan**
* So, yeah, Yeah, looks like it has been merged. it received, approvals from other authors. So thank you for providing the background here. 

**Victor**
* Cool. Thank you. 

## CI: Bump rakefile deps ethereum/EIPs#6813 [2.45](https://youtu.be/K3IPrhMX-lY?t=165)
**Pooja Ranjan**
* All right. the next one is pull request number 6813. that is to, that is a CI change for Bump rakefile deps. I see a lot of, comments here. and, there are some changes made by the proposal. Fully wonder what other editors think about merging for this proposal. 

**Sam**
* I think it just needs to be, tested. it looks like one of the builds is failing, so the, the CI checks, so. 

## Update EIP-1: Remove eip preamble entry ethereum/EIPs#6790 [3.43](https://youtu.be/K3IPrhMX-lY?t=223)
**Pooja Ranjan**
* Okay. And I think Panda left a comment over there, right? So, yeah. All right. let's move ahead with the next one. This is created by Panda, and it is, to remove eip preamble entry. I think I can, see a lot of comments. there are some people in favor of it and some are not. I don't see Panda on call today. if anyone would like to maybe, say why they are in favor or not about this particular PR 6790. 

**Lightclient**
* I'm just gonna reiterate what I said on the PR. I don't really see much pointed in removing it. Like it's, it really isn't affecting anything. It might make the CI bot slightly more complicated, but it's a longstanding part of the EIP process, and I think we should just retain it. 

**Victor**
* I support that. We don't, remove it. I share even stronger that I think in a content of the, EIP, we should have a, have a number just like, even if you might have title somewhere, you should also have the title in inside of the, the inside of the content. And, EIP number is an important piece of that information and should, should be duplicated and double check. 

**Edson**
* So I'm missing the, the argument on removing it. So is it just, because the EIP number's in the title or in the file name that he wants to remove it? 

**Lightclient**
* Yeah, it's in the file name. So, so it's kind of duplicated in those two places? 

**Sam**
* Well, it's a little bit more than just that, right? Like, we're working on making the EIP number signing bot, and it's, you know, 1% easier if you only have to change it in one place instead of two places. So I think that's where this is coming from, but, it really doesn't matter too much technically, which way we go. 

**Edson**
* Creates some overhead though, right? Cause it's not exactly progress compatible. 

**Sam**
* Yeah. Yeah. We'd have to go through and, and change, old EIPs and stuff, so it's a little annoying there. 

**Lightclient**
* Yeah, I mean, let's just close it. There's not really a strong argument for it Very well. 

## Website: remove dependency on eips preamble entry ethereum/EIPs#6799 [6.24](https://youtu.be/K3IPrhMX-lY?t=384)
**Pooja Ranjan**
* So I think one of the editors may be able to close it. it looks like most of them are not in favor, so we don't have a clear consensus on that. Moving ahead. The next one is, website remove dependency on eips preamble entry ethereum/EIPs#6799, and it's by pan again. looks like it's waiting for some review. 

**Sam**
* Yeah, this is only necessary if we remove the EIP preamble entry, and if we're not removing it, we don't need this change either, Right? 

**Pooja Ranjan**
* Yeah, that's why I had it like, followed by the, yeah, eips preamble, so we don't need this either, right? 

**Sam**
* As far as I know, no. 

## Update codespell-project/actions-codespell digest to 57beb9f ethereum/EIPs#6805 [7.21](https://youtu.be/K3IPrhMX-lY?t=441)
**Pooja Ranjan**
* Okay. If, any of the editors may close these two, number 6790 and 6799. Next one is a update code spell project, action code, spell digest. I'm not sure if it is created by a human or a bot, so I just thought of, bringing it, to this meeting. Wonder what people think about it. The number is 6805. 

**Sam**
* Yeah, these are made by a bot. This is the mend renovate thing that PandaPIP wanted to do. And, it makes useful for pull requests. I just haven't gotten around to reviewing, any of them yet. 

**Pooja Ranjan**
* Okay. Then I'll, like let it live. maybe when other editors also get chance to take a look and Sam, if you can, because you are closely looking into bots. So yeah, that would be good to have. And that, concludes our first, like new discussion items, our pull request. 

## Discussion continued from earlier meetings
## Add EIP: undefined ethereum/EIPs#6269 [8.18](https://youtu.be/K3IPrhMX-lY?t=498)
* The next one is a discussion continued from the past meeting. someone requested to have the first two sub items for this particular, section. The pull request number is 6269, and it is about, full EVM equivalence in Ethereum. So it looks like it was, discussed earlier, I think when we had Greg on the call as well, and we didn't have any clear consensus on it. So after three, four meetings, the proposal has requested to be discussed again to see if there is any new stand, by the EIP editors. And if we can probably move this forward. 

**Victor**
* Do we have consensus? The executions back should be linkable? 

**Sam**
* Yep. 

**Victor**
* I think, I think we can let the, proposer just split it out and then put this, the execution first and then yellow paper, I think, Sam and Matt is against, and then Greg and I were, support. So we can discuss that further. We, we wanna just minimize the block on whoever proposed the link and Oh, It's not the links. 

**Sam**
* It's not the links that are blocking this. 

**Victor**
* Okay. 

**Sam**
* Well, I mean, they, they are, but if they remove the links, I still wouldn't let them merge this, because you can't make any EIP enforce things on other EIPs, so I don't see the point in having an EIP that just makes a definition without some sort of technical, like substance or proposal. Right. So I don't think the content of this EIP is suitable for this repository. 

**Victor**
* Oh, are you talking about this content is Oh, you mean, yeah. The, the content of this EIP is not relevant to actually being on EIP. Right? 

**Sam**
* Exactly. Yeah. It's like, yeah, Of course.  if you wanna define what full VN equivalence is for your proposal, go for it. But making one proposal to define it for everybody  is not something I think we should do. 

**Victor**
* Until, I mean, until, when there's use cases where multiple independent EIP p needs a definition, and that definition is non-trivial. So maybe just too early or, It doesn't make sense at all. 

**Edson**
I'm looking through it. This is full EVM equivalence and it's just definition of it, it seems like to me, like a marketing term could be done at blog doesn't really. Exactly. Yeah. 

**Victor**
Yeah. Agreed. Agreed. We should close in that case. We should close it. 

**Pooja Ranjan**
* Okay. so yeah, the last comment was from the saying that let's discuss this in EIPIP meeting. And, from today's meeting, probably we can add a comment that, editors are in favor of closing. This may not the best place to add it in EIP repo. 

## Update EIP-1: Permit links to Execution Specs ethereum/EIPs#6306 [11.51](https://youtu.be/K3IPrhMX-lY?t=711)
**Pooja Ranjan**
* The next one here is, poll request number 6306. It is by the same author, a same proposal, and, it looks like, we have two comments. One in strong favor and one strongly thinks that it should not be added to EIP one, Victor and Matt, if you would like to share your thoughts and arguments. For, and against. 

**Victor**
* Oh, this is actually the one that I, I was confused with. so, I think the proposal was to add, to allow link, a permitted links, and then one is to execution, execution, spec, which we all agree. And then the yellow paper, which we disagree. And, so, I think we can let the proposal, let, submit the merge for the spec first, and then we can wait for consensus.

**Lightclient**
* What do you mean wait for consensus? Because I feel like we rent this problem a lot where there are opinions, and then we just leave it open for six months. And I'm, I got not going to change my opinion on this because  I really don't think the yellow paper makes sense to link to. It's a deprecated resource and people should start linking to the execution specs. 

**Victor**
* Can you make a, argument that I know that is lack of updates, just like execution is currently being the canonical one to update, and then we kind of socially agree that execution is up to date, but how can you prevent six months or a year from now? The execution spec is also continued to be maintained. And then like  I believe that people were, the community maintained yellow paper back then when they write it, when they updated with, with Berlin updates, they didn't think that it will be not a, it will cease to to be maintained. Right? So the fact that you think that it is currently, a lack of maintained, I don't know if that is consensus. I'm actually proposing that, and Greg and I were proposing that we should actually look into it and, have people contribute to, with the, to put, yellow paper back to up to date. So that's why I feel that, using the arguments that yellow paper is no longer maintained as a way to block links is for one week and for two, it doesn't also apply to execution. And even longer, I don't think deprecated documents, is one thing, is a reason to stop, linking to them like it.  for us, we believe that, giving people historical context is also sometimes useful. 

**Lightclient**
* We don't really give historical context in the e repository that much, that's not really the point of the EIP. The point of the EIP is to specify and to give rationale for the decisions. 

**Victor**
* So Where there's rationales usually needs to carry historical decision, context, right? 

**Lightclient**
* Otherwise, how do you make our, our rationale, Our whole point of EIP is to not link to a whole bunch of stuff. And if we were to be providing a lot of historical context, then we would be happy to provide a lot of links to, oh, there was a discussion here on Twitter then at this interop we had, you know, this decision. And originally it was like that, like this isn't, you know, assimilation of a whole bunch of information about how we got to this certain point. It's trying to concisely define the spec and then trying to concisely define why things were chosen and summarizing a bunch of conversations. But that to me is like not that big of a point. The point is, is that the yellow paper isn't updated past the merge. There's not really people working on it. If that changes, then we can reopen the discussion and think about it some more. But right now we have three full-time people working on the execution spec. It works post merge, it works for Shanghai. We have people maintaining it for the foreseeable future. If it gets to the point where it's not maintained, then we can have a discussion, okay, this thing is not maintained anymore. Is this something that we need to keep supporting links for? But that's just not where we are today. 

**Victor**
* So again, I understand where you're coming from. but I feel, and I believe Greg feel very strongly that we should allow authors to link and, the fact that we don't, if You can get the yellow paper to support Shanghai, I think We Should conversation. I don't, but it doesn't Shanghai paper. I don't think yellow paper needs to, yeah, yellow paper needs to be updated in order to be qualified to be linked. That's the point. Like, I'm not arguing with you that yellow paper is out of date. That is sad fact. We agree that, but the fact that we don't allow a linking to at yellow paper, and then the fact that we are not allowing, we're linking to other, live clients back, live  clients on implementations. I believe that is making it very hard for authors to, that's A Separate debate to make their arguments. 

**Lightclient**
* Yeah, That's separate in yellow paper. 

**Victor**
* No. So, I'm saying that restricting, we should have very strong reason to restrict link unless there is a need, rather than we should by default link, this permit link without, with, unless we have a strong reason. 

**Lightclient**
* And what, from What heard why into the yellow paper, like what, what good does it do to link to a resource that doesn't accurately reflect the current state of Ethereum? 

**Victor**
* So what's the point of linking to an EIP ? Like what's the point of, it is to link to ERC 20, to ERC 721, 

**Lightclient**
* Because these are finalized standard that represent the state of the art.

**Victor**
* It doesn't represent the state of art ERC 20. 

**Lightclient**
* It does. These things are finalized standards that are accepted. You can't link to something and become final if it also is not final. 

**Victor**
* That is not how we define linked, but you begin with It is, We are using the proposal, EIP proposal to let people make arguments, make technical arguments. And even like to begin with, we, there is an RSC that people were following we're use must and should. And then even that one, that RFC is being updated, that was, that was duplicated and then we linked to it without, no, without a problem. So we are just empowering ourself too much to restrict link. And then again, I know that we are not, I'm not going to convince you and then, you are not going to convince me either. And I think that we can put aside a, 

**Lightclient**
* So then We should close this issue because if we're just gonna sit here and like argue it about it every single meeting, this is not useful. Like proposals that we to change the Ethereum repository, the EIP repository should generally be accepted unanimously. And if they're not, then we just need to move on and start working on next to the next problems. 

**Victor**
* I am agreeing that we should, allow executions spec to be linked. And that was what I proposed. And we know that, what yellow paper is, being is not being, in concerns yet. So that's what I proposed. We split it out and then we let the execution  to be permitted go to go in and for the yellow paper, we can just wait another six months or a year, and then we'd come back to discuss. How's that,

**Lightclient**
* That's fine with me, but I think that something needs to material change to discuss, again, like we have discussed this several times now, and nothing has material changed on the front until like, I am not gonna be okay with accepting the yellow paper until it supports the latest fork. I reserve my opinion, You reserve Your opinion, but I don't wanna talk about this next week or in two weeks. 

**Victor**
* Or like, there's two other possibilities that either there is this material change or, the sentiments in the, in a group changes. How's that? 

**Gajinder**
* So My opinion on this is that, is there an instance where we are actually severely impacted by not letting, the reference to yellow paper come in by EIPs? I mean, if there is such an instance and we are really being impacted and there is a real impact, then it becomes something to discuss about us. The discussion is moot. 

**Victor**
* The impact is that, author, when they're making, EIP arguments, they want sometimes need to cite the historical context. And then, EIP yellow paper has historically been a very good source of the, of the, execution there. 

**Pooja Ranjan**
* I think this would be probably a good place to, let this, discussion, settle down on maybe if, people are more interested can add more, like, you know, support on the, pull request itself. because, you know, 

**Victor**
* Hold on.  I think I have a one question for, for my client. My client. Do you think we should permit per link to e execution per, spec, or do you think that we should permit LiveLink to execution link? 

**Lightclient**
* What is the differentiation? 

**Victor**
* Per link? Per link is gi gi is GitHub's link that includes the commit, which links to a, non-changeable, specific snapshot of exec, of a repository live link links to a relative place of inner repository that may change. So do you think that we should allow per link to executions spec or we should allow live link to executions spec? 

**Lightclient**
* Let's, live, I mean, we can't allow a live link. Okay, Link says that we have to link with the perma link, Right? 

**Victor**
* So if you link to a perm link, it doesn't change, it's gonna be out of date. 

**Lightclient**
* So by your, we're Already, we're already shooting ourselves in the foot by accepting a resource that's not being updated. Like why take on this Steps? 

**Victor**
* That's the, that's the point. You can't, like in the world of war links, you can't assume the source is going to be up to date. You never will be like, yeah, that's why, that's is like, I'm just using this argument to show you that you cannot assume that that's fine If you, Why accept something is already not up to date. 

**Lightclient**
* Like, it's not nothing that we have to assume. We already know that nobody is currently working on the yellow paper. I don't know if that's ever gonna change. It probably isn't. It's gonna be really hard to define the merge in the context of the yellow paper. And so why go ahead and accept this thing if the most like, it, it's gonna be just become less valuable over time if the execution spec stops being supported at some point. That's unfortunate. 

**Victor**
* By definition, by your definition, the  link stops being changed, it stops evolving. So that that, that, that's exactly the same place where like if you don't think execution spec as one thing, but as snapshots of each one of the individuals themselves linking to each one of them is going to be out of date. No one is maintaining and changing that pera link because it cannot be changed. 

**Lightclient**
* There's No points to have multiple resources pointing to the same things. The execution spec already implements all the historical hard forks. The yellow paper is not being updated. We don't need to have two ways of linking to something depending on how you feel or like what resources you're use used to. We should be forcing people down this one funnel that's supported right now, and if something changes in the future, we can address that issue. But this is just how things are stand right now. 

**Victor**
* I don't think you answered my question. How could you, how could link to the, per link maintain the up-to date status? I mean it you Using, you using the argument? 

**Gajinder**
* It doesn't, but someone is supposed to come and update it back, with a current, I think that's how it should work. 

**Victor**
* Sorry, I don't hear that. I'm not sure if I follow you. 

**Gajinder**
* No, we first, we can't link to a dynamic link because, dynamic link can change and the content in the EIP can basically go very tangent to what now the dynamic link contains, right? So, if, and the issue of permalink needs to be resolved by the fact, by the matter of updating the EIP itself. So I guess, you know, permalink needs to be there, but the EIPion also needs to be, hap needs to happen if something material changes in the link, Right? 

**Victor**
* So I'm not arguing with you that we should add live link. I'm just saying that the same reason that we disallow LiveLink. And so the same reason that we disallow yellow paper is going to be the same link that we disallow per link because perm link don't change, it will be out of date. 

**Victor**
* I'm arguing that's, I'm sorry, go ahead. 

**Gajinder**
* I want to say that we, I think the, what really matters is what context does yellow paper has that execution specs don't have and people can't refer to. I think if we can answer that question, then maybe we can make a logical decision about this. 

**Lightclient**
* I agree. I, so, I mean, don't forget, the reason that we are having this debate is because the informational EIP for EV equivalence that we just said we should close was asking for it. This is why we're trying to put the yellow paper in for something that we don't even wanna support the repo. 

**Victor**
* There's a lot of other EIP that has tried to add link to yellow paper. Like the fact that this come from the context, the adding an EVM that one, I, I don't think it, it really matters. 

**Lightclient**
* There's historically other, a lot of other EIP that is trying to link to yellow Paper did let them open a PR to add a link to the yellow paper. Easy. 57. 

**Victor**
* 5757, Sorry. what was the, the number? 

**Lightclient**
* 5757, the EIP that defines how to add links to the EIP one

**Victor**
* And then, sorry, I don't think I heard your last sentence. 

**Lightclient**
* I'm saying if people want it, then let's close this and wait for someone to come back and say, I have this EIP, it's really important that I have the link to the yellow paper right now. The person who said they want the link to the yellow paper wants to try to define something an informational EIP that we don't think is a good fit for this repository. If at this later point an author says it is critical for my EIP that I link to the yellow paper, we can have this debate again. 

**Victor**
* Okay. Alright. Right. If that is, that is a possible, new information, I would accept that to wait for, this discussion. Like I can accept we, put this discussion on hold, until either  yellow paper changes or a number of, editors who feel that we should allow linked to yellow paper changes, or there is an author, who have, strong re-reason in their own EIP that needs to, allow this, it needs to allow this, how's that? Otherwise, we put this discussion in on hold for another 12 months or so. 

**Pooja Ranjan**
* There could be another reason. There could be another reason when Bot decides to, make it stagnant. So I hope, one of the conditions, come earlier than, bot, so we can probably bring it back to the agenda. 

**Lightclient**
* I mean, yeah, I feel like we should close these things and not just let them sit there because then we get notifications when it's stagnant that we wanna talk it about it. Again, we've kind of reached this impasse where there isn't really a good way forward, and so we should close it. And if somebody comes and reopens the PR or decides to open a new PR that does this thing, we can have the discussion again. 

**Victor**
* Sounds good. 

**Pooja Ranjan**
* All right. 

## Add EIP: undefined ethereum/EIPs#6269 [29.56](https://youtu.be/K3IPrhMX-lY?t=1796)
**Pooja Ranjan**
* Maybe for like, another issue that we just, another poll request that we just discussed, 6269, if someone can maybe close that, that would be nice Saying, yeah, I don't feel comfortable closing it because I'm the one who is very vocally against it, so if somebody else wants to take care of it, I'd appreciate it. 

**Pooja Ranjan**
* All right. Yeah, I mean, which One? 

**Victor**
* I can, I can try. 

## Update EIP-1: Permit links to Execution Specs ethereum/EIPs#6306 [30.26](https://youtu.be/K3IPrhMX-lY?t=1826)
**Pooja Ranjan**
* 6269, Okay. That we decided that it should not be a part of EIP repository and followed by, 6306. If we think that we can probably take up the discussion back, to the meeting when we have an example for a proposal, who really needs it For 6 306? 

**Sam**
* I split it in two. So there's one for the yellow paper and one for execution specs now, yeah. 

**Pooja Ranjan**
* Okay, then okay, fine. Then we need to add a comment there maybe for the proposal to know about it. And this again, will be either closed or will be just one part of it in the PR. Alright. so we can probably move on to the next one. 

**Pooja Ranjan**

## Customizable editors ethereum/EIPs#6650 [30.59](https://youtu.be/K3IPrhMX-lY?t=1858)
* The next one is PR number 6650. And it talks about customizable editors. Sam, do you want to discuss 6843 right now?

**Sam**
* I'm looking at it. let's see. Oh, I see. Okay. So this is for, yeah, so it'll only give editors, like, it'll only tag editors for certain, keywords or for the lack of certain keywords in, proposals. I don't really feel strongly about this unless we have like a more, rigorous categorization system, but, yeah. 

**Pooja Ranjan**
* Okay. So we are still discussing 6650. 

**Sam**
* Yeah, I don't know if this is ready for, an EIPIP discussion yet. 

**Pooja Ranjan**
* Yeah, right. I just wanted to provide background here. Like, you know, in the last meeting we asked the proposal like what is the proposal? And he ably added, few more context to it, like what, is being tried to be done here. I just wanted to let just know so they can take a look and provide the feedback. There is no pull request for this proposal yet. Okay. And I see that, PR #6834, is already there. Thank you Sam, for creating that. That is to allow links to the yellow paper as a separate discussion. Okay. Fair enough. I'm gonna add that in the summary for today's meeting. That concludes, oh, sorry. A anyone wants to share something? 

**Victor**
* Yeah,I try to close #6289 Six nine. I don't have closing. I don't have closing rights. Anyone who has closing, right. please close it and then I already notes down our making notes to say that we will close it, Ma'am. 

**Pooja Ranjan**
* Thank you, for that. Matt, maybe if you can give it a try because Sam wants to be reserved. He's like, vocal about it and he just want to reserve from this. So if you can give it a try sometimes today or later It worked. 

**Sam**
* Yeah, Matt closed. 

## 3. EIPW bot Issues [34.01](https://youtu.be/K3IPrhMX-lY?t=2041)
**Pooja Ranjan**
* Okay, I have to refresh my agenda so it can reflect it here as well. Oh yeah, it does. Alright. the next one isEIPW bot Issues. JA, if you have any updates to share. 

**JA**
* Hello? Yes, I think that I finally managed to get the, the code, not panicking. I already sent a brief, summary to you Sam, so I'm gonna work on the test this weekend. So when I will get that done, I hope so. 

**Sam**
* Awesome. Thank you so much. 

**Pooja Ranjan**
* Cool. If there is any other issue of high priority that you would like to take next, maybe you can check with Sam because he generally manages this spot repository. 

Speaker: 6
* Yeah, for sure. Thank you. 


## 4. EIPs Insight - Monthly EIPs status reporting. [34.33](https://youtu.be/K3IPrhMX-lY?t=2073)
**Pooja Ranjan**
* Thank you. Moving on to the next item. It is EIPs insight, so have added hackmd for the month of April as well. We have four new EIPs as draft to promoted to review and two EIPs in last call with three EIP getting into final status 
* Last call proposals are #EIP 6220 with the end date on 18th April, and the other one is #6105 with the end date of 4th April, which has already passed. So the author is requested to create a new pull request. If there is no major feedback for spec changes, they can create a new pull request to move this proposal to the final status. 
* The three final EIP are EIP 4736, that is CLWP consensus layer withdrawal protection. There are two ERCs, ERC 5006 rental, nft, NFT user extension, and ERC 5219 contract resource request. all of them are added in the Hackmd added to the agenda. that's all on EIPs inside for EIP editing hour.
* We had our last meeting yesterday. There would be another meeting two weeks from, yesterday. And I have added agenda to the new meeting. People may request any pull request. They have question about their particular proposal and that will be answered by EIP editor. Sam generally takes out this office hour to, talk to authors. 

## 6. Review action items from earlier meetings [36.41](https://youtu.be/K3IPrhMX-lY?t=2201)
* And then last item for today's discussion or maybe information is, action item from the earlier meeting. I have added link to the notes. I'm just taking a quick look. Okay, so the first one was related to 5682 to no consensus. 6579 was approved.  Obviously it would've been merged. And the third one was, about this straw man proposal discussion to be continued in the, link provided there. 
* So probably there is no action item, specific on anyone. So yeah, that all concludes, for the items listed here today. 
* Anyone has anything to bring up share? I want to discuss, 
* I have one thing that I wanted to mention here. Like I mentioned it in the meeting as well. I'm not sure if we have all the proposals for Shapella upgrade in the last call I saw only one proposal in last call and one is already final because that is a meta and that is not going to be deployed. But there are I think, three more proposals that needs to go in the last call. Now we do not have even two weeks. It's less than that. But, I'm wondering like, what would be the next step? Is it okay that, someone from Cat Herders may create pull request 

**Sam**
* Yeah, Certainly. Fine. 

**Pooja Ranjan**
* Okay, fine then I'll go ahead and do that. 

**Sam**
* Thank you. I appreciate it. Okay. 

**Pooja Ranjan**
* Okay, that's all. Anyone has anything else to add for today? Cool. Vince, thank you all for joining us today. See you in two weeks on April 19th at 1400 U T C. Have a good, Yep. 

**Edson**
* Bye everyone. Thanks. 

**Victor**
* Thanks everyone.

**Pooja Ranjan**
* Thank you. 

---------

## Date and Time for the next meeting

Apr 19, 2023 at 14:00 UTC

---------
## Attendees

* Pooja Ranjan
* Sam
* Gajinder
* Victor Zhou(@xinbenlv)
* Lightclient
* Justin florentine



