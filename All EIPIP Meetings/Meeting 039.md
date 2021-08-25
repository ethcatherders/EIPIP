# ECH Meeting 39 Notes
## Meeting Date/Time: Wednesday 11 August at 15:00 UTC
### Meeting Duration: 0.5 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/82)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=eo90AIGv3jw&list=PL4cwHXAawZxpLrRIkDlBjDUUrGgF91pQw)
### Moderator: **Pooja/ECH**
### Notes: Jim Bennett

----
## DECISION ITEMS

**DECISION 39.1**: Revisit the topic of version release process and documentation in three weeks [see 2:29](https://youtu.be/CYX0BzZKPH0?t=545)

**DECISION 39.2**: Put the limit account nonce EIP on the next AllCoreDev agenda. [see 15:59](https://youtu.be/CYX0BzZKPH0?t=1070)

**DECISION 39.3**: Document in EIP-1 and in the EIP template not to have authors put the EIP number in the title [see 24:10](https://youtu.be/fKQVb-s0Tzs?t=1959)
----

## AGENDA

## 1. [Network upgrade version release process & documentation](https://www.youtube.com/watch?v=eo90AIGv3jw&list=PL4cwHXAawZxpLrRIkDlBjDUUrGgF91pQw)

**Pooja/ECH**
Welcome to EIPIP meeting 39. I have shared the agenda in chat. And the first item on the agenda is Network upgrade [version release](https://github.com/ethereum/eth1.0-specs/issues/290) process & documentation. So I found this item in the Eth 1.0 specs repository in the Issues section and the issue number is 290. It generally has received positive feedback, and people seem to be in agreement about the version release time. There should be cautionary for network upgrades. Wondering if people would like to discuss this. Is it an agreed-upon process for it? That's number one. And number two is, if there is, where can it be documented or where people can follow along?

**Tim Beiko**  
Yeah, let me just check the issue real quick. So I think we still have some time before we need to actually do this. I suspect the merge is probably the first one we need to figure it out for. And I personally would like to see how the executable spec comes along, before the merge to see if we're gonna have that. Yeah, I don't know. I'm just not sure. It feels a bit early to make a final decision on it. I'm not sure.

**Pooja/ECH**
Yeah, I mean, I was just wondering if there is something already in place, then if you can follow along, or if it is the Eth 1.0 spec repository that people need to keep an eye on?

**Tim Beiko**
Yeah, I think the ETh 1.0 spec is the best place, and in the next few months, there should be some updates on that. But I don't think it is super soon. Yeah, unless anybody else wants to own this, but I suspect I'm probably the one who's gonna have to figure this out.

**Pooja/ECH**  
All right. Maybe we can revisit it after a couple of weeks if there is any progress. My best guess would be it should be README of off Eth 1.0 spec where you can follow and find more information if there is any process in place or if there is any formal agreement. But as Tim mentioned, this is too early for an announcement, so we will come back on this topic after three weeks.

# 2 [EIP/ERC editors (in-training) progress](https://youtu.be/eo90AIGv3jw?t=182)
Moving on, the next item on the agenda is EIP/ERC editors (in-training) progress. So yesterday, William Sharpe, I, and Matt Canard, we had this meeting for an in-training meeting. This was the third one in a row. We went over more than five proposals. And after a few discussions, lightclient added comments on all of them. So we came across a few topics or issues we can say that we would like to bring to the attention of a broader audience. The number one was EIPs marked as Final while there is an open pull request for the proposal. So this issue was identified for two proposals. So both the proposals were Final, and we came across that there was an open pull request, which was mentioned earlier, or we could have addressed. So we were wondering if this can be resolved with the help of a feature addition to the existing bot. For that, my suggestion was if if there is a pull request to change the status to Final, the bot makes a quick check in to all open pull requests to list if there is any other pull request for that particular proposal. And if so, then send a warning message to the editor as well as to the author with the list stating that this cannot be moved to Final because there is an open pull request that needs to be closed before merging this proposal to Final. I'm curious to know, what do people think in general? Is it something worth spending time and effort and getting it done? Or is it something that is very rare, and it should be managed manually by the EIP editor?

**Micah Zoltu**
I mean, it'd be nice if the bot did that check for us, but I don't think it's high priority for me. I think it's a pretty rare situation. When it does come up, it's usually manageable. It's not a big deal. Usually, those last minute pull requests are non-normative changes. And especially for core EIPs, they're usually not normal changes. And so  I would say yes, add it to the To Do list for bot things, but as low priority.

**Pooja/ECH**   
Right. Any other thoughts on this? Unfortunately, I do not see Alita on the call. So I'm not sure if she would be in a position to add any thoughts or how does she find the issue. If not, then we can also open it for people interested to contribute maybe. Alright, so let's consider it, but not a very high priority task. So there was another thing- checks needed for proposal in Last Call. So the concern here was what to do with the review date of a proposal if waiting on the author's response. So at present, EIP 1 describes the Last Call status change, and it states that a proposal needs to be there for 14 days - no specific instruction of what to be done next if there is some complicated situation or something adds up to an abnormal scenario. Say, for example, suppose an author created a pull request to move the status to Last Call and receives a comment from an editor or anyone from the community to address something. And that author is unavailable for the next 13 days or maybe more and then shows up after the Last Call period has passed. So there could be two situations with that one, when a pull request is already merged and we're waiting for those 14 days and this happens in between. And the other situation can be the pull request is still there, and it is not merged, and the author is unavailable for 14 days. So what do people generally think should be the next course of action? I'm asking it from the new editors learning point of view, what should be the normal course of action. And if there is something, should we document it in EIP 1 and add it there.

**Micah Zoltu**  
So the current process is I generally want the Last Call end date to always be two weeks from when it enters Last Call, approximately. And so if an author puts out a PR saying move on with his Last Call, I give them some feedback that I'd like them to address before moving to Last Call. And then they address it. Usually, I'll then say, "Oh, can you also update the Last Call date," or I'll update it for them. Either one. But the idea generally is we want things to sit in the Last Call state for two weeks. And so just ask the author, it usually goes pretty smoothly, I just ask them to update the Last Call date. The times it doesn't go smoothly is when it took a long time to get to Last Call because there's no editors reading. I feel bad for them, because a person puts up a PR to move to Last Call. And then like a week later, someone reviews it and then says, "Oh, can you update the date for another week," and then a week passes again, and it's back and forth. In those situations, I'll usually just update it myself and merge it and apologize for the delay. Again, the goal is two weeks in Last Call. And ideally, any delays to get into Last Call are caused by the author, not the editors.

**Pooja/ECH**  
Yeah. So my question is if it is because of the author and the author's unavailable for some time, even after receiving some comments, he could not make it to come back and respond to it. What would be the next step? Should we keep the original date of the Last Call, or whenever he shows up and does that, it has to be restarted?

**Micah Zoltu**
Are you saying after it's been merged, the Last Call has been in Last Call for two weeks. Okay, so in that situation, I'm fine with just - you know, two weeks, the point of the two weeks is to make sure that, in theory, people are aware of the EIP and have time to submit feedback. Whether the author listens to that feedback or not is entirely up to the author. And so it's on them to do what they want with their feedback. That's not really our place to say you have to listen to feedback. Our place is just to make sure that there's a process in place that gives people an opportunity to provide feedback. So my general feeling is if the author really wants to rush through Last Call and ignore all the feedback they got, it's up to them. Their choice. We just made sure that the process was in place that there was a way to get feedback.

**Pooja/ECH**
That's helpful. That clarifies a lot of confusion. So it is on the author to decide whether to address that or not. Fair enough.

**Micah Zoltu**
Yeah, basically, the one exception I might make, and this has never come up, and I don't think it will come up. But like for core EIPs in particular, if the authors are non-responsive, and the EIP does not match what's actually implemented on mainnet, then I might step in and take a heavier hand. Again, for core EIPs specifically, and only if the EIP did not match mainnet spec, I don't actually know what to do in that situation exactly. I might just create another EIP and say, "Sorry, your EIP's not mainnet because you didn't update it.

**Pooja/ECH**   
Right. And I have actually left messages for authors of some proposals, that are core proposals, but for core proposals, which actually does not require the hard work or the upgrade that would like to undergo, is there any other specific requirement for them to be moved into the Final status If the Last Call period is over?

**Micah Zoltu**
Don't all core EIPs have to be consensus changes? Like, that's the definition of a core EIP?

**Pooja/ECH**  
I see there are a couple of them. The numbers are 2681 and 3338. To my understanding, they may not require the upgrade, but they are still a part of core EIPs.

**Micah Zoltu**
Oh, these ones. Yeah. These are tricky. And this is kind of why these ones have been taking forever to get through, unlike most core EIPs,  we don't have a good mechanism for coming to consensus among client devs on it. So it's a core EIP in the sense that this is a consensus thing, clients need to come to consensus on this. It's just they happen to come to consensus on it right now as a side effect, not as an intentional thing. And so Alex is trying to make it more official and say, "Look, this, these are the rules, they're very strict rules. And  everybody has to follow them." And everyone does follow them. Right now, we're saying that new clients also need to follow these. But we don't have a process in place for getting feedback from the coordinators to make sure that all the core client devs actually agree to this. And so I don't have a good answer for you. And these ones in particular are complicated and weird. Maybe Tim has some ideas.

**Tim Beiko**   
So I'm on my phone, which ones are the actually EIPs?

**Micah Zoltu**  
So one of them is limit account nonce two to the 64 minus one. So right now, there are no nonces in Ethereum. They go past that. So it's de facto a standard. But Alex is trying to make it official and make it so it's an actual consensus violation to go above that somehow. I don't know how we get consensus on that from the core devs because we don't actually have to do anything.

**lightclient**
First you have to convince Micah to that 2 to the 64 is the right bound.

**Micah Zoltu**
That's fair. There are two issues here. I disagree with Alex that the right bound is 2 to the 64.

**lightclient**
He disagrees with me now, because I was trying to finalize this, like, six months ago.

**Micah Zoltu**
Alright, so I gotta disagree with both of them. And so really, what we need is we just need core devs to say, is it 2 to the 52nd or is it 2 to 64?

**Tim Beiko**  14:13  
Can you put it on the agenda for this Friday or next Friday? The agendas are pretty empty right now. So if you have a backlog of things you just need the plus one on, I think we can probably - and especially if you put it on the agenda a couple days at least before, people can see it and comment.  I have, like, zero opinion. I agree that if that's the behavior we want, we should get it documented. I don't care what the number is. But I think, yeah, just getting different client teams to kind of state what they think. And we actually don't really need a hard fork for that.

**Micah Zoltu**
There's no fork. It's asserting rules that are in place as an accident. Both these rules are satisfied right now and for all history.

**Tim Beiko**  15:20  
I guess it would take a lot for somebody to actually break that rule, right?

**Micah Zoltu**
Yeah, the gas costs would be insane.

**Tim Beiko**  15:34  
Just imagine the amount of throughput we have on the network, right? You get like a million transactions.

**Micah Zoltu**
This is really just something that will help integrators integrate a little bit, having concrete bounds, because it makes it easier for them to just know that "Okay, I know, this number will never be too big. So I don't have to worry about this whole class of problems like overflows and whatnot."

**Tim Beiko**  15:59  
Okay, yeah. Yeah, let's just put it on the call and see if there's any reason not to strictly bound it, but I doubt there would be one.

**Pooja/ECH**  16:09  
I can add it to the agenda to understand what could be the process for these proposals. And then we can probably discuss it and see if this can be moved to Final status, because my review period has already ended. And these have been in Last Call for over a year now.

**Tim Beiko**  16:30  
I think I think the process is probably to have them on AllCoreDevs. And the reason this is six months is just because it was way less important than the past six months of conversation. And not that it's not helpful to have this rule, but as we were planning London, I guess it's just not the priority. And we ran out of time on a bunch of calls. Yeah, it's weird. The Last Call period might not be two weeks if these things just are not high priority. And if there's another really big high priority thing, say, in four months, if we're in the middle of the merge, I suspect something like this would also sit for a couple calls at least.

**Pooja/ECH**  17:12  
Yeah, yeah. Sounds good. Yeah, you wanted to add something, lightclient?

**lightclient**
I'm just looking at these. They're hilarious. These two Last Call EIPs fighting it out for the upper bound at the accounting.

Now that the balance supply of Ether is bound, we can come to consensus on the nonce bound.

**Pooja/ECH**  17:44  
So as I understand, one has to go and one has to move out. Right?

**lightclient**
Couldn't have said it better myself.

**Pooja/ECH**  17:55  
Okay, I'll add it to the AllCoreDev agenda, and let's see what people there think about it. Yeah, so moving on. There was this one last item that I wanted to bring to the attention to the group that is related to ERC title format. So I don't know if these are the right people to talk all about ERC, but because this is related to process, I just am looking for some good feedback here. So at present, the title that that is added in an ERC even for the new proposals, those are variable. Some people add it as like "ERC 123" and then whatever the ERC is for, and some people do not write the "ERC 123" part; it's just EIP and then whatever the proposal is about. I'm wondering if we can have a standardized format. So I looked into eips.ethereum.org and the first ERC is ERC 20. I think that was created by Vitalik. So in that, the title states specifically that it is an ERC and then mentioned it as token standard. So it is written as EIP-20 and then ERC-20 token standard, but this is not the case with most of the ERCs. What do editors think in general should be the general practice? If we standardize it, we can start educating people and let them know it's a good practice to have in place.

**lightclient**
I don't think that we should prepend ERC to the title.

**Tim Beiko**  19:56  
I will defer to lightclient.

**Pooja/ECH**  20:04  
Okay, because there is no clear instruction here in EIP 1 how it should be written.

**Tim Beiko**  20:18  
Yeah, we don't have "core" in the core EIP titles, right?

**lightclient**
Yeah, that's the point of the category. If it says its an ERC in the category, it shouldn't repeat that it's an ERC in the title and then repeat its number. Unfortunately, a fair number of really big ERCs have done this. I'm looking now at ERC 721 is "ERC 721 - non-fungible token standard." It should have just been "non fungible token standard." ERC 1155 should have just been "multi token standard." I think we can go back and replace a number of these with just their titles. But some of them don't make so much sense with just the title they havem like "ERC 777 token standard," if we just replace it with "token standard," it's not quite clear. Yeah. I don't know. I think, again, we can probably go in and replace most of these and just try to keep people from doing it anymore.

**Tim Beiko**  21:15  
Do we need the author's plus ones to change that? I assume so?

**lightclient**
Yeah.

**Tim Beiko**  21:20  
Yeah. So I guess it would be helpful to know how many. If there's, like 50 of them...

**lightclient**
Actually I don't know. Some of them, I would say no, the ones that actually have good titles. I think we could do 721 without having an author approval, because it already says "non fungible token standard." That's really a very non-normative change. For 777, I would want to add something that describes it a little bit better.

**Micah Zoltu**
So hopefully, you guys can hear me. So I would I kind of agree with Matt [lightclient] there. I think that for all of them, we should remove the EIP number from the title. For some of them -

**lightclient**
Ah, he cut out. We lost you.

**Pooja/ECH**  22:19  
Alright, so my next question here would be, is it something that can be done on Final proposals if we get author's permission? Or can it be doneat the guest level?

**lightclient**
I think most of them can be done, the ones that make pretty good sense without the ERC in front of it, we can just do. The ones that are less clear, maybe we can ask for author's opinions to help. But it looks like most of them can just be removed.

**Pooja/ECH**  22:53  
Yeah, I don't see there are too many. So this can be handled. I think it's less than 10. Yeah. 7, I think. Less than 10. It can be done. We'll try to reach out to the authors and request the changes. I'm not sure changing the title of the proposal, more than just removing the ERC number, is that something acceptable because this is already in Final status?

**lightclient**
It's fine.

**Pooja/ECH**  23:30  
Oh, okay. Okay, then we'll try to connect with the authors and see what we can do. Would it make sense if we add a line in EIP 1 stating "Do not repeat this thing that ERC-123 before your title" so maybe the future proposals that come up do not have it added?

**Tim Beiko**  23:58  
I think either EIP 1 or the template, right?  In the template, we can maybe add a comment beside the title saying "Don't put the EIP number here."

**Pooja/ECH**  24:10  
Right. Yeah, yeah. For backlogs, we can do it manually, reaching out to authors, but for the future, we'll try to get it documented. EIP 1 is the best place and attempt it as is suggested, so we'll try to get it done. Maybe someone will create a pull request to do that. Or they try to do that too. Okay, I think Micah added something on the comment, which is something to discuss description field in the header, header, place of summary section. Let me pull out that pull request number. I think it is by Axcic. Oh, Micah, you're back. Please go ahead.

**Micah Zoltu**  
Maybe. My internet is being terrible. So the TL/DR is that we currently have a simple summary, which is intended to be a place where you provide a very, very short description of the EIP, like one sentence long. I usually recommend people think of it like an email subject line or GitHub pull request title, or the kind of short description on a forum thread, something like that. Alex would like to move that to a description field and put it up in the metadata. So that way, we can render it specially, like it has more of a special place. And so when we have tables and lists of EIPs and whatnot, we can integrate it better into places that render EIPs in different ways. And I generally agree with this, I think it's good idea. And so we're seeing if anyone has any problems with that change.

**lightclient**
I'm on board.

**Pooja/ECH**
I like that. In fact, I like the number two format that was suggested here.

**Micah Zoltu**
If no one has any problems with it, then we all tell Alex to go ahead and move forward with it. Sounds like everybody generally likes number two format, so probably go with that one. All right.

**Pooja/ECH**
Yeah. So that's about it. And that, yeah.

#3. [JSON RPC API spec progress update](JSON RPC API spec progress update)

The next item on the list is a JSON RPC API spec progress update. Alita wanted to provide some updates. But unfortunately, I do not see her on the call. So we might want to skip the item. It seems like this meeting is going to be a little shorter than usual.

#4. [Review action items from the previous meetings](https://youtu.be/eo90AIGv3jw?t=1609)

I'm moving on to the next item, which is getting into action items and decisions made from the previous meeting. And if people find some other topic that they would like to discuss in today's meeting, we can probably pick it up after this one. So the action items, it says that Pooja will consider feature update to present EIP bot as a task list and ask detail to provide your feedback. Yeah, but unfortunately, we do not have Alita on the call. So maybe keep it open for the next meeting. And we'll come back on it. Yeah, we added bot tracking inactivity period. I think it is still there. Yeah, I think we have covered whatever we added in the agenda for today's meeting. Anyone wants to bring up anything else?

Well, if not, then we I think we can give everyone 30 minutes back. We are ending up early. Thank you all for joining us today and see you all in two weeks. Thank you.


# Attendees

* Brent Allsop
* Tim Beiko
* Jim Bennett
* lightclient
* Pooja/ECH (Host)
* Micah Zoltu



# Date for Next Meeting: Aug 25,2021 at 1500 UTC
