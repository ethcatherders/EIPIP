# EIPIP Meeting 49 Notes

## Meeting Date/Time: Wednesday, Feb 09, 2022, at 15:00 UTC

### Meeting Duration: 40 minutes, 36 seconds

### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/107)

### [Audio/Video of the meeting](https://youtu.be/ATlQApSKDeM)

### Moderator: Pooja Ranjan

### Notes: Shashank

----

## ACTION ITEMS

**ACTION 49.1**:

**ACTION 49.2**:

**ACTION 49.3**:

## AGENDA

**Pooja**: Welcome to EIPIP Meeting 49. I'm going to share agenda here in the chat for people who may have missed it. The first item listed here is about EIP bot, but i don't see any team joining in so far. So we'll come back to that item and because we have Liggy here let's go ahead and pick up his proposal. That is item number 3 resurrect eip-1328. So, we came across this EIP in a PEEPAnEIP meeting, for eip-4361 Sign-In With Ethereum. Though we realize it is not required for ethereum Sign-In proposal but is an important one for other projects. I had a chat with Liggy last week to resurrect this proposal and he had some questions around that the process changed that happened since the proposal was documented. So yeah, over to you Liggy if you have any question and would like to share with the EIP editors.

**Liggy**: Yeah. It was basically about the new items, but we just filled it out with Pedro now. So to just like fulfill this new property. So basically I think we should have filled everything... should have filled all the changes. Yeah. So everything exit was saying was missing and also added for the new 2.0 standard basically there was a little bit of change there. Yeah. Want to work a little bit more on the security considerations there's a little bit missing. I just talked to Peter before because but he couldn't make it to this call. But afterwards we hope it's mergeble. So yeah, because it's used... it's widely used and we kind of want to make it final saw the path to find it so make it draft first and then wait two weeks and then make it final.

**Pooja**: So, going by the earlier comments on this pull request it looks like it is okay. I have added the link to the agenda so if there is anything that is needed from uh editor's point of view please leave a comment just wanted to bring it to attention, that we would like to direct. 

**Liggy**: Yeah. Thank you for that, I hope we can get it alive again.

**Pooja**: All right. Thank you. Moving on the item number 2 here is "What to put in the test cases section". So, this is inspired by Mikhail's comment which is there on the discord ETH R&D Discord. But, I suppose it will be useful for other authors as well... is there a general guideline for adding test cases section? So by general guideline I mean, can it be updated in later statuses? For e.g., eip-3675 that is moving to review. So is it okay to add a test plan or the link to the test plan and when the testing is done, before moving it to last call, that will be updated.

**Micah**: So the test cases section... test cases section is optional and part of the reason for that is so people don't have to make sure have test cases ready at the beginning. So whenever you have test cases ready add them in if you don't have them then just leave the section out entirely.

**Pooja**: So, by optional it means for proposals... I'm sure it will not be the core proposal but any other proposal if they do not have test cases just the reference implementation should be working right there should not be a blocker.

**Micah**: Oh yeah. Reference implementation is also optional so if either the sections are missing the EIP can still go through the full process and we recommend them like it definitely helps to have good test cases and reference implementation but they're not required.

**Pooja**: Cool. All right, that is good to know. We will update the author. I think that was it on this particular item. I see shashank joining the call. So, I suppose we can pick up the item
of the eip-bot, coming back to item number 1, following the working of the bots in the past few months we all know that automation has helped us a lot and I was discussing to some other others
and they mentioned that it has helped us and like moving things faster. Comments on Github and ETH R&D discord shows that there are still room for improvements. We are making progress of course so to continue these improvements I have added this as recurring item for EIPIP meeting. The first sub item is the progress on documenting working of different bots, I know we discussed in past few meetings from Shashank if you may have for that update on this to share.

**Shashank**: Yeah. Yeah. So, I discussed with Alita on our ECH discord and I realized that while I was working on the documentation all the documentation that was actually necessary was already present and any of the rest of the flow that was required to understand as how these bots are working. That specific part is already present in the yaml files in the configuration files and any of the doubts that I had was cleared by Micah in the last meeting... I guess last meeting so I'm failing to understand if we should even continue working on the bot documentation because i don't feel it's necessary anymore. Because major of the confusion that I had was understanding where it's starting and where it's ending but if you just see the documentation and go through the code it's actually pretty much self-explanatory if i can say.

