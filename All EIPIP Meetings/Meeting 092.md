# EIPIP Meeting 92 Notes
### Meeting Date/Time: Oct 18, 2023 at 14:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/281)
### [Audio/Video of the meeting](https://youtu.be/KUT2cIzuu_w)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
92.1 | **Web Page Rendering for EIP & ERC**: @Pandapip1 is coordinating a meeting of EIP editors scheduled for October 25 at 14:00 UTC.
92.2 | **Web Page Rendering for EIP & ERC**: Discussion will be around the evaluation of setup, website and other tooling to ensure everything after the split should work uninterrupted.
92.3 | **Web Page Rendering for EIP & ERC**: Except @xinbenlv all other editors on the call were against having a separate website.
92.4 | **Web Page Rendering for EIP & ERC**: @Pandapip1 will come up with a repo-dependent layout to have a unified website to render EIPs & ERCs. Updates will be provided in the next EIPIP meeting.
92.5 | **Call For Input**: Allow links to CVEs #273 - Decision: Yes. Issue Closed.
92.6 | **Call For Input**: Renumber EIP-5000 #274 - Decision: After a long discussion, it was decided that an EIP will not be renumbered retroactively. Close the related PR.
92.7 | **Call For Input**: Allow links to the Yellow Paper #275 - Decision: Yes
92.8 | **Call For Input**: Updating EIP-4804 (Web3 URLs) #276 - No consensus, just closed.
92.9 | **Call For Input**: Accidental function in ERC-223 #283 - Voting is open till Nov 16.
92.10 | **Changes to Final proposals**: Update EIP-5773: fix typo ethereum/EIPs#7866 - Merged
92.11 | **Changes to Final proposals**: Update EIP-6963: fix typo ethereum/EIPs#7863 - Merged
92.12 | **Changes to Final proposals**: Update EIP-6492: fix typos ethereum/EIPs#7843 - Merged
92.13 | **Changes to Final proposals**: Update EIP-6672: fix typos ethereum/EIPs#7840 - Merged


# Intro
**Pooja Ranjan**
* Welcome to meeting 92 on agenda. We have some items to be discussed, some open issues, and then we will get into some pull requests which are open. But they are with respect to final EIPs. So we will perhaps get some solution and thoughts from editors, whether to merge that or close the papers.
* We will have discussions from the past meeting which will also include the EIP IRC report split. Then we'll have EIPs insight, followed by editing Office Hour and review action items from the past meeting. 

# Topic Group [0:46](https://youtu.be/KUT2cIzuu_w?t=46)
**Pooja Ranjan**
* So here the first item is topic Group. Since past few meetings we have been discussing about the split of IRC repo, and currently this is in work in progress. I know in the last meeting we discussed about having a meeting of EIPs editors to discuss more about it. Panda, if you would like to briefly update us where we are on that, and if we have that meeting, what are we planning to take care of? 

**Gavin John**
* So that meeting. So there's a few things. One, the review bot is not in a state that can be kind of like like no changes to accommodate the split will be able to be made, but or will be able to be merged into actual split repositories by the in seven days. Additionally, there is not. Additionally, we can't do the website updates on our own.
* We have to actually get some people from the ethererg team in order to do that. As such, really, the only thing things we can do during that meeting are actually split the repositories and transfer a bunch of requests. 

**Pooja Ranjan**
* Just to be clear for you mentioned about we might want to have some ethererg team member to take care of certain things. I think we can have that. There is a participant. I don't see him on the call today, but he was in the last call. if you want, we can extend the invite to him and if any support from ethererg team will be needed, we can perhaps take care of that. 

**Gavin John**
* Sure we have a calendar invite. Greg, would you mind, actually, in discord DMing me or. Sam, just just your email address so that we can forward on the invitation to you. 

**Gcolvin**
* Man. I had to find my mute button and I have a mouth full of apple. An invitation to what? I'm sorry. 

**Gavin John**
* This is the meeting in seven days where we are going to be doing the actual repository split itself. None of the CI, because the CI isn't in a place where we can do the split, and we're not. We're probably not going to be doing any of the website related stuff for because we need someone to actually do the configuration stuff. 

**Gcolvin**
* And what would be my job. 

**Gavin John**
* The job would just kind of guess the reason we're having, like, just like. I imagine there's probably going to be some debate as to, well, we want this one in the ERC. No, we want this one in the ERP. And so kind of just like the more people there. actually, I guess the more people there, the more discussion there's going to be. But like, the fairer the discussion would be. 

**Gcolvin**
* And I'm so tired of this discussion. 

**Gavin John**
* I kind of agree. Like there is definitely basically working. 

