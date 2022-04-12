# EIPIP Meeting 53 Notes
## Meeting Date/Time: Wednesday 6 April 2022 at 14:00 UTC
### Meeting Duration: 1.1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/118)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=5VbbS-3MQss)
### Moderator: **Pooja Ranjan**
### Notes: Jim Bennett

----
## DECISION ITEMS

**DECISION 53.1:** Don’t rename "Master" branch to "Main" branch [see 08:24](https://youtu.be/5VbbS-3MQss?t=50t)


**Pooja Ranjan**  
Welcome to EIPIP meeting 53. I just have shared the agenda in the chat. And we see some new people on the call today. Do we want to go with a small introduction, brief introduction, if anyone is interested, and then we can get into the agenda items? Anyone if you would like to go ahead first.

**Zainan Victor Zhou**
00:30
Okay, I can go first. Yeah, hi, everyone. My name is Victor. On GitHub, I go by XINBNLB. And I am the author of ERC 1202 and EIP 2135: It's a voting standard. And the other one is a consumable interface. And I joined this meeting because I think it's a little bit harder for me to see how to move forward on it and how to get adoptions and how to discuss to get more consensus. So looking forward to your advice and guidance here. My name is Victor. Thank you.

**Pooja Ranjan**
01:16
Thanks for joining, Victor. All right, Greg?

**Greg Colvin**
01:26
I’ve been at this so long, I can't remember. But for editors, I'm not quite an OG, but close. Me and Hudson and Nick pretty much put together the current EIP 1, and then then some of you people have made a lot of changes. You used to have only two statuses.

**Sam Wilson**
01:56
Hey, I'm Sam, I'm responsible for breaking a lot of changes that Greg mentioned. Well, a few of the more recent ones anyways.

**Pooja Ranjan**  2:19
We have one more new person. He is Jose. And Jose, if you would like to introduce yourself briefly, please go ahead.

**Jose**
Yeah, thank you. Hi, guys. Since two weeks ago. Helping, learning, try to contribute for the issues in the EIP bot. Specifically, we have been trying to get issue 53 and isue 58 and actually trying to figure out about issue 55. Well, thank you for the opportunity. I am here for, as I say, learning and helping. Appreciate.

**Pooja Ranjan**  03:11
Right, we can get into those issues maybe later on the agenda. Well, thank you so much for joining us today. Alright, with that, I think we can now just get into the items that have been listed here for today's discussion.

## AGENDA

## 1. [Rename master branch to main branch](https://youtu.be/5VbbS-3MQss?t=209)

The first item is renamed master branch to main branch. This item was requested at the EIPIP issue section. And also at the EIP GitHub issue section by Banta EIP one hour he has closed the EIPIP issue, but that is still open at EIPIP GitHub issue. I think I have added the link. So if people want, they can take it there. And he listed a list of if he didn't GitHub repositories or where this change is requested. It seems that there was a voting to rename it as well. I don't know what other editors have to say on that.

**Micah Zoltu**  04:16
Voting - what are you referring to the voting?

**Sam Wilson** 04:19
There is a thumbs up / thumbs down form of voting on the issue.

**Micah Zoltu**   04:26
I'm not a huge fan of democracy personally.

**Pooja Ranjan**  04:33
Well, I think I'm more curious on understanding if we really need to have this thing done. Do we really need to rename? What is breaking if we do not rename it?

**Sam Wilson** 04:45
So I think the argument for doing it is that it might make the repository less accessible to people who find the term “Master” offensive. And the argument against it is “master” is a commonly-used word, and it doesn't necessarily have those connotations for everybody.

**Pooja Ranjan**  05:13
I didn't know that. Any other thoughts that people may have?

**Micah Zoltu**  05:26
Just to reiterate what I said in the discussion, my general feeling is that if we retain it, it will offend the people who are against the renaming. If we don't rename it, we'll offend the people who are for the renaming. So in order to remain credibly neutral, I think we should do nothing. And in this case, do nothing happens to side with the people who prefer the term “master.” But that's the most neutral path we can take. Because it's basically follow the defaults.

**Greg Colvin** 05:55
It’s been Master for so long. Why would we want to create confusion by changing it? I think Master branch and so many GitHub projects

**Sam Wilson** 06:23
I don't know. It's a difficult topic, right? And there is precedent in the Ethereum ecosystem for making the change. Like changing “suicide" to “self-destruct.” And I think this change has a more technical side to it than that one did. But I just want to make it clear. I'm actually against the proposal. I just think I'm the only one here who would argue for it.

**Pooja Ranjan**  06:51
So from what I hear, I think all three editors are against. If I get you correct, Sam, you're against the proposal, right?

**Greg Colvin** 06:57
I'm very weakly against.

**Pooja Ranjan**  07:04
I think the counter argument here, as mentioned by Greg, is that we have been using Master for so long, why confuse people? Whatever changes we make, it requires a lot of information sharing in terms of making the community aware that this change has been made. And even after years, we find our people coming back to us, and we were never aware of what the changes are. And I'm not sure if there is a hard and fast necessity to change it, just renaming it for the purpose of this. I would be happy to hear others thought as well. But I think three of the editors out of five are voting no for that. So considering this as EIP, especially for EIP GitHub repository, I would like to collect more thoughts and see if there is gender change on the other repositories of Ethereum. If they agree to change it, maybe that would be a good way to proceed.

08:04
I think that's my biggest concern. If we do make this change, it should be uniform for all repositories under the Ethereum organization. And also, we probably shouldn't discuss this too much today, because the issue’s champion is not on this call, as far as I know.

**Pooja Ranjan**  08:24
I agree. So we can just communicate that this has been discussed in the meeting. And this is what most of the people in the meet people present here. Thanks. But anyone, if you aren't strongly in favor, please speak up. So we can update the issue accordingly and see what the person wants to keep it on. Or close the issue. think you're muted,

09:01
I'm very sensitive to the issue, especially as an American and our horrible history with that. But it does seem like a lot of disruption. So we should move into it pretty carefully. And I noticed that GitHub has changed it for new repositories they’re creating, but they're not going through and changing existing repositories. Right. So we start rearranging the other thing.

**Pooja Ranjan**  09:47
Right, that's right. So I think in this meeting, we are specially discussing issues which are related to the EIP GitHub repository, and because that is a part of Ethereum GitHub. So we will wait for making any changes on our end until it is done at the organization level itself. Does that sound like a fair consensus for the group? Well, if no one opposes, then I would consider it like this is the general consensus, the draft consensus. Isn't the draft consensus on which we generally try to handle things here? Alright, so we will keep it there only.

AGENDA ITEM #2

Moving on to the next item: discuss appropriate date for Created in EIP. So this item is added based on the recommendation from the last meeting. The group was discussing useful and possibly less useful field have an EIP that we have at the moment. And it was brought up that how confusing dates can be. So I wanted to bring it up to this meeting today so we can get more feedback from people. What do they generally think of having a “Created” field in the EIPs? For example, I'm taking ERP 4430: described transaction. This particular proposal was documented on 7 November 2021, but it was merged just yesterday, that is 5 April 2022. But when I look into this particular proposal in EIB s.edm.on, it looks like the Created field will show the date on which this proposal was documented. However, it can be very confusing for people, if they are referring in later future, that the Created means that it was created in November 2021. But definitely it was not available for anyone until April 2022. So I want to just check, what is the general thought? How do we want to see this thing?

Micah  11:59
My personal preference, in an ideal world, the rainbows and unicorns would be that the Created field is automatically filled in, and it's based on when the file was initially added to the repository. And this would all be done by CI, and we will not have a field. In the EIP itself, it would just be like when you look at the eip.ethereum.org, it would be generated automatically from the file creation date. That being said, I recognize there's a non-trivial amount of engineering effort to achieve that. And until we have that, I don't think like I can appreciate the desire to keep the Created field.  On a more personal note, I personally find no value in the Created field. I don't care what they tell you. It's great. It doesn't matter to me. And so I don't know, if everybody else is okay, I'd be totally fine. I just ruined field entirely. But maybe other people have a reason that they think it's valuable, in which case I'm okay with keeping them as well.

12:58
I like seeing the age of an EIP. So until we have a technical solution for it, I think we should keep it.

**Pooja Ranjan**  13:11
Greg, you might want to unmute yourself.

Micah  13:15
Just assume Greg is talking to himself.

13:18
Yes, my internet connection keeps dropping. So if I seem to have gone away, it's because I've gone away. Yeah, it's useful for showing more or less how old something is. A precise value doesn't matter that much. But if it's six years old, it's good to know that.

**Pooja Ranjan**  13:43
Well, in that case, it looks like that the best middle way would be to keep looking for someone to be maybe able to update the value of the field as the merge date of the draft. And until we get there, we continue having it on the EIP the way it is, but definitely we keep our search on. Maybe we can create an issue to get this field updated by CI, and let's see if we can get some contributor working on it. Alright, maybe we can add it as an action item, we create the field and keep looking for people who may be able to contribute on this part.

ACTION ITEM 53.1: Look for contributor to get the Created field updated by CI.

AGENDA ITEM #3

Item number three is Discuss EIP status that may or may not be added to a new proposal. So this item is added based on comments that we have found on Fellowship of Ethereum Magicians for some of the EIPs - definitely more than one. That's why I'm saying some, because I could not read all of them. We actually organize a Peep an EIP meeting for a few core proposals in the past week. So I'm taking examples of those - proposal number is EIP 4895 B contained push withdrawal as operations. So in that particular proposal, there is a mention of EIP 4788, which seems to be an alternative method of getting be contained withdrawal. done on the mainnet. This proposal is in Draft, but most likely it will be dropped because we have to go with one proposal. So, if we are going with 4895, we will not be going with 4788.

Micah  15:34
Yeah, so I'm pretty strongly against having Final yet to use Reference Draft or Draft. The reason for this is because drafting views are highly mutable. We’ve had people in the past who just take the EIP and basically rewrite the whole thing before it gets from Draft to Review or Review to Final. And so that mutability means you're effectively linking, you have some final EIP that is supposed to be a canonical specification for a thing, linking out to another EIP that is completely mutable, and may be something totally different in the future. And so what I generally tell people is, just take the key points. Often this comes up like the issue you mentioned, where someone is saying, “Hey, here's an idea.” And then in the rationale section for when we're describing why we didn't do something else, they say, “we didn't do this other thing.” And then they pointed to the other thing that will never make it past Draft. And they say we didn't do the other thing, because XY and Z. My general recommendation is people just extract out, a one or two sentence description. Yeah, the other thing and include it in line. The rationale section is just to give people some some answers to common questions and reasons why path A was chosen and sort of bumpy. And I don't think it's necessary to link to an entire specification, especially one that is going to be mutable, and I wouldn't rather see them include an immutable short description, that stands the test of time.

17:06
That doesn't work. In the in the Ethereum work, we've got a collection of EIPs which are mutually interrelated. And just having a sentence or something is inadequate that they need each other.

Micah  17:25
So this is very specifically for EIPs that are mutually exclusive. Like when you have a set of EIPs that need to work together, I'm totally okay with linking between them. This is when someone has an EIP that says it like sometimes people will create swim up there like two different solutions to that same problem. Only one of those solutions will ever make it to final, the other one will just die and it will go away. And

17:51
so why would only one of them make it to Final, but you finalize an EIP even though it's never adopted?

Micah  17:57
So this is for CoreDevs? If he’s specifically in CoreDevs, if he's on the current process as CoreDev, if you've only get to Final. The final equals Ethereum. We've talked about having quite a peaceful listening similar to ERC is where, you know, you can move to Final if you want, whenever and unrelated to the Ethereum mainnet launch, but that got a lot of pushback from CoreDevs. They want the EIP status to be correlated with mainnet.

18:29
I'd much prefer having them separate and then having an adopted header field that actually lists what hard fork it was adopted in. Makes more sense.

18:39
No. I'm sorry, I guess my feelings, because because I was there when certain decisions were made. When the editing is basically handed off to the CoreDevs to do what they need to do, and a final standard that was never on the mainnet is not final, it can be changed at any time before it finally gets on to the mainnet. Otherwise, you'll need to go back and edit it before it gets on the mainnet, because things on the mainnet can have changed. We went through this with 2315. It was going to go on the mainnet and was yanked out very close. And I decided to keep editing 2315 rather than throw it away and start over. Was that the right decision? I don't know. But other attorney EIPs it'll just be not quite, but later. It's just the EIP process and the CoreDevs process were never intended to be totally tightly intertwined like this. So if a core EIP was not to be final until it hit the mainnet, people wanted some sort of Final status for non-core EIPs. So that people trying to implement systems that depended on each other could point to the EIP and say, “This is the standard. If you want to interoperate, we all need to follow this standard.” So you need a Final there. So having a final EIP for a core EIP that has not been put on the mainnet really means it's not vital.

Micah  21:00
Yeah, I think that summarizes exactly what Greg said. And what other feedback we got is that, because EIPs can change up to the last minute before they go into onto mainnet, that's happening, I feel we find bugs in the EIPs right up to public test networks, and sometimes after the public test networks. And when those changes happen, we need to be able to rapidly iterate and so pragmatically, we can never make any EIP final because by all means, so if we maintain the stance, that final means immutable, then we cannot make any EIP final until after it hits mainnet, because it's not until it hits mainnet that we actually know that it's not going to change, like with a bug fix or something. And so because of that, even if we don't have like an actual assertion that core EIPs can't be final until they hit mainnet, medically, that's what ends up happening, because we can't reasonably say they're immutable until we're sure that's what's going on to mainnet. Maybe we could, but we have the problem where we have to tell the core Devs you know, at the 11th hour, sorry, even you if he was already marked as final. So you need to you know, draft a fork of it and create new one get new number, update your code with that new number if you have that number in your code somewhere. Which leads to a lot of problems. And so I tend to agree with with Greg though, perhaps not as passionately?

22:29
No, I think that makes sense. So is there maybe a, a final but not deployed status that we could use, like withdrawn? Or is that still immutable?

Micah  22:40
Last Call is. So first thing is that are slated to go on to main net. And Last Call is meant to kind of serve that purpose for core EIPs, where we're saying we're pretty sure this isn't going to change, but we're leaving the door open for changes in the 11th hour. But if you're referring to things that are like these alternatives, that we're talking about where you've got some alternative EIP that we know will never go to mainnet but we want to permanently record in history, we could we could come up with some status that is final but not deployed and will never be deployed. Just so we can do this crosslinking. It feels weird. I'm not absolutely against it. I just don't want to add too many new states. Like we already have so many states. I don't think we need more of them. I was just thinking if we could use Withdrawn for something like that.

Micah  23:42
I believe Withdrawn can be revived. Withdrawn means the author decided not to pursue it at this time, but maybe at some point in the future, if they decide to pick it up, or someone else wants to take the torch, you can pull it out. So you can keep the number.  Keep consistency.

Sam Wilson 24:02
Yeah, that makes sense.

**Pooja Ranjan**  24:04
Okay. I'm sorry, I think I am lost. So for Withdrawn, is it allowed to keep the number there?

Micah  24:15
So if something goes into Withdrawn, and then later the author wants to pick it up again, I believe we decided you can and so you just move it back from Withdrawn to whoever, maybe I'm misremembering. I know there's a bunch of discussion about this.

**Pooja Ranjan**  24:29
Yeah. I think the section that I can read here from EIP 1 right now, because this has been discussed a lot so I can totally understand how you may be getting confused here. It states that Withdrawn - the EIP authors have withdrawn the proposed EIP. This state has finality and can no longer be resurrected using this EIP number. If the idea is pursued at a later date, it is considered as a new proposal.Even if the text is identical?

**Pooja Ranjan**  25:02
Yeah, we cannot allow the same number, you have to use the different numbers.

25:09
I mean, if that's the case, I'm perfectly happy, like using Withdrawn as like you can link to withdrawn EIPs and Final EIPs. I think that makes sense.

Micah  25:18
Yeah, I'm convinced by that argument.

**Pooja Ranjan**  25:21
Well, my next part of this question was related to a withdrawn EIP. It was for proposal 3855: push zero instruction. And there was this mention of an EIP 2733:  transaction package, which is currently withdrawn, and we know that it is never going to be in the final list of EIP GitHub repositories. Is the mention of a withdrawn EIP okay for a new proposal, or should we try avoiding that?

Micah  25:53
I'm fine with it if we retain the rule Withdrawn as a final state, like Terminal - immutable, like FInal. I’munder the assumption that if we change that assumption, then I’m not OK with it.

26:08
this is getting so complicated. The ITF has managed the internet for a very long time, with two or three statuses. Basically, Withdrawn to me sounds like the author is indicating they don't want it to go in. With the Creative Commons, anyone can pick it up. And in that sense, a new number makes sense. Perhaps this is more like a stagnant EIP. It may get picked up again, it may not. But if it does, it's still basically the same proposal. It's just now time to try it again, because situations have changed.

Micah  26:54
That definition for most people is Stagnant, not Withdrawn. If you have any inclination that you might want to do this in the future, Stagnant is definitely a better choice. Withdrawn is like the author saying, “I don't think they should go in. I am actively against this.” The situation we're in right now with these kind of mutually exclusive EIPs is a great example of this, where the author is saying, “I have decided I want to champion this one. I think that should go in, and this withdrawn one, I don't think should go in as the alternative.” And we can leave them both in Draft or Review right up until the end. And then when one goes Final, the other ones goes to Withdrawn. That way, we get the immutability of the Withdrawn one, so we can reasonably link to it. And it can provide context for some other EIP that didn't go in. And we don't worry about it changing in the future.

**Pooja Ranjan**  27:47
I see hand raised by Victor, you have something?

**Zainan Victor Zhou**  27:52
Yeah. I was about to mention, Greg, that Stagnant seems to be relevant in this context. And also, there is another state called Leaving. If we are anticipating that the  dropped EIP is in a state of that's relatively formal but still you can expect change, then Leaving might also be one of the states that is relevant here. And from an ERC perspective, I also see many proposals that can get into a state that is already finalized but not adopted. So I think if we didn't want to have another state and maybe Final, instead of naming Final but not adopted, maybe we can have one after an option is have one after Final as adopted. And I want to mention the question is also since we, as a decentralized system, we also anticipate that many adopted in that are different than implementation. So if we really want to pursue another new state that indicates the adoption or implementation or go to mainnet, then that will bring up a new problem whether one or two adopted, what would that state be like? So I just want to put that in.

**Micah Zoltu**  29:26
My general thing is that once the EIP is Final, it's done the RFP process and the work that gets picked up by users or used or whatever is a separate issue. EIP 2830 is a good example of this. I think it was that was the access list. No one uses that.I think there's like three access list transactions on all of mainnet history. So one could say it's on mainnet, but it hasn't been adopted by the community, and I'm fairly strongly against trying to define what adopted means. If there's only one person using it mean adopted? And this gets way harder with the RCS where, you know, adoption is one guy using it somewhere on the internet, is it adopted? Or does it need some sort of critical mass? And so I would much rather keep that out of the EIP process. The EIP process kind of terminates at its immutable state, and then some other process can pick up tracking what people are actually using. You know, I definitely see value in the community as a whole having some place they can go to see what are the ERCs that people are actually using out there. You know, 115 is used and 741 is used and 20 is used. But there's plenty of ERCs that no one uses. And so, I do think there's a value that someone could provide and have a website or something like that. I just think that it should be outside of the scope of the process personally.

**Pooja Ranjan**  30:56
Yeah, I would agree the adoption can be different at different statuses, though we encourage people to share reference implementation if I can find any to be added or shared in the EIP. But mention of adoption is something that is after the standardization process is finished. I remember Victor mentioning about leaving a status. I'm not sure if we were referring to some other other blockchain but for Ethereum blockchain, I don't think that is a valid status that we are following for the standardization process, though, there is one which is called Living, but that Living is for only just for EIP 1, because we keep on editing it forever. And that is the only special proposal here. For any other proposal it has it starts from Draft and ends at either Final or Withdrawn. That’s the last status. In Stagnant ,they are kept there for an unlimited period of time until someone wants to pick it and bring it back to life. But once it is finalized, or withdrawn, it cannot be brought back into the process.

Greg 32:27
We're about to run into trouble with that with VM proposals, since they now have a validation stage. And if you add new opcodes that need to be validated, the validation for them will need to be integrated into the validation for all the other opcodes. And you can't just do that with one EIP, necessarily, because you don't want validation defined as do this, do that, do that, do that, do that, and by the way, it's your job to turn them all into a single algorithm. So a living document, where you keep updating the validation constraints and algorithm as new opcodes get added, seems to be what we need. Or maybe that falls into the the core EIPs and executable spec world. Yeah. But anyway, you understand?

**Micah Zoltu**  33:45
Yeah. I'm curious, can you create anew EIP that says the new validation algorithm, as of this hard fork will be x [unclear](https://youtu.be/5VbbS-3MQss?t=2036)

33:56
You could do it that way. You wind up with a pretty big stack of EIPs over time, but you could do it.

**Micah Zoltu**  34:07
Next few little sec. I think it makes me It simplifies that. Yeah, this executable spec succeed, just because you are right. There are situations you know, where you're, you're saying, okay, modify this fairly large and complex algorithm to now do something slightly different. But that's slightly different may require, you know, integration in like five or six different areas within that algorithm. And having that single stack, you know, you can get a diff that shows, you know, okay, here's the three, three things you can change from a reference implementation point of view, which definitely, is much easier.

34:41
But we're struggling with this right now. Because we have some proposals. There's some alternatives. You know, I'm being asked, Well, can you put a PR in this other proposal to show how this is going to change? And I'm like, Well, sure, but I don't see the point. Ain't until we've actually agreed that we want this other one to go in. And we've agreed as to what this other one even is. But it's just sort of a mess. And I'm not entirely sure how we'll straighten it out. I guess for this round, we'll, we'll have one document for the, for the upgrade they're going into, and we can we can work this out later. But it's the sort of thing that a living document might might handle. So you have one place to keep going for the current, the current set of constraints, but it might be the damn executable spec. We'll it will be where we go. And I think that's the next topic.

**Pooja Ranjan**  35:52
Right is there for executable specs. We'll go there. But before we move on from this item, I just want to summarize it for people who may be new for documenting their proposal or for future editors that they can follow this while reviewing the proposal. So from the discussion today, it seems like EIP editor's are on board with a mention of final e IPS as well as withdrawn ei B's, but not any other statuses because any other statuses can change. Is that the right summary?

**Micah Zoltu**  36:31
I fine with it as long as we retain the withdrawn, withdrawn as terminal or change that rule. Then I no longer Okay.

**Pooja Ranjan**  36:42
Okay. Yeah. And as per the present EIP one withdrawn is a terminal status. So final and withdrawn are the two. All right. Moving on to the next item is code EIP is in an executable spec. Walter. I know from the last meeting we did discuss about the proposal that is already on the table by Tim Miko. There is a definition fellowship of Athena magician tried to share comments over there. But I thought that we were also discussing to have alternative proposals. I'm not sure if there is any.

**Micah Zoltu**  37:27
Scrub the wait and see if we buy for 15 minutes, I'm guessing is moving from McDonald's to KFC?

**Pooja Ranjan**  37:35
Yeah, yeah, that that makes sense. So maybe we can come back on this topic. If he's back. In the meanwhile, we can move on.

37:45
So yeah, it's most important topic to me. But yeah, because yeah, Sam needs to be involved.

**Pooja Ranjan**  37:56
That's right. That's right. He he just left a comment that he did back soon.

38:01
It's important because it's moving quickly. And I have I have strong objections or a strong need for for things to change. I've been trying to read the CL specs, and I can't read them. And I don't want to go spend a week with a Python book. And even then, way too much informations missing. Reading, reading, it doesn't give you the concepts you need to understand it. But I guess we'll discuss that just a little later.

**Pooja Ranjan**  38:41
Yeah, we'll come back on that topic. I hope today, if he's back within the time. So in the meanwhile, let's move on to the next topic. So when he's back, we are covered with the rest of the topics which are there for today's discussion. Then number five is EIP bot issues and EAP issues. I know, Jose has been working on issues for bot and the number he mentioned is number 53 and 58. I don't know Jose if you have any question to discuss the process or the approach that you were trying to follow to solve that issue if you have questions feel free.

39:21
Thank you. Well, I basically basically have just one question is what the idea for any author is to follow the eip one expects right? However, having said that, why? I'm sorry if I fail I don't get this great. Okay. Why is so is so is so much going on? about helping They are supporting the Alto to, to follow the AIP one specs per template for writing in the proper way the proposal and I understand that the board is is there to you know, for a definition set for simple issues, but and this is just a question is not suppose any outdoor that want to make a proposal to, to follow the specs considering the all the definition that you have there to fill follow the proposal. I mean, there is something going on that the to make to make to make the question and just shut up and listen to you guys, is something going going out that avoid avoid that also to follow the mark the markdown format for the AIP proposal in the AP One or this is just me that I'm so new and I don't get sorry. That's it.

**Micah Zoltu**  41:09
So I think what you may be asking, and correct me if I'm wrong here is why do we manually enforce if you want instead of having the bots enforce rules that we're asking?

41:24
No, I'm asking that but in the opposite why we need to, to enforce the outdoors that are supposed to follow the eip Wellmark markdown template? I mean, I don't I don't know I don't understand it should be at least the the first requirement to make a proposal that that you will feel follow the the eip one markdown format, at least for the template, whatever.

**Micah Zoltu**  41:58
Yeah, so that that is where you are correct. That is a currently requirements. And the reason we have that loop to make sure the videos you know, when they show up on the website, they're consistently formatted and easy to read once you get to know like how to read up. So we want consistency, like we want you about the same. And right now we do enforce that. But the enforcement comes from EIP Enders when someone submits a PR Theatreland through and say please fix this fleet successfully 60s, it would be better if we had a bot that automatically did all this, we just have not had the time to write about the puzzle that

42:41
okay, got it so. So we can we can leave with the what the idea would be to ensure in the automatic way that the template and the markdowns. Yes, are are fulfilled for the for the outdoors. I mean, fine. I understand that but is going to be always I'm correct me if I'm wrong, is going to be always say a reviewer or editor that is going to approve that. Right.

**Micah Zoltu**  43:15
Yeah, and the editor. So if we had, if we had all of the automation that we wanted, so bots did a lot of the work, then the editor would just kind of read the IP, make sure they didn't have any, like grammar errors, or they didn't have you know, make sure it makes sense. You know, make sure it's readable. It's not spam, less work that editors have editors doing and the more work we can have about doing the better. It's just writing bots and time consuming. And so we haven't done it at all. But there will the plan is to always have editors involved. But we want the editors to do as little as possible. Like ideally, the editors just do one read through and they said yep, this is good. And but okay for everything else.

44:01
Okay, thank you. It's good. Good.

**Pooja Ranjan**  44:08
Thank you for looking into issues. If there are any further questions, you can always drop them as a comment if you think I'm hoping that either the person who created the issue or any of the eip editors may be able to help you answer we're there. So that means speed up and that may not be a blocker for you to continue working on it

44:35
okay

**Pooja Ranjan**  44:41
I'm just trying to look into other questions here change to Eb one with a single editor approval. Okay, I remember it now. Okay, there was this a br That was that is currently merged, I believe. But I think I found a comment like why was it much And why did not wait for autos approval, I guess?

**Micah Zoltu**  45:06
Yes. Or I guess, there's not a bug if no one feature request, which is the means it needs multiple approvals. Like it shouldn't just be one editor approved, it shouldn't be like four or something. And I have a little thing in there, my proposal is just if the change tip one has been open for it was just recently opened, that requires borders, approvals. But the number of editor approvals required decreases over time and down to one like over the span of like two months. And their idea for this is to make it so we don't get blocked. If we there have been times throughout the history of the editing process where we have been down to like one editor for a very long period of time when active editor. And so just in order to prevent us from getting totally blocked, the idea is that the number of editors required to approve change the if one decreases, the longer a change is open, just so that if we've got lots of editors, then you know, we need more consensus. If we're to one of the in one of those dry spells, where we have one active editor, we can still make four changes, though. And then also, if any editor rejects the change, then it should block me entirely. So it shouldn't be like a one person rejected. And I always have to wait for responses. If someone actively rejects the change, then it just stops right there. And so there's a feature request after the bottom. Great to have automation on, we don't at the moment. And so if anyone's looking for opportunity.

46:48
Either confused here, I think I I made a PR on on AIP. One, I should have made a draft. But I had and I was a bit confused and making it that it actually wasn't the right way to change things. And I think we were all surprised when it just suddenly merged. I'd never actually approved it. It seemed like just because I was an editor that just said, Oh, okay, put it on in. So

**Micah Zoltu**  47:19
it's I think, I think in your case it was so there's two issues here one, if an editor author's new IP, I believe it still requires one other approval, but I actually did approve it because I thought your training was fine. I had approved, mostly because I forgot that as an editor, if I approve your change 51 It will then get auto merged, I should have not approved it and just give them a thumbs up or something. I think it was really for that one that was my best. And this is again, ideally, if the book was written doing to do things the way we want, then I could have approved it and then it would have still sat and waited for Sam or like client or Alex to approve it. And then once we have for approvals, then it would merge. Or if it got three approvals and waited a month, and it would merge or if it got two approvals and waited three weeks or whatever the thresholds are, it would merge but that is yes, that shouldn't have merged. It was my fault because I hit the blue button there because I forgot. Okay, if you want that special.

48:17
Yeah, I think there was some other one. It there's some other one I think I approved and it just snapped right in. I'm going what?

**Micah Zoltu**  48:27
It's not desired, but it is the by the way that was programmed to do.

48:33
That's the problem with bots.

48:36
For living like instead of special casing ERP one should be special case like living EIPs in general, or

**Micah Zoltu**  48:45
I'm okay, it's either one since EMP one is the only living tip and the only living EPI is the IP one. So

48:54
the IP one should not change without actual discussion and consensus. I don't think anyway, it's special.

**Pooja Ranjan**  49:09
So if I can summarize here, it looks like this is a small bag on the bot side, maybe we have to update the bot for make it minimum of two approvals required to get it merged. Is that correct?

**Micah Zoltu**  49:24
So we have two options, one, just a minimum of two approvals required and that's kind of like the if we don't have time to write things well then that's, I feel like that's more acceptable than the current situation. And the other better option I opinion is to have a thresholding system so it depends on how long the the PRS open for and so if it was freshly opened the need for approvals if it's been open for less than a month, or sorry, it's been open for like two weeks and it drops down to maybe three approvals and if it's been open for a month then drops down to and if it's been open for two months drops down to one. And again, the purpose of That is just to avoid the situation where, you know, four of the editors have disappeared. And we're down to just one or two people, and we can still move forward. But I agree with what Greg said, like, if you want changes should get consensus, if possible. So I think in one of the issues that you linked, I actually describe this visually, you know, someone who wants to work on the box to go, one of those who solutions.

50:27
Yeah, I don't like some complicated system of thresholds and times, because then the bottle still just do things unexpectedly. Because who can remember thresholds and times? almost easier to tell, just tell the bot never do anything to EIP? One, it's

**Micah Zoltu**  50:48
yes, I would actually be okay with just as a the simplest solution, just update the bot to not touch the IP one. Or not actually, if you see that neither one. And that is by far the simplest thing requires zero programming, or very little programming. And maybe someone can just hack it out in an hour. I don't know.

**Pooja Ranjan**  51:11
Yeah, that's right. I think we have shared the issue here. That is issue number 53. That talks about the tear editors approval required for ambiguous prs? Yeah. I think the quickest fix is obviously to update the board for make it minimum of two. And then I'm assuming that Jose is already working on this particular issue. So if we can come up with the alternate solution that MITRE has proposed, that would be really good to have. Any final comments from anyone? Because I know we have left at five minutes. And I really quickly want to jump to Sam's part like he has to share anything on execution layer.

51:52
Oh, I don't really have anything new to share on it. I think there's the discussion thread that I've been keeping updated with the proposals. I think the only thing is, I might raise a few issues against the eip bot to add features. But that's it so far.

**Pooja Ranjan**  52:11
Yeah. On that, and I was wondering like, in the last meeting, we discussed about having alternate proposal for the updating of the process, the core EIP process? Did you get a chance to look into that? Or?

52:28
Yeah, it's a it's in the discretion of strength.

**Pooja Ranjan**  52:33
Okay, that sounds good. Right, just trying to look what all the last bit.

**Micah Zoltu**  52:48
Greg had some comments about the accidental spec. Yeah, please go ahead.

52:56
With for how fast is this moving? I don't want to write a long essay. I want to have a discussion. Because there's things I don't understand. But from what little I've heard, it's just a terrible idea. Is it I guess, Sam wasn't here, I've been trying to understand the CL specs. And they're pretty much impenetrable. I started with the beacon chain, I pretty much understand the beacon chain. And I'm just going along and like, this is just a heap of Python. I can write scripts in Python, I could get a book on Python and learn enough of it to read more. And even so I have to like reverse engineer the concepts from the Python code. And so anyone who's not a programmer, it has no hope of understanding this. And even a programmer is going, the best they could probably do is just do a port from Python to whatever language they're working in, rather than being able to understand the concepts and come up with an appropriate design in their own language, especially if they're working in a language which is much more declarative. Because pythons is a very procedural language. I've got E IPs that are basically almost completely declarative. And there's an example algorithm but you could throw the algorithm away, and the eip is complete. The wasum specification is a few 100 pages of declarative spec, and then an example algorithm at the end that specifically says this is just an example to show that you can validate these declarations in linear time. But the spec is all declarative. You can't write such a spec in Python. So I I just don't know what to do with that. Having having a having a client, which is executable, and is considered to be the reference client is certainly useful. But having having a heap of Python be the spec. It's less useful than the yellow paper, the yellow paper is really very simple mathematics is just not well written. So, but I don't know where the meetings are to push back on this, or if it's just going to happen. And we'll have an unreadable, unreadable specs.

**Micah Zoltu**  55:37
Think this, this meeting is currently the best one to discuss. I'll hand over sound, but I believe the suitable specs will have a human readable portion to them. And I think, Sam, you have some ideas on how that will integrate.

**Pooja Ranjan**  55:55
So I just see a message from him, it says that he will write back got a phone call, maybe I can do one thing, like we can bring it back in the next meeting, if that's okay, if it's not back in a minute or two.

**Micah Zoltu**  56:13
So I will try to stand in for my Sam head on. So my understanding of the plants LexisNexis, the actual spec will be like you said it will be referenced client, and there will be a requirements to update it. So when you're writing a change to do it, and so in your in your example, you know, you're right, you had a little reference implementation of your thing at the end. And so that would kind of translate over to the the piece that you would add to the reference. Or you work with someone who is you know, I thought he's more of a Python to to handle the heart. But if I understand correctly, the executable spec will also contain, you know, some files. And again, I leave to Sam, if you ever returns to good, thank God trying to speak for you and failing miserably. Greg was basically what can you explain what your thoughts are on how, where the real human readable natural language portion of your piece goes in the actual spec?

57:22
Sure. So there's, there's two parts of human readable text that's going to end up in the spec, there's going to be like the annotations on the spec itself. And those will be stored as Doc strings in the Python code. And that is going to look a lot like the annotated h2 spec. But I don't think that's what you're talking about. I think you're talking about like, the motivation and rationale sections.

57:46
Go on. I'm sorry. No, no, go ahead. Just go on.

57:52
Yeah, so the those are, I would like to store as markdown files in the execution specs repository, that way there alongside the code change that they represent. And yeah, I think that's probably how I like to structure it. But I'm open to other ideas as well.

58:10
My concern is specifications that need to be or best written, or the author prefers to write declaratively. Not here's an algorithm you can run. But here are a set of constraints that these op codes need to make. And you can validate the constraints. Or you can implement it the algorithm any way you like, it just needs to meet these constraints. And that isn't just annotation or commentary. That's the spec.

58:50
Yeah, I think that makes sense. Like I think, like prime example of this would be like if in the spec, we use a dictionary to represent state. Right? And that is absolutely not how any client would implement it. So you're asking about that go on. I'm sorry. Oh, yeah. And you're asking how how do you say like what state is without specifically choosing an algorithm that implements it? Except for more generally, obviously. Well, I mean,

59:27
it's 615. I, I tried to keep very close to yellow paper terminology. Yellow papers never been expressed in Python. It just in general, I don't want people to have to learn enough Python to read and write the specification. Python doesn't even have a formal spec, a Python specification is is is pretty much locked into a current version of Python. On. But to actually know the semantics of the current version of Python, you have to read it source code. It's there's no, there's no formal specification for Python. We're just we're building on sand.

1:00:18
I think that's a really valid point. And, yeah, I think it's a difficulty. Like, we don't have a formal. If we don't build on a formal base, our specification isn't, you know, formal. And that's concerning. But I think, you know, the primary use case for the yellow paper and the specs is not for anything horrible, but for client developers to implement their clients. And I think Python provides a firm enough base. To do that, even though it isn't, you know, solid, concrete or bedrock.

1:01:01
It's, you mentioned the dictionary, for instance, it's very hard in a reference implementation to separate the the essence of the specification to the accidents of the programming language it's written in. So you go through and there's a dictionary, and it's like, does it need to be a dictionary? Oh, well, what are they actually doing with the dictionary? Oh, these are the actual parts of the dictionary they need. That's it? What data structure in my language? Should I use? Or should I design to do this best? Oh, this algorithm has been expressed recursively in my language, if I try and do it, recursively I'll blow stack way too soon. Okay, what's, what's the actual concepts here? So I can do it in an iterative way or so I can do it with continuations. You know, the yellow papers on an algorithm. It's, it's a description of a world state, and a set of state transitions. And different languages have different ways to represent state and transitions. And it's it's just much easier to ask somebody to say, go learn this little bit of very standard mathematics topples. Very simple, very simple logic. The math is so easy. And in the yellow paper, it's just, you know,

**Micah Zoltu**  1:02:42
I would argue that given the target demographic for the, like client dubs as a target demographic, I think, learning Python, I suspect for the vast majority of them is going to be easier than learning mathematical notation. Just because they're starting from a base of they're all software engineers, like everybody who was going to be looking at these and implementing these is software engineers, they probably know one or more languages, at least one of those languages is almost certainly going to be a Python, like language, like Python, Go rust, see, like that are called that that class of languages. Like, nobody's going to be, oh, I only know Escale. I've never touched anything else. I think just given the demographically, like, maybe if you starting from zero, maybe the mathematical notation is easier, though I even questioned that. But I can appreciate the argument there. But starting from a groundwork of coordinates, I suspect Python is much closer than math, which is why I also suspect why many people complain about the old paper because it's written in math language, and not in the programming language, anybody knows.

1:03:54
So I kind of want to take what you said, Greg, and split it into two parts. The first being that choices that are decisions that are made because of the language of the spec, are going to end up leaking into downstream clients. And, you know, I think that's a legitimate concern. Like, for example, like if we choose, like, a particular algorithm to implement, let's say, state, again, using that example, then, you know, that algorithm might end up in clients, even though it's a horribly inefficient algorithm. And that's 100% of problem. I don't know how to deal with it. I'm just going to say that right away, like I think the pure note like notation that the yellow paper uses is 100%. better in that regard. But to tie that, to what Mike just said, I think the readability improvements and like the starting from a share base among software engineers, is kind of the benefit that I'm weighing against that. And the second thing I wanted to say is, I think regardless of whether we use Python or for math notation. There's this step of translating the written document into a mental model of how that like what the spec is describing, right. So in in the yellow paper, you have to translate the mathematical notation, which is algorithm agnostic into, like what the spec is saying to do, and then translate that

1:05:25
down with the spec. Your back. Okay. Oh, I'm

1:05:29
sorry. I didn't realize I cut out there. So yeah, basically, I'm just saying that there's

1:05:33
Sam has gone for me.

**Micah Zoltu**  1:05:36
I think Greg is disconnected. Can you hear me, Greg?

1:05:42
I don't hear Sam at all. I don't know if anyone hears me. I can hear everyone.

**Micah Zoltu**  1:05:58
think Greg connection. You mentioned earlier, he was having connectivity problems. This is really good. All right.

**Pooja Ranjan**  1:06:09
I don't know if you want to have a solution for this particular thing today. I'm not. I know we had a lot in the agenda prior to this discussion points. So maybe we were running short on time for this. I'm happy to bring it back on the agenda next meeting. And that will be like in the first or second number so we can discuss it properly. Because this is a very this is of high importance right now. It's going to be changing. I'm assuming that.

1:06:42
My sorry, my connection dropped. And I heard almost nothing that Sam said.

**Micah Zoltu**  1:06:50
At what point did you lose them?

1:06:53
But don't start again? Probably. Sam,

**Pooja Ranjan**  1:06:57
would you have the recording? Yeah, we will have the recording, Greg, maybe whatever you miss will be able to catch it up over there.

1:07:04
Yeah, Sam, would you have a little time after the meeting for us to actually just discuss this?

1:07:12
Yeah, I mean, sure.

1:07:14
We got more than 10 minutes worth to get through. It's actually difficult for me to type right now.

**Pooja Ranjan**  1:07:22
And I? Yeah, I'm fine recording. It was just that I don't I don't know if we would want to keep this discussion be a part of meeting notes. So

1:07:31
it's, I'm asking Sam, if the two of us can just take some time. Oh, that sounds good.

**Pooja Ranjan**  1:07:43
Well, any final closing for this particular topic from Sam, Greg on Mica.

1:07:49
I'm good for now.

**Micah Zoltu**  1:07:51
Which probably, if we're gonna put it on the agenda for next week, which I do think it's a good idea. We put it earlier on the agenda. So we make sure we have time

**Pooja Ranjan**  1:07:58
for startups. Definitely, I will try to make it the number one item. So we will discuss this because there seems to be a higher priority. With things changing moving faster, we will definitely discuss that. All right, I know we are 12 minutes past that time, we had a couple of more agenda items to discuss, I'm not going to go through all of them just trying to share the information here for EIP is on site, the link is added to the agenda. So anyone wants to follow the latest update, it is available over there. And for EIP editors apprenticeship meeting, the meeting was organized yesterday, the summary and the recording is added to the agenda, the link is added there, you may be able to follow that. And for review action items. Maybe we can look into the items quickly if there is anything. Okay. I think all the items have been already taken care of. But if if people come up with something new, we can bring it back in the next meeting, hopefully. Well, thank you so much, everyone for joining us and staying a bit longer. I know that you joined the meeting, but we did not get a chance to discuss your proposal. If if you want to discuss it with the eip editors. Maybe we can add it to the next meeting agenda or there is another meeting called EAP editors internship meeting. That happens on Tuesday at 1500 UTC, you're more than welcome to join that and share it with people. So if you need any kind of review or comments, you can do that.

1:09:33
Sounds good. Thank you. I will look at the context.

**Pooja Ranjan**  1:09:38
All right. Any final thing from anyone? Well, thank you again. And thank you again, everyone for staying a bit longer on this. See you all around in the disk and yeah, see you in two weeks. Have a good one everyone. Thanks, everyone. Bye bye.

# Attendees

* Pooja Ranjan (Host)
* Micah Zoltu
* Sam Wilson
* Greg Colvin
* Zainan Victor Zhou
* Jose
* Brent Allsop
* Jim Bennett



# Date for Next Meeting: April 20 at 1400 UTC