**Pooja**: Good to know. We just wanted to make sure people who are trying to join here or finding ways to contribute as a new contributor should be able to find that now that we are sure that everything is already there and should be easy. It's good to know. We are currently collecting issues on eip-bot github repository. So if there is anything related to eip bot that people find is
not working please add an issue on the eip-bot github. The link is added to the agenda. Related to bot I had couple of... couple of items to be discussed by sub-items actually. There is this tag ambiguous uh I'm wondering like uh what is the logic behind that like uh how do uh bot decide that it needs to go ambiguous and not new or anything else. Are we aware of...?

**Micah**: Yeah. I believe ambiguous is the label it gives when it can't tell what type of eip it is. So uh normally the bot, I think, will label things as like an ERC or an EIP etc. If for some reason the bot... I'm able to figure that out, usually because the header data is incorrect I think that's when it labels it ambiguous and basically this means some editor needs to look at it and give feedback to the user to tell them. What to fix their problem basically.

**Pooja**: So the error is in the header data right? Probably?

**Micah**: I think so. You have an example of one that marks flag ambiguous?

**Pooja**: I think there was one that we came across yesterday that was a new proposal. But we were not able to figure out why bot marked it as ambiguous instead of a new proposal. I'm trying to pull out...

**Micah**: Let me take a look. I can find one.

**Pooja**: Okay. I'll try to point it out!

**Micah**: So my guess is it might have gotten confused because there's two files in this PR. I thought the bot handled that but maybe on new EIPs it struggles with that still. That's my initial guess.

**Pooja**: That makes sense having two file number can create ambiguity there. Oh yeah that makes sense.

**Light**: I thought the issue was there was no eip number in it yet and so it probably just parse the preamble.

**Micah**: No I mean you can... it'll parse the preamble without the eip number I believe wouldn't it? And also...

**Light**: It could. It should be able to that doesn't mean it does though.

**Micah**: Uh yeah. Okay so looking at the bot message it did parse the EIP itself but then it failed to parse the the image. Oh I think I see we're saying. Okay. Yeah. So the image was put into the folder eip-xx not eip-4780 and so the bot is confused what this file is because it's not in a folder that it recognizes. So yeah I like client's right.

**Shashank**: So is it that it's not about the eip itself but the placement of the file, right? Is that it?

**Micah**: Yeah. So if you look at the conversation on eip-4780 and you look at the bot message it has two little sections there one, where it has details about eip-4780.md and the other one about the
asset file and it got the ambiguous classification from the asset file.

**Shashank**: Yeah. Found it.

**Micah**: The resolution it has and you can see that the file name is assets/eip-xx that should be assets/eip-4780

**Shashank**: Yeah and it happened in the auto-merge-bot of fail check.

**Micah**: Yeah so as soon as the user fixes that it should... I think the bot should resolve.

**Pooja**: Yeah the reason why I was stuck to it because my initial thought process was, if a proposal is new we should not be expecting eip number over there. So it should ideally be categorized as
new proposal instead of ambiguous.

**Micah**: So I think at least right now it is classified as a new eip it's just also ambiguous because it has a second file that it doesn't understand. Once the second file is understood then it should be just new.

**Pooja**: That makes sense. So, that's a very good use of labels and I also find the usage of a new label called *editor needs to review*. Yesterday we were discussing how we can like make it easier for eip editors to figure out which new... which proposals or pull request needs review. This is basically for the new reviewers who are trying to join the group and maybe uh help with looking into some of the proposals. Wondering if we have all already set logic for editors need to review or is it being manually added?

**Micah**: I believe it's manual at the moment.

**Shashank**: I think uh so I'm checking on eip-4671 non-tradable token by Omar... and in the bot it shows that this PR requires review from one of light client and basic and that's it. I'm not sure if the label was... the label happened because of that. Is that it or...?

