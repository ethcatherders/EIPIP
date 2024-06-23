# EIPIP Meeting #97

### Meeting Date/Time: January 3, 2023 at 16:00 UTC
### Meeting Duration: 21:36
### [GitHub Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/302) 
### [Audio/Video of the meeting]( https://www.youtube.com/watch?v=eO6tqGEJsH8) 
### Moderator: Pooja Ranjan 
### Notes: Metago
### Next Meeting Date/Time: January 17, 2023 at 15:00 UTC

## Agenda

### EIP Process Standardisation

**Pooja**
Welcome to EIPIP Meeting 97. This is issue number 302 on Ethereum cat herders. So first there is this announcement that the Ethereum Cat Herders GitHub repository address has been changed, so please make sure to reach out to Ethereum Cat Herders GitHub repository at github.com/ethcatherders.

On agenda we have a first item called EIP process standardization, then there is a list of open PRs There are certain PRs with respect to proposals which went into final but there is a request of making small edits, mostly with respect to typo. We'll go over call for input and then we have some discussion continued from the past meetings. We have added EIP’s Insight for the entire year, and yeah, that would be all for overall discussion today.

#### Webpage Rendering

So let's begin with the first item on the agenda, which is EIP process standardization and the first item listed here is web page rendering. So we have been approached by a few groups to understand what are we thinking of a rendering RIP related proposal but since the repo split of EIP ERC, we are also discussing the rendering of EIP ERC on a certain web page. So I would let Sam explain. I know he has been working on a rendering part. 

So Sam if you would like to maybe let us know where we are on that.

**Sam**
Sure. I haven't really done anything over the holidays. You can still see where we're at, at github.com/ethwg, so eventually I'd like to add support for RIPs if they want to become a working group and yeah as long as they follow a general EIP structure of a repository, the scripts can import them. So yeah it shouldn't be too much work. 

**Pooja**
So there was this important point, if they would follow the general process or the GitHub repository structure, because we know that most of the pages are with the GitHub repositories that we have. 

#### RIP Process Documentation [2:39]( https://youtu.be/eO6tqGEJsH8?si=IPn3qF8hIBUgCxvA&t=159) 
#### Type and Category for Rollup Proposals
#### Need for update definition of Standard Track - Core in EIP-1?

I wonder if we can perhaps discuss the RIP process documentation. We may use some of the clarity on that part, for example what could be the type and category for rollup proposals and how should we move it forward. We don't have much documentation around that. 

**Sam**
Yeah I'm not really sure how we want to approach it. I've kind of been just working on the working group stuff and was going to work on that after, but you know I'm not the only editor so.

**Pooja**
I wonder if anyone else has any thought on this?

The one concern that I specifically want it to be addressed is the type and category thing. For example, currently there is only one RIP in the RIPs GitHub repository and that is standard track core. As we know standard track core are mostly EIPs which are for the Ethereum mainnet and most of them when get deployed are marked as final.

Now the special case would be when this RIP gets to final and if it retains the category as core, that would be a core which is not deployed on Ethereum mainnet, would be marked as final, and if we want to keep it as is, do we want to update the definition of a standard track code in EIP 1?  

**Sam**
So I guess my opinion is until we have a unified process I think they can do whatever they want. 

**Pooja**
This is interesting. I think they have actually proposed their first proposal here on the EIPs GitHub repository to create room for, especially for RIPs. I guess I'm trying to find out the link here so I can share what would be the right approach. I wonder because the RIP meeting that happens, they clearly say that it is not governance related meeting, and we only have editors meeting as EIPIP meeting.

So this is a PR where an informational level proposal is added to reserve pre-compiled address range for RIPs, so they are definitely trying to align with the EIP process but community can use some clarity. I don't see Matt on the call. I wonder Gajendra Singh, if you have any thoughts or any suggestion how we can move forward with these proposals to be maybe included in the EIP process in long term.

**Gajinder** I don't really have any opinion regarding this work here. Maybe we can check on the call here.

**Pooja**
Or dev core what people think and how we should align if we do not have enough editors here to provide feedback or thoughts.

## Open Issues
### [Update EIP-684: Fix typo ethereum/EIPs#8061]( https://github.com/ethereum/EIPs/pull/8061) 
### [Update EIP-225: Update eip-225.md to fix typo "singer" ethereum/EIPs#8038]( https://github.com/ethereum/EIPs/pull/8038) 
### [Update EIP-145: fix typo ethereum/EIPs#7958]( https://github.com/ethereum/EIPs/pull/7958) 

