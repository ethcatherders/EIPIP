# EIPIP Meeting 73 Notes
### Meeting Date/Time: Jan 25, 2023 at 16:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/208)
### [Audio/Video of the meeting](https://youtu.be/z1iQsv2Wt84)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
73.1 | Moderation & governance around community interaction: **So, if we come across any more such issues, we will most likely seek out the moderator of FEM in the future.**
73.2 | Update EIP-5000: Renumber to EIP-5159 ethereum/EIPs#5270: **We dropped the discussion because Matt and Sam were not on the call. To resolve this, we will limit the next meeting to five minutes.**
73.3 | Update EIP-1: Permit links to Yellow Paper and Execution Specs ethereum/EIPs#6306: **Proposal for new external sources under EIP-5757: Very good. So it appears that Sam will consult with Matt, Greg is already in agreement, and if there is no strong disagreement, the agreement will be merged.**
73.4 | Add EIP-6269: Full EVM Equivalence ethereum/EIPs#6269: **The decision is to continue gathering feedback on this specific proposal.**
73.5 | Adds @xinbenlv as an EIP Editor (#5502) ethereum/EIPs#5703: **Present editors seems to be in agreement but decision will be pending @lightclient's thoughts on earlier concerns. Will be added to the next meeting.**
73.6 | What are the prerequisites for someone to be considered a viable reviewer?: **We would seek additional reviewers because the current list is insufficient to continue with the peer reviewing process. So, if you're interested in listening to this call, please contact the EIP editors, Sam, or anyone else and have your name added to the list. It would be advantageous if you have previously authored a proposal, are familiar with the process, and are in a position to review the proposal that is about to become an Ethereum standard. So, yeah, please assist us with that.**
73.7 | Open issues: Issue-6027: Greg is fine with Toggle switch. Can be closed.
73.8 | Open issues: Issue-6131: Greg thinks it will be a good idea. Next steps- Make a PR to update EIP-1 & update EIP bot to add the check.


## Intro [0.01](https://youtu.be/z1iQsv2Wt84?t=20)
**Pooja**
* Welcome to EIPIP meeting 73. Have shared agenda and chat. We have a few items, added here for discussion today. Not a ton of them, but yet, some of them are important to be discussed and probably we can make some decisions, to move forward with. The first item here is, Moderation & governance around community interaction. 

## Moderation & governance around community interaction [0.30](https://youtu.be/z1iQsv2Wt84?t=26)
**Pooja**
* So we all are familiar with, this spa issue that was happening on GitHub. Like people show up to write whatever they want, but with moderation support from EF personnels, we are able to keep it in control and like delete spam comments and one, use it, etc. 
* And we are also familiar with like Twitter trolling and people screaming on Twitter for work and not done as per their wishes. But recently, it was brought to our attention that similar behavior is observed on Fellowship of Ethereum Magician, a place where we think that every developer can share their thoughts about a proposal and probably, share some ideas for governance. 
* So, it was related to the contributors who are trying to help us with EIP peer reviewing process. Obviously people have shared their thoughts on this discord, and, we think it is important to discuss moderation and governance around community interaction for providing a healthy ecosystem to Ethereum users. So anyone here, if you would like to share any thoughts on the issue or suggestion on moderating FEM or EIP GitHub in general? 

**Sam**
* So, so what's been going on? Just like spam or is it more serious than just spam? 

**Pooja**
* I'm referring to more of the conversation, which was shared here in the ECH discord saying the author is, suggesting that reviewer is not capable of doing the reviewing. 

**Sam**
* Oh, you're talking about the, the guy who called me a schizophrenic? 

**Pooja**
* Yeah. Yeah. 

**Sam**
* Okay. I don't know what to do with that. He hasn't messaged me since, or, or they haven't, I don't know who they are. if they're rude to me again, I'll give them a warning and, I'lljust stop interacting with them. But, for the time being, I don't know if we need to do any like, systemic changes, just this one person so far. 

**Pooja**
* Yeah. It seems like that one individual was not only, showed this kind of behavior on FEM, but he was also doing the similar actions on EIP GitHub repository. I suppose there was a link shared by Pandapip, for his earlier action. So I wonder like if, we have any plans, to maybe take help of FEM team or, yeah, I don't know. Greg is here. Greg, if you may have any suggestion for adding warning to these kind of users or maybe having it, like banned or something like that for some time. 

**Gcolvin**
* It just hasn't been an issue in the past, so we've had no real policy about it. But if it's, I hate getting into policies. If it's just one bad actor, you give a warning and you block them. 

**Sam**
* Yeah, it's kind of what I'm thinking too. 

**Pooja**
* Is there a way to report these, people like, in, when we get any spamming issue on Github, we have a forum where we report it to EIP editors and those are banned and like deleted comment and everything else. Can we do similar actions on FEM as well? 

**Sam**
* There's a flag button, so I flagged the messages. I don't know what the mods of Ethereum magicians do, but yeah. 

**Pooja**
* Yeah, flagging is definitely the first step and first good step, in the direction of letting mods know about someone not behaving properly very well. I just wanted to share this, so people are aware. I just want to also communicate that we want to keep, all the discussion forum clean. 
* By clean I mean that everybody is here to contribute, so let's try to help each other rather than like, so if we come across any, such issues further, the end future probably will seek out moderator of FEM. 

## Update EIP-5000: Renumber to EIP-5159 ethereum/EIPs#5270 [4.36](https://youtu.be/z1iQsv2Wt84?t=276)
**Pooja**
* All right. moving ahead. we have few, discussion continued from the earlier meeting. I think some of them were proposed by Sam, but unfortunately he wasn't there. So the first one is, I'm gonna share a link here. It is related to EIP 5000. If I have not mistaken, the pull request number is #5270

**Sam**
* Yeah, renaming 5,000. I don't think we can talk about this today. I don't think we have Matt here and he's feels pretty strongly about this one. 

**Pooja**
* Okay. Yeah, I get it. Yeah, last time you could not do it in your absence. I hope Matt joins later today so we can continue the discussion. Otherwise, I will. 

**Sam**
* I think he's in Austria right now, so I don't think he'll be joining. 

**Pooja**
* Oh, interrupt session. 
* Yeah. Okay. Got it. Very well. I'll add to the next, About 5,000 again. 

**Gcolvin**
* Sorry, I never want to talk about 5,000 again. If, if that's the stupid numbering argument 

**Sam**
* Yeah, I think that's definitely one of those straws. 

**Gcolvin**
* I thought we'd agreed to just have the bot assigned numbers and forget about it In the future. 

**Sam**
* Yeah. But we ha like we haven't decided what to do with Eth 5,000 specifically. I'm okay with just leaving it. Like, I, close the PR

**Gcolvin**
* Yeah, I absolutely do not give a shit what we do with it. So I guess I prefer we just leave it alone and move on. whatever. 

**Pooja**
* Has it been merged? I'm just trying to check it. 

**Sam**
* Yeah. Yeah. EIP 5000 been merged. 

**Pooja**
* Okay. 

**Gcolvin**
* No, really it, it's been merged. It has a number. Some of us don't like the number that it has, but, it's not the only EIP with the number that was chosen cuz someone liked it and it was available. 

**Pooja**
* Okay. So maybe we can drop the discussion for now. Of course. And if people would request then we can bring it back in the next meeting. Oh, though it is open, 

**Gcolvin**
* I'm just bringing it up cuz I'm always likely to miss meetings. So Noted Once again, register in my longstanding opinion that we should drop this. cause I feel like a parent who wants to send their children to the room, say, go to your room, don't come out until you're ready to stop arguing, So it goes Right. No, really, I don't have enough years left in my life for, for this kind of stuff. 

**Pooja**
* I hope we don't get into this for, for very long time and we get it, resolved. unless that, request is closed, I mean someone has to do it, either close it or have the discussion continued. last time we didn't have like Sam, so we could not get through it. Now we don't have Matt, so I hope in the next meeting both are there and we resolve it in time box five minutes only kind of thing. So we do not spend too much of time on it, but definitely, we noted your opinion, Greg, thank you so much for that. 
* And obviously people who are here for a longer time, they're experience and advisor, always helpful.

## Update EIP-1: Permit links to Yellow Paper and Execution Specs ethereum/EIPs#6306: Proposal under EIP-5757 to add new external sources. [8.39](https://youtu.be/z1iQsv2Wt84?t=519)
**Pooja**
*  Moving on to the next, item that is about the updating the permitted links for EIP-1. the number is 6306. just we want to have general opinion thoughts from the present editors if they have, have any objection and having it approved. 

**Sam**
* So I'm somewhat hesitant to allow links to EL, just because we might be changing the process a little bit, but I don't really care that strongly about it. If we want links to ELs, we can do that. And I think, the yellow paper is the other one and I don't really see a problem linking to the yellow paper. 

**Pooja**
* Okay. so from the last meeting, and as I can see it listed here on the comment section as well, looks like, Matt had the exactly opposite, view on that. Like he was plus one on execution specs, but, minus one on yellow paper stuff. So either we have to like break this PR into two and then see if we can go ahead with one. 

**Gcolvin**
* Is this on the agenda? I'm not finding it. Oh, there it is. I need new glasses. 

**Pooja**
* Could we add a comment, like have it, like do not try to have two changes in one PR and then we can take it separately 

**Sam**
* In the interest of not driving this person crazy. I think if we want to do that, I can split it into two PRs. 

**Pooja**
* Okay. Greg, do you have any thoughts on this one? Like any particular suggestion on yellow paper or execution layer? 

**Gcolvin**
* I'm still using my bad eyes to find and this the browser keeps popping up a dialogue with no way to close the dialogue. Okay. Files changed one triple dot view file, wait a minute. This is like from 2015 

**Pooja**
* To provide some additional context. Like, earlier we are trying to avoid, adding links, in any of the EIPs. And with 5757 I think we have, certain links, accepted. But here, this is about, getting permission to add the link for execution specs as well as the Ethereum yellow paper whenever and wherever needed. 

**Gcolvin**
* Okay. So we don't have an EIP for this discussion? 

**Sam**
* No, we, we decided not to have EIP for these discussions. 

**Gcolvin**
* Okay. Is there anything else to read on this or did I just sort of miss out? 

**Sam**
* No, this it is. It's somebody wants to link to the yellow paper and and the execution specs in their EIP  and so they're made a PR to allow them. 

**Gcolvin**
* We need a PR to, to allow them to do that. 

**Sam**
* Yeah. The yellow paper isn't a a source we allow right now. Well, do you want it to be the source or no? 

**Gcolvin**
Yes, it's the yellow paper And, and execution specs. 

**Gcolvin**
* Good. I think they're good specs for writing a client from you can basically port a client from those specs. They're hard to reference for a particular point cuz that point gets spread across the implementation. 

**Sam**
* Yes, absolutely. But are are, are they a valid place to link to from an EIP?

**Gcolvin**
* Yes. 

**Sam**
* Is the question. Okay. Yeah. So you're your're plus one on both of these things? 

**Gcolvin**
* Yeah, the okay. It might be that that linking into the EL is exactly the right thing to do to make your point. and it might not be the yellow paper might be yes, here's this, here's this piece of math which is going to unload into 10 pages of code and other times it's, here's these, you know, five lines of code that unrolled from that math. I don't care about the math, I care about these five lines. that's why I've always said we we're gonna wind up needing more than one spec and just keeping them together and the EL is, is likely to stay current cuz we can, you know, basically keep it on the cycle with the other clients and the yellow paper's just gonna run behind. We sort of need to beg the foundation to get resources on it, to keep it up to date, or else decide that it's trash and just end of life. It. I think that would be very unfortunate cuz the, the academics, especially the formalists and mathematicians, find that they can work with that paper pretty well. and a lot of them would not be able to use the EL at all cuz they're mathematicians, they're not computer program. 

**Pooja**
* So one reason that has been prominent enough, the reason why people do not want links to be added is the chances of getting it changed. Execution specs. My understanding is it may change over the period of time. If I'm wrong, then probably it, could be allowed. same goes with yellow paper. Like if there are no changes expected after a certain point of time, then there shouldn't be any problem in having it. But as per my, knowledge yellow paper is being updated time to time, we had, updated few EIP to them. Yeah. 

**Sam**
* Yeah. I mean I'm okay linking to it. I'll, I'll poke Matt and make sure he's not like, like violently against, allowing links to it and as long as he's not like horribly against it, I'll merge the PR

**Gcolvin**
* There's just nowhere to go otherwise. 

**Sam**
* Yeah, no, I, I I know and that's kind of why I'm okay linking to it too. 

**Gcolvin**
* I think the yellow paper itself, I'm gonna have to bring it up. the yellow paper itself has a, has a version, says what version it's caught up to. here we go. 

**Sam**
* I'm quite surprised it doesn't have a DOI number. 

**Gcolvin**
* That'd be a good idea. It, I think it costs money to get yourself into the DOI system. yeah, right at the top of the yellow paper. I think the current one is, B E A F I don't know what the B E A C F B D means, but it says 2022, 1024. So there is a, they are timestamped. So mainly when you, when you reference it, you should reference the entire, the entire title including the timestamp. 

**Sam**
* I Think the proposed format is to link to the, specific Git hash that the yellow paper is published under. So we can get like a cryptographically secure version for it. 

**Gcolvin**
* That would also work. Yeah, that would also work. it's a little bit less, less useful, but the read me includes, read me includes a link to the PDF. Very few people are gonna download the download the repo and build the PDF  and source. I don't think I've ever succeeded at doing that I've, I've tried. Okay. 

**Pooja**
* Very well. So it seems like, Sam will check with, Matt, Greg is already in agreement and if there is no strong, disagreement agreement is, would be merged and 

## Add EIP-6269: Full EVM Equivalence ethereum/EIPs#6269 [18.38](https://youtu.be/z1iQsv2Wt84?t=1117)
**Pooja**
* The next one number is EIP-6269: Full EVM Equivalence ethereum/EIPs#6269 - I think. that is also related to the same issue that was blocked because, there was no acceptance of yellow paper and execution specs. When we get resolution to that, hopefully we can take care of, this pull request as well. 

**Gcolvin**
* Yeah, this is a hard one. There was some discussion of it. I participated in gas costs was was one of the sticky ones. but I mean this is sort of a marketing term, so it's, it's kind of hard to go in and tell marketers what to say. 

**Sam**
* That's why I'm kind of against allowing this one because like, what is even the point of making an EIP that defines this? It's not like we're like the source of truth or anything. People can completely ignore an EIP mm-hmm. So I don't, I don't, I don't just don't see a point in putting it in. 

**Gcolvin**
* Yeah, it's not, it isn't telling anybody how to build Ethereum. It's trying to tell marketing people. you know. 

**Sam**
* Yeah, Yeah, exactly. 

**Gcolvin**
* I'm just shaking my head at at, you know, I've read marketing blurbs of things that I've done. I'm just going like, that's not even close but you know, they say what they need to say to sell their product. 

**Sam**
* If you could leave a comment on that PR just like a short one or something, that'd be great. If not, like I can write a note. 

**Gcolvin**
* Yeah, I think I did. Probably not to that. If back there were sticky semantic issues, you know, gas is one, you know, there's contracts that depend on it and in some, in some sense, yes, it's part of the semantics cuz it affects the behavior of the code. but in the other sense it really wasn't intended to be a permanent feature of any op code.
*  We're hoping to just get rid of the gas hop code so you can't know how much gas you're spending. and then, then you're down to the definition of semantics. I think in most language design it's, you know, it's pretty much down to what is the output. and gas doesn't change the output except that it changes when your program will terminate. but that's true in other languages. 
* If you blow a stack, your program will, will usually crash. and you can't really know when you're going to blow stack. and the term of art in, I know the term of art in the c++ and I think the C standard is that it will follow these rules, within its resource constraints. 
* And so running out of resources isn't part of the semantics of the standard. so I think we're in that sort of place, but it's hard to explain that to people. but we we don't have a document that precisely defines all of the terms that we're using.  We refer over to the  it's, I don't think it's clear on this. 
* Like we'd have to dig in to what does it say about the ways that an internet client can fail that aren't considered, you know, part of the definition of the client's behavior. They have no idea how big a can of worms they've opened up here. 

**Sam**
* Yeah. Yeah. 

**Pooja**
* Given the like type and category like, in it being an informational EIP, like it would be nice to hear thoughts on like, should this kind of proposal be getting a place in EIP repo  as informational, though it is not providing any specs for design. 

**Gcolvin**
* It would obviously be more reasonable as an informational EIP, but even than I would, I'd wanna see more discussion of these hard choices, probably since you can't just lay down the law on these things. But yeah, be more a discussion of, you know, these are the things that are quite clear. I've seen some discussion of it that just goes into, you know, do we just mean the core computational part of the, of the EVM, but what about that last stretch of call op codes that relates to the environment that it's in? which is a whole nother layer of complication. 

**Pooja**
* Sounds good. So if that's okay, could we just drop this from the agenda, for the next meeting and let the discussion be continued on fellowship of Ethereum magician as we can see that, it's already getting some traction and people are sharing thoughts over there. 

**Gcolvin**
* Yeah. They may want some feedback, you know, beyond that discussion, more feedback from the editors that this should be informational. and as such should probably incorporate more of the discussion in order to be informative. but there's just nobody in a position to lay down the law on this. 

**Pooja**
* Yeah, I think the proposed proposal is an informational type. 

**Gcolvin**
* It's okay. It's, Yeah, this is a hard one. 

**Pooja**
* Okay. So I know it was requested in the comment of, this PR to have it discussed in EIPIP

**Gcolvin**
* And Well, I'll make a comment there if, if I have time,  I'm looking for a job so I'm pretty busy with that and I'm trying to get a startup going so that I don't have to look for a job. exciting. It is. We have some really cool tech, but monetizing tech is always hard. 

**Pooja**
* Very well. So, Greg, if you can drop a comment, to this PR, that would be nice to have and we will add in the, like, discussion section. The decisions is like, is to continue getting more feedback on this particular proposal. 


## Adds @xinbenlv as an EIP Editor (#5502) ethereum/EIPs#5703 [26.06](https://youtu.be/z1iQsv2Wt84?t=1566)
**Pooja**
* Moving on to the next one is, 5703. it was brought to EIPIP meeting a couple of more times earlier. we mentioned the last time that we should bring it back after a few weeks to see where EIP editors are on this proposal. So this proposal is to add Victor as an EIP editor. Victor is here with us in the meeting today. And yeah, Greg and Sam if you guys have any thoughts on that. And yeah, we do have Victor, so if you have any questions for him, I have nothing new to add. 

**Sam**
I think this would be something that needs Matt again. 

**Pooja**
* Matt is on unavailable on a very good day. 
* Victor, if you would like to add anything from the, the last conversation

**Victor**
* I left some, my, have some of my thoughts and read writing and love to, hear what people think and get some feedback. And I do see the, the re this capacity of, EIP are not catching up enough with the, big development in the activities of ERC proposals. So we wanna kind of provide my capacity to help. 

**Sam**
Yeah, I think we're definitely are short editors for rcs. and you know, I think I've gotten to know you reasonably well, so I don't think I'd have a problem adding you as an editor. but that, that's the same, I think as last time. I think the big Matt, I think is the biggest objector. So I don't know if we can do anything until Matt's here. 

**Gcolvin**
* I've talked with Annette about this a little bit and mentioned it many times. I haven't been in a position to do any work on it, or at least I haven't done any. But, we really, I think intended for the magicians and working groups, to, to help here a lot more. And I, the working group concept I don't think is really panned out that well. Partly cuz we just don't do enough in person and partly, I don't know why, but anyway, if you have more of a peer review process than the editors more have the right to, you know, finally merged at that. 
* Thing, but, we shouldn't need tons of actual editors to, to do the, the review of these. you know, it, it seems that for any given ERC there, you know, should be one or two people in the community who can take a look at that, and review it with some amount of subject expertise. there's just so many of them and they span, they span on a wide range of a wide range of topics. and I don't, I'm not sure what a good way is to, to pull in peer review. 
* Some journals I know will ask the, the author to recommend reviewers. 

**Victor**
* Yeah, I am. Yeah, I'd love to kind of help out in, if needed to design the review process. But I guess the question now is for you to see what you're feeling about adding me as editor, so that I can kind of, help out, or do you confer that I stayed out of, a not, stay out of editing and kind of help out in other way? 

**Gcolvin**
* Oh, I would like to add you as an editor. This is a more general point that we need a way to get people reviewing particular ERCs without  a commitment to review lots of them. most people don't care about most ERCs 

**Sam**
* Yeah.  I would say the, the big list of peer reviewers that I compiled has 90% been completely useless. So, we need to go back to the drawing board on that one. 

**Gcolvin**
* What, what if we ask ERC reviewer author to find a reviewer? 

**Sam**
* I think we try to do that. I mean, I do when I mm-hmm. like talk to people, but yeah, I don't know. We'll, we'll, yeah, we can do that. I think that's a good idea. Just make it a, a general policy to make a comment saying that they should nominate and add a reviewer,

**Gcolvin**
* Nominate, ask for volunteers. I don't know, the magician serves as  a good forum for discussing things, but it's been a hard way to, to get anyone organized to do anything. 

**Victor**
* Thanks, Greg, so can I, also, I appreciate your encouragement and, for Sam, can I get a sense of, do you prefer me to stay out of editing or do you prefer me to kind of continue add, contributing on the editing side, I, when I get rejected from the, being added as editor, I saw the  being puzzled, like I, I'm not sure what, what it means, like, am I not editing in the right way? If so, then what is the area to improve or kind of, what is the signal that, that you, look in your mind? 

**Sam**
* I don't think I'm opposed to you being an editor. Like I think you've demonstrated, like, you give good feedback, you participate in the process. Like, I think you've met all of the, like, technical, like you've met all of the bars that I would set for your contributions to be an editor. I think, like, that's great. I think you've, you've definitely,  at least you've said that you're willing to put like the principles of the EIP thing above like above your own, for like this part, for the process. Like, you know, you are okay with, you know, not allowing, like allowing Origins that charge for lengths will, like, I'm not, and I think those kind of discussions are good, but you're okay enforcing the rules as we decide as editors, and I think that's, you know, the, the most we can ask for new members. so I don't, I don't think I have a problem with you being an editor. I think you just need to talk to Matt. He's the, the only, the only person who is like, very much against It. 

**Victor**
* Yeah. Let's talk about Matt's. so I saw the different behaviors in Matt's, or different standards in Math  activity. What happens is that on the items of, numbering 5000, despite that all EIP editors were agreed to put on hold, he go ahead and issue a number and decline other people's request to revert his, yeah, his editing. And then in the same situation where three editors shows Elise, I think Panda and Greg shows support in my being editor, and you at the time was supporting, but now even if you're neutral, was executing adding me as an editor, and then so he come up and respond, no. So, how does governance work in this situation? I mean, in Matt's own standards, should, a general consensus be adopted or should generous consensus be able to blocked by one editor if it's okay to be blocked by one editor? 
* Then back in the time Matt was an editor and he blocked it and Matt go on and, and executed. So I'm curious what our, governance approach, is to this type of disagreement. 

**Gcolvin**
* It Used to be very informal, but we never used to run into this story of stuff. But we disagree and we keep talking until we reach consensus.

**Victor**
* That usually means that a person that speak the loud enough is able to bake, basically bot blocked anyone else, right? Like I, because the reason I asked is not about personally, but in general, in any community, if that is the approach, then the person who stands down, still would get the best of the, the most weight of it. And then it basically, per paralyzed the system. if someone's trying to block, well,

**Gcolvin**
* Personally, I think we're just, we're imposing too high a standard to get things into draft. lots of things I think we could handle in the review process. we're, we're trying to impose on draft, and that's, it's making it harder. It's making it harder on us. Anyway, yeah, it used to be a draft was just a draft, and pretty much if it, you know, if it was readable English and, and met the formal standards, and the formal standards weren't that hard, it got in as a draft, and then when it went to review status, there was plenty of time to, to deal with these things. But anyway, we didn't used to have a lot of trouble reaching consensus. and it wasn't a matter of who talked loud as it was, you know, finally, you know, getting consensus on the arguments. but things have changed. We have more people, and stronger opinions apparently, but in general, in such situations, Matt has to decide is, am I blocking? You know, it's really so important to me that I won't let this person be an editor, or I don't want him to be an editor, but if everyone else is for it, I'll stand aside and that just express my opinion and move on. And so it's, it's kind of Matt's call there and then it becomes the group's call to say either, okay, this is a legitimate block and we'll move on, or, okay, we've heard you, we've heard you out, Matt, but we don't feel that you've got legitimate reasons to block this, and we need this editor. We want this editor, and we're gonna move on despite your objections. and if your objections are so strong that you want to quit being editor, well, we're sorry. And as I said, I have not wanted to pay attention to this, so I don't know at what state we're at, but I think it's kind of up to Matt to make it really clear this is so important to him that he'd rather stop being an editor, than to go with the consensus. 

**Victor**
* Thanks, Greg. I think that's very clear to me. 

**Gcolvin**
* Yeah, th there's , there's three states. Either you agree with the consensus, you disagree, but you're not gonna block it or you block it. And then if you block it, the whole group has to decide to do what has to decide what to do with that block. and really consider the arguments for the block. The arguments then matter, not the opinion, the arguments.

**Victor**
* Thank you, Greg. 

**Pooja**
* That's really helpful. Thank you, Greg. So, while Matt is not here, I don't see a point of having, continued discussion on, on the topic. like maybe, he may have a different.  I don't see a point of having, continued discussion on, on the topic. like maybe, he may have a different, opinion by this time by looking into your contribution or by looking into the argument, or the comment that you have added on the pull request. we should wait for his, thoughts as, Greg mentioned that we would come back to his points, why it was blocked in the first place, and if that holds true even now, then the blocking could be continued. But if that does not hold correct at this point and it has been addressed, so probably we can go ahead with that. But in his absence, I don't think it would be good to come to a conclusion.

**Gcolvin**
* Agreed. 

**Sam**
* So we table this until Matt's here, I guess. 

**Pooja**
* Yep. I hope he joins the next meeting so we can come to a decision on onboarding sooner rather than later. Agreed. Thank you. 

## What are the prerequisites for someone to be considered a viable reviewer? [40.10](https://youtu.be/z1iQsv2Wt84?t=2433)
**Pooja**
* Let's move on to the next item, which we kind of partially discussed in this, prior discussion of, adding one more editor. So it was, from the last meeting, Sam, it, may be, referred to you. We were trying to understand the prerequisite for someone to be considered as a viable reviewer so we can help you like, get more reviewers and if there is any documentation or any resource that we can point it to new EIP authors or authors who are experienced, yeah, they can follow and help with the peer reviewing process.

**Sam**
* There are no requirements to be a peer reviewer. You can just let me know. I'll put you on the list and then you can, I'll ping you sometimes That's it. 

**Pooja**
* So is that list available with  all EIP editors, maybe placed somewhere or how it, yeah, there's a Hack MD that I've sent to all the editors and I can do it again if anybody needs it. 

**Gcolvin**
* Anybody can show up and review. Yeah, Exactly. It's just these, this is a list of people that have volunteered to be messaged and like directly, like named Yeah. To do a review. So That's great.

**Victor**
* I Have also been kind of test out this new, another approach  in compliment to that. And I wanna hear editor's idea, feedback on this approach. whenever a new ERCC or EIP was fired, I would jump in and ask, Hey, have you seen this other EIP p if so, like, can you elaborate your difference or how your dependency work out and maybe reach out to collaborate? And if not, then or if they reject it or you intend not to just, mention that in the merge. So I kind of use that as a way to both force them to do some more research, elaborate, and also kind of find an opportunity for them to ping and discover the, discover and ping relevant editors and new, relevant, authors so they can have a chance to, to talk using that as a one way  to trigger ad hoc reviews.

**Sam**
* Yep. Sounds good. 

**Gcolvin**
* Are you talking about, proposals that are closely related, but the authors may not know that? 

**Victor**
* Yeah, I would generally try to kind of, put down what I think is rel sound looks relevant or sounds relevant, either relevant in that they solve the same problem and they're competing or relevant in that it might be useful to be dependency of one another. and then I'll ask them, what they think about and encourage them to reach out and, and ask for either reviews or collaborate or make a decision to compete.

**Pooja**
* Would you mind maybe documenting that Victor and share it?

**Victor**
* Yeah. I think that's what I put down in the EIP author handbook just to say that you should do research and you should reach out to people who have relevant EIP. And then I'm, and I was waiting for this group to approve that into a, informational, EIP so I can point people to, from a more, canonical links. 

**Pooja**
* Okay. I think that is coming from the last meeting, if I have not mistaken, the strawman proposal. Are we talking about that? 

**Victor**
* Oh, the straw strawman proposal is a different, okay. It's relevant related, but, slightly different. It's about what qualification do you need to have to advance as a, to the next status because people come up asking, 
* Okay. Yeah. So that needs to be addressed. I don't know if we will have enough time today.

**Pooja**
* Yeah, Yeah, yeah. I think, I have, made a mention, to an earlier document that was published by Ethereum Cat Herders stating like, for which status, what we need to have, if there is anything more to it. happy to update that, but yeah, I'm not sure, I do not have the link handy for the, editor's handbook that you are talking about. if you would like to share for rest of the editors to maybe take a look. 
* Okay. So that's mostly related to issues and pull request. Those were added for today's discussion. And we had quite a few discussion on, the peer reviewing process as well as Sam mentioned that we would be looking for more reviewers because the present list is not good enough to continue with the peer reviewing process. So if anyone interested listening to this call, please reach out to EIP editors, Sam, or anyone and have yourself listed. It would be helpful, if you have already authored any earlier proposal, you know the process and you are like, in a position to actually review the proposal, which is coming up next to become an Ethereum standard. So yeah, help us out with that. 

## Close Open Issues [46.22](https://youtu.be/z1iQsv2Wt84?t=2782)
**Pooja**
* Moving on, the next supply I have listed here is open issues. I'm not sure if we can take all the issues today, but if people can quickly take a look and let us know which can be closed because now this is like growing. It's, 18. Yeah, I can see 18 here. Anyone has any thought on any of the issues that can be closed by just taking a high level look here, A quick skim? we should not hide stagnant. 

**Gcolvin**
* It withdrawn even that's a maybe, but not stagnant. Cuz stagnant, they just get moved automatically. And so you don't know whether the author is intending to, get back to work on it in the future or not. and on the page, on the page that I think the foundation maintains that pulls out all the EIPs together, the stagnant ones will just disappear. and I don't think that'll be at all a good thing. I think I've got one or two that have gone stagnant. but they're still referenced by other people. I'm likely to resurface one of them, but all of EOF has to get in first. So sometime next year I'll resurface it, but if it's fallen off the list and I can't reference it, it gets harder. so if something's withdrawn, well it's withdrawn, but even then it, it can be useful published information. So it just seems, 

**Sam**
* Yeah, I'm, I'm kind of against getting rid of them too. I think we can probably close that one. 

**Pooja**
* So, by closing here means that, I mean we are allowing people to add withdrawn in require section

**Sam**
* Oh, sorry, I thought we were still talking about just hiding them from the list. 

**Pooja**
* Oh no. So the, I think if I am, correct. Are we discussing, the issue number 6131? Greg?

**Gcolvin**
* I'm just looking at the titles on the issues page. Yeah. so the second  6027, it's really small type. I'm sorry. Okay. I really need new reading classes. 

**Pooja**
* Oh, no. You are correct. I think I misread it. So I was like on top five and you were looking way beyond that, so Fair enough. So, no problem. 

**Pooja**
* Yeah. 6 0 2 7. Okay. So we are good to close this. That means we do not need to hide anything like stagnant or withdrawn from the list. Are, is that the correct, understanding ? 

**Gcolvin**
* Okay. Very well. I don't know who maintains that page. If, if they wanna make it a two pager and move them over to a second page, something like that. If they feel like the webpage is just getting too long. I don't know. That's a, that's sort of a webpage design issue. 

**Sam**
* Okay. Yeah. That's panda that does most of that. 

**Pooja**
* Yes. So we can go ahead and close this one. Right.

**Sam**
* I think I'll, I'll rename it. because we, we agree we don't wanna hide them, but Greg, you did say you might be okay with making them less visible. 

**Gcolvin**
* So Yeah, I can understand that. It's a very long list, but it list, it doesn't bother me that it's long, but it, it is a webpage design issue. I just don't want them to be inaccessible. 

**Pooja**
* So toggle button would help there, right? Hmm. Toggle button. I think that is the proposal. We can have a button toggle if people want to see it, they can click on the option. If not, then it would not be.

**Gcolvin**
* Yeah, or just page one, page two. what? Whatever I, I don't care how it's done. I just, if we have a list of EIPs, I want all of EIPs to be on that list somehow. 

**Pooja**
* Okay, that's good. At least we are able to come to decision for one issue. Yeah. Yeah. So we have, about six minute left. if we can look into anything else, 

**Sam**
* Your issue about linking to withdrawn EIP in required. I think we can close that one. There's no real reason to do it except to say like we're using a little bit like a piece from an withdrawn EIP but I don't think there's any technical reason why we should disallow links to withdraw EIP. 

**Pooja**
* Actually the one technical reason was there that we should allow only EIP  which reaches to a finalist status and withdrawn does not complete the cycle. It gets terminated before getting to the final status. 

**Sam**
* But a withdrawn EIP can't be edited or changed or anything. No. So I think it's fine to put it in requires like, it's like even though it doesn't go through the entire process, it's done. It can't change. So I think it's fine to link to it. 

**Gcolvin**
* Well, no, the, it hasn't, it hasn't been reviewed to a state that were agreed that it's, you know, even technically accurate. So  you're linking over to something that might be nonsense. You're just go ahead and no problem Yes, it is. If, you know, incorporate what you need directly into your own EIP at that point. Okay, then. Yeah, but that's my thought. It's, it's withdrawn, so it's, it's as good as gone from that point of view. so maybe in in inter Yeah, maybe as information it could be useful, but so it goes, if it's, if what's in that withdrawn EIP is required, that is, it's normative then. but to withdraw an EIP, no, you can't do that. 

**Sam**
* I was just say, I'm still like, I'm still weekly Okay. With allowing links to it, but , if you guys wanna change it, I can change it. 

**Gcolvin**
* I certainly in the specification section, you just can't, you can't refer to something that isn't a standard of some sort. in a motivation section, you know, you could maybe say that this EIP was withdrawn, and this the current EIP is a replacement for it, you know, it could be of historical interest, things like that. But, I don't think we've really discussed my opinion that we should have different requirements and much tighter requirements for the specification section of an EIP  and much looser requirements per motivation and rationale. so that, that's sort of a different discussion that's closely related, much easier to just disallow it rightnow, and take it up on a case by case basis. Cause I don't think many people will want to do it. Right. 

**Pooja**
* Yeah. This is not a frequent case. we are just trying to clarify it for people who may come up with this in future, like right now, if I understand current, the current EIP bot has this check that it does not allow, any EIP in requires section who the status is, like, prior to the current status of the EIP, say, for example, eip  X has a status of review. It cannot have any EIP  y in, draft status. 

**Gcolvin**
* That's a little harsh for me, but I'm not gonna argue about it. But I Triple E has the same policy that once something becomes an internet standard, everything, everything that it refers to, normative, the i e e has that rule. It also makes a clear distinction between normative and non-normative links. And once something goes to standard, all normative links must be links to standards. So if we're following that model,  which was our original model, the time you get the final, everything that's required has to also be final. or the product, the final product of some other standards organization that we've decided that, that we'll count on. so that's where I'm at with it. 

**Pooja**
* Yeah. Sam, do you think, this is the present model of our EIP and, we can probably have it, like if we agree to this model that we want to have EIP in required section, which reaches two final status, we probably cannot have EIP which are in Withdrawn. Right? We will never have it in final status. 

**Sam**
* Sure. 

**Pooja**
* Yeah. In that case, we may have to make, changes at two places, maybe in the bot as well, as, having it, added to the, EIP-1 probably so people don't get confused and come up with this question again, like what can be added and requires section. 

* Okay. So we are at time and I don't think we have, any more time to take upon any further issues. We'll try to take a few in the next, meeting. I quickly want to, just talk about a few other things. We have added,  EIPs Insight - Monthly EIPs status reporting for the month of January. We have 14 EIPs in review status and three in last call status.
*  The last call status EIP are, I'm gonna quickly check here. that is EIP P 52 67, which is retrieval of EIP seven 12 domain, and the deadline is 23rd January, which has already passed. 
There is another  2135 consumable interface. The deadline is February 1st 
* and EIP-6150 NFT, which is, 25 January. That is today. 
* So if people have any thoughts, comments they would like to add last minute, comment for authors, please go ahead and do that. Otherwise, these proposals can be moved towards the final status with, addition of a new pull request. 
* A couple of quick announcements. Ethereum magician, Anat and Victor from Ethereum Cat Herders have organized a session Eth denver on I think it is on March 2nd. 
I have added the link here in the agenda for people who are there in Denver. Please try to attend it. It is a session for all EIP authors. You can come and talk and meet other people, meet other authors, share your idea. Probably we can get some implementation of these proposals during the the devner,
*  there is another one interrupt Summit. we have a governance session there. I and Matt would be there. so people, if you are around, please try to join us, share your thought with us. And, yeah, I think that's pretty much it for today. I have had a look on the action items from the last meeting. I think we have covered almost all of them. Yeah. Anyone else has anything to Yeah, share? 

**Victor**
* Yeah, just really quick, I left the notes here. generally it is the topic proposal job to client document meeting notes, but for, 5703 pull request, that adding me as added, I should probably recuse myself. So who should be the best to kind of, document this, whether we discuss today? 

**Sam**
* I'm perfectly fine with you documenting it. 

**Victor**
* Oh, can you, Sam, can you, I, I wonder if you actually, you, it would be better for you cuz you are least neutral. If you and I, I apparently cast the bias. So our discussion today, yeah. 

**Pooja**
* I am going to leave a comment, at the end of the agenda, with whatever we have decided with for today's discussion. I'll try to include it over there if that's helpful, Victor. 

**Victor**
* That will work. 

**Pooja**
* Yeah. and like from the past meeting, I have started this as a practice that whatever we conclude in the meeting should be added in the agenda so people get an idea on a very high level what was discussed in the meeting if they missed attending that meeting. 

**Victor**
* Sounds good. Yeah. Thanks. Yeah, I, yeah, I usually document, but, this one actually I should recuse for. Yeah, Not A problem. Cool. Thank you. 

**Pooja**
* Thank you everyone for joining us today. I hope to see you all in two weeks at 1600 UTC.


## Date and Time for the next meeting

Feb 08, 2023 at 16:00 UTC

## Attendees

* Pooja Ranjan
* Sam
* Gcolvin
* Victor Zhou(@xinbenlv)



