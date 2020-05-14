# EIP IP Meeting 7 Notes
## Meeting Date/Time: Wednesday May 6 at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/13)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=-ZUOWpEuAEU&t=1393s)
### Moderator: Hudson Jameson
### Notes: Jim Bennett

----

## ACTION ITEMS

**ACTION 7.1**:  Make the EFI EIP an active EIP and make it live.

## SUMMARY

Discussion focused on editing EIPs and the challenges and benefits of giving people more access to make changes. The consensus was to avoid migrating EIPs to ethereum.org and whether the EFI process should be added to EIP 1 or kept separate, with the grough consensus being that they should be kept separate. There was also a review of a recent survey on the EIP process that resulted in a discussion of governance structures that would allow greater participation and communication throughout the Ethereum community, and about how large groups of people can communicate and make decisions asynchronously.

## AGENDA

**Hudson Jameson**
It looks like we're live. Hi, everyone. Welcome to EIPIP meeting number seven. I posted [the agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/13) in the group chat, and we'll start with item number one, the EIP-centric model subgroup.

## 1. [EIP centric model subgroup](https://youtu.be/-ZUOWpEuAEU?t=8)

**Hudson Jameson**
I think that was something James brought up a meeting or two ago, but I forgot what that meant.

**James Hancock**
I think that's probably related to the thing that Jamie also had talked about of having a group of people who are administrating the EIP repo but aren't EIP editors and having a role for them.

**Hudson Jameson**
Okay, interesting.

**James Hancock**
That's at least what I remember it as. Does someone else remember otherwise?

**Hudson Jameson**
Yeah, I think you're right. I don't know if I was at that meeting, but that sounds like a good idea. So I guess what that would mean is if you are something else besides an EIP editor, you can still make and push changes to stuff if you are the hard fork coordinator, or if you are - what else? I don't know other roles.

**James Hancock**
In the EIP-centric model EIP, rather than spelling out a bunch of names of people in this group, you could say this group is allowed to make edits to this EIP, and then have a living EIP or an active EIP that specifies who that is. And then we can give and remove permissions as it makes sense.

We also talked about having at the bottom of an EIP an in house form like if you go to the DMV, there are the notes that the other side of the table is taking. And so certain changes in the EIP could be made by this group. But there are things that they wouldn't have access to. So stuff like upgrading processes, we could have better tracking of the process of an EIP within the EIP itself if we had people who had access to those pieces to make those changes.

**Hudson Jameson**
Would we be able to make granular enough permission sets within GitHub to do that? Or what would that be risking people being able to do what they want in the repo?

**James Hancock**
Granular enough. You just use the EIP automerge bot to make sure they only touch sections that are laid out specifically for them to have the permissions.

**Hudson Jameson**
Wouldn't they have to get write access to the repo, though?

**James Hancock**
No. If the EIP automerger verified that it came from someone in the group and was in a place that they're able to edit, the automerger can do it, in the same way that I don't have write access to a repo, but as an author, if I make a change and the bot determines that it fits rules that are okay to merge, it merges that automatically.

**Hudson Jameson**
Okay. What do other people think of this?

**Brent Allsop**
Sounds like a cool idea.

**Hudson Jameson**
Yeah, as we start to update the bot, let's look into doing that for sure, I'd say. Anybody else have comments on that one?

## 2.[EFI admin update & process documentation](https://youtu.be/-ZUOWpEuAEU?t=227)

All right, EFI admin update and process documentation. I don't know, I think that might have been you, too James. Or maybe Pooja?

**James Hancock**
I haven't been here for the last two meetings, so if it was something recent, then it would have been something brought up by someone else.

**Pooja Ranjan**
This is coming up from one of the AllCoreDev calls in which it was suggested that for this EFI process, it might be helpful to have a documentation of that, like, how does it work properly? And also, if there can be some more admins added to the EFI than it would updated more frequently. So it was coming from a conversation on Telegram from maybe a couple of weeks back. James initiated the conversation, so that's why it was added to the agenda here.

**Hudson Jameson**
Okay, what does everyone think of that?

**Tim Beiko**
Wouldn't it just be adding it to EIP 1?

**James Hancock**
That's kind of my first question is I don't know. Do we want it in EIP 1, or do we want it in its own place? Because it goes back and forth.

**Hudson Jameson**
Yeah, I think we need it in its own place. I think EIP 1 should have a level of brevity about it.

**Pooja Ranjan**
So my understanding here is EFI itself is an EIP. So if we would want a documented process, we could go ahead and do that. And about the EFI EIP process itself, sometime back we discussed that it should not be a meta. It should be some kind of informational EIP, and that should be referred to in EIP 1. So I'm not sure what the process is agreed upon, but that was the initial proposal.