**Gcolvin**
* We're basically working hard to do something I never wanted to do in the first place. 

**Gavin John**
* I am inclined to agree with you. 

**Gcolvin**
* All I could do was try to reduce the damage. 

**Gavin John**
* I'm inclined to agree with you here, but it's being done. 

**Gcolvin**
* Okay, we're talking next week. 

**Gavin John**
* We're talking next week. The time kind of Wednesday at 9 central time. That would be 10 eastern time. Like I don't know. Is it 14 UTC? 

**Pooja Ranjan**
* Yep. 

**Gavin John**
* Okay, so 14 UTC. 

**Gcolvin**
* Why don't I just say no rather than than saying maybe and saying no in the end anyway? 

**Gavin John**
* Okay. 

**Gcolvin**
* I'm hammered. We've got our seed funding, and we're trying to work every waking hour. Now we've got. 

**Gavin John**
* Funding. For what? 

**Gcolvin**
* For a startup. 

**Gavin John**
* Oh, cool. 

**Gcolvin**
* That Ethereum is only at the edges. We take Ethereum in payment, but internally it's it's nothing much to do.

**Gavin John**
* Cool. Good luck. 

**Gcolvin**
* And so I'm busy trying to build a very secure VM that can run Python. Good luck. Sam is probably giggling. 

**Gavin John**
* Anyway. Yeah. So in terms of actually stuff that would need to be done for the split, the list is quite long, considering that there is also this request to split the websites, which I'm still very firmly against and would veto if I felt that that veto would actually do anything. 

**Gcolvin**
* Why in God's name split the website. 

**Gavin John**
* Yeah I think. I, if I remember correctly. Lightclient, I'm sorry if I'm misrepresenting your viewpoint here, but the argument here is that, one it might be a little bit more work to make it happen, considering the repositories themselves will be split, there might be a bit more, and it.
* And the argument is also that the user experience would be better because you don't actually have to shift through any of the not any of the EIPs that you don't care about, which I find to be an extraordinarily odd argument, because you don't have to do that anyway if you just use the search functionality that's already available in my rewritten version of the website.
* Which light client did not accept for admittedly somewhat fair reasons, although those reasons are now outdated because the press is now in a stable release. By the way, for anyone that doesn't know what my rewritten website is, would you mind if I just shared a link to it in the chat? Okay, here we go. Come on.
* So there we are. It's just the website, but rewritten in press so that it looks a prettier and be loads faster. And C is actually in a status that we can actually develop, develop on which the Jekyll website currently nobody knows. Nobody knows how to completely like if we needed to add an entirely new plugin, I don't think any of any of us had like none of us are Ruby experts.
* I am the closest one to being able to make major changes to the Jekyll website, but even then, like. I'm not able to make that big, that that big of changes. And that also kind of goes into another problem with what splitting the website would entail. 
* And that's that. Well, there's nobody to maintain the EIPs side of the website. They need to find someone to learn, probably an entirely new language. Guess there's around three. Sorry. What? 

**Gcolvin**
* What possible objection is there to this? 

**Gavin John**
* I really don't know. I wish my client was here. What? 

**Gcolvin**
* I mean, what do they want to split from What? 

**Gavin John**
* They want to have? ethererg and ERC ethererg. 

**Gcolvin**
* Like we have six panels here and they don't like one of them. 

**Gavin John**
* Is anyone here in favor of having two websites? And if so, would you mind speaking up? 

**Victor**
* I am in favor of having two website, not because I want to have EIP and ERC showing up on to website I generally am in favor of. Competing of like having people of people have access to different approach to see what to see. And so I want ERC and EIPs to show up with just one of them. 

**Gavin John**
* That that's possible with just one website though. Can I can easily change. I can easily just change the layout file or create a different layout file that changes depending on whether or not it files in the EIP repository or ERC the repository.
*  This would require about ten lines of code. Why would anyone like me to go ahead and get the framework there so that so that we can have a kind of. I Geth Repository dependent layouts. 

**Sam**
* I think you're kind of debating a ghost right now because, like, I want to. 

**Gavin John**
* Yeah. 

**Sam**
* Do the split. So I think we can just table this until the actual meeting we have with Matt next week, and then. Yep, we can hammer all this out then, because I don't think we're going to make any progress on it without Matt here. 

**Gavin John**
* I guess. Can we move on to number 273? The deadline passed and everyone has voted yes. Doesn't that mean that the form has now been reduced to the three yeses and it passes? 

