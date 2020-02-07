# EIPIP Meeting 2

### Meeting Date/Time:  Friday 10 January 2020, 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/1)
### [Audio/Video of the meeting](https://youtu.be/oviaIsMLb8M)
### Moderator: James Hancock
### Notes: Jim Bennett

----

## AGENDA

## 1. [Ordering the most important issues to address](https://youtu.be/kt59-FEeWTI?t=178)

**James Hancock**
All right. So I have the agenda here. This is the EIPIP Meeting. I am hosting it. Hudson isn't able to make it today after being sick. The general purpose of this meeting is to improve the EIP process. Thank you for everybody who is joining.

We have a three-point agenda. And then I have some ideas to present on things that I've been thinking about. This is a very much a meeting of coming together about ideas and proposing things. This isn't proposals or official ones. All of those will go through its own kind of EIP. We just want to accelerate discussion around them, so we can have a little bit more momentum to implement. Ordering the most important issues to address, dividing into teams to come up with ideas for solutions, And three, the next call. I'm not sure of the best way to do that.

You have something, Tim?

**Tim Beiko**
Sorry, I unmuted by accident. We still can't see your screen.

**James**
I guess we can just go into my ideas unless there something else someone wants to bring up or something else to put on the agenda, we can put that on now. And if we have a short meeting today, that's fine. If anyone has other things to present, please let that be known.

So going into EIP 1, there is kind of a lot going on. In general, what is my experience over the last while is that the important information in the EIP repositories is sort of all over the place. So if I want to find if I want to look at the hard fork I have to go into here, it's to the hard fork meta EIP, and that tells me information about it. There's an EIP for the process of hard forks, which is another EIP. There's an EIP that tracks [unclear] which I wrote that hasn't gone through yet and one of the reasons is that it's confusing to have all of this different information in different places.

**Brent Allsop**
The page you're on now, that's EIPEthereum.org, does that update from the real EIP or does someone maintain this and keep them in sync?

**James Hancock**
Yes. So the the EIP repository, if I make a pull request to this EIP that changes this text, this website will be remade.

**Brent Allsop**
Okay, cool.

**James Hancock**
Any EIP that's been accepted into these status after it has been accepted as draft, then it will show up on this website.

**Brent Allsop**
Okay, yeah. One of the ones I have is ready to push to abandoned. And so I'm just wondering and curious about that.

**Speaker 3**
Would it also be possible to add the creation time and the last update on each stage?

**James**
The creation time on the EIP?

**Brent Allsop**
Yeah, that would help.

**Speaker 3**
Yeah, when the EIP he was created and when it was last updated. And the reason I'm asking is because I've been on this website many times, and you . And you don't know, when you look in a directory, you don't know if it has been replaced or superceded or whatever. And it would help in terms of skimming through the content.

**James Hancock**
Yes, One of the reasons I think hat's not there is that I think that's not there is what part of what happens with an EIP is - we should also mark that as something to put in. And I think I have a way to integrate that or a way to make it so more of us can update that information in a timely, more organized manner. Because the reason why stuff like that falls out is because the only people that can end this text is the EIP editors and then these authors. We could have a bot update it, but if we're going to have someone update it, it would have to be one of these people. And the EIP editors are already doing way more than is required as far as information and specialty. They should be focused on other things.

At the same time, all that information is really important for people approaching the EIP, and the repository, so they can understand what's going on at a quick glance. Currently, there isn't a good with to handle information like that. It's kind of like meta information about the EIP itself, and there isn't an easy way to update it without relying on the authors who aren't doing it.

We'll get back to that if there's any other comments or questions from people taht are going through. I'm happy to be interrupted., And ideas about things to be put in, I want to make sure to make a list for people to  talk about.

**Speaker 4**
James, what about adding hard forks into the [unclear]

**Speaker 5**
So I think the only meta EIPs peeps are basically the hard forks ones, no?

**James Hancock**
Yeah. There's the standard - there's the formal process for heart forks that Alex wrote, which is with the old system. The EFI will be somewhere in here. Then we have a whole bunch of hard forks and EIP 1.

**Speaker 5**
To me, that seems right. It seems like "meta" basically means "upgrades." I think it's good that the process is listed there, and if we actually change the process, which we have, then it makes sense to also see the old process there. I think this actually works. My only quibble - I posted about in All CoreDevs - is that your EFI list is still not merged. But I think as soon as that's done, it would show up in there, right?