**Hudson Jameson**
I like the idea of EFI being its own EIP and then it being mentioned in EIP 1. And the status of the EFI EIP to active. So the same status that the EIP 1 is, which would mean that it can be changed through whatever process is the same as EIP 1 being changed, which I think we determined last time we're not entirely sure about.

**Pooja Ranjan**
Yeah, that that was the discussion about how it should be an active EIP, which is live. And if in the future we would want to change, that status can be changed. That was the initial proposal.

**Hudson Jameson**
Okay, Yeah. So let's make it and make it live. That's a good thing that we can do today to define the rules of EFI as it relates to core EIPs.

**Brent Allsop**
So when you say define the rules, that means specify what is required to be met for an EIP to be EFI.

**Hudson Jameson**
Yes, and it can be very loose if we want it to be, or the EIP author of the EFI EIP if they want that to be a looser thing. And I guess James would be the best person to either do it or advise on it, because you had a big role in coming up with the EFI process. And I can help too.

So, for instance, it would just say, "EFI stands for eligible for inclusion. In order to attain EFI status, the core developers have to come to rough consensus that an EIP is eligible and has a greater than 50% chance of going into a hard fork." Something like that. Whatever rough criteria we have defined, because it's still a little loose right now. We don't have a hard number of "X amount of clients have to say this is a good idea" or, or even what it means to be blessed by a CoreDev or stuff like that.

**Pooja Ranjan**
So if I am not mistaken, James I guess you were the author of that EIP?

**James Hancock**
Yep.

I've been jotting notes about making it more clear. Going back a little bit, I initially wrote it as being a separate thing, and then the EIP was blocked from being merged to draft because Alex wanted it as part of EIP 1. So then, I started making that change, but that's why it's been in draft for a long time. It wasn't even merged as draft for a long time because the prerequisite was it shouldn't have any information; it should only contain the registry of EIPs, and then the rest should be in EIP 1. Then I guess I'm saying that as a point of frustration. We're working with the EIP editors. I don't really know what to do with the non-consensus among the EIP editors on pretty much whatever is going on.

**Hudson Jameson**
And if everyone wants it to be in EIP 1, it's not a deal breaker for me as long as it doesn't get too crowded. Can you link to the EIP, James, so I can see how long it is? Because to me, the the succinctness and the length of it is gonna be what would make it better to go in EIP 1 vs. not better to go to EIP 1.

**James Hancock**
Yeah, I can update. I can send that.

**Hudson Jameson**
Okay. I guess EIP 1 can be pretty long. Do other people have different opinions or complementary opinions?

**Edson Allyon**
I think you for keep adding to EIP 1, it'll get pretty crowded. And isn't it where someone being introduced to the EIP process for the first time goes to?

**Hudson Jameson**
Yeah, it is. And especially because EFI doesn't relate to 99% of people who are visiting EIP 1, that's another argument against it, I think.

**James Hancock**
Yeah, I had originally thought of it as EIP 1 being the center of truth for things related to Ethereum and the EIP process, or just governance in general, being the place that people can reference as the single source of truth. You can make it usable by adding in a table of contents and organizing it very well. So even if it gets long, people can find the information they need quickly. It doesn't really matter how long it gets, because you don't need to read the whole thing. You just need to be able to get to what you need to quickly.

**Hudson Jameson**
That's a good point.

**Brent Allsop**
Yeah, I like that.

**James Hancock**
But a point against that is that EIP 1 has a really high friction to get anything done on it, and so being me able to update it would be difficult. So having it be separate actually would make it easier to keep up to date with the process.

**Tim Beiko**
Yeah, I feel like people would also be able to monitor the changes. So say I care just about the EFI process and it's an informational EIP that's linked in EIP 1 that I can just kind of keep track of that EIP, right? And then the link in EIP 1 will just always point to that other EIP. It might be easier to make changes that way.

**Brent ALlsop**
Yeah, that sounds good as long as there's a link to it that EIP 1 says the definition for what's required for EFI status is defined over there, so people know there's still a single source of truth.

**Hudson Jameson**
Yeah. So also just as a point. would it be an informational EIP or a meta EIP? Because EIP 1 is a meta EIP, I just found out.

**James Hancock**
It would be a meta EIP. I think anything related to the governance of stuff should be meta. Processes should be meta

**Hudson Jameson**
Like self-referential EIP processes. Got it.

**James Hancock**
I did have some other thoughts on things that the EFI list could be used for, or like the process of EFI could be useful for other things. If you look at it from the general, the CoreDevs have consensus to say, "this is a good idea to move forward with as long as it continues to make sense."