**Sam**
* Yeah. So yeah. So we're going to stop talking about ERCs and EIPs for now. And then 273 is the next open thing. We have one too. Yep. So yeah this one we can close. Everybody who's everybody who has said something on it has agreed with it so we can close it.
* The actual pull request implemented I think was already merged, so it's kind of pointless.
* So 274 let's take a look at that one. So this is renumber EIP-5000. All right. So you have vote no. Okay. This is a fun one. This is the renumbering, the EIP. So. does anybody have anything they want to add on renumbering EIP-5000 before we stop talking about it forever? 

**Gavin John**
* Well, I mean, there's no consensus yet, so it's not clear. So it's not close. The deadline is passed, but that just means the form is reduced to the number of active people, and there's two yeses and two nos. 

**Sam**
* So we don't need unanimous, right? That's kind of the whole point of having the keeper of consensus. 

**Gavin John**
* Yeah, we don't need unanimous, but we do need consensus. And the keeper of consensus can only decide when consensus has been reached. It evidently hasn't because it's tied. 

**Sam**
* It's tied on votes. Right. So we have to for renumbering one against and then Victor. You're in support of renumbering and then I'm in support of renumbering. So I mean, I if nobody else has anything to add here, I would say that this we we would merge it. 

**Gavin John**
* So I'm just going to reiterate and kind of summarize the points, kind of I believe that are foreign against it for renumbering it so that it kind of sets the precedent that if you find a loophole that like, allows you to do something like renumber your EIP, do something nice, or like any other loophole that you get to kind of abuse it. 
* It also, I guess, kind of makes the editors look bad for like accepting what could be considered some form of like preferential treatment. The arguments against renumbering and I am against renumbering is one it wasn't actually against one at the time.
* Two, yes, and to the correct thing to do in response to something like this is to modify ERP-1 to prevent anything similar from happening in the future.
* Would you say? Would everyone here say that's an accurate categorization of both points? 

**Sam**
* I think that's reasonable. Yeah. 

**Gavin John**
* Does anyone have anything to add? I guess I'd have one thing to add to the no. And that's that we can't set the precedent that rules can be changed retroactively, which I think we I think we should set the precedent that if something is okay at the time it's done, we can't just subsequently be like,  that doesn't feel right.
* We can't have that and punish kind of punish someone for something that was totally okay when they did it. Was was anyone's way to buy either part. 

**Sam**
* I'm still in favour of renumbering. 

**Gavin John**
* I still against renumbering. 

**Sam**
* All right with. No other comments assuming nobody else wants to make them. And the comments on. The pull request being the latest, I will go ahead and merge that pull request. 

**Gavin John**
* Well, it's still tied 33. There is no consensus here. Yeah. We've got you voting. Yes. Remember? We've got me voting no. We've got Lightclient voting no. we've got Victor voting. Hold on. Victor voting. Yes. We've got a abo Gallup. I totally butchered his name. Probably voting no. That's three. Three. 

**Sam**
* I didn't think they were. 

**Pooja Ranjan**
* So we are we are considering editors voting here only, right? Yeah. 

**Gavin John**
* Oh, well, then we have you. You? Yes. Me? No. is is G11 governing or not? 

**Pooja Ranjan**
* He is an editor. 

**Gavin John**
* Yes, but is he a governing editor or not? Basically, does he have voting power? 

**Sam**
* Oh, yeah, there's that whole debate. Where do we land on that? 

**Gavin John**
* I think we land. I think we landed that anyone. Well, the intent was that anyone in the governance section of the ERP editor's dot yml file has a vote. 

**Sam**
* All right. 

**Pooja Ranjan**
* So does it mean that, like we recently had voting for who can be editor? So whoever are selected in that list and continues to serve as an editor should have this governance power, like governing power and his vote, his or her vote should be counted. So. 

**Gavin John**
* And so I think there's kind of either two ways of like there's two ways of doing this. The reason why the ERP review bot can merge pull request and merge pull requests is that delegated it the power to do so. the config file itself is just a representation of who has the power to do what. And in and of itself, the peer review bot delegates some of its power to the people in that file.
* And so I guess we can work backwards and say that therefore anyone in the governance section is an editor. Anyone that's not is for the purposes of the ERP one definition of editor, not an editor. And for the purposes of are they really an editor? Yeah, they're an editor. So it's. Confusing and probably should be made more clear. 

**Pooja Ranjan**
* I agree to that. I think for the time being, if people are open to accept this concept, perhaps what we can do is apart from bots, let's talk about human here. Whoever are EIP listed as editor in one should be considered for voting.
* And they're like, you know, their opinion should be mattered for at least for this call for input process in place is my suggestion here. I don't know what other people think. 

