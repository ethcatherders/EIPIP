# EIPIP Meeting 65 Notes
### Meeting Date/Time: Wednesday, Sep 21, 2022, at 14:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/176)
### [Audio/Video of the meeting](https://youtu.be/0miajHm8JXs)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## DECISION ITEMS

**DECISION 65.1**: Victor to create an PR to further discuss on the copyright waiver section instead of mandate the CLA.

----

## Intro [0.00](https://youtu.be/0miajHm8JXs?t=1)
**Pooja Ranjan**
* Welcome to EIPIP Meeting 65. I have shared agenda in chat and, we have a few open pull requests and some issues from EIPs Github repository here, for discussion and probably make some decisions so we can move forward with the pull requests at least. And then we get into, the progress on EIPs bot with some EIPs insight and, maybe action items or decision made from the earlier meeting. So let's get started. 

## CI: Add Markdown Linter ethereum/EIPss#5367 [0.42](https://youtu.be/0miajHm8JXs?t=42)
* The first one listed here is a CI: Add Markdown Linter. I suppose it was added by Sam Wilson. Sam, if you would like to maybe talk about the proposal. 

**Sam**
* Sure. The idea is to add a bot that, corrects common markdown issues and tries to keep people to the lowest common denominator of markdown so that it's compatible with different renderers. there's been a lot of discussion on that pull request already. I think we've settled on a relatively decent set of links to start, and we just wanted to get some, consensus before merging that PR. 

**Pooja Ranjan**
* Sounds good. I don't know if Greg, you have any thoughts to add here? I know you earlier mentioned that it is related to bot, but yeah.

**Greg Colvin**
* No, on late breaking agenda, I noticed Sam is here, so it could be an opportunity for he and I to discuss, the reference client and how that's going and how, how we should be relating it to the, the EIPs work, since we're making progress on that as we we clear through these other smaller issues, that would be maybe a good time for us to talk. 

**Pooja Ranjan**
* Yeah. Okay. I'll put a note on the agenda for that. 

**GColvin**
* Okay, good. 

**Pooja Ranjan**
* Cool. I don't see any other EIPs editors, I can't see, Sam, sorry, Lightclient or, or anyone else. Pandapip mention that he would be a little late for the meeting today, however, this Pull request is by him, so I'm assuming that he is definitely on board. So, maybe we can just let people know one more time in discord channel and move ahead with the decision sounds fair?

## Website: Add MathJax ethereum/EIPss#5596 [3.03](https://youtu.be/0miajHm8JXs?t=185)
**Sam**
* Yeah, I guess, we can go to the next one. The MathJax one.. Yeah, I think that's a, a less, suggestion. It's just adding a JavaScript library that can render late tech. and I think, Greg, you mentioned you like that, so maybe that's a good thing to to add, 

**Pooja Ranjan**
* So the idea here is like we are trying to, make all editors aware of any changes which are proposed and also being merged, by active editors on board  however, it is good to always collect, kind of rough consensus from all the present editors. So yeah, if you have any thoughts on that. 

**Golvin**
* Yep. That's all. 

**Sam**
* So you're, are you okay or not okay with, adding mathJax? 

**GColvin**
* I'm just asking whether it renders properly at the end of the line. 

**Sam**
* Oh, I'm not sure. I didn't hear you ask anything. Yeah, I've never used it. I think it's probably okay. I think it's the most common JavaScript, latex renderer, but, we can, we can do some tests if You'd like. 

**GColvin**
* Yeah, I mean, that's the big question. The last time I tried to use it, I couldn't get it to work, but that doesn't mean it doesn't work. It just means I couldn't get it to work.

**Sam**
* Yeah. No, I, I know how that it goes. I guess if there's anything in particular you'd like to see, like a test of, put it in a comment on that PR and we can try it out. 

**Golvin**
* Okay. I mean, EIPs are full of, of math that winds up getting, you know, sort of butchered with, with, you know, asking math in line. that would looks much better if it was, you know, properly type set, and snatches from the yellow paper and things like that. 

**Sam**
* Yeah. Okay. Well, I'll try to get it to format some stuff from, yellow paper. Yeah. 

**Golvin**
* Yeah. Maybe one of the other formats works better. I really don't know. I don't know where in the pipeline that final, copy gets rendered, by what system, is the name of the renderer we use. Okay. So somewhere there's documentation for the, the dialect of markup that it accepts. 

**Sam**
* Yep. Somewhere I, I've never looked Really, 

**Golvin**
* Really good system back in the seventies. It, it had its quirks too. It it definitely did. 

**Sam**
* Right. But, you know, they all do. We knew what they were. Yeah, that's true. So I don't, we have enough editors on today to talk about adding a new editor. I don't feel like two of us is sufficient, and I think, 

