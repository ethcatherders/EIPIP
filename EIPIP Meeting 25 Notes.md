# EIPIP Meeting 25 Notes
## Meeting Date/Time: Wednesday 27 January at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/48)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=zz1IhYKztuc)
### Moderator: Pooja Ranjan
### Notes: Shane Lightowler

----
## DECISION ITEMS

**DECISION**: The new Cat Herders website should focus on being an index/intro rather than an in-depth content repository. It should point to canonical sources elsewhere (eg Eth1.0 specs repo, Ethereum.org) to avoid duplication [16:03](https://youtu.be/zz1IhYKztuc?t=963)

**Decision**: Consensus that offering a gitcoin bounty of 7000USD for 1 months work for a contractor to move the merge bot to GitHub actions is a good idea. This to be followed up on next Cat Herders call. [29:43](https://youtu.be/zz1IhYKztuc?t=1783)

## ACTION ITEMS

**ACTION**: Confirm with Sam @ ethereum.org whether the intention is to have ethereum.org point to the Eth1.0 specs repo, or vice versa. Where does the canonical content live? [6:14](https://youtu.be/zz1IhYKztuc?t=374)

**ACTION**: (mainly James) Work out what content we think we should be surfacing on the Eth1.0 spec repo and network upgrades content for Ethtereum.org, and then speak to Thomas and Sam for their views. [18:28](https://youtu.be/zz1IhYKztuc?t=1108)

**ACTION**: Cat Herders to consider EIP information for Ethereum.org site. [19:48](https://youtu.be/zz1IhYKztuc?t=1188)

**ACTION**: Brent to continue investigation into sources of EIPs information. [31:36](https://youtu.be/zz1IhYKztuc?t=1896)

**ACTION**: Cat Herders to progress EIP status cleanup. [34:12](https://youtu.be/zz1IhYKztuc?t=2051)

----

# 1. Discuss the content to populate the Eth1.0 spec repo with useful information on the Eth1.0 chain & the possibility of creating a bounty.


**Pooja** - Welcome to eipip meeting 25. The first item on the agenda is 'Discuss the content to populate the Eth1.0 spec repo with useful information on the Eth1 chain and the possibility of creating a bounty'. We discussed this in an earlier meeting. The Cat Herders were in touch with ethereum.org people and we were trying to support them with the network upgrade pages yesterday. Unfortunately he had a confict and could not join today. But he shared some thoughts around not duplicating effort - there are some things that are already available on the ehtereum.org website in addition to things that we are planning to put up on the Eth1.0 spec repo. We need to work out what things are missing (on the Eth1.0 spec repo) and what things we want to have. They would then be happy to point back to that repo.

**James** - Is that the ethereum.org team?

**Pooja** - Yes. This is Sam's comment in [the meeting agenda.](https://github.com/ethereum-cat-herders/EIPIP/issues/48#issuecomment-767968085) There are three sections we are talking about... One section is the Ethereum wiki which is not very well maintained. They are owning that and said that they would be taking json rpc from there and try to update the information to have it on ethereum.org. If we want that to be on Eth1.0 spec repo they are willing to help, so it's on us if we want that to happen. I believe in the earlier meeting we discussed that we would want to have some developers-related docs on Eth1.0 spec repo so that client development teams or any new person who would like to understand what the specs are for clients, they could find it here. So we want to have this as a canonical resource.

**Hudson** - I think for the json rpc spec specifically we need to have a conversation with Thomas from Nethermind, because i think, and maybe Micah saw this or Lightclient saw this in the eth R&D discord, maybe even someone else like James in the chat, I think they're doing a call on this every other week.

**Micah** - Yes, I just got out of that call.

**Hudson** - Oh cool. Do you think they would have an opinion on this?

**Micah** - Yes that's what they're planning. The goal of that group is, tentatively, this is the first meeting, it sounds like they want to clearly specify the json rpc standard across the clients and get them in sync basically. So that is a project that they are actively working towards. This is a brand new group so it's always an unknown how effective a good new group is going to be but that is at least their plan.

**Hudson** - Yeah, let's just ask them where they want it. I'm gonna guess they're gonna do github because then they can do pull requests more easily and the one point of specs repo just seems like a better place in my opinion but yeah let me see... adding a section and then linking to the one. Oh I see, so I think Sam is wanting to have a section on it like on the ethereum.org side, but that's not the canonical source necessarily - it links to github. Is that kind of what he's getting at?

**Pooja** - It's other way round. If we want to have the canonical source as the Eth1.0 spec repo we will have it but they will point it to...

[cuts out]

**Brent** - I missed most of that. Am i the only one that missed that? She broke up. 

**Hudson** - Yeah you broke up a little bit Pooja. If you could repeat the last part

**Pooja** - Okay is it better now i hope?

[muffled]

**Hudson** - Interesting okay. 

**James** - You mean that they'll point the etherum.org site to the specs repo?

**Hudson** -  The opposite, I think.

**James** - I couldn't understand that Pooja. I think your internet might be going slowly or something.

**Hudson** - Yeah i think what's happening is ethereum.org wants to host the spec and then they want our eth 1.0 specs... oh go ahead Pooja. i think we might have lost Pooja temporarily.

**James**  - the ether1.0 specs or if...

**Hudson** yes specs or the ethereum dot org 1.0 page

[unclear audio]

oh i like that idea.

**James** - Yeah all right. Yeah that'd be great there's a couple things that have floated around that are like this, like the jason rpc spec, like e365 I think we're on, or e67, like the networks specification, the yellow paper, some testing framework stuff which came up over the week, any kind of neutral inter-client communication standard would be nice to fit under there and we can get the right people to have permissions because it will be less political - they don't have to be eip editors to be able to work on the network spec or whatever because those people are usually kind of different.

**Hudson** - Okay I think that for the next piece we would have to list what we want on the Eth1.0 spec page that makes sense. The first step is to talk to Thomas about where they think they want it and if they think this is a good idea and then we'll give our opinion too and get back to Sam. I think this is the best way to move forward with this piece of the agenda for the json rpc spec.

Well that's good that they're willing to help and Pooja since your audio's cutting in and out I can take over the next part if you want

**Pooja** - Yes please 

**Hudson** - Sure okay, so the next one is network upgrade information from the comment, i think because we're doing all of these okay... Sam spoke with Pooja about this. It'd be great to collaborate to improve the ethereum.org history page with network upgrade information because there is pieces missing including a section that says where to look for the latest stuff on that and where to follow for updates. I can see the ethereum.org history page having a list of network upgrades and then also where the blog posts were combined with the blog post at ethereum.org and a chart and the block number and then a link to the eth 1.0 specs repo where we have retrospectives and stuff on it.

**James** - That sounds like a great hybrid, like what information goes where.

**Hudson** - Okay 

**Micah** - And then in there you said you included the list of eips included in each hardfork, is that correct?

**Hudson** - Yeah that would be that'd be another good thing to put in there. It'd be like a little chart or something

**Micah** - That's the number one thing that i think is missing 

**James** - And that part should be in the specs repo, i'd say, and then the website can have most of the rest of it

**Hudson** - Yeah the website can have a list of the eips once it's final but the Eth1.0 specs repo would be the canonical source and then ethereum.org would both point to it but have a list of the summary. That's like a trend I think we'll be seeing as long as Sam's okay with it. And then also spoke to Pooja about eip information so summaries, list of links, and discussion resources. So the page right now just goes over what an eip is how to participate, a history of eips, it has the list of vip editors and it's incredibly outdated, so the goal here would not to be replace that but merely supplement the material with resources from the community. As an example the content of ech curates on 1559 provides a large amount of additional context versus the eip itself. Okay so bringing resources like that together might make sense i'd have to think about this more.

**James**  - There has been a little bit of a gap of what to do with the articles that Tim Beiko has written basically, and micah as well, like some of the more 'why we're doing something' and less of the spec kind of idea.

**Micah**  - There's definitely a missing piece exactly as James just said where you've got the spec which is a technical specification. It's kind of motivational section but that's meant to be like a brief little thing just to get people in the mood. It's not meant to be an argumentative essay. It's not meant to be an opinion piece, it's the motivation section - like "hey here's some things that this would be useful for". Like here's a short list of uses or here's a few benefits we get when playing this. Meanwhile of course along with the EIP there's also the opinion pieces, there's the user stories, there's the essays, there's the analyses that are being done -  eip 1559 is a great example of this because we have a ton of this stuff and there's currently no place to put that right now. Tim just has a hack.md article or page that he's creating...

**Brent** - Did we lose Micah?

**Hudson** - Yes,we lost Micah. I think the summary of what Micah was saying... unless, Micah you back?

**Micah** - Where did I cut off there?

**Hudson** - You were talking about what was missing or the the fact that there were definitely some things that were missing and there were articles that were written that provided supplemental information that could need to go somewhere.

**Micah** - Yeah that's basically it. We've got eip 1559, a great example of this. We've got tons of supplemental information and nowhere to put it and so we can link people to it of course when we have a channel and we have people coming in and talking to it but there's no place that people can know to go to read more about any supplemental information about an eip because we want to keep that out of the eip itself because the eip is a technical document. But we don't have somewhere else to send the person to say "hey if you ever want to know more, like opinion stuff on an eip, go here."

**Hudson** - Ah okay 

**Pooja** - So that is the thing that we are proposing here. I'm gonna share the link in the chat - this is the place i mean. On the ethereum cat header website we are trying to curate a list of resources for any eip under discussion. For example right now we have three or four eips;  1559, 2938, evm384 and all that stuff, so whatever resources other than the eip at magicians forum, like blogs published by you and others, we curate it and keep it there. The idea here is that we can make it publicly available with the help of ethereum.org. They are thinking in this direction and looking for some thoughts like if this is something good that we should be doing.

**Hudson** - Moving the resources from cat herders website to ethereum.org makes sense to me because that consolidates information from one less source because no one really goes to our website. Or if they do they just want to know about the cat herders and if we start trying to make it an information hub that's gonna be like the seventh information hub. So although we should have something on our site about stuff like hard forks and where to find information, it should funnel to the eip's website or ethereum.org or the eth 1.0 specs repo in my opinion. So it's like an index more than a listing.

**Pooja** - Right, and the another benefit that we thought of, like in cat herders it is with us only if we update that is getting updated but if it is there on the ethereum.com, even if some educational resource is missing, people can simply create a pull request and add it over there.

**Hudson** - Yeah that sounds good to me.

**Micah** - Yeah that works for me. I didn't know about this page so i think this page basically is what i was looking for.

**Pooja** - Yeah i mean that's the thing we wanted to share here. It's like we are already doing this curation of resources but it's not publicly available so if ethereum.org either pointed towards us or maybe move this section entirely on that page would be readily available for people.

**Hudson** - Yeah I'm in favor of moving entirely to that page and having our site point to it but i want to hear other people's opinions too obviously.

**Micah** - What is our in that context

**Hudson** - Cat herders. The cat herders page.

**Pooja** - Okay, we will bring it into the cat herders meeting and then see but from this meeting I believe that people are being positive towards moving the entire thing to the ethereum.org site. That's all three points that we discussed yesterday and we wanted to mention it here.

**Hudson** - I'll be honest here, i'm having so many meetings this week i thought this was the cat herder meeting until like a minute ago.

[Laughter]

Anyways, I think we're done with that topic.

**Pooja** - Before we move on I just wanted to have some clarity on the next step like who, what, when kind of thing. As per my understanding, James is listing the resources that we would want to have on the Eth1.0 spec repo and then if people think that we should have a meeting with ethereum and with nethermind for the json rpc thing we can arrange for that or how do we want to proceed about it? In the next meeting we'll discuss this or we'll have a separate meeting for this particular topic. 

**Hudson** - My opinion is... for the json rpc let's try to keep that asynchronous and text based in the all core devs channel or with a private conversation with Thomas. Actually there's about to be a discord channel created for this rpc spec. It's going to be in the eth1 section of the ethernet discord, likely, and I'll be creating that in the next hour. So that'll be one of the first discussion topics in there and if we need a call we can have one but let's try to just talk it out in there first instance. What do people think of that?

**James** - I like it.

**Hudson** - Network upgrade information section - that's going to be a James thing mostly, so just coordinate with James. And then for eip information that'll be at the cat herders meeting.

**Pooja** - Cool

**James** - And as far as me writing up a list about what should and shouldn't be there, if i like this sort of organic, the stuff that should be there seems to be finding its way and not having to dictate it I think we'll end up making better participation from those involved. We want to bring stuff to the repository.

**Hudson** - I agree after the initial pulling of the data. I think we need to be dictatorly on the initial content that's on there and then afterwards have it be organic because otherwise people won't know a direction or examples.

**James** - Yeah that makes sense. We can do that.

**Pooja** And there was another sub part of this item... it was the possibility of creating bounty. I'm not sure if this is something that we will consider on later part when we get more clarity on how much effort has to be put on the advanced pack repo. Am I correct to think that?

**Hudson** - I think so.

**James** - Yeah. That's kind of revolving. I think it depends on what gets left out from these groups that are working on

stuff.

**Pooja** okay okay sounds good to me. 

# 2. Contracting out to someone to move the bot to GitHub actions

**Pooja** - The next item is contracting out to someone to move the bot to github actions. So it's a link. If you click the link it's coming up from the discord conversation a few meetings ago. We discussed looking into contracting out to someone to move the bot to github actions. But i'm not sure if some something happened or we had some decision on that. So on the request of micro comment uh i have added it to the agenda. Micah would you like to add things or change?

**Micah** - Sure just for anybody who's not aware we have an auto merge bot. It goes up and down, has bugs, needs fixes like any other piece of code. Nick was the original author of it and he's very busy with other things and doesn't work on the eip group really anymore. So it would be nice if we had a new owner. Nick said you know this should really be moved to github actions. I agree Github actions are the perfect place for it. Github actions did not exist when Nick wrote it back in the day so it's a new tool that we have that just makes this a lot easier for group maintenance because anyone who can see the repo can see the action and tune it and play with it. It's obvious to anyone who uses github. So generally a good thing to do. Contracting is one of those tasks that is really easy to outsource because it doesn't require really much knowledge of ethereum. You just say hey we've got this tool here, tuned in python. It's very short. We need someone who can convert it into a github action so that's why i thought that if there's something to outsource this would be a good thing to do.

**Hudson** - I think this is a good idea. I think that there's a bigger issue around funding that'll be a completely different topic in today's meeting, if we have time, or a different one. But I think this is an important enough change that we should ask the cat herders for funding for it now that their treasury has gotten bigger from the price increase, especially if we're going to be paying out an eth or something like that. But we'll have to talk to the rest of the cat herders about that so that should be on the agenda for their meeting and then if that is approved for funding from the cat herders we could do git coin. I'd prefer git coin but we don't have to use git coin for it necessarily.

**Micah** - Today i learned the cat herders have money!

**Hudson** - Cool 

**Pooja** - Yeah but I believe getting an estimate of what amount of funding or the effort that we are looking for here would help us. 

**Hudson**  - Yeah that would be helpful for a cat herders decision. Micah do you have any ideas or anybody else in the call?

**Micah** - Eestimating software is the hardest job in the world. So relative to building an ethereum client this is a trivial task. This is one of those things like it depends on the skill level you hire and whether the person already has at least some knowledge of how this works. If you were to hire lightclient or me it would be an easier job than if you've hired some stranger but i think lightclient and me both are going to be more expensive and have little time available. If anyone wants to interrupt me please do. 

**James** - Do you a rough sense of how many days that would be?

**Micah** - So for me i've used github actions all of one time and i used an off-the-shelf action. It took me a few hours to figure out how to use github actions, how to make the off-the-shelf action work which was like pick from a marketplace, fill in my things, then a couple hours to fix it, because it didn't work on the first try of course. This would be a more complex github action in that it's got custom code but i think github actions can run basically any language so you can run python, you can run javascript, whatever. And so whoever you hire would presumably work in a language they're familiar with and so if they already know github actions and they already know their language I want to say days to mvp, and then another week or two for testing, but this is really off the cuff.

**Hudson** - Yeah I would say if someone really knows python and github actions and they decide to take this i think a week for all of it sounds more accurate if you really know your stuff.

**Micah** - Use Hudson's prediction. Come on, it will help you to be held accountable.

**James** - It would be nice if there is some expectation of maintenance for maybe at least a couple weeks, so when someone finds something a week later we have someone to talk to but that wouldn't be a lot of time. It would just be like hey...

**Micah** - Yeah a little bit of  on-call after the fact, a number of hours of on-call support? Ideally the longer term the better i think because it's like for example we just ran into a bug with the most recent failure of the bot was we added the review status a while ago and for the first time someone tried to submit a pr against their own review... their own eip that was in review, and that's like a month or two later and the bot just broke. Like it just choked on that entirely. And so ideally we'd have someone that we can call up on a retainer or whatever that means where you say hey there's a bug, you're looking for some more work? That being said once in github actions i think it'll be easier for us to swap out people to work on it so if they're not available we can find someone else.

**Hudson** - The average developer salary according to the first post in google for a python developer is $110,000 per year. Therefore if we were to take math and do math then that's hard... we would do a hundred ten thousand dollars per year, divided by twelve, divided by 53 dollars an hour. 53... 57 i think i did salary divided by 12, divided by four, divided by...

**Micah** - Oh that's because you're not four weeks a month. Yeah if you do divide by 2080 that gives you hourly rate from annual, so it's about 53.

**Hudson** - Okay, 53 an hour. So it's 53 an hour and let's say we do... we can be a little liberal with this and say two weeks of work. So we can get the hourly rate first. That's like a good starting thing so 57 an hour. And then we could say two weeks of work to implement and write documentation for it and then one week of service with the idea that we can also hire them again for more larger changes.

**Micah** - It sounds like as good of an estimate of their software project as any.

**Hudson** - So two weeks is four five eight three so that would mean one week is... wait i did divide it by one that's not a thing... two two two nine one. So all together that would be let's say seven thousand dollars to round up but it's six thousand eight hundred seventy four.

**Pooja** - Something between six to ten k would be an ideal one if you want to go ahead this thing but it would be my personal preference for people who are already involved here should go ahead with that but what do people think? Should we proceed with some kind of gitcoin bounty or try to reach out to people who are already engaged here?

**Hudson** - I like the idea of setting a precedent for a gitcoin bounty because that could attract more people to both eip stuff, cat herders, ethereum in general. I always like the idea of bringing brand new people in especially if we're charging this much for someone that's more python than ethereum.

**James** - You're likely to get something pretty good because i doubt it will be full-time every day that they have to do all of this.

**Hudson** - Yeah we would give them like a month to do it or something weird like that.

**James** - That would be that would be pretty reasonable then.

**Hudson** - Yeah. This also is me trying to fund eip things for the future from different organizations. If we can set a precedent we might make another gnosis safe for a community fund for eip editors and for eip related tasks. We can say we've already done this once and it worked.

**Pooja** - Yeah that sounds good. Okay then i will bring it up in the cat herders meeting and we'll see how much progress we make over there and then bring back the decision to the next eip meeting.

**Hudson** - I'm going to put the salary estimates as a comment on today's meeting.

**Pooja** - Sure i like that.

# 3. Single source of truth for EIPs

**Pooja** - Okay moving on, the next item on the agenda is a single source of truth for eips. I guess Brent is working on that?

**Brent** - I haven't had a lot of time to work on this yet and i think i've been trying to educate myself around what all the sources of information are and i think i'm getting out of hand and getting lost. So i think the first task i'm going to focus on doing is just that there's two sources of truth evidently. There's the eip.ethereum.org and there's also ethereum.org/eip. The latter is only referenced by a few people on the internet, whereas the former seems to be by far what everyone points to. So i'm just going to focus on getting the ethereum.org eips... to get that to redirect to the eip.etherium.org and just focus on that task. Does anyone else have any other thoughts on that?

**Pooja** - I think that is the current situation with ethereum.org/eips that it is just an overview page and it actually points towards the eips.ethereum.com?

**Brent** - Okay i'll look into that some more. I gotta find some more time to work on some of this stuff so still working on it.

# 4. EIP status change (update)

**Pooja** - Okay, so moving on the next item is eip status change update. The cat herders have been working with eip authors for the proposals which are in a draft status or maybe not in the correct status even if it is in like in review. In the last call it is more than a month or so so we are trying to reach out to those authors and asking them to change their status. So we made some progress i think. At least three of the eips we closed last week. By close i mean that it wasn't draft status, now they are in review. For berlin eip i think there are three eips which are still in draft and that they that they need to move into review status. If there is no change done by the author this week  we will be creating a pull request to change it to review. The eips are eip2718 eip2929 and eip2315. All these three are in draft so we would like to have that in review.

Other than that with the help of p penny series we interacted with quite a few authors and we suggested them to make a request to move on their eip from draft to review but there are quite a few which haven't created any pull requeste yet. If they are not done by the end of next week cat headers will be reaching out to them and try to create a pull request to change the status.

**Micah** - I'm excited for the cleanup.

**Pooja** - Yeah thank you Micah. I have seen that you have already closed this thing so yes i'm happy to contribute here. I'm also looking forward to it. Many eips are still draft status - when i look at it i still get confused why they are there even if they are not active for over two years.

# 5. Review action items from the previous meeting

**Pooja** - Okay moving on to the last item. That is review action items from the previous meeting. There is one decision and two action items that removed linked eips on eip1 that are dead. I have already created a pull request to remove the eips which are not active right now. They were just from the pull request they never made it to the eips.ethereum.org and the pull request number is 3218. So Micah, lightclient, Hudson, all editors, if they would want to give it a look and yes we can close that if that is if there's nothing wrong with it.

And then next two action items where James is collecting ideas for a single source of truth which he will report on in the next meeting and James would be working on hard fork information into at the 1.0 spec repo so i think James would be working on this.

**James** - Where you have the berlin specification on the website there, the previous hard forks are not there yet. I think we have a pretty good list now of stuff that we're thinking about adding to the repo so i'm pretty happy with where that's progressing.

# 6. Edson to work on EIP editor roles, responsibilities blog

**Pooja** - Yeah that's really good. The next one is Edson to work on the eip editor's rules and responsibilities block. I thought i saw edson today in the meeting?

**Edson** - Yeah i'm here. I actually forgot about this item. I'll try to get it done this week.

**Pooja** - Sure no problem so that's all from the agenda that were added here if people have any more topics?

# 7. Anything else

**Hudson** - I added an item, sorry to interrupt. Funding for eip editors etc... I'm starting to have more of an idea of how to do this. Based on other models we have a few different options. I think as everyone's seen opengrants.io, i'm posting the link here... wait a second, no never mind. Ignore that link, it's the continuous grants thing that eth2 uses. Do you know what i'm talking about?

**Micah** - Quadratic funding?

**Hudson** - Yes but there's a specific page that uses it. Dang it, why can't i remember it? All right, either way, it's a website - i'll have to find it later - where everybody pools their ether together into a contract that over time gives out ether to a set of participants in a multi-sig based on milestones. So my thinking is we could have one for eip editors, there's one for eth2 developers, we could have one for eip editors, and then people can contribute to that. So that would be a cool thing for organizations to show their support. Could we put their logo on the eip repo or is that corporate sponsorship bs?

**Micah** - I don't have preference on the logo side of things. What would be the milestones you had in mind?

**Hudson** - Oh, it wouldn't be that complicated. It would just be like being an active eip editor based on consensus among x number of people or something. I don't know, i'd have to think more about what the milestones would be but it wouldn't be anything like x number of pull requests handled or anything like that. That would take someone an extended amount of time to actually calculate because we don't need to waste time. It might just be having people decide who deserves the money by consensus or something or voting.

**James** - It's still not really clear who gets to choose, who gets to be eip editors, or who would not get funding. We'd have to just figure that out. It's gonna take some time.

**Hudson** - Yeah this would be a longer process and it would be cleaning up the eip editors who are currently on there. Kicking people off who aren't active would be step number two. And then if we decide to go that route it might be complicated to use a brand new thing like that. And then we can go the traditional gnosis safe with companies who have a voice in deciding where their money goes. Or they can delegate to the eip editors themselves who have to pick among themselves and have a third neutral party like the cat herders, if we can call that a neutral party.

**James** - That's some kind of mechanism for keeping it from being like a lobbying organization we've kind of avoided because no one gets paid for anything.

**Micah** - Yeah that's the ultimate solution. The ultimate solution if there's some money to be made no one will show up.

**Hudson** - Yeah so there would have to be a weird a thing on like if someone's giving money, you can't prioritize their eips, or something like that. 

**James** - This some kind of guard mechanism or checking and balancing mechanism, which is good to build into thinking about it.

**Hudson** - Today's kind of the kernel of the idea because i've thrown around the idea of funding a few meetings and i want to get moving on it. So i'm actually officially putting it on my to-do list for eip funding strategy.

**Micah** - It's a really good idea. You guys can have this so each editor will state the projects they're passionate about and they're only allowed to be sponsored by people who hate those projects so there's no conflict of interest so i can only be sponsored by miners.

[Laughter]

**Hudson** - It's reverse conflict of interest, yeah.

**Micah** - That's right.

**Hudson** - We're making a new term. We're groundbreaking again. I'll think on this more and if you're interested i'll probably move the discussion to eip editing and the discord.

**Pooja** - Sounds good.

**Hudson** - And that's it for my item.

**Pooja** - We are making quite good progress. So we have been discussing about this eip editors funding for a while and now that we have some clarity on how we should proceed, i'm excited for it.

**Hudson** - Awesome.

**Pooja** - That concludes all the items listed for today. If anyone has anything else to bring up we have some time? If not thank you all for joining us today. The next meeting is in two weeks from now - that's on February 10 at 15:00 utc. Thank you everyone for joining.


# Attendees

* Pooja Ranjan
* Hudson Jameson
* Brent Allsop
* James Hancock
* Micah Zoltu

# Date for Next Meeting: February 10th at 1500 UTC