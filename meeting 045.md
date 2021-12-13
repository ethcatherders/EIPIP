# EIPIP Meeting 45 Notes
### Meeting Date/Time: Wednesday, December 1, 2021, at 15:00 UTC
### Meeting Duration: 0.5 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/95)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=cJXWOu5aefs)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION ITEMS

**ACTION 45.1**: Pooja will talk to Jamie or someone from the ops team and try to get this new repository created for eip validator

## AGENDA

## 1. General consensus for closing recent most "discussion-to" issues.

**Pooja Ranjan**:  Welcome to EIPIP meeting 45. I have shared the agenda in chat. The first item listed there is a general consensus for closing recent “discussion to” issues. I understand we were discussing it in the last call. Like how do we manage the long list of open
issues and how to point people to the right place to start the discussion to link for any new proposal. I suppose we have updated the eip1 with a strong recommendation actually to start the discussion thread at fellowship of ethereum magician but still we are receiving some of the new issues where this particular section is being used as a discussion link for new proposals.
I understand a few meetings ago we decided and there was a bot which was updated to  generate messages for new issues. Saying that this is related to proposal discussion. Please create a fem thread and close this issue. Micah I see your comment that the message was supposed to be for the new contributor only.

**Mica Zoltu**: Yeah it's the greeter bot that gives that message out right now.

**Pooja Ranjan**: All right, sorry I thought that it is for all new issues that have been created. But I suppose this can be updated and as per your comment so it doesn't look like. You are
against it so what do you think? would that be a good idea to start for every new issues 

**Mica Zoltu**: I mean I guess the question I have is what do we want to actually use the issues for and maybe? This is a discussion that will need a bigger quorum than just you and I to hash out but what's what is your initial thoughts on. What are the appropriate types of issues?

**Pooja Ranjan**: That's right I mean this is a broader discussion I agree but my thought process here was like the issue and challenges that are being faced by new people who are trying to contribute with their proposal or their ideas in the sense. Like not only for discussing the proposal but also the challenges that they are facing during the writing of it. What kind of help they are looking for and if something sucks. Maybe I am hoping to use that particular section to be a point where people come up with their issues and that issues could be discussed here in this eipip meeting in future to help out and maybe streamline more processes around eips and network upgrades.

**Mica Zoltu**: So the issues would just be for basically editor discussion.

**Pooja Ranjan**: Correct, Yeah because that is an eip  github. So it should be mostly for editors
discussion here.

**Mica Zoltu**: I am fine with that but like I said we'll probably need to get more feedback from other editors. See if they agree. Yep the easiest way is probably if you want to create a PR to eip1 and just mention Alex ,Matt, me maybe Tim as well.

**Pooja Ranjan**: All right, yeah this is not something that has been added to eip1 yet. But I think it would make sense if we are in agreement or maybe we I can start with creating an
issue in this issue section saying that how about we start using this issue. Shepsen for different purposes I mean, I am not discussing at this point like  whether or not we should close the earlier issues which were created for that may require a separate discussion but at least this new I suppose

**Mica Zoltu**: Was that a question I think I missed?

**Pooja Ranjan**: No, I mean yeah that was kind of a statement but yes I suppose we should keep it open for next meeting or maybe I can go ahead and start discussing in the github itself.
We will see what feedback we receive there.

**Mica Zoltu**: Yeah

## 2. An appropriate placeholder for the link to active "eip validator". Ref [PR](https://github.com/ethereum/EIPs/pull/4442/commits/a3128d894d210d5964ca5c51b3250f4714d41e6a)

**Pooja Ranjan**: Thank you . I know today it is all on you because we have only one editor in the meeting. Sorry about putting you on the spot for this.  Okay, so the next item I have added here is an appropriate placeholder for the active eip validator so I see this pull request which has recently updated the readme of the eip repo which is good like we should not be having the old ruby one and we should be redirecting to the right one but I was wondering like this points towards an individual's github repository which I think would not be a good practice. I understand that currently he is a great contributor and we would like to keep it that way but it would be nice to have a placeholder for this eip.So that uh in future we can also get pull requests and updates from community as well as it would be easier for us to maintain rather than keeping it individuals. This came up in the past Matt is totally willing to move it over to ethereum. We just need someone from the ops team to do so. Okay I mean I am not sure if you
have any sense of what is required. Maybe I can follow up with the arts team and try to get it