**James Hancock**
Yeah. And the reason it hasn't been merged is I've gone back and forth with Alex a couple times about it. And when it was first proposed, and when I was first thinking about it,Alex is thinking as well, is that it really should be a registry. Only a registry. So in the EIP text for the [unclear] conclusion, when I went to write it out, I just wrote this list here. Here is a registry of the eligible EIPs. And people who are authors are able to edit that. When I was writing it, I realized no one has any clue what any of that means or what the whole process is, so I wrote it out here in this simple summary and abstract.

And someone who was just coming to the repository isn't going to know to go to EFI to read the EFI part and then go to EIP 1 and to get the other part. All of this information should be in EIP 1.

**Speaker 5**
Yeah, I agree with that. I still think we should probably merge this sooner than later, because right now, we don't have a hard fork or a meat list to point people to. And that's been a problem. I talked with the [unclear], for example, and they're like, "Oh, what EIPS are being considered?"" and I basically sent them to your PR. I agree it's not perfect.  I think if we merge this because I think EIP 1 would probably take weeks, if not months. That's been my experience trying to get small PRs in it.  I don't think like it's gonna be done in a matter of days or weeks. So it's probably good to just have this list that we keep in the meantime.

**James Hancock**
Yeah, I agree. I saw your note in AllCoreDevs about this discussion. So yes, we should get this included. As far as administration stuff, we should do this soon. Talking about how do we improve the process of the process. It's how do we get this information to everyone.

We have the EIP 1, the intro. We have a table of contents that points to different parts of EIP 1 that has all the things and then in our list that go to registry EIPs, and those registry have indicates the EFI list - it has lists of EFIs, but it doesn't have the information about how the EIP process works. To read that, you'd have to read in EIP 1 somewhere. And this this would get pretty long, but I think that's okay, because it's better to have everything in one place so stuff doesn't get fragmented conceptually.

**Speaker 5**
Yeah, I agree we should be much more liberal linking stuff in EIP 1. Every time there is a new fork meta we should add it there.

**James Hancock**
So the way we extend the functionality of EIP 1 is the authors of these different registries do whatever they need to do to make them work. Right now, we're pretty limited. Something I'd like to add is another list. So something extending this is going back to Louie's point that we don't have a good way of seeing some of this important meta information, and we don't have a good way of editing it as a community or a good process for it is to have another registry EIP, and people who can edit a certain part. I'm thinking of them as EIP maintainers. And their goal is just to maintain the repository and keep information up to date that isn't on the same level of needing understanding like any EIP editor would.

That's probably a lot of words, so I'll get into a more concrete example of what I mean. So, going back to Istanbul, I made this Google document that tracked the more fine-grained process that the EIP was going through as a way just to figure out where we were on each one, so we could know which ones we needed to work on. Because there were something like 35 that applied. And then how do we go from 35 to the 4? It was just a big mystery.

It's just stuff that would be nice to track, specifically about an EIP that an author doesn't need to. Because I
wasn't the author of any of these EIPs.

So is there a PR? Was it formatted correctly? Has it been reviewed and merged? All of those things an author doesn't need to do, and an EIP editor doesn't need to track either. But it's good to track, and it's good to show the progress of the EIP itself.

So how do we make it so this kind of information can be tracked? And my solution to that is to have a group of people like us, and I assume many of us would join it, of maintainers that have access to edit this information as part of an EIP.

So a kind of real life example - If I go to the DMV to get my driver's license, I have this form that I fill out that has all this information. And if you think of any EIP being like this form and having questions that need to be answered and then the specifications like that, that's all done by the authors. But there's also this part of the form that is the "office use only," and the author doesn't edit this. The people at the counter do.

So somewhere like at the bottom of the EIP we could have a blank spot that is that anyone who is on the meta EIP for the maintainers could have access to edit without the permission of the authors and without needing permission from the editors. So we could create a footer of things like "last updated," or where they are in the EFI process or, really, anything at all. The easiest way technically would be just to have a section of the footer need to exist, and that any changes to that footer could be done by anyone who is on the meta registry as a maintainer.

**Speaker 5**
How would permissions be handled?

