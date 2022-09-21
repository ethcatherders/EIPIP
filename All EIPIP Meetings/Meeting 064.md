# EIPIP Meeting 64 Notes
### Meeting Date/Time: Wednesday, September 07, 2022, at 14:00 UTC
### Meeting Duration: 28:53 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/174)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=JKsUrL0VOxU&list=PL4cwHXAawZxpLrRIkDlBjDUUrGgF91pQw&index=1)
### Moderator: Pooja Ranjan
### Notes: Metago

## DECISION ITEMS

**DECISION 64.1**: To understand the meaning of 'requires' authors can refer to EIP-1. You can find discussion of the meaning in the notes below. 

**DECISION 64.2**: EIP editorial decisionmaking process can be improved by providing enough time for feedback from editors, as well as trying to get a rough consensus from editors, before making changes. Also, documenting the decisionmaking process and discussing it in the meetings will help clarify how decisions were made and help future editors to understand the context of the various processes.

**DECISION 64.3**: Sam will look into EIPIP GitHub issues 34, 63 and 95. 

**DECISION 64.4**: Pooja is working with aspiring developers to create a dashboard for EIP’s chart that at present would not be a part of EIP's GitHub repository, once it's successful Pooja will like to come back and propose it, if people find it interesting it can probably be added with less maintenance. If anyone has suggestions on any other charts or dashboards that you would like to see on top of whatever is already existing in EIPs Insight or hackmd please share it with Pooja, she will try to have that incorporated. 

**DECISION 64.5**: EIP-1 is the reference document for the external links policy for EIPs. If anyone in the community is interested in helping with EIP bot and external links policy related issues, please reach out on ECH discord. 

**DECISION 64.6**: EIP editors will review prs 5572, 5586 and 5596. 

**DECISION 64.7**: if you are an author with an active proposal in the EIPs GitHub repository and if you have questions you want to reach out to EIP editor, please feel free to attend EIP Editing Office. You can find details on ECH Discord. 

**DECISION 64.8**: EIP number bot and EIP asset licensing issues will be discussed in the next meeting. If anyone is interested in contributing please reach out on ECH discord. 




----


# AGENDA

## 1. Discussion: 
### 1. Guidelines for 'requires' [0:00](https://youtu.be/JKsUrL0VOxU)
**Pooja**
Welcome to EIPIP meeting 64. I have shared agenda in chat. I have tried to list items as per our general discussion that is there in discord channel and also in the EIP’s GitHub repository. 

So the first item for discussion today is discuss guidelines for ‘requires’ and changes in EIP process and EIP-1.  So let me quickly give a little background about why ‘requires’. So ‘requires’ came across in one of the issues that we were reviewing yesterday in EIP editors office hour, and there was this question that sometimes authors get confused like what to put in EIPs’ requires section, like which particular EIP should be added as required and when it is that it is mandatory to be added as ‘requires’. So yeah I’ll be curious to hear thoughts from EIP editors. I know Sam has already shared some, but Sam, if you would like to summarize a little bit more here and then we can probably take some input from Matt?

**Sam**
Sure. So the ‘requires’ header, there are two kind of opposing viewpoints on it. The viewpoint that I have is that the ‘requires’ header is where you list EIPs that you have to read before you can understand or implement the current EIP and the other camp is that the ‘requires’ header should list all EIPs that you mention in your EIP, whether or not they are just context or are required reading.

**Pooja**
Awesome. So it looks like there are two major points, so if any proposal is needed just to understand, to work on the new proposal as an EIP that can be, and another one if there is any mention of it, like any kind of dependency on the other proposal. Matt, I wonder if you have different thoughts, or if you would like to add any other point that an author should consider while adding proposals to EIP’s require section?

**Lightclient**
What does EIP-1 say? 

**Pooja**
That's a very good point.

**Lightclient**
Sorry, I'm frothing some milk at this exact moment…

**Sam**
It says EIPs may have a ‘requires’ header indicating the EIP numbers that this EIP depends on.

**Lightclient**
I mean we can be like pedantic on the wording,, or we can just, you know, elaborate more but I feel like depends is what Sam is saying like you have to understand this EIP to implement the EIP that is required or like I mean I don't know I'm not even sure understanding is the bar I think like it has to utilize something from that EIP, whether it's like a concept or a specific technical aspect of it. I don't think that we should be listing the EIPs that I just mentioned. 