**Mica Zoltu**: I don't know what the process is. I have never looked into moving a repo. My guess is that they just need to create a new repository named. I don't know eipv or whatever they want you want to name it and then they would just clone like clients repository into that
essentially make sense basically just do a little bit of magic.

**Pooja Ranjan**: Okay, maybe I will talk to Jamie or someone from the ops team and try to get this new repository created. cool

## 3. Incidence update for PR#4478, 4479, 4484, [4485](https://github.com/ethereum/EIPs/pull/4485)

**Pooja Ranjan**: Moving on to the next item it's about an incident which was reported for pull request 4478,4479, 4484 and 4485. So the thing is I can't find eip 722 in any of the repo. I mean sorry the atm repo but my understanding is all these merges are associated with that. I saw that there were some comments reverted but I was wondering yeah why did it happen in the first place.

**Mica Zoltu**: It was a bug in the auto merger. It accidentally auto merged something that shouldn't have. It's all the user created a new eipip with a number they gave themselves. They didn't realize that they weren't supposed to and the auto merge not just said sure and emerged. Alita very quickly fixed that so it shouldn't happen again and the eip has been moved to an
appropriate location

**Pooja Ranjan**: Yeah right because I was seriously surprised like it can happen once it can
happens twice, it happened four times. What's going on? Yeah great thank you Alita for saving us

**Mica Zoltu**: Yes,I believe the problem was the initial PR got auto merged and then the user was able to edit their eip because they now had eip 722. and then I think Alex finally got in contact with the user and moved it to the right location. So it didn't exist anymore so if you
looked after the fact it wasn't there.

**Pooj Ranjan**: Yeah right I think I looked a little late and I could not find the proposal
and that's caused me to wonder, thank you for updating that.

## 4.[ EIPs Insight](https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/) - Monthly EIPs status reporting.

**Pooja Ranjan**: The next item listed here is eip insight. That's a monthly reporting on eips, so for the month of november we have three new proposals introduced as draft. We have three eips those are moved to stagnant and three resurrected from stagnant two back to review and one is moved to draft from stagnant to proposals will move to last call but I suppose the review period is already ended and now there are a pull request in the repository to move it to the final
status. There was one eip which was withdrawn by the author. None of the eips were moved to review or the final status but I suppose there were some non-normative changes for eip 2681 and 2124. Some of the noticeable updates for this month for eip1 where we have updated the eip process. The process image for stagnant status and there is now description for preamble
fields to eip1 change in the field review period end. It has now been updated to last call deadline
and the updated field has been removed from the template. Couple of other updates, the one is running the rule for the discussion to urls, so that's on the eip inside side.

## 5. EIP editor apprenticeship meeting

**Pooja Ranjan**: The next item listed here is an eip editor's apprenticeship meeting. We could not conduct the second meeting this week but I have seen quite a few interest from the community and they have started contributing from different proposals. Yeah it is and I also talked to a couple of people individually and they said that like we can see some of the inputs to the comments on the repo itself but there are people who are also working in the back end. Connecting with authors, there is this guy who is talking to Richard because Richard is trying to pull his proposal back and it's nice to see people are trying to engage themselves. I suppose we will get one.

**Tim Beiko**: Sorry yeah what do we think is the right next step to keep these people engaged? Like how do we ideally eventually convert a couple of them to eip editors like
What do we want to see or like. Yeah I am curious. You know how? Because I think we want people to like you know proactively do stuff and whatnot but once they are doing it. How do we encourage them and get them to keep them engaged ? Yeah they stick around ideally.

**Mica Zoltu**: That is an excellent question. I still don't know why I stick around so I don't have an answer.

**Pooja Ranjan**:  Yeah I think it's something that we need to think about. Sorry stefan I saw
you were unmuting, please go ahead.

**Stefan**: Yeah thanks, from my point of view I just contributed in my first two bounties and I just learning everything and having a look around and I think  what you do brilliantly is all the
documentation it's really good to get the foot in and  I think you're a strong community.That's the base for a good onboarding. I will report back when I have got more information from my point of view if that helps.