**James Hancock**
Permissions would be handled by the EIP bot. So currently, if I'm an author on an EIP, and I make a PR to the EIP repository, the EIP auto merge bot checks that I'm only editing stuff and that I'm an author, too. And if it's true, we'll just merge it. It doesn't need any permission from the editors and it doesn't need anything else, because I'm an author. I'm listed as an author on that page. Then I can edit that EIP and it gets auto-merged. So you could do a similar check in the bottom footer where someone submits a PR that edits the tracking footer, it could check "Are you a user in this registry of EIP maintainers?" or whatever we want to think about calling them. And if it's true, then it could just accept it.

**Speaker 6**
That would also restrict permissions of a maintainer who would try and sort of maliciously merge or anything like that, a bot would be able to stop it?

**James Hancock**
Yeah, they wouldn't be able to edit any other parts of the EIP.

**Speaker 6**
That's super cool.

**James Hancock**
So you have this little part of the form here. And as long as you're living in that form, we could make it whatever we want. I want to be able to make it updatable and not get us into a certain format. The first thing I think would be nice is having an EFI tracker or Last Call. As soon as we have a system where we have a group of people that can actually make the edits, then we can get rolling. At this point, I think I'm rambling, so I should probably pause and see where people are kind of confused.

**Brent Allsop**
I made a change to EIP 3 in my own forked repository and I wanted to show you the direction I was pushing. Would now be a good time to look at something like that? Because this is exactly the kind of stuff I need to know.

I contacted the author and he said, "Yeah, let's close that one down." He was happy that I was willing to help with that.  So I have a pull request ready to submit, but I wanted to show you guys and make sure I'm doing the right pull request and the right process.

**James Hancock**
That's a little that's a little bit of a different conversation, but I'm happy to have it.

**Brent Allsop**
Okay, if it's later, then that's great. Whatever.

**James Hancock**
Because the problem you're running into is kind of far was one of the things I want to help solve. Again, these are all ideas. This isn't a "Hey, let's do this." It's a "I want us to think and talk about it and discuss to decide." So you updating the status, you're not able to actually do that because you have to do the PR and then get someone to approve the change, which in the case that a change is substantial to the EIP itself, then an editor should approve the change. If it isn't, he doesn't need to, you're just adding in extra steps.

**Brent Allsop**
Right, this one's here is going from draft to abandoned.

**James Hancock**
That would be one that would be good for an editor to do. So that would make sense.

**Brent Allsop**
So when you say editor to do the PR or me to do the PR and get an editor to approve it?

**James Hancock**
An editor approving your PR.

**Brent Allsop**
So I do the PR first and send it to him  - find an editor or something like that?

**James Hancock**
Yeah, You make the PR.

**Brent Allsop**
I've started on a PR. It's just a draft. I sure won't be the final one.

**James Hancock**
I can show you in this. So this is my PR I made for the EFI, and once I've made it, it shows up against the Pull 2378. You can't see it because I'm now sharing the wrong screen.

So this is my pull request that I made [unclear] Patch 5 five with Ethereum master.

Now perhaps just doing a workshop of this is a good idea. We should add that as a thing to do.

**Brent Allsop**
I just showed a link to to my fork modification of the EIP to the chat channel if you want to click on that, I could just show you.

**James Hancock**
I turned my Telegram off.

**Brent Allsop**
No, the Zoom chat.

**James Hancock**
Oh, the Zoom chat.

Yeah, I think we should add a workshop of anyone who wants to work on going through the process of doing a pull request EIP. That'd be kind of cool.

**Speaker 6**
Do you have a particular conference in mind with that?

**James Hancock**
No, I just think like a call would work. Basically what I'm talking about with Brent right now, but open to more people and more explicitly saying, "Hey, this is how you make a pull request to the EIP repository."

So this is your EIP here?

**Brent Allsop**
Yeah

**James Hancock**
It is a fork. You haven't merged it or you haven't made it a pull request.

**Brent Allsop**
Oh, yeah. Of course. I'm just practicing on my own fork until I can get it right. You can see I changed the status to "abandoned." That's one change I made. And then I added that abandoned statement. Since it isn't Martin that's gonna do this pull request. But, anyway, I was just thinking along those lines that I'm probably going to  need to do it different from that.

**James Hancock**
so this is totally right. This I would put in, like, if we had the section I'm talking about having, it would be perfect to have something like this where we could say, "Oh, yeah, his is a substantiation for something that happened" and just put it in the footer for you managing. That'd be perfect. It wouldn't fit in the abstract, but it should go somewhere. Just better information in general is good.

