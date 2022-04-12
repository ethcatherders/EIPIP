# EIPIP Meeting 15 Notes
### Meeting Date/Time: Wednesday 26 August 2020 at 15:00 UTC
### Meeting Duration: 24 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/29)
### [Audio/Video of the meeting](https://youtu.be/y6LBpY6byd0)
### Moderator: Pooja Ranjan
### Notes: Jim Bennett

## Summary

## Decisions Made:

Decision Item | Description
-|-
**15.1** | Bring up EIP repository scope and triaging permissions in next meeting
**15.2** | Discuss EIP repository scope and triaging permissions in next meeting if hard fork coordinator is available for questions.
**15.3** | Wait two weeks to discuss onboarding EIP editors survey after receiving survey results.
**15.4** | Wait for James to discuss clarifications for how a precompile address is decided.


## AGENDA

## 1. [Network upgrade process](https://youtu.be/y6LBpY6byd0?t=7)

**Pooja Ranjan**
Hello, everyone. This is EIPIP meeting 15. The first item on the agenda today is network upgrade process. In the previous meeting, we had two different proposals, and we had some discussion on what the network upgrade process should look like. There is an repository - eth1.0/specrepo that has been created to have network specific proposals contained there. We are trying to move EIPs, those that are not directly related to technical specification to network upgrade. The first one was proposed by Edson. Edson, would you like to just give a quick recap and then we can discuss further?

**Edson Ayllon**
Yeah, so we've been working on improving the network upgrade process. Last time, we looked through different options for hard fork coordination statuses.We decided on a combination of statuses. I can post the [link to it in chat.](https://gist.github.com/edsonayllon/e9b91a2c3a8e2d4e242cfc236162e106) And then during the AllCoreDevs, I presented the EIP statuses. It looks like there wasn't any resistance. There's not much feedback. So I guess the next step would be creating a PR on EIP 1 and then seeing if there's any feedback there, then merging it. So we still need to spec out the process for hard fork coronation since last time it was postponed because James isn't here. James isn't here again. So do you want to postpone this again?

**Pooja Ranjan**
I think we can share both the links. And there was another proposal by myself as well. It was just about the process of how we are going to maintain it. And I had a discussion with James offline, and what what he suggested is that we should be talking about the stages that we should be considering for EFI - Eligible For Inclusion - proposals that we are trying to consider here. So if people have different thoughts on how we can categorize these different stages and would like to discuss, I'm happy to open the floor for anyone, if they have any comment

**Alita Moore**
They look good to me.

**Pooja Ranjan**
So, yeah, if we would like to wait for him because this is something that is directly related to hard fork process, so I agree that we should be waiting for him to make a decision on it, or maybe in his presence we can discuss it further. So if there is no further comment on this topic, we can move on to our next item.

## 2. [EIP repository scope and triaging permissions](https://youtu.be/y6LBpY6byd0?t=216)
The next item is EIP repository scope and triaging permissions. A couple of meetings back, there was this discussion that we should limit the EIP repository scope. And this network upgrade process was coming directly from there. I see a few people on the call. If they would like to add things, like what should be the scope for EIP repository only, like what kind of EIP should be submitted in there. And then we discussed the other time the triaging permissions. And I think lightclient, was if I'm not mistaken, lightclient is also working on a permission. So if they would like to provide us the status or how we are working towards it.

**lightclient**
I'm still waiting to connect with Hudson about setting up the triage status, the triage roles on each repo.

**Pooja Ranjan**
Okay, so, unfortunately, Hudson is not available today. So maybe in the next meeting, we will to bring this up again.

I see a comment by Micah on the chat. I'm going to read it:

"My desired scope for EIPs repository: Technical specifications, as free from politics (which includes mainnet inclusion) as possible," and he also mentioned examples as RFCs. Sounds good. And I think we are trying to separate the EIP repository and hard fork process. It's better to get these things documented [crosstalk]... would help any other author in future what kind of proposal he is trying to submit and where he should submit. Maybe we could continue discussing on this topic in the next meeting when we have the hard fork coordinator as well available for the meeting. If anybody else has any comment on it?