**Gavin John**
* So it is up in the air whether or not people that are in the government section or not in the government section can vote, because for one thing, we had all those culvert embeds for editor removals at the Sam Oakland. And one argument could be made that when people were voted either kind of yes or no to having them removed as editor when it was voted no, they aren't removed as an editor.
* That kind of implies that they are an editor according to the charter and therefore can vote. The other argument is they can't actually have any effect on whether or not. Peers that modify a living EIP, such as EIP-1, are merged or not. The intent.
* When the intent, at least according to light client that when Victor was brought on as an editor. I was that he couldn't have a vote. I don't know if that's still the case.
* I would argue that we should have a vote. He has clearly demonstrated that he is a very competent, very engaged member of the project and probably and almost certainly deserves a vote. In fact, everyone in the ERP Editor supplemental file I believe deserves a vote. Yeah. 

**Sam**
* I think everybody listed on EIP-1 should be the set of editors. That's the only thing that works for me. 

**Gavin John**
* I mean, guess. I guess the best thing to do here is create a call for input that that's for. Hey, let's define. Let's define kind of an EIP editor as well. Let's, let's define the initial set of editors right that have voting power. And from there we can use the editor add removal process to keep that list up to date. But, Jessa, that we're on the same page as to what the initial list of editors is.
* Mean again, there were all the there were all those, there are all those office for editor removals that you opened. Yeah. 

**Sam**
* And so everybody survived. So I think yeah, everyone survived. 

**Gavin John**
* But more to the point, Even Lightclient voted no, let's not remove, Victor as an editor, which strongly implies that. Victor was an editor and still remains an editor. Yes. 

**Sam**
* So I've been operating under the assumption that our EIP one is our governance document. And the editors listed there are the editors. But yeah. 

**Gavin John**
* There are think. 

**Pooja Ranjan**
* Think we should continue like as long as possible to have that as governance document. And it is listed in the EIP one is I mean our editors. The one caveat here was, which I understand is like they may or may not have permission to merge the pull request. That is, I think, a separate topic.
* We can perhaps talk about it, but as long as governance is involved, especially if we talk about Victor's case, the only thing for him was that he would not be maybe actively involved for core EIPs, but other than core EIPs, he was definitely involved in every other set EIPs interface except PRC. 

**Gavin John**
* Except he's not listed in the governance section. the editors dot yml file. 

**Pooja Ranjan**
* And that's because that's maybe because, you know, we do not have a specific merging power for as of now. But I hope that would be fixed. When we have. 

**Gavin John**
* We do we do actually have a separate section for emerging ERCs vs. Interface versus networking versus core versus informational versus meta. There is actually very fine grained detail in review for this stuff. 

**Pooja Ranjan**
* Can we can we have respective PRs? Victor. Maybe we can have that. And let's see where we are now. I know things were different in the past, but a lot have changed in over a period of two three months. 

**Gavin John**
* Okay. For the purposes of this meeting, let's just consider all of the all of the editors in EIP-1 to be voting editors. In that case, wouldn't the PR to renumber 5000? Either it would be 43in favor of renumbering or 33 tied. Either way, I'd say arguably there is not the rough consensus needed for the keeper of consensus to determine that consensus has been reached. 

**Sam**
* Again said that. 

**Gavin John**
* Because there's about just under half of people that disagree with it. That's. Not consensus by any stretch of the imagination. Oh, like rough consensus. 

**Sam**
* It can be right. 

**Gavin John**
* What what is the definition for rough consensus here? Because I thought that rough consensus was like, okay, there's a there's a few objections, but we need to get this merged anyway, even though that there are some objections, we can sort them out later. Not half of people actually just don't want this and are strongly opposed to it. 

**Sam**
* So I can read it here. So working groups make decisions through. 

**Gavin John**
* Basically. 

**Gavin John**
* But basically, I didn't think that the keeper of consensus had the power to determine what consensus was. 

**Sam**
* That is there? Well. 

**Gavin John**
* I thought it was to determine when consensus has been reached. 

**Pooja Ranjan**
* So I think it is there for a reason. Like all editors are putting their faith in the keeper of consensus, so whatever decision at the end is made, should be acceptable by the group. At the same time, definitely there should be a valid reason for going ahead with it.
* Like the decision making rough consensus could be like, you know, even if it's like kind of very close tie or not. All of the editors may have voted.
* So there are some grey area that we are giving permission to the keeper of consensus to maybe take a decision there. 

**Gavin John**
* Okay, just one quick thing before we re-emerge. The 5000 renumber PR. You are aware that this effectively does set the precedent that we can retroactively change. Yep. ERP One. Right. Like say like say okay. That is basically even though that was allowed, then it's no longer allowed. Because that is the precedent that's set here. Yeah. I think the. 

