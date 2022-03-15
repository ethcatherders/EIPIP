# EIPIP Meeting 51 Notes
## Meeting Date/Time: Wednesday, Mar 09, 2022, at 15:00 UTC
### Meeting Duration: 1/2 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/112)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=GkL99zdY2_8&t=116s)
### Moderator: ****Pooja Ranjan****
### Notes: Metago

----
## ACTION ITEMS

**ACTION 51.1**: EIP editors will complete survey to finalize time and date of future meetings. 

**ACTION 51.2**: Discuss potential alternate names for future EIPIP meetings

**ACTION 51.3**: Pooja will add a list of exceptional cases that may allow editors' non normative changes to final EIP, to a hackmd file, as a reference for EIP editors.

**ACTION 51.4**: Pooja will contact fem re ability to edit posts. 

## COMMUNITY PARTICIPATION
** 51.1**: Please reach out on ECH discord if you have experience in Ruby on Rails
** 51.2**: Please reach out on ECH Discord / ECH Github if interested in open issues related to [EIP](https://github.com/ethereum/EIP-Bot/issues) and [EIPV bots](https://github.com/ethereum/eipv/issues). 

## LINKS SHARED IN THE CHAT

**Pooja Ranjan** [Pull Request no.4762](https://github.com/ethereum/EIPs/pull/4762) 

**Pooja Ranjan** [EIP 3326](https://github.com/ethereum/EIPs/blob/master/EIPS/eip-3326.md)

----

## AGENDA ##
## 1. Discuss policies to merge Pull Request to update an EIP in absence of author's approval. [Ref](https://discord.com/channels/595666850260713488/746566142700814426/950500546815598622)

Pooja Ranjan starts meeting and shares agenda in the chat. 

**Pooja** 
I have added the link from the ETH R&D discord from Sam Wilson's conversation. Actually I was also thinking about it a few days ago, while working on EIP Insight. I came across some old pull request, the number is 4766. What I found is that the general recommendation is that the interested parties should fork and create a new proposal and submit the pull request. Pooja asks whether in exceptional cases, people think that the editor should be permitted to merge the pull request with minimal or very trivial edits request. 
So what Is the general thought here? 

**Micah**
In the past, I have, if it's like just a typo or something, like someone just fixing a typo or they're just like, maybe it's a very non-contentious like word change, like a grammar fix and whatnot, pretty much anything that is definitely…so nothing normative can happen to a final EIP at all. That's just…straight up can't do it. If the change is substantial in any way, I can strawman why someone would disagree with it, then I usually wait for the author, so this includes like who it was wanted to go through and change the usage, change a bunch of word choices throughout all the EIPs, like i forget what it was, think blacklist…they wanted to change to something else, like block lists. I think that is something that I’m unwilling as an editor to override. So again because it’s a very political thing it's not just a grammar fix like the EIP isn't incorrect it's not invalid grammar it's not like a spelling error like this new person is coming in and saying I think this should be worded differently because I have a different worldview or belief system or whatever for those ones I am very much against editors overriding the author even though they are technically allowed changes like that are non-normative and therefore they're allowed for final EIPs. What was the number for the one that you were referring to, Pooja? What was the EIP number?  

**Pooja**
The number is 4766 so the only change here is a removal of a semicolon which is which looks like an additional is not needed there.

**Micah**
Sorry, this is not an EIP 4766 is it a pull request 4766?

**Pooja**
That's correct.

**Micah**
Yeah. Oh, I see. The code is wrong and does not currently execute. Yeah, I’m fine with merging this one. It’s just a non-normative correction that fixes the bug in the example code. Normally I so for the first situation like this usually what I’ll do is I’ll wait a little bit to see if we can get a hold of one of the authors to get them to approve it, just because I prefer to not override the process if it can be avoided, but for something like this…it's been a month. I’m okay with merging it without the authors..

**Pooja**
So I was hoping, if we can come to some suggestion or guideline for this for future EIP editors to be referring to, just like we have a policy for EIP 1, like it is open for two weeks and it is approved by a couple of editors, it can be merged after two weeks even if we do not get all EIP editors approval by that time. So for these kind of small changes which are considerably no brainer, I mean, like I know EIP editors are educated enough to identify if it can be or not and it is approved by them, then probably after a month or maybe two weeks’ time it can be merged, so just wanted to have some decision on that side. 

**Micah**
Yeah, like I said, the main thing that I care about is making it very clear that this would be for grammar and spelling and incredibly trivial changes only. Any changes that someone might find contentious for any reason, I think we should avoid doing so. As long as the wording kind of makes that clear, I’m okay with it.

**Pooja**
Absolutely. I’m also referring to one more pull request, and its number is 4513. It looks like this is also a small change in fixing a typo for a function name. And that also seems to be, like you know… been done in a while but still hanging out there. 

**Micah**
So if an editor wants to go through and actually review this, I am okay with it, but, like from that line alone, I can't assert that that is not a normative change. Like someone would need to actually, like read the EIP and make sure that that this is in fact a correct change to make things better and not something that makes it incorrect. This gets into the problem of…we don't have enough editors to go through and review everything. Which is why we lean on authors to verify stuff like this.

**Pooja**
All right. I think I got your point here. I was also looking into one more pull request. It's 4417. I'm sorry. I kind of collected all these numbers which I thought that might need some attention here. So about 4417. It looks like it was approved by one of the editors but we haven't received any response from the author and the change seems to be like smaller one and obviously this is like a longer duration. So is it fine, like proposals like this should be merged…

**Micah**
Some of it, like just removing the white space from the end of lines like that part I’m fine with. I’m guessing they fixed the table rendering for one of these. Yeah, again this one's this one's kind of bordering on the..this is starting to get to be a fairly large change and as an editor I don't particularly want to read through it at all and determine whether it's valid or not and it's great if we have authors that can take care of that instead. Also none of this is…so like the white space changes for example are not necessary. They don't actually change the rendering at all. I’m fine with them but it feels very opinionated and I’m generally apprehensive of making opinionated changes to other people's EIPs. Yeah, I think for this one personally I would rather get author approval but also it's an ERC so I wouldn't be the one to handle it anyway. So we can leave it up to Sam, and Light, and Alex and Greg

**Pooja**
All right. I think I have also added in the later agenda. I think its point no. 2 also that if we can in some way automate these things and send reminders, I will bring it back when we get into item number 2. But for item number 1, I think it is okay to have like grammar or spelling or like trivial changes, small trivial changes can be merged after one month of period, and once it is approved by some of the EIP editors. Does that sound reasonable, like I will obviously I’ll try to reword it better and then make the suggestion added

**Micah**
Yeah, I would say if it's been sitting for a month and it is a trivial grammar or spelling change or typo or just like very very minor bug like missing semicolon, or extra extraneous semicolon some code and it's been sitting for months, then yes I’m fine with it. That seems reasonable to me. So any at that point any of the editors can override and maybe one day we have a bot that helps with this, but i don't know… overwrite I think works.

**Pooja**
All right.  Sam Wilson, do you have any thought on that? I mean this is from the discussion that you initiated on Eth R&D (discord).

**Sam**
I mean I’m kind of in the complete opposite direction as Micah. I mean, I think we should probably like have a formal process for taking over EIPs, and for like assigning new owners, and all of that stuff, and I, but I’m new right, like I don't really have, I haven't, you know, battle tested my opinions yet, so we'll see how this goes for a while and see what happens.

**Pooja**
Yeah, I think one thing that we discussed probably before you joined the call, this is like for exceptional cases especially for the edits related to final EIPs, because I don't think it makes sense that we go ahead and create another EIP fork, and create another pull request for same EIP, which is already in final, making small changes, right? 

**Sam**
Well yeah for editorial changes that I think that's the term that greg used for them, I think, yeah, it makes sense to let editors merge.

**Pooja**
All right, and does it need to be updated somewhere on EIP1? I, on my end maintain a hackmd file where I try to add these exceptional cases for reference of new EIP editors, like people who are from the apprenticeship program, but do we think that it needs to be updated somewhere on EIP 1 as well?

**Micah**
EIP 1 currently says final of this EIP represents the final standard a final EIP exists in a state of finality and should only be updated to correct errata and non-normative clarifications. I think that's all the text we have on it in EIP 1 and I’m fine with that as it is personally.

**Pooja**
All right, then probably I will add it into the hack md file so people and exceptional cases may be able to refer to that. Thank you. I think we have kind of a recommendation ready to be added, moving on to the item number 2, unless anyone has anything else to add on, item 1, which I believe…

**Micah**
did we want to have the longer discussion Sam just brought up?

**Pooja**
I’m open to it, like the process change, for the entire process change for EIP editors overriding.

**Micah**
Are you interested in pitching your thing Sam?

**Sam**
I have another call in 10 minutes so I probably wouldn't be able to participate very much in the discussion.

## 9. EIPIP meeting time and name [survey](https://docs.google.com/forms/d/e/1FAIpQLSchmERP_dueiskdi-SlJCa57s7p7Ku5u_wTOJtlqTefpENglg/viewform)

**Pooja**
Okay, in that case, Sam, I would like to straightway come to item number 9, which is about a survey for having a new time. I would like to see more EIP editors joining this call, but looks like the time is not working the best for everyone, so I have created a small survey. It has only three questions. One is what would be the best time for you. There are a few options. You can select from that or maybe you can suggest something that works best for you, and if in future, we would like to rename this meeting…the current name is EIPIP, and there are a few suggestions. If we would like to rename or just go with that, I would highly appreciate taking out time, and responding to that survey, and based on information collected from all EIP editors, maybe we will propose new time for the meeting.

## 2. Discuss the possibility of
bots replacing the PR description with a standardized template. Ref [Discussion](https://discord.com/channels/595666850260713488/746566142700814426/950490767850348585)
bot sending reminder to author for action required
bot sending reminder to editors for action required

**Pooja**
All right moving on to item number 2. Number 2 is discuss the possibility of bot replacing the pr description with the standardized template. I think this is also suggested by Sam Wilson.

**Sam**
Yep. Yeah just a lot of authors seem to, or a lot of people making pull requests, I should say, don't replace the the text of the pr with anything useful. They just keep the template there, so you know, I think, some things that I’d like to see is, like a link to the rendered EIP, maybe a description of the change, a little bit, just like, it just, to make it a little bit easier but it's really a low priority thing.

**Micah**
Are you suggesting we have like a bot that handles this, or would this be something that we'd request of users?

**Sam**
It would be done by the bot. So it would just take whatever text the author leaves there, puts it in a specific section, and then adds a header to the comment.

**Micah**
Oh yeah, I’d be totally fine with that if we have a bot for that.

**Pooja**
So I am assuming that this would not be EIPV but it would be the general EIP bot that we have right? An enhancement for that?

**Micah**
Yes.

**Pooja**
We'll create an issue for this and see if someone can work on this particular item. Just for bots enhancement, I have added few more items here one is like what sending reminders to author for action required and what sending reminders for editors for action required. So I have few pull requests here, for example pr 4762, it seems like it has been open for authors response for very long time. What do people think about having a bot sending reminder after three months because after six months we just make the proposal stagnant and it would be nice to have sending a reminder before that and similar thing for the EIP authors. I have seen that, for example pull request number 3975 has a response from the author and it appears to me like now editors have to take action on that but I’m not sure if that is slipped because we have like over 50 pull requests open.

**Micah**
Can you provide a link to that?

**Pooja**
of course i can do that, sharing here in the chat. So, the request here was to make some changes and to move it to final. I'm concerned about this particular EIP because this would be required for the merge EIP because in that I think 3675 this proposal is mentioned and we generally recommend that if a proposal is getting into final status, we make sure that all the proposals which are like required should be in the final status and I’m not sure why this is being blocked for so long if it is just waiting for editor's response so maybe we can send a reminder using bot.

**Micah**
So for this one in particular, I am unwilling to approve it, so we're waiting to see if we can get two other editors that disagree with me to approve it and currently Matt has approved, so we're waiting for someone else to say yes. I’d like this to go through and to prove that EIP editing is not actually a dictatorship. My reason is, I don't think this should be an EIP at all, like I think this should live somewhere else, and not be in the EIP repository. It's essentially fiber correctly, it's consensus spec-ish thing and it's lived in the, it's got put in the EIP repository because, as Danny mentioned in discord today, it's dumping ground for homeless standards and specifications and I'm very much not a fan of the EIP repo being the dumping ground for homeless standards and specifications, but if two other editors are up for it, feel free to override me.

**Sam**
Is there a precedent for something like this being merged?

**Pooja**
Actually, this is an informational category. Sorry.

**Micah**
Yeah so there have been precedence for overriding Micah. Yes, like there have been EIPs I’ve refused to merge because I disagree with their presence at all, and yet other editors agreed that they should go in and so it has that aspect, has essence, historically, we also have stored lots of stuff in the EIPs repo that is not an Ethereum technical standard or at least a core layer technical standard. This one's not even a standard or specification, which is also why I don't like it. It's just kind of like a description and I really feel like this should be a blog post or a docs documentation site or a readme or something like that somewhere else, not an EIP, because there's no standard, no specification here. It's just like, hey, this is a description kind of ish thing of, I want to say it's a proof of stake like it's a vague high level it's not, it's not sufficiently specific either like it just kind of glosses over some very important parts of how a proof state works and it has you know a thousand external links to a bunch of other different documents so it's not self-contained like this, has everything that I hate about going in when one EIP is like one EIP that kind of encompasses all the things that I think should not be in an EIP um so I have…that is why I’m blocking it. But again, that doesn't mean that all the editors agree and matt has already expressed that he thinks it's fine as an EIP and so he's just waiting for one other person, because he feels that if an editor is saying no and another saying yes then we should have a tiebreaker basically, and I tend to agree with them and in the inverse situation I do the same thing. So if you're up for it, Sam, feel free to take a look at it and be there.

**Sam**
I’m way too new for this, I’m not getting involved in a controversial EIP.

**Micah**
Also, unfortunately we have you, Greg, and Alex, and we need one of you to get involved in the controversial EIP and it's been five months and neither Greg nor Alex have gotten involved so thats why it's kind of sitting here in this really uncomfortable neutral middle ground state because we don't have enough editors to act, actually block it and say no this will never go in. We don't have enough editors to actually approve it, so it just sits here in pr, waiting. Yeah.

**Sam**
Yeah, so it it's now going against EIP 1, so we can definitely delay it for a lot longer.

**Pooja**
So actually I think a little different here, I mean I may have a little different opinion because this particular proposal is an informational category that can be allowed because informational proposal by definition is not a mandate that people need to follow. It's just a piece of information around the protocol development, which this proposal is actually trying to provide here, in terms of like what was planned with the beacon chain and like how people want to continue working on the beacon chain and some of these inspiration has been implemented in the proposal 3675 I believe, and at least the terms are being referred to, so I think because this comes into an informational category, if editors find it okay to be allowed to be merged as a pull request, this would be one of the best informational categories proposal because we are really scarce on information around the protocol changes in this particular category, especially.

**Micah**
Yeah, so if you agree the informational category is a reasonable category to have, then this EIP does fit that. I've been trying to get the informational category removed from the EIP repository for a while. Yeah, I think things that do end up in the informational category should really just be like their own web page, like or their own doc site or go to ethereum.org and draft up like a thing there, or hackmd article or any number of other places that is not a technical standards. Again, I’m mostly alone in this, like I think Greg has spoken out about being generally in favor of informational EIPs and previously Nick was in favor of them I believe. So you wouldn't be going against the grain if you decided to approve this, you would just be going against Micah, and you know I really don't care. I’m just not going to put my stamp on it that's all. 

**Pooja**
Yeah, I think that is fair. Unfortunately, Sam has to drop off but I think the recording will help him follow your opinion on this, and I am not an EIP editor. I cannot definitely approve that, so we'll wait for more EIP editors to chime in. I was just hoping to look into some of the enhancement features to be added for bot that some reminders can be sent out to the EIP editors like if that is long lost. 

I think there is another pull request, which I believe is created by you. The number is 4601, created by Micah, and yeah, this looks like the even the author has approved it but this is waiting because two reviewers have been requested to review and it's pending on that.

**Micah**
Let me take a look. A valid concern. I think it was Alex who said they were against the change and that's kind of why it stalled out I think their argument against it was reasonable and so I’d be very hesitant to override that, especially for a final EIP. 

**Pooja**
All right, the reason I found these things to be addressed soon, because if you don't do that this will again start piling up and the number of open pull requests would be so much that it would be again the same problem, so if we came across these kind of pull requests and we think that it is not good to be proceeded probably we can…

**Micah**
Can take another look at this and see if it's worth keeping open? I’ll need to sit down and read through the whole discussion again. If you don't hear from me, like in a day or two uh feel free to ping me again about it.

**Pooja**
Sure. Thank you. 

**Micah**
’ll at least try to leave a comment saying what my current thoughts are.

**Pooja**
Yeah, I think that would be helpful. Okay so that was it. I am not sure like if we have any recommendations suggestions for creating issues for having this bot sending reminders because I know this is like of the lowest priority if at all we consider this because there are a lot of other open issues that needs to be addressed before this so maybe I can let it live here, come back in future meetings and discuss this again. 

## 3. Github discussions for discussions-to [Ref](https://github.com/ethereum/EIPs/issues/4879):

**Pooja**
Moving on to the next item listed here. GitHub discussion for discussion 2 link. I have picked this one from the issue that is there on EIP GitHub, also from the earlier discussions regarding this particular issue. The issue that was highlighted was fellowship of Ethereum magician does not allow to edit the post like author cannot edit the post so I tried to reach out some of the maintainers of their website and from what I was communicated by the team there is this field - post edit time limit. It was then set at a certain number which was greater than zero, however it is possible by setting it to zero that means an author who has some reputation on that forum, say tl0 or tl1 they are allowed to edit their post for like unlimited period of time, so if an author is really new, maybe that would not be working for them, but if he or she has certain reputation and they belong to tl0 or tl1 author, then they would be able to edit the poster and my understanding is like the team agreed to make it to zero though I cannot say it for sure because I haven't verified it, so I would appreciate someone looking into it and if there's issues still persistent maybe we can reach out to team. 

**Micah**
Does anyone does anyone have a very old Ethereum magician post that they've written that they want to try to edit? I don’t know if I have any. 

**Pooja**
I’m not an author of any proposal. I proposed many times but it ended up somewhere else and that's okay. So maybe if it is fair we can maybe consider that this issue is something that can be taken care of if someone has any challenges editing author stuff, then we can definitely reach out to team but I think it should be resolved and that should not be a case. Other than this particular issue, do we have any other thing that needs to be addressed for the fellowship of Ethereum magician to be considered as main discussion to link or the place? 

**Micah**
I believe the ability to edit original posts was the primary thing that would like, the primary argument that was made against using Ethereum magicians. So I'm currently looking at very magicians and it does not appear that I can edit an old post of mine.

**Pooja**
Have you authored that post by any chance?

**Micah**
Yeah, so I have a post that I wrote back for instance for eip2718. This is back in June 2020, and I do not see an edit button for it, which I assume means that I don't have the ability to edit. 

**Pooja**
Okay thank you so much for highlighting that. Maybe I can go back to the team because I understand from my last conversation, the team agreed to make it zero, that it should be allowing people to be able to edit it for any period of time. Okay, yeah find out if they actually did that or not.

**Micah**
I don't see it anywhere or maybe it's not retroactive but I would assume it would be.

**Pooja**
Okay, yeah, I will definitely check on it. Okay thanks. All right. Yeah anything more on this topic? I’m definitely owning this task to check out with the team and get this issue resolved but I’m hoping that if this issue is resolved probably we can start promoting fvm as a forum for discussion tooling.

##4. EIPs GitHub page renderer has a critical vulnerability (can lead to RCE). [Ref](https://discord.com/channels/595666850260713488/746566142700814426/949253019558641664):

**Pooja**
The next item on the agenda is EIP's GitHub page renderer has a critical vulnerability. I believe Micah has pointed out this thing on discord. Just wondering if this issue is resolved or do you need any resources. 

**Micah**
This is an ongoing issue. We don't have anyone on our team who is a ruby expert or even knows anything about ruby at all and since Jekyll is ruby when there's a vulnerability or we need to do a Jekyll update or some or ruby dependency update, none of us know how to do that and none of us have the time to go and figure out how to do that.

**Pooja**
Not a problem. I think we can ask our community for help and we may be looking for someone who has knowledge on ruby and if they are willing to come and help on updating the Jekyll updates here. I just wanted to be sure that if this requirement is still open so we shared the word out and try to get someone.

## 5. Execution specs. & the proposal for Core EIP standardization process.

**Pooja**
Okay. I'm gonna skip the number five item execution specs. I know Sam Wilson has
to drop off so I’m gonna skip this item number.

**Micah**
Sorry. I just realized I was talking about the ruby stuff and didn't realize I was muted before the…so for the previous one I was restate what I thought I even told you is an ongoing issue we don't have anyone on the team who knows ruby or has an inclination to learn ruby but Jekyll which is the thing that renders the pages in to the eips.ethereum.org is written in ruby and so when we have a vulnerability that we need to address or we need to do an update or something none of us know how to do that or how to evaluate such an update or how to make sure it works anything like that and so we need somebody who has some amount of knowledge of ruby to help with that, ideally on a recurring basis, because it's not the first time this has come up. 

**Pooja**
Okay, we can add that information. Just curious, do you think it will help that this piece of code be written in some other language and then be used, like we did rewrite the bot eip bot again, so do you have any thoughts on that?

**Micah**
That would be a pretty large undertaking. I'd be hesitant to go down that route, just because I know how like big and complicated of a task that will end up being. It's not impossible but I wouldn't recommend it. 

## 6. EIP bot Issues and eipv Issues updates

**Pooja**
Sounds fair. In that case we will continue our search for a ruby expert to look into these issues. Okay the next item, bot issues and EIPV issues. I know there are a lot of open issues right now and I am looking for more people to join in to help us get those issue worked on so if someone who is listening to the call and would like to contribute to the Ethereum EIP Github repository, please take a look at the EIP bot issues and EIPV issues links are available on the agenda. 

## 7. EIPs Insight - Monthly EIPs status reporting.

**Pooja**
The next item is EIP's Insight. So in the month of March, so far, one significant change is merged to EIP 1 and that is limiting links to external resources and there are certain wordings that have been changed to EIP 1. So please take a look at it, if you are an author and maybe try to avoid using any external link going forward. There are two new proposals which are merged. EIP 4844 and EIP 4863 and only one proposal so far has been moved to stagnant, that is eip3326 wallet switch etm chain rpc method. This is just the start of the month so we would be expecting more mergers coming soon, but on this particular proposal, Micah, if I can ask for your opinion here, the proposal number 3326, it looks like it's an interface proposal right, and earlier we decided that the process would be different and we may not be continuing 3326. You said…

**Micah**
That's correct. That's the ERP's repo. This looks like it's merged. What's the question?

**Pooja**
I know most of the EIPs on the interface level are going to be moved out of it, so that's it like, should we start closing it or we should wait for bot…I think waiting for bot would be a good idea right?

**Micah**
I’m fine with just letting them fall into stagnant eventually um if they're not finalized and if they are finalized. I’m okay leaving them there and at some point we may just remove the interface section from there I know we shouldn't do that. Yeah, I think my preference is to let the bot turn them stagnant eventually if they're not finalized and if they are finalized just leave them there for the time being that's my weak preference but I’m open to arguments against them.

**Pooja**
Yeah. I think in the next six months we would be expecting some major overhaul with this EIP process, so if at all possible taking the advantage of change of the process we can try to add or remove the categories we want to see or we don't want to see in the EIPs in future. 

## 8. EIP editor apprenticeship meeting
Meeting 14 (Planned on March 22)

**Pooja**
Yesterday we could not have the meeting and the next meeting is planned on march 22nd number nine is EIPIP meeting time and name survey. I did talk about it in the meeting earlier so if you are an eip editor and you would like an alternate time for this meeting because it would be nice to have all EIP editors get synced once in two weeks and close the open issues. I hope that that is going to be helpful for people so if you are open to it please fill out this small survey for us.

## 10. Review action items from the previous meeting

**Pooja**
So from the last meeting it seems there were three action items formal on boarding off for William Schwab and Sam Wilson. Sam has already been added as EIP editor and I believe EIP 1, it's also updated because I remember seeing simple requests to update eip1, but William Schwab, I have shared the link with him and I’m hopeful that whenever he gets a chance he will make that pull request. Yeah, action 50.2, Pooja will get in touch with Andrew in order to remove EIP 1706 from the yellow paper: So Andrew confirmed me this morning that the yellow paper has been updated and I hope that 1706 is removed from the yellow paper. Now action number three, Shashank will create an issue to fix the validator check field withdraw reason I don't see Shashank on the call. Maybe we will check on this issue list, if that is created or not, if not, then I will follow up with him.

# Attendees
* Pooja Ranjan (host)Micah Zoltu
* Micah Zoltu
* Sam Wilson

# Date for Next Meeting: March 23, 2022 at 1500 UTC