**Golvin**
* I think he's done enough good work that there's, I can't imagine any objection, but Okay. 

**Sam**
* Yeah, I'm, good with that then. 

##  execution-specs [7.22](https://youtu.be/0miajHm8JXs?t=442)
**Pooja Ranjan**
* All right. In that case, we can, jump over to the latest item that is added by Sam. Thank you. And I, I believe, Greg also wanted to discuss that, that's the execution-specs. 

**Sam**
* Yep. So we're, almost done implementing London. we've quite a paused so far on on discussing how we wanna integrate it into the process. since, you know, the merge and core devs kind of wanted a break for about a month, so, Oh, yeah. Yeah. There's not gonna be much happening in terms of like what we're planning on doing. we're just in the final stretch of polishing up the, well finishing, you know, catching up to Paris and then, and then polishing. 

**Golvin**
* I'm really happy that it's coming together. you may have noticed that the, that the VM or real EIPss are, are all moving to Python as the, as the demonstration language, but I don't, Pardon? 

**Sam**
* Have you learned Python or? 

**Golvin**
* I can hack it out. It probably wouldn't run. It's, but it's decent pseudo code. That's the problem is it's, it's not code that's coming back out of a tested client. So, not Yet. 

**Sam**
* Not yet. 

**Golvin**
* Well, I mean, that'll be an issue. I don't, I don't think I want to learn how to get that client running and Yeah. Learn enough Python to actually integrate code and test it into another client. but I can write sudo code that's good enough and it can be a bit better than that. cuz I'm basically stealing code from the Ipson group, and it's, it's better code. but anyway, that code is not particularly related to the, reference implementation because it predates it. and that could be aligned. I don't think it can be aligned just by, you know, GitHub diffs. the code is there to demonstrate an algorithm, not to demonstrate a diff to any, some other system. 

**Sam**
* Yeah, putting it in the patch notation would probably clutter it up. Right. 

**Golvin**
* Well, getting it, getting it aligned. so it's recognizably the same, you know, the same algorithm in both places. Not gratuitously different, but, the other trouble with the diff is that that client moves on, so you've gotta diff against some earlier version of the client. and the, that works against the EIPs being reasonably self-contained specification. but anyway, that's one place where things, things have moved to Python and it's a question of how do we keep that Python aligned with the, the reference specification, using the same notation to the extent that it makes sense. 

**Sam**
* Yeah. Like same constant name, same function name is where applicable. Yeah, exactly. 

**Golvin**
* Yeah. Same algorithm. Yeah. 

**Victor**
* One, one of the, one, one of the scenario I can think of is that there was a, recent pull request to update the, one of the parameter names to be consistent with 1559. I, I just wanna call out that that's a good thing because keeping parameter name the same across different, at least different EIPs is gonna be helpful for readability and understanding. 

**Sam**
* Yeah, for sure. I think having just like a, a uniform language to talk about Ethereum is a huge benefit. 

**Victor**
* One thing though, about specifically using Python is that I realized some of the early EIPs didn't specify parameter pipe. Like one question I have is for EIPs7 that at introduced delegate call and Vitalic wrote, the, the, there's six operands being taken, but I had a hard time figuring out like what, what length of those parameter operands needs to be. Python doesn't give you that. I wonder if thoughts have been given to make it more explicit of the length of parameters. 

**Sam**
* So if you're talking specifically about the parameters to delegate called the opcode itself, they're all popped off the stacks, so they're all U256s. but in the execution specs, we do use typed Python. So everything has types. 

**Victor**
* Do we wanna suggest or mandate that implementations in Python as, reference implementation should, be in type? 

**Sam**
* I think we can probably make that comment on a PR, but really it's, that's up to the author. I think that's like a, more of a content thing than a like formatting thing. But yeah, we can definitely suggest it. 

**Victor**
* Yeah. I feel it's editorial because it's, like if you want people to adopt your EIPs, you have to be specific in, in a type, so that the client implementing your EIPs is consistent across the board. 

**Pooja Ranjan**
* All right. So, I think, Sam's suggestion may work here. We can probably leave a comment on the pull request and that author decide on that. but going back to, the discussion of executions spdec, if I remember correctly, a few meetings earlier, we were on a page where we were hoping to have a meta E for the changes those are proposed. I am wondering, if we are there yet, or, we still see some discussion needed to be reaching that proposaling status. 

**Sam**
* We have the same status of the hack MD that Tim put up. we haven't really progressed beyond that yet because like I said, the merge and and all core dev  is paused for the time being.

