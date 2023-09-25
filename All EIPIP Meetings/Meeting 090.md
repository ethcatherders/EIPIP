# EIPIP Meeting 90 Notes
### Meeting Date/Time: Wednesday, Sept 20, 2023, at 14:00 UTC
### Meeting Duration: 0.5 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/271)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=PuHXWqWkbXg)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION/DECISION  ITEMS

**ACTION 90.1**:  We will wait till October 5th to make a final decision on PR-7665

**ACTION 90.2**: In regards to Call for Input (Multiple items) Ref:[EIPIP Issues](https://github.com/ethereum-cat-herders/EIPIP/issues), We can talk about decision items in the following EIPIP meetings.

**ACTION 90.3**: In regards to [EIP-5069](https://eips.ethereum.org/EIPS/eip-5069)'s new charter stuff, will follow the proposal to learn about EIP Editors' working process.

**ACTION 90.4**: [Ethereum/EIPs#7550](https://github.com/ethereum/EIPs/pull/7550)PR is good to merge.

**ACTION 90.5**: In regards to EIP-ERC GitHub repositories Ref. [EIP-7329](https://eips.ethereum.org/EIPS/eip-7329), Matt's PR needs to be rerun before merging. @SamWilsn will send an invite to @lightclient, @Pandapip1 and others to work this through and updates will be provided in the next meeting.

**ACTION 90.6**: PR-7230 will be closed.

**ACTION 90.7**: @SamWilsn will look into rewording the exit process for EIP editors in EIP-5069 as suggested by @gcolvin.

—------------------
## AGENDA

**Pooja Ranjan** [0:00](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=00s): Welcome to EIPIP meeting 90. This is issue number 271 on EIPIP GitHub repository. I have shared an agenda in chat.  We have a pretty light agenda for today. We have discussed open issues / pull requests  discussion continued and updates from the past meeting
0:23
monthly Insight a little bit about EIP
0:26
editing office hour

# 1. Discuss Open Issues/PRs, and other topics

**Pooja Ranjan** [0:28](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=28s): So starting from the very first item.

- [Website: Remove Networking and Interface categories ethereum/EIPs#7665]( https://github.com/ethereum/EIPs/pull/7665)& [Call For Input: Remove Networking and Interface categories (ethereum/EIPs#7665) #272](https://github.com/ethereum-cat-herders/EIPIP/issues/272)

 **Pooja Ranjan** [0:31](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=31s): 
I have added a pull request here which is 7665. It is about website removing networking and 
interface categories. It seems that there are a lot of discussions on this particular pull request and we are still not having a concrete decision. I would love for someone to maybe  summarise this and let people know where we are on this. I also see a  similar call for input for making decisions. I'm going to wait till the date is there but yeah if anyone would like to summarise it and explain where we are.

**Sam** [1:22](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=82s): I can't summarise in depth why but I can give a little overview. So I think it's because having a network as a separate category doesn't really make that much sense from a process perspective. Networking changes will often go through a lot of the same decisions and then they have all the same people as core EIPs. so merging them with core eips makes some sense and then the interface category. We have kind of pushed it off to the execution EIP repository. so getting rid of the category might encourage people to stop making new ones. That's kind of my understanding but yeah it's Panda Pep's proposal. So I don't really want to speak on his behalf.

**Lightclient** [2:14](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=134s): I just don't understand why we can't leave them there and deprecate them.

**Sam** [2:23](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=143s): Yeah I think we can. I don't think it's that big of an issue.

**Lightclient** [2:27](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=147s): I just keep saying that we cannot do this. It's not possible and we're just making these things 
up.

**Pooja Ranjan** [2:42](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=162s): Well I think historically speaking Korea is where a part of upgrade and moving an interface on networking to the list of core EIP doesn't feel right to me as as an individual. So I'll be more in favour of letting it live where it is. But there should not be any further new proposal. We can just replicate that category

**Lightclient** [3:08](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=188s): Exactly.

- Call for Input (Multiple items) Ref:[EIPIP Issues](https://github.com/ethereum-cat-herders/EIPIP/issues)

**Pooja Ranjan** [3:16](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=196s): So there is another call for input as I mentioned open for the specific discussion and I hope to get some consensus over there the deadline suggested October.

**Lightclient** [3:30](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=210s): I mean they will not just get consensus. There's three of us here. I don't know how Greg felt about it but it seemed like none of us are in favour.

**Sam** [3:46](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=226s): So I'm not in favour of doing anything until we figure out like the ERC EIP split and whatever we  end up doing with working groups. I do think putting networking and core  makes some amount of sense just because the way I kind of envisioned core is anything that can cause main net to Fork. So if you implement networking differently enough you'll end up forking. If you implement the EVM differently. You'll end up forking so that's why I put them together into their own working group but until then I don't want to until we have working groups and the ERC EIP split. I don't want to mess around with anything.
**Gajinder** [4:27](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=267s): I more or less agree with Sam and Lightclient  over here. Basically we can leave it untouched for now and my  opinion is maybe over time. We can see more of them as tags rather than 
Categories. Basically have a fuzzy kind of a thing where you can tag. You can have multiple tags on an EIP and sort of you know mix have sort of say that this has an impact on these X number of areas.

**Sam** [4:59](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=299s): Yeah  that makes sense too. Okay.

**Lightclient** [5:02](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=302s): But I don't mean we're not going to go back and change the EIPs that exist though is the thing.

**Gajinder** [5:09](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=309s): Yeah I'm finding that.

**Lightclient** [5:15](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=315s): 
so I would just like to leave the EIPs as they are as artefacts not accept new ones and we can figure out the working group.I mean the tags is nice but I don't want to Retroactively 
update all these networking EIPs nor do I think we should move them because then we're going to break links.

**Sam** [5:39](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=339s): Yeah I think breaking links is not going to break links well. We can make that a rule but if there's a like if we change the rendering system so that it uses tags for example then I think it makes sense to update everything that way. We don't have to maintain two different rendering systems but that's a discussion for when we update the rendering system.

**Pooja Ranjan** [6:06](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=366s): So, I wonder Greg if you have any thoughts on this.

**Pooja Ranjan** [6:24](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=384s): Sorry you may be on mute Greg.

**Gcolvin** [6:27](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=387s): Oh I'm muted instead of unmuted. I'm still way too hammered by this move to have been thinking about any of it. Unfortunately but I would tend to think that the networking stuff really is core stuff even though it isn't directly part of the protocol. If it's important at all it generally
has to do with networking with. I'm sorry uh I'm not coherent today.

**Lightclient** [7:05](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=425s): I mean I don't disagree with people that networking is very core thing but we just don't use EIPs for Network anymore. So it's not really a debate about. Will we in the future have more EIPs in this networking category should future EIPs related to networking B and core B in networking B in a core tag with networking. We just don't have networking IPS so it's a question about what to do with old EIPs that are a networking category.

**Gcolvin** [7:34](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=454s): Oh! just leave them alone. They're existing, that's how they were categorised. There's nothing to do with them but leave them that way.

**Pooja Ranjan** [7:52](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=472s): So if we try to split it into topics, there are two topics of discussion. Number one what to do with the older EIP and it seems like most of the people on the call. They are okay to let it leave the way it was living and the next question is should we have any further networking or interface. VIPs in future and if we do, we might need a working group. It seems we may not need.

**Lightclient** [8:20](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=500s): Yeah I mean I think that's something that we can figure out in the future. I think we should focus on coming up with the working group for core changes as we Define core to be today. And if at some point in the future. People desire to write EIPs related to networking then we can cross the bridge but I don't want to try and you know figure this out ahead of time before we really know what people want.

**Pooja Ranjan** [8:51](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=531s): That makes sense and hopefully this is the right time to maybe even Define core and based on the definition of core maybe we can have people for coworking grow.

**Lightclient** [9:11](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=551s): Yeah I mean core to me is something that modifies the consensus protocol.

**Pooja Ranjan** [9:23](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=563s): Perfect so if we have to move on from here. I'm trying to just move on from the first item that was PR number 765. It seems We want to leave where we are  moving from here. If we have to define the different categories like the core and the ERC, I believe will be the two major categories for which we might need a working group. I have a proposal, I don't know if this is fair or not but um just want to share it with people here. Do we really need to keep the category? Can we redefine them as types so like earlier we have one standard track and we have four different categories over there. It creates confusion when we are trying to organise the EIP types categories and the process as a whole. What do people think about instead of
calling it standard track ERC. We just call them our VRC standard track core as just core and meta and informational.

**Sam** [10:38](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=668s): Yeah I think that generally makes sense. I'm still kind of fleshing out some of the details on working groups but that's kind of what they look like. It's just like you have just working groups, a core working group like in eip's. Meta governance working group and then that's it pretty much all the categorization we have.

**Pooja Ranjan** [11:04](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=664s): The reason for the proposal is like I really do not see a relevance of all these like you know proposals being a part of the standard track type. So they can live independently and I think that would be easier for communication purposes as well.
**Sam** [11:23](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=683s): Yeah that makes sense to me.

**Pooja Ranjan** [11:27](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=687s): Okay anything more on this item before we move on.

**Lightclient** [11:39](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=699s): Can we close this remove networking interface categories.

**Pooja Ranjan** [11:45](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=705s): That's a good call to hold request number seven double.  What do people think?

**Sam** [11:50](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=710s): So
point point of order. We can't close it until we get input from the exec consensus.

**Sam** [12:02](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=722s): We don't because access hasn't presented an opinion yet. 

**Lightclient** [12:07](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=727s): Guys 

**Pooja Ranjan** [12:10](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=730s): Oh don’t worry, we have a deadline for that and that is on the 5th.

**Lightclient** [12:17](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=737s): Guys it's already a rough consensus. The majority of us already agreed let's do this. Why are we? I mean we're just gonna waste a bunch of time. Now we're gonna rediscus. This three more times.

**Danno Ferrin** [12:38](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=758s): Asics removal expires in about 15 days, so that's the real deadline.

**Pooja Ranjan** [12:43](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=763s): Yeah Sam if you could maybe explain what happened. Majority or any decision on any decision items.

**Sam** [12:57](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=777s): It's  every editor is entitled to their opinion so everybody gets to say what they think. If they don't answer within 30 days from the call for input then whatever the consensus is at the 30 days from the call for input is the decision. so it isn't a vote, it's still a rough consensus and each decision is limited to 30 days at most.

**Pooja Rajan** [13:24](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=804s): So if we do not have absolute favour or denial we will go by rough consensus like whatever is majority we will get there right.

**Sam** [13:35](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=815s):  Yeah so here we're going to be electing somebody as keeper of consensus. Which is kind of just a
person who determines what the rough consensus is and when it's been reached. Then yeah that's what if that person says, there's a consensus that's been reached then the decision has been made as long as everybody has the opportunity to you know give their input.

**Pooja Ranjan** [14:05](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=845s): Sounds good. So do we want to when the deadline is met. Do we want to just bring those items on EIPIP meeting just to communicate the decision to the community or will it just be close in the issue. What do you think will be right.

**Sam** [14:25](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=865s): I mean we can definitely talk about it on EIPIP. I don't have a problem with that.

**Pooja Ranjan** [14:36](https://github.com/ethereum-cat-herders/EIPIP/issues/271&t=876s): Sounds good. All right I think we should perhaps wait till the deadline of the discussion item and we'll bring it after the fourth on 5th of October. Anything else on this one?

# 2. Discussion continued or updates from past meetings 

**Pooja Ranjan** [15:04](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=904s): All right let's move on to item number two which is a discussion continued or updates from past meeting

- [EIP-5069](https://eips.ethereum.org/EIPS/eip-5069)'s new charter stuff.

**Pooja Ranjan** [15:12](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=912s): So I see EIP  5069 that has incorporated Charter staff and it is added as meta. It explains the mission structure, membership decision making process and everything else I wonder about. If there are any further things that we would like to communicate or do we need to update it any further. Very well, so that's there are people coming up on this card for questions around what EIP editors can or cannot do for those people I highly recommend following EAP 5069 that explains what is expected by them and what authors should be performing on their own
foreign.

- [Consider adopting a Community Specification License terms for the new ERC repo  ethereum/EIPs#7482](https://github.com/ethereum/EIPs/issues/7482) - Anyone has any update to share? [Ref last summary](https://github.com/ethereum-cat-herders/EIPIP/issues/260)

**Pooja Ranjan** [16:21](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=981s): Okay next one is from the past meeting, So the item for discussion was considered adopting a community specification licence term for the new ERC Depot and we were expecting some updates from I suppose it was from Victor and I believe Vector is not on the call today. But he drew some comments here on the discord. It suggests that the copyright licence for ERC left Depot  thinking of a pc0 plus Apache 2.0 dual licence and that's what it's from his side. Anyone else has any other information to add here.

**Sam** [17:12](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1032s): Licences suck at it that you don't ever want to talk about.

**Pooja Ranjan** [17:18](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1038s): I think we learned about a new licence type yesterday as well.  I think in the last EIP editing office hour we came across. A new something new I may have been missing never mind. All right so that's the only update shared by Victor.


- [Update EIP-721: Add ERC links ethereum/EIPs#7550](https://github.com/ethereum/EIPs/pull/7550) - Good to merge the PR?

**Pooja Ranjan** [17:53](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1073s): Yeah we can move to the next one next one was updating EAP 721. I suppose the decision made on the last call was if there was no objection. We can merge The Proposal after two weeks and it's more than two weeks so I was just wondering if it is good to merge the pr number is 7550

**Sam** [18:32](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1112s): Yeah I think I'm okay to merge this still.

**Pooja Ranjan** [18:38](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1118s):  Okay cool. So we'll Market that and yeah whenever you get a chance please merge that.

- EIP-ERC GitHub repositories Ref. [EIP-7329](https://eips.ethereum.org/EIPS/eip-7329)

**Pooja Ranjan** [18:45](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1125s): The next one is EIP ERC GitHub repositories. So I see proposal 7329 ERC EIP repository split a meta proposal by Matt and Deno is now in the final status. I wanted to bring it to the agenda to maybe figure out what are the next steps from here when we are expecting this repo split. Is there any new PR or Matt initial PR still hold good or anything that we would like to share with the community in form of announcement or updates on this

**Danno Ferrin** [19:36](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1176s): Matt, would we need to rerun your script to update the EIP? I mean the PR.

**Lightclient** [19:44](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1184s): I mean definitely but this isn't really something I think we can just like do on our own like we
i need to sit on a call with panda and Sam. You know spend two hours and really just urge it and do this do the split in because I don't think that the pr is perfect.

**Sam** [20:07](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1207s): We can schedule the call. I'll send out an invite or something this week.

**Pooja Ranjan** [20:21](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1221s): Can we expect the call in between the next EIPIP call and today so we can have some updates for the next meeting and I can put it up on this and therefore.
**Sam** [20:33](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1233s): Yeah for sure I'll try to get it scheduled either this week or next so.

**Pooja Ranjan** [20:41](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1241s): That would be great thank you. We do have Greg on the call although he mentioned that his connections keeps dropping. I wanted to check the PR 7230. Greg uh that a pull request by you about EIP pain relief. Do we still want to discuss that do you want to close it where we are on that.

**Gcolvin** [21:12](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1272s): Pieces of it are showing up in this. Other work and I'm not sure what status to put it in. It's not exactly withdrawn. I guess it's just a PR so it can sit there. Yeah I think I'm pretty close to satisfied with what's in. There is making it into the various decisions. We're making but it would take
some review but like I said the moves a horror show and my girlfriend's health is has been
 collapsing stage by stage so unfortunately I just have not been able to give this any attention at a fairly crucial time and all I can do is apologise for that. 

**Pooja Ranjan** [22:08](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1328s): No worries I hope things get better at your own pace. Just curious if you find some of the pain points are being addressed with other pull requests. There could be two possible options if you do not want to continue with this Pull request. you can close it perhaps otherwise we can keep it open but if unattended for over two months or so but may strike and it can go into stamen and eventually get close. So yeah totally open for that but if it is not something that you would want me to bring on the next meeting I can perhaps drop it from the agenda for the next meeting onwards.

**Gcolvin** [22:48](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1368s): The next meeting is two weeks out. Let me briefly look at my calendar.I don't think there's any other conferences happening man. Well there was going to be but I'm not going to be able to make it to that one. Yeah I mean it could just be closed. The information is there and no it's not going to get merged as it stands. So it can just be closed because open or close the information is still there

**Pooja Ranjan** [23:47](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1427s): Very well so we will market for today's decision that PR number 7230 will be closed.

**Gcolvin** [23:54](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1434s): Yeah, it's just like I say it's ideas for things that I wanted to see changed but those changes are happening in pieces in other places and it really couldn't even be merged the way it is now without a lot of work. 

**Pooja Ranjan** [24:15](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1455s): Right I'm glad we are at a better place when this PR was only originally drafted. 

# 3. EIPs Insight - Monthly EIPs status reporting.

**Pooja Ranjan** [24:23](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1463s): All right moving on to the next one is EIPs inside for EIPs inside of the month of September. As I can see we have a huge number of EIPs moving in. We have 20 drafts, 12 reviews, 11 proposals in the last call, five proposals are final and 16 proposals are in stagnant status. 60 is a big number for proposals moving into stagnant. We understand that is because of the proposal being unattended for a long period of time. I would take this opportunity to maybe request EIP authors. If you are here if you are making a pull request to create a standard for the ethereum ecosystem.  Please stick around if you have questions. We do have an EIP editing office hour that happens every other Tuesday. Please check out EIPIP GitHub repository issue section for the next meeting and please come up there with your questions. You can add your PR for discussion and we have EIP editor Samuels and they're answering your questions in case you need any help pushing your proposal to what they funnel status. We can check out eipinsite.com with details of all Eips in different statuses proposals in last call. We request EIP authors to make a pull request after the deadline is completed to move the proposal to the final status. Be sure that the pr contains only the status change. If there are more changes with the pull request we would like to review it and perhaps we can extend the review period so we get everything sorted before we finally move the proposal to the final status

# 4. EIP Editing Office Hour

**Pooja Ranjan** [26:34](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1594s): The next one is EIP editing office hour as I mentioned we organise this meeting every two weeks recording from the meeting 25 has been added and agenda for meeting 26 is up there. Please take a look and add your pull request if you have any and that pretty much summarises all the items listed for today. Anyone has anything to bring up. I see a question here in the chat. I'm sorry unfortunately this is not the meeting where we look into the Pull request for draft and review.  If there is any final EIP we consider only those EIP for discussion here. However, thank you for sharing this. I hope this circle request will be reviewed by EIP editors in case of any help please reach out on ethereum Caterers discord. Anyone else has any anything to bring up today share for this meeting.

**Gcolvin** [27:46](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1666s): Just I mentioned it to Sam, I think in 5069 the handbook  forcibly removing and editors is seems an unnecessarily violent way of putting it.

**Sam** [28:07](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1687s): I'm looking to it.

**Gcolvin** [28:11](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1691s): Thanks

**Pooja Ranjan** [28:13](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1594s): Awesome! very well we can give 28 minutes back to all our participants here today. Thank
you everyone for showing us. See you around have a great day everyone

**Sam** [28:29](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1709s): See you

**Gajinder** [28:32](https://www.youtube.com/watch?v=PuHXWqWkbXg&t=1712s): Bye

  ---------------------------------------
# Attendees

* Justin Florentine
* Gcolvin
* Pooja Ranjan
* Sam Wilson
* Light Client
* Jason Windawi
* Zainan Victor Zhou

# Date for Next Meeting: October 5, 2023 at 1400 UTC.



