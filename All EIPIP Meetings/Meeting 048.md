# EIPIP Meeting 48 Notes
## Meeting Date/Time: Wednesday 25 January at 15:00 UTC
### Meeting Duration: 1/2 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/105)
### [Audio/Video of the meeting](https://youtu.be/0oW6n9yuwoU)
### Moderator: **Pooja Ranjan**
### Notes: Jim Bennett

----
## ACTION ITEMS

**ACTION 48.1**: Check to make sure the greeter bot gets activated only for the issue section, not for the pull request. [see 14:21](https://youtu.be/0oW6n9yuwoU?t=862)

**ACTION 48.2**: Anyone with suggestions about the merger bot should reach out to the EIP editors or the Cat Herders team. [see 17:01](https://youtu.be/0oW6n9yuwoU?t=1022)

**ACTION 48.3**: Include Spurious Dragon updates in every alternative meeting [see 27:37](https://youtu.be/0oW6n9yuwoU?t=1657)

**Pooja Ranjan**  00:00
All right, welcome to EIPIP meeting 48. I just have shared the agenda in chat.

## AGENDA ##
## 1. [EIP bot](https://www.youtube.com/playlist?list=PL4cwHXAawZxpLrRIkDlBjDUUrGgF91pQw)

The first item listed here is EIP bot. So as we know that there has been a lot of work going on on the EIP bot side. In the last meeting, we discussed some of the working of different bots to be documented. And I have also added some of the items which were picked from the Discord discussions. So let's start with the updates, if there are any, on the working of different bots. Shashank, would you like to take this one?

**Shashank Yalamanchi**  01:03
So I verified there are two bots, basically one that lightclient built, and then the other one was the the one that Alita built. As far as I'm aware, there is no third bot.

**Pooja Ranjan**  01:47
So I think we have two bots here for sure. But I was wondering if there wasn't a third bot. One I can see is the EIP bot. And the other one is which GitHub actions bot, right?

**Micah Zoltu**  02:04
Yeah, so we got the GitHub actions. We got a bunch of bots. There's the greeter bot; there's the merge bot; there's the validator bot. There's the old validator bot. And I think there's one or two more.

**Pooja Ranjan**  02:21
So I think the greeter bot is the same as GitHub Actions bot. I just read the name over there on the issues and pull requests that were mentioned earlier.

**Micah Zoltu**  02:32
All of them use GitHub Actions, but I believe they are separate. GitHub Actions is a kind of a tool suite, and you can set up a number of different bots that utilize that. And so the greeter is run by GitHub Actions; the merge bot is also run by GitHub Actions. The validator is not. It is run by Travis CI.

**Pooja Ranjan**  02:57
Got it? I think Shashank is back.

**Shashank Yalamanchi**  03:03
Maybe I should speak a little louder. So I identified that there are two bots, one written by Matt and the other one was written by Alita. So I'm currently going through the bots. I didn't get time because my health wasn't - I kind of got COVID and got sick, so I didn't get time to go through the entire code. But I've been able to identify how the bots are being triggered, exactly when they are being triggered. So I've been making small nodes here and there. So that I basically first understand what's exactly going on. But there are a couple of things as to how are these EIP editors being assigned for specific reviews, and how the reviews are happening for each EIP or the issues or PRs that are being submitted that I'm still trying to figure out. So that's the part that I have a little bit of a bottleneck to understand exactly how is that process being defined?

**Micah Zoltu**  04:08
So I can answer the question of how are EIP editors assigned. There's a file somewhere that just has a list of the different EIP types. So you have ERCs and Core EIPs and informational EIPs. And there's a file that says these are the editors that should be mentioned if it's ERC, these are the editors that are mentioned if it's Core EIP. I'm trying to find it right now. There it is. So it it's line 18 through 26.

**Shashank Yalamanchi**  04:49
Got it. Got it. Okay, it makes sense.

**Micah Zoltu**  04:57
And then I don't know how the bot reads that, but it's space is passed into the auto merge bot. So, like, a set of variables, I think...

**Shashank Yalamanchi**  05:07
Yeah. So these are basically the GitHub user names of the individual EIP editors, as far as I understand.

**Micah Zoltu**  05:20
Yeah.

**Shashank Yalamanchi**  05:20
Okay. Got it. And how does the review process happen? So let's say if I submit an EIP, which is like in pre-draft, just call it pre-draft, because it's not submitted. So as soon as it's ready to merge or be pushed into the EIP repository, how is that process different?

**Micah Zoltu**  05:44
So as soon as you submit a PR to the repository, the bot will see it and assuming the bot can figure out, assuming it's formed well enough that the bot can identify whether it's a Core IP, or an ERC or whatever, then the bot will mention the appropriate set of editors, and then one of them will, at their earliest convenience, review it, give you feedback, and then once everything's good, then it will get auto merged. Or rather, then the editor will approve the PR.

**Shashank Yalamanchi**  06:16
And after that, it also is being submitted on the EIP web's subdomain, right?

**Micah Zoltu**  06:30
Yeah.

**Shashank Yalamanchi**  06:30
Got it.

**Micah Zoltu**  06:31
As soon as it's merged, then it basically every EIP that's in the repository shows up there. Minor exception, I think. I don't know if we ever got rid of "Stagnant" from the EIP site. I think they still show up on the EIP site, but maybe they're not in the list or something.

**Shashank Yalamanchi**  06:48
Okay, and were there any edge cases in the past? Or are there any specific that have to be remembered when working with the bot, especially regarding the EIPs?

**Micah Zoltu**  07:04
Everything that's a problem with the bot should be filed in for the merge bot at least. We had a lot of trouble - Alita's been working on it, keep trying different things, trying to fix it. And they keep having problems. The EIP bot repository should have a number of issues. That is where we track all the little problems.

**Shashank Yalamanchi**  07:24
 Okay, makes sense.

**Micah Zoltu**  07:27
So Ethereum/EIPbot, and then if you look through the issues, there are only a few left. So yeah, a bug and a feature and an unknown.

**Shashank Yalamanchi**  07:43
Yeah, I think there's one persistent issue that we're having with Greg. they get Greg's username has been defined, and I think that specific bug hasn't been reproduced again. So I'll keep an eye on it. Because I haven't seen that bug being reproduced. So basically, that bug was, I think, Micah, you yourself pointed that out that Greg was being showed as the first-time contributor. And so maybe that was a bot, I guess, but I hadn't seen that bug in a while again. So but I'll keep an eye on it.

**Micah Zoltu**  08:17
What are you referring to? I'd forgotten. If you find it, send me the link.

**Pooja Ranjan**  08:29
I think that was a long back issue. And I am hoping that that must have been fixed by now. Because Greg is already added as an EIP Editor. So possibly, the bot would not recognize him at least as a new contributor. And that should not reappear.

**Micah Zoltu**  08:47
Oh, yeah, that one. I think Alita fixed that one.

**Shashank Yalamanchi**  08:49
Yep, yep.

**Pooja Ranjan**  08:50
Yeah, and other than that, there are a couple of more open issues. I have shared the link here in the chat, so you can visit that. And you can also look into the history of earlier bugs. Those were fixed by Alita. And maybe it will help you understand what kind of issues are generally faced by those working on the bots.

**Micah Zoltu**  09:14
And for the validators, so those issues are related to the merge bot. For the validator bot, there's lots of room for improvement. There's a number of things that I manually review that could easily be validated, like making sure the "Discussion to" link goes to Ethereum Magicians and making sure that the EIPs that are dependencies of the EIP in question are in the appropriate state to be dispenses. A Final EIP should not depend on a Draft EIP. That bot could very easily say, "Hey, this can't be merged until you move those other ones forward first." Circular dependency's another one. You can't have EIP 5 dependent on 4 and 4 depend on 5. It's got to be the one way. Lots of little things like that. So if someone has a desire to work in Rust, then the validator definitely has room for improvement.

**Shashank Yalamanchi**  10:21
Yeah, there was this one open issue that I'd like to pick it up, because I couldn't find time to do because I got sick. So I'll pick it up and also try to get into that part. So my current process to understand the bots, and any information that I can find, I can find us reading the code, understanding the amplified context as to why this specific merge happened, or why this chain was introduced. So that kind of helps. But yeah, it's taking a bit of time. But yeah, the code aspect of how the workflow is happening and stuff like that, that I kind of understand. But there are a couple of things that are still being done manually, although the bot was supposed to do it, provided that bot already had that. The automatic sometimes doesn't happen, like you have to close and reopen the chute to make it automatic or something like that. So I might have to talk to Alita once.

**Micah Zoltu**  11:29
Alita has been fighting with the auto merge sometimes not working. For three months, we tried three or four different tools, tool suites. She's optimistic, but I think also at the same time with a good dose of reality behind her that the newest one, Kodiak, will work more reliably. So we'll see. We just got that one set up.

**Shashank Yalamanchi**  11:56
Alright, makes sense. Other than that, it's fine. So hopefully, by the end of the week, I should have a bit of a small document so that anybody who wants to pick up an EIP bot issue can kind of understand what's happening exactly, at least the workflow part. Maybe not the entire details, because it just takes a lot of context to understand.

**Pooja Ranjan**  12:25
Yep. Thank you, I think it's going to be a learning curve for everyone joining here for the first time because Alita has actually contributed in building the bot, so she has a better understanding of it. And with some of the documentation, and maybe looking into the process flow would be easier for new people to join and start contributing more. Well, I appreciate you working on documenting some of that stuff. That could be very helpful. Thank you.

## 1b. [EIP bot - GitHub-actions bot greeting Pull Requests](https://youtu.be/0oW6n9yuwoU?t=781)

Some of the next sub items that I have added here is GitHub action bots creating pull requests. It was mentioned by Micah on the Discord. And I remember that in one of the EIPIP meetings, we discussed we should have a greeter bot for letting people know who are creating the issue for the first time, even if it is not for the first time, even if it is just that they showed up and they are trying to create an issue on EIP GitHub and that is related to general EIP discussion, they should be moved to the Fellowship of Ethereum Magicians. It looks like the fix that Alita worked accidentally triggered for both pull requests and the issues. So that looks like a small fix, and we might want to deactivate that, just close that the greeter bot gets activated only for the issue section, not for the pull request. Is my understanding correct, Micah, that was the concern here?

**Micah Zoltu**  14:11
That is what I thought we agreed to but I also forget many things, so if that is not accurate, someone please correct me.

**Pooja Ranjan**  14:21
Based on the statement that the bot is reflecting, it appears to be that way, because it says that if this issue was created as a "Discussion to," so in my understanding is it is mostly for the issue section. Definitely we'd like to go back and check and if that is correct, then we can just have a small fix here to get this deactivated.

**Shashank Yalamanchi**  14:45
So that workflow currently runs for both the issue and the pull request.

**Pooja Ranjan**  14:49
Right, but it has to be just for issues, not for pull request.

**Shashank Yalamanchi**  14:58
Okay, so what would be the reasoning for not having the greeting message for the pull request?

**Pooja Ranjan**  15:08
Because that message simply states that if you are creating this issue for "Discussion to" for an EIP, please create a thread for Fellowship of Ethereum Magicians. And that's just a simple one-liner message. And it has nothing to do with the pull request.

**Shashank Yalamanchi**  15:27
Okay, makes sense.

**Micah Zoltu**  15:29
More generally, we don't have a problem with people incorrectly submitting pull requests. We do have a problem with people incorrectly submitting issues.

**Shashank Yalamanchi**  15:38
Got it.

**Sam Wilson**
Does the bot actually catch that as like a failed issue in the PRs?

**Micah Zoltu**  15:46
What do you mean?

**Sam Wilson**
Like if somebody puts a link in the discussions to a GitHub issue, does it flag it as invalid?

**Micah Zoltu**  15:52
No, that is something that would be great if someone wants to take up if you love Rust. The validator bot is written in Rust, and it should be an easy thing to add.

**Pooja Ranjan**  16:05
So by validator bot, you mean the one that is run by Matt right now like the EIP V? Or is it a different one?

**Micah Zoltu**  16:14
I don't know who runs it. The most recent version of it was written by Matt. You know who runs it now?

**Pooja Ranjan**  16:22
No, what I meant by that, like these issues, we can probably go and create issues over there, and then start sharing the link for people to come forward and work on those issues. I just wanted to make sure - where do we want to create these issues?

**Micah Zoltu**  16:41
Elevations things I would assume would go on the EIP validator repository and things with the auto merger and the greeter and things everything else should probably go on the EIP bot repository. At some point in the future, it would be nice, perhaps, if those were consolidated, but at least for now, that seems to make the most sense.

**Pooja Ranjan**  17:01
That makes a lot of sense. Alright, so moving on.

## 1c. [Issue with the auto merger bot, any alternate proposal Ref: Discord](https://youtu.be/0oW6n9yuwoU?t=1030)

The last item here was issue with the auto merger bot. I suppose Alita is looking for any alternate proposal. And as Micah also mentioned earlier, if someone has any suggestions, the merger bot is something that people are struggling with. If you can help with that, please reach out to us, anyone on the Discord, the EIP editors or the Cat Herders team.

## 2. [The state of Execution specs. & an introduction to the proposal for Core EIP standardization process.](https://youtu.be/0oW6n9yuwoU?t=1056)
The next item here is the state of Execution specs and an introduction to the proposal for Core EIP standardization process. So as we know, this is not a new item for the EIPIP meeting, as the execution specs repository itself is the result of discussion in the past EIPIP meetings. At present, the Quill team is working on documenting specs for application clients, I suppose in Python. And the Cat Herders always want to support the work and communicate it to the rest of the community. So we hope to have Sam Wilson talking about the updates. And also based on the progress, maybe we can start discussing an alternate approach for the standardization of core EIPs. So, Sam, if you would like to speak?

Sam Wilson
How's my audio? Is it alright? I'm using a different headset today.

**Pooja Ranjan**  18:34
Perfect.

**Sam Wilson**  18:34
Cool.

**Micah Zoltu**  18:35
As beautiful as always.

**Sam Wilson**  18:39
Back-handed compliments. Alright, so I don't know how closely everybody's been following the execution specs, but it's basically just a Python reimplementation of the yellow paper. Peter and Boyeth have just put up the PR for Spurious Dragon. So we're slowly but surely catching up to mainnet. The documentation tools are pretty neat. You can go take a look at them. I'm not sure what kind of an update you're looking for on the actual progress. But yeah, we're getting there. As for the actual proposal for how we're going to do EIPs in the future, there is that Peep an EIP video that probably goes over most of it. The short form is I'd like to replace the specification section for core EIPs with a diff into the  execution specs repository. And then we can collect all of the EIPS as markdown files inside that repository. And that way, we get to separate ERCs from EIPs, which I think Micah would probably appreciate. And we also get a bit of documentation that goes along with each code change in the same repository. And I think that's going to make it a lot nicer for following along when you're implementing a client.

**Pooja Ranjan**  20:06
Thank you. With the updates, I was just wondering if we should keep people updated on how far along we are. As you mentioned, that spurious dragon protocols are already up. That's really good progress. We have a few more upgrades to catch.

**Sam Wilson**  20:23
Just a few.

**Pooja Ranjan**  20:24
Yeah, not bad. So that is nice to know. And about the new proposal, I have shared the link in the chat for people who may have missed it. But it would be interesting to hear more thoughts on it. I know Micah and many others are very much interested into having a separate process. So it would be interesting to learn about what are the prep work that we can do, like Cat Herders can support with to just bring this proposal to the community and maybe actually help out. And using this, not for the merge, of course, after merge, whatever, if it is Shanghai or whatever it is, if there is any thought on that.

**Sam Wilson**  21:08
I mean, I think coming up with how we want EIPs to look like when they're incorporated into that repository would be a great step.

**Micah Zoltu**  21:18
Six feet underground?

**Shashank Yalamanchi**  21:20
Well, you just don't want any English description whatsoever? You just want Python?

**Micah Zoltu**  21:24
That's right. English language has been failing me for the last 40 years. I'm done with it.

**Sam Wilson**  21:30
All right. All right. We'll migrate off that. If you're a Lodge Fan fan, then we can use that.

**Micah Zoltu**  21:38
Okay.

**Sam Wilson**  21:39
Yeah, so I think, yeah, that'd be a great start is just playing around with ideas for how we want the EIPs to look and what kind of structure we want for them. Obviously thinking about how the bots are going to have to change to enforce whatever constraints we want on the new repository. Yeah, and obviously, just socializing the idea of changing where we look for EIPs and maybe getting feedback from CoreDevs on, you know, do they think it's useful to be pinged. Because  I think we're far enough along in the specs project that you can look at it and be like, "this is a good idea," or, "this is not useful" as a CoreDev. And I think we should start getting that kind of feedback as soon as we can. Yeah, those are kind of my thoughts.

**Micah Zoltu**  22:20
If someone wanted to - let's say we live in the future, and all we have is the specs repo. And someone heard about EIP, I don't know, 151 or something, and they wanted to go look it up? What would that look like? And specifically choosing an EIP that is in the past? Like something that currently is the oldie-type EIP? Do we have any ideas of how we might be able to port those over somehow?

**Sam Wilson**  22:53
I think the goal would be to have all of EIPs ported into the same format as the the new EIPs.

**Micah Zoltu**  23:07
For Core EIPs, specifically, right?

**Sam Wilson**  23:08
Yeah, exactly. Yeah. ERCs, you really can't represent in the same repository.

**Micah Zoltu**  23:15
Yeah. And so what what do you imagine that would look like in your perfect world?

**Sam Wilson**  23:20
Okay, so I think the way I'd want it organized is... So it's hard to separate an EIP out from the fork it was in. But I think you should be able to get a decent idea from the diff between the fork or the previous fork, which we generate, and the the text document that describes the changes. And that's probably how we're going to have to do it.

**Micah Zoltu**  23:48
Okay, so you're thinking that, along with each fork, there will be a text document that will describe the changes.

**Sam Wilson**  23:56
Each EIP would have its own text document, and then each text document would have to describe what fork it belongs to.

**Micah Zoltu**  24:04
Oh, I see. So you would have, like, an EIP 151 document that describes the change and then would link to the diff, or the change was included for the actual specification part?

**Sam Wilson**  24:19
So that'll be a lot easier in future EIPs when we have the process formalized, but for older ones, I think it's just going to have to be like all of the EIPs in a fork are in one diff, because it's hard to maintain individual diffs per EIP. Yeah, like even maintaining diffs per fork is proving to be challenging, but yeah. I can actually show you what one of those looks like. Give me one sec. So we want something in Tangerine Whistle. What was in Tangerine Whistle? That was the DOS protection if I remember correctly, right?

**Micah Zoltu**  25:06
No idea.

**Sam Wilson**  25:08
Come on. You guys are supposed to be experts on this.

**Micah Zoltu**  25:12
I'm a noob. I don't know anything before London. Before Berlin. Nothing before Berlin for me.

**Sam Wilson**  25:20
So I'll put this in the chat here. So this is actually - could you share my screen? That's even better. Yeah, I cannot share my screen. So sorry.

**Pooja Ranjan**  25:28
Just give me just give me a second.

**Sam Wilson**  25:30
Oh, it's not your fault. It's mine. I'm in. I'm in Wayland. So I can't share my screen with Zoom. But yeah, so you can actually take a look at what those changes look like in the render documents. And this is something we're working on, you know, improving and making more readable, but I think it's coming along nicely.

**Pooja Ranjan**  25:57
So if I understand correctly, the idea here is to have all the earlier EIPs that went into one of the earlier folks to be documented in one diff. And for the upcoming EIPs, which are to be considered for upgrade, they will have their separate diff. And in that, other than the the specs, there will be a separate .TXT file, which will contain other information, whether or not they go into the upgrade, like it is a separate thing. But we will have one text document for every proposal that is being proposed for upcoming upgrades.

**Sam Wilson**  26:35
Exactly, yeah. And then, I kind of imagined the way it'll be developed for an upcoming fork will be every EIP will be developed in its own branch. And then we'll be generating the documentation from all of those branches merged. So you can kind of see what the next hard fork is going to look like. But then when the actual hard fork is decided and made, all of those things will be merged. And you'll be able to link to each commit where those EIPs were merged.

**Pooja Ranjan**  27:02
Yeah. Definitely sounds interesting. It will be more interesting to actually get this implemented. I understand we are at the very earliest stages, but having this discussion at least giving up a high level picture of what is being imagined here. Maybe in the upcoming meetings, we can try to have something documented, and then think more about it and then see how it comes up to be.

**Sam Wilson**  27:31
Yeah, that sounds about right.

**Pooja Ranjan**  27:37
Thank you. Thank you for that update. And yeah, anyone has any question comment before we move on to the next one? If not, we'll try to keep this item like, if not, in every meeting, maybe in alternate meetings to at least kind of reviving this. So people should be aware of this new process and the process that is being proposed even if it is not finalized. We can start collecting feedback and discuss feedbacks in these meetings to kind of formalize the process.

## 3. [EIPs Insight - Monthly EIPs status reporting.](https://youtu.be/0oW6n9yuwoU?t=1695)

Moving on, the next item is EIPs Insight. That's a monthly EIP status reporting update. Since the last update, there is one new proposal added in the past two weeks, and now we have a total of four new EIPs in Draft status. And there are three EIPs under Review status: EIP 4200, EIP 4626, and EIP 3668. Obviously, EIP 3668 is no more in Review, but it is listed here in Review status because it changed it's status in the month of January itself. For that particular proposal, that has now completed its Last Call, and we should be expecting a pull request to move it to the Final status very soon by the author. The last call period for three of the proposals which were earlier in the Last Call is now over. So ideally, all the proposals are eligible to be moved to the Final status. 368 is one of them. And the other two proposals are EIP 3448 and EIP 3607. There is one additional proposal which is resurrected from Stagnant to Review, and the number is EIP 2980. That is Swiss compliant as a token, and there was already one proposal which was resurrected from the now Stagnant status. Technically, we have more than three. We should have five in the Review status. But again, one has completed the Last Call, so only four left in the Review status. There are four proposals which moved to Stagnant because they were inactive. And there were a few minor edits to the final proposal, please check out the EIP Insight for January to learn more about the EIPs activities. Yeah, I see that comment from Micah, and it is really good. These updates from Sam give everyone, not only Micah, hope for a brighter future for a reason. Not to just live, just to be a part of this community as well. Thank you, Sam.

## 4. [EIP editor apprenticeship meeting](https://youtu.be/0oW6n9yuwoU?t=1845)

Moving on, the next item listed here is EIP editor apprenticeship meeting. We had this meeting yesterday. There were reviews on some of the pull requests which were submitted over the past two weeks. The highlight of the meetings, including some of the pull requests, as those were discussed yesterday, are added to the summary section, which is available in the comment. To add the agenda to the meeting, we can expect at least one more proposal moving to the Final status. That is EIP 1271. It's an old proposal, and it's a big win for the team, because this was a long due proposal to be moved into the Final status. There were some edits and recommendation to other pull requests. One of those was EIP 2982, which is an informational EIP for certainty phase zero. Please check out the video and the summary link in the EIP meeting agenda for the details of the discussion that happened in the EIP editor's apprenticeship meeting. And this meeting is bi-weekly. So we would be expecting the next one, two weeks on Tuesday. That's mostly what was listed here on the agenda.

## 5. [5. Review action items from the previous meeting](https://youtu.be/0oW6n9yuwoU?t=1930)

And the last item is review action items from the previous meeting. So from the previous meeting, as we can see, there are only two: Shashank will be working on documenting the EIP bot improvement. He is already working, and we should be having something added to the maybe README file or in a doc for new people to contribute to. And I did chat with William in Trident. And unfortunately, I did not receive any response yet. But for some of the questions, those were asked in the earlier meeting. If we get any response, we'll try to add them in the upcoming meeting. To address them, of course, and I'm also talking to the DevOps team to finish the migration. It is still not done for the EIPV that we are discussing from past few meetings. I will check back with the team one more time. And let's see, we hope to have this migration done to the Ethereum GitHub repository, I hope by the next meeting. I don't know yet. I'm just waiting on the response. So that's all anyone has anything to bring up. The EIPIP meeting seems to be a little shorter, but I think we are trying to cover the basis on whatever is going on, and if anyone has any question or concern related to the process, and they would like to be addressed. So if you are one and you want to contribute or if you have questions, please leave a comment to the agenda so we can pick it up and we can bring it to the next meeting. Well, thank you everyone for your time. Hope to see you guys around in two weeks. We'll try to be on the same call. Have a good one, everyone.

# Attendees

* Brent Allsop
* Guru
* Jim Bennett
* Jose's iPhone
* lightclient
* Micah Zoltu
* Pooja Ranjan(Host)
* Sam Wilson
* Shashank Yalamanchi
* Texas Farmer



# Date for Next Meeting: February 9 at 1500 UTC