**Pooja Ranjan**
* Yeah, no, I'm gonna share the link here, or you already did? No. Okay. I have shared the link to the [Hackmd](https://notes.ethereum.org/@timbeiko/executable-eips), that, Tim has, shared earlier for people to refer to. I believe the changes has to be done on both the EL and CL sides, so we should look forward to the meta proposal that is coming up for the expected changes with executable spec. Thank you for sharing all updates. 

## Issues section [14.38](https://youtu.be/0miajHm8JXs?t=878)
* Sam. Moving on to the issue sections. I have listed a few issues which I collected from the EIPss Github repository. A few of them are created by Panda. I know he is not on the call, but I just wanted to share with all the, present participants if they have any thoughts that they would like to share or else they are always welcome to leave a comment there. 

## New contract interface and EIPs should be required to include a privacy considerations section ethereum/EIPss#5682 [15.16](https://youtu.be/0miajHm8JXs?t=916)
* The first one listed here is new contract interface and EIPs should be required to include a privacy consideration section. This is by, a new user. Yeah, anyone has any thought on this? 

**Sam**
* I think we're a blockchain and we're not a shielded blockchain, so I don't think, we really need to write privacy sections, but that's just my opinion. 

**Golvin**
* I see there are, I am not a lawyer problem here. 

**Pooja Ranjan**
* That's a good point. All right. yeah, I mean, like obviously if, if there are some changes that people are interested in proposing any changes, the next step would be to propose it in form pull request. Creating an issue definitely gives a good start so people can start adding thoughts over there. Yep. And I think the next one, which is, EIPs should preemptively add a CLA is also from the same author, I believe. 

## EIPs should preemptively add a CLA ethereum/EIPss#5662 [16.14](https://youtu.be/0miajHm8JXs?t=974)
**Victor**
* I think, Penda is also, in favor of having CLA, with patent waiver. I however, personally feel that, that I, I have concern, that will make it harder to contribute to EIPs and, before, Mihkail quit, I think he was a strong opinion about, not having CLAs. yeah,  I think my sense is weekly against having a CLA I can see the value of it, but I can also see the, the barrier it creates. I just wanna hear other editors, opinion on this. 

**Sam**
* I guess I'm weekly in favor of having a patent grant. I don't necessarily like the idea of having a separate CLA. and I'm also not sure I like Micah's approach of just ignoring legal concerns. But, yeah, I'm not a lawyer again, so, I have no idea. 

**Victor**
* Yeah. we are in some way creating the new legal precedence. I guess I wonder, I don't think Greg, Yeah, Greg, go ahead. 

**Golvin**
* I don't think other organizations, go to all of this effort. it's, it's a lot to ask of an author to be signing off on all of this legalese. if an author's concerned, they can, the author themself can add the legal ease that they feel they need. but otherwise it's just being offered to the world. here it is. 

**Sam**
* Yeah. I think the concern is more on the side of, like consumers, Like if somebody's implementing an EIPs, they might be concerned that, the author has a hidden patent that they haven't released. 

**Victor**
* Even if the author is not, is releasing the patent, chances are, they buy infra someone else who have not have anything to do with the Ethereum Right. You can influence a patent. Have, you can just run into a patent without the author being aware. 
* So even if you, so a client has to make their, the implementing client have to make their own judgment and research. If they're serious about this, I, I'm in favor of the practice that we can recommend, that's EIPs proposal to say that they release the patents. So my take on the EIPs is that it's an improvement proposal. Therefore, if you want to be adopted as an author, then the easiest for you to like, the more, the easier you make it to adopt it, the better for you as an author and wearing a hat of, of like editorial or editorial contributor, I would say making authors from different background, the easiest to contribute the better for the entire EIPs repository. So that, I would say using that argument, I was trying to advocate that we can recommend, but not make it a, a mandate. 

**Pooja Ranjan**
* Okay. And I also have shared the link to, a document created by Panda and favor of, this proposal. So yeah, people may go through, probably leave their more comments there. 

**Golvin**
* I agree with that. I definitely agree. 

**Sam**
* Sorry. The recommendation is to create an optional CLA or 

**Golvin**
* No, no, what Victor just said. 

**Victor**
* I think, I'm in aligned with you, Sam in that, CLA might be a be a bit too much, so we can have something recommended in the content of EIPs. 

**Sam**
* But oh, So yeah, I missed that part. Yeah, just like a little note, the copyright waiver section. 

**Victor**
* Yeah. So you optionally sign off any patent that you are aware of and you own, but like, as a, as a group, of EIPs repository, we don't require it. we don't mandate it. that, that would be my suggestion. I wonder if that's a concern. 

**Sam**
* Yeah, I think that's a reasonable, would you mind putting up a, a PR so we can discuss the specifics of, of what you're suggesting? 

**Victor**
* Should the, the CLA issue be a good place to continue the discussion? 