**Tim Beiko**:  Yeah 100%. And if there's things you know you think are confusing or it can be done better or like yeah that are just like friction points if you can share those that's really valuable. Yeah because it's the first time that we have kind of interesting people. Yeah and I think we want to make sure that we don't lose people because like we just have a bad process or whatever.

**Stefan**: Sure yeah we'll do yeah

**Tim Beiko**: Awesome thanks

**Pooja Ranjan**: So we have planned the next meeting on december 7th. As I mentioned earlier I hope to see more people or people coming to share their experience for the past two or three weeks and if they have any new questions. So anyone listening to this on youtube. If you are interested and by insurance if you have missed an earlier meeting, please make sure to join this one otherwise the recording will always be shared with the community.

## 6. Review action items from the previous meetings
 
**Pooja Ranjan**: All right that was it and we are almost at the last item that is listed on the agenda for today. The review action item unfortunately we do not have the notes for it. I was informed that it will be later today. Sorry for the delay guys but I have a point listed out what were the action items from the last meeting. So I  made a poll request to update the web link to text removed from bibliography from eip1. I see it has been approved by one of the editors but it might require an address like one more approval from the two editors uh to be merged. There is this period made sorry please

**Micah Zoltu**:  If it goes another two weeks with no one else reviewing it we can just go ahead and merge. My policy is generally if we get two editors to review then we merge right away. If we can't if we only get one person to review then just wait a month and then merge.

**Pooja Ranjan**: Oh! all right, that's nice. Okay and uh the couple of other pull requests are
one to update the discussion to place and status cases and I think it has been merged already. Yeah, there was one action item on me to create an issue where we can start looking into adding labels to PRs. I have shared the eip bot github repository with a few people in the community like the new contributors whom we are interacting with and I am looking forward to getting some input, getting some updates and help from these people. I know stefan is one of thoseI shared the eip github repository. So we may be expecting some help in future. I know Alita left some comments, unfortunately she is not here for this meeting. She is traveling but she
left some questions and concerns that she has about this sharing responsibility or transitioning
responsibility. As of now I do not have any one single person in my mind like who can take over completely but if you do not get anyone I am hoping to make it decentralized like making these chats bounty based and get it done. But for sure we will be having people around to take care of ECH engineering. That's all from the item listed. I know Tim, you  missed the discussion on the first item when we were discussing about. The discussion has two links for general issues, so I am hoping they are like maybe we can create an issue or pull a request and tag you and the rest of the eip editors and have the discussion over there. Yeah that's all anyone yeah please anyone wants to bring anything up.

**Micah Zoltu**: Regarding Alita's comment on or question that she has in the agenda. I am fine with her just picking so if she wants to do number two of her options I am okay with that.

**Pooja Ranjan** : Yeah that's all right. Yeah I mean it's on her comfort level like of whatever she wants to do like any thing I mean generally we try to label them and out and I don't think there are a lot of issues so when it's like when there will be a lot of issues then can be priority based but that's okay good to know. Yeah anything else anyone wants to bring up otherwise this is going to be one of the shortest meetings of eipip.

**Micah Zoltu**: It's nice when no one shows up because they're all out makes it very easy to come to decisions.

**Pooja Ranjan**: Yeah right

**Micah Zoltu**: I have nothing else.

**Pooja Ranjan**:  All right folks, thank you for joining. The one major change that I am hoping to get done in future is about whatever the issues and challenges people are facing that need to be added. Somewhere from where we can start getting data because it's random and I have to search on all the discord and the issues and  github's repository. So I am hoping to make the eip github repository issue section be the section where anything that you want to be discussed or brought into attention offers the eip editors can be listed and we can take it out and start discussing in this eipip meeting. So folks if you are listening and if you have questions comment
concerns anything either show up on our discord channel or add it there in the issue section. We will try to bring it up in this meeting. Thank you everyone for joining us today, I hope to see you in the next two weeks have a good rest of the day. 

**Tim Beiko**: thank you likewise.

---------------------------------------
# Attendees

* Tim Beiko
*  Stefan
* Micah Zoltu
* Pooja Ranjan

# Date for Next Meeting: 7 December 2021 at 1500 UTC.





