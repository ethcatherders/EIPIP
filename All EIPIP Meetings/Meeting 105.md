# EIPIP Meeting 105
### Meeting Date/Time: June 05, 2024 at 17:30 UTC
### Meeting Duration: 35 mins
### [GitHub Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/337) 
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=5yhgfqMWg_M)
### Moderator: Pooja Ranjan
### Notes: Meenakshi  Singh
### Next Meeting Date/Time: July 03, 2024 at 17:30 UTC
____

## Summary

|S No :  |  Summary  | 
| -----|   -------- | 
| 105.1| EIP-8607 Rendering issues on eips.ethereum.org. @poojaranjan found no issue, but rendering in GitHub may be problematic. CI needs fixing before merging.|
|105.2| EIP-8590 Okay to merge, but remove “TBD” if moving to Final. Check with @SamWilsn and @lightclient on Discord.
| 105.3|  EIP-8390: One-month review period seems reasonable. Suggest making a Call For Input to gather thoughts from other Editors| 
|105.4| EIP-8247: Comment flagged as spam. @SamWilsn approved; awaiting two more Editors’ approval.|
|105.5| EIP-8503: Requires 3 Editors’ approval. @g11tech and @xinbenlv approved; check with @lightclient.|
|105.6| EIP-8610: Unclear user query. Suggest leaving a comment and helping the user create a thread on FEM.|
|105.7| EIP-8034 proposes adding a changelog section to the Preamble. Proposed in 2023, it received attention on FEM. Editorial and governance considerations discussed. May be proposed to a “Working Group.”|
|105.8|Versioning should be managed manually; linking EIPs to specific commits may increase burden. Optional changelog field suggested. |
|105.9| Consider making the proposal “Informational” rather than “Meta.”|
|105.10|Discuss adding it to the Preamble in upcoming EIPIP meetings.|
____

## 1. Discuss Open Issues/PRs, and other topics

### Edit to Final Proposals

### [ethereum/EIPs#8607](https://github.com/ethereum/EIPs/pull/8607)