**Sam**
* Yeah, Yeah. I'm just saying like a PR would be good to actually put the, like decide the actual wording. 

**Victor**
* Okay. Okay. That sounds good. Yeah, I can do that. 

**Sam**
* Great. Thanks. 

## Errata'd EIPss ethereum/EIPss#5652 [21.38](https://youtu.be/0miajHm8JXs?t=1298)
**Pooja Ranjan**
* Thank you. Moving on. The next one is EIPs. It is proposed by Panda. Looks like a new one, not really new seven days ago, but there is a proposed change, to EIPs number if anyone would like to take a look or have any opinion on thoughts on that. The number is 5652. 
* Okay. we can, if anyone has any thoughts, they would like to share right away, it's fine. We can, we can discuss that. Otherwise, have shared the link, probably we can add comment over there. 

## Dynamic Required Approvals ethereum/EIPss#5651 [22.30](https://youtu.be/0miajHm8JXs?t=1350)
* The next one is a dynamic required approval. So there is some proposal of, okay, how many approvals should be required. I'm gonna share the link here. that is 5651 issue number 5651 again, by Panda. Yeah, I would encourage you. 

**Sam**
* So this is the more complicated, approval system that Micah had proposed. I don't think I have any problems with doing this. I just think it's complicated. 

**Pooja Ranjan**
* Yeah, I wonder if the suggestion is to be using BOT to get this thing done, like Yeah. 

**Sam**
* Yeah, it is. It's to have the bot like change the approvals over time where the required approvals. 

**Pooja Ranjan**
* Yeah. I mean, if this has to be done by bot, even if it is complicated and it can be put into like codes and can be run, then I think should be fine. Right. So we can probably the next step would be to have, a pull request to the EIPs bot repository to maybe see if this works. Okay. Now we, we don't have Panda on call, so maybe we can bring it up later. 

## Automatically merge all new EIPs drafts ethereum/EIPss#5641 [24.16](https://youtu.be/0miajHm8JXs?t=1456)
**Pooja Ranjan**
* The last one here is, automatically merge all new EIPs and the number is 5641. 

**Sam**
* So I, I'm a little torn on this one because a lot of EIPs still have, like mixed up motivation and rationale sections in, in the first draft. but you know, the formatting has certainly gotten a lot better lately. So maybe we do this, I don't know,

**Pooja Ranjan**
* Actually, I also have an opinion on this particular proposal. I feel like it should not be merged as draft on by itself without a reviewer reviewed by an EIPs editors. Even if bot is doing a good job, I believe there is manual intervention needed at least for two statuses. Number one is when it is merged for the first time as draft. And number two, when it is merged as final, I believe that, we want to create a standard. So the first task as draft is also very important as we have the final pass as final because we don't want to spam our repository with all proposals getting in as draft and it never goes through, different statuses and never reaches to final that will swallow up the repository. I mean, it'll add a lot of, maybe not so useful proposal, even if they are syntex wise correct it if they, even if they are drafted properly. So that's my thought on that. 

**Sam**
* I think that's a really good point. I think you just convinced me that we don't wanna do this. I think a lot of EIPss get abandoned in the draft stage, and so the only time and editor gets to review it is before it gets merge as a draft. So yeah, I think I'm against this. 

**Golvin**
* Yeah, I think we want to encourage people to, start from bigger ideas on the magicians, start of discussion from something closer to an EIPs and let things die on the vine there. but people will work the way they're going to work, and we no longer use the issues for that purpose like we used to. 

**Pooja Ranjan**
* Right. I would agree. So the best way is to like, encourage people to start and have more discussion on fellowship would be like pre-draft section right? Till it is being merged? 

**Golvin**
* Yeah. Yeah. An actual pre-draft status might, might be helpful to keep those sorted out. to make clear that this is, you know, this is an intended EIPs this isn't just a general idea to discuss 

**Sam**
* And then maybe not assign an EIPs number to pre-draft until they actually go into draft. 

**Golvin**
* Oh, definitely do not assign. 

**Sam**
* That's an interesting idea. 

**Golvin**
* Yeah, I think that's Something absolutely no number. Do not call it an EIPs. All it has is a title. 

**Pooja Ranjan**
* Right. And unless we are at a point where, the EIPs number is assigned by EIPs bot, I think, it, we can also call it in the form of pull request. I mean, if not the title, because title sometimes could be hard to find, but pull request number is very easier to find. It. It, it can rest in the pull request. 

**Golvin**
* Yeah. There need not to be a full request. It can, it can live at the, it, you know, the very top entry in a magician's thread. it can be arbitrarily large, marked down, and editable so it can, and it maintains a history. So, a draft, a pre-draft can be maintained there for discussion. It doesn't need any help. from GitHub 