**Sam**
* Precedent that I'm setting is that the EIP editors can do whatever the hell they want, whenever they want, but these are generally the rules we're going to follow. 

**Gavin John**
* That to me doesn't seem. Well. That is kind of not the precedent I'd like to set, but okay. 

**Pooja Ranjan**
* Yeah, I mean, I know my vote does not count here, but what I meant to say here is like EIP editors can or should do the numbering thing before the PR is merged as draft. I kind of agree with the. 

**Gavin John**
* The PR is already merged. Yeah. So the EIP is already merged with the number 5000. 

**Pooja Ranjan**
* Yeah, kind of late for that. Maybe we can have this process. Yeah. Please go ahead. 

**Gavin John**
* I mean, I guess. The best thing we can do is wait for it to go stagnant. And I mean, I'm kind of of the opinion that if like at some point we should start deleting stagnant IPS, right? They're still they will still remain in the git history, but we don't need. Say, three year old stagnant pipes in the repository and still being published.
* And I feel like we should set a threshold for that. And then problems like this will just go away once.
* Once they go to stagnant and then they go too, because the authors of 5000 have simply gone AWOL, they're not maintaining it. They're quite a. 

**Pooja Ranjan**
* Core proposal, right? 

**Gavin John**
* That's what. 

**Pooja Ranjan**
* That's a core proposal, right? 

**Gavin John**
* Sorry. Couldn't catch the core or. Cool. Yeah. 

**Pooja Ranjan**
* Yeah. Core. yeah. I'm just wondering if that proposal is enacted pursuant anymore or not. 

**Gavin John**
* I quite frankly, I think it's I mean, considering that no progress has been made on it. I'm not I'm kind of not in favor of renumbering, but but I'm actually starting to get in favor of just deleting it just because, like. Well, deleting it once it reaches stagnant, they the process shouldn't be too hard for them to just submit another.
* The So basically do we accept kind of a once the proposal stagnates, then it gets deleted as kind of a compromise. No. Okay. 

**Sam**
* No

**Gavin John**
* Even stagnant ones. 

**Juan Caballero**
* Delete from repo or just not display on the rendered version. 

**Gavin John**
* Actually delete from the repository, but it remains in the Git history. 

**Pooja Ranjan**
* I think that would not be fair to many authors, because getting stagnant is a status people can bring back. They can resurrect. If we start deleting, they will lose this opportunity. 

**Gavin John**
* Okay, how about this, though? The sense of these ERPs are still in the git history. Why don't we? It's therefore possible to verify as verify whether or not a particular proposal was stagnant or not. That doesn't mean we need to actually keep all the stagnant, stagnant ERP actually in the repository. We just need to have it possible have it have a kind of a workflow for stagnant ERP to be brought back from stagnant.
* But I don't think we need to have the ERP number therefore still reserved. We just need to kind of have. Have a process to bring those back. 

**Sam**
* I think this is a little off topic from whether we're remembering. Agreed. 

**Pooja Ranjan**
* Yeah, this is like way off topic. We should get back for today's like, you know, this proposal for. 

**Gavin John**
* I'll create a proposal. but yes. Can we therefore agree that there's not actually like. Okay, guess. I guess we have different definitions of rough consensus. My interpretation of what rough consensus meant was that, okay, it like. Like, we kind of like there might be some opposition to certain parts of it, but it's still not too dissimilar from what we originally had, which was anyone can veto it.
* Instead, now it's any anyone can kind of like raise objections.
* And once the cube of consensus has determined that those objections have been kind of sufficiently dealt with. Do you feel like your. 

**Sam**
* Objections have been heard? I guess is the important part here. 

**Gavin John**
* I feel that my objections have been heard, but I don't feel that they've been completely understood. Like I feel like. I feel like the implications of like the we can just do whatever the heck we want. Haven't been completely thought out because like.
* I will say, like career wise, the reason that there are career ERP is because the process is considered to be, at the very least, somewhat fair that the that the editors are bound by certain set of guidelines that they have to accept proposals and that like basically there's kind of a certain degree of legitimacy that is kind of earned by not doing whatever the heck we want.
* And so that's kind of why I feel like we should not set the precedent that we can do whatever the heck we want. 

**Sam**
* I do. I hear what you're saying, and I think I understand what you're saying. And I think we should endeavor to be the most fair and just that we can. 

**Gavin John**
* Would you say that? That given that the rules were what they were at the time, it is fair to. Kind of change in ERP number, even though there was nothing that was technically done that was wrong at the time. Sure, there was controversy and now we would consider it if it happened today to be wrong and probably worthy of remembering. But at the time it wasn't against the rules. 