**Sam**: I think that's a little bit different than what we want right? Because that's saying like we need a like permissioned editor to come along and do like a something that requires authentication like merging or something on those lines, which i think what we actually want is more like a label that says 'hey somebody has looked at this' and they have like tagged the bot to say now we're waiting for the author and then the author can reply or push a commit and then it just flips back to like an editor mode.

**Micah**: Yeah. So, that one I added the tag for and I don't know why.

**Pooja**: But that actually helped, Micah. Because I think if this is a tag which is available probably we can look into automation of it and how to make best use of the tag.

**Shashank**: So what would be the case where this tag would exactly go? Like how would you suggest which part does the bot identify says, okay, this is the part that it's not matching the spec, maybe and it needs this label called the editor needs to review.

**Micah**: So I would say it needs... I don't need to review, ideally would show up automatically when the eip is passing all CI and it is a status change or its new EIP. So basically when it's at a state where editor needs to review it and the user has already resolved the CI issues.

**Sam**: And if it doesn't meet those criteria it needs a waiting for author tag I think.

**Micah**: Yeah. Like if we're gonna do about have the bots use labels like this then it would be reasonable to have an inverse tag for awaiting author something.

**Pooja**: So I think here is like in general cases whenever it is like status change or what is passing other ci and other checks there is this label status change that can help editor to know that okay fine this is done. But there is one specific case where editor is not able to identify whether it is up to him or up to the author. For example when a label is added by an editor requires  author's response even if author respond to that a comment that label is not going off and it is not changing to a back to editor needs review. I think this could be a good use case where we can make use of this label.

**Micah**: Yeah having bots do the labels automatically is nice because like you said they will go away when you're done with them whereas a human brain label on thing probably won't remember to remove
it later.

**Shashank**:  Yeah because that takes the pressure off of the eip editors and also authors, right? You can save a lot of time instead of manually tagging each of these Pull Requests.

**Pooja**: Maybe i can create an issue on the eip-bot github. I'll will try to figure out how to make best use of these labels. I mean particularly editor needs review. But, is there anything else Sam and lightclient you would like to add from yesterday's discussion um I get one point where the author is unable to remove the tag of author has already reviewed it and would be good to have  editor's response tag over there.

**Sam**: No, I don't have anything else to add there.

**Pooja**: All right maybe we can start with that um we'll see if we can try... if we can automate that response and maybe make use of this tag. Okay, that's on the eip-bot. So we already have covered no. 2 and no. 3. No. 4 this topic was added by William. So a few weeks ago we discussed some of the comments left by William in the EIPIP meeting and based on the recommendation he created this pull request to update the readme file. And um I invited him to add today's meeting I don't see him here so probably we can skip the item. But I have added the link to the pull request that he add.. he created for mission statement in readme file looks simple and I suppose it has already been approved by one or two editor there so if there is anything any change is recommended. Feel free to leave a comment and maybe we'll try to bring this item in the next meeting when he is around. Item number 5 is about execution specs so we discussed it in the last meeting and I remember Sam Wilson also talking about on AllCoreDev meeting last friday I'm not sure if there is anything new to add but if not this is just from the last meeting Sam.

**Sam**: Sorry I missed it.

**Pooja**: I have added it since the last meeting we discussed about it and i know that you have already shared update in the ACD meeting last friday so just wondering if there is
anything new to add if not we can move on.

**Sam**: oh no no no no no.

**Sam**: Alright. Not a problem yeah please.

**Micah**: It would be nice if uh the execution spec people i.e Sam and Peter I think and the EIP editor people could come to the table and come to some sort of agreement on what we think the future of
EIPs is I think if we can present a united front to the Core Devs we'll go a lot smoother than if uh the execution spec people and the eip people are bickering, while also trying to get feedback from those.

**Sam**: I definitely agree with you there.

**Micah**: I don't know when the right time for that is but um when I would say before you want to start to bring up with the core devs a change in process we should probably have one or more discussions.

**Sam**: Oh for sure. Yeah I'd like to have like the actual process documented before like actually in like a text file before we uh bring it up.

**Micah**: Yeah. I just want to make sure that we don't like jump the gun and core dev starts giving input um which is going to be a uh a lot of bike shedding I suspect this would be nice if we had you know this is the bike shed you're gonna get this is the color it's gonna be deal with it.