**Pooja Ranjan**
* Okay, let me share the link to Panda, looks like he's around to have to join this meeting. We can, on and see when he joins and if he may have any thought to, we can get back to this one in the essence of time. Let's move on to item number 2. I'm assuming that we do not have any decision, or do we, on this topic. 

**Golvin**
* If I could back up for a second to the patent issue. I, I looked at the Creative Commons license again, and it, it specifically says that it does not, does not affect patent and trademark. and I think that's appropriate, that, that we just not have a policy. it's simply a specification. We don't endorse the specification, we don't certify. it's simply that, and it's totally on the user of the spec, to, to be aware of any patent or trademark issues. And it's perfectly fair for the author to hold patents, with the intent of, of, you know, licensing patents. That's, that's fair. It's a specification. That's all it is. 

## What license to use for EIPs assets [29.57](https://youtu.be/0miajHm8JXs?t=1794)
**Pooja Ranjan**
* That sounds fair. And I believe the next topic that is listed as here for formal discussion is about license and yeah, what license do use for EIPs assets? We discussed this in the past, but I believe there were no, conclusion or decision on that, and we wanted to have a little bit more of discussion here. So, yeah. some, if you would like to give a little bit background on this topic, just jog the memory of everyone here. 

**Sam**
* Some editors want to force all assets to be cc0. And I, I don't want to do that. I want anything that isn't, copy left to be allowed for assets. 

**Pooja Ranjan**
* Greg, do you have any thoughts on this? 

**Golvin**
* I'm not a lawyer. 

**Pooja Ranjan**
* All right. I mean, on a high level, I personally think that when we are talking Ethereum and we are talking about having something as a standard and giving a place in Ethereum repository, we should try to make things as much as open source, free, no patent, no, like trademark things, so people can use it freely, Ethereum is an open source blockchain. We are like trying to, I mean, anyone is welcome to come and use it, so why to add things which may or may not have, permissions to be used or reused, actually. But that's my thought on that. I would be happy to hear other, editors thought on that. 

**Sam**
* Yeah, that's my thought as well. Like if somebody wants to come in with a mandate that you have to use a certain algorithm in an EIPs and then, you know, a year later they start suing everybody, because they patented that algorithm, I think that's completely ridiculous and we should try to avoid that situation. 

**Pooja Ranjan**
* Right. And, now we are joined by Pandapip, Panda. We were discussing a couple of proposals, by you, issues that you have listed, and one of the latest one, which is currently in a discussion is about the, patent and also the use of license for EIPs assets. I wonder if you have any thoughts to share on that? 

**Pandapip**
* Sorry, didn't catch that second part. 

**Pooja Ranjan**
* So it's about the, license usage for EIPs

**Pandapip**
* I'm right next to a road right now when I'm outside and on really, really, really bad internet and a bad computer. 

**Pooja Ranjan**
* Okay, Not a problem. if you can hear me now, we were discussing about, if we should be allowing patenting, stuff or maybe assets, which may have some trademark already or should it be only, which is free for people to reuse license issues. If you have any thoughts on that, probably you can share. 

**Pandapip**
* Well, I think it's pretty obvious that, well, I mean, for one thing, all of the, assets should be, sorry, all the EIPs should be cc0, just so that anyone can just use an EIPs  without having to worry about randomly being sued, like in any case. and I feel like patent and trademark, waivers are just like kind of an extension of that. You should be able to use an EIPs without having to worry about randomly being sued for using it. 

**Pooja Ranjan**
* Right. That looks like general thought process of, some of the editors here too. So, yeah. 

**Pandapip**
* And this is probably particularly relevant for core EIPss because you don't want Ethereum itself to suddenly get patented. 

**Sam**
* Yeah, I don't even know what would happen in that case. Maybe we should include like some patented image algorithm in Ethereum just to see what would happen. 

**Pooja Ranjan**
* Graffiti with that. No, we can't expect that. Okay. is it fair? 

**Golvin**
* I just think that's too much to ask of an author. patents are a mine field. you can't, you can't help but violate them. At Oracle Engineers were not allowed to look at patents because the penalty for knowingly violating a patent was three times the penalty for unknowingly violating it. so it's, it is just a mind feel. The author can't be expected to do a patent search. and it's unfortunate, but it's just a risk that, that the client teams take. I think part of the defense is simply that they're, they're, if they're not being done for money, 

**Pandapip**
* So the particular patent waiver I added is basically the authors. If they have any patents, that they use in the EIPs, then they aren't allowed to sue anyone for using the EIPs. 

**Golvin**
* Well, they should disclose them Right now. 

**Pandapip**
* They're not obligated to though. 

**Golvin**
* That's true. 

