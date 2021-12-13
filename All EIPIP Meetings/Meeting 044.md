EIPIP Meeting 44 Notes
# EIPIP Meeting 44 Notes
## Meeting Date/Time: Wednesday 17 November at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/91)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=e1fTsIMa4bE)
### Moderator: **Pooja Ranjan**
### Notes: Jim Bennett

----
## DECISION ITEMS

**DECISION 44.1**: Add identifying a new EIP as a feature request to the EIP bot[see 2:09](https://youtu.be/e1fTsIMa4bE?t=129)

**DECISION 44.2**: Create a PR to disallow creating new discussion issues outside of Fellowship of Ethereum Magicians. [see 15:49](https://youtu.be/e1fTsIMa4bE?t=2290)

**DECISION 44.3**: Create a pull request to standardize referring to statuses in EIP 1 with a capital letter first and then lowercase after that. [see 38:10](https://youtu.be/fKQVb-s0Tzs?t=1959)

**Pooja Ranjan**
All right. Welcome to EIPIP meeting 44. I have shared [the agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/91) in chat.

## AGENDA

## 1. [Add Labels to PRs](https://youtu.be/e1fTsIMa4bE?t=9)

So the first item that we have added here is [Add Labels to PRs](https://youtu.be/e1fTsIMa4bE?t=9). This was brought up by Greg Nanterre and Greg Coleman, but the one with chains if you mentioned it in the EIP editing Discord channel. I was also interested in sorting these PRs and once requested to get that triaging permission. But it was brought to our attention that triaging permission is not possible with the present Ethereum GitHub for so many reasons. So it was dropped. But I really like the idea of flightline of having it done by the bot. I was hoping for some thoughts on that. I don't see Alita on the call. But if anyone else has any thoughts, like, is it going to be really difficult?

**Micah Zoltu**  1:02  
I'm a fan of the bot doing everything. Of course, it takes engineering to do it. So you decide whether it's worth it or not. So for purely status change, it should be relatively easy. So the problem is analyzing a diff is non-trivial. It's possible, but it's a bit of work to analyze a diff and identify what changed within a PR. So from an engineering standpoint, I think it's going to be a good amount of work. And relative to the benefits, it's not obvious that it would be worth it, at least not at the top of the list. There are other things I think it'd be more beneficial to have the bot to. For new EIP, that one could be done automatically pretty easily. Relatively easily. The other two, though, I think are gonna require a bit of work.

**Pooja Ranjan**  2:09  
Yeah, I was thinking that new would be easier, relatively. Okay, I will go ahead and add that as a feature request for the EIP bot. And obviously, we'll try to prioritize the tasks that are already listed there. And let's hope to keep it in the list.

**Micah Zoltu**  2:36  
Yeah, I'm a big fan of just having a backlog of all the things that we would like to see the bot do. And then whether we get to them or not is a separate conversation.

**Pooja Ranjan**  2:47  
Sounds good. All right.

## 2. [General consensus for closing the "Discussion to " issues](https://youtu.be/e1fTsIMa4bE?t=177)

Moving on, the next one is [General Consensus for Closing the "Discussion to" issues](https://youtu.be/e1fTsIMa4bE?t=178). So I have referred to three lengths here. So I'm a little lost here, maybe I missed some important piece of information. I thought the group came to an agreement that we will try to enforce a Fellowship of Ethereum Magicians as the only discussion group place. And the bot was even updated accordingly to provide a message whenever any issue or new issue is created, mentioning that if you are creating this issue for discussion, please close it and open it at FEM. But recently, I came across a new issue, and that is marked as "Discussion to". So I was wondering if by any chance anyone has any information that something may have changed.

**Micah Zoltu**  3:52  
So if I remember correctly, the conclusion we came to was that we would strongly recommend Ethereum Magicians, but we wouldn't strictly enforce it. So you tell people that you should really use Ethereum Magicians unless you have a very good reason not to, whatever that might be. We didn't really specify, but the idea is that issues are still acceptable, but frowned upon. Given that, there are some people who feel very strongly that they want to create an issue discussion, not an Ethereum Magicians discussion, and so they do. And separately, we also have discussions from a long time ago. So before we made that change, there's lots of discussion issues for that. And so even if we do strictly enforce that, we still have to decide what to do about discussion issues going for the old stuff.

**Pooja Ranjan**  4:45  
Oh, well, I agree. Yeah, that was a strong recommendation. And definitely it wasn't enforced, though. The idea was that slowly we can move people, unless they have a very strong reason for bringing it back to the issue section. For older issues, I don't know, when we started running the bot to make it, still the idea was to close the issues which which are not an active discussion. However, if that proposal is on the GitHub repository, the "Discussion to" link is available there, even if the issue is closed, and that will always accept the issues. So that is something and if people want to keep it open forever, it definitely will get lost, because nobody scrolls back like 10 or 12 pages to find a particular issue to comment on that. But with the help of the link added to the proposal, it is way easier to do. So I think the idea was to stop getting more "Discussion to" issues created. So we can use that particular channel for the useful issues that people would like to generally discuss. I mean, again, this is not up to me, because I'm neither the author nor the EIP editor, but I was just trying to get a clearer picture to the community. So they would know what to do and where to go. So if we are recommending from even with the help of bot that you should be going and opening a "Discussion to" link at FEM and at the same time, we are allowing people to have this open here, I don't think we will be at a place where where we can actually share the information in the right way. So it will be again the same thing where we started.

**Micah Zoltu**  6:37  
Unfortunately, Alex isn't here. He's the primary proponent of keeping discussion issues open. Matt, do you want to try to steel man his argument?

**lightclient**  7:01  
I don't really know what his argument is to steel man. But my argument would be why? I don't really see the argument to do anything. And so I just the argument is it's acceptable right now, I would be in favor of saying you can no longer use issues, but ones that exist, I don't see a reason to change that or close them.

**Micah Zoltu**  8:22  
I think the idea is we want to have the GitHub issues list be an actually useful list.

**lightclient**  8:30  
But won't they fairly quickly become useful if we just stop allowing people to create new issues that are discussion areas?

**Pooja Ranjan**  8:42  
Yeah, that was the idea of when we started using bots.

**lightclient**
So we don't necessarily have to have to clean all of the issues for the issues to become useful. We just have to stop letting irrelevant issues come into place. Of course, there's still gonna be a few dozen issues scattered in history that are always going to be difficult to find, but I think that this is like a much more reasonable path to having useful issues and clearing all of the issues that exist. I think that's a really large task, and we're going to upset people who oppose their issues.

**Micah Zoltu**  10:13  
So my counter argument is twofold. One, there is value in having the issues list be actually actionable things. Because when you look at GitHub, and you see there are 41 open pull requests, that is much more actionable than 500 open pull requests like we used to have. Similarly with issues, if you see 450 issues, no one's gonna read through those. Whereas if you have 50 issues, some new apprentice might be like, "No, I'm gonna go through the issue and see if it's something I can handle or something I can do" if they're  actually actionable items. The second one is that I would tentatively argue this: no one in their right mind finds a discussion link for an EIP by going to the issues list and looking for the EIP. They always start with the EIP and get linked to it. And so closed or open is irrelevant. And so there's no downside to closed. And there's a very minor upside, which is the issues list.

**lightclient**  11:09  
The downside to closed is that it looks like the discussion has been closed. And that may mean that you do not comment. That's my only concern for having them closed. Otherwise, I think you're right, nobody goes to the issue.

**Micah Zoltu**  11:30  
Your concern is just the kind of psychological effect of closed versus open.

**lightclient**  11:34  
And discussion is complete now. I'm mildly against closing the old issues for what it's worth. It's not something I'm going to lose sleep over.

**Pooja Ranjan**  12:14  
So I suppose we are actually talking about two things here. One, closing the old issues, and the second one, allowing people to open the new issues. So if we talk about allowing people to open new discussions, is there a general agreement that we can try to request that the author, assuming that he does not have very strong reason, to go ahead with issues and not go to the FEM. To start the "Discussion to" link? I'm especially referring to issue number 4431  that I think has been started just 10 days ago, and it's fairly new, and there is not much of a discussion. And I don't know why, but the bot did not provide a message saying that you should go ahead and start discussing at FEM, though it was designed that way.

**lightclient**
I just don't think we've made it an absolute requirement. Unless we have and I misremember.

**Micah Zoltu**  13:24  
We didn't. In EIP 1, we might have updated it.

**Pooja Ranjan**  13:32  
At some places, not all. Because I remember adding it somewhere that it is highly recommended. But when I was checking it today, I found that there are other mentions, and there, they have this permission to open it at issues. So I was wondering if we can unify that EIP 1 and do it if all the editors are on board? If not, then we have to leave it the way.

**lightclient**
I think whether or not we close the issues, you should stop letting people create new ones for discussion threads. We're never going to have that useful of issues list if that's the case.

**Micah Zoltu**  14:18  
Yeah, I generally am in agreement. The one downside is just that telling people, "Hey, go create an account at this other place, just so you can do something... it doesn't have GitHub signin?

**lightclient**  14:36  
It does have GitHub signin.

**Micah Zoltu**  14:38  
And does it ask you for a bunch of ridiculous permissions to do so, like a lot of bases do?

**lightclient**  14:43  
I don't recall it asking you for anything other than potentially your email, but also it may not even ask for email.

**Pooja Ranjan**  14:57  
One thing that I want to mention here is generally people who are creating issues or generally they are trying to add a new proposal, they are already there on FEM. It's rare, I mean, definitely, I haven't seen in my experience that someone is not there on FEM and they are trying to do something here on GitHub. So I don't think

**lightclient**  15:17  
If they're not, maybe it's a good filter.

**Pooja Ranjan**  15:32  
I'm not sure if we can come to a conclusion on this right now, because I know a strong argument is coming from Axcic, and he isn't in the call. So maybe I will try to write something.

**lightclient**
So put a PR and change it and discuss it with him on the PR.

**Pooja Ranjan**  15:48  
That makes sense. I'll go ahead and do that. If it is fine by this group to make it highly recommended, I will create a pull request to make all the possible changes in EIP 1 where we are suggesting where to open the "Discussion to"" link.

**lightclient**
But you may also want to update the template.

**Pooja Ranjan**
Oh, yes, I can do that too.

## 3. [ EIP editor apprenticeship meeting highlights](https://youtu.be/e1fTsIMa4bE?t=987)

Okay. Okay, now let's move on to the next one. So the next one is [EIP editors apprenticeship meeting](https://youtu.be/e1fTsIMa4bE?t=987). The meeting went well. Of course, we had a decent attendance of new contributors. So thanks to Tim Baker for generating the momentum, and help us getting people to reach us on the Discord channel. And many thanks to Mac the net for answering questions from the group. There were a lot of questions. Just in short, in the meeting yesterday, we had a quick introduction of possible contributors for their background. I presented a 10 minute overview of EIP type category and the present process. Matt took the stream of questions as well with revealing a pull request, which is now much as an EIP in draft status. I hope most of the questions that we could have expected were answered in that meeting. And the recording is also available now on Cat Herders YouTube for anyone interested to follow what what actually happened in the meeting. So we have shared all this information and if someone is still having a question or they would want to reach us, please reach us on ECH Discord EIP Editors channel to share your question. We have EIP editors on the Discord. So we hope that your questions will be answered, and we can plan the next meeting in two weeks. If you would like to add anything. Did I miss out on anything?

**lightclient**  18:07  
Two weeks. Hold on.  I don't think I will be available in two weeks, actually. I think that Tuesday I have something going on all day. But we can figure it out.

**Pooja Ranjan**  18:27  
Yeah, we can do it. I think I see some comments here on the chat. We'll get back to that. Let's finish up the agenda item first because those are really low in number. So we are almost on the last item listed on the agenda for today. It's an EIP insight, the monthly EIP status reporting. I have updated the insight for November after 15 November. So far we have three new drafts. One EIP is withdrawn and two have been moved to Stagnant, and three EIPs have been resurrected from this Stagnant status. The good news is EIP 64 and 65 are finally in the Last Call with the review period ending on November 19. There are a couple of non normative changes to final EIPs - EIP 2681 and EIB 2124 And there are a few other improvements to EIP 1. That's all about EIP insight, and the link is available in the agenda.  

**lightclient**  19:58  
Nice.

**Pooja Ranjan**  20:08  
There is one thing that I wanted to bring here, before I actually make a pull request for that. In EIP 1, the bibliography section. If we can check it out, it looks like something is wrong with the for**lightclient**ing because I don't see any text over there. Whenever looking into the raw draft, it is available. Is it an error, or it is supposed to be that?

**lightclient**  20:35  
Which one? I'm checking.

**Pooja Ranjan**  20:37  
The bibliography section, it's done.

**Micah Zoltu**  20:42  
Looks like it's just missing.

**Pooja Ranjan**  20:46  
Actually, I found the data is already there.

**Micah Zoltu**  20:52  
Let's see. I think it's because markdown is recognizing this is just a link lists. And it is using it to backfill links.

**Pooja Ranjan**  21:10  
When I was looking into the .MD file, it looked like to me the way that it should be for**lightclient**ed is not correct.

**Micah Zoltu**  21:18  
So the markdown render sees that list of links and it's saying, "Hey, these are just link references." And then elsewhere in the document where that link shows up, it will replace - like if you do square bracket Dev P2P square bracket somewhere else in the document and replace that in rendering with that link but doesn't display that below. So you can just get rid of the header and put that. I'm not personally a fan of this style of markdown, but some people like it. I prefer just inline links. So if you search the document, the raw version, a document for Dev P2P, you'll find it in two places- one up in the EIP types section. And just as square bracket P2P square bracket, and that's it. And then you also find it down in the bibliography. If you look at the rendered version, and you go to the EIP type section, and you hover over the Dev P2P link, you'll notice that it links to github.com/ethereum/wiki/wiki/wpwireprotocol. And so what's happening is those links down there at the bottom are backfilling to any place that just uses the square bracket notation. It's a feature of markdown that is doing this. So they're not supposed to render on the page at all. It's not supposed to be a part of the document that renders visibly. So we have two options. One, we could just stop doing the bibliography style of links. That's my personal preference. So that means where you see square brack P2P squared bracket elsewhere in the document, you change that to square bracket Dev P2P p2p square bracket, open parentheses then link, they do that instead of just P2P instead of that. You're the first one to the second one, and you can get rid of the section entirely. But someone will just need to go through and update all the links throughout. The other option is just delete the bibliography subheading so it doesn't look weird when it's rendered and just leave the link list and maybe put it at the very end of the document after the copyright. I don't know. My preference is to just not use that style of markdown links. I find it confusing. But I'm not that passionate.

**Pooja Ranjan**  23:59  
Any thoughts, lightclient?

**Pooja Ranjan**  
I don't mind.

**Pooja Ranjan**  24:19  
So if I understand correctly, a session is required because we have been using this style for providing the links at certain places in the document. And we cannot simply remove this section unless we have these things listed somewhere down.

**Micah Zoltu**  24:51  
So we can delete the section. Someone just needs to go through and do the work to do so. So right now throughout the document, there's a mix of linking styles. In some places, we link with title. Some places we use that format, and some places we just lose. we just use that format - the square bracket followed by parentheses. That one is an inline link. And so that works just like you'd expect. The title will be what you see when it's rendered. And the link in advance sees what happened. You click on it for the other format, where it's just square bracket, title, square bracket, and there's no parentheses afterwards. That one refers to a link that is somewhere else on the page. So the markdown render will then go through the page and look for somewhere that has something in the format of title:. But it will look for that somewhere else in the page. And then when it renders, it will fill in the link. So if we want to delete that section, somebody needs to go through and convert all the links that are just square bracket links without the parentheses to the ones that have the square bracket an parentheses. That make sense?

**Pooja Ranjan**  26:13  
Yeah, it does.  I'm just trying to think over here is it definitely is helping. And when it was written for the first time, it might have been very helpful, because they don't have to repeat adding the link everywhere. And if someone has to go do that, that shouldn't be a problem. Because that is going to be just a one time task to be done. And people can start following that as a practice for anything new to be added here. I'm just wondering if that should not be something heavily debated. So before doing that, maybe I can create an issue or maybe a pull request and then see what is the general opinion there. Because this seems like a big change. Because people who have written it initially might have considered not mentioning it again, and again, maybe for so many reasons, just removing it.

**Micah Zoltu**  27:06  
So that's the theory behind it. In this case, I believe that every single one of those links is used only once. So it didn't actually work out that way. I did a quick check, and so far, I have found no duplicates in my quick spot check. They're all linked exactly once without the link in exactly once down the bibliography section. And none of them are reused. And so the argument to be made is the reason people say this is a better way. But in practice, it doesn't appear to actually be benefiting us at all. Now, in fact, some of them are in the bibliography and don't exist anywhere else even in the document. Yeah, so the pull request link is in the bibliography, but it doesn't exist anywhere in the page anymore. And so the problem with those sorts of links is it's very easy when you edit the document to just like delete a line. And then you don't realize that there was a bibliography link that needs to be deleted as well, which is why I prefer the inline.

**Pooja Ranjan**  28:08  
Alright, I can take up on this task. Maybe I'll get some time and look into what all links need to be updated, whatever is referred in the document. And if these are not like so many places, then definitely we can go ahead and do that. Okay. That's on that. I see on that comment you have mentioned about some ideas? Do you want to speak for it or not?

**Spore_Druid_Bray**
Yeah, so it's just something that didn't get that much attention back in the R&D Discord. I was wondering if anyone read that and had some thoughts there, but we can discuss it another time. Or maybe just the general vibe is just say you have very complex things, step[s for EIPs that I don't know.

**Micah Zoltu**  28:59  
We definitely have talked about it and thought about it a lot. Currently, Sam and others, Sam fl is working on an executable spec for Ethereum. The idea is basically a version of Ethereum written explicitly for being readable, not for being performant or usable. And so it likely - in fact, we know it will not be able to run in the real world. It's written in Python; it is unoptimized. You will not be able to sync mainnet off it; you will not gonna run it, but it will pass all the tests and it is a functional client. And again, the goal here is it's written to be incredibly readable. The idea is in the future, hopefully near future, we'll see how fast they can get that done. Instead of having the yellow paper which is both unreadable and non-executable, we will have the actual spec which people can read and execute. And so when we do changes, we can just make a PR, essentially a diff against that external spec and say "this is the change." And the reason this is valuable is things like EIP 1559, for example, we basically had to kind of redefine a bunch of stuff in the specification section of that. So that way, the change made sense. In order to explain the change, we had to first explain the existing system. And this is very tedious and annoying, and it leads to bugs and whatnot. So that's the idea is an executable spec in the future. When that lands, the question then becomes, do we still use EIPs or do we not use EIPs? And there are definitely several different camps of people in this discussion. Tim's in the camp of he would like to keep the EIP process and have the EIPs maybe link out to a diff against the executable spec and the specifications section. Sam, I believe, wants to keep the certain sections of the EIPs such as security considerations, backward compatibility, rationale motivation, in an isolated document, but in the specs repo, so maybe in the form of, like, still a markdown document of some kind, and they would sit next to the change itself in some way. And then there's people like me who are on the far extreme. I would prefer to just say, keep all that information, because I consider it to be transient information. Keep that information in the PR that is goes along with the spec change, but don't retain it somewhere permanent. And so there's definitely lots of discussion on this. Lots of differing viewpoints and opinions. I think at the moment, I think we're always kind of waiting for the actual spec to be finished before we commit anything, because we want to wait and see how that turns out and wait to see structures and maybe try a few different things before going too hard on one solution. So does that answer your question or would you like to discuss it more?

**Spore_Druid_Bray**
Yeah. That's awesome. Is that Sam Wilson?

**Micah Zoltu**  32:11  
Yeah, Sam Wilson is the one I think Matt might know better. I think Sam is leading that charge.

**lightclient**  32:18  
Yeah, he is.

**Pooja Ranjan**  32:24  
Recently, Sam Wilson provided the latest on the execution layer specs that he is working on for documenting in Python, as well as he proposed his new idea of an EIP process that he thinks could be useful. But that's in thought phase right now. Probably, we'll keep on iterating and think what will be the better way or better approach to continue the EIP process once the spec is fully functional and people are out of the merge thing and start thinking in this direction.

**Micah Zoltu**  33:08  
Do you have a link to that Peep an EIP episode by chance?

**Pooja Ranjan**  33:11  
Yeah, I will send it to you.

**Micah Zoltu**  33:17  
I was gonna go watch it and then I think I got distracted with a bunch of other stuff and never did.

**Pooja Ranjan**  33:22  
No problem. I will share that with you. I'll email and I want to bring one last thing. Oh, okay. If we are done with this topic of Britain, did that answer your questions?

**Spore_Druid_Bray**
Yeah, that was awesome.

**Pooja Ranjan**  33:38  
Okay, thank you. So I just wanted to discuss one more thing before we can leave for today. It's just for for**lightclient**ing. I've seen that EIP 1, we try to refer status in different ways. Sometimes it is in running letters, sometimes it is in capital letter. So I was trying to think is it any value making it a standard that whenever we are referring to a status, it should be all caps and wherever it is where you're referring it to a word it can be in running. See for example, Review. Review is a review that we do for proposal, but Review is also a status, so when we are trying to refer it as a status and if we start using it as an all caps, that would help people to differentiate between what we were talking about. I mean, it's just my general thought. What do you guys think?

**Micah Zoltu**  34:33  
I find myself sometimes doing that. Just out of habit, I think for the same reason that you just described, I do it. It's kind of subconscious, and when I catch myself doing it, I correct and remove the all caps, but if everybody agrees to do all caps, I'm okay with it.

**lightclient**  34:53  
I don't really like all caps, personally.

**Micah Zoltu**  35:02  
Would you prefer all lowercase?

**lightclient**  35:09  
I guess I haven't thought about this very deeply. But it doesn't feel like the status needs to have more caps on it.

**Micah Zoltu**  35:17  
What about if we prepend it with an underscore? Would that make you feel better?

**lightclient**  35:21  
A 0X in front of it? You can 0X Final.

**Micah Zoltu**  35:31  
Sold.

**lightclient**  35:37  
I don't really care that much, but I don't really like all capital words.

**Micah Zoltu**  35:45  
So I think the differentiation between an official status and just discussing the general concept of something's in Review or something's in Draft is valuable. I do wonder, though, is it sufficient to just capitalize the first letter for the status? TThat follows normal English language conventions, where you consider it a proper noun, sort of.

**lightclient**  36:11  
Yeah, I would be more on board with that.

**Pooja Ranjan**  36:16  
Alright, because in the EIP 1,  at the moment, I see that it is a mix of both. Some places when we are writing it explaining the statuses, it is all caps and somwhere it is running, so.

**lightclient**  36:37  
I'd also be down with symposium backticks using lowercase.

**Pooja Ranjan**  36:46  
So are you recommending that wherever we find it on all caps, which it can be upgraded to lowercase, all lowercase, or just the first letter as capital?

**lightclient**  37:00  
I'm just proposing an alternative.

**Micah Zoltu**  37:03  
I think of those three, my personal favorite is uppercase first letter everywhere that we're referring to the actual state. If someone has a strong argument otherwise, I'm open to it, though. Not a hill I want to die on at all. It's not even really a hill I want to  fight on.

**Pooja Ranjan**  37:27  
It just came to my attention because sometimes in my general presentation, I talk about statuses. And I myself write it in both ways, sometimes running and sometimes in all caps. So was thinking to bring it to a standardization that I can follow it for myself. And that's why I wanted to bring it up to you guys.

**Micah Zoltu**  37:50  
So if no one has strong opinions and everybody's okay with just capital first letter, why don't we just go with that. It's in the middle of all lowercase and all caps. So it's a compromise, right?

**Pooja Ranjan**  38:10  
Okay, that can be the third pull request, because I see some some places that is all caps. So I can make a pull request to update that in EIP 1, too.

**Spore_Druid_Bray**
With multi letters, multi words, would it be the first letter of each word?

**Micah Zoltu**  38:26  
Yes. So Last Call is a good example of that one. Last Call is two words. And the L and the C are both capitals.

**Spore_Druid_Bray**
Sweet.

**Pooja Ranjan**  38:45  
All right. Sorry, you were saying something, Micah?

**Micah Zoltu**  38:53  
I said you're right. It is definitely inconsistent in this document. They use just about every form.

**Pooja Ranjan**  39:03  
No problem. I'll try to update it with whatever we agreed here. I hope that it's not something that people will oppose doing. Okay, let's move on to the last item. That's the action item from the last meeting. 43.1 is renamed Review Period to Last Call and to be added in EIP template. I saw a recent merge which suggests that is something different than Last Call and I don't want to debate on that if it is fine by everyone. So I think I saw the pull request where we have actually updated this particular feed, but it's not as Last Call and it's something different. It's Review Period Last Call or something?

**Micah Zoltu**  40:05  
Oh, yeah. We renamed Deadline, or Deadlines, whatever it was called.

**Pooja Ranjan**  40:13  
Yeah. Deadline. Yeah, I think it is.

**Micah Zoltu**  40:16  
Review Period End, maybe?

**Pooja Ranjan**  40:19  
Last Call or Last Call Deadline, something? I don't know. I mean, again, not a hill I would like to die on. But I just want to say that it has been updated. What was discussed was something different, but there is an update that might reflect that it's about the Last Call period, not the Review period.

**Micah Zoltu**  40:38  
I'm trying to understand something. You're talking about Alex's PR, right? Where he updated the template in EIP 1 to use Last Call Deadline?

**Pooja Ranjan**  40:58  
Yes. And the number is 4438.

**Micah Zoltu**  41:07  
This is in the midst of his race to 4444 with **lightclient**.

**Pooja Ranjan**  41:16  
Oh, sorry, yeah, I think **lightclient** updated it. Now's it renamed Review Period End to Last Call Deadline?

**Micah Zoltu**  41:26  
Yeah, that's fine. In our last video, if I remember correctly, no one cared what it was called. And we all agreed that the name could be better. And so I'm totally fine with the person who made the PR gets to decide. I think I even told someone that in Discord.

**Pooja Ranjan**  41:45  
Right, right. Yeah, I was just trying to make it a point that it has been updated. Now it's no more Review Period ending; it's reflecting the Last Call. Not exactly the same wording, but the field is updated now. And it should be better, making more clarity. All right. The next one is what it takes to be on the list of active editors. Oh, it's just a listing of it. 43.3 to agree on who gets mentioned in EIPs. I think, **Micah Zoltu**, you already have a merge that pull request there, right? EIP

**Micah Zoltu**  42:23  
Yeah, I think so.

**Pooja Ranjan**  42:25  
4390 And the next one is EIP registries. We are still looking for it. So if anyone is hearing this call, we are looking for a champion who can jump in the idea shared by Nick Johnson in the EIPs issue section. And if you're willing to put in time, please reach the EIP editors or the Cat Herders anywhere on the Discord channels. Last one here is Pooja to open an issue with EthBot repo to check the bot merge. I think the bot has merged the EIP 2070 that we were having issues with. And yeah, I think that's all from the action items from the last meeting. We have about five minutes left. Anyone want to bring up anything?

**Micah Zoltu**  43:20  
That's enough time for me to chastise **lightclient** on EIP number farming

**Pooja Ranjan**  43:27  
4444?

**lightclient**  43:29  
Yeah, it's actually pronounced "four fours." Yeah.

**Micah Zoltu**  43:36  
I'm very conflicted, because on the one hand I am a huge opponent to people in positions of power of using the rules. And I feel like those in power should be held to a far higher standard and punished far more severely than regular plebs who break the rules. On the other hand, I don't have the energy to actually give you a whipping.

**lightclient**  44:03  
I find it useful. PRs on the race to four four four four. Any pleb could have done that. If some pleb slides me, I would have accepted, and I would have waited till 55555. It just means that a lot more work would have been done in the meantime.

**Micah Zoltu**  44:20  
Note to self: next time I set up an alert, page me in the middle of the night. Wake me up if I see **lightclient** doing a lot of work. **lightclient** is way too productive today. Seems fishy.

**lightclient**  44:38  
What's the next nice looking number coming up?

**Pooja Ranjan**  44:48  
5k.

**Micah Zoltu**  44:53  
it's gonna be a doozy.

**Spore_Druid_Bray**
Actually, this might just be a real quick topic, but I've noticed at least for two ARCs or proposed ARCs, I think one was Diamond Standard, and I can't remember the other. They had subtypes and like an ABC version. Is there an official idea for the subtypes, like alphabet vs. numerals?

**Micah Zoltu**  45:17  
So EIP numbers are just numbers. So it's just gonna be a number from like, one to 10,000 or whatever. Now people can put whatever they want in the title, we generally leave that entirely up to the author. I discourage people from... so, I mean, there is only ERC 1155. There may also be ERC, you know, 7234, which may depend on 1155, or may be derived for 1155. But that is not ERC 1155. It is ERC 7234. If I saw someone referring to their EIP as another EIP number than what it is, I would probably step in and correct them. And if you see someone doing that in the EIPs repo, point it out to me, because that is definitely not acceptable, in my opinion. The numbering system exists for a reason. When I see what you just typed there, my gut is that someone's basically trying to use the marketing pull of 1155 in order to pump their own thing. And I'm very much not a fan of that. The numbering system should not be a marketing scheme. Its numbers are meant to be monotonically increasing and strictly for organizational purposes. Title is what you should go by. If you want a cool title, give your EIP a cool title. As much as I hate the Diamond Standard naming system, that's a cool title and it's nimble, and so he won't call it the Diamond Standard. So the short answer is you should not be naming any EIP that is not EIP 1155 as EIP 1155 dot something, nor should you name it ERC 1155 dot something.

**Spore_Druid_Bray**
Okay, I didn't got that clear across very clearly. I think it was more that I've counted at least two proposed ERCs is that there was some types within the document in some sense. It's like a stronger version, like three different versions within the same ERC. I can find the examples. I'm not sure. I found them before.

**Micah Zoltu**  47:39  
Yeah, I can imagine people doing that. Have you seen that, **lightclient**? You look at ERCs a lot more than I do these days. I also learned you don't actually read the ERCs when you edit them, so...

**lightclient**  47:52  
I read them once, the first time I edit them.

**Micah Zoltu**  47:54  
I'll have to think on how I feel about that.I feel like if you're going to have two standards, you should just have two standards. In the past, for core EIPs specifically, I strongly advocate to every single author that if you can break an EIP up into multiple IPs, you should. They go through smoother; they're easier to implement; people can choose whether to implement all or nothing or one or the other. From a communication standpoint, it's way easier. From a coordination standpoint, it's way easier. People should be writing very small IPs that do the least amount possible. It's similar to the general concept in software engineering, or if you're going to submit a change request, it should be as small as possible. And you submit multiple small change requests that are each individually useful and individually tested rather than one monolithic one, it just makes the process a lot easier. So I feel very similar for EIPs, that if you've got multiple standards within an EIP, that's a very strong signal to me that you really have multiple EIPs, so you should just create multiple EIPs. So yeah, I guess my answer is I don't have a strong opinion on the subnaming because I don't think people should be doing that or getting into thatr position in the first place where they need to set a name. But I probably wouldn't force that on anyone.

**Pooja Ranjan**  49:18  
I think this is something that has to be given by the EIP editor. So the author should not try to grab a number for himself or herself right in the first place. And when we are doing it with the help of a pull request or issue number, I don't think this kind of number system should exist in the first place.

**Micah Zoltu**  49:38  
Yes, in this case, what they're saying is that someone wrote an EIP, so let's say EIP 1234. And then within EIP 1234, it has two different standards defined and they're saying how do you refer to the two different standards? Do you do EIP 1234 dot A and dot B, or do you have 1234 dot 1 and dot two, or something else? My argument is you just have the EIP 1234 and EAP 1235.

**Pooja Ranjan**  50:05  
Whatever. Let's support your argument here. Because as you mentioned that you already have been advocating it for the core EIPs. And that turned out to be really good and it is helpful and implementation as planned is easy to implement. So I'm hoping that it would be helpful and even on the application side, if any developer wants to pick up only one part of the EIP and there are two separate EIPs proposing different solutions.

**Micah Zoltu**  50:35  
Okay, apparently Tim is still on American time.

**Pooja Ranjan**  50:41  
He's right on time. It just that we started an hour early.

**Micah Zoltu**  50:48  
Right on time only if you're living in a previous point in history.

**lightclient**  50:59  
He's so ashamed. To be fair, I don't know if the calendar was updating until this morning, right?

**Pooja Ranjan**  51:14  
Yeah, it wasn't like, and there is this. There is this calendar that is created by Ethereum team, and so that might also need some updating, because that's also showing the older one. And the one that I run,  I updated it this morning.

**Tim Beiko**
So what time should this be? An hour ago? But this is right on the calendar. Oh, it should be an hour earlier. We're starting an hour late this week.

**Micah Zoltu**  51:45  
So we already had the meeting. We just finished is what we're saying,

**Tim Beiko**
Oh, shit, sorry. Okay.

**Micah Zoltu**  51:52  
We've agreed that it's not entirely your fault. It seems that the calendars are, yeah, not all up to date.

**Tim Beiko**
So I guess, is there anything really urgent that's like, you really needed me for that? Okay. Sorry about that. I'm going to change the timezone on the protocol meeting invites to be UTC, which I think we can do now. So that means that it actually stays kind of fixed.

**Pooja Ranjan**  52:22  
If possible, I would also like to share the Zoom link there. Do you think it would be a good idea to share the Zoom link in that invite?

**Tim Beiko**
It's already there. That's how I joined.

**Pooja Ranjan**  52:34  
Okay, okay, fair enough.

**Tim Beiko**
Quick question. I'm curious - how do people feel about the new - crop is probably too strong of a word, but a couple of people who have joined into the EIP editor channels. Anyone make a contribution yet, or is it just too early to tell?

**Micah Zoltu**  53:00  
I haven't seen any contributions, at least on the part of the EIPs that I watch. But it's very early, so hard to say if that's just people are still trying to figure out where they fit.

**lightclient**  53:11  
So I also haven't seen a lot of contribution, but I have had a couple people DM me. So it was like they're trying to figure out the situation and do some contributing at some point.

**Tim Beiko**
Cool. By the way, is this meeting every two or four weeks because the the protocol invite does every four weeks? but yeah, okay. So I'll change that as well. Okay, so that means that the next one would be basically  December 1 at 1500 UTC.

**Pooja Ranjan**  53:46  
Thank you, everyone, for joining us today. And hope to see you in next two weeks. And thank you, Tim, for already updating the universal calendar that we are recommending people to join and follow. So thanks, everyone. See you in two weeks.

# Attendees

* Brent Allsop
* Tim Beiko
* k
* lightclient
* Micah Zoltu
* Pooja Ranjan (Host)
* Spore_Druid_Bray



# Date for Next Meeting: December 1 at 1500 UTC