**Pooja**
This is any way an optional field like an author can add or not add, but yeah, if we go by the present description in EIP-1, it looks more like EIPs on which it is dependent.

**Lightclient**
Well, the optional part of that is we don't have very good granularity like it's an optional field but it should be required if the EIP actually does depend on another EIP.

**Pooja**
Oh that makes sense. Sorry about the confusion. Thank you for clarifying. So I hope that will be documented in notes for this meeting, so going forward if there is this kind of confusion, we can probably refer to it and just for general people listening to this call, whatever is documented in EIP-1 is correct, and that's what it literally means, so please try to follow that.

### 2. Change in EIP process & EIP-1[4:18](https://youtu.be/JKsUrL0VOxU?t=258)

**Pooja**
All right, the next one here is changes in EIP process and EIP-1. So in the last meeting, we were discussing about some changes and the pull request number was 5463, however it seemed like it was not given enough time for discussion, so the pull request is reopened with a new number that is 5533 and yeah if we can probably discuss on general guidelines…however I tried to document some of the decisions from the past EIP editors meeting in the apprentice handbook but we can have a general guideline for people to refer to. Sam I know you have reopened the pull request. If you would like to maybe provide a brief intro of that and we can probably discuss it. 

**Sam**
Oh yeah, so the previous pull request added an adoptable field and so the adoptable field is kind of like a signal to editors that says if the author isn't responsive, we are allowed or encouraged to assign it to a new author at our discretion. It's not my proposal. I kind of on the fence about it like I am with a lot of these things, I think it's a little bit extra to add this field so you can just make a new EIP and you know make yourself the author on it, where on the other hand it's nice to be able to like ensure some continuity between EIP numbers, and yeah so you know I'm a little torn on it and it was my bad for merging the first pr without getting rough consensus among editors so I reverted it and opened this new one to discuss. Since Pandapip isn't here, I'm not sure if we'll actually be able to debate very well. 

**Pooja**
That is right. I totally understand that. I think in general like it's my understanding that in general we can or we should keep any discussion open for at least two EIPIP meetings so we get to share the information with the EIP editors because sometimes some of the editors may miss their discussion. So yeah, Matt, if you have anything to add on this particular proposal, the adoptable one or in general you want to talk anything about the process?

**Lightclient**
I just think that we need to leave things open for a fairly long time if editors disagree, definitely for a couple EIP meetings, we should discuss it synchronously if there's disagreement before merging and I mean just generally waiting for, you know, mostly consensus among the editors, or at least the editors who are active, and I don't think that we should have the adoptable field so, it's my take. 

**Pooja**
Yeah one other thing that I would like to make a mention of generally in case of any changes to EIP-1 earlier we were having like two editors’ approval, but now we have like around five editors available, so it will be nice to have minimum three editors on board and get that approval done. I'm not sure if this is already added in the bot and it is taken care of, but if not, I think that would be a good idea.

**Lightclient**
There's also like a general courtesy I think that we haven't merged too many things in the past where editors disagreed even if we had two editors, unless the editor who disagreed said I’m not going to block this, like there is, does seem to be a bit of veto power amongst single editors if they think a change is bad, I don't want to like encode that but I think that it's like a reasonable courtesy to not just merge things after two, even if somebody has already said they're pretty against it.

**Sam**
Yeah, that was entirely my bad, like it's entirely my fault, like Pandapip has been adding EIPs to a manual merge-like list because some of them require it and I didn't realize that we didn't have consensus on this one so that's entirely my bad. 

**Lightclient**
I mean it's all good. It happens. There's a lot of EIPs to go through. 

**Sam**
Yeah, I guess I'm just saying, I don't think…you know the process is wrong I think I just implemented it incorrectly.

**Lightclient**
Yeah, there's no [inaudible]...I think Pandapip has also merged a few things recently that didn't really have everybody's agreement or like didn't go through the correct process and so it's useful just to say again.

**Pooja**
Yeah in general I have noticed a huge spike in number of comments going on in the repository and if they look into the EIP’s Insight report that I generally share, it's like up I don't know maybe over… it's very very high which is not a bad thing because we are trying to improve process but I feel like for certain decisions which is like not that easy and we definitely should have consensus of EIP editors, we can probably wait for some time and give it enough time for EIP editors to provide feedback. Unfortunately Pandapip is not here. We would love to hear what he thinks about it and probably be considerate in future in merging all these proposals.