**Pandapip**
* So, This basically just means that they don't, they can't patent troll. It has to be someone else, a third party. 

**Golvin**
* We, yeah, we specifically, we specifically say that, that we have nothing to do with them. so I'm generally in favor of just leaving it as it is. I hate putting more requirements on authors and we haven't had any problem yet. 

**Victor**
* I feel similar with Greg. I, I can see the value of, requiring patent to be granted or be disclosed. I feel it's a little bit too, too much to ask. And also, you can't prevent someone who propose an EIPs and influence someone else's patent, if they're not aware of. So I think it's general. 

**Pandapip**
* That's what I'm, what I'm suggesting is that basically the bat wave I've added is that the authors can't sue people for, for their own patents. Other people can other, anytime that it's a patent not owned by the author, it's like, say like some, some random third party, they use some random third party, image image, thing that's, that is, patented. The authors had no idea, patent waiver wouldn't apply there, since it's specifically the authors is authors is, right set are waved. Not those of the third party.

**Victor**
* I'm in favor of, have it optional and make it a convenient way for people to wave the, the patent. because as author, if, if it's a sincere author, the easiest it, it is for the adopters, the better for the EIPs. So any sincere author would try to make it as easy as possible. But I, coming from an industry that cares a lot about patent and EIPs, for like, for, for people like me, I'm, I'm not even sure if I were able to contribute to EIPs anymore if there is a mandate for patent granting because of, other type, agreements that I have with, for example, like my employer. So that, that's the background. So, I when, when Greg mentioned that, in Oracle employees were not even permitted to make, patent search, I, I totally resonate because that's some other trainings I've seen as well. So I, I think we're entering a space of legal practice and, none of us, I, I assuming is a lawyer here on this call. I, I can see the value and a good heart behind it. but I, I think we, we need a little bit more, We might need a little bit more expertise, in the, in a call for, for making it such a strong decision. I, I think optional is definitely valuable. Like making it optional I think is definitely valuable to be, 

**Pandapip**
* Yeah, All that PR does is add it to the template. Authors could absolutely, probably just delete it. I, I, I've seen authors sometimes change the cc0 to something else, which oftentimes gets very quickly corrected. Sometimes it requires a bit of prodding. in terms of the agreements with your employer, that applies to licenses too. You have to get permission from your employer. In fact, explicitly states that in the cc0 license that you have to get permission from your employer if it might be the property of your employer. 

**Victor**
* Yeah. cc0 is much less like copyright Require. 

**Pandapip**
* I could agree. I I am, I am weekly in favor of requiring, there to be a lawyer present, before requiring. 

**Sam**
* I think another thing here is I don't think I want this optional, because I think that would create more uncertainty in the minds of people implementing EIPss. I think we should either leave it completely unstated and that way no, like everybody knows or doesn't even think about it and it's up in the air, or we should do it for every EIPs, if we have some EIPss that give you a patent grant and some EIPs that don't, that's gonna make people really hesitant to implement EIPs that don't have a patent grant. So I think it's better to just, to just not have, or have it not in between. 

**Pandapip**
* So why would that be a problem if people are more hesitant and hesitant to use EIPss without a patent grant? What's a problem in that? They absolutely should be more hesitant. 

**Sam**
* Well, then they shouldn't, they shouldn't be in the EIPss repository. Basically. It's like we want EIPs to be as open as possible, and if we're considering patents for some EIPs, we should consider them for all EIPs. 

**Pandapip**
* If we want EIPs to be as open as possible, why are we even considering not having a patent grant? 

**Sam**
* Because we're, we just wanna ignore the whole patent issue entirely. We're just assuming that there are no patents and everything is open and free, and as soon as we acknowledge that patents exist, we should acknowledge they exist for all EIPs. 

**Pandapip**
* I guess that's fair. Let's keep, let's keep the PR open.

**Golvin**
* We're using the cc0. We've been using it for a while. It's no problem. It's been carefully crafted by lawyers in this domain. It's got precise language on patents, and it's carefully just saying, We have nothing to do with that. This is a specification. Follow it at your own risk. 

**Victor**
* Yeah. And also patent is a very jurisdiction specific thing. I wouldn't be surprised if there's some, even some jurisdiction that doesn't even consider patent, a protected thing. it's, it's very widely used in the western and in, in many countries, but, I don't think it's a natural thing as well. so maybe leave it to the implementers and their own jurisdiction to determine whether, patents in their place is any specific patent is still valid in their own jurisdiction. 

**Pooja Ranjan**
* Right. so, as Panda it suggested, we can probably keep this pull request open, if we have pull request number as I don't see that on the agenda and we can continue discussing on that. Looks like we have the other opinion here. It would be nice to collect thoughts from other editors. Anything anyone would like to like, add to just wrap this up and this topic, in their sense of time? Probably we should move on. Yes, please go ahead, Panda. 