**Gcolvin**
* So why are we wasting time on this? What's done is done. Just let it go and move on. 

**Gavin John**
* What has been done. 

**Gcolvin**
* A number got assigned to a document. 

**Gavin John**
* Yeah, a number got assigned to a document. 

**Gcolvin**
* So. 

**Gavin John**
* Well, I mean, the the argument for renumbering is, I'm sorry. 

**Gcolvin**
* I've heard the arguments that they go around and around that it wasn't against the rules when it happened. It wasn't a big deal. Changing the number just is. More confusion is taking a lot of our time. we spent more time arguing about numbers than anything else. 

**Gavin John**
* Well, the reason why we are currently debating it is because Sam feels like consensus has been reached, and I do not feel that consensus has been reached. 

**Sam**
* Well, now that Greg has said something, I feel the consensus is going the other way. 

**Gcolvin**
* Yeah, I slept really badly last night, so I'm slowly waking up to what the issue is on this one. 

**Gavin John**
* So we are now tied. 

**Gcolvin**
* Generally on like 44. Top with it. 

**Sam**
* So, Greg, your opinion is that we leave it as EIP 5000. 

**Gcolvin**
* Yeah. 

**Sam**
* Just who cares? 

**Gavin John**
* So now we are tied for 44. 

**Sam**
* So I'm just going to. We've spoken way too long on this. I am saying officially as keeper of consensus that we are closing this pull request. Consensus is to not change it. 

**Gavin John**
* It's okay. 


# 275 Call for Input: Allow links to the Yellow Paper [37.08](https://youtu.be/KUT2cIzuu_w?t=2224)
**Pooja Ranjan**
* All right. With that, we can move on to the next number. That is 275. Most of them suggested. Yes, and the deadline has passed. 

**Gavin John**
* But being. Let us both reiterate. Why think it's. I mean, I say yes because it meets the requirements set forth in ipsum five 275. 

**Pooja Ranjan**
* I'm sorry, I think I just missed. Can you please repeat? 

**Gavin John**
* It meets the requirements for an acceptable source. Like I get that. Lightclient says it has not been updated for several forks, and that bringing it up to date post merge would be a huge effort.
* That doesn't change the fact that it is free. It's a free source and commits are immutable and therefore this meets the requirements to be accepted. 

**Pooja Ranjan**
* Them. Would you like to maybe just confirm or if you have other thoughts? 

**Sam**
* Sorry, I'm just updating my notes here. Give me one second. 

**Gavin John**
* The problem is that, again, the Lightclient is the only one that's saying no here. And he's not on the meeting. 

**Pooja Ranjan**
* And the date has passed. That's one other important thing here. So whatever thoughts and like voting has been collected can't be. 

**Gavin John**
* Again the deadline only set. The deadline is only there to make sure that things will eventually pass. Basically that. If someone most likely acts like if we're going to be totally honest at the moment. Doesn't actually vote on something that it's not held up until say Alex or whoever doesn't vote starts to vote on. 

**Sam**
* Greg, should we allow links to the yellow paper? Yes or no? 

**Gcolvin**
* Yes. Okay. 

**Gavin John**
* I would say there's a strong enough consensus, I guess. Victor links the yellow paper. 

**Victor**
* I strongly in favour. 

**Gavin John**
* Okay, that seems pretty strong consensus. 

# Call for Input: Updating EIP-4804 (Web3 URLs) #276 [39.41](https://youtu.be/KUT2cIzuu_w?t=2381)
**Pooja Ranjan**
* All right, so we can close it by marking it. Yes. And the next one is number 276. I'm sharing the link right here in the chat. Oh added 275. Command v six. Okay. So this is for for 804 web three URLs updating. EP 4804. 

**Gavin John**
* So what happens when the quorum gets reduced to zero? Editors. 

**Sam**
* That's a good question. 

**Pooja Ranjan**
* We did not receive any input in this one. 

**Gavin John**
* The form is now zero. Editors. 

**Sam**
* Oh, that was the 4804. Let me let me develop an opinion on this quickly. 

**Victor**
* Shall we have a different between consensus? Yes. Consensus. No. A third kind of status, which is no consensus. And we will table this until certain time. I think it's just keeping an issue. 

**Gavin John**
* Open that's literally just keeping the issue open. 

**Pooja Ranjan**
* I think there is a respective PR for this particular case. We can let the PR be there and get stagnant. If no one is coming up in strong favor or strong against, especially from the editors communities for this particular topic. 

**Gavin John**
* Wait. Hold on. This is just adding an. Why does this require consensus again? 