**Sam**: Is there anything that uh you know we don't agree on so far from the vague presentations I've given?

**Micah**: I think the only thing that I don't agree on is keeping the EIP process as it is like I would rather see things move more to something new like I feel like this is a good opportunity to break from the old particularly for core EIPs for ERC or whatever we can be separate but I think this is a excellent opportunity to break away core EIPs into their own new thing that is separate from everything else.

**Sam**: Yeah i think i think we do agree on that. I'd still like to keep them into all the EIPs though.

**Micah**: I mean you could probably convince me on that. I weakly want to get rid of the name just because the name brings with it history and I'd rather not bring the history but um that's not something that I will not heal out without die on. And I'll die in a lot of hills.

**Shashank**: Michah could you give an example as to how these core EIPs can be broken further?

**Micah**: You mean how can we move them out into the execution spec stuff?

**Shashank**: Yeah. Just an example

**Micah**: Like in my perfect world of rainbows unicorns that will never exist. We would have as people are doing pull requests for the execution spec we would document in there um somewhere the like the human readable version of the change control process it would not be over in the EIPs repository it would not be a separate document it would be somehow integrated with execution specs um
and and or the pull requests to them. So, that way when you're looking at a diff you can see the human readable version along with the diff in some way.

**Sam**: So, I think the only um concern with that is it would be very... so, we can do um a diff per hard fork fairly easily. Well, I mean it's not fairly easy but that is the path we're going down but if we want to maintain a diff per EIP. That would probably be a lot more work.

**Micah**: So, I do not feel a strong need to keep a diff per eip but I suspect there will be people who demand that. And so having... in particular I think people want the ability to point at a change set and give it a name slash number slash identifier of some kind and I think that's gonna be the hardest thing to fulfill.

**Sam**: Yeah. I mean so that's pretty easy when you have um like during the development process for an EIP but once it become like once we're done and we're moved on to the next hard fork um every change set that we want is we like has to be maintained. So like right as a good example of this yeah so um as a good example this eliminating the account nonce to 2 to the power 64. Like that chain like for every diff that we maintain we have to backport that change to it. So if we have more like if we track each eip separately then we have to back port every like kind of refactoring every uh soft fork yeah and it gets really tedious.

**Micah**: Yeah. So, I'm with you um and this is part of why I think that we should all agree before we go to the core devs um so that way there's a better chance we can fight for these things that are kind of bigger and are going to be more contentious, such as dropping the permanency of unique identifiers for changes.

**Sam**: I think we can still have those it's just like the active hard fork you'll be able to get a diff per eip and then for past hard forks you'll only get like a rolled up diff for all the EIPs and that hard fork and I think that's probably the best we can do.

**Micah**: And that rolled up diff would also like wherever we're storing the human readable version of these changes um that would also be rolled up with hard forks.

**Sam**: Yeah exactly yeah you'd get all the motivation here's all the everything yeah.

**Micah**: Right. Yes I think that that's the one piece that I suspect we're gonna get some pushback on I like it and I'm with you on it. I just suspect there will be people that strongly want to have like the ability to link to you know eip-1559 or whatever and have that be a kind of permanent link that lives forever and is isolated to just that change not all other changes in the same hard fork. I agree with you I don't want that like because I think that it's gonna be complicated things too much. But I do think there are going to be people that are going to lobby for that pretty hard.

**Sam**: I mean it's unfortunate for them but it's impossible so you can answer.

**Micah**: That's nice you can't have it.

**Sam**: Yep. I mean if they want to you know give me 12 developers full-time that literally go through and you know my newly changed diffs sure. But I don't like me and my three volunteers can't do that.

**Micah**: Right. Yeah okay and uh i think we're on the same page then.

**Sam**: Okay good I have to hop off to my sink call so I will talk to you all soon.