If you have a question, go for it.

**Tim Beiko**
It's sort of like a moving forward thing, so I'll just sort of throw it out and I'll see if this is constructive for conversation of if you'd rather my move on to what you were saying. There was some talk before about the
difficulties of making changes to EIP 1 itself. I was wondering if it's useful to make a distinction between historical EIPs and future EIPs, as in if you were going to change the EIP template for the future, isn't it only for EIPs after whatever. Would that make it easier? Would that expedite being able to make a change to the EIP process versus only changing historical ones? Or maybe it's the exact opposite. I just basically wanted throw out the idea if it's a useful distinctions to make a distinction between EIPs that have already been made and changing EIPs for the future.

**James Hancock**
On one hand, it doesn't really matter at all, because a Github file is a Github file is a Github file, and it could be whatever it wants. So you could reorder and do everything completely different. Where there are some limiting factors is the bot, the Jekyll program or whatever that creates the website is looking for certain things and expects a certain format.  And if it didn't get that, it breaks.

So more to what you're saying is that any changes that break that format, we need to make along with updating the web to be able to handle the new format. I hadn't meant that, actually, from a technical standpoint. It;s more from, I feel reluctant to use word "political," just in terms of getting consensus for acceptance.

**Tim Beiko**
So I think for that part, it's kind of hard by design. I think it should be hard, and, especially going forward, because what you're saying is that changing the way it works for future EIPs, it's kind of changing the rough consensus on Etherum of how we actually make changes, which is a pretty big deal. So I think it's okay that this is not the quickest process, because the last thing you want is for this to change and for people to feel like you they didn't have a say in it and that things are happening behind closed doors. I think we should really try and make everything explicit and give  time for people to comment and give feedback. So I don't think that's particualrly a bad thing.

It seems like the process for core EIP and other EIPs is very different. And how we make that more explicit - we already have the EFI process, and we probably don't want the EFI process for non-core EIPs. And if that's the case, we probably need just the clearer separation between core EIPS and non-core EIPS, where we probably leave the process for non-core EIPs unchanged.

**James Hancock**
Yes, and going to something else I remember you saying earlier, Tim, was that the EIP process as far as the core devs and coming to decisions and in making them actually works pretty well. What is lacking is EIP repository lags significantly. It doesn't follow very well the decisions that are made and when they're made or consensus.

The way the AllCoreDev calls will go through an EIP works well. What is missing is the EIP repository doesn't follow it very well.

**Tim Beiko**
Okay. Yeah, that I agree. Yeah, and I like your idea around like that sort of "office use only" part, that I 100% support. I think those are two different things, right? The process tracking, we probably should try to get that as quickly as possible, because it's not really doing much except just providing more visibility. But this first bit, slides 2 and 3 on your proposal, that seems like a much bigger undertaking. That's all I wanted to highlight.

**Speaker 9**
I just wanted to add that in the CoreDev decision making, I completely agree that overall, it works very well. I did spot at least two cases of where there was a lack of a well-defined process. And because of that, we created some sort of [unclear - floating?] time where we didn't really know how to push or not push the case forward. The first one I was thinking is the one that relates to Blake2b. Blake2b was not done properly, and the reason is because people were pushing it were sort of like [unclear.] The CoreDevs could keep pushing it because there was no one to reject it. But at the same time, there was no one there to defend it. And it went on and on, and until the time we realized the spec for us was not fully defined. And what this says and what spec we're doing was slightly different, and that I think that should be addressed before.

So that was the first example, and I have another example [unclear], It involved a skill set that the CoreDevs may not have. Those should have a process that needs to be better discussed and defined.

**James Hancock**
And that would be good examples of stuff that would be great to fit into a section of EIP 1 that we could have linked to a table of contents. I would really look forward to your help on that on clarifying some of that and then getting some language that the CoreDevs could agree with. Because I can say on the other side of the Blake2b, having helped get that through...

**Speaker 9**
I'm not blaming the Blake2b. He worked. The problem with Blake2b is that I feel... it;s out of the scope of today, but I have a discussion for what the champion of the EIP should be doing, but in the case of Blake2b, , yes, I think there was something wrong there.