**Victor**
* Yeah. 

**Pooja Ranjan**
* I think because that is. 

**Pooja Ranjan**
* Final EIP. Yeah. 

**Gavin John**
* No it's adding a new EIP. Yeah. 

**Sam**
* So the EIP that, that pull request used to be editing an EIP and they changed it to adding a new EIP. 

**Gavin John**
* So this doesn't require consensus anymore. No not. 

**Sam**
* Anymore. 

**Gavin John**
* Okay. We can just close that sentences right. 

**Victor**
* Yeah. 

**Sam**
* Just just close that.

# Call for Input: Accidental function in ERC-223 #283 [42.31](https://youtu.be/KUT2cIzuu_w?t=2551)
**Pooja Ranjan**
* We are at least reaching on decision and moving faster. The last one here is active actually 283 that was opened yesterday. It's about accidental function. In ERC 223. I see that there are already some inputs there. Want to discuss or have thoughts here? 

**Gavin John**
* That is my chat. Yes it is. I was the one that opened it. or rather opened the PR. so basically when reviewing the adding, the kind of adding your ERC 223 as an actual, it used to just be a GitHub issue and not a real EIP. I've noted that effectively there was this function standard that was just out of scope of the.
* The ERC 223 is a standard for kind of a, a standard that is designed to address some of the problems that ERC 20 has.
* And one of the functions that your ERC 223 originally had was standard to kind of differentiate between whether or not the token was an ERC 20 token or an ERC 223 token, because otherwise they might look somewhat similar.
* I said that that that was out of scope for the because, well, it's not an interoperability and you can just use one of the other ones available like 165 or a victor's ERP for interoperability and Dexter.
* And agreed, because it is in fact out of scope for the EIP in a later PR dexron kind of either mistakenly included the function again, or forgot and kind of forgot that it was removed, or. I guess the the PR itself kind of suggested that. 
* Like he had a slight misunderstanding as to what my objection actually was, and it got put into the ERP into the again the became final. But with the actual function that should have been removed still there. And so my PR is suggest remove the function that's out of scope and not sufficiently defined. Because it says identifier.
* I'm using air quotes because identifier is not defined anywhere. Only that the identifier for 2 to 3 is some string. So it can be it can be used sometimes to detect whether or not something is or ERC 223 it. It is an odd standard, but I could see it being its own EIP. But it does not belong in ERC 223. 

**Pooja Ranjan**
* I guess the question is anyone opposed to this? We still have some time to collect inputs from other editors. Whoever, not whoever have not submitted their. Response. Here I see Sam, Panda, Vector and Gajendra Singh have already added their thoughts. Gavin. Sorry Greg, you have any thoughts on this one? 

**Gcolvin**
* Not really. They're not yet. 

**Pooja Ranjan**
* All right, so the deadline date is November 16th. I know there are more editors, Matt and Greg. They have not added, if anyone has any thought, perhaps they can go ahead and add it. The issue number here is 283. 

**Gavin John**
* So, Greg, do confirm that you are abstaining. 

**Pooja Ranjan**
* I think we can wait till the end of the day. If it does not come back, we can consider that as. Yeah, abstaining. 

**Gavin John**
* Greg, you said you don't care, right? So that's an abstain. I just want to make sure that we have as many votes as we can, whether or not they're for or against. Again, this deadline thing is is was more designed as a encase like an editor just is not available and is not designed to be the default thing. We're trying to get everything. 

**Sam**
* The default should be. Everybody just gives their opinion as soon as possible and we can move on and that. 

**Gavin John**
* That's why I'm asking Greg whether or not he's abstaining or not. 

**Pooja Ranjan**
* I mean, this was just opened yesterday, so we can perhaps give some time for people to, like, get the idea, realize the concept. And yeah, in case we do not hear back from Greg and others by the next meeting, we can see where we are or before the deadline. Totally got the concept of having a deadline.
* Deadline definitely helps us move past an issue, giving sufficient time for people to come back with their for and against argument. 

# Update EIP-5773: fix typo ethereum/EIPs#7866 [48.18](https://youtu.be/KUT2cIzuu_w?t=2898)
**Pooja Ranjan**
* I think we are running out of the time today, so let's try to move fast a little bit. I have listed a few open pull requests next, which are the, you know, two final tips. If anyone have thought on it like the first one is PR number 7866, which is changing EIP 5773, it says that it is a typo fix. Anyone objects to that. 

**Gavin John**
* No, it is in fact a typo fix. 

**Pooja Ranjan**
* So we are good with that merging. 

**Gavin John**
* So all of these are just fixing typos that where people have misspelled overwritten, apparently. 

