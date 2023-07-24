# EIPIP Meeting 85
### Meeting Date/Time: Wednesday, July 12, 2023, at 14:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/248)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=dapg2BAmCI8)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION/DECISION  ITEMS

**ACTION 85.1**: PR 7295 ,7261 and 7183 have changes to the Final proposal. Sam will take a look and respond. 

**ACTION 85.2**: In regards to [ethereum/EIPs#7230](https://github.com/ethereum/EIPs/pull/7230),Some of the editors were not in agreement with the proposed change to EIP-1 wrt EIP number allocation. Also @gcolvin agreed to split the PR and will be revisited in the next call. Needs to follow the [recording](https://www.youtube.com/watch?v=dapg2BAmCI8&t=622s) as it was a long discussion. 

**ACTION 85.3**: In regards to Progress on Bots, EIPw will work fine if the same config is kept on the other repo. Also if we create a new repo and have new secrets for that repository for eth-bot then it will work  fine.

—------------------
## AGENDA

**Pooja Ranjan** [0:11](https://www.youtube.com/watch?v=dapg2BAmCI8&t=11s): Welcome to EIPIP meeting 85. We have agenda issue number 248 at EIPIP GitHub repository for discussion. We have some EIPs which are already in final status and there are respective PRS to make. some changes in that will be discussing the issue of EIP and ERC GitHub repository that we have been discussing for past few meetings and I can provide updates on EIPs inside and maybe followed by EIP editing office hour.

# 1. Discuss Open Issues/PRs, and other topics

## Changes to Final proposals

### Update EIP-5169: Fix uncompilable memory in event ethereum/EIPs#7295 

**Pooja Ranjan** [0:49](https://www.youtube.com/watch?v=dapg2BAmCI8&t=49s): So starting with the first item listed on the agenda changes to final proposals. The first PR here is a 7295. This seems to be a small change but it's a keyword in the spec. I suppose the user is trying to remove the word memory here. Wondering what editors think. can we merge it or do we have to say no.

 **Sam** [1:20](https://www.youtube.com/watch?v=dapg2BAmCI8&t=80s): If it was valid solidity when it was written then we should probably keep it.  If it's invalid solidity then it's fine to change it.

**Pooja Ranjan** [1:33](https://www.youtube.com/watch?v=dapg2BAmCI8&t=93s): I am not sure if we have anyone from salinity to confirm that?

**Sam** [1:42](https://www.youtube.com/watch?v=dapg2BAmCI8&t=122s): Yeah I'm checking right now.

**Pooja Ranjan** [1:52](https://www.youtube.com/watch?v=dapg2BAmCI8&t=132s): Could we move on to the next item, and I just wanted to bring it to my attention.

**Sam** [1:58](https://www.youtube.com/watch?v=dapg2BAmCI8&t=138s): Yep

### [Update EIP-6059: Clarify the backwards compatibility section ethereum/EIPs#7261](https://github.com/ethereum/EIPs/pull/7261)

**Pooja Ranjan** [1:59](https://www.youtube.com/watch?v=dapg2BAmCI8&t=139s): Perfect, so the next one is a PR number 7261 it is a change proposed to EIP 6059. This also seems to be a small change. The author here is willing to add a sentence which is like you know when this proposal may not be good and it's just a statement to like.  Let implementers know about it no spec changes here again the pr number is 7261

 **Sam** [2:48](https://www.youtube.com/watch?v=dapg2BAmCI8&t=168s): I'll have to think about this one but I'll keep it open perfect

**Pooja Ranjan** [3:00](https://www.youtube.com/watch?v=dapg2BAmCI8&t=180s): Okay, before we move on I see we are joined by more editors here. so just to let people know that we have already taken up two PR's 7259 and 7261 those are proposed changes to funnel eips if you guys have any thought comments or objection on that PR,  please add as a comment so we can close it and we can also inform the author and if it seems generally good and not a big change we can perhaps merge that.

### [ Update EIP-2612: Make consistent indents in json ethereum/EIPs#7183](https://github.com/ethereum/EIPs/pull/7183)

**Pooja Ranjan** [3:36](https://www.youtube.com/watch?v=dapg2BAmCI8&t=216s): Moving on to the last proposal here the PR number is 7183. It is a change to EIP 2612. it seems a bit confusing because I'm not sure if the proposal is just trying to adjust the space or too much changes into it. So it would be really nice to have. Let us take a look at it and maybe respond.

**Sam** [4:14](https://www.youtube.com/watch?v=dapg2BAmCI8&t=254s): Will do.

# 2. Discussion continued or updates from past meetings

### EIP-ERC GitHub repositories?
### Ref: [Task list for ERC/EIP Split](https://hackmd.io/A1zfRkO7RKKV6BIaSXpcbw)

**Pooja Ranjan** [4:16](https://www.youtube.com/watch?v=dapg2BAmCI8&t=256s): Thank you. All right moving on to the next item which is discussion continued from the past meeting. we have EIP ERC GitHub repositories split that we were discussing. So for a quick recap. Lightclient opened a PR 7206 to split the GitHub repository in the last meeting we were evaluating the effect of split on ERC community.  Victor and ERC editor wanted to have this proposal shared with ERC Community via all ERC Dev meeting and respond back in
today's meeting and in the meanwhile we were to assess the functioning of existing and the
process for the new repo. Juan pulled up the task list for ERC EIP split. It's in a hack MD which is also added to the agenda and he also mentioned that he is willing to volunteer on the editorial board post split. I don't see William. I'm sorry I don't say Victor on the call today but he has already updated on the Discord that he had a meeting of all ERC Dev and it seems like ERC developers or authors are not strongly opposing this split. They are generally okay with whatever the process is. They just want a clear communication so it can be followed. Yeah with this perhaps we can start sharing updates and add comments and I suppose it would be a good idea to take a look at the hack MD and discuss next steps to get volunteers for specific actions. I don't know Juan if you would like to maybe talk about the document and share the next steps yeah and yeah perhaps update all of us.

**Juan Caballero** [6:24](https://www.youtube.com/watch?v=dapg2BAmCI8&t=384s): I don't have very strong opinions about the process. I was trying to just sort of as The Outsider play secretary and just write down ideas I saw in different threads in different places on the across the Discord additions and the PR threads and I don't necessarily you know I'm unqualified to own it or to mediate if people disagree with any of the items I was just trying to throw it together to have you know a draft to work from if anyone has strong opinion, the hack MD hopefully is not access controlled and anyone should be able to change it.
 
**Light Client** [7:13](https://www.youtube.com/watch?v=dapg2BAmCI8&t=433s): yeah I mean thanks a lot for making that hack MD I was yeah pretty useful. There's a lot of stuff that was kind of like outlined in different places but yeah putting it all together here so that we can see that it was an  awesome thing.  Thanks 

**Juan Caballero** [7:27](https://www.youtube.com/watch?v=dapg2BAmCI8&t=447s): But maybe Pooja , the request that I walked through line by line or or item by item or just overview it.

**Pooja Ranjan** [7:39](https://www.youtube.com/watch?v=dapg2BAmCI8&t=459s): I was wondering if you know what would be our next step. It seems like we do not have a strong opposition to go ahead with the split so what would be the right Next Step to begin this process I understand from Sam's comment.

**gcolvin** [7:54](https://www.youtube.com/watch?v=dapg2BAmCI8&t=474s): I've expressed strong opposition blocking opposition over and over and have not changed. 

**Light Client** [8:02](https://www.youtube.com/watch?v=dapg2BAmCI8&t=482s): We decided last call that we're just going to go ahead and do it regardless this is blocking 

**gcolvin** [8:09](https://www.youtube.com/watch?v=dapg2BAmCI8&t=489s): I will resign. This is blocking. I will resign.

**Lightclient** [8:15](https://www.youtube.com/watch?v=dapg2BAmCI8&t=495s): you made that clear last call.

**gcolvin** [8:17](https://www.youtube.com/watch?v=dapg2BAmCI8&t=497s): Okay this if the other editors are willing for me to resign over this issue I will resign

**Pooja Ranjan** [8:27](https://www.youtube.com/watch?v=dapg2BAmCI8&t=507s): Okay  I do have Greg's proposal added as the next item. I am fine going over that because if I remember correctly like mentioned that if we take a look into his PR that perhaps will help him you know get motivated to you know think about it and it will solve some of the issues. Do you think that would be a good approach to First discuss that and we can come back on this hack MD after that issue.

**gcolvin** [8:56](https://www.youtube.com/watch?v=dapg2BAmCI8&t=536s): I've made clear that my opposition is not to splitting per se my opposition is for splitting without a plan. For how that split is actually going to help the problems that we have 

**LightClient** [9:11](https://www.youtube.com/watch?v=dapg2BAmCI8&t=551s): We've outlined how it's going to help but you don't like you know what we've said that is going to improve the situation.

**gcolvin** [9:19](https://www.youtube.com/watch?v=dapg2BAmCI8&t=559s): I believe it will cause more harm but I don't want to have that.

**Lightclient** [9:23](https://www.youtube.com/watch?v=dapg2BAmCI8&t=563s): Yeah but then again we have given reasons that it's going to improve the situation. Well you just said that we haven't. We said that we're going into this without a plan and we do have some specific thing.s we think it's going to improve and whether or not you think that those are useful that's like a separate discussion but like we do have some plan.

**gcolvin** [9:46](https://www.youtube.com/watch?v=dapg2BAmCI8&t=586s): I'm not finding it adequate. That's  why I've made the pr to indicate the direction of a plan that makes sense to me. we can discuss this or not.

**Pooja ranjan** [10:03](https://www.youtube.com/watch?v=dapg2BAmCI8&t=603s): Okay I think that is the next item on the agenda. so if you would like we can perhaps discuss the pr that you have suggested and then we can come back on the hack MD. All right so let me bring up that 

### [Update EIP-1: EIP pain relief ethereum/EIPs#7230](https://github.com/ethereum/EIPs/pull/7230)

**Juan Caballero** [10:24](https://www.youtube.com/watch?v=dapg2BAmCI8&t=624s): Sorry, quick quick question point of order is screen sharing distracting or this is not really the standard way to do this. I just sort of default to screen sharing anytime I talk in any kind of meeting. 

**Lightclient** [10:36](https://www.youtube.com/watch?v=dapg2BAmCI8&t=636s): I think we're too lazy to screen share usually.

**Juan Caballero** [10:38](https://www.youtube.com/watch?v=dapg2BAmCI8&t=638s): Okay okay cool.

**Pooja Ranjan** [10:41](https://www.youtube.com/watch?v=dapg2BAmCI8&t=641s): Yeah but that should be fine.

**gcolvin** [10:44](https://www.youtube.com/watch?v=dapg2BAmCI8&t=644s):  The comment on the commit pretty much summarises.  I think of course if you have particular things to go through that's fine too.But for General discussion the comment is I think still a good summary.

**Juan Caballero** [11:03](https://www.youtube.com/watch?v=dapg2BAmCI8&t=663s):  Yeah I think maybe since it's your PR and there's you know change requests throughout and
1some topics you could you could guide us to what you'd want to discuss with a group to decide on change requests then update.

**gcolvin** [11:26](https://www.youtube.com/watch?v=dapg2BAmCI8&t=686s): See Victor wasn't able to make it today. The pain I've seen and experienced as an author. In my opinion we're in general way too picky. But especially we're way too picky way too early. It's a pain just getting a draft into the system but until you have a draft. It can be difficult to get discussion threads going to have a number to refer to. So people know what the proposal is so I think it should be easier to get a draft in the first place. We're not going to run out of numbers. Microsoft's not going to run out of hard drive space. So the main concept here is just to make it easier to get a draft in and tighten the standards as we move through the process and so I've made specific PRs but I'm not wedded to the specific PRs. I simply and presenting the concept of tightening as we go and doing it at the transition points. so people can get into the process and work on their proposal without a constant battle of your doing fine. You make a change and the ipw says Nope not anymore and suddenly a short session of work becomes a long session of work or you discover that. Oh! you can no longer use that link. Your whole proposal is stuck, just these are pain points. It's just a painful process for people on link policy. I really think we're too tight on it but certainly at the draft phase if someone needs to use a link or wants to in the draft. Okay we've set it up that we will need to go through a process of approving that but please let it into the draft so that the draft makes sense while we go through that process and I've suggested actually tightening up legs as much as possible having a full citation into the literature. So that if a link goes 404, you're not just scratching your head, you have an author, you have a title and hopefully you have the journal a publication date. So you can probably find another copy online. If necessary you can go to a library and get a copy on an interlibrary loan. you can send an email to the author lots of ways to get a copy if a link goes 404. so having a link is nice but it's actually less important than a proper citation.

**Juan Caballero** [14:42](https://www.youtube.com/watch?v=dapg2BAmCI8&t=882s):  Or the DLI idea because DLI or even ipfsc ids sort of create a location independent fall back. I like that a lot. I think there's going to be much pushback on any of those details. I think the
block like the things to resolve to merge, this quickly would be the technical assistant idea. There's seems to be a little contentious and I don't know the history there. If I definitely know the analogy to ITF and I guess if you it probably isn't the right place to talk about money or formal recognition but if it is a concept that already exists. If there is already a way to call
someone an expert enough to advise is where's the disagreement I think.

**gcolvin** [16:00](https://www.youtube.com/watch?v=dapg2BAmCI8&t=960s): The problem is we have got too many low quality drafts. I don't think we can bot our way out of that problem and we haven't gotten like the ITF a solid working group system and I suspect it's just too hard for us to do that because what comes in is erc's just covers a huge range of stuff and keeping a group organised hasn't happened and then I ask what do other Publishers do and the answer is peer review.  Something comes in for publication and you know two or three experts review it before it goes in and we've had some talk on this that if you can't find two people to help you with this draft. Then is it really worth standardising if nobody cares to read it but you what's the point if we can establish this as a practice and often Publishers push back on the author to say hey find some reviewers. we're not experts here, we're just editors. Find us some reviewers to work with you on this um so that we have some reason to think. It's technically sound, that's a barrier that I'm happy to put up before a draft goes into a technical barrier.

**Juan Caballero** [17:45](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1065s): What's actually going wild right now with ideas about that.

**gcolvin** [17:50](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1070s): Oh I
don't have my chat up.

**Juan Caballero** [17:55](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1075s):  oh sorry, so I think people are thinking about being permissive of PRS but postponing the numbering perhaps and that I don't know if that balances the pain of proposers against the pain of editors well enough but I do think you know like just to give a comparative perspective Casa which is you know pretty different pretty different animal but like diff two sort of has an informal two competitors rule. I've been trying to make it more formal at dif that a new work item proposal, that just comes from people that are already collaborating on a product or you know a thing. they're building where they're already collaborating. That isn't really a place for a standard. I think that to publish it as a document you could require BYO technical assistant or you could require orbs something that looks like the thinnest possible precursor to a working group.  those might be ways I mean particularly if combined with this idea of a pre-numbering or you know except the PR but don't give it a number till it has someone to review it.

**gcolvin** [19:29](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1169s): that's uh that's what draft PRS are for

**Juan Caballero** [19:32](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1172s): Maybe other people should speak I'm not sure I understand that the unnumbered proposal well enough Sam

**Sam** [19:40](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1180s):  oh it's just if we give draughty IPS a number and URL that changes when they get promoted to a review whether that's you know a different number or using the title or whatever I think that would give enough difference between a draft and a real EIP that I'd be okay with like a lower standard for those EIPs

**gcolvin** [20:06](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1206s):  I'm suggesting an initial stage which is just a draft PR. They can hang out there forever and never be merged and they don't need a number and that's the stage which you want some peer review before it's numbered and becomes a draft and then it has .

**Sam** [20:27](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1227s): You want the peer review before because right now we have drafts. You don't even have to have a finished EIP. right? you can leave to do's and all sorts of stuff and that's where we want peer review not after it's you know complete

**gcolvin** [20:45](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1245s):  I think so we're just getting flooded with drafts that are too low quality to bother looking at or just they're too far out of anyone's technical expertise to help with, so it's simply not uncommon for technical journals to do a phase of peer review before it gets very far at all. They don't put in the work of actually editing until some peer reviewers have said this is technically sound.

**LightClient** [21:19](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1279s): I mean we've tried for a pretty long time to have people engage with the eips as they move along the process and they just don't .

**gcolvin** [21:29](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1289s): I understand it  has to be sort of a rule. it's just like no

**LightClient** [21:34](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1294s):  I mean it is a rule. it's in eip1 it says before you create your draft you should ask the community and make sure this makes sense.

**gcolvin** [21:42](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1302s):  I don't I'm saying a rule, the editors will not merge a draft until some peer reviewers have actually looked at it.It will need to establish a little bit of process there. so it's clear this is a process. This isn't going out and finding some things. We want actual work on the draft PR until the reviewers are happy with it.

**Danno Ferrin** [22:11](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1331s): 
so I think this is a good spot to jump into my meta complaint. This doesn't address the issue that the core eips and the erc's are two increasingly Divergent communities with two increasingly resurgent processes. Getting a person with the technical knowledge to review a core EIP proposal is going to be easy. It's all over the place and getting someone to review a random ERC for a random token protocol that may or may not be viable is going to be  increasingly difficult and the standards that need to be put to a core EIP versus. Some ERC standards that just need to some extent have well-formed solidity are increasingly in diversion and have very different needs. This addresses the lowest common denominator needs but that's the problem. We're trying to put two Divergent processes together that really need to diverge.

**gcolvin** [23:52](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1432s): well, it doesn't seem complicated with GitHub you put in a draft PR. It doesn't merge until the editors approve it. So it's easy for the editors to say we're not going to merge it until I guess at least one technical expert helps us review it and that can be a standard process or at our discussion. Often an editor has the skill to look at it and and do that job often that it or doesn't have the skill.

**Danno Ferrin** [24:30](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1470s): We don't need this type of a process to move stuff in the core. Core will ignore the EIP process and set up their own standards rather than go through these. The needs are Divergent, very divergent. This is not something that core protocol changes go through except as a final box checking step. Just to satisfy some people we're increasingly abandoning the EIP process because it's not serving the needs of the core protocol. I understand why we need to split it. If you understand it, why don't you support splitting it.

**Pooja Ranjan** [25:05](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1505s): Again I'm sorry for jumping in. Oh yeah please go ahead because I do want to hear. sorry I just want to hear.

**gcolvin** [25:13](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1513s): I thought he was against this discussion so many times for so many years and I'm not alone in my opinion.  It's more like the people who agree with me have just gone away. But I'm not, I unalterably proposed. What's laid out doesn't look so bad. I have strong fears that the Divergence will actually hurt us .so we're better off preventing the Divergence.

**LightClient** [25:49](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1549s):  How is it going to hurt us?

**gcolvin** [25:50](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1550s): It'll simply spread resources out and cause ethereum more and more to become a fragmented Community.

**Lightclient** [26:02](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1562s): What resources will be spread out because we already review all of the eips and erc's and that's not really going to change when we split them.

**gcolvin** [26:11](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1571s):  Well see now we're getting into the details that I don't want to get into.

**Lightclient** [26:17](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1577s): But you're not really giving actual reasons against.

**gcolvin** [26:21](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1581s): I know I'm not giving vague.

**Lightclient** [26:23](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1583s): you're giving vague generalisations. 

**gcolvin** [26:26](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1586s): Yes
because I don't want to get into the details. We've done that. I'm trying to discuss a proposal, not that.

**Lightclient** [26:33](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1593s): But I'm saying that you  and your arguments against splitting, they don't have a lot of basis and reason. I've heard just generalisations about. It's going to fragment the process. It's going to make it harder you know ERC but there's not like specific things that you're stating like this is a bad thing. Whereas we've given specific things about the split that will benefit the All core Dev community and generally people from the All core Dev community and the ERC Community are not opposed to these questions. 

**gcolvin** [27:04](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1624s): Yes I'm waving my hand in the general direction of more detailed conversations in the past. But I mostly want to discuss my own EIP here. 

**Danno Ferrin** [27:16](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1636s): So you mentioned can I respond to one of the points you made Greg said that you were not the only person in favour of this but everyone that you had that disappoint with you has since
left this is the symptom of failure. 

**Sam** [27:31](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1651s): Sorry guys and I still am not in support of this change.

**Danno Ferrin** [27:36](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1656s): People are leaving because they can't get what they need out of it. That's the problem.

**gcolvin** [27:43](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1663s): I mean people have left the discussion just stalls every time we have this discussion. we decided not to split the repo. We do not come to consensus on splitting the repo; we've never had it consensus.

**Danno Ferrin** [27:56](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1676s): We're on the precipice of people abandoning. The EIP process; it's already happening in the core protocol. We have execution specs. We have execution spec tests nothing networking has gone through in a long time slowly but surely it's peeling off and this is bad. I mean if you're going to wind up it's just an ERC repo anyway. if we don't acknowledge this. 

**gcolvin** [28:19](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1699s): Understand. I want to fix it. I have an EIP which will not totally fix these things but I think we'll reduce the pain for everybody and I think it's a good idea. If we can reduce the pain for everybody.

**Danno Ferrin** [28:35](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1715s): it doesn't reduce the pain. enough people are still leaving we've been through this you know going through this for years and people are still abandoning it

**gcolvin** [28:44](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1724s): I'm suggesting we do the parts of this that we can come to consensus on and will reduce pain if nothing will reduce all of the pay

**Danno Ferrin** [28:54](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1734s): This is death by a thousand paper cuts. You're the one with a dream of paper.

**gcolvin** [29:05](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1745s): No if I walk away that's okay. I'm a very busy old man. That's not a hostile act on my part.It would just be you people need to do what you need to do and if I'm not comfortable with doing it that way, it's okay for me to say okay do what you need to do. It may well work out just fine.

**Lightclient** [29:37](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1777s):  I think it's time to do what we need to do. We've had the eipip process for three years now.

**gcolvin** [29:45](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1785s): You need to change the way you organise your repos. so your repos are more useful to us and I do look and say a fair amount of your process. Could you try again? Yes some of it looks like the core devs are trying to use the EIP process for things that have nothing to do with the editorial process the the status of something as a an edited document and the status of a proposal moving through to get into the protocol have different stages the core devs can pull something to CFI at any stage in the editorial process. They're not bound by that process.

**Lightclient** [30:39](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1839s): Splitting the repos is not really related to this yeah I'm trying to say this

**gcolvin** [30:48](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1848s): I'm sorry I'm not being really clear here there's too much on the table. We don't have core devs here to discuss this in part.

**lightclient** [31:00](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1860s): What do you mean Danno here Danno  is requesting that on behalf of the other core devs that we've talked to on all core devs who were in support of this and we have Arias two weeks ago who said they wanted this.

**gcolvin** [31:16](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1876s):  I had our Time complaining that well we've got stuff spread across hackMDs and this and that I'm scratching my head.

**lightclient** [31:23](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1883s):  Tim
wants to split the repos.

**Glcovin** [31:26](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1886s): I understand but I'm just going, why is it the editor's problem that you can't keep track of the status of your work.

**DaoFerrin** [31:35](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1895s):  Because we want to change the process and it takes a year to get a process change through and that's just it doesn't align with what we need with our workflow where we're putting in hack MDS. We're putting in separate repos. Why are we basically abandoning the process because it's not suiting our needs ?

**gcolvin** [31:54](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1914s):  Why are the core devs trying to use the IP process to track their development process.

**Danno Ferrin** [32:01](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1921s):   It is the ethereum Improvement protocol; it's where we can get consensus on the changes that we're working on for ethereum not for the application layer. I mean the w3c is capturing the ietf is what's going on.

**gcolvin** [32:16](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1936s):  No this feels more like the  IETF editorial organisation has decided that there's way too many different kinds of proposals for the internet and so they're going to break up the ietf into multiple organisations.

**Danno Ferrin** [32:32](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1952s): Like the w3c Like what would like there's all sorts of things that are like the PIP I mean they split to reflect the needs of the communities when they diverge.

**gcolvin** [32:45](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1965s): Those from new organisations that rose up for new needs.

**Danno Ferrin** [32:52](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1972s): But this one at the end of the ietf, the other tables.

**gcolvin** [32:55](https://www.youtube.com/watch?v=dapg2BAmCI8&t=1975s): The ietf editors did not divide themselves into multiple organisations just because the ITF  covers a huge range of Technology. So I'm going to loosen our workflow. So it's not in their way and find out how you can clean up your workflow. I get that protocol level. They've been working directly with their python specification and that's where some process probably needs to change that.  the EIP really isn't done until after they've done their work on the reference implementation and I don't have a problem with that. we just need to work out. 

**Danno Ferrin** [34:02](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2042s): Work out how that works and part of that I think just making it easier to get a draft into the system and move it through, So there's always a document in the system that can be referred to and
The author has control of the problem because we have two Divergent layers trying to use the same system that is not serving either one of their needs very well at all.

**Juan Caballero** [34:30](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2070): And your concern is going to split it. I think it's going to strengthen it. People are going to see that they can get what they need out of what out of each different group and they're going to use it more.

**gcolvin** [34:41](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2081s):  you think?

**Juan Caballero** [34:42](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2082s): 
yes I do.

**gcolvin** [34:43](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2083s): Yeah and I don't and we're going we're going on hope here not a plan.

**Danno Ferrin** [34:50](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2090s): We have a plan. You made us a tablet so we could discuss your plan. It doesn't address the issues.

**gcolvin** [34:56](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2096s): It addresses a few other issues that I think are easier to fix and would help a lot.

**Danno Ferrin** [35:03](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2103s): But we're focusing on a low-hanging fruit when we need to go to more substantive issues. We're distracting ourselves by avoiding the core issue that we're diverging these communities. A lot of these ercs do not necessarily ever need a raw and Mainnet they could run on all sorts of the pick your random alt L1 or L2. The application layer has nothing to do with changes to the consensus layer with changes to the networking between the two clients between the two different layers. They're fundamentally different layers that only interact in very few places.

**gcolvin** [35:41](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2141s): Okay, we're just editors in the end. We just want to publish a high quality document and I get that. We don't want the process to be in the way of that but I do think that people are trying to use the IP process for things besides simply having a final document at the end to manage their own workflow and I know that GitHub tends to pull things that way and cause problems that way. But still I'm going. It's not our problem if you prefer to use hack MDS rather than use Ethereum PM.

**Lightclient**  [36:33](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2193s): I'm just saying, it's not that we prefer to use hack MDS. People want to use the process it just doesn't work with. How they normally work.

**gcolvin** [36:45](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2205s): I'm looking back to how it was working. You know I only sort of disappeared for a year and all of a sudden it was a different world. So I've never recovered from that and I'm the last OF left. So
I'm the last one going. This was our intention. Iit was a pretty solid long-term intention so that's a lot of what's going on here and I have a lot invested in that.

**Danno Ferrin** [37:11](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2231s):  But the community has moved on from what was intended and maybe what is intended isn't what's working. I mean I think you're articulating the core issue here.

**gcolvin** [37:17](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2237s):  Yes and that's where with no hostility. I will need to move on if I've decided the philosophy no longer corresponds to the philosophy we had, which is that we were Publishers. All we're trying to do is to get a good final document at the end and with the core devs. We always considered them to be a separate organisation. Who could pull documents out of our process because their workflow is not ours. All we wanted was to do our best to get a final document ready to describe what actually went on to the mainnet.

**Lightclient** [38:02](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2282s): I mean that's still the goal, It's just the way that we're going about it. It is disenfranchising the people who are writing the documents and involved in the process of dealing with the documents so it's kind of ingenuous to say that's the goal to have the best final documents when we don't listen to the feedback from the actual creators of these documents.

**gcolvin** [38:25](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2305s): I'm hearing two sorts of problems. One sort is just the difficulty of dealing with the editorial process and that's this IP is trying to solve some of those problems and its low hanging fruit is low-hanging fruit.

**Lightclient** [38:45](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2325s): If you just but again at the very beginning of this debate. We came to a specific proposal that you made where you feel that. There should be more peer review that happens before something goes to the draft Daniel says specifically this would be easy to have with all core devs. At some stage in the process it's very hard to have with erc's because they're so fragmented and so this is just a clear place where we can't easily have some you know rule across both categories of VIPs and apply them in the same way.

**gcolvin** [39:17](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2357s):  The Proposal is at the editor's discretion. The editors can go and review enough. This is solid or we can't tell if this is solid we need help and it is purposely a technical barrier the core core proposals can meet much more easily that's true.

**Danno Ferrin** [39:37](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2377s): 
so we're already saying that core has a different process than erc's why are we keeping them in the same file cabinet.

**gcolvin** [39:44](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2384s): No, I'm simply in this case. I'm simply saying the court proposals are more likely to be reviewed and solid right away and erc's are more likely to be not solid or not useful.

**Sam** [40:02](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2402s): So right if you had the same  same rule for both core eips would get approved easier and erc's wouldn't be and that's okay.

**Danno Ferrin** [40:12](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2412s):  It's not okay that it's not serving. The needs of the two Divergent communities.

**gcolvin** [40:17](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2417s): The added at the editor's discretion and the authors can argue with the editors. you know we can either say we will look. You know we will move this to draft.

**Danno Ferrin** [40:31](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2431s): What we're seeing is the authors are abandoning the process rather than engaging in that fight.

**Gcolvin** [40:35](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2435s): That's not a fight for the core things. We don't say technically, we're not going to put this in. We say we're not going to put this in because it doesn't meet our rules. It won't get through our bot. So we're not going to put it in until it does. That's an easy pain point to get rid of it's clearing out low-hanging fruit that's not very controversial is worth doing. It eliminates some pain right away.

**Danno Ferrin** [41:08](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2468s): And we're going to see pretty quickly that the core issue is that these are two communities that have different needs from their editors.

**gcolvin** [41:14](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2474s): I would be 
happy to see the court issue get quite clear in that way

**Danno Ferrin** [41:20](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2480s):  it is clear you're just refusing to see it.

**gcolvin** [41:22](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2482s): No, I'm disagreeing that it all needs to be fixed in the editorial process. What I think needs to be split is that the core devs need to own their workflow and we need to simplify our process so that it doesn't interfere with workflows.

**Danno Ferrin** [41:45](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2505s): How is giving the core devs special privileges any different from splitting the repos. 

**gcolvin** [41:52](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2512s): I'm explicitly not giving anybody special privileges and already it's the case that the editors have to approve a draft before it goes into the repo. I'm simply saying it's the editor's discretion. They can ask for outside technical review and tell the author that we are not confident to review this or to the extent. We don't think this is up to Snuff and you need help. so we'll work with you to try and find that help and this is not a core Dev versus ERC. We will get Court proposals that have the same. You know you look at it and you just go, this doesn't make sense. If it does, somebody needs to help this guy. 

**Danno Ferrin** [42:45](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2565s): So we're going to increasingly have editors apply different standards to different kinds of eips and that is just reinforcing that there's two communities going on here at the same time.

**gcolvin** [42:57](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2577s):  I just said We will get core proposals that also need outside review fewer than erc's. If a court proposal does need such review it will be much easier to get that review. I don't think that'll be a problem at all.

**pooja Ranjan** [43:18](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2598s): I would like to cite an example. Here is one of the latest CL side proposals that has been added to the EIP repository as core and the proposal number is 7044 and there is another proposal in progress which is an eip6110 for both proposals. What I noticed for them is that their discussion thread is completely empty. There was no discussion that was public. Because discussion definitely happened with the client. Dev meeting and perhaps in the client. A specific spec repos so it is not easily accessible following the process of whatever has been established so far is also helpful for core EIP is what I'm considering. It's just that we need to let people know about the process, one other common thing about these two specific proposals coming up from the CL side. I'm sorry 6110, I guess it is on El but 7044 is on sale and they are not aware of the Proposal. I think the spec has already been implemented because that is a part of upgrade but the proposal still is in draft status. It is not even in the review status which would be an ideal status for that proposal so what I felt was the proposer and the author had no issue moving the proposal from draft to review. It's just that they are not aware if we let them know that this is the process and you want to follow. I'm still hoping that it will work out for those people but going back to Greg's initial PR I think Greg it would be a good idea to talk about 7230 the pain relief point that you are suggesting and get an agreement on what we agree and if this can be merged because I'm assuming that if this can be merged perhaps we can move on. So I see from the chat Lifeline is not in favour of the draft and numbering idea. Please correct me Matt if I am mistaken over there but if this change is added. Would you be open to discuss and perhaps pull in or yeah Remove this part from the PR. so we can go ahead and merge the PR where we are on that would be a good idea to discuss.

**gcolvin** [45:44](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2744s): I'm happy to split this PR up because clearly some things are more controversial than others.

**Pooja Ranjan** [45:52](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2752s): It's always a good idea to have a smaller PR so we can get clarity on the situation. We can keep moving on if this particular section draft numbers thing can be moved out what is the next point that we don't agree on. As an editor's group they are not comfortable moving this to eip1 if they are then that's a small step but a step forward in improving the process. Any other point from Greg's PR that people would like to be removed or be a part of a different PR. so we can go ahead and have this one merged.

**gcolvin** [46:43](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2803s): 
we can take it up in the thread on PR.

**Pooja Ranjan** [46:52](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2812s): 
the idea we can definitely take it up in the thread and Greg  not saying that. It is going to happen just today but again considering both the possibility of splitting as well being one of the possibilities for repo. It would be a good idea to follow the you know proposed and next steps to understand if at all we go ahead with the splitting we are in a good position. We are in a comfortable position and nothing is breaking up. So if it is fine we can perhaps  in the next 10 minutes. Quickly go through the hack MD that is being proposed here. it will give an assurance to the community. I suppose that if the split is happening we are not abandoned. We are in good hands. All right I think of just to make good use of the time. Let's quickly go
over the points we will continue discussing Greg's PR in the thread and see if it can be split and PR number 7230 can be merged at least it will give some relief to the present process and editors and then we will we will separately discuss the PR which is split or coming up as new and for this time for people who are in favour of having this a split but they are wondering if the split will be useful or helpful. Let's go ahead with the hack MD with the proposed process. I think collecting thoughts from Matt and other people who are in support of this split would be a good idea and it will be helpful for people like Juan and us too. You know, coordinate and have things in place before the split. Juan if you would like to maybe pull up the document and we can discuss specific points there. Looks like he has been disconnected but okay fine. I have also added here in the agenda I'm gonna re-share it. Okay someone did pull up. Thank you. Any specific point that people think is worth discussing in this group. We can perhaps talk about it any objectionable point would be priority because that's what we would like to resolve first.

**Lighclient** [49:32](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2972s): 
omega's first thing is what is the latest on this numbering bot is that ever going to happen.

**Pooja Ranjan** [49:41](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2981s): 
I'm not sure if the panda is not on the call. I suppose he is working on the numbering part but unless the part.

**Lightclient** [49:47](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2987s): I think he is probably working on the number I thought.

**Pooja Ranjan** [49:50](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2990s): I did stop okay

**gcolvin** [49:54](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2994s): I mean that's even or not one series uses. The other Theory as soon as you can forgive them you know.

**Lightclient** [50:04](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3004s):  The problem is that, it's only works post split and so it's not really a good thing to enshrine because then nuke People's Community will think that odd numbered eips or or erc's 
do you know one or the other category and then you go back and you look at 1559 and you're like that should be an ERC because it's odd and it's not. So I'm pretty against even and odd.

**gcolvin** [50:27](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3027s): It's a technicality.

**Lightclient** [50:31](https://www.youtube.com/watch?v=dapg2BAmCI8&t=2083s): Yeah to do the technicalities. 

**Pooja Ranjan** [50:32](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3032s): Do we have any alternate proposal for this EIP number ?

**Lightclient** [50:37](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3037s): I mean I have proposed on many occasions even outside of the conversation of the splits that we should just have a shared document. some sort of hackMD, some sort of GitHub or Google sheet. Whatever spreadsheet that we can all use and just update the latest number that's used in the PR. It's assigned to and just manually assigned them like we have so many problems with numbering. We should just do that instead of using the pr numbers. That's something we can do right now.

**Pooja Ranjan** [51:06](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3066s): So this question will be equally valid for core eips as well what we are planning to do. They are planning to continue with the pr number and I remember Danny's proposal.

**Lightclient** [51:20](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3080s): Well I'm still proposing that. It's roughly sequential. The only thing is that we just have a spreadsheet that we look at to see what the last assigned number is whether it's EIP ERC. It doesn't even matter about the split, we can do this now.

**Pooja Ranjan** [51:40](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3100s): Okay, I think that is a good point and perhaps we'd like to get an agreement of all eip editors because they are responsible for allocating the EIP number and we have been joined by a new editor.I don't know we can call them editor but definitely helping with the EIP number allocation and it would be a work in which all the EIP editor and that user would work together to allocate. So I am open to keeping this as a discussion point for the next meeting. How do we want to go ahead with the EIP numbering?

**lightclient** [52:13](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3133s): Maybe we can, I mean can we just do it like anybody against doing this.

**gcolvin** [52:21](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3141s): It's easy enough and if we find a way to automate it. It's easy enough to switch to automation.

**lightclient** [52:28](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3148s): Well I mean theoretically Panda should have automation done at some point but that was you know one and a half, two months ago and we don't have it yet. 

**gcolvin** [52:41](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3161s): Think they need to be sequential and they need to never be the same.

**Lightclient** [52:48](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3168s): Yeah I agree.

**gcolvin** [50:50](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3170s):  The numbers diverge too much that gets confusing as far as time.

**Pooja Ranjan** [53:02](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3182s): So it looks like we are generally in agreement with the allocation of EIP number using one common file that will be shared among the EIP editors as well as a user who are supporting us with the EIP number allocation.

**lightclient** [53:17](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3197s): Sounds good I'll make a Google sheet and share it with people.

**Sam** [53:21](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3201s): And the idea is that when we merge the draft PR. we rename the file.

**lightclient** [53:27](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3207s): I think we can just assign the EIP number and have the author do it.

**sam** [53:31](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3211s): Okay, works for me. So this is just to get in the routine of doing it. 

**Pooja Ranjan** [53:38](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3218s): Do we want to have it  for a particular number in mind because it would be easier to 
communicate it to the community that from this number onwards whatever number allocation you see is based on this process. We added seven thousand something right so let's check on the latest number and whatever is closest to 100 of that perhaps that would be a good idea to start from there even if it is not an ideated number. We can start that as the first number. 

**Lightclient** [54:10](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3250s): Sounds good. Okay let's go ahead and do that . I said other main questions just like what is going to be the situation with the Bots has any progress been made at all on having the configurability to have them manage multiple repositories.

**sam** [54:36](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3276s): So, as long as you keep the same config for EIP. I think that would be the idea and yeah I've added configurability to the command line tool. I just haven't added it to the GitHub action yet. so that'll probably happen shortly. Okay I have no idea about the review bot. I think Panda said that it would work fine as long as it has secrets.

**lightclient** [55:02](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3302s): yeah I mean yeah okay that makes sense.

**Pooja Ranjan** [55:04](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3304s): Which I assume by forking it will be there.

**sam** [55:08](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3308s): We won't be able to Fork because then we won't have issues or pull requests and code search won't work. So, we have to create a new repo and push the commits to it.

**Pooja Ranjan** [55:21](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3321s): okay in that case we need a plan to have the secret  shared over there as well.
**Lightclient** [55:29](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3329s): I mean we would just have new secrets for that.

**Bumblefudge** [55:34](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3334s): And you can  transfer issues. Maybe I misheard but were you saying that it's not that.

**Sam** [55:39](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3339s):  Saying for the fork. Yeah if you Fork a repository on GitHub, the fork has limitations like it can't have a Wiki. A code search doesn't work. There's a few minor things. We'd want a clean copy. 

**Lightclient** [56:00](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3360s): Yeah I think that's the biggest outstanding things but we can see if there's anything on the PR 

**Pooja Ranjan** [56:12](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3372s): Okay so definitely will communicate this to Panda and whenever we are ready, we are just trying to make sure that our checklists are covered. so whenever we are ready we can do that. If at all needed. I think it's a good discussion for today considering we still have some pros and cons going on and I'm hoping that if some of  the concerns of Gregs are already answered and the PR is merged. Perhaps we can have him on board as well and we will get to understand better. We have just two minutes left on the call and uh yeah anything specific

# 3. EIPs Insight - Monthly EIPs status reporting.

**Pooja Ranjan** [56:58](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3418s): Very well I have also shared the hackMD file which is for eips insight and I've tried to add this image for you know how many proposals we get every month and how many gets merged as final. Definitely we agree that most of the proposals which are not merged as final are from ERC side because the number of ERC proposals are higher but at the same time this is also true that proposals which are being merged on month-to-month bases are mostly from ERC side as well. So ERC people are also trying to follow whatever they have been advise to and get their proposal merged with ERC. Well that's a discussion for the next meeting going through the EIP. Inside we have received four final eips for the month of July. As on July 12th and all four belong to ERC category there is one proposal in last call and I suppose its deadline has passed so we will have to reach out to the author to ask him to make a proposal to make it to the final status with three new drafts.

# 4. [EIP Editing Office Hour](https://hackmd.io/@poojaranjan/EIPEditingOfficeHour)

**Pooja Ranjan** [58:01](https://www.youtube.com/watch?v=dapg2BAmCI8&t=3418s): The EIP repository seems to have a lot of open pull requests which would need some addressing. But the EIP editing office hour has been doing great. Thank you Sam for taking out time and responding to particular questions of new Authors who are trying to follow the process. We have added the EIP editing office to our meeting recording from yesterday. You
can find that the agenda and agenda for the next meeting is also linked there. so if people have any questions with respect to any specific pull request. Please be sure to add it over there. We do not take a general review in EIPIP meeting only final proposals can have a
discussion in EIPIP meeting. Well that's all for today. Anyone have any final comments? If not then I think we are good for today and hope to see you all in two weeks. Thank you everyone. We did great and we made some progress. Thank you everyone.

—-----------------------------------------------------------------------------------------------------------

# Attendees

* Justin Florentine
* Gcolvin
* Pooja Ranjan
* Sam Wilson
* Light Client
* Jason Windawi
* Zainan Victor Zhou
* Bumblefudge
* Gordo Wright
* Gajinder
* Danno Ferrin
* Juan Caballero

# Date for Next Meeting: 26 July 2023 at 1400 UTC.