**Pandapip**
* Let's wait for there to be a lawyer on the call. 

**Pooja Ranjan**
* Fortunately we have one person on the call today. She has a legal background, but I am not sure if she is ready to be talk talking on this topic today. Shubhangi, you have any thoughts if you would like to share anything? 

**Shubhangi**
* Hi, yeah, I, I've taught international contract law and, intellectual property law for many years, so I don't teach anymore. but yeah, it's a complicated topic, so, I would rather not, basically what I said in the chat that it may be easier to just talk to a practicing lawyer who's more familiar with the community and can give good advice. 

**Pooja Ranjan**
* That sounds like a fair advice coming from lawyer we can expect this. so yes, if people are more interested, we can probably reach out to foundation team and see if, if there is any, scope for change. though Greg already mentioned that it was crafted very well, taking into considerations of all legal aspects, so we should have our trust in there. But because this is open source, because we always welcome changes, it's good to keep this open for some more time and let's, hope we get some traction from the foundation side. Is that a fair, like, midwat to move ahead? 

**Pandapip**
* Sounds like a good idea. 

## EIP Bot [45.26](https://youtu.be/0miajHm8JXs?t=2726)
**Pooja Ranjan**
* Good. Thank you very much. All right. let's move on to the next topic, which is EIPs bot. We have, a few people on the call. I know there are some progress going on. JA, if you would like to share any updates. 

**Pandapip**
* So there's the, so there's the EIPs bot, there's the other kind of bot I'm working on, which is EIPs bot, but faster and bit less code and not automatically tested. So that's probably something that I'm going to have to, add sooner rather than later. Main upside of it, I think more simple code base, also works with deleting files. the ability to add or remove, basically it kind of works, pretty simple simply. So adding new rules, removing all rules, modifying them, really like that easy. They're all in one place separated by file name. downside, of course, it's been manually tested but doesn't have automatic test cases, which is something that I think about. It probably should be added before it, it's merged. as for the EIPs bot itself, I'll leave it to JA. 

**JA**
* Thank you, Panda. Well, we closed the issue 34. it was PR merge. That was, last week. I just test the, the issue 63, which concerned the fact that the deleting the EIPs 5000 in that time through the EIPs 5255. Actually, it is no problem with the, with any of the two existing bots, the EIPs double double B and the EIPs bot. you are very common in the, in the issue 63 respectively. And there, therefore you will, you can see there the, the test and why the, the bot didn't fail. I mean, basically, just to briefly summarize, if you're gonna delete an EIP file, you are not gonna delete it right in a, a file without the EIPs one format, claiming to delete any EIPs file. Anything straight is gonna be tried to be merged to the EIPs repo must follow the, the rules. And that's why basically the, the bots in that time fail. Not, not precisely because they were not, actually that the fact not, Go ahead. Go ahead. 

**Pandapip**
* That's not entirely true, although the CI was failing there. EIP bot was also failing, because, in, in the code, it's assumed that firewall exist always exists. When a file is modified, ie. Added, changed or deleted, it'll always be accessible. The problem is when it's deleted, that's not the case. it, when it, when the, bot calls, the GitHub API returns a 404 not found, and if you, go to that pull request, hold on, delete. 

**JA**
* Well, I, I don't know Panda. I was testing this, and basically when you delete the file, the, the EIPs bot doesn't even start because the bot activated with the pull request number, which is associated to, to a five please, which is associated to the file that pursuing contains in the EIP. And therefore that that's, that's the idea of the whole bot. just to finish.  The same case goes with the EIP double b, if, the rules start following, following the template for the, for the file, if you want to delete the file, you just go and delete it. You, you try to, to merge it, and it's gonna be, EIPs  doubled P is gonna check the, the template. The EIP is not going run and the CI will run, which just need to consider the fact that there is a, that there is an identifier. What you're trying to, a non-existent file, what you're trying to, or deleted file. What you're trying to match in was of, of course you can, write a, you can write another bot or, Okay, this bot, I just, just as I commending the issue just to consider the fact that you are, the, the pull request I referring to too, merge is just, from the, from the fact that the file doesn't exist. I mean, that's it. That's, that's, that's the best case. But, as it is, it's not failing. 

**Pandapip**
* Yes, it is. Objectively it's failing. 

**JA**
* Yeah, that's fine. That's fine. Whatever you say. 