**Pooja**: Thank you for joining Sam. Well that was the idea I  totally agree to uh Micah and Sam uh we wanted to have this process well explained here in these calls and when we have something real solid we can go back to the ACD meeting presented so people be on board and that would be the time of getting feedback from them if there are some small changes requested. I talked to one of the cat herders who is trying to contribute on the execution spec right now. He is also trying to kind of put something together maybe in form of document or representation with the help of Sam and Peter and we hope to see some updates coming soon on this front. Okay, anything else? All right moving to the next item it is eip insight for the month of february. In february we have received two new drafts eip-4750, eip-4527. eip-4750 is EOF function and eip-4527 is QR data transmission protocol for the offline wallet. There is this one proposal which is in the last call eip-2098. So, this proposal uh eip-2098 it is compact signature representation it's an informational type proposal uh we had a chat with the author for PEEPAnEIP for this particular proposal. And it appeared to us like this proposal should not be informational but it can be an ERC and both the co-authors um Richard Moore and Nick Johnson are in agreement that it should be moved to the ERC category. I wanted to bring it to this this discussion today because the last call period is ending on February 13th and if we have to make any changes it has to be done like sooner rather than later so any thought from any editor here.

**Micah**: Sorry which number you say?

**Pooja**: eip-2098. It's seems like an ERC but presently listed as informational EIP.

**Micah**: That can go either way. I generally don't like your uh informationals at all like I like them just not exist so I have a weak preference for ERC on this one.

**Pooja**: Yeah because this is like in the last call and is almost ready to final uh we thought that we should discuss it with EIP editors because authors are in agreement and we hope to see a pull
request soon requesting for a type change.

**Micah**: Yeah. I think I would accept I mean I don't handle erc's or informational so it'll be up to Matt (lightclient) and Alex ultimately but I don't see a problem with it.

**Pooja**: Sounds good. Unfortunately, uh Matt has to go. So he is not in the call but we'll bring it up later on with him maybe when the pull request is available and uh for other proposals um this month... okay there is one more thing that I might want to check with you Micah you may be able to help me here it is eip-663. So, in the EIP inside I'm going to share the link right here um
what happened like exec created this pull request to maybe update it something went wrong and then it was reverted and then new pull request was created. So I'm wondering like first of all like why did it happen uh in the first place because exec is both author and the editor it should be fine. And um if you have any insight on this particular issue.

**Micah**: So, I'm not familiar with the issue referring to but an editor should not be able to merge their own EIPs. They should be requires a second editor to review them so like Alex is an author
he needs me or Matt or Greg to merge.

**Pooja**: Yeah. I just have shared the pull request. eip-4752 is the one when it was resurrected I believe and the other one was again... let me get it for you. eip-4749 it is. So I didn't understand the reason why it is there but um both showed them as much and now there is this new pull request. So, I was wondering like why do we need to have a new pull request and why is it not getting auto merge I'm also sharing the...

**Micah**: So the 1st one eip-4749 was Alex submitted full request to change the status from stagnant to draft because he's the the author it should be waiting for an approval from an editor before it emerges but it appears that... it looks like Alita said she... oh okay so it looks like it was a bug in the bot and Alita has a bot a ticket open to get it fixed I guess.

**Pooja**: Yeah I think I got the problem right now I mean like as you mentioned that because it was uh because exec was author and he was trying to resurrect the proposal that's maybe the reason
it is waiting because I was wondering like the new pull request number 4754, why is it still waiting. I got it. Thank you so much. Yeah I think that's all on the eip insight I have added a new dashboard this month uh that is for the proposals uh that are added as draft versus proposals that actually moves to final um it will be interesting to see it like very few proposals are getting to final status in comparison to proposals which are added as draft, which is normal of course, but yeah I'm excited to uh look into these numbers. That's about EIP insight and EIP editor apprenticeship meeting is the next item we had this meeting yesterday I have added the recording and summary for people to refer to um it is again the simple process where uh EIP edit is explained
to the new people new contributors who want to be reviewers. So it would be it would be a good learning although we had some hiccups yesterday, internet was broken, but yeah people can go back
and refer to the next meeting is planned in two weeks from yesterday. The last item for today's meeting is review action item from the previous meeting. I have added a link here I suppose and
action items were checked to make sure the greeter bot gets activated only for issues section not for the pull request. I haven't seen any new comment from greeter-bot by any chance anyone else has observed. Maybe we can revisit it and look into it. I am hoping that this issue has been resolved anyone with suggestion about the merger bot should reach out to the eip editors or the Cat Herders Team. I haven't received any new requests but this is still open if anyone has an interest or capabilities to look into the merger bot please reach us. 48.3 includes furious dragon update in every alternate meeting. We did talk a little bit about the execution specs today we hope to see more updates in upcoming meetings. That concludes the item those are listed here. But there is one thing that I wanted to maybe bring up today. I see there are three new issues created for three respective eips. I suppose this would be a good time if we can ask the author to move to the FEM portal for having a  discussion to link. Micah I remember there was some concern in the last meeting about the updating window that was allowed for updating at  fellowship of ethereum magician.