For example, yesterday when Tim's PR for changing the names from hard forks to network upgrades came up - that's a PR. It's not an EIP. I don't think it should be an EIP, but there should be some way for the CoreDevs to say they're okay with it, then it could be added as part of it's "eligible for inclusion," quote/unquote, kind of expanding the definition a little bit. But then could this be a way to then make that into Draft and then have it be Last Call, and then say these are lists of PRs and things that are governance and process related that have gone through the system.

**Hudson Jameson**
Yeah. Okay. I like that. I almost want to just push EIP 1 through the changes and then have part of EIP 1 saying editors have to be this active and they have to be involved with EIP 1 updates. Because we have gotten hardly any editor involvement, and I'm guessing they're going to not be happy if we push EIP 1 changes through without consulting them, even though they haven't been here. So I don't know how to tackle that one yet. I have to think about it.

**James Hancock**
We could start by at least recording that it's been "blessed," quote/unquote, by the CoreDev call by the CoreDevs that are on it.

**Hudson Jameson**
Yeah, for the network upgrade thing, I think that's one thing where it's got enough coverage and so few detractors that we can go forward with it.

**Tim Beiko**
I disagree with that one, though, because, I posted it on Twitter, and I think 100% of the reaction from the community has been negative.

**Hudson Jameson**
Yeah, I guess you're right. I didn't look closely at your Twitter post.

**Tim Beiko**
Yeah. That's kind of a sidetrack, but I wouldn't be comfortable pushing it through at this point.

**Hudson Jameson**
Cool. Sorry. I think we got on some tangents. James, What was the main point for the EFI?

**James Hancock**
Where it sits with the process and functionally and then adding people to it, I think we kind of got to the end of the discussion. Yeah, the rest are kind of an addendum.

**Hudson Jameson**
I think next steps on that would be kind of up to you since you're writing it. If you want it in EIP 1 or if you want to try to push it separately, I think that's kind of your decision, but it's good that you're getting input from everyone. And it could go either way. I'm leaning more toward it being separately, personally, for the reasons that we've talked about - because it could they updated easier, and because it wouldn't clutter EIP 1 unnecessarily, and a few other things.

Any other comments on that? Anybody?

## 3.[EIP best practices - EIP 2565](https://youtu.be/-ZUOWpEuAEU?t=997)