**Louis Guthmann**
One thing I just want to add is that I 100% agree with EIPS that are very technical. And the problem with the process right now is they get treated very differently.

Take specific examples. You look like at EIP 1962, which is being proposed now. There's a lot of concern by developers and, like, we might not be able to evaluate its properly because it's kind of advanced crypto. And it seems like there is general consensus, but there's some consensus around, "Okay,you have two different implementations. They give out the same thing. It's probably good enough Don't care. We're gonna get it." Whereas if you look at ProgPoW, because it has this added element of political contentiousness. it won't even get discusssed unless there's an audit, even though had a working testnet and whatnot. And it felt like it kind of had a a higher technical burden because of its political implications. And a lot of people on the CoreDevs call felt like the audit was just kind of a distraction to kick the can down the road.

And so, yeah, I agree there's probably a lot of value in trying to get to the rigor we demand for EIPS. And you know, like recently when [unclear] came on the call, he wasn't sure for 1559, right? What is the sort of rigor that we should demand for a change like that, which is not maybe as technical but has wide ranging economic implications?  I don't think there's an easy answer to that question, but I think having some answer is probably better than our current...

**Speaker 9**
I definitely agree with this. [unclear]

**Louis Guthmann**
Yeah. But we need to find what's the right level. Do we expect any sort of major EIP like that to put in 10 to $100,000 for an audit? Whether it's a technical audit or economic audit, and if so, we should make that clear. And, you know, the downside is that obviously discourages anybody who can't afford or can't raise those funds to propose such an EIP.

**Speaker 9**
There is something greater. I think there are ways to make it. It would also in my opinion depend on the sophistication of EIP - [unclear] If it's broken, the client knows what to do. It's their job. For an EIP like ProgPoW, you're right. If something's wrong for whatever reason, it happens to be -- some vector somewhere -- what should they do? ,That is the sort of process we need to put in place to [unclear] fast pathway to withdraw. Because I think that is most likely the biggest burden for me, the EIP closer. I think, that is in fact, better than to languish.

**Louis Guthmann**
Yeah, I agree, that makes sense.

**James Hancock**
I also agree if there was some sort of expectations. It's a healthy relationship with people. If there are
expectations ahead of time, things go away better vs doing stuff and then figuring out "Oh, I was wrong about that when the entire time, both people wanted to do what was right and they were just doing what they knew. And it just keeps going.

So it sounds like we're in agreement that there are certain things that it would be good to articulate around expectations for people who are doing a certain complexity of EIP.

**Louis Guthmann**
That's a yes. Yeah. And then how you set that bar is an exercise for the reader.

**James Hancock**
Yeah. So articulating it, recording it somewhere - that, I think, is going to be a long process, a long thing to get right. Yeah, it kind of sounds like a subgroup forming. Maybe that's something you would be interested in, Louie, is kind of figuring out some of the language around that.

**Louis Guthmann**
I'm not sure I would know how to do it, but if anyone wants to take the lead, I would be happy to join the discussion. I'm just not sure how you would want it to be.

**James Hancock**
I'm just thinking of dividing into teams and coming up ideas for a solution with just one part of the agenda. This is a clear place we could create a team.

**Louis Guthmann**
Let me think about it. Let me get back to you offline.

**James Hancock**
And I would be interested in joining that team as well, if there was a team for free for figuring that part out as well.

**Louis Guthmann**
Sure. I need to think in terms of a schedule. Let's take this offline.

**James Hancock**
So as far as stuff that I was gonna present today, it's really those three things - reorganizing EIP 1 to being the canonical place for everything informational, pushing all of the permission things that need to be edited on to different registry EIPs. Another one that would be nice would be doing a registry for EIP numbers so we would have a logical numbering system. I think that kind of system is pretty extendable and also approachable for people doing the system tarting this idea of What is it that EIP editors don't need to do, that a group of us can do and manage, which is kind of around this idea of any EIP process tracking footer which is like the "For Office Use Only," and if that's the right way to go, and if that's something we agree on, how do we develop that into the EIP bot to make it work technically?  More feedback on the idea or

**Tim Beiko**
I think I agree, And this all looks good. One thing, maybe like a fourth idea that we should start discussing is how do we add more EIP editors? I know this has been brought up again and kind of dropped a bunch of times, but it feels like something where we have this huge backlog of EIPS, and it the people we have are kind of overworked to do that, and at the same time, there's a pretty high bar that you need to give access to those people. So it's not easy question either. But what's a process we could have to add EIP editors that makes sure that the people end up being there don't abuse that privilege?