## 3. [Further discussion on EIP working groups](https://youtu.be/y6LBpY6byd0?t=348)
Okay, then let's move on to the next item. The next item is further discussion on EIP working groups. In the previous meeting, We discussed some working groups suggested by lightclient like what, who and what goals we are trying to achieve. There is a [link in the agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/25#issuecomment-664579942). If we get into that, we can see all different categories of that. We discussed what these groups could be, and they would like to discuss it further how we are actually trying to or who can be actually be grouped there. So if you would want to talk more about it.

**lightclient**
Any major updates this meeting? That is something I still think is really important, and I'm trying to write some proposals and figure out how to do this in a way that's going to be most effective. I think I was a lot more ambitious last meeting whenever we brought it up, and after, when I was talking to some people and trying to actually formulate what this would look like, I've gotten a little bit less ambitious about it. Because I think it's really difficult to get the community oriented around something that has a sort of accountability, something that's not very easy to force upon people unless they also want it. So I'm trying to figure out how to put this in the best light so it's something that people want, rather than something that I'm trying to force on. So hopefully, two weeks the next meeting, I'll have something more concrete to share on this.

**Pooja Ranjan**
Sounds good. Looking at a glance, I feel like the first three , we have been actively discussing in this meeting, the EIPIP meeting. So that should be not that difficult, but coming up to the rest of those like networking, ERCs, and RPCs, we would like to definitely hear something, some better process for that. I think that's going to be helpful for us as a group to suggest to the developers and follow it in the future.

**Brent Allsop**
I'm not seeing a governance working group. It seems like, to me, there ought to be a governance working group. Is that something we hate so much that we don't want a governance working group?

**lightclient**
I'm purposely trying to avoid anything related to governance, focusing on the technical aspects of building working groups and helping direct resources in to places that people think are going to be useful for the future roadmap. The questions of what should be on the roadmap, and if this thing is built, should it go in, I just don't know if I have the experience to really come up with anything around that.

**Brent Allsop**
Yeah, I'd love to be involved in something like that. And that seems like to me there ought to be something where anyone who's interested in governance could be say, "Okay, I'm interested in governance, I should go there." And I would love to be wherever that is, but I just don't know where that is.

**lightclient**
I feel that should fit in with the new repo that Hudson made for the Eth1.0 spec, the network upgrade sort of repository. I don't think they've done really any work to actually set up a structure for that yet. But my mind that's where the governance discussions will be happening, should be happening.

**Brent Allsop**
So tell me what that is again? I'm not familiar with that.

**lightclient**
I'll send a [link in the chat](https://github.com/ethereum/eth1.0-specs) in just a second. But maybe two meetings ago, Hudson had mentioned that he was going to create a repository focused on network upgrades and separate that from the each repository and he named it Eth1.0specs.

**Brent Allsop**
Okay, cool. Thanks. Thanks for that update.

**Pooja Ranjan**
Adding to this, there are a few comments from my car in the chat box:

"I have a dream where we one day split ERCs from EIPs repository.  But I think that is far in the future.  😊Historically, everyone participating in Ethereum has actively avoided any kind of power structure, which includes any form of governance."

But I think that even this EIPIP group in itself is a part of governance. We are trying to help out structure as much as possible, discussing everything that may or may not affect the general flow of Ethereum governance.

## 4. [Onboarding EIP editors survey to set expectations of an EIP Editor](https://youtu.be/y6LBpY6byd0?t=627)

Moving on, the next item is onboarding EIP editors survey to set expectation of an EIP editor. Edson, I think you were running a survey, so please take it away.

**Edson Ayllon**
I think we should wait another two weeks to receive the survey results.

**Pooja Ranjan**
Sure.

