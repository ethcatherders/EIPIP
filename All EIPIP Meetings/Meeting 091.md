# EIPIP Meeting 91
### Meeting Date/Time: Wednesday, Oct 4, 2023, at 14:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/278)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=mutOWZV2uOw)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----------------------------------------------------------------

## ACTION/DECISION  ITEMS

**ACTION 90.1**:  In regards to [ethereum/EIPs#7806](https://github.com/ethereum/EIPs/pull/7806)Panda will draft a PR to add a field "Superseded by" in the Preamble which will be discussed in the following meeting. So PR kept open.

**ACTION 90.2**: [ethereum/EIPs#7423](https://github.com/ethereum/EIPs/pull/7423)is approved by editors and merged.

**ACTION 90.3**: In regards to manual merge for [ethereum/EIPs#7505](https://github.com/ethereum/EIPs/pull/7505), Lightclient wants to take another look before merging.

**ACTION 90.4**: [ethereum/EIPs#7506](https://github.com/ethereum/EIPs/pull/7506) is approved in earlier meeting and merged.

—------------------
## AGENDA

**Pooja Ranjan** [0:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=01s): Welcome to EIPIP meeting 91. This is issue number 278 on EIPIP GitHub repository. I have shared an agenda Link in the chat. So for today's discussion we have open issues, pull requests and some other topics. Will perhaps discuss things that we have discussed in the past meeting and we'll see where we are at that. We'll share a EIPs insight about editing office hours and we will follow some action items from the past meetings and I see one announcement added to the agenda here.

# 1. Discuss Open Issues/PRs, and other topics

## Changes to Final proposals

**Pooja Ranjan** [0:041](https://www.youtube.com/watch?v=mutOWZV2uOw&t=41s): So starting with the first item. These are changes to the final proposal we have a two PRS added here.

-	[Update EIP-6059: Adds comment about 7401 superseding 6059. ethereum/EIPs#7806](https://github.com/ethereum/EIPs/pull/7806)

**Pooja Ranjan** [0:51](https://www.youtube.com/watch?v=mutOWZV2uOw&t=51s): The first PR which is 7806 was recommended by Panda to be discussed here. This is about updating EIP 6059. The pull request number is 7806. Panda if you would like to or maybe provide a brief background about this PR. 

**Gavin J** [1:16](https://www.youtube.com/watch?v=mutOWZV2uOw&t=76s): Yeah when I tried to meet myself I crashed, so that was unfortunate. I'm not sure whether now I think about it whether or not that was due to me pressing the commute button or switching to our Wi-Fi. If it's the Wi-Fi, I might actually crash again but in the meantime one is because we don't actually have a process for indicating stuff that's superseded and I just want to double check that we continue to not actually no that no editor actually wants to pursue superseded as an actual thing that people can do.

**Lightclient** [2:04](https://www.youtube.com/watch?v=mutOWZV2uOw&t=124s): Yeah I think it was a bit complicated on how to actually deal with superseding because we used to have it and the question arose like if an EIP by a different author comes in and says I'm superseding this EIP. That kind of is conveying that from the point of standardisation. This is  the next thing when the other author may not agree. So we just kind of removed that totally.

**Gavin J** [2:32](https://www.youtube.com/watch?v=mutOWZV2uOw&t=152s): So we should then just probably close that Beyond. 

**Pooja Ranjan** [2:41](https://www.youtube.com/watch?v=mutOWZV2uOw&t=161s): Yeah I think in the past there was also a discussion about the erc223 which was according to the order should be superseding erc20 and this was the similar decision at the time as well.

**Gavin J** [2:58](https://www.youtube.com/watch?v=mutOWZV2uOw&t=178s): Well that's a bit different because the office.

**Pooja Ranjan** [3:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=181s): Yeah yeah that's right yeah but superseding in general I don't think it has been a precedent here. I mean definitely it was in the past.

**Gavin J** [3:09](https://www.youtube.com/watch?v=mutOWZV2uOw&t=189s): There is a president actually in the year 19 and 20. Oh I'm just thinking that the recent questions. I'm wondering if we might want to allow it. Maybe adding a comment and perhaps a security concern. If for example a new I EIP allows for fixing of the security issue and it's otherwise pretty similar in content to the old one. I'm not sure if that's the case here but thoughts anyone?

**Lightclient** [4:05](https://www.youtube.com/watch?v=mutOWZV2uOw&t=245s): I didn't catch the last thing you mentioned. 

**Gavin J** [4:08](https://www.youtube.com/watch?v=mutOWZV2uOw&t=248s): Ah! well I'm just wondering maybe if it might make sense to allow for updating of this your security consideration section, if there is any IP that is otherwise pretty similar in content to the old one but also fixes the security issue.

**Lightclient** [4:31](https://www.youtube.com/watch?v=mutOWZV2uOw&t=271s): Are you saying if it's final?
**Gavin J** [4:35](https://www.youtube.com/watch?v=mutOWZV2uOw&t=275s):  Yes but only the Securities consideration section no other section not the front matter.

**Lightclient** [4:43](https://www.youtube.com/watch?v=mutOWZV2uOw&t=283s): Yeah I think that would generally be reasonable. I also wonder if it should be possible for an author to withdraw a final EIP or have a different status for something that was final but deprecated by the author.

**Gavin J** [4:58](https://www.youtube.com/watch?v=mutOWZV2uOw&t=298s): Maybe final hyphen withdrawn could be a status.

**Lightclient** [5:06](https://www.youtube.com/watch?v=mutOWZV2uOw&t=306s):  Your mic is really low Victor.

**Gavin J** [5:11](https://www.youtube.com/watch?v=mutOWZV2uOw&t=311s): Victor or me?  

**Lightclient** [5:13](https://www.youtube.com/watch?v=mutOWZV2uOw&t=313s): Victor's bike is very quiet.

**Zainan Victor Zhou** [5:16](https://www.youtube.com/watch?v=mutOWZV2uOw&t=245s): Microphone is broken so I think  final Dash deprecated with final Dash superseded by would be something good to consider at least in the context of erc's. We can borrow the wisdom in eip where they allow. They specifically have a place where the author can say hey this one is superseded. You should use the other one and we even use I think RFC 8190 that was superseded by that that is superseding the 2197. Must ensure it was updated before so at least in the ERC context this makes sense. The problem is the difficulty of governance so who gets to decide which one is superseding which one and does the author get credit in the next one as well.

**Gavin J** [6:13](https://www.youtube.com/watch?v=mutOWZV2uOw&t=373s): For some reason I think no the author does not get credit because of the way cc0 should work in terms of actually superseding. I think again the final hyphen with Ron thing would be better but also allowing for a superseded front entry which indicates a list of erps that the author considers to supersede the current one.

**Lightclient** [6:48](https://www.youtube.com/watch?v=mutOWZV2uOw&t=408s): Yeah none of these sound perfect. We might have to spend some time and think a bit more about it. I mean we don't want the situation where something is final and widely used then the author decides they want to go Rogue and quote, unquote withdraw it.

**Gavin J** [7:05](https://www.youtube.com/watch?v=mutOWZV2uOw&t=425s):  Yeah I think probably the best thing would be some phrasing along the lines of the author considers a EIP at eip y and eip z. You have superseded this EIP or something like that.

**Zainan Victor Zhou** [7:31](https://www.youtube.com/watch?v=mutOWZV2uOw&t=451s): Yeah in context with what Matt says one example is the rc20 has widely been used and the lack of ability to check who they sent to is being attempt, is being addressed to erc 223 and 1363 and also the the author himself has in different occasions says that needs to be superseded or it needs to be deprecated  things like that is an example for motivation like this.

**Gavin J** [8:09](https://www.youtube.com/watch?v=mutOWZV2uOw&t=489s): So yeah in that situation I think that we should again I think the correct thing to do is defer to the authors and again use the phrasing the authors consider these eips to have superseded. This current EIP and maybe we could also add lines along some lines. This may or may not reflect Community opinion.

**Pooja Ranjan** [8:40](https://www.youtube.com/watch?v=mutOWZV2uOw&t=520s): In my mind like having a superseded thing over there is kind of deciding a winner or suggesting to the community what is the best thing, best proposal or best standard available here to be adopted. But if we go by the handbook that is recently updated  5069 I'm talking about. I think the recommendations here are for editors. We do not decide winners. We are just like editors are just making Corrections on the proposal. They are just making sure that proposal is right and it is up to an individual and implementer or adapt developer to pick what is the best suited for them.

**Gavin J** [9:20](https://www.youtube.com/watch?v=mutOWZV2uOw&t=373s): We wouldn't be deciding winners. The author of the previous eips could decide that they would prefer if a different EIP was used instead and that would be literally kind of what it would indicate. Not that some eips are better than in others but it in the subjective view of the original happiest authors certainly IPS should be used instead. 

**Pooja Ranjan** [9:47](https://www.youtube.com/watch?v=mutOWZV2uOw&t=587s): I'm imagining this may lead to add an additional field to Preamble and if that is an additional perhaps optional may lead to some of the confusion but yeah I'm totally open to the idea whatever group designs.

**Gavin J** [10:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=601s):  Is there anyone particularly opposed to that idea? I'm gonna go with that as being no.

**Pooja Ranjan** [10:22](https://www.youtube.com/watch?v=mutOWZV2uOw&t=622s): Right, so just to understand it correctly, are we hoping to have a preamble field added as superseded and we would enter an EIP number over there. If that is a proposal we can perhaps add it to the next meeting as well. Just for other ideas to join though I know Sam is not here so we could collect some feedback from there as well and have a decision in the next or following. 

**Gavin J** [10:53](https://www.youtube.com/watch?v=mutOWZV2uOw&t=653s): Yes I can wrap that PR and it would probably be a field that says superseded by but also the way it would actually be displayed is not as superseded heightened by Erp numbers. It would be a very clear indication that this is not the editor it's deciding this is of an opinion of the original eip's authors that a certain one should be instead.

**Pooja Ranjan** [11:21](https://www.youtube.com/watch?v=mutOWZV2uOw&t=681s): Sounds good.

**Justin Floretine** [11:23](https://www.youtube.com/watch?v=mutOWZV2uOw&t=683s): So yeah real quick so if you treat it as a deprecation problem you can leave the endorsement of what it should be replaced by as an optional. So if your concern is you want to make sure that people can you know disavow old things but you're worried that they might have to implicitly endorse the new thing you can make that optional.

**Gavin J** [11:48](https://www.youtube.com/watch?v=mutOWZV2uOw&t=708s): That seems like something that definitely should be possible. 

**Justin Floretine** [11:54](https://www.youtube.com/watch?v=mutOWZV2uOw&t=714s): There's you know right it's also kind of a jerk move to deprecate something and not give somebody a good way to replace it. But you know there can be valid reasons for doing that sometimes.

**Gavin J** [12:05](https://www.youtube.com/watch?v=mutOWZV2uOw&t=725s):  Yeah maybe a superseded hyphen pulse.

**Justin Floretine** [12:09](https://www.youtube.com/watch?v=mutOWZV2uOw&t=729s): I mean I would just set the status from final to deprecated and in the Preamble. Put if you have.if the deprecations have an opinion that it should be dedicated by something else updated there. 

**Gavin J** [12:25](https://www.youtube.com/watch?v=mutOWZV2uOw&t=745s): It would still remain a final status. Again nothing about the EIP would change from basically should nothing about VIP should change except for that opinion being displayed.

**Justin Floretine** [12:41](https://www.youtube.com/watch?v=mutOWZV2uOw&t=761s):  Okay then it's just a matter of phrasing them.

**Gavin J** [12:46](https://www.youtube.com/watch?v=mutOWZV2uOw&t=766s): Correct I think we can move on to the next agenda item. 

**Pooja Ranjan** [12:56](https://www.youtube.com/watch?v=mutOWZV2uOw&t=776s): That is correct so just to get the Summary here about this particular pr7806 are we going to keep it or we are just closing it.

**Gavin J** [13:06](https://www.youtube.com/watch?v=mutOWZV2uOw&t=786s): Let's keep it for the time being. We are kicking that can down the road.

[Update EIP-1559: Clarify who pays gas fees ethereum/EIPs#7423](https://github.com/ethereum/EIPs/pull/7423)

**Pooja Ranjan** [13:18](https://www.youtube.com/watch?v=mutOWZV2uOw&t=798s): Right all right moving on to the next one, we have another proposal: a PR for a final EIP number is 1559 and the pull request number is 7423. I think this has been sitting for quite some time. I wonder if any editor has any thoughts on this pull request.

**Gavin J** [13:39](https://www.youtube.com/watch?v=mutOWZV2uOw&t=819s):  Page from the link in the chat.

**Pooja Ranjan** [13:50](https://www.youtube.com/watch?v=mutOWZV2uOw&t=830s): Yeah I just shared. So this proposal is to clarify who pays the gas fees here.

**Lightclient** [14:18](https://www.youtube.com/watch?v=mutOWZV2uOw&t=858s): Yeah I mean it seems fine.

**Pooja Ranjan** [14:24](https://www.youtube.com/watch?v=mutOWZV2uOw&t=864s): And I see it has already been approved by pandas in the month of July as well. So, perhaps it can be merged with what it requires.

**Gavin J** [14:36](https://www.youtube.com/watch?v=mutOWZV2uOw&t=876s): It looks like it's been approved by Panda. well me why did I refer to myself in the third person that was weird and like mine. So I think we only need one more reviewer anyway.

**Pooja Ranjan** [14:52](https://www.youtube.com/watch?v=mutOWZV2uOw&t=892s): Pending reviewer just suggested eip bot. 

**Lightclient** [14:55](https://www.youtube.com/watch?v=mutOWZV2uOw&t=895s): I mean, is it going to merge with all the linting errors?

**Gavin J** [15:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=901s): No it won't need to be manually merged. right?

**Pooja Ranjan** [15:10](https://www.youtube.com/watch?v=mutOWZV2uOw&t=910s): Okay yeah can anyone maybe leave some comments.

**Gavin J** [15:15](https://www.youtube.com/watch?v=mutOWZV2uOw&t=915s):  Victor do you approve?

**Pooja Ranjan** [15:22](https://www.youtube.com/watch?v=mutOWZV2uOw&t=922s): I think Gajindra Singh just approved.

**Gavin J** [15:28](https://www.youtube.com/watch?v=mutOWZV2uOw&t=928s): okay I'll add it to the merge View

## Manual Merge

**Pooja Ranjan** [15:30](https://www.youtube.com/watch?v=mutOWZV2uOw&t=930s): Perfect moving on to the next section that is a list of some manual merges. I believe it was discussed in an earlier meeting and perhaps none of the edited objects for it and it is queued for manual merge; the pull request number is 7505 and 7506. If someone here may be able to merge it.
**Gavin J** [16:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=961s): I believe client has manual merge permissions or is that access.

**Pooja Ranjan** [16:12](https://www.youtube.com/watch?v=mutOWZV2uOw&t=972s): I'm hoping it must be Sam on Light Client but Sam is the author here when it matters you can maybe take a look and be able to merge it.

**Gavin J** [16:23](https://www.youtube.com/watch?v=mutOWZV2uOw&t=983s): If it is Arctic that has override permissions can we actually remove actic for the override permissions and transfer those to plan because Lightclient is a lot more active.

**Lightclient** [16:43](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1003s):  I can manually merge.

**Gavin J** [16:47](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1007s): Okay feel free to do that for those two PRS and also for the PRs. We were just talking.

**Pooja Ranjan** [16:55](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1015s): Yeah I think that 7423 is now merged and yeah whenever you get a chance please merge for 7505 and 7506.

# 2. Discussion continued or updates from past meetings

## [Update EIP-721: Add ERC links ethereum/EIPs#7550](https://github.com/ethereum/EIPs/pull/7550) 

**Pooja Ranjan** [17:07](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1027s): Moving on to discussions continued from the past meeting. We have another pull request to update eip721 which is a funnel EIP but the pull request is also coming up from the original author and we discussed in the last meeting no one objected. I wondered if this can be manually merged as well the pull request number is 7550.

**Gavin J** [17:44](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1064s): So I do approve of this one. It maybe changes a tiny bit too much but I also don't but I also don't mind that because in general this is more compliant than it used to be.

**Pooja Ranjan** [18:05](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1085s): Sounds good.

**Gavin J** [18:07](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1087s): Specifically it changes almost all instances of references to other VIPs and things and it doesn't need to do that but honestly that just by chilling.

**Lightclient** [18:23](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1103s): Yeah I want to look at this a bit. This description is pretty.

**Gavin J** [18:28](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1108s):  It's requested to be copied directly from the simple summary it used to be.

**Lightclient** [18:38](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1118s): Oh is it? Okay I've never heard someone call it a deed.

**Gavin J** [18:44](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1124s): That it is not for the sense wording.

**Lightclient** [18:48](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1128s): Yeah in that case I'll take a look at it and we'll see if we can merge it.

# Call for Input

**Pooja Ranjan** [18:55](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1135s): Awesome all right. Let's move on to the next item listed here that is call for input as we know with the new process we are trying to have decisions collected over issues created and it is for EIP editors to respond within one month's period.

##  Issues 263-270 & 272-273: Due on Oct 6th

**Pooja Ranjan** [19:19](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1159s): Issue 263-270 seven issues here plus 272 and 273 all of them are due on October 5th which is a day after today, so I have not included the decision hoping that we should give another 24 hours for those editors who may not have gotten the opportunity to respond to it or may have missed it want to add it in the last minute that includes a bunch of proposals including editors active status which editor could be removed. They have listed all the editors if this is good to be removed or not and then there is one other very important input needed for the keeper of consensus election. so I would recommend all EIP editors here or maybe listening to the call after this please take a look at all the open issues and respond to the issues then add your input and perhaps we can discuss the result in the next meeting but in the meantime if people would like to discuss any particular issues. We can happily wait as well but yeah please go ahead and let us know if anyone has any particular thing that they would like to discuss.

**Gavin J** [20:41](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1241s): I see like client just commented on the backseat editor removal would we be willing to kind of. is there a system in place for a light temporarily removing an editor for a short like one month period of time and then they got get automatically re-added because I think that because I think none of us here actually one and gone because we think that distributions wouldn't be useful I think we want him basically not to block any of this stuff.

**Pooja Ranjan** [21:26](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1286s): Not sure if blocking is a concern.

**Gavin J** [21:32](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1292s): Because of the way that the current Charter is set up basically every editor needs to have voted in order to for it to pass before 30 days and currently we're trying to get stuff passed before the 30-day Mark which is currently not happening because axic has not been reviewing the call for inputs.
**Gajinder** [22:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1321s): I agree all basically all the feedback from the editors at least the first feedback from editors should at least happen in the first week of the issue itself. I mean usually but if it doesn't happen for a month long time. It's not really you know a good thing, It's a waste of time to wait and just to see that. Okay  that response is never going to come and we'll anyway uh go with the decision without that particular editor's feedback.

**Gavin J** [22:34](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1354s): So the way the cut Charter currently works is that basically there is. Well first of all I'm not sure we can actually get. I'm not sure we actually have enough boats to elect. Anyone as kind of the first keeper of consensus without that sick voting additionally.

**LightClient** [23:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1381s): I think after 30 days, we looked to see how many people voted for you.

**Gavin J** [23:08](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1388s): Has it actually been 30 days until 30 days shall we for  time being consider Samos a very temporary keeper of consensus.

**Pooja Ranjan** [23:36](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1416s): Is there any specific decision item that we are waiting for? I mean like I know Sam is on vacation till 17th of this month. 

**Gavin J** [23:45](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1425s):  The specific item is a kind of call for input editor removal exit on the EIPIP. GitHub issue number 266 and by the way I do approve. Again I have been advocating for this kind of a reduced requirement editor thing where by default kind of you are considered to have abstained in your vote until you actually vote.So basically for the purposes of Forum you don't need to vote but your vote still counts if you didn't vote.

**Gajinder** [24:51](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1491s): I actually like the current way the charter is set up so that you know everyone has to give some sort of a review. Even if it's too abstaining. Basically I think the point that we want to make over the hair is that there needs to be a responsiveness to the issues that are being raised and that's why this particular issue exists. There is no response from the executive and if he can participate actively then definitely we all also have expressed that we can sort of reinstate the editorship.

**Gavin J** [25:29](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1135s):  The problem is that I think we all kind of want access to be able to participate wherever we can but we also recognize that right at the moment he's not able to participate in everything. His input would be valuable for a lot of these things but we also should be able to pass things without his input for the time being.How do you correctly pronounce that I  guess I haven't figured that out yet. Can anyone help me with this?

**Pooja Ranjan** [26:08](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1568s): Yeah that's how we refer to him as his full name is Alex barig zazi.

**Gavin J** [26:15](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1575s): I'll just say Alex and yeah I think we all want Alex to be able to participate uninterrupted but I think we also don't want him to interrupt us.

**Gajinder** [26:31](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1591s):  Maybe we have a negative status where basically we say these ideas. 

**gavin J** [26:37](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1597s): But what I was proposing having an intermediate status where for example if say you're on vacation that would be something, that would be useful like hey I'm gonna be on vacation. I might not being able to keep on top of everything but if there's something that catches my attention. I would still like to review it or something like that is something I would like or even more more permanently as currently you haven't been kind of on top of everything. But also we still think that your contributions when you've contributed have been valuable, kind of something that client you're the other kind of governing editor on this. what do you think?

**LightClient** [27:31](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1651s): I'm not sure if I have a good side of how to deal with this. Alex has put a lot of time into the EIPs setting it up to be where they are today and I know that he hasn't been as active for the past year or so but I want to find a way for him to continue contributing as long as he's going to as long as he's Desiring.

**Gavin J** [27:55](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1675s): Yes and it's pretty clear that he does desire to continue to contribute so do you think of that kind of
almost vacation mode thing as a good compromise for the meantime.

**Lightclient** [28:21](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1701s): I also don't really want to make these processes more complicated and add different types of statuses for people. So I kind of feel like we should see to it.

**Gavin J** [28:31](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1711s): That end I would agree. However something I will note is actually I think we can do this without actually requiring a consensus vote because of kind of the ability for us to kind of delegate
Stuff. So I think that all access should need to do is just say hey I delegate my votes too. So whenever a new call for input given is received I automatically vote. I'm saying until my vote has changed no consensus required.

**Gajinder** [29:18](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1758s): 
yeah I think it should be easy enough in the sense that I can just say that I don't want a sabbatical and that's basically that's it I mentioned from this time period to this time period.

**Gavin J** [29:32](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1772s): Light client, do you agree that it should be possible within the current framework.

**Lightclient** [29:42](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1782s): Yeah I think either saying I am going to be away for this period of time or I delegate my votes to the specific person either of those would be acceptable. I'd rather not change the actual Charter
description to support it explicitly but I think implicitly this is something that we can accept.

**Gavin J** [30:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1801s): Okay that's good. I will therefore change my vote on the call for embed foreign.

**Pooja Ranjan** [30:21](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1821s): I'm trying to find out I don't think I see Victor spot here for exec because the process suggests that it has to be unanimous minus the editor being removed.

**Zainan Victor Zhou** [30:37](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1837s): Yeah I have seen a very valuable Community member and editor and he was very good at authoring and reviewing. so skillswise, experience wise. I look up to him and he likes him to stay um but the current status is that he is not being active enough. So I think it's more about the intention. I think my view is similar to what Matt says. As long as he wants to continue contributing. I'll be voting to keep him. If he doesn't have enough intention to stay or if we cannot continue to provide a good environment to motivate him to stay, I think we need to think about what we can change or if he wants to leave this Duty. Yeah but I think it's really up to his own intention and I just want to make sure that we have a good communication with him and understand what his intention is and also he voice out his commitment.

**Pooja Ranjan** [31:51](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1911s): Sounds good. Maybe Panda if you can update your profession on this. oh you did good and a Victor if you can also add. I see your comment now yes Victor you can also maybe add your thoughts over here and the last date on this is October 6th. So I know by that time Sam will not be back but if we have a unanimous decision, we can perhaps mark this as oh you know .

**Gavin j** [32:31](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1951s): so the way the unanimous really works here is, if everyone unanimously votes  it doesn't require unanimous no vote as long as a single person votes no that would be like and also me now. Then it is basically automatically closed. Probably this one's not going to pass as for all the other call for inputs. I'm pretty sure my client you've reviewed all of them but can you just double check you have. I'm also checking myself. Oh lightclientyou haven't actually voted for the first keeper of consensus that action you should do that.

**Pooja Ranjan** [33:38](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2018s): All right maybe we can revisit this in the next meeting to see where we are at conditions

**Gavin J** [33:51](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2031s): Actually there's a few of these copper inputs that, like the client we haven't reviewed yet, would you mind doing those kinds of now. Perhaps during the call like the majority of them are just editor removals that I think most of us would agree are obviously no but had to be open to just like as a formality and there's also the election which is important enough that I think we actually do. Well I mean without you or someone else. We don't actually have enough votes to finalise it so please do that.

**Pooja Ranjan** [34:42](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2082s): I'm like yeah I see you response here in the chat says yes so I am hoping that he would take our time to respond to all the issues here amen respond to call for input added here in the issues.

## Repo split - [EIP-7329](https://eips.ethereum.org/EIPS/eip-7329)

**Pooja Ranjan** [34:57](https://www.youtube.com/watch?v=mutOWZV2uOw&t=1951s): In the essence of time let's move on to the next item which is about a repo split EIP number here is 7329 I suppose in the last meeting the EIPIP meeting editors decided that there would be a meeting to discuss. Matt's earlier pull request and if there are any changes to that I wonder if there is anything that the group would like to share.

**Gavin J** [35:23](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2123s): I propose at the time for the meet one week from today normal eipip time. I guess not everyone's here but there's a well light client and Victor are you available at that time.

**Zainan Victor Zhou** [35:41](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2141s): What time sorry if I didn't scratch that.

**Gavin J** [35:45](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2145s):  One week from today same time as you know as a normal EIPIP being meeting.

**Zainan Victor Zhou** [35:51](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2151s):  one week from today so next week. right?

**Gavin J** [35:53](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2153s): next week 

**Zainan Victor Zhou** [35:56](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2156s): I think, I should be able to make it

**Lightclient** [36:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2161s): It works for me but I think we should probably have Sam there also.

**Gavin J** [36:07](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2167s): Yeah I need to check with everyone 

**Lightclient** [36:09](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2169s): yeah well I just don't think we can pull him from vacation to split the repos laughs.

**Gavin J** [36:20](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2180s): Also speaking of  this is a pretty last minute change as to splitting the repos I have come around to actually I agree with that spilling groupers is a pretty good idea I still think that it's core that differs from most of the other EIP types not ERC. I again still would kind of prefer if it were the Corey EIPs that were split. This is a last minute change and I don't imagine that anyone's gonna approve of it but just throwing it out there. Lightclient and Victor what do you think?

**Zainan Victor Zhou** [37:04](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2224s): I felt that the interface seems to go between to go closer to erc's.  I know that Matt has a preference for interface and network to be deprecated. So far erc’s are all about smart contracts if Network and interface are deprecated. Some of them can go into executions back and consensus back. Some of them seem to be relevant to other things such as the recently finalised 6913. The one that allows multiple wallets providers to be injected into the browser environment. Those things need to have a home and I would like to know what people think at this meeting about what kind of EIP or ERC should go into.

**Gavin J** [38:05](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2285s):  So I think the way it was supposed to be with the interface was kind of everything that was in between smart contracts and applications wanting the inner Space with smart contracts. Well yeah or go interface. Unfortunately what I think it's become then ERC would be every kind of everything that doesn't fit into any other category or go ethereum request for  comments. The problem is that instead, it's been the other way around: ERC has become only smart, only kind of smart contract related stuff and then everything else has now gotten into interface. I think there is not too much distinction between interface and ERC.  Ergo, that was why I tried to.  I did add that thing that moved the inner interface into ERC and some of them into core. I'm still not sure if I think the client did not like any of them going into core. If so that's fine but  at the very we've gotten really off topic here we're talking about this repo split. What I'm suggesting is for now does it make more sense to split erc's and everything that's not pour out into a separate repo or does it make sense to split only ercs and leave core and everything that's not ERC in the repo.

**Gajinder** [40:00](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2400s): I think what we decided was that anything that requires hot program needs to be implemented on protocol level would go into eips and everything else into erc's.

**Gavin J** [40:11](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2411s):  Okay and this is the repositories or the kind of categories.

**Gajinder** [40:21](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2421s): We also decided not to have any categories and deprecate the categories.

**Gavin J** [40:28](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2428s): Okay so that's an idea. Yeah with that in mind I'm actually going to be closing my call for input for removing the networking and interface categories because that seems to be kind of well actually I won't close the call for input. I'm just gonna change the decision to get rid of the networking and interface and then close the original PR because that seems to be effectively what we've decided on already has something to say.

**Zainan Victor Zhou** [41:25](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2485s): Oh  I think I agree with  What Gajider does. I think we simply think like anything that the half Forks require much more senses and anything that doesn't require hard folk is like you do it. If you like
and we'll see how many people.

**Gavin J** [41:48](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2508s): Yeah so I agree with that definition that seems pretty well defined. One minus again it leaves networking up. In this nebulous state where it actually does have if they're networking despite not kind of directly being able to cause hard Forks because again it's not part of the chain. It's just how the nodes talk to one another nonetheless if you again it does have the power to cause chain splits. If I understand correctly, it's kind of like basically like think of if and networking Erp was made that kind of had a like basically made some backwards and compatible change which shouldn't happen because of the way networking governance. Yeah okay yeah I see but like it is to some degree consensus critical. Does anyone disagree with it being consensus critical?

**Danno Ferrin** [43:01](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2581s): So I think we need to look at the model. I mean whether it's consensus critical or not. Because I mean there's absolutely networking changes that can be ignored and still reach consensus and you can get everything wrong and still reach consensus but it's the developer audience that's looking at those is where things differ. So core would be like the core developers working on the core consensus and execution layer clients and erc’s would be like dap developers. There's also um looking at the comment thread and I think based on some of the other things. I've been reading in the community a separate wallets group that would deal with issues like the 6968 or whatever EIP that one about the injection of how you Marshal a wallet from an adapter page. I think the developer audiences are more important than what other lines we draw around it. It's who's going to look at these and decide whether they need to be implemented, whether or not it requires a hard Fork whether or not it causes consensus failures, it's which particular layer in the stack these changes are going into I think is the most important.

**Gavin J** [44:00](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2644s): Network the problem is that networking is its own layer here and doesn't therefore fall into either of the other two 

**Danno Ferrin** [44:10](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2650s): I would like an example of the networking layer that does not address consensus or execution clients.

**Gavin J** [44:17](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2657s): Well I mean I'm pretty sure that for example one of them was just a way to kind of export the validation keys which to be fair that one doesn't actually need to be networking and would be perfectly fine. There's an ERC as I think lightclient pointed out but at the same time to me. It definitely looks like networking the ipus to share more in common with quora eip's process wise than they do with well except maybe they don't kind of what I'm thinking of is that all core devs already encompassed to very distinct groups I see the kind of execution layer groups and the consensus layer groups and I think that probably the networking group would be pretty easily integrated into this system.

**DannoFerrin** [45:19](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2719s): Yeah I think it works well because when I hear networking Dev P2P or P2P lib. I don't think of  Json RPC. So I think about lower level networking that's below everything on the stack. So putting again in ERC none of the RC people care about um you know the particular packet structure of the dev P2P packet or whether it should be deprecated and going to live P2P. So based on that we can probably exclude it from ERC anyway.

**Gavin J** [45:46](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2746s): But we also can't speak on behalf of the core devs here and whether or not.

**Danno Ferrin** [45:52](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2752s): All core Dev, I am speaking on behalf of All core Dev.

**Gavin J** [45:55](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2755s): Oh great perfect so you would be okay with kind of integrating networking people into the core Dev kind of and in that case we will currently transfer the networking eips into the ERC repository but if you ever want them feel free to take them for now.

**Zainan Victor Zhou** [46:22](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2782s): Can I use one example to help being Devil's Advocate with you. So one example is that insper has been used for our sharing  mem pool with each other and actually if people want to propose something different. They could and they should be able to and in fact. I think it would be good for people to have this ability to have competing proposals and some proposals can explore censorship resistance approaches. Maybe even add their own incentives approach um so that is something that could be addressed that maybe or they need to look into it but also aboard your audience the less control needs to be in would be would benefit. This kind of thought exercise. So far if you want to run your own minor, if you want to run your own mind cluster, you can actually just share them in a database. If you want to do so this is significantly different from what needs to be in the consensus layer or in the execution layer. If we use that as a start exercise what would be your thoughts?

**Danno Ferrin** [47:49](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2869s): You might have thought it would be to put it into core because it's mostly the kind of work the core devs do. I think one measure we could use is if it shows up on one of italics road maps it's probably going to be in core and so that would be whisper.

**Zainan Victor Zhou** [48:06](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2886s): I'm not sure if I heard that stake. I mean not  competing to see which one wins. I mean competing to cope with existing even longer. Sorry repeat that I missed it so basically allowing different sharing approaches to co-exist for a much longer time. The long term you can have multiple approach to share your transactions uh can to to share your mem pool

**Danno Ferrin** [48:40](https://www.youtube.com/watch?v=mutOWZV2uOw&t=2928s): So mem pool is absolutely a core Dev consideration. It doesn't have to be involved in a hard Fork. I think for it to be in the core devs, it's not the layer above that the core is. I mean we're talking about sharing transactions that you know immediately sounds right at the core layer of producing the networking consensus. So that's why I don't think that the required hard Fork is necessary. The right standard with it. It's more the core Dev audience that's going to be addressing it because stuff like PDF and eips has also shown up on the Telex roadmap and that is stuff you know when you're interacting with with the transaction pool that the core devs typically concern themselves with.You know are concerned about when they see or not concerned about when they see other developments. They think you know when I say concern, I say take interest in. It's probably a better phrase than concerned about but they would take interest in developments. You know possibly one way to look at it is things that might end up becoming merged into the core protocol even though they're not merged right now is the other sort of thing. I don't think erc20 is going to emerge in the core protocol but again the stuff that you mentioned. You know standardising the way transaction gossip happens long term for storing stuff like proposer builder separation. I think those are right up the lane of the sort of discussions that the core devs as an audience discuss so that's why I feel the separation based on audience is what is most relevant and I see right now probably three audiences. There would be a wallet audience, an adapter audience and a core Dev audience. Most of the faces would move to ERC. Yes I would probably agree with that

**Gavin J** [50:25](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3025s): So can I kind of say for now we are basically when the split happens we are sending networking and core to one Repository and every and ERC and interface to another and also probably  allowing transfer because there's going to be some things that eventually we feel that we probably feel should not be in that Repository.

**Danno Ferrin** [50:51](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3051s):  I think transfers are fine. I think when we get a full topic group. we're working with a group model as well. We'll need to consider that to and possibly consider multiple ownership of a spec where there's a primary owner and you know other interested groups that want to track it as well. I think that's a topic worth discussing too but I think this is an interim step until we get the functional topic group model up. 

**Gavin J** [51:14](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3074s): Okay so for the time being do we think that it should just be do we think that we need both sides to agree the transfer any IP or just decide that once the EIP or Justice or just decide that doesn't want the EIP.

**LightClient** [51:29](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3089s):  I mean what does it mean to transfer an EIP.

**Gavin J** [51:32](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3092s): So obviously we're going to have two repos and it's literally deleting the following one repo and adding it to another.

**Lightclient** [51:39](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3099s):  I mean yeah but it's not so simple like we have links that go to that repo. We have links that go to eips.etherium.org and so every time we want to transfer these we have to set up this redirection and things.

**Gavin J** [51:51](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3111s): So I think that we're probably gonna have to reject the website, so right now we don't actually have a way to redirect. so we're actually going to have to create a new repo basically because you know in the repo split EIP it does say that there should be a new website. However there's a few things that again would need changing before that can become a reality. The first thing is that we need a way for that to be able to happen. We might have a subdomain setup but like none of us actually have the power to set that subdomain.

**Lightclient** [52:28](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3148s): Additionally the sub domain is already set.

**Gavin J** [52:32](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3152s): Yeah but well the the subdomain is set up to be able to like have a Pages site there but also that there needs to be a GitHub Pages site to put there and right now that's there is actually a GitHub Pages site at arcs.theorem.org.

**LightClient** [52:54](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3174s): Yeah it's I think a private repo right now ER ethereum slash erc's. We have control over it. It's really just a matter of putting the correct files in the repo and making sure that the configuration of the website is set for erc's versus eips.

**Gavin J** [53:14](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3194s): Okay I see, so what I think they've currently done is actually just a team named it to EIP. It's not ethereum.org on that basically means that the two sites are currently mirrors of one another so they have it set up kind of in a temporary way for the time being. Can I propose that I basically take out the website code from the eip's repo and stick it in a new one.

**Lightclient** [53:48](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3228s): 
I mean why not just keep it where it is and have this I mean the C name is set to erc's. Right so it's a different website.

**Gavin J** [53:56](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3236s): Because when the repo split happens again, we have to set up all the links to the new site so that things don't like eips.etherium.org EIP slash eip20 don't give a 404 page. So all those redirects will have to be set up well for one thing. If I'm being honest I don't think anyone
in the core Dev team actually knows an FJ call to be able to make those happen. I believe I am currently the resident website expert for this and even then it's going to be a lot of Hassle and is going to require a bunch of configuration files and I'm not actually sure even how I would go about doing that. I mean one thing I would do like that would be extraordinarily temporarians instead of deleting all the EIP files. I would have to go through each of them and stick. yeah I know that I think about it I don't even know how I would do that .

**Lightclient** [54:58](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3298s): I mean that's kind of what the script does on the original PR. It goes through all the erc's updates with text that says this has been moved to this repository.

**Gavin J** [55:08](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3308s):  Oh but it does not automatically redirect and it does not change the canonical URL.

**Lightclient** [55:14](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3314s):  it does not automatically redirect yet

**Gavin J** [55:17](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3317s): Okay so then the website change itself has to be blocked until that is fixed because the canonical URL must be changed at the very least thanks and again. So this is again what I think it might be worth separating out the website from the rest of the kind of the erp's repository because honestly every single other bit of cooling linting the review bot. All of these are outside of the eip's repo because they don't need to be inside the erp's repo. Things don't update to the EIP review but happen after changes to eip1. They follow each other but yeah so ethereum the ethereum.org. So the reason why this is all trickier than it would actually usually be is because of the fact that we're using GitHub Pages. GitHub pages do not support 302 permanent redirects. So you would have to do it. I think the way that you would tell search engines. Hey this page is moved by obtaining the canonical URL and having another meta tag that has an auto refresh of one second to the new URL. But yeah I think we're nearing the end, basically a light client.  can I just confirm that it would be okay for me to try to at least separate out the website.

**Lightclent** [57:04](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3424s): I and yeah I'm pretty against it. I'm happy to review a proposal for doing so but generally it feels like something that I don't think we should do.

**Gavin J** [57:19](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3439s): Okay let's discuss this further on Discord then because we are at 10:01.

**Lightclientr** [57:27](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3447s):  Yeah I have to hope off. Cheers everybody. Thanks for the call Pooja

**GavinJ** [57:33](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3453s): Thank you.

**Pooja Ranjan** [57:36](https://www.youtube.com/watch?v=mutOWZV2uOw&t=3456s): Thank you everyone, hope to see you in two weeks from now. Have a great day

  ---------------------------------------
# Attendees

* Danno Ferrin
* Gavin J
* Pooja Ranjan
* Gajinder
* Light Client
* Joshua
* Zainan Victor Zhou
* Juan Caballero

# Date for Next Meeting: October 11, 2023 at 1400 UTC