**Brent Allsop**
How are the current EIP editors selected? What made them EIP editors?

**Tim Beiko**
They were all basically working at the EF in 2015-ish. So, like when when Ethereum started. And I think at that point the project was small enough that it was easy to get a set of editors, but it hasn't really grown since.

**Speaker 9**
So the people we're dealing with are the same people who were there in 2015?

**Tim Beiko**
Not exactly, but yes, more or less. To my knowledge, maybe there's some exceptions here, but most of the editors are very longstanding Ethereum community members, which to be fair is not a bad criteria.  It's probably something you only want people who've been part of a community for a long time.  But we haven't added a second or third wave of editors. And looking at that list, people like Vitalik obviously don't have time to to do this. Not that he should be removed, but he just doesn't contribute as an editor, which makes sense. And to be fair, some of them still do, and it's great that they do, but we should find a way to help them. And at the same time, we should still keep a very, very high bar for people that should be added to that list.

**Brent Allsop**
Just brainstorming an idea for how to do that kind of stuff - at Canonizer, we have what's called a peer-ranking expert system, where peers can rank each other. And so that gives you a quantitative measure of their rank in the community, and we could set something like that up where everyone could vote for people. And then the peers could rank each other and then you get a quantitative score. And if you meet a certain bar, then you can become an editor. Just an idea.

**Speaker 9**
Ranking people for the technical things is not something I'm very comfortable with, but I wonder if the EF would have some more funding to pay for more tests. I'm sure we could find people even if they were not paid a lot of money, but just something to contribute for their effort.

**Tim Beiko**
I think we probably finding other people unpaid if we had a clearness of criteria of what they want. I'm a bit conscious of adding a tool or a dependency in this process. I feel like it has to be kind of half explicit criteria, half rough consensus, probably from the current EIP editors. But I think we probably definitely need more people.

**James Hancock**
So when I was talking with Alex earlier, one of the EIP editors, they spent some time trying to finding other ones previously. One of his feedbacks was it was hard to find people really are active. To say it another way, what we don't wanna have happen is create a system that finds the best EIP editor but then never shows up. Being qualified technically, wanting to do it, and also doing it are three sides of a Venn diagram.

**Tim Beiko**
People can probably do this without getting paid are people who work on Ethereum full time - they work on consensus or EF or someplace like that for another company where it's their job that gets them to work on Ethereum full time, and this is just part of the open source work they do. And then the challenge is also. is it the best use of of that person's time? Like, what's the Venn diagram of, like, the person could be writing code to contribute to Ethereum or writing EIPs and other people who are just like technical enough to do the EIPS part, and it's maybe not that big of an opportunity cost for them to actually be doing this work?

**James Hancock**
Two different conversations - one is what is the bar for becoming an EIP editor? The other one being how do we get people that fulfill it and start working on it?

**Tim Beiko**
Just one other thing. I have actually talked about this internally with people at Consensus to get their thoughts. And one question that people had is what's the commitment? If they're an EIP editor,time-wise and responsibility-wise, what are they agreeing to do? I think if we could say something like it's, I don't know, five hours a week or 10 hours a week or whatever and these are the things you actually have to do - that might help find people.

**James Hancock**               
Yes. The other kind of interesting thing is that anything an EIP editor does, you can do without being an EIP editor, as far as responding to PRs, making comments, saying, "Hey, you need to do this." "Okay, this is good to go." Everything except just hitting the merge button.

So I think there are  parallel things that can happen. If we can take some of the stuff and put it into things that that maintainers can do, like the "Office Use Only" form. Things that need to be tracked there can be done by them. So we're offloading what we can from the EIP editors. Define what the EIP editors do. Define what the bar is for an EIP editor. This is sounding like another group is forming, more like a group idea around defining this.

Then, through a system, where people participating in this or being a maintainer, you can see someone's being active. Then it's pretty easy to say, "Oh, yeah, if this person was an editor, that'd be great."

I'm not saying that exactly right. How do we get people to start participating? Instead of saying, "Hey, let's find people and then get them to participate, just get more people participating and then turn them into editors. Does that makes sense?