**Lightclient**
Yeah I mean it's awesome the stuff that Pandapip has been adding I think we haven't had someone who like understands the process and is able to do as much work in the CI this is able to do so it's great, but I’m getting worried that everything is changing, and we can end up in a situation where, you know, if Pandapip stops editing, then we don't understand how this, some of the things work, whereas like, in the past, people like the editors have sort of known or like the thing is so old that we've been working with it for years.

**Sam**
You know, as a newer editor I never had any idea how the build system works, so this is a no change for me okay but I think most of the changes have been pretty reasonable, like I've tried to be reviewing most of them, just to keep on top of them and like it's mostly been non-critical things like the labels and like some of the merge rules and those kind of things and I think those changes are like they're not part of the core approval process like it doesn't matter if it has the right tag, so I think we can afford to be a little fast and loose with them but I would like to start stabilizing the build system again, and, you know, cut down on the number of changes.

**Lightclient**
Yeah I agree.

**Pooja**
Yeah, totally there. I know a lot of things is being bot driven now. We are talking about bots and we have recently made some changes in bots as well, so we can definitely expect a lot of comments going on into the repository which is again not a bad thing, it's a good thing to happen, but at the same time discussing it in these meetings or may be able to document it somewhere else will help other people to follow along and maybe community to like follow after whenever they would like to refer it to so yeah that's all good. Thank you Sam, thank you Pandapip and yeah thank you Matt for sharing your thoughts over here. 

## 2. EIP bots related discussion, updates, agreement on merging PRs & closing Issues: CI: Upgrade EIP-Bot to eip-review-bot ethereum/EIPs#5508, eip-bot Issues and Pull Request[12:31](https://youtu.be/JKsUrL0VOxU?t=751)

**Pooja**
All right. I think it's safe to move on to the next item. So the next item is EIP bots related discussion, updates agreement on merging prs and closing. Generally I keep this item on number three after the GitHub issues and pull requests but we are not getting enough time to discuss this item so on request of Jose, this has been bumped up. We will get into the EIP bot issues but before that there is a one pr which is 5508 that is to upgrade EIP bot to EIP review. I just wanted to share it with editors, if they have any comment concern with that. It looks like it is a change for the EIP bot. So yeah any thoughts any comments?... and if not then probably you can check it, review the quotes and yeah if needed much as I wanted to just share so this should not be blocked for very long time.

**Jose**
Yeah, just for curiosity I cannot find the 5508 in the EIP pull request, maybe I don't know maybe you just can share the link whatever whenever you want or can. That would be great, thank you. 

**Pooja**
Yep, I just shared.

**Jose**
Cool.

**Pooja**
This is just for attention, but in other than that Jose did you wanted to share any update or anything in specific you wanted to discuss on this topic?

**Jose**
Well just to let the basically Sam know that if you have the time I agree with Pandapip to take care of the issues 95, 63 and 34 from the EIP bot so if I just don't want to that was something that I was briefly talking to him I just don't want to get into something that someone else is working on suddenly you know so if you have the time Sam, I really appreciate that you take a look in the issues.

**Sam**
Oh yeah, which one's sorry you're in the EIP repository you said 93?

**Jose**
No, 95, 63 and 34. 

**Sam**
Okay 95. Sorry, I’ll just open these up now and I’ll take a look at them.

**Jose**
That's okay, thank you. 

**Sam**
95, 63 and what was the last one? 

**Jose**
34

**Sam**
34. Okay, I will take a look at those today.

**Jose**
Thank you I appreciate it. That's it from my side. 

**Pooja**
Very well. Thank you so much. I think that also covers the second point which was related to issues and pull requests. 

## 3. From GitHub Issue or Pull Request[15:55](https://youtu.be/JKsUrL0VOxU?t=955) 
###  Issues; Make EIPs Website a PWA, Advocate for EIP editors to clearly explain the current external link policy to new authors.