## 5. [Peep an EIP - An EIP focussed series](https://youtu.be/y6LBpY6byd0?t=669)
So the next item here is [Peep an EIP](https://github.com/ethereum-cat-herders/PM/projects/2) - An EIP focussed series. I wanted to bring this to the EIPIP meeting, because I think that is going to help us along the path somehow. With this series, we are trying to get information about EIPs in a community understandable format, not very, very technical, and people should be aware of EIP. I'm trying to figure out the answers to the questions that we as a group are trying to find. One of those questions is that we have a number of EIPs in draft status. We don't know how to move with that.

So, first of all, I would like to start by saying a big thank you to Matt, the lightclient, who has given a very good presentation on how to write an EIP. So it's a very good episode stating about what are the do's, don'ts, what EIP proposal can be considered as good, and which one has chances of moving ahead. I would highly recommend people to go ahead and watch that episode on Peep an EIP.

Now, the thing I wanted to bring with this topic is what and how we are planning to deal with ERCs. I remember reading comment of Micah that in the future, EIPs and ERCs should be in different repository, but now they are in one, and there are plenty of ERCs which are in draft status. One of those is EIP 173 that we discussed in this series. And the author is very much interested to push it forward. The EIP has already gone into Last Call. And I think the Last Call date has already passed somewhere in early August. So I'm looking forward to the next step. How such EIPs can be moved forward, whom they should reach out to, to push these. If people have any suggestion on that?

**lightclient**
I think the next place to go would be AllCoreDevs.

**Pooja Ranjan**
The thing is, these are not core protocols. These are ERCs, so I'm not very sure about bringing it to AllCoreDev meetings. I don't know how it has been done historically. I think in here I'm gonna going to remember Hudson, because he has been part of this process for a very, very long time, and I had hoped that he could have advised something here. But nevertheless, I would like to keep this agenda item open, how we can clear out the draft EIPs. Those are there for over two years. This particular EIP that I'm talking about, it was proposed in 2016. And then from 2016, it was actually Draft in 2018, and now it is 2020. We're still there. So I think we should work on a process to take care of these proposals, and then we will be able to clean up our repository. So that that's the thing I wanted to bring up with this topic, but in general, I would highly recommend people to go ahead and watch this series, which is available on [Ethereum Cat Herders YouTube](https://www.youtube.com/channel/UCD9iiIwTRtLDYcEWONs2Q3A), and let us know what other proposals people would like to hear and how we can make this beneficial for our community.

## 6. [Clarifications for how a precompile address is decided.](https://youtu.be/y6LBpY6byd0?t=895)

Moving on, the next item on the agenda is clarifications for how a precompile address is decided. There is [a link in the agenda](https://ethereum-magicians.org/t/proposed-process-for-assigning-opcode-address/4302/3), and I think this is a proposal by James, and he was working on it. I do not have any updates. If anybody else has any, please feel free to share. Or else maybe we will wait for him to join us in the next meeting. Then we'll discuss this further.

## 7. [Discuss the EIP-1 Brainstorming Document](https://youtu.be/y6LBpY6byd0?t=940)

The next item on the agenda is [a link](https://hackmd.io/TKGYSvz9Rt6v5VaNpGaWHw), actually. It's for EIPS to do. It's a document that we created a while ago, and this is actually listing what we are trying to do as a group, like EIPIP group. There are certain goals that are listed. Number one is reduce the number of PRs. I think teh Peep an EIP series is going to help us and move in that direction. Next goal is reduce the number of abandoned drafts. We are trying to identify drafts which are not of any significance, or maybe they have been overwritten by other proposals. In that case, we might want to remove that and ask the author to withdraw or close it. Matt, is it okay to ask that the validator bot that we are updating, will that help us in identifying these proposals and remove them from the repository?

**lightclient**
I don't think the validator's gonna help in this effort. I think this falls under the auto merge bot more.

**Pooja Ranjan**
Got it. But that is another thing that we might have to look into if it is a manual work, or we will try to filter out the proposals or Yeah, let's see how does it come out.

The next goal mentioned here is move a bunch of ERCs to the final status. We are trying to reach out to the authors at this time. We have very, very few ERCs in final status and over 100 of them are in Draft. So we are looking into each of these proposals to push it to the next status. I think that's it from this document. This is originally maintained by James Hancock. So if he has further things to discuss, we'll look into the next meeting. I think it's going to be a very quick meeting today.

## 8. [Review actions from previous meetings](https://youtu.be/y6LBpY6byd0?t=1071)

So the next item is review actions from [previous meeting](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20014.md).

## Decisions Made

Decision Item | Description
---|---
**14.1** | Hardfork coordination upgrade talk awaiting until James joins.
**14.2** | EIP repo scope constraint awaiting until James joins.
**14.3** | Small working groups to be tested.

I know we discussed and lightclient mentioned that he would be coming up with a more formal proposal in the future meetings, and then we will start testing on it.

**14.4** | Get final approval from ACD on new EIP statuses.

As Edson mentioned, he has already shared this with the AllCoreDevelopers, and there was no strong opposition. So I think the next thing would be to draft it in a PR and add it to EP 1. But in one of the previous meetings, we discussed that we would be doing it when we get clarity on network upgrades as well. The processes would be combined together, and then we will create a pull request for all.

**14.5** | Create triaging permissions for Github.

Lightclient would be working with Hudson to look into the triaging permissions.

With that, I think we are at the end of the meeting. Anybody else has anything to discuss, feel free.

**Brent Allsop**
Yeah, I'd like to just get everyone's opinion on EIP 2878, the block reward reduction 2.5 Eth. Just kind of wondered if anyone here is either strongly for or strongly against that. It sounds like the community in general wants that. But it sounds like the miners don't want that, of course, because it's going to take away money from them. But anyway, I wondered if anyone would think it would be worth creating a petition or something like that, but it sounds like that's kind of a controversial EIP. And I wondered if anyone here thinks pushing for or against, or doing some work trying to put possibly a [Canonizer](http://canonizer.com) petition together to try and build and track consensus around something like that. Or is that something that no one here would be interested in either fighting for or against? Anyway, just wanted to get if anyone has any thoughts on anything like that?

**Pooja Ranjan**
Would it be possible for you to just [link this EIP in the chat](https://github.com/ethereum/EIPs/pull/2878) so people can give a quick look at it.

Meanwhile, I would like to read a couple of more comments that we received in the chat about the PR blockage backlog problem. Micah suggested:

"Solution to the EIP PR backlog problem:1. Add one or two active editors.2. Go through backlog and start closing PRs and marking EIPs as abandoned."

Yeah, I think this is what even James was proposing, that we have to start marking that as abandoned. We started this, but we stopped in between, because we were looking for getting clarity on statuses for EIPs. Now that we have it in place, we can restart this process Cat Herders are maintaining a list or where virtual IPS are in draft status and who is reaching to which EIP author to check with him if he would like to pursue that EIP if it has been superseded or we can go ahead and close it as abandoned. So we would like to revive that process. And with that, I hope that this backlog problem could be at least minimized.

Okay, on EIP 2878, Brent has [shared the link in the chat](https://github.com/ethereum/EIPs/pull/2878) if anybody has any quick comment, I see that many people have already commented on the pull request. So if people have any comment, feel free to add it over there. And if it still needs to be discussed, we might want to bring it into another call, but I'm not sure if we are trying to discuss individual here, but something that is related to any particular EIP, we would be happy to discuss and come to a resolution there.

So with that, I think we have almost covered the items that were listed to discuss today. Anything that people would like to be discussed in future meetings, please leave that in the agenda, or you can always say it anywhere related to this GitHub repository. So yeah, that's it from my end. Thank you, everyone, for joining us today.

Before we end, I would like to mention two more comments received for EIP 2787. It is from one of the editors. Micah, you mentioned that at least 2787 needs to be fixed so it is a valid specification. Currently, it has a bunch of problems. And I guess lightclient has already commented on that pull request. Likely the specification doesn't actually specify anything. I'm sorry, the number is 2878. We may discuss it again in the next meeting. And I think with that, we have covered everything that we would like to discuss today. Thank you, everyone, for joining us today. It was a very quick meeting. I hope next time the hard fork coordinator is here and we'll be able to make decisions on many other things.



# Attendees

* Alita Moore
* Brent Allsop
* Edson Ayllon
* Jim Bennett
* lightclient
* Pooja Ranjan


# Date for Next Meeting: 9 September 2020, at 1500 UTC.