**Tim Beiko**
Yeah, I think that's probably just doing a better job, you know, like this EIP editor responsibility is kind of buried within EIP 1. The cat herders can probably help with this. And I know William and Brent, if I recall correctly, had done a bit of this, but how did we just make it clear what people should be doing and and can do and market that?

**William**              
Only Brent, I feel bad taking credit.

**Tim Beiko**              
Okay. Sorry about that.

**James Hancock**                  
Yeah, And there is some disagreement already among the EIP editors about what that is themselves. So that is kind of another thing to work through.

So maybe we can reach out to frequent EIP submitters like Alexey to check. They would be interested. Alexey, to me would be one of those individuals that needs to not be an EIP editor. Could be, but as far as time goes, and this is just such a hard thing because the bar high means you're high contributing member.

**William**                  
There's an old American joke about jury duty. Since I don't think this is an all-American crowd, I'll explain it in about 10 seconds. Jury duty is completed with people randomly picked to be jurors in court cases in America. So there's an old famous line that anybody who is smart enough to serve jury duty is smart enough to get out of it. I feel like this is a similar kind of paradox. Anyone good enough to be an EIP editor is necessarily going to have demands on their time. It's just trying to figure out exactly where to find a good equilibrium in that chaos.

**James Hancock**             
Well said. This is an hour, right? Right. So we're at three minutes left.  Does anyone have opposing thoughts to the having a process tracker with some maintainers that have the ability to edit it and reforming EIP 1? Any other feedback or concerns?

**William**               
I guess the real question is what now? What can we do now? Is there anything actionable right now?

**James Hancock**                     
Actionable is if we think it's a good idea, then we then we figure out how to get the bot to do it.

**William**                     
Who does that? Who controls the bot?

**James Hancock**                  
No one controls the bot.

**William**
Someone should have permission to encode it.

**James Hancock**                
Yeah, yeah. I see what you're saying. The permissions are the EIP editors. I remember Hudson saying that there was one coder from that was interested in participating in this from the EF, a Web developer.

**William**                
So it would be about getting in touch with someone, having them them make a PR to modify the bot, and getting that merged? That's what we're looking at right now?

**James Hancock**  
Yep. And then the website would need to be able to render it. So two parts: the auto-merge bot would need to be able to [unclear] need to support it, and then the Jekyll web builder would need to be able to render it and deploy it.

**William**                 
And other than that, you're saying there's no there's no sort of consensus issue in the way? Basically all you need to do is get in touch with this person who's willing to program the bot. They program the bot, and then that's it.

**James Hancock**                  
Yeah, on the consensus part,we bring it up in the AllCoreDev call and figure out how some of the other things fit in with that.

**William**      
Does that need to happen first? What's the next step? The next step is AllCoreDevs first, or is it programming the bot?

**James Hancock**               
Finding someone to program the bot.

**William**                  
I misunderstood. I thought you said you had someone.

**James Hancock**              
There is someone that Hudson talked about, but I don't remember who he is, and I don't know what level he's involved. But I remember him saying there was a Web developer that was interested in participating, so that person could do it. It's figuring out if it's possible through the system that I described technically. And then if it's possible,  get it done, and, at the same time, make sure everyone's okay with it so we're not just deciding right now.

**William**                  
It sounds like this is mainly things that you yourself are doing. James. Correct me if I'm wrong, but we need to find someone who can handle the code for the bot to see if this is even realistic, and you want to simultaneously try and propose to the AllCoreDevs the various  change ideas going on now?

**James Hancock**
Yeah.

**William**
Cool.

**Brent Allsop**             
I would bet the boat could pretty much do anything you want as long as you clearly spec it out. It's that detailed spec that I think would be the hard part.

**James Hancock**                 
Yeah, we'll have to talk to an editor about that. Someone who's helping. As far as redoing EIP 1 in this kind of format, that's just a matter of making the PRs and then having people talk about it enough, which will take a long time. But it makes sense.

That's it for me.

**William**               
Are we scheduling another meeting now?

**James Hancock**                
Oh, yeah. Schedule another meeting. Should we do one week or two weeks?

**Brent Allsop**             
I like a consistent time  - every two weeks or something like that.

**Tim Beiko**                  
Yeah. I think two weeks is easier than one week.

**James Hancock**          
Okay, two weeks from today. That sounds good to me. Same time, same place. Thanks, everyone.