**Pooja**
Moving on, this is from general GitHub issues and pull request, there were two issues added in the past two weeks, one is make EIP’s website a PWA, it's a proposal by Pandapip and he wants to volunteer, unfortunately there is no plan shared, but yeah wondering if anyone has any comment?...if not I think I have…

**Lightclient**
What was it?

**Pooja**
PWA, oh yeah issue number is 5608. Let me show you here. 

**Lightclient**
What does PWA stand for? 

**Sam**
Progressive Web Application

**Lightclient**
I think we shouldn't do that.

**Sam**
I don't think we need to like if you want to browse it offline just download the repo um yeah.

**Lightclient**
I mean in a perfect world it would be cool but at the same time again I don't want to add more things that can break that we have to fix. 

**Pooja**
That's a fair point. All right so yeah I mean I wanted to bring it up because we have mentioned that we will be talking about issues which are there, it's good to collect some thoughts, on a separate note, I have shared it in the past as well, and I want to mention it again that I have put together a small team of aspiring Ethereum developers like they are not developers as of now they are aspiring developers to create a dashboard for EIP’s chart but that is at present would not be a part of EIP's GitHub repository, however this is an experiment I’m trying to do it on a different GitHub, once it's successful I will like to come back and propose it, if people find it interesting we can probably add it with less maintenance of course. And yeah if anyone has any suggestions on any other charts or dashboards that you would like to see on top of whatever is already existing in EIPs Insight hackmd please share it with me, I will try to have that incorporated. The next issue here is advocate for EIP editors to clearly explain the current external policy to new authors. I know this is like repetitive we have discussed about it at multiple time and the proposal is also not on the call but anything that any of the EIP editors would like to mention again on external link policies. 

**Sam**
I mean it's in EIP-1. External links to external authors should not be included, external resources may disappear move or change unexpectedly I think that covers the current external links policy pretty well maybe we should be more polite when we're expressing it in prs but that is pretty clear.

**Lightclient**
Right well it actually says should which they should not be in an EIP.

**Sam**
Yeah that's what I said, should not.

**Lightclient**
Well, I don't think that's that clear though, like there's no definition of should like, that seems like it's up to the editor to decide but the system does not allow you to have links.

**Sam**
Yeah, without like overriding EPW?

**Lightclient**
Yeah, but if you already… then like it's not a one and done like every time they edit eve now, they have to get written.

**Sam**
Yeah sucks. I have an issue open on ew for somehow giving like EIP editors the ability to override specific errors I just I haven't really thought about how to do that yet so.

**Lightclient**
Sure.

**Pooja**
Do you have the number handy Sam? Maybe we can try to reach out to community if anyone is interested taking a look at it, maybe well…

**Sam**
It's not specified yet like here I’ll get the link here it's...

**Pooja**
Yeah I mean and that would be nice we can probably share it in our next Cat Herders’ calls as well if anyone is interested to make contribution they would be there. But yeah summarizing this current external link policy, the policy is same as that is listed on EIP-1 and there is no change, so please follow what is listed there.

**Sam**
We can definitely expand it though, like do we want to say something more like you know unless there's very specific circumstances or we can definitely be more clear about it.

**Pooja**
All right I think in that case maybe a pull request with the revised words would be better and there we can collect more thoughts?

**Sam**
Sounds good.

**Pooja**
Awesome and thank you for sharing the issue number here. 

### Pull Requests: 1.  Website: fix index.html issues ethereum/EIPs#5572 2. Configuration: Add "furter" to whitelist ethereum/EIPs#5586 3. Configuration: Add MathJax ethereum/EIPs#5596

**Pooja**
Next one is pull request. I have listed three pull requests. None of these are EIP related but it looks like small changes into process and some of the internal file that is helpful, so if we can discuss this quickly that is fine. First one is issue. Anyone has any objection maybe quickly want to take a look?

**Lightclient**
Yeah, I can go through this after the meeting.

**Pooja**
That sounds good. So there are three pull requests I'm just sharing number 5572, 5586 and 5596. If other editors may take a look it looks like that needs some kind of approval or merging yeah, please feel free to do that. 

## 4. Past meeting discussion continued: Update EIP-1: Add adoptable field ethereum/EIPs#5533 [22:35](https://youtu.be/JKsUrL0VOxU?t=1355)

**Pooja**
Next one is from the past meetings discussion continued. It is I think from the adoptable, yeah probably we can skip this one and move on to the next one that is EIP's insight. 