[6:28]( https://youtu.be/eO6tqGEJsH8?si=9ZksFWuMX0kohxdJ&t=388) 

Yeah okay, let's move on to the next one. We'll try to get it included in the next agenda item in for meeting. Moving forward, we have a few open PR with respect to final proposals and those are fixed typos. The first one here is a PR number 8061 to fix 684 and I have added two more. How do we want to go about it? Can someone maybe take a look? 

**Sam**
Yeah they're all merged. 

**Pooja**
Okay perfect, thank you.I wonder if my GitHub is not updating it but that's good. Very well the next item here is call for input. So we have two call for inputs added here, 291 and 293. The deadline for both call for inputs are completed. Sam, if you would like to maybe provide a brief summary and help us with the result and if we want to close these call for inputs…

**Sam**
Sure, so the first one here is Add security consideration to ERC 1271, there's a security vulnerability or flaw or missing piece of information in 1271 but 1271 is final so if you don't object Gajinder, I'm going to not change 1271, because I think I'm the only editor who's commented on this so far, so are you okay with rejecting a change to 1271 or…

**Gajinder**
Yeah I'm fine I'm in all right perfect 

**Sam**
Sorry I didn't mean to cut you off there. 

**Gajinder**
Yeah no I said just I'm good with what you have decided to reject the change.

**Sam**
Okay yeah and I think the other one is similar. This is adding a new informational EIP describing flaws and erc20. Yeah I'll close both of these later if you have any comments just leave them on the those PRs or issues and I think that's it for calls for input. 

### Other discussions continued or updates from past meetings [9:10]( https://youtu.be/eO6tqGEJsH8?si=9ZksFWuMX0kohxdJ&t=550) 

#### Changes to Final EIPs
##### [Update to ERC-1363[(https://github.com/ethcatherders/EIPIP/issues/302#issuecomment-1872058595) 

**Pooja**
Perfect, thank you Sam. And with that we can move on to the next item which is the discussion continued or updates from the past meeting. So there were a handful of proposals to update ERC 1363 which unfortunately we could not address in the past meetings. They have been listed by a user in the comment, so I wonder what editors think about it. There are three updates adjusted for 1363. 

**Sam**
These are pretty substantial updates, so I'm inclined to say no, yeah that's kind of my opinion on these.

**Gajinder**
Okay if we don't need to do them I think we should just leave the EIPs like that. We don't unless the updates are really required. 

**Sam**
Yeah even then I think we can just tell the author to make a new EIP.

**Gajinder**
 Yeah. Correct that is the right way to do it that the new EIP override is the previous one and we sort of in the UI UX experience, we can basically tell the user to go to the latest one. 

**Sam**
Yeah perfect. I'll take care of commenting and closing these.

**Pooja**
Thank you so much. 

####  Why Final EIPs are "Immutable"? [11:00]( https://youtu.be/eO6tqGEJsH8?si=9ZksFWuMX0kohxdJ&t=660) 

Moving on, there were few questions those were like a raised earlier maybe to get some clarity and if possible we can perhaps document even if it is not officially document somewhere in notes or summary, why final EIPs are immutable, specify conditions under which final EIPs can be updated.

I think this would be useful for accepting pull request for final EIPs if we can create this as a guideline for user, then in that case they may perhaps understand when to create a new proposal altogether or when they can perhaps send PR to make changes. 

**Sam**
So just like a little document that's like, here are some non-binding rules on what we are allowed to change, what are, we not allowed to change.

**Pooja**
Yeah I think that would be helpful if we can document anywhere that would be nice.

**Sam**
Yeah exactly yeah guidelines yeah cuz like things like formatting changes, as long as they're minor and don't change anything substantial, are fine, spelling mistakes are fine, but you know anything like you know adding text or changing the meaning of things, it's probably not fine. Yeah.

**Pooja**
So EIP 1 is considered to be purpose and guideline document. Do we think that we can perhaps make use of updating it I'm sorry if I over spoke somebody please go ahead.

**Gajinder**
Yeah I was saying yeah because if the text is changed, somebody competent actually needs to check whether the semantics of the EIP have changed or not. I mean we can sort of figure out few of the things but there are some technicalities where you know expert opinion / the EIP author's opinion is needed and yeah that's why we should basically try not to have too many text changes and the language changes in the EIP.

**Sam**
Yeah exactly. 

**Pooja**
I am not sure maybe an EIP template would be right place or maybe EIP 1 would be right place to document these changes not changes, actually guidelines I meant.

**Sam**
So you you like one of us sorry 

**Gajinder**
Wherever our chapter lives I think that is the fine place I mean we can have a short paragraph over there. 

**Sam**
Yeah sure I think that's a good idea.

**Pooja**
Okay yeah that sounds good. Okay in that case then we will get the link and we will start sharing that link with people so they understand. 

#### [Update on Versioning Scheme for EIPs](https://ethereum-magicians.org/t/add-eip-versioning-scheme-for-eips/17295) [14:07]( https://youtu.be/eO6tqGEJsH8?si=9ZksFWuMX0kohxdJ&t=847) 

Very well the next item here is another proposal that was discussed in the past meeting which was versioning scheme for EIPs. I don't think this proposal has been merged yet in the draft. I can see this is still open and I also shared a little bit change to the proposal to have versioning but this versioning will help us understand the status specs patch. I was hoping that if we go by this this might help bot a bit more to work accordingly.

We can use the values there with status and everything else. I would love to get any feedback if people have here or maybe add later on, so I just have added the link to Ethereum magician. And I'm aware that there was some discussion going on in on Discord Channel, I wonder if there is any update on moving ahead with this or yeah if people have anything to share here?

**Sam**
No updates on the versioning yet. At least for me.

**Gajinder**
Yeah same here no opinions yet.

**Pooja**
Okay, very well. I find this proposal quite interesting and I'm looking forward to get this merged and draft and yeah I have shared the link here in the agenda for people to add thoughts on Fellowship of Ethereum magician with respect to this proposal. 

### EIPs Insight - Monthly EIPs status reporting [15:49]( https://youtu.be/eO6tqGEJsH8?si=9ZksFWuMX0kohxdJ&t=949) 

Moving ahead on EIPs Insight, so I have added summary for past three years here, like I was just trying to collect data with respect to how we are doing, in terms of proposals that are being received and how many proposals are being moved to final status.

I'm very happy to share that this year 2023 we have in the past three years we have increased the number of proposal that reached to final status and as for December we received three proposals in final.

All three belong to the ERC category. For last call we received five two EIPs, two ERC and one RIP. So here is the thing like this RIP proposal that was added as core proposal and there is no history of the proposal getting into draft or review it just went to the last call so that's something that we would like to breach at some point of time and yeah the proposals going into stagnant has also decreased significantly.

Last month only four proposals moved to stagnant status so this is a good news and thanks to all editors contributing to help move these proposals forward. We are in a very good state where we have increased numbers of proposal move to final. Thank you all.

**Sam**
And thank you for keeping us organized.

**Pooja**
Yeah no I'm really happy we have been trying and this is like third year and the result is definitely better here. All right, people can check out the hackmd or eips.insight.com for a different charts and details.

###  [EIP Editing Office Hour](https://hackmd.io/@poojaranjan/EIPEditingOfficeHour)  [17:50](https://youtu.be/eO6tqGEJsH8?si=Zwb1z3O3cNhA0xLx&t=1070) 

The next one is EIP editing office hour so this meeting is organized to support new and existing EIP authors. If they have any pull request that they would like to discuss with editor, they have any question, they can reach out to EIP editor, and the meeting is planned for January 9th at 1500 UTC.

This is issue Number 301 at ethcatherders at GitHub.com. We are hoping to support new authors to document their proposal in in a well way and we organize this meeting every 2 weeks to answer any question so people if you have question or if you know someone who may be in need of some kind of support with respect to documenting an Ethereum standard, irrespective of type and category, core / ERC / RIP, please feel free to share about this meeting we would be happy to extend support and I think that's pretty much it.

I'm quickly taking a look at the summary section from the last meeting. I think we have covered all the open items from here. So this quite short but I look forward to have more discussion on governance and streamlining the EIP process. 

Anyone has any thoughts final comment they would like to share? 

**Sam**
I think we good thanks so much Pooja.

**Pooja**
All right um Before I Let You Go just one final question. I missed on this part. What about the meeting time it was mentioned by one of the EIP editor that 1500 UTC may not be working. We moved here because there was no protocol meeting there at this time, do we want to keep it or is it okay to move it by an hour? 

**Gajinder**
An hour is going to affect my etherum just update meetings we can move early or we can move a little bit more later. I mean I suggested a time we can move early as well I mean that is also fine.

**Pooja**
Okay Sam what is your preference is that okay to move it to 1400 UTC?

**Sam**
So 1 hour earlier? Yeah I can probably do that, it's a little a little early for me but it's okay.

**Pooja**
All right.

**Gajinder**
As of now after the proposed timings as well I mean we can move later as well.

**Pooja**
17:30?

**Gajinder**
Yeah because I will anyway be completing my ethereum Js update meetings and post that I can join this.

**Pooja**
Okay, would that work for you Sam 17:30?

**Sam**
Yeah yeah I think so Thursdays are pretty open or whatever day this is Wednesdays are pretty open for me yeah. okay um but I I don't think we should decide anything until like more than two of us say something cuz yeah.

**Pooja**
Yeah no I wanted to just collect your feedback thoughts here so we can propose alternate timing in the discord channel to maybe get some consensus there.

**Sam**
**Pooja**
Perfect all right so let me propose 1400 and 1730 and whatever votes like maximum votes we will collect we'll try to keep it that one for the next meeting planned on January 17th.

**Sam**
Sounds good talk to you then.

**Pooja**
Thank you thank you everyone for joining us here bye take care bye-bye

## Attendees
* Pooja Ranjan
* Gajinder
* Sam Wilson
* ZKSAFE – George
* lightclient
* Daniel from zksafe
