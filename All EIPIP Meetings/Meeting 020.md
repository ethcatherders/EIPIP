# EIP# EIP IP Meeting  20 Notes
## Meeting Date/Time: Wednesday 4 November at 15:00 UTC
### Meeting Duration: 1 hour 30 minuts
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/38)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=m1A3F4v7H4M&feature=youtu.be)
### Moderator: Pooja Ranjan
### Notes: Jim Bennett

----
## DECISION ITEMS

**DECISION 20.1**: We will have a Review state for EIPs.

**DECISION 20.2**: Meta EIPs will now be called Special EIPs, and only EIP-1 will have a Special state.

**DECISION 20.3**: If there is a change to the process that is proposed via PR to the EIPs repo, the editors will be tagged on it. And then after two weeks, if none of them have responded, or if the only ones that have responded have responded positively, then we'll go ahead and merge it.

----

**Micah Zoltu**
[Starting at 3:58](https://youtu.be/m1A3F4v7H4M?t=238)
I would say to get your EIP at least into Draft. I've seen plenty of people try to bring EIPs to the CoreDevs without it even being in Draft yet. And that's almost certainly not going to work well for you. The other thing I think you can do is, once we institute the Review step, assuming that goes through, then getting it all the way to Review would be most appropriate. The Review stage will, if we go forward with that, indicate that the EIP is ready for general consumption and review. And ideally it means an editor will go through and make sure that everything is structurally sound, well worded, stuff like that. So by the time it gets to review, hopefully, you'll have at least one other person who has looked it over who is familiar with the process and understands how things work and has at least tried to work with you on getting it into a good state.

I think the last thing is, I mentioned this in the Peep-an-EIP discussion, keep your EIP small. Small and short. So change the least possible amount of things in any EIP as you can. And also try to keep the the text to a minimum. While I know it's tempting to write a long essay about why your EIP is great, CoreDevs are very short on time. And having something that's quick for them to scan over and read is very valuable. And this is where the abstract comes in very handy. And simple summary, keeping the simple summary very simple, like one sentence, like a subject line of an email really does help. And the abstract, have it be a human readable and very short version of the specification. So CoreDev who just wants to get an idea of is this something that I support can just read the abstract and be done with it in a minute or two. So if you want to get your EIP merged, that would be my advice. None of this is a guarantee, of course. But I think that's your best bet.

**Pooja Ranjan**
[Starting at 1:06:13](https://youtu.be/m1A3F4v7H4M?t=238)
So while we have a good amount of editors on the call. There is another item, which was sometimes discussed, but it has never appeared as a part of an agenda item here about the meta and information EIP. What is the general opinion on that? We have heard certain people's opinion, including mine, too. But is there anything new to be added? Do we really think that we should have meta and information EIPs be the part of the EIP repository or not?

**Hudson Jameson**
I believe we should have meta. That serves a better purpose than informational. I'm indifferent on keeping informational, because I think it's not used very much. And I think it was Micah or Greg or both who said that this is a specifications repository, and therefore, having an informational EIP kind of throws a wrench into things as far as the purpose of the entire repo.

**Micah Zoltu**
It's a slippery slope. Because there's no clear line to draw, in my opinion. There's no clear line for, "This is acceptable for this repo, and this is not," because I've seen people submit informational repos or informational interviews are like, "Hey, I'm documenting my app in the EIPs repo, and it's informational, so that's okay." And as an editor, I do not have a strong argument other than I feel that it's not appropriate for this. And I'd rather have better statements than I feel.

**Greg Colvin**
Yeah, I think we've had those for a while. We picked them up from the EIP. Yeah, I think we can just tighten down the standards on those. They should still be technical documents, not necessarily specifications to build something, but technical documents offered for technical discussion. And it's not that slippery.

**Pooja Ranjan**
So a recent addition in the information category is EIP 2982. That is about the Serenity Phase 0, or that is created by Danny Ryan and Vitalik Buterin. It talks about this Ethereum 2.0 Phase 0.I personally feel that these kind of informational EIPs are valuable. And for that purpose, we should certainly have the informational EIP in that repository. And of course, we can do screening or what could be approved and not approved. But that's my general thought on that.

**Greg Colvin**
Well, that's that's an example where substantively it's very controversial. But I think when we were done, the editors and the authors were satisfied that it was a technically useful document that wasn't making commitments to do anything, or just going over the history of things, but saying, "This is a plan to improve Ethereum that we're working on. And it's a separate project, but here's what's relevant." Yeah, so it was a useful technical document that was informative to those working on the 1.0 chain. And I think we can start to draw those sorts of lines.

**Pooja Ranjan**
All right. Drawing lines would certainly help, but the purpose of informational documents is to provide all kinds of information that is valuable in the Ethereum ecosystem. That is still a question of how we want to go about it. And about that meta EIP, historically, we have been using meta EIPs for having all the proposals which undergo any network upgrade. Now we have Berlin coming up, do we want to maintain that meta EIP for Berlin?

**Micah Zoltu**
I believe we've all agreed to the best to move it to Eth 1.0 Specs Repo for hard fork coordination.

**Pooja Ranjan**
Right. So, in that case, I don't really see any more use of meta EIPs there. Do we still want to have it, although it explains the process. And that was one example that I came across explaining of the process, and the other one is to keep the list of EIPs. And if we are containing the list of EIPs at the 1.0 Spec Repository, do we still see the need of having metal in the EIP repository?

**Hudson Jameson**
Well, isn't EIP-1 meta?

**Pooja Ranjan**
That is, yes.

**Hudson Jameson**
What else would it be if it wasn't meta? That's my number one reason for keeping meta is for EIP-1.

**Micah Zoltu**
So the question is, is there anything else that would go into meta besides EIP-1? Or is meta literally just EIP-1?

**Hudson Jameson**
It's literally just EIP-1 for now. And if there's anything in the future that requires it, like if we were to eventually split out ERCs and EIPs, for instance, there might need to be a meta talking about that. Otherwise, no.

**Pooja Ranjan**
So we have this discussion in this call today about EIP-1. So EIP-1 is considered to be the process explaining the process of EIPs. And it's a documentation for explanation of the process for EIP standardization. Similarly, we have a process for different other things. Again, I do not want to get into that network upgrade in this thing. But yes, we decided that the network upgrade process should not be documented in meta, but it should be in the readme file. So there was another discussion of EIP-1, before some of you who joined today, about having readme and EIP-1 in the same page? Do we need to have these two separately, or should we have it in one?

**Micah Zoltu**
Before we move on, real quick, I don't want to go too deep on this rabbit hole, so just know I don't actually have a strong opinion here. I wonder if there's value in renaming the "Meta" status to "Special," just to indicate that this is not a status that anyone should probably ever go create an EIP with this status. This is for very special and specific things that only the editors really understand, so don't try. Just kind of making it more clear that the meta EIPs are not the thing for end users to be using, so stop creating meta EIPs.

**Hudson Jameson**
I'd be fine with that.

**Brent Allsop**
Sounds good.

**Micah Zoltu**
Sorry, that's a sidetrack.

**Pooja Ranjan**
No, that's all right. That's really helpful. So I think when we are having that blog, I know Edson has dropped, but we would like to let these points be included in that blog, so that this information should be publicly available for people to refer to, and then the confusion around this will be solved about whether it should be meta or it should be informational and others. That's my hope.

**Micah Zoltu**
I'm fine with blogging about anything. Anyone wants to do it? I tell a lot of EIP authors, "You should go blog about this instead of writing an EIP."

**Hudson Jameson**
Yeah.

**Pooja Ranjan**
So yeah, I think most of the items that were added for discussion today we have covered and we went a little over time. Sorry about the confusion created with the Daylight Saving Time. This EIPIP meeting generally takes place at 1500 UTC. And we would like to keep it that way if we do not come across many people saying that we may want to change it. But if not, then the time is 1500 UTC. So, if anybody has anything else to discuss, we can take five more minutes, otherwise, we can wrap it.

**Brent Allsop**
I would like to take a sec, just to review the decisions made.

It sounds like one decision made is we will have a Review state.

And the other decision made was we're going to convert Meta to be Special, and that EIP-1 is the only one that has a Special state. Have those decisions been made?

**Micah Zoltu**
That's what I got from this conversation.

**Brent Allsop**
Okay, just wanted to make sure.

**Micah Zoltu**
And Micah is Dictator for Life.

**Brent Allsop**
Oh, yeah, yeah, yeah. Gotta get that.

**Micah Zoltu**
More specifically, we're saying that if there is a change to the process that is proposed via PR to the EIPs repo, the editors will be tagged on it. And then after two weeks, if none of them have responded, or if the only ones that have responded have responded positively, then we'll go ahead and merge that.

**Brent Allsop**
Oh, great.

**Pooja Ranjan**
So thank you everyone for joining today. The next meeting is on November 18 at 1500 UTC. See you all in two weeks.

**Micah Zoltu**
Really, really quick before you stop recording, since we have Hudson and Greg here, speaking of "Micah as Dictator," there are a few EIPs that I personally am not merging because I disagree with them. But I believe that I'm alone in not merging them, so we need some other editor to step in and merge them. I should not have the power to block.

**Hudson Jameson**
Can you send me the links to those? Because my GitHub notifications are a little out of control.

**Micah Zoltu**
Where's a good place to get ahold of you?

**Hudson Jameson**
Discord or Telegram. Either one is equally fine.

**Micah Zoltu**
Okay. I can send them over to you. I'll have to dig them up. Pooja, you actually know what they are, because I think some of them are yours. Basically, any informational or meta EIP, I have been personally blocking. Not blocking, just refusing to merge. My hope was that some other editor would step in and merge because they think those are okay. And I don't necessarily want my personal opinions to be dictator-like, but they're ending up that way, just because I'm taking a personal stance by not merging. But if someone else merges, I'm not gonna fight it. And it's turning into, I'm blocking things and that doesn't make me feel good.

**Hudson Jameson**
Okay, sounds good. I can help.

**Micah Zoltu**
Okay, I'll try to find them and send you links tomorrow.

**Hudson Jameson**
Thanks for running this, Pooja.

**Pooja Ranjan**
Thank you, everyone for joining.

# Attendees

* Brent Allsop
* Edson Ayllon
* Greg Colvin
* Hudson Jameson
* James Hancock
* Micah Zoltu
* Pooja Ranjan (Host)



# Date for Next Meeting: November 18 at 1500 UTC