**Pooja Ranjan** [00:00](https://www.youtube.com/watch?v=WYBETopsYL4&t=0s): Welcome to EIP IP meeting 105. This is issue number #337 on Eth Cat Herders EIPIP GitHub repository. On our agenda we have items to discuss with respect to open issues and pull requests. We would like to discuss some of the changes to the final proposals. Some updates to EIP 1 which has been standing for quite some time. And there are I think one or two issues that may require some attention. Other than that I'm curious to hear thoughts about EIP versioning proposal. This proposal is in the Pull Request for about 6 months now but in the recent days we have received strong recommendation coming up from the testing team. So I would love editor's feedback on this proposal. And if we can perhaps merge this and look into some of the other details that requires editors attention. There is a process document shared by Tim Beiko recently about All Core Dev Network upgrade and Eth magician process Improvement. So if we can collect some feedbacks and thoughts on that that would be nice to have. We can perhaps take a look at EIPs insight for the month of May as well as June. Yeah so that's all about it let's go ahead and begin with the item number one which is edits to final proposal. We are talking about the PR on EIP GitHub repository and the number is 8607. It suggest a change to proposal EIP 2982 to fix table. Yeah but surprisingly I don't find an error. When I look that EIP on eips.ethereum.org I wonder if anyone can see it differently and if there is an error can we Merge this PR.

**Victor** [2:03](https://www.youtube.com/watch?v=WYBETopsYL4&t=123s): I can take a look and I think it's okay if they actually say display. Sure we should.

**Gajinder** [2:12](https://www.youtube.com/watch?v=WYBETopsYL4&t=132s): I think he has just arrayed the header and I think that the rendering might not be an issue at all. So there could be no actual issue, maybe the person is just trying to get in a contribution but even then I think the CI is not passing. So unless he can fix other things in that particular EIP to make CI pass. We won't be able to merge it anyway. 

**Pooja Ranjan** [2:44](https://www.youtube.com/watch?v=WYBETopsYL4&t=164s): Right, that was my fear in the first place that when I look into that EIP it seems perfectly all right and table is rendering just perfect. So I wasn't sure what this pull request is all about. Very well I don't know if it.


**Victor** [3:03](https://www.youtube.com/watch?v=WYBETopsYL4&t=183s): Yeah it seems it's rendering correctly this one doesn't add Merit.

**Pooja Ranjan** [3:08](https://www.youtube.com/watch?v=WYBETopsYL4&t=188s): Then in that case we might want to close the PR.

**Gajinder** [3:11](https://www.youtube.com/watch?v=WYBETopsYL4&t=191s): Maybe try rendering it in the GitHub itself. Maybe there is some issue over there I don't know. 

**Pooja Ranjan** [3:24](https://www.youtube.com/watch?v=WYBETopsYL4&t=204s): It would be nice like someone can maybe review and if that seems to be not adding value to the existing EIP which is already in final status. we may perhaps want to close that pull request. Very well. 

## [ethereum/EIPs#8590](https://github.com/ethereum/EIPs/pull/8590)
**Pooja Ranjan** [3:40](https://www.youtube.com/watch?v=WYBETopsYL4&t=220s): The next one is on the EIP GitHub repository and the PR number is 8590. So this seems like we have received a two editor comment here. One says that it can be merged and another one says that it cannot be merged. I wonder what people think? We need to create a call for input for this to make sure that we have all editors on board. Yeah please share your thoughts. 

**Gajinder** [4:12](https://www.youtube.com/watch?v=WYBETopsYL4&t=152s): I mean it's only adding the fork time to a value which was EBD which should not have been in the first case. When it was sort of move to review as but at least at the final call. So I mean I'm okay with this, I don't see a problem. 

**Victor** [4:36](https://www.youtube.com/watch?v=WYBETopsYL4&t=276s):There were many previous core EIPs that's the if they specify Fork number. It was left TBD until very long it seems common we don't have a I don't think we currently have very strict way to track to like we didn't make it a strict rule to enforce this as far as I can Remember. But I'm also okay for this to be merged into it. I don't have strong objection.

**Gajinder** [5:08](https://www.youtube.com/watch?v=WYBETopsYL4&t=308s): Even if an EIP is going into final there should be no TBD.

**Pooja Ranjan** [5:14](https://www.youtube.com/watch?v=WYBETopsYL4&t=314s): I agree yeah we can perhaps make it a point like whenever anything is moving from last call to final proposal there should not be any TBD either you remove that section entirely if you do not have any final value to be added there or else we should have a number. Very well it seems like Victor is also not opposing merging the PR. We can perhaps like maybe check with Sam as well if he has any strong opinion otherwise this pull request can be merged. So we can wait for another week.

**Gajinder** [5:56](https://www.youtube.com/watch?v=WYBETopsYL4&t=356s): Either we need to check with Matt because He's the one who sort of proposed it.

**Pooja Ranjan** [6:03](https://www.youtube.com/watch?v=WYBETopsYL4&t=363s): Right okay. So we'll keep it open for another meeting or if we can get any answer from Matt I will try to check it async on our Discord. We'll Marge it otherwise we'll bring it up in the next meeting. 

[ethereum/EIPs#8390](https://github.com/ethereum/EIPs/pull/8390)

The next one is a PR number 8390 which is for fixing EIP 152. It's a kind of a fixed reference test. It seems like a the authors who may perhaps approve or or like confirm the changes they are not around. I remember a few years ago we had this discussion like what do we do with the Pull requests for which we do not have author around the general idea was to merge it with editors permission like editors can overwrite the author's permission here but there was no timeline defined like after how long? What we were practising in those days were like keep it open for about a month and if we do not hear from the author and editors strongly feel that this can be merged there is no problem in merging that. They can perhaps override and merge. I wonder what editors on board here think about it and can we maybe we add one sentence defining the timeline about how long should we keep this kind of proposal open when editors are fine merging them. Okay call for Action. That's a good suggestion. We can do that but in general what are your thoughts like maybe we can keep it open for a month does that four weeks timeline sounds okay for any PR to be open where editors are fine merging them and we do not hear from author. Okay cool. So we can perhaps create a call for input for that One. 

## Update to EIP-1

**Pooja Ranjan** [8:23](https://www.youtube.com/watch?v=WYBETopsYL4&t=503s):  The next one is an update to EIP -1. I'm not very sure about the user also who has added some comments at the bottom so just wondering if that user seems to be a spam?

**Bumblefudge** [8:38](https://www.youtube.com/watch?v=WYBETopsYL4&t=518s): Definitely spam.

**Pooja Ranjan** [8:40](https://www.youtube.com/watch?v=WYBETopsYL4&t=520s): All right. 

**Bumblefudge** [8:42](https://www.youtube.com/watch?v=WYBETopsYL4&t=522s): Its a bilingual jokes but if you speak Spanish it's definitely spam. It's kind of a de nut comment. 

**Pooja Ranjan** [8:48](https://www.youtube.com/watch?v=WYBETopsYL4&t=528s): Very well and this Pull request seems to have 


**Gajinder** [8:52](https://www.youtube.com/watch?v=WYBETopsYL4&t=532s): Even PR is not Spam but yeah  comments in the Spam.  


**Pooja Ranjan** [8:57](https://www.youtube.com/watch?v=WYBETopsYL4&t=537s): Yeah the PR is not. The PRs seems to have received quite a lot of Thumbs Up and I remember seeing some tweets around that as well it seems people are generally on board. Is there anything specific that we are waiting for or can it be Forced merged. 

**Bumblefudge** [9:19](https://www.youtube.com/watch?v=WYBETopsYL4&t=559s): Fine with me I'm not waiting for anything.

**Gajinder** [9:22](https://www.youtube.com/watch?v=WYBETopsYL4&t=562s): I think Sam already approved it I don't know yeah what it's waiting for? 

**Pooja Ranjan** [9:30](https://www.youtube.com/watch?v=WYBETopsYL4&t=570s): I'm not sure if someone can maybe try closing and opening the issue it may merge this proposal directly if not then I will bring it to the next editing office hour to check with Sam if he can push it. 

**Gajinder** [9:43](https://www.youtube.com/watch?v=WYBETopsYL4&t=583s): I think required two more reviews. So I can approve it and then I think one of the either Victor or Matt needs to approve it as well.

**Victor** [9:54](https://www.youtube.com/watch?v=WYBETopsYL4&t=594s): Sorry which one?

**Pooja Ranjan** [9:57](https://www.youtube.com/watch?v=WYBETopsYL4&t=597s): 8247

**Victor** [10:01](https://www.youtube.com/watch?v=WYBETopsYL4&t=601s): 8247okay. yeah. I was approving the previous one they just need another approval. Okay. I need to take a look it seems like.

**Pooja Ranjan** [10:17](https://www.youtube.com/watch?v=WYBETopsYL4&t=617s): Very well. So it's just approving issues looks like for that one if someone can approve and it gets merged fair enough if not then we'll bring it to the next office hour to make sure it is Merged. 

**Gajinder** [10:31](https://www.youtube.com/watch?v=WYBETopsYL4&t=631s): Should I approved it and I think one more approval would be needed. 


**Pooja Ranjan** [10:38](https://www.youtube.com/watch?v=WYBETopsYL4&t=638s): Thank you.  Victor if you get a chance please take a look and if you find it okay then maybe it can be merged automatically. The next one is a PR 8503. It seems to be a pull request by Sam Wilson to update EIP-1 for EEST. I think EELS test EELs is the specification that they are building around execution client to me it seems like it is just waiting on editors approval. So if editors can maybe take a look at this one as well the PR number is 8503.  I'm not sure if this is defined anywhere but it should have been maybe EIP-1 changes requires more than three editors approval. Cool.


**Gajinder** [11:41](https://www.youtube.com/watch?v=WYBETopsYL4&t=701s):  Yeah I think so I approved it as well so maybe two more on edit. 

**Pooja Ranjan** [11:47](https://www.youtube.com/watch?v=WYBETopsYL4&t=707s): Yeah and I don't think Sam would be able to because he is the author of this one so we might want to look for other editors on call. Okay cool thank you Victor. 

**Gajinder** [11:55](https://www.youtube.com/watch?v=WYBETopsYL4&t=715s): So Victor and matt.

**Pooja Ranjan** [12:02](https://www.youtube.com/watch?v=WYBETopsYL4&t=722s):  Victor has already approved so we'll check with Matt for all of these if he can approve
Them. The next one is a miscellaneous issue and the issue is. Okay fine I'm not sure what proposer wants to do over here it doesn't seems like it is added with some of the pull request. If it is a general question which the author which the user could not find a good place to write the question to receive an answer this could be one or else it could be a Spam one. 

**Victor** [12:35](https://www.youtube.com/watch?v=WYBETopsYL4&t=755s):  Are we talking about 8610?

**Pooja Ranjan** [12:38](https://www.youtube.com/watch?v=WYBETopsYL4&t=758s): That's right.

**Victor** [12:56](https://www.youtube.com/watch?v=WYBETopsYL4&t=776s): The person says they are not able to Pro to create. 

**Pooja Ranjan** [13:04](https://www.youtube.com/watch?v=WYBETopsYL4&t=784s): Well. Yeah this seems unclear like what is the question here what kind of response he's Expecting? Maybe someone can take a look and if this seems like an spam definitely the next comment seems like an spam here it's in different language.

**Gajinder** [13:27](https://www.youtube.com/watch?v=WYBETopsYL4&t=807s): Sort of a technical Query that he wants to do some signing and across chain and I don't know what he wants it to happen in certain way.

**Victor** [13:41](https://www.youtube.com/watch?v=WYBETopsYL4&t=821s): My view is this should be post on the Ether spam ethereum magician. This is a technical discussion and this the way how they. It is not the best way to generate the proper discussion. If they cannot do it I can help cross post it. I don't fully understand what they meant. But yeah I don't think anyone is blocked from using ethereum magician. 


**Pooja Ranjan** [14:11](https://www.youtube.com/watch?v=WYBETopsYL4&t=851s): That's right. Maybe we can add a comment over here to check with the user. If he has any specific query with respect to like changing chains with respect to EIP 712 and if he can maybe start a conversation at FEM. 

**Bumblefudge** [14:28](https://www.youtube.com/watch?v=WYBETopsYL4&t=868s): Yeah it sounds to me like something specific to like metamask or VM or some the the the question isn't even a question that I think the authors of EIP 712 could answer it's like something more mundane about implementation while or browser implementation. In any case I think Victor is right that they're it is very weird to post here because you can't figure out the discourse plug it you know identity system. Eth magicians is pretty easy to set up an account I mean I guess I haven't done it recently but I wonder what they meant about not being able to post there. 

**Pooja Ranjan** [15:13](https://www.youtube.com/watch?v=WYBETopsYL4&t=913s): All right. So we can just drop a comment for the user and you will take it from there if he or she may find any issue creating an account. We can perhaps help getting that done. Very well. We do not see any call for input this week. Ah that's great, surprisingly this is the first week as far as I can remember that there is no call for input. 

## 2. Other discussions and updates from past meetings

So let's move on to the next section for the agenda and that is other discussions and updates from the past meetings. So in one of the earlier meetings we talked about EIP versioning proposal. I think I have added the link to the pull request that is 8034. This EIP was proposed back in December 2023. It seems we had quite a lot of conversation and discussion on Fellowship of ethereum magician and these people are very much willing to get the proposal merge in like you know in draft. So they can use this number start talking about it and recently in today's EOF meeting and also in earlier EOF meetings testing team. Team showed great support of the versioning scheme for EIPs. The questions that they are wondering are like can we add this change log section to EIP template in like Preamble section. And who should be the best person to update this change log like can it be the author? Can it be the editor? They want this thing to exist
in order to make sure the test cases they are developing are with respect to a specific EIP. And they would be following it easily if the change log number is changed. So they know that their spec is not up to date and they can perhaps update that I wonder what editors think about it and can we merge this proposal. 

**Victor** [17:19](https://www.youtube.com/watch?v=WYBETopsYL4&t=1039s): So editor opinion on my side editorial opinion is that this kind of proposal should be able to merge as a draft and as a proposal to generate more discussion. Because it's a policy discussion my governance comment on this is that I'm generally in favor of supporting
versioning and upgradeability like Improvement on EIP and ERC's. The hard part is about defining who gets to own the newer version who gets to decide which newer version is the canonical one. There's definitely going to be cases where there's a base version that say EIP 712 as an example. And there will be different opinions and how they would be it
Extended. So I think Bumble is here so he has experience ietf. I well how iatf works is that they create this kind of they Define this kind of working group. And working group owns the current and future rfc's under that working group. And the ietf has governance process to Define which ERC which rfcs for under the the the care of which working group and how to start a working group. Currently it's hard. So I think this the this the governance of this meta proposal should be surfaced to the working group to the road map that project you also proposed to should be included in that kind of discussion. Otherwise it is going to be hard to to do within the current setup. So in some quick summary editorially I am in favor of merging it so that people can discuss. On the governing govern side I don't know how to do it I think it needs to be included in the working group and road map discussion of. 

**Gajinder** [19:37](https://www.youtube.com/watch?v=WYBETopsYL4&t=1177s): So just to be clear is the proposal saying that while the EIP is in review it can have multiple versions. I don't understand because once the EIP is final there is just single conical version because it's talking about standard RBS.

**Pooja Ranjan** [19:58](https://www.youtube.com/watch?v=WYBETopsYL4&t=1198s): That is correct. The idea here is to like when client goes for implementation they come up with different spec changes. So keep track of these spec changes they want to version it in terms of major minor and patch. And there are further discussions around like what they would like to capture according to them major should be any breaking changes to specification. Minor could be anything in addition to specification but does not require changing and existing implementation. And Patch could be like something cosmetic if we are doing for example I mean even I was engaged in this conversation for example here like if a proposal is under draft or review and they are being considered for an next Network upgrade client can go ahead and Implement that with one spec. But if there is any minor spec change or major spec change that is not possible to be tracked because we do not have versioning and testing team are not aware of that. So this particular proposal will be able to provide them that visibility and once the proposal is final it is fun then we do not expect any  change. But in case of any cosmetic change say for example we receive some typo error. So we can perhaps change the number of patch it is in terms of x. Y. Z. So we can perhaps keep on changing of the number of patch and testing team does not have to do anything with that but for General people they would know that this proposal may have received some changes. Well so that's the idea here.

**Gajinder** [21:49](https://www.youtube.com/watch?v=WYBETopsYL4&t=1309s): I think my my opinion on this is that we shouldn't be doing anything because for example if we look at the devnet process right. So how it moves is that at some particular Devnet Target. You have some particular spec that is already outlined and the spec team can just link the EIP with the particular Comet hash right. So it doesn't really change anything I think it only increases the bookkeeping and is unnecessary in my opinion. Because more things you ask people to keep hard the
process will be.

**Bumblefudge** [22:37](https://www.youtube.com/watch?v=WYBETopsYL4&t=1357s): Yeah I I kind of agree I've been thinking this whole time that like with suspects sometimes we do commit specific links. If something's changing and you know there's commit specific links were just added from you that the EIP-1 PR to add Casa links part perhaps because we started that precedent of using them internally to refer back to like you know but be sometimes when a there's major changes to a spec a cape before final we say before this commit the syntax was totally different. So old implementations older than that may have like whatever so yeah I mean I I would also say that since it's already happening on GitHub maybe GitHub is good enough or or simpler to Peg to testing I would say that if if this were added  it could be maybe like optional front matter so that if  an EIP just totally wants to ignore it they just can and and if someone messes it up it doesn't throw a wrench in the whole thing like I feel like if you make it loadbearing and then someone forgets to bump the version or bumps a y instead of a z when they're just fixing a typo then it creates this whole governance thing because you were assuming they were always accurate like if you made it sort of a optional informational s thing it might be really useful to some working groups or Some EIPS. And then the rest could ignore it. I don't know.

**Pooja Ranjan** [24:29](https://www.youtube.com/watch?v=WYBETopsYL4&t=1469s): That sounds like a good suggestion like for example we have a an optional Preamble field where we add the EIP number as like you know required EIPs for the proposal it's not for all of the proposal but for certain proposals which are kind of enhancement on any existing one they use this field. So if protocol upgrade texting team is requesting for this kind of specs editors may consider it for as an optional field. And this may or may not be needed for say for example ERC's or EIPs. It can be used as needed otherwise we can define a default value that can be used for example EIP 712.00. So no changes nothing like that we can start with a default value and only for the proposals which may require this kind of changes spec changes can use that. I wonder Gajinder do you think it is still adding too much on authors or editors to maybe keep a track off. 

**Gajinder** [25:40](https://www.youtube.com/watch?v=WYBETopsYL4&t=1540s): Yeah I mean given editors won't be able to take a call on all the proposals whether it is a minor version or a major version or a patch version change right and but again we can defer it to the EIP authors for that but or maybe optional can work but again in terms of practicality. I actually see I mean it's it's basically easy for someone just to clone the repo and attach a tag to it and use that tag to circulate it. So I'm not really sure basically but like if if this is just to be for people who are doing Dev work on that EIP. I mean they they can track it in better mechanisms and actually for example what I mentioned earlier was that people would want to look at some particular devnet spec rather than at some particular version because that is what they are targeting to Dev with other teams.

**Pooja Ranjan** [27:00](https://www.youtube.com/watch?v=WYBETopsYL4&t=1620s):
Thank you. Victor do you have anything to add on this one.

**Victor** [27:07](https://www.youtube.com/watch?v=WYBETopsYL4&t=1627s): I don't think it's up for the community to decide whether they want it. I just I think it's okay to merge into it. And then also I would personally suggest them to make it informational rather than meta. But other than that it should be okay to at least ask. 


**Pooja Ranjan** [27:29](https://www.youtube.com/watch?v=WYBETopsYL4&t=1649s): Yeah all right. So I think we had three basic questions here number one can this be merged today. It seems like there is no strong objection on merging this one. Number two can change lock section be added to Preamble like it can be added as a preamble optional but that would require again EIP template change which we will bring it in the next meeting. And the third question was like who will be owning this change log update it's it's very much convincing that editors may not be able to make a decision on that so it has to be on the author if he or she decides to change the log. I mean update the log. One thing just quickly to respond to Victor I don't think it can be an informational it has to be a meta because if we are adding it in Preamble that needs to change the template as well and that can only be done on if it is something to be followed by all proposals but as an optional field it would be again optional for the proposal to include or not include this particular field in a proposal. 

**Victor** [28:36](https://www.youtube.com/watch?v=WYBETopsYL4&t=1716s): If it needs to be add to this Preamble I agree it must be Meta. I think actually adding it to the Preamble could be a separate meta proposal rather than proposing this versioning schema. I think the versional schema could start as an informational and every EIP author who wants to do it can just specify it within their own the body of that EIP. Nobody can can disagree with them that there's aversion in their own body  once more we see more adoption I think we can put them into the Preamble. I would be a little bit worry about prematurely adding Preamble for this practice before it becomes widely adopted.

**Pooja Ranjan** [29:31](https://www.youtube.com/watch?v=WYBETopsYL4&t=1771s): Sounds good to me. And thank you for merging the proposal. We can perhaps have further discussion on all core dev meeting and try to collect some feedbacks from client development team as well as testing team I'm hoping them to be there as well on the call to maybe share their point of view and that would generate the status change for this proposal . Very well well at least now these guys will have an EIP number. So they can start talking about it with different teams thank you for merging it. Thank you. Moving on the next one is a proposal change we will briefly discussed this in the last EIPIP  meeting it seems that in naota there was some some discussion around the EIPIP meeting. The processes around EIPs and how some of the network upgrade process can be improved. I know this Fellowship of ethereum magician thread includes process Improvement around multiple aspects. I'll be curious to maybe hear thoughts on the network upgrade process specifically. If I remember correctly yes so there is this proposal of aligning EIP with respect to network upgrade proposal process. So I'm curious what people think about integration in particular and yeah in general if people have any thought on this particular set of process improvements we can take it and maybe if requires like longer discussion can be a part of upcoming meetings agenda
item. I mean people can add the feedback async as well here. I wanted to bring it up in EIPIP meeting because I think if it is for process Improvement we might want to implement some of these proposals or may want to discuss it. So yeah if it is too early we can perhaps discuss it in the next meeting. Very well  the next is EIPs insight and monthly EIPs status reporting. So I think the dashboard is up till May but the EIPsinsight.com provides information for June as well as the hackmd provides the information for the month of June. It seems like we have only two proposals added as draft. Both are ERC and I think there is one more but the the Scheduler is updating this dashboard once in 24 hours. So we might want to take a look into that. And we have received one proposal which is an interface proposal. It's EIP 5792 wallet call API. The last call for the last call deadline is June 26. If anyone interested to add any feedback comment to this proposal. Please feel free to do so you can always drop a comment on Fellowship of ethereum magician. And yeah it would be nice to see the proposal moving forward. So that's on EIPs insight and after that I think I have added a link to the agenda for EIP editing office our meeting number 38 people can also watch the recording for meeting 37. And just quickly taking a look at the notes from the last meeting. Wow, most of them are now closed. All right I don't see any open action item pending for anyone and Sam is not here. So we should be hoping to hear about working RP chatter in the next meeting or whenever he's around that's pretty much covered the agenda for today. If anyone has anything else to maybe add or propose for the upcoming meeting. Well thank you everyone for joining us today and I look forward to see you in the next meeting. Two weeks from now. Thank you.
___
## Attendees

* Pooja Ranjan
* Gajinder
* Abel A Ambriz Jr
* Bumblefudge
* Zainan Victor Zhou

 