## 5. EIPs Insight - Monthly EIPs status reporting.[22:51](https://youtu.be/JKsUrL0VOxU?t=1371) 

**Pooja**
Next one is from the past meetings discussion continued. It is I think from the adoptable, yeah probably we can skip this one and move on to the next one that is EIP's insight. I am trying to open the link here quickly. 

So in the month of September we have received one final EIP, okay, and other than that we have received nine ERCs as draft and the one, I’m so sorry about it for some reason my computer is lagging and two EIPs in review status, so the EIP which is in final status is EIP-3525 semi fungible token. Congratulations to the team for reaching out to the final status and the EIPs into review statuses are EIP-5216 and EIP-5484. Please check out the link in the agenda for details of all these EIPs. 

## 6. EIP Editing Office Hour: Meeting 1 Recording [23:57](https://youtu.be/JKsUrL0VOxU?t=1437) 

**Pooja**
Next one is EIP editing office hour. We had EIP editing office hour first meeting yesterday and the recording is added to the agenda. This was very interesting in terms of like this is the first time we were inviting all authors to come forward to share their questions, comments, concerns related to the EIP process or anything that they are facing in documentation of the process. We were also looking into some of the new EIPs plus the EIPs which are getting into last call or maybe in the final statuses. So if you are an author with an active proposal in the EIPs GitHub repository and if you have questions you want to reach out to EIP editor, I think that is the best one for you to reach out to. The next meeting is planned on September 20, at 15:00 UTC. You can find the details at Ethereum Cat Herders’ discord. So that's about it. 

**Felix**
So that's the new apprentice, like meeting? the new name for apprentice?

**Pooja**
So the apprentice meeting was for people who were interested in becoming EIP editor and obviously there would be some learning which can be useful for people interested in becoming editor but this is generally to invite authors, EIP authors who are trying to document a proposal to make it an Ethereum standard. We are receiving as you can see this month only in in past seven days we have received nine ERCs as merged as draft, so these authors if they are facing any challenges they are invited to reach out to us and we will be happy to support moving their proposal towards final.

**Felix**
Okay, so for the YouTube channel we will you guys have the new series of like a playlist or will be the same as the apprentice?

**Pooja**
Yeah, I remember creating it yesterday, may have missed making it public but definitely I'll do that today. So yes there will be a new playlist, it will be it is known as EIP editing office hour and all the meetings from this point forward will be added in that, so yeah, it will be easier for you to just follow one playlist and you can get all the meetings.

**Felix**
Okay, thank you. 

## 7. Review action items from the previous meeting: EIP number bot, what license to use for EIP assets

**Pooja**
Okay. Next one is a review of action items from the previous meeting. I know we discussed about EIP number bot I'm not sure if there is any progress on that. Anyone has any information or update on them? 

All right looks like this is still open, so we will keep it that way just wondering if this has been added as an issue on any of the GitHub repository. Sorry Matt, you were trying to say something. I saw you unmuted.

**Sam**
I know Pandapip was talking about adding it to their bot but I’m not sure where they're at so far. 

**Pooja**
Okay, I’ll take a look and if it is not added in the EIP bot GitHub repository I will make sure to create a new issue for this and what license to use for EIP assets looks like…I'm blanking…did we make any decision on this? I remember discussing this topic…anyone remembers that I don't know if we made a decision yet?

**Sam**
I think I’m kind of being stubborn about wanting other things than just cc0.

**Pooja**
And is there any action item like anyone can help support get that thing done or do we want to have it added in the next meeting?

**Sam**
I think keep it on the next meeting it's probably a good idea I know a lot of people feel strongly about this so.

**Pooja**
Okay, then I will move it on to the next meeting well that's all. Looks like added on the agenda today anyone else want to bring anything looks like we are having some time if anyone has any point to discuss, we can probably check it? If not I think it's an early release for all editors as well.Thank you everyone for joining us today. Hope to see you in two weeks, have a good one everyone. 

**Sam**
See you and thanks for hosting.

Everyone wishes goodbye. 

---------------------------------------
# Attendees

- Pooja Ranjan

- Sam Wilson

- Jose

- Lightclient

- Felix


# Date for Next Meeting: 21 September 2022 at 1400 UTC.