**Pooja Ranjan**
* Yes. So we can perhaps take a look and close at least all these bars. We have a lot number of open PRs these days. 

**Gavin John**
* This one's for lifetime. Thank you. Whoever has opened all these PRs for submitting these PRs. 

**Sam**
* It feels like Bots doing this. It does feel like. 

**Gavin John**
* Bots doing this. Am absolutely fine if bots do this. However, this is constructive. 

**Victor**
* There was one time. Oh, wow. So many. Different persons submitting a report of a typo change. 

**Gavin John**
* Yeah, I'm almost certain these are bots, but that's fine. They are completely valid suggestions and deserve to be approved. So. Whoever, whoever made these bots, I think. Yeah, that's. Thank you. 

**Victor**
* I am in favor of having bots fixing this. It's. And and I thought there was one person who submitted a very long list of typo fix of a lot of. And I suggest them to split them up into different ones. The concerning part here, so I'm generally in favor of that.
* But concerning part is that I noticed that typos fixing are coming from different GitHub accounts. Did you notice that? 

**Gavin John**
* Yeah, I noticed that too. It could be. 

**Victor**
* Farming. 

**Gavin John**
* I quite, quite frankly, that's GitHub's problem, not ours. 

**Victor**
* They become our. They become our contributor. 

**Gavin John**
* They do become they do become contributors. 

**Victor**
* First one. 

**Gavin John**
* There. Is that a problem, though? 

**Victor**
* I'm not sure it could. 

**Pooja Ranjan**
* Yeah, it could in future like unless that is a significant contribution. Just a typo contribution could make them look like a contributor and can be, you know, potential scammer or something like that. I'm not saying that this person or this bot is actually, but that is a possibility. 

**Gavin John**
* So we we don't have any evidence. This apart from the fact that the PRS were submitted close to each other by different user accounts with the same, with the same title, which definitely doesn't look good. But again, this is kind of anecdotal evidence and doesn't actually. So these are basically these are all kind of valid things.
* And I'm pretty sure that like again, this is actually kind of the contributions we want. Right.
* These are exactly the kind of contributions we want people to do. And also if they're if they're kind of doing CI for us is not necessarily a bad thing. 

**Pooja Ranjan**
* They could suggest. One thing here is like maybe checking out that GitHub account of these resources. Like if that is completely empty, then it could be a bot and could be a possible scammer. But if they are not, just like for example, I'm looking at 7840, I don't know. 

**Pooja Ranjan**
* I'm looking at. Yeah. And it sounds like they are genuine. Not kind of so bad. 

**Gavin John**
* So I'm looking at issue 186. They actually have the pull request shark badge. And so to me, this definitely looks like a bot that has probably just submitted a bunch of typo fixes. 

**Gavin John**
* The let's see and get the actual web view for this. This. 

**Pooja Ranjan**
* Well, we are running out of time. I would like to get this thing, you know, under the radar of EIP editors. Maybe they can take a look and respond. I've already. 
* All right. So hopefully those those will be merged. Auto merge. If not. And if manual merge will be required we can bring it back. I know there are a lot many other discussion point which we could not be able to take today.
* I'm just curious about one, action item or decisions from the past meeting about superseeding comment Panda, did you get a chance to maybe take a look into it?
* I suppose the decision was that you would be coming up with some pull request for that. 

**Gavin John**
* Yes. That, I can't remember. Did I come up? Did I make the pull request or not? I'm pretty sure I did. 

**Pooja Ranjan**
* In case you did. Yeah, in case you did not, or even if you did, it would be nice to have it added to the agenda for the next meeting. We can perhaps take it in the next one because we are out of time to discuss it here. Any final comments thoughts from people they would like to share it today. 

**Gavin John**
* I mean, yeah, the split meeting is going to be in a week. I'm interested to see how this goes. 

**Pooja Ranjan**
* Absolutely. And will DM you the email address of the resource from ethererg if you would like to invite him for the meeting. If you think it is needed, then only I will share the details with you. 

**Gavin John**
* Well, everyone on this meeting has disagreed with splitting the website now, or have at least determined that there is a better alternative available. 

**Pooja Ranjan**
* I see your point. Okay, in that case, we'll wait till the result coming up from the meeting plan on next Wednesday at 1400 UTC. By editors. Well, thank you all for joining us today. Hope to see you around. Have a good one everyone. 

**Gavin John**
* Thank you very much. Mhm. 

---------

## Date and Time for the next meeting

Nov 01, 2023 at 14:00 UTC

---------
## Attendees

* Pooja Ranjan
* Victor
* Gcolvin
* Sam
* Gavin John