**Micah**: Yep. Has it been resolved?

**Pooja**: I'm not that I'm aware of I will check with the team uh but I mean I know that this is uh from like a free software that was mentioned by  Greg in one of the meeting earlier so I will check with the team if this is still the case or people can update it but if there is some something like someone is looking for some immediate help we can probably get it updated from back-end.

**Micah**: Yeah it's the the one thing that I'm waiting for before I really start pushing hard on people to move over is that because Greg did bring up a good point that if you can't repeatedly edit indefinitely your original post then it doesn't serve as a complete replacement for github issues
so as long as we are unable to edit marginal posts I think that we will have a hard time asserting to people that they need to move.

**Pooja**: That make total sense. I don't know Liggy are you part of that team uh the fellowship of ethereum magician sorry to put you on the spot I'm just wondering like who would be the best person to reach I know uh Annet and maybe Jimmy but anyone else who are aware of the process behind the scene for fellowship of a ethereum magician. They seem to be stepped away from the microphone maybe for a while but I'll check with the team and we'll try to have some update by the next meeting. And yes one item that I already have shared in the discord channel that now the eipv the eip validator that has been moved to ethereum github repository. So, that's one good thing that we achieved in a while and that also concludes the item listed here anyone else has anything to bring up?

**Micah**: We should probably discuss not many more people in the call but we should probably discuss making Sam and or who is it? Will? tried
quite a bit of editing lately.

**Pooja**: That's right yep uh yeah I did chat with the light client on this in one of the meetings maybe earlier I don't remember when and we agreed on your suggestion when you recommended that people who feel like being an editor uh should come forward and say that they have been continuously making contribution as you mentioned that we don't have most of the people around do you want me to add it in the next meeting as agenda
item we can probably have a discussion on this.

**Micah**: Sure

**Pooja**: All right yeah that's a very good point. Now that William and Sam Wilson are there we can probably have them write accesses and it will be helpful to make things moving faster. Okay and um there is one last issue that I can find it on the EIP github that is related to proposal 4337. I don't know if anyone looked into it or not the number is 4783. Maybe, any editor can look into it and leave some comment these are just some uh typos changes, must, should not but I'm understanding if they are under a special bracket there should be a reason behind it.

**Micah**: Let's see which one?

**Pooja**: 4783. Pull Request number is 4783. And the changes are suggested for eip-4337.

**Micah**: Oh yeah. This is this is not any PR. This is just an issue so someone can just comment to on the issue and just tell the user please submit a pr.

**Pooja**: Yeah I was just trying to verify here are these like valid corrections or maybe we can tag author here to jump in right?

Micha: Yeah. So when you create when the person creates an EIP to make these changes or sorry when this person creates a PR to make changes the author will automatically be tagged

**Pooja**: Okay. And then the general recommendation would be like maybe we can comment on this issue asking the person to maybe create a pull request to uh such as these changes to the proposal.

Micha: Yeah this still it might be that the user doesn't know how to create a pull request and so you might just need to walk them through the process.

**Pooja**: Okay. We can look into it. All right that sounds good and I think it has concluded everything anything else anyone would like to bring up today? well in that case thank you so much for time and thank you so much for joining. And I'm gonna create the agenda for the next meeting right after this meeting. Please free to add your items that you would like to be discussed in upcoming meetings with the eip editors obviously it will have the regular items. But, it would be good to hear more issues that people would like to be resolved that is related to eip process or any
particular proposal. Thank you everyone for joining us today. Have a good one everyone.