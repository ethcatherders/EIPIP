# EIPIP Meeting 43 Notes
### Meeting Date/Time: Wednesday, Nov 03, 2021, at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/90)
### [Audio/Video of the meeting](https://youtu.be/EV7plRxP0A4)
### Moderator: Pooja
### Notes: Alen (Santhosh)

----

## ACTION ITEMS

**ACTION 43.1**: Rename review-period-end to last-call-end to be added in the EIP template, EIP-1 and General consensus.

**ACTION 43.2**: What it takes to be on the list of active EIP editors: You anticipate that person responding to pings from the bot with a reasonable delay. And to attend these meetings, say, once a quarter.

**ACTION 43.3**: To agree on who gets mentioned in EIPs - Lightclient and Alex get mentioned for everything in EIPs. And Micah gets mentioned for core.

**ACTION 43.4**: Micah to merge Pull request [#4390](https://github.com/ethereum/EIPs/pull/4390), as the editors has approved it.

**ACTION 43.5**: EIP registries - Looking for someone willing to put in the time to be like the first editor or equivalent

**ACTION 43.6**: Pooja to open an issue in the Eth bot repo for Alita to check if the bot will merge it as a stagnant if there are no new pull request but just with comments.

---

## 1. Rename review-period-end to last-call-end or last-call-deadline. Ref: [Issue](https://github.com/ethereum/EIPs/issues/4413)

**Pooja Ranjan**
* Welcome to EIPIP-43, I'm going to share agenda in the chat here. The first item on the agenda and listed here is renamed review period, and two last call N on last deadline. So this has been reported by, um, ASIC. I have added the issue, , for reference, um, generally makes sense, like now that we have review as a status, not as just the last contribute period. , so, um, we try to add the entered review period for the last call, not for the status review, but yeah. Looking for general opinion so that it can be used as a standard field from here on 

**Lightclient**
* Fine 

**Tim Beiko**
* Fine with the change. 

**Pooja Ranjan**
* So there are two options, which one is, 

**Tim Beiko**
* So I would have it be like last call review period, or he had a better name for about the basically just changed the name to better signify what we actually mean by it. 

**Pooja Ranjan**
* Right. So the two options are, yeah, please go ahead

**Micah Zoltu**
* I have a very, very weak preference for last call end, but I don't actually care if within two options. 

**Tim Beiko**
* Yeah, I will. 

**Pooja Ranjan**
* Alright. So, maybe closer to the earlier nomenclature, like it was review period. And so maybe we can take it for last call and, or the, yeah. Alright. , so this might need to be added in like template EIP template and EIP-1, and obviously we'll add the general consensus of here so that issue can be closed. Quick.  

## 2. Discuss qualifications for being on the Active Editors list. Ref: [Comment](https://github.com/ethereum-cat-herders/EIPIP/issues/90#issuecomment-954722410)

**Pooja Ranjan**
* So the next one is, , discussed qualification for being on active editors lists. So there are multiple agenda items that, um, suggested when Micah to be added on the call today. And this is the first one. So we have listed some of the qualification, I suppose, back in February when they were trying to document what it takes to become an EIP editor that was just for inviting more participation from the community. Um, but it looks like it's time to revisit and maybe do a bit that EIP 1. So over to you, Micah, for your suggestions or comment for this topic. 

**Micah Zoltu**
* So the reason this came up was, um, the editors lists up until very recently included a large number of people that didn't actually do any editing. I think some of them were, they're just included just because when the EIP process was created, they happened to be around. Um, and those people aren't even anymore. Um, some of them were active editors for awhile, but are no longer active editors. Some of them are people that help put the EIP process EIP process together, um, but haven't done active editing. And so the idea is, is that, , if we're gonna have a list of editors, it feels like the primary purpose should be to serve users. And, um, when users go looking for editors, they should find a list of people that are actually editors, like people who are actually actively involved in the process and they can talk to and get feedback from, and, and also importantly names they should look out for on their PRs. 
* So like here's the people who, you know, have some, some, it gives you if you get a PR review from random person, which we actually get quite a few spam PR reviews, um, you can ignore it, but if you get a PR review from an editor that kinda holds a little bit more weight. So the idea is to have that list be, um, include all the people who are actively editing, but at the same time, um, not be, and at the same time, not be too long because if it gets too long, then it turns into a list of, you know, a hundred people and that's not a useful list. And so we want it to be concise and accurate and also like keeping the list short. It makes it more obvious that we were understaffed. Like when there's 10 editors in a list, it looks like we got plenty of people. 
* We don't need help when there's three editors and lists. It's more obvious that we very much need help. So, um, the question then is, is what is the process for removing people from that list? And I'm going to try to provide, since Greg's not here, I'm going to try to provide his arguments. We've been discussing this a little bit. Um, I'm probably not the best person, um, because I'm against him on this, but I'll do my best to represent him. And I think what he, his belief is is that anyone who is interested in being an editor, um, continuing to be an editor and continuing to be on that list should be allowed to remain on that list. And I think the idea is, is that, um, these are people that have expressed an interest and even if they don't have time right now, they, they have good intentions and maybe they do help out here and there, like maybe someone sends them a DM or something or mentions them, they will show up and help, but they're not actively editing. Um, and so the question just comes down to, you know, do people get, once you're an editor, always an editor, or once you're an editor, you can lose that status or more importantly to lose like that slot on the list at some point. 

**Tim Beiko**
* Yeah. It's almost like you want to part-time that you have like, full-time, part-time, you know? 

**Micah Zoltu**
* Yeah. Like I said, I go with the list it's primary for the users. And, um, I feel like in the more complicated list is the harder it is for users to make actual use of it. 

**Tim Beiko**
* Yeah. I'm not sure it's actually a good cause all the editors are kind of hard time by definition. Right. 

**Micah Zoltu**
* Like I don't think anyone works 40 hours a week, 

**Tim Beiko**
* So I not sure how to phrase this better such that it'd be well phrased, but like, is this like a process problem? Or like if people problem, um, because I, I suspect, I know I've talked with,Vitalik and I like explained to him and he was kind of fine being taken off the list, the active editor list that would be basically Micah, Lightclient, and Exil right. 

**Micah Zoltu**
* Yeah. Um, like if we sorted those, that would be the right order as well. I think in terms of, 

**Tim Beiko**
* Yeah, Right, right. Yeah. Okay. Um, and then, so it's like, if we're sorting, it's like Micah, Lightclient, Exil and then Greg kind of who's like worked on some of his EIPs, but I don't think he's like worked on like he's helped edit any EIPs that were not his, is that correct? Like in the say like last year or whatever, like recent past, 

**Micah Zoltu**
* I do not remember his name coming up on as an editor, like, um, helping people. Um, he has indicated to me that he has, um, helped people out with EIP offering in the past. I don't have much more context in that., he, he has not had an active role in like reviewing EIPs and approving them and pushing them through the process that, that, that piece, at least nothing, the visible, 

**Tim Beiko**
* Yeah. I tend, so I tend to agree with you. That's like, there's a lot of value in signaling who are the actual editors and maybe like a very new stretch hold for that is like, you know, they've like commented on like at least one EIP in the past two months or something like I'm like, we probably want like, to be somewhat relaxed with like what the threshold is, but like, yeah. I, I, I do think there's not even having like a clear delineation of like, these are EIP edits. Like these are people that you can pay and expect  a response on your EIP PR within a week. Right? Like maybe that should actually be kind of the, you kind of flip it and say, what should the user reasonably expect? Right. Like, and it's not good. It's not necessarily a guarantee that it happens every time. But like if I were submitting an EIPs and I'd look at that list, I kind of hope that if I paid, you know, somebody on that list, they would get back to me sometime during that. 

**Lightclient**
* I think right now. I feel like a reasonable, very reasonable qualification is to attend the EIP meeting, meeting every couple months, just so that there's like a synchronous moment to just talk to each other. Like, 
* I'm not saying come to every meeting, but at least one every eight weeks or 12 weeks or something, that way there's some sort of cadence of talking to a person in a secret manner. 

**Tim Beiko**
* Yeah. I think that's fair. It's like, you know, Kenny be pinged on GitHub, but can they be expected to show up once a quarter to one of these meetings that seems like a very low bar., yeah. And, and that's also something we can ask Greg, right? Like, do you want basically, do you want to be paid by random people on their EIP is, and to have like a soft expectation, that's like, you'll deal with these pains. Um, and do you want us to leave? 

**Micah Zoltu**
* Yeah, currently all the editors are pinged by the bot every time the EIP is put out to for review. So we, we are getting paid. We know we're getting ping, he's getting pings and he's not showing up. Neither was any of the other people that removed from the list. Same thing. I think Alex also barely shows up to the pings. I think he has some ignored. Um, yeah. 

**Lightclient**
* Well, he just commented on mine because it's like, everything is a pain.

**Tim Beiko**
* Yeah. Yeah. And I do feel, I dunno, my perspective as like somebody who's like loosely involved to this from the outside is like, Alex is, he's not like as involved as the two of you obviously, but like he is somewhat involved. He just commented on my PR. And I think like he does show up when like there's important discussion. So I think he would fit this news, you know? And I suspect that if we asked him to come to one of these meetings per quarter or something, he like he would, um, especially if there was a reason for him to be here, like, um, rather than just like shaking the teeth he actually showed up. But yeah. 

**Pooja Ranjan**
* Yeah, I think, , having like, , this kind of synchronous meetings definitely add value to whatever is being done asynchronously and they'll meeting once a quarter is like the lowest minimum bar that we can say. Um, but yeah, if not visiting here regularly, not biweekly, at least getting some comments on other pull request makes sense. And that's not being observed in case of Greg. I mean, I didn't remember anything. Um, definitely in the past one year I can say I was looking into that and then Exil he showed up and he just wants to that. 

**Tim Beiko**
* So, So what's the next step. Um, so Greg has already removed from The list again, We'll have like merge access to the, there was something that he was, he was complaining about being removed from something There's yeah. 

**Micah Zoltu**
* There's, there's two separate issues. One is who, who are con who's classified as editors and two is who has right access to the repo. Um, the, I believe the ops team was doing, I don't know, but I'm guessing the ops team was just doing general cleanup and removing people who that's, what you're supposed to do, you know, as good security practices, you clean up people who don't need access anymore. And I think they just cleaned up a bunch of people and that included, , Greg, again, I'm guessing speculating here, but if I was a security ops team, that's exactly what I would do. Um, so, so yeah, so two separate issues. One can be an editor and not have right access there. Access to be under all like that for the longest time. 

**Lightclient**
* Oh, I mean, I don't think I have right access to anymore. I think I realized this yesterday, while we were doing this like EIP editing session. And I was like, wow, I understand here, LARPing as an editor, I can't even write for fucking repo. 

**Pooja Ranjan**
* Yeah. I'm walking on that. I mean, I, again, , um, Jimmy for this, , for getting the access, um, I don't know, admin or write or whatever is needed, but I'm waiting for his response. Maybe Tim me if we can give him a little nudge and get this thing through would be helpful. Yeah. That stuck because we do not have it's requested by Micah and now we need another addicted to mergers because it cannot be like most likely. 

**Tim Beiko**
* Okay. , let me see if I can do something about this. Yeah. So lightclient, you basically need to be have right access to the EIPs repo that would fix that. 

**Lightclient**
* It would be great to have admin access so I can override the bot in these scenarios. 
* I think. So. I don't know if it's right or admin, but Okay. I've never been able to overnight the bots and I just assumed I had right extra. So maybe I've been confused. 

**Micah Zoltu**
* Um, let me, let me look. 

**Tim Beiko**
* Does your GitHub handle having an asset SDM map? 

**Lightclient**
* no. Just like client 

**Micah Zoltu**
* You're right. 
* Sorry. , you, you do have right access. You do not have admin access. I thought, right. I got you. Yeah. Apparently I can make any admin. Excellent. And just do it. I mean, I mean, I have, I have tried to avoid this because it's not like I don't want to overstep my bounds. Like if maybe there's a reason that the operations team has not given Matt, 

**Tim Beiko**
* But otherwise right now I'm going to log in to get in the dev ops, EF teams, backlog that says add lightclient as an admin. They'll probably ping me and ask me, why do you think lightclient should be an admin? I'll tell them that. I think he's a very active contributor to each repo and it's blocking things that he's not an admin. 

**Micah Zoltu**
* So then they tell you, well, we did a background check on lighclient and, , really rather not give him. 

**Tim Beiko**
* Yeah, I think I think he can just add a Micah. I'm not doing a background check on unlike lightclient, Just one reference. 

**Pooja Ranjan**
* I'm sharing a pull request number 4390 here. So this has been stopped because I mean, we were looking into proposals  yesterday proposals and pull requests in the EIP found in meeting they found that because this is done by Micah, it needs to be managed by Lightclient and he cannot do that without the admin access. If someone needs a reference, this would be a reference why he needs access. 

**Tim Beiko**
* It's fine. Yeah. I I'm fine. , taking any backlash that comes from adding Matt as in EIP admin, not backlash. 

**Micah Zoltu**
* I think I'd rather wait for the ops team because I'm seeing some Ruby in his code history. And that just makes me really uncomfortable. 

**Tim Beiko**
* Well, you've read a scat on his wall address, right? Yeah. 

**Micah Zoltu**
* He said some things on social media. Well, and you said That's right. I just, I think we should make sure we list that security team do their job before I add anybody. 

**Tim Beiko**
* Okay. Well, yeah. Okay. So that's not, yeah. 

**Pooja Ranjan**
* Yeah. I'm coming back to just, just to have a summary of it. So the note taker can actually document this and we can record it as required for what it takes to be an active, , to be in the list of active list. If someone can summarize it for 

**Micah Zoltu**
* Be like a Micah, Matt, or Alex. 

**Tim Beiko**
* Right. So I guess what I understood is you expect that person to respond, to respond, to pings from the bot at a reasonable, you know, would a reasonable delay. Um, and to show up to these meetings, say once a quarter. Um, yeah, I think, No, that's it. 

**Micah Zoltu**
* I think to clarify a little more, well also remaining in vague, I'm not a huge fan of like really strict rules. Cause then you're sending with people, rules, lawyering, like, oh, I posted my one comment. I get to keep my access. Um, I would say that, um, you are actively responding to random, like, , people, people looking for editor editorial support on the EIPs repo at some regular interval that is, you know, on the order of months. Um, so, so not just like, oh, well I review my friend's PRS. Like, like we have editors in the past who have, you know, they, they show up, but they only show up in edit, you know, PR is by their friends or by them. Um, and we really want editors to be people that are helping everybody. Um, this is part of my soap box that I'll get to later on the agenda. Um, but I don't like the idea of giving special treatment to prominent figures within the community. So like when Vitalik opens a PR and he's got like four editors jumping on to review it, because the problem there is that means every time Vitalik doesn't think there's a problem. Like they're not like thanks to the EIP process is working fine because for him it always works fine. And you see this in really corrupt governments where like some government official will go through a process and they're like, yeah, everything's fine. But like regular people, it sucks. Like it's horrible. The reason it's fine for those speed other fields because they get special treatment. And so I really want to avoid giving special treatment. And so that's why I want to specify that if you're an editor, that means you're editing for everybody, you're helping all the people who want to participate in this EIP process. You're not just helping, you know, a couple of friends that will vote for you when it comes time to vote for who the editors are or whatever it is. 

**Tim Beiko**
* I think that's reasonable. Yeah. 

**Pooja Ranjan**
* All right. Do we take that this is something that needs to be maybe added some that even in EIP one, I mean, I already maintained something separate and a hackmd file when we are trying to add all the corner cases or special instructions that cannot be added to every one, but is it worth adding to one?

**Micah Zoltu**
* So people, I don't think so. And the reason I say that is because I think that it's best. If we try to keep  EIP one focused on what users need to do to create EIPs and not distracted by like the, behind the scenes you're you're accuracy of the editorial process. 

**Pooja Ranjan**
* Yeah. That makes sense. At least we have it somewhere documented, wherever needed. We can point it to the right place. Sounds good. So I think, , we can now move on to the next item, unless anyone has any time to comment on this. Okay. And so why we are discussing this, um, I would like to skip the number three and come to number four, because both are relevant. Agree on who gets mentioned in the EIPs. Micah, created this pull request to like who should get mentioned and that, I mean, at least that should be based on the present EIP active list. I don't know why this has anyone has any, 

## 3. Discuss Registry EIPs and what to call them: [ethereum/EIPs#4335](https://github.com/ethereum/EIPs/issues/4335) Ref: [Comment](https://github.com/ethereum-cat-herders/EIPIP/issues/90#issuecomment-954722877) (Skipped as it is relevant to 4)

## 4. Agree on who gets mentioned in EIPs: [ethereum/EIPs#4390](https://github.com/ethereum/EIPs/pull/4390) Ref: [Comment](https://github.com/ethereum-cat-herders/EIPIP/issues/90#issuecomment-954728126)

**Micah Zoltu**
* Yeah. I just wanted to bring it up with people. Um, before we merged that, , currently it's  lightclient and Alex get mentioned for everything. And Micah gets mentioned for core, Let's say for everyone, okay. With that, no, one's got an opposition or wants something different. 

**Pooja Ranjan**
* It sounds fair because, you have been vocal about it that you want to review good proposal. So it sounds fair. And rest of the two editors were there maybe get pinged for every thought of a proposal. 

**Micah Zoltu**
* Yeah. And I'm okay with people move, moving themselves. Like Matt decides he doesn't want to get pinged for core. I'm totally fine with that. 

**Pooja Ranjan**
* Okay, so this needs to be merged, I see that this has been approved by all the editors. So bot can do that or any of you can do that. 

**Micah Zoltu**
* I just want, I was just waiting for a the agreement. Okay. 

**Pooja Ranjan**
* Awesome. Sounds fair. Moving onto the next item. It's discussing registry EIP as to what and what to call them. This issue is created by any chance. I see some discussion between my Micah and Alex. So I let Micah explain to this. 

**Micah Zoltu**
* So the TLDR is, it'd be nice if there's a way to have lists of things in the standard repo. So like when you create a standard for thing, you could then have a, a list. A great example is transaction types, right? We've got three transaction types now going 4 or 5 in the pipe. And we just, I mean, I said, there's a place that we can record all these numbers in one place. So I list probably with the, the traditional EIP is that they are immutable, which means you cannot change them once they are final. And so following the normal process, you would not be able to actually maintain this list. The, after some discussion and thinking with Nick, my recommendation, and it sounds like is as well is to have some new type of standard or file or whatever. That's maybe in this repository, maybe in another. 
* Um, I think he he's lobbies for another, and I'm fine with that, where it is, and only, and the author of the registry, it's up to them to include very clear instructions as to what is necessary to get included in the list and the idea behind this, as we want to maintain censorship resistance within our process, as much as possible. And so we don't want it to just be like, oh, Bob runs this list. And then when Bob disappears the list, doesn't, it doesn't get maintained. Or we have, you know, fights over who gets the rights to access. So the idea is, is someone can draft a new registry. Um, and as part of that process, they would say, anyone can get added to this as long as they meet these requirements. Like if you achieve, you know, this, this, this, and this, then you can get added. And then the EIP editors or registry editors would do the job. Just making sure that when someone submits a PR to add themselves to a list, they include an argument for why they meet the requirements. And then they would say, yep, you check all those boxes. So we will add your line for the list. Like yep. You, you check all the boxes for having new transaction types. So we'll add you to the new transaction type list. 

**Pooja Ranjan**
* Any thoughts and comments? Tim, Lightclient.

**Tim Beiko**
* No, 

**Pooja Ranjan**
* I see, lightclient unmuted, but unforunately we are not able to hear anything his end, atleast not me

**Lightclient**
* I guess I'm not able to get on my phone. Okay. Okay. 
 
**Pooja Ranjan**
* So anything from like, um, the editor sides need to be done, or is it something that, , that can be suggested to Nick Johnson and, , 

**Micah Zoltu**
* Thing is we need someone who wants to actually like shepherd this process. I think until we have that we can't really move forward at all. Like we need someone who is interested enough and willing to put in the time to be like the first editor or equivalent. I don't know if that's Nick, Nick might be might've created the issue because he specifically is hoping that someone else will take it, take up the torch. That is not me. Same, do not have the time. 

**Pooja Ranjan**
* Okay. And that gets, maybe we can spread the news and see if we can find someone to actually champion this idea or convert it into a proposal and then come back to submit proposal for my purposes for that. Um, and if this sounds reasonable, we can probably move on to the next issue and let, let's keep that issue open the same time. And so we can refer like people do. , see if they are willing to champion this idea, 

## 5. EIP file name error problem for new submission Ref: [Issue](https://github.com/ethereum/EIPs/issues/4398)

**Pooja Ranjan**
* Moving on to the next item listed today is a EIP file name error problem for new submission. So this issue is created by,submitted by an author author who probably is documenting the proposal for the first time and is looking for some help. Um, I'm not sure this is for a Alita, 

**Micah Zoltu**
* I believe that was just a bug report. And so it's filed away later. We'll hopefully handle it at some point. 

**Pooja Ranjan**
* Alright. Yep. Thank you. Then we can skip this item.

## 6. [EIPs Insight](https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/) - Monthly EIPs status reporting.

**Pooja Ranjan**
* The next item is EIP inside us. So we have shared this report for October 122 EIPs have been moved to stagnant. Five new proposals were added as draft and two EIP are moved to review one EIP resurrected from stagnant that's for the Oct and in November. So far, there is only one proposal which has been added as a drafted that is EIP 4396, time aware ESB calculation. So that's on the EIP status reporting. I have one question for Alita. Um, I wanted to check what happens to, um, move to stagnant pull request pack created by bot. And if someone respond to that pull request, when is the next time that is reviewed or considered, will it be open for next six months? 

**Alita**
* So the only way to like get. Yeah. I mean the only way to like prevent the bot from reopening a pull request against it is to actually push a change to a file. Um, either that, or you have a pull request open against a file. Um that's yeah. If you could leave a comment on the, on the pull request, nothing will happen. 

**Pooja Ranjan**
* Yeah. So my question he had is like, , suppose bot created a pull request to move, , an EIP to stagnant and someone responded to that. So just as a response to that response, but may not move it to stagnant. The question here is when it will be reviewed next after the six month. 

**Alita**
* Well, no, the, I guess I'm trying to say is, , if a person just, are you saying like that, like they leave a comment on the pull request, 

**Pooja Ranjan**
* Right, Um, and it is nothing related to changing any status or something just as simple comment. 

**Alita**
* Okay. So yeah, in that case then it would, it would just be merged. So like it wouldn't, they wouldn't prevent the EIP would be marked with stagnant. We can, I can add that feature, but that's not how it currently works. 

**Pooja Ranjan**
* All right. So there was this one specific case that I had identified. It was for EIP 2070, which was , stagnant. And it was my simple comment that that should be like move to withdrawn. I found that that hasn't been merged as a stagnant. So I was wondering like, what would be the next review PDF or would it simply be most because there is nothing from the author's side. 

**Alita**
* If that's the, I think I saw your comment, it's going to be merged, , it, so the pull requests are open for two weeks and then they're merged unless a change is made to the file and, or, um, the pull requests, a pull reference has opened, , notably right now, actually that feature doesn't really work because, um, it checks to merge, , open PRS for two weeks. Let's actually just go back. I don't over-complicate this. Um, so to answer your question, it's going to be immersion week. Can we get a stagnant unless the PR is opened or, um, unless a change is made of that file. 

**Pooja Ranjan**
* All right. So I see here this, I mean, this pull request was open about 18 days ago, and there was this, this one comment. So if I understand that correctly, , if there is any comment, but no new pull request, the bot will merge it as a stagnant. 

**Alita**
* So I think maybe is a bit of a false positive. I would suspect that, um, first off, I think maybe create an issue in the Eth bot repo, , about this specific pull request that you're talking about, and then I can investigate what's going on with it. the behavior that you're describing is not something that we attended. 

**Micah Zoltu**
* I believe the issue is, um, somehow it added the wrong label, I think should have had the stale label and instead added a big number. So it looks like just a bug and there's currently three issues in there with that weird label. So I think some bug needs to be fixed 

**Alita**
* And large number is the bot, um, ID ID. So Well, and that's like, the idea is at the bottom, the pull request a minute, labels it with that to make sure that, you know, it's easy and it's guaranteed that, um, any pull request with that label has, um, is from the bot. Anyway, I can look into it and try to figure out what's going on. But so I think the best thing to do here is to just create a issue in Eth And, I can take it from there. 

**Pooja Ranjan**
* Sounds good. I'll create an issue there. All right. 


## 7 Review action items from the [previous meetings](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20042.md)

**Pooja Ranjan**
* Moving on. The last item listed here is review actions from the previous meetings and, first one is Plan a PEEPanEIP with Sam Wilson, we did it yesterday. I will provide release the recording. Um, next Monday, EIP-1 to mark “Stagnant” as another terminal state.. I'm not sure if this has been addressed. I did not make any pull request on my end. Might have to check if anyone else did it. If not, then I will try to create the pull request this week for it. 
Run a bot for issues in EIP, GitHub. I have seen the bot activity. That's correct. Thank you. So, , the course of action is very much similar to the pull request, right? It will. First market was stale and then eventually closed, right? 

**Alita**
* Yeah, that's correct. 

**Pooja Ranjan**
* Thank you. The last action item in the list, it is update PR to update the list of EIP authors in EIP-1. So we have made some changes. We have added their metadata as the editors there, but it looks like from today's discussion that this list might need to be updated further. So maybe, , we can revisit the EIP list after a couple of weeks and see if we need to make the changes to it. That's all from the agenda item. I suppose 

**Micah Zoltu**
* You left off my last one. I'm guessing because you assumed I wasn't being serious, But I actually would like to, , to just tell, share with everybody and the two people who actually watched the recordings of this call, um, why I am such a Dick about EIPs. Um, cause I know I am like, I know what, what my actions look like from the outside. And I've explained this to people many times in EIPS, but the message doesn't seem to get it out there. So the gist of it is, is that currently I give people a hard time and tell them, Hey, this is the process. Follow the process. You know, we have these rules. I don't like the rules, but we stick to the, I stick to the rules no matter who they are. And I frequently get people frustrated, I think because they are, um, people of notoriety within the Ethereum community. And they are obviously not bad actors. They're not trolls. Like they're not the people we're supposed to be protecting if they're him. Yeah. If he process from, um, and so they feel like it would be reasonable and this is reasonable to just let them, you know, put their stuff in there, whatever that is. Um, be it external links, be it extra sections in the EIP, it's skipping certain steps in the process. Like all these things are things. People request of me as an offender. And the reason I say no to all of them is twofold. One it's because we are very understaffed right now. And the processes we have in place are largely there because they're incredibly simple to implement. These processes are like no external links. That's really easy to implement. If I see an external link, I just say no. Like it takes me two seconds. However, if the process is, you know, extra links that are likely to 4 0 4, um, or extra links from people that have an authored a bunch of EIPs before now, all of a sudden the process becomes much harder to implement is no longer simple for me to just say no, I now have to look who the author is, look at where the link goes, try to evaluate that link. 
* Um, and then on top of that, what this leads to is an, I actually do get this a lot. This is not just me making stuff up. When I approve PR that allows a link through. And then I disapprove someone else. That person I disapproved will say, but you let so-and-so through. And now I need to have a very long discussion with the second person explaining why the why link a is okay. But link B is not okay. Or why section from this guy's EIP is okay, but the section in their EIP is not okay. And so, um, that is one of the reasons why I'm a Dick on the EIP and why I just make everybody follow this silly bureaucratic process. Um, because we were very understaffed and the bureaucratic, the processes in place to make sure that the little staff we have can actually get things done. 
* If people want the rules to change, the number one thing you can do is becoming yet yet EIP editor or recommends me IP editors. If we had more staff, we could make more wishy-washy decisions. We could have fuzzier rules. We wouldn't, we could have time to explain to users why, you know, LinkedIn is good, but LinkedIn is bad, but at the moment we don't have that. We have me and Matt and sometimes Alex. And so, um, so yeah, so that's, that's one of the reasons the other reason is, and this is kind of tangent sort of related. There are people who are notorious within the Ethereum ecosystem, you know, Vitalic being the obvious one. Um, but I don't actually get this problem from him, but just as an example, and then there are people who are not, so who have never shown up, maybe they created a new GitHub account anonymously. 
* And so I have no idea who they are and both these people are spending AIPs. And there's a desire for the people who are notorious to get there yet, be pushed through a little quicker than everybody else like they want, um, they don't want to follow the process. They don't want to go through the steps. They're, they're just, they're frustrated. They're like, why can't you let this through? Like, you know who I am. I'm not like this isn't spam, obviously, et cetera. And for those people, the reason specifically, I do not push them through. In fact, I put them at the like whatever place in line they show up at that's where they get, they don't get special treatment. And the reason for that is, as I mentioned earlier, I really want everybody who is in positions within the Ethereum ecosystem to recognize how understaffed we are. 
* Like, as I said before, if the people who are in positions, that they can actually have a voice, they can, you know, tweet to people and people will actually hear it. They can solicit for assistance. I want those people to understand how painful it is for everybody else. Like when you're that random dude off the internet who doesn't have, you know, friends in the right places and it takes you three weeks or a month, or in my case several years ago, like I hadn't yet that sat for over a year, waiting for an editor to review them when you're those people, like, you don't know who to reach out to you, you don't, you don't have a better system. And so I want the people who have, have a voice to recognize how painful this process is. And hopefully they can then use that voice. They have to solicit additional assistance and additional help and get more people like working on this so everybody can not suffer. I don't want to just be like, okay, I'm going to help. So-and-so because they're important or they're special. And I'm going to ignore all these other people. So that is why Mike is a Dick, the short version. I just want to everybody to know that it's not because I derive pleasure from being a Dick though. I do. But that is not the reason in this case 

**Alita**
* Here, here, I don't know. That's the written statement. That's great. 

**Pooja Ranjan**
* That's right. Um, and I would agree here, B you have been a hero here because many things that have, that we have changed in the past. It's because you like climb a Hudson for some time and people like you, they showed up and try to make a decision. And then we, the Catheaders tried to document them formally and share it with the rest of the community, that this is the process. There was always like a flow, but there was no defined line what to follow, what, not to follow whom to reach. And now that catheter said there, we have seen people reaching out to us on the cat herders discard, where we send it to a game to the EIP editors and we try to help and suggest them, what is the right process? So this would not be, , I mean, we would, , we would not be at the place where we are right now, if that's not because of you like Klein and Hudson and other people who actually became rigid and help us define this process. So thank you for all the work you have done here 

**Micah Zoltu**
* On that note. Do we have any, , potential people interested in an editor's? 

**Alita**
* I mean, I don't have enough time, but I'm happy to help out at some point. 

**Micah Zoltu**
* Yeah. The one we need and plenty of people with time, 

**Tim Beiko**
* I wonder how we can like advertise this better. It seems maybe we did like a pin post on these magicians or something, you know, say like EIPs editors needed. Um, cause it seems like it's hard because if you make it like too open as like, , , to open up like a process, you you'd probably get people who like, um, don't add a lot of value and actually stuck five away from like Micah and math, which is not great. Um, so I'm not sure if like what's the right place and it feels like the people who are aware that there's, , editors lacking are basically the people and the ether in deep discordant. And most of those people, um, most, most of them, yeah. They have jobs and they're also kind of, yeah, they've, they've considered doing this and they chose of two basically. Um, so I, I, I'm not sure, like what's the, what's the sweet spot. Um, yeah, this is the question about funding. I think we've had a bit of funding and like, if that was the maintenance, if that's the main blocker, I'm sure we can get the funding. Um, the part that's hard is it's kind of a very part-time thing. So it's not sure, like what's the best model to fund this, but maybe we can pay it or to whoever the person is. 

**Pooja Ranjan**
* Yeah. So just to provide us some update here, this EIP editors internship meeting that we do by weekly, we have one, , resources from catheters, of course, and he's under trading. And, , it seems to be like, um, I have seen William and Lightclient kind of nudging him and training him and maybe we can have him on formula editing, but right now he's in like very early stages of it. So it's trying to understand how the process work and what would be, , you know, the right place or the right context to add comments, which can add value in at least the drafting, the proposal. So, yeah, I think adding it as a a magician would definitely be helpful, but if you would like to send people, please do send it to like this small group who is trying to treat, , train people. Um, and like we have couple of resources we are trying to train that would be helpful. And Matt is there. He shares all the valuable information. 

**Tim Beiko**
* Yeah. Um, I guess, does anyone want to write a draft for the EIP editor? I can do it if, if you all are too busy, , but can maybe try and draft something that we could post. Um, yeah. 

**Pooja Ranjan**
* Yeah. But I, I don't know. I have shared this, um, posted that was shared on the Cat herders medium. So it was general guideline when we share idea how, if someone is interested to become any idea, which to us, um, we did get a couple of responses and we have picked up one or use it from death. So if this is helpful, you would like to add something more. 

**Tim Beiko**
* It's really helpful. Um, yeah. I'll have a look at it and I'll, I guess I'll take some time tomorrow to try and figure out what's the best place to post this. Like, how do we go about getting this visibility? Um, and yeah, maybe just like modifying does a bit. Yeah, 

**Pooja Ranjan**
* That would be helpful. Thank you. So I think, yeah, that's all from the items and comments listed today. Anyone wants to bring up anything new. So did the question off act the possibility of funding? Yes. CAC holders. So, , working with, , different grants last time, it was supported by ESP. And this time we are trying to reach out to and some of the fundings, if we have people we will be definitely working on And put your school quiet for everybody else. 

**Pooja Ranjan**
* I thought I saw in my meetings like that he is trying to add something because last time he was helping out this process. Yeah. Okay. Yeah. We should not be an issue. As you mentioned that if, if someone is interested and he's a willing to be a part-time editor, please reach out to us. I'll be happy to talk to them and lead through the process. What we have currently, we are trying to help out with whatever works, to get more people on both. Can reach out in Cat herders discord and my DM is also open on Cat herders. That's all from the items listed here. And if nothing else, we are almost on time. Thank you everyone for joining us. Hope to see you on the next two weeks. Have a good one, everyone. 

---------------------------------------

# Attendees

* Pooja Ranjan (Host)
* Tim Beiko
* Micah Zoltu
* Alita More
* Brent Allsop

# Date for Next Meeting: Wednesday, Nov 17, 2021, at 15:00 UTC