Right. The next one is number three: EIP best practices - [EIP 2565](https://eips.ethereum.org/EIPS/eip-2565) I think this is a carryover from the last time. All we're saying by this item, if I recall, is to say this is a really good example of an EIP that we should reference in EIP 1 as an ideal core EIP.

**Pooja Ranjan**
Yeah, and that's about right. It's a carryover item. This is what was discussed in the last meeting.

**Hudson Jameson**
Okay. Anybody else have comments on this?

## 4.[EIP migration to ethereum.org (PR)](https://youtu.be/-ZUOWpEuAEU?t=1036)
Okay, the EIP migration to ethereum.org [(PR)](https://github.com/ethereum/EIPs/issues/2607). That kind of fizzled, for the most part. We have an EIP page on there now. I think we ended up basically coming to rough consensus over time that it's not a good idea to move things from eips.ethereum.org to ethereum.org/eips, because although there would be SEO benefits, it would be - what was the reasoning?

**Pooja Ranjan**
They're planning to add the search button to it. I have just added the [link in the chat.](https://github.com/MadeofTin/EIPs/blob/c81eec79d612359770131116678ee1c992df01b9/EIPS/EIP-xxx.md
) So it's about adding the search button to the existing one. Hopefully, that would be helpful. Depending upon the results, it would be decided or discussed further if we should go ahead and migrating the entire data, or should we keep it the way it is as of now? So that's that's the PR open for comments. We agreed to have comments about it

**Hudson Jameson**
As long as we're not drastically changing the site, adding search is great. I just don't want that to come with moving all the EIPs over to Sam's ethereum.org implementation yet until it's agreed upon, if it does get agreed upon. But I don't think we're there yet, right?

**Tim Beiko**
And it seems out of scope for ethereum.org, right? It's all just pointers to other places. I think the way we have it now is actually pretty good.

**Artem Vorotnikov**
What was the reason that this was rejected the last time?

**Hudson Jameson**
You mean the move to ethereum.org/eips?

**Artem Vorotnikov**
Exactly.

**Hudson Jameson**
So Sam showed us an example of what it would look like. If you've been to ethereum.org, and you go to  - here, I'll post [an example link.](https://ethereum.org/eips/
) Right now, this is how what it looks like - what is an EIP, what is the history of it, etcetera. But if we were to move the EIPs to ethereum.org/eips to where they're searchable in here, it would have that top frame of individuals, developers, enterprise and Ethereum. And it would feel more like a part of a website than a standards platform. It would have a different feel to it. It wouldn't feel as professional or technical is what some people were arguing, including Alex Beregszaszi.

**Tim Beiko**
I think they were also SEO implications?

**Hudson Jameson**
The SEO implications were actually in favor of moving it, because we would get more traffic by having it be ethereum.org/eips rather than what it is now.

**Tim Beiko**
Got it.

**Artem Vorotnikov**
Also, I suppose we could integrate EIPs into the unified translation platform. I don'tr know if this has been considered.

**Edson Ayllon**
Yeah, that was another argument for, that they could help with translations.

**Hudson Jameson**
We could do the translations without the integration, though. It's not like fitting like a glove when you do that. I'm not super versed in the way they're doing translations right now. Also, that would be a lot. I don't think they would want to take that on for translating on the go every EIP that comes in. That is something we should strive for, for sure. But I don't know if they're gonna want to take that on. That would be a question for them.

**James Hancock**
Even just translating EIP 1 would be really hard. We don't even know what it all means.

**Hudson Jameson**
And the wording is overly technical, Not overly technical for what it is, but overly technical for a translator. How would you translate EFI?

**Pooja Ranjan**
Recently I discovered a script translator on Google. I'm not sure if that would be helpful for EIP 1. Somebody can try that.

**Alita**
I would say, in general, you should be very careful with anything automated, because automatic translations are typically like the Holy Grail. So we're not there yet, if that makes sense.

**Hudson Jameson**
You're saying it's a rough translation when that happens.

**Alita**
Yeah, basically, the ability to translate effectively between languages is the goal of current research in speech recognition stuff. So I find it highly unlikely you would find one actually usable. You'd probably be better off finding a good translator.

**Hudson Jameson**
Yeah, or a combination. Do people do combinations? Anybody heard of that? They do the auto translate and then have someone come in and clean it up?

**James Hancock**
My experience with Japanese is that it's really, really doesn't work. But that's probably because Japanese is really, really different.

Overall, I would say if I was looking for a translator for EIP 1, I would probably want basically a lawyer-like level of understanding of language while translating. Because a lot of weight is given to a lot of these words, and not knowing nuance or context to certain things, especially technical ones.

I know that to be a patent attorney, you have to have a dual degree of law and of engineering, specifically because of this kind of stuff. I feel like this is a little bit of distraction, but crowd sourcing EIP 1 translations - I wouldn't be really comfortable.

**Pooja Ranjan**
So there is this team of translation led by Taeyeon from the Ethereum Foundation. And if people find it's worth having the translation of EIP 1. We can probably reach out to her and try to get it.

 **Hudson Jameson**
Yeah, we can definitely get her and put on that if we want to do that. But that's probably lower on the priority list overall. We all understand that, because we're trying to overhaul the system itself in English. So any other comments on that and the migration to ethereum.org that isn't really happening right now, except for added search functionality of the current Jekyll site?

 **James Hancock**
There's still an unsolved problem that there are blockers to changes in the EIPs or EIP processes are on, then being able to render it on the site. Not to go into it, but I'm just noting that that has still been a problem if we aren't having resources and team for it.

 **Hudson Jameson**
That's true. Moving it to ethereum.org, we're kind of less independent, the EIP process and the EIP Jekyll integration is less independent, because then you're relying on links to ethereum.org/eips and whatever they have set up, whether it's Jekyll or an automatic markdown grabbing thing that Sam set up, rather than eips.ethereum.org, which is just a Jekyll plug in. So it's a little more transparent.

 **James Hancock**
I was meaning the other direction, because we don't have any anyone looking at the EIP's site. Like if I wanted to have a change to the header file that added in "Champion" to the header part where the square is, added in "Champion" to that, and then you could put one name, there isn't anyone who could make that change on the website.

 **Hudson Jameson**
Got it. Okay.

 **James Hancock**

And if it was under the ethereum.org team, then there is a team of people that would be able to keep up with any of those changes, like the one we had talked about earlier of making it so the eips.ethereum.org is like a data availability - anyway, I don't want to go all the way back into it. But if it was more raw - it's trying to do both things and it's kind of failing at both of them. So that's just an ongoing problem. And we should mark that down, and we can talk about it next time.

 **Hudson Jameson**
Yeah, I don't know if we'll solve that one today. But are there any comments on that and the others? Okay, we'll think on this more for next time. And it's not a pressing one. Sam's working on the search integration, it sounds like, but not on any further efforts to move the EIPs there right now.

## 5.[Survey on the EIP process](https://youtu.be/-ZUOWpEuAEU?t=1628)

Next up, a [survey](https://docs.google.com/forms/d/e/1FAIpQLSeadXscoQgrKznUOAEB_jSzNNFKHWDEFJxKH1LpDsDsC6mXpw/viewform?usp=send_form) on the EIP process. A blog was released, and I think Edson can talk about that.

**Edson Ayllon**
Yeah, so a blog was released. There showed up patterns of all responses. So I collected the patterns. I can [link to the blog below.](https://medium.com/ethereum-cat-herders/the-feedback-that-improves-ethereum-ff4f3f36a8e2
) Do you want to talk about the findings? Or should save that until all the final responses are received? Or we can start working on solutions.

 **Hudson Jameson**
Maybe wait until all of them are received. I don't have a huge preference. What do you all think?

 **James Hancock**
Whatever Edson wants to do.

 **Hudson Jameson**
Yeah, it's your call.

**Edson Ayllon**
I think we could start figuring out a wave of solutions or at least know what the current problems are. And then we could bring solution for the next meeting.

 **Hudson Jameson**
Okay. Sounds good.

**Edson Ayllon**
So the major ones are politics. How can you keep the EIP process apolitical? How do we create a sense of finality? And how can controversial EIPs be introduced? All these have to do with decision making. So the overall question of how to solve this is how can we formalize a decision-making process for EIPs? How can we create a formal decision making process for EIPs?

That's a bigger question, because decision-making comes on under governance. So we have to create some sort of formal governance structure for deciding what EIPs go through. Some sort of formal decision-making processes is one of the biggest needs found through the survey.

**Tim Beiko**
I think related to that, there's another conversation about the CoreDevs call and the value they have and potentially moving them asyncs. I feel like maybe there would be a way to kill two birds with one stone here. We already have a rough threshold of what it means for EIPs to be implemented, right? It's basically all the client implementers agree to them, and they don't see major objections. And I can imagine us doing that async.

As for the political piece, you're never going to make controversial EIPs uncontroversial, right? And I feel like if we moved things async where client developers just said, whether they're confident or not implementing this part of an upgrade, and you can leave it the client developers to decide whether or not they want to implement it, which seems to have worked okay so far with ProgPoW, I feel like you could probably move most of the process async and by not having the actual CoreDevs call where the decisions get made, you open it up to more people in the community to voice their concerns and be part of the conversation. This is obviously a pretty huge change, but I feel like it's the way we could kill these two birds with one stone. I'm curious what others think.

**Edson Ayllon**
One more thing about that. One of the individual feedbacks was making the EIP process, less reliant on live conversations.

**Tim Beiko**
Yeah, I 100% agree with that. For example, for our team at Pegasus, half the team is in Australia, so half the people who are actually CoreDevs have never been on a CoreDevs call because it's two in the morning for them, and we kind of lose their opinions on that. Nick Johnson's another good example. I think he's in New Zealand or something, and he doesn't show up, but he he would leave really valuable feedback async. So yeah, I think there's a lot of value there.

 **Hudson Jameson**
Yeah, I agree. I wrote a really, really, really rough draft of something a week ago that I just dropped off. It was called Ethereum constellations. And it was basically a series of chat rooms that were connected through Telegram, Discord, and Gitter, and they were per topic. And there would moderate to strict rules on what chat rooms could be created and what their purpose was. One of them was for deciding when hard forks would happen, like scheduling. And that would be completely separate from deciding what EIPs into. go a hard fork, which is completely separate from the sub topics on EFI EIPs. So, like, 1559 is EFI right now, so there would be a topic room on that, and then it would move through to the different rooms as it goes through.

**Tim Beiko**
Why not use something like EthMagicians, though? I'm a bit skeptical of chat for that, because it's just so hard to search and to record decisions.

**Artem Vorotnikov**
I have a suggestion here. You know the Rust language core development team that developed the Rust language? And they had this problem where they also have the old process called "request for comments," (RFCs.)

So basically before implementing a change in the language, it should first be adopted as what they call an RFC. And we call this an EIP in the Ethereum community. So basically they have GitHub as their primary communications platform on various RFCs,  and GitHub didn't really scale as far as I know. But what they did was they tried out Zulip, and Zulip helped them a lot. So I am also trying it out for participating in the Rust language development, and also we are piloting it for open Ethereum as an alternative to Discord.

So, basically, it allows you to manage your conversations much more smoothly than you can in Discord. And it's also very easy to search through various topics in the history as compared to Telegram or to Discord, especially Discord. So it seems a lot more organized.

**Tim Beiko**

I think there's maybe two different things here, right? One is the conversational day-to-day chat rooms. But I feel we probably also want something a bit more permanent. And that's why I like EthMagicians for that, because it's been there for a long time. And it's more of a long-form forum than chat. But because if we have to record - say there's a thread about an EIP and we have to record, you know, Open Ethereum status, Besu status, Geth status, Nethermind status,I feel like you want a permanent thread rather than a chat that people have to scroll up forever. I'm not strongly opinionated on the tool, but I think there's definitely a way we could do this async.

 **Hudson Jameson**
Yeah, Artem, how do you spell "Zulip?"

**Artem Vorotnikov**
Zulip. Z-U-L-I-P. Let me [write that down in chat.](zulipchat.com)

 **Hudson Jameson**
Yeah, I would be interested in looking at that tool for sure.

**Alita**
Have you all considered using Slack? I've had a good experience with it. It seemed to scale really well. It has 50,000 members, and it works perfectly.

 **Hudson Jameson**
Because it's closed source and costs money to store messages, that's kind of the deal breaker, because someone would have to pay for it.

**Artem Vorotnikov**
Zulip is actually slack on steroids in many respects. It looks very much like Slack, but it's open source, and more than that, it allows us to have more fluid threading [unclear - mortal?]. You have channels, but they can also easily be divided into sub streams. So basically, streams divided into topics. And you can search topics that are listed in the order of the history, and basically you can have multiple conversations in the same chat room, but which will be subdivided into topics which are also listed in history.

And if, for some reason, the conversation goes off topic, for example, you have a general dev chat room. Then you have a discussion about one EIP and then suddenly you start a chat about another EIP, then you can easily move that conversation about another EIP into its own separate topic, and it will easily be searchable. It's very easy to reach it, and it will not be lost.

**Alita**
That sounds very, very, very good.

**James Hancock**
A few thoughts on this. I've been seeing some of this stuff about separating and doing async and stuff, and what I've read it as is there is a movement that people would like to see the EIP standardization process be separate from the deployment on what is decided to go into a network upgrade. I wonder how much of the try to make an async process is really actually trying to make that happen, that separation happen. Like, the AllCoreDevs calls used for EIP standardization and then for something like EFI, but you have the actual coordination in decisions about what gets deployed being separate or at least done separately would still be good.

And having the calls, having a cadence of the client developers coming together is something I've seen as important, and cohesion among the clients about what actually is being developed. Without some way of all the clients coming together and regularly talking about it, I don't really see that asynchronously really happening very well.

It's already hard to keep everyone on the same page, and one kind of practical example for hard fork coordination or network upgrades, I actually have zero authority over any client team. I have no way of making any of them do anything. So a really useful thing that has happened on the AllCoreDev calls, and just to be really frank about it, is if we identify something publicly and if I ask what is the status of the implementation of this, and they know every two weeks they have to report on it, it's likely to get done. I could follow up all day and all night, but without that collective accountability, I don't see clients really moving together.

**Tim Beiko**
So I think there's two bits here, right? One is the implementation parts. I feel like you could get that mostly async, right? So say we have EIP 2315. There is an EthMagicians thread. If Besu hasn't begun our implementation, you can @ us on that thread, and we can comment. I think I agree that around the scheduling and whatnot, that's maybe harder to do, I think, but it feels like we could probably take most decisions async and get more input from the community and have the place where the decision is made be async and then use the calls as the kind of way to resolve these tricky issues that are just hard to resolve async.

And that's already kind of half of what happens, right? Half the conversation happens in the GitHub PR for the EIP, and the only part we're missing there is, like, four clients adding, like, a plus one that, okay, this should be accepted. And that doesn't seem that hard to do async. But I agree that the more fuzzy scheduling is hard.

**Edson Ayllon**
One comment on that. There has been a need expressed in the survey for clarity on where the EIP process ends and where the hard fork coordination begins. Or at least how those two are separate, clarifying that part.

**Pooja Ranjan**
I would agree to most of the part, with James as well as Tim. Right now, the process of EIP and the hard fork is not actually separated. In my opinion, the EthMagicians is a very good forum, we can go ahead and do that. In addition to James's idea of collecting information from individual clients, we can also start referring (EthMagician) to the point of discussion. And if we make it a preference of having EthMagicians instead of the PR, we would be having collective information in one place. And even if it is async, we're also getting a synced information during the AllCoreDev call.

So there is basically a fine line between the hard fork process and the EIP process itself. I tried to document that sometime back in one of the EIPs - it must have been moved somewhere else. But yeah, I find that this may be a good way forward in which people will be getting accurate information even about all the clients and where they stand at any point in time.

**Hudson Jameson**
Okay, so we've kind of agreed that the process of hard fork management and EIP development should be separate, or implementation should be separate, right?

**James Hancock**
The EIP standardization and the network upgrade deployment should be separate.

**Hudson Jameson**
OK, so we're all there. We're saying that there might need to be new tools in order to make that happen. We're also saying there might need to be, or that there is value in having some type of asynchronous coordination beyond the AllCoreDevs Gitter chat for people who are in different time zones, and that there might be tools we need to bring up to do that. I think I got that all right. Is there anything I got wrong?

**Pooja Ranjan**
Probably, we already have existing tools. We just need to enforce the acceptance and implementation of that. We have a discussion forum, the Eth Magicians. In my understanding, most of the EIPs are there, and they are referred to be as a point of discussion. But sometimes what happens, the discussion shifts to the pull request. And there we lost the track. So if we can make a standard process, a standard place, that this is it, and this is where you need to go, and we refer the link in AllCoreDev meetings, that might bring all the information to one place.

 **Hudson Jameson**
And that would be a change to EIP 1. Because in EIP 1, we say you should probably use EthMagicians. But you can use Reddit and Issues and other stuff.

**Pooja Ranjan**
Yeah, it's a kind of a recommendation, but I think to make it standardized, enforcement would be required.

 **Hudson Jameson**
Yeah, and I don't think that's a bad thing.

**jpitts**
Yeah, I agree with that. This is Jamie - I dropped in part way through the meeting, but, yeah, I think that's actually a really good idea. I've been thinking about that myself is to have a place that links to all kinds of different related discussions, but in a single URL. And it could be per EIP or per a meta EIP or hard fork EIP. I'm not sure where you would put such a URL or such a resource, but it's important, because there's even Gitter chat links. And you know, there's just so many places where decisions are being made or discussions are happening.

 **Hudson Jameson**
Yes.

**Pooja Ranjan**
It can be for EIPs in the beginning, because the meta EIP for an upgrade would be the next step. So we can start with going individual EIP-wise, and then we can also create a thread for Meta EIP - just a link, the discussion should be in one place with the EIPs only. That's my thought process.

**Edson Ayllon**
I had a question in general. Previously, we were talking about governance in the Telegram. And the consensus we got to was that thinking about an entire governance overhaul would be a process that might take a few years and require funding for research, I had an idea, probably creating the precedent for having an upgradable governance structure, so we can make changes now and then upgrade them later more formally through research and stuff like that. What do you guys think about that?

**Hudson Jameson**
Would that be in the form of an EIP, or would that just be something we do?

**Edson Ayllon**
So that would be in the form of an EIP. I guess it might be either information or meta. It just would be a proposal for a credible governance structure. Then we can extend that with how frequently should should the governance be reviewed to be upgraded. I was thinking a decay, so early on it would be more frequent and then later on it would be less frequent.

**Brent Allsop**
Did you say something about determining a president?

**Edson Ayllon**
No, precedent. Like an expectation.

**Brent Allsop**
Oh, precedent. Not liek President of the United States.
United States.

**Edson Ayllon**
No, no, "precedent," an expectation.

**Alita**
I wanted to say I might be kind unaware of a lot of this, but my take on it is that a lot of cryptocurrency stuff works on the idea of general sovereignty and decentralization. And I remember that we were talking before about the nodes, the node holders that may decline to make the final push and decide whether or not a change is made. Have you consider giving them more governance then say, the CoreDevs, that kind of thing?

 **Hudson Jameson**
We've talked about that before. That's a really good point to bring up, actually. So we've talked about that before, and from my recollection, the number one issue when I've had conversations with people about that is getting participation, and the fact that there are groups of enterprise node operators who have multiple nodes, maybe hundreds of nodes they run, and they can singlehandedly sway discussion or decisions.

**Alita**
That makes total sense. I really like the way the U.S. government is set up, in the sense that you have multiple different checks and balances. And then you have, for example, the node controllers. And then you have the CoreDevs that, say, have the opportunity to veto or something like that?

 **Hudson Jameson**
Yeah.

**jpitts**
The way I think about it is it's up to them to organize. And the people at the table now are the ones who are organized and engaged and interested enough to be a part of the governance process. And if a group wants to be a part of this system, they could come to the table, and I don't think there's anything stopping them. And when there's a problem, a group converges around it, like what happened with with the Cat Herders. There needed to be more management of the releases, and so they coalesced around it. They formed a group, and the same goes for if miners or node operators or any group out there wants to participate in the process, it's up to them to organize, and we would help them organize. I think all of us who are involved in the process would help them organize.

So rather than form a legal structure or any kind of ideal structure, let those parties be involved and encourage them to do so. And then, much like what's happening here, formalize it a little bit, but don't go formal first is basically what I'm saying. Just encourage people to organize if they want to have agency and be a part of the process.

**Edson Ayllon**
So I guess my suggestion was to say we're open to upgrading our governance structure, but not necessarily going into the entire overhaul right at once. I was thinking of maing small changes now and then making larger changes later on. What do you guys think?

**Hudson Jameson**
I have to think about it more.

**Alita**
So my take on the slow output is that that's definitely, in my opinion, a good idea. I think you would be good to always test things and also treat it like it's a financial transaction, maybe, in the sense that, like Hudson was saying, taht you can expect the worst and expect certain a node group to coalesce and take over, so going slowly would be beneficial. Because if the current system is stable, then you don't want to jeopardize that. That's my take on it. And then another thing I liked was the suggestion of the core governance structure as it exists right now, if it exists at all, unfortunately, I'm not too aware of it, but if it exists, then they help smaller groups coalesce as they want to get involved. That's a good idea.

**Edson Ayllon**
One thing that might also be helpful is to define what governance means. So the way I'm using it for what I'm saying is just decision making, just the formal way of how decisions are made. For us, it would be for a hard fork coordination.

**Artem Vorotnikov**
So if I may, this is a mostly relevant for the potentially contentious EIPs, as far as I understand, like ProgPoW. And so there's two things here. First is that many, most EIPs are purely technical and do not carry any social implications. So they're of little interest to most of the community for the most stakeholders, only to client developers. But then there are social, so tp speak EIPs like ProgPoW again, which are of interest to everyone. And second, I think that it's just important to get visibility to social EIPs, basically. And if we get enough visibility for them, then there will be no more divisions or no more scandals like ProgPoW. That's my take.

**Tim Beiko**
I agree with what you say about the bit that most EIPs are not that divisive. I think the challenge there, though, is you want the system to be set up in advance and to handle all of the non-controversial EIPs, so that when we have a controversial EIP, the system is already there. Because for ProgPoW, for example, if we introduce a new system now, people just won't think it's legitimate, because say we introduce a new system and the system results in ProgPoW going live on the network, everybody who's against ProgPow says it's a bad system and vice versa. If you introduce a new system and ProgPoW doesn't go live, everybody that's pro-ProgPoW says it's a bad system. So this is why I think it would be really valuable to come up with a more open system that works in these non-controversial cases that we can start using and get some some actual traction on. And then once the next controversial thing comes along, you already have that system in place, and you don't have to put it up as as you're dealing with the controversy.

**Alita**
I definitely agree with that. Just seconded.
**Artem Vorotnikov**


**jpitts**
That make a lot of sense, that approach. Be prepared for the for the crazy things by creating a process for the normal things.

**Hudson Jameson**
And it looks like we have 30 seconds left. So last thought.

**Artem Vorotnikov**
Visibility. Visibility is paramount here. We need to work on getting visibility to potentially controversial EIPs.

**James Hancock**
My read is the core problem is that the Ethereum community doesn't feel like they have a say what goes into Ethereum. And I think a lot of this trying to figure out different ways of doing governance is a long way of getting around to that, and smaller changes to do smaller things - we're a group of 10 people on a call right now trying to get governance buy-in for any governance changes is - we could do or we could write whatever we want right now. But then how in the world are we going to get the entire network to agree with it? And how are we even gonna know when the entire network agrees with it? But maybe I'm just a little more pessimistic than usual.

**jpitts**
It's always going to be rough. I think it's always going to be rough. If you watch British Parliament on YouTube, it's difficult to form a government or have governance. But I think overall, we should expect there to be conflict. And when there is, it's a natural thing. And we do our best to try to address it. And I think those structures are existing and what I said before, just slowly proceed with it.

**Alita**
So I have two things. Number one is that we should assume that every every sort of governance change will lead to a catastrophic failure. So you should only implement changes where catastrophic failure wouldn't destroy the network. For example, of somebody passing an EIP that devalued the entire currency and as far as I can tell, that is a feasible thing. Number two is I personally don't understand how people can say that you can have a governance structure of any kind to make changes to something, especially when it has to do with money, without politicizing it.  As I understand, Bitcoin, they just don't make changes.

**Hudson Jameson**
57:03
Yeah, Bitcoin's very stagnant. Yeah, we're a minute or two over, and I have to get on another oom call, which means I have to end this one for my account to do that. So sorry about that, everyone. And let's take this back to the Telegram chat and see you all in two weeks.

# Attendees

* Alita
* Artem Vorotnikov
* Brent Allsop
* Edson Ayllon
* Hudson Jameson (Host)
* James Hancock
* Jim Bennett
* jpitts
* Pooja Ranjan
* Tim Beiko


# Date for Next Meeting: 22 May 2020 at 1400 UTC.