**Pandapip**
* And I've, And I've, I've determined that this is because the any, I have determined that this is because, files are being deleted. The, PR that's updating EIP 2335, sorry, whatever it is. the diamonds one, the one that updates, that deletes a file, deletes the two files actually is failing with the exact same error. I once created the PR that update my EIP the leader, the file, the assets folder. It failed for the exact same reason. It's very clearly because it's sending a get requested to GitHub APIs, they fetch the contents of a file, which no longer exists. That is the reason why it is failing. Admittedly, there are other reasons why this particular PR can't be automatically merged. The EIPs W issue, the, issues and the hemo, proofer issues, both mean that if, that if we wanted to manually merge it, it wouldn't work. But it is a bug that you cannot delete files. Even if, even if you modify your own EIPs p delete a file on the assets folder. EIPs W, sorry, not  EIPs bot will currently error because of a bug where it tries to bug That. 

**JA**
* But that's a different issue. That's an 90 that, that's an 92, which is not, not the fact that deleting the EIPs file, which is the each issue, 63, that that's what I'm testing on and speaking about. What you're speaking about is the, is deleting a file that belongs to the any EIP that's a separate issue that I haven't tested, but I just tested. Is, is, is the point that you delete on the EIP file and I just retest right now, and, and I mean, it's no problem. 

**Pandapip**
* They are the same bug. It is the root cause. The root cause for both is the same. I happen to know this as a fact. No, Well, For EIP asset, it works for EIPs asset files. It works for, just random files. When I, when I, deleted and added new CI files, it threw the same error, and it's from the same error for when EIP 5000 is being deleted. 

**JA**
* Well, the idea that EIP 5000 was 5000 wasn't deleted for the bot, is because you were not delivering the EIP 5000. What you were doing was trying to merge another EIP that was wrongly configured. Which, which was the, the file that was, I was wanna tell, which is, which is, which is totally different to the case that deleted the EIP file. I mean, you were tried to merge the, the EIP 5255, which the third line was delete a EIP 5000. That's not the, I mean, that's not going, the both are gonna due to the fact that that's not the way that you write. And If you don't like Any EIP, I I mean the, at least that you want to include, I don't know that, that you want to include a condition into the EIPs one that say that when the file says, when the file says the delete an EIP, you're gonna have a particular case say to analyze the, the bot, I mean, to, to, to make the boss wrong. But the reason that this, what you say is true, because, that's a, that's a separate issue. But the issue for deleting an EIP file is, is exactly what I test. I haven't test your case to, I mean, to refer to what you say, and I'm quite sure that if there is a issue open for that is because there is a bot. I actually, we discuss it in that, in that time when we were reviewing the, the open issues. But for this issue for deleting, an EIP file from the EIP repo, I just tested, but needs to be considered into the CI what I see is the case that the, that, that the file doesn't, is not gonna exist anymore. But I recommend that this should be done. I mean, manually, I don't know for any of the editors or whoever is in charge of, which is a person that are the editors, whoever is in charge to maintain the EIPs repo integrity. But the Yeah, I see what now now you understand what you say. You say that that's the other issue that we were discussing, one or two weeks ago. yeah, that, that issue, I haven't yet them, which is the 95, Correct. 

**Pooja Ranjan**
* But Sorry to interrupt you JA and Pandapip. That's, That's Okay. Yeah. Looks like we are getting into weeds this, technical, proposals, pull request and , issue, probably we can take it offline and continue discussing on the Git repository. Yeah. we are on time, like we are one minute past the time. we would like to quickly wrap up this call if that's okay. And we can continue discussing either on the Discord channel or on the Github pull request. So thank you. yeah, thank you JA. And thank you Panda for sharing, the updates. 
* I would quickly like to like just check on the agenda item. We do have EIPss insight and EIPs editing office hours for EIPs editing. The second meeting was conducted yesterday. It went well. We discussed a few pull request and tried to help some new authors with their questions. I would encourage more authors to join meeting if they have any question concerns or if they would like to learn anything about the editing proposal process. And, for EIPss insight, I have already added, the link in the agenda on a very high level. We have 5 proposals merge as draft, and we have 2 proposals in last call with, deadline for proposal 5528, which is refundable fungible token with the deadline is 16th of October and there is another one which is, 4834 hierarchical domains, and it has a deadline of 30th September. So if you are in, if you are adapt developer or anyone interested in either of these proposals would have comment or suggestions or would like to reach out to author, this is the time before this proposal move into final status. So please leave a comment either on discussion tool link added to the EIPs. and yeah, I think, that's all the time we have got for today's meeting. Thank you everyone for joining us today. Hope to see you in two weeks from now. Thank you everyone. Have a good one. 

---------------------------------------
# Attendees

- Pooja Ranjan
- Golvin
- Sam
- Jose
- Victor
- Pandapip
- Shubhangi


# Date for Next Meeting: Wednesday, Oct 05, 2022, at 14:00 UTC


