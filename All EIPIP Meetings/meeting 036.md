# EIPIP Meeting 36 Notes
### Meeting Date/Time: Wednesday 2021/06/30 at 15:00 UTC
### Meeting Duration: 50 mins
### [GitHub Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/75)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=wt7EB8MujgA&ab_channel=EthereumCatHerders)
### Moderator: Pooja Ranjan
### Notes: David Schirmer
## Action items
| Action Item | Description | Video ref |
| ------------- | ----------- | --------- |
| **1**   | Evolving EIP process | [0:15](https://youtu.be/wt7EB8MujgA?t=21) |
| **2**   | New EIP/ERC editors | [31:49](https://youtu.be/wt7EB8MujgA?t=1909) |
| **3**   | JSON RPC API update | [36:18](https://youtu.be/wt7EB8MujgA?t=2178) |
| **4**   | Canonical source for EIP | [33:59](https://youtu.be/ZSMrxG1LAck?t=2039) |
| **5**   | Review action items | [44:32](https://youtu.be/wt7EB8MujgA?t=2672) |
## Decisions Made
| Decision Item | Decision Made |
| ------------- | ------------|
| **1**   | TBD, more time is needed to find a solution  |     
| **2**   | Short video will be made showing the basics of editing |  
| **3**   | Coding finished, formatting meeting will be held at a later date. |  
| **4**   | Not finished, need more time. |  
| **5**   | Time limitation will outsource to community for issues. | 

## Meeting Notes
**Pooja Ranjan**( Evolving EIP process)
All right welcome to eipip meeting 36. I have shared the agenda in the chat and the first item on the agenda is evolving EIP process so we have been discussing this from the past few meetings and I wanted to bring it up to this meeting particularly as an agenda item so we can discuss how we are looking into the changes that can be expected with the merge and like future upgrades so yeah I like that if you would like to go ahead and share your thoughts on it.

**Lightclient**
 sure so we originally like got this idea from kind of how ETH 2 has been handling discussing core changes and it feels like the way you know the way they do it they're able to kind of create just a diff against their specs since they have this executable pi spec it's easy to write some code that actually implements a feature that's being discussed and then people can focus on discussing like the actual mechanics of that whereas for ETH 1 right now if we want to propose a core change we need to write a full eip and that eip almost always has to redefine a lot of things in the system just to build the scene and be a complete spec i think 1559 is a good example of something that basically implements not in working ethereum clients just to show the things that it's trying to change and that's kind of like where our motivation came from just seeing how things are not working as well for ETH one and how they've been successful in ETH 2 so we've been working on this pi spec for about a month now and the goal of that is to be a complete implementation of ethereum in python and be of a format that's very readable very modifiable something that's not doesn't require a lot you know over engineering it's not very pythonic it's just focused on being incredibly clear and concise. It's not really clear to us how to go from having that spec to like enforcing it as this thing that drives forward core changes so I’m curious if what if people have thoughts around that I don't think that eips or like the concept of them will go away because I think that there is a lot of value in a lot of the pros that goes into an eip just defining like why do we want to make this change what's the rationale for these things to me this is you know really replacing the specification part because to me the specification part is where we're creating like a lot of duplication. If anyone has thoughts on paths to requiring eips have diffs against this spec be curious

**Micah Zoltu**
 My personal preference for those that are new or just tuning in for the first time I'll repeat it my personal impressions is that we just have PRs against the spec and those PR's would include the motivation rationale stuff like that I know a lot of people disagree with me on this I believe that motivation rationale etc is transient for lack of a better word like it does it's not something that needs to survive forever like we don't need to you know have a permanent record of why it was decided that we added chain id to specification four years ago or whatever it was that being said I have no problem with storing that information somewhere but I don't think it needs to be like in version control i think it's fine if that's just like on a doc site or inside a hackmd article or in a blog or something like that like I feel like we're in a youtube video where a peep and eip type video or someone talks about it like i think those are all very reasonable places to store motivation and reasoning for things I think the spec is the piece that must be stored in version control system and have history and like be easy to diff be easy to see the change set stuff like. So I’d my preference just to put all the other stuff that's not the spec itself into the PR and then it's okay if that kind of goes away over time.

**LightClient**
 I think like one interesting model that we could learn from is how rust does rfcs against the language they seem to be similar to EIPs in a lot of ways they have these things like summary and motivation and talk a little bit about how did they come up with this idea and then they link to github PRs and issues the top that either like implement these or places that a lot of discussion happens on those so I you know i tend to agree that i don't think EIPs necessarily like the text around it or things that have to be version controlled and live forever but i do appreciate the ease at which you can find the stuff like i'm curious about some certain feature and rust it's really simple for me to pull up the rfc and then I can immediately just read like a brief summary and these are things that are like kind of informal they're no really long things they're generally just really quick summaries and like motivating reasonings and then it links out to these places these github places where I can see okay here's where like a lot of discussion happened these are kind of the entry points and so that might be an interesting way i think it like kind of removes it avoids fully removing this idea of eips like i'm not sure how a lot of people feel about that i'm afraid that a lot of people will say oh well we like eips that's what ethereum is and here at least we get to keep those exactly what they'll say yeah so yeah I’d be curious to unfortunately the problem is it's just a different format than we have eips already like it's a little more informal it really just focus on linking to these github things and so anytime we make a big change to the eips repo it's not clear how to retroactively apply stuff or if they should be retroactively applied at all.

**Pooja**
so on the um thought of removing the idea of eip like completely I mean maybe I am in the camp that I would say that let it be there for some more time it's really helpful for new people like I’ll consider myself to be relatively very new who is trying to understand the process and read about these proposals while doing my research like earlier when I learned about eips and proposals there were different categories I got it from eip1 and started reading about it doing my research but while my research I came to know that there was eip4 which was actually superseded by eip1 and there we get all these types and categories so if we find the history that would help us connect the dot so maybe we can keep the history but the template how we store it could be different maybe in the if we say for example if we want to keep it in hackmd let it be like it's dot md file is also
not bad maybe we can change the template of eips and move the technical part directly as a pull request and keep the other content relevant or the text part in this hackmd or maybe dotmd file that could be something that we can think of.
 
**Micah**
 another idea if we want to do a slow transition like we don't want to just go all in we could just keep the eips as they are and just change so that the specification section now just needs to link to a PR against the specs repo and that's it and anything else in specification section is invalid and that's just the entire specification section everything else stays the same that would be a very easy transition it would vary I don't think anyone really disagrees with that strongly it's nice and simple and makes sure that we’re getting keeping the specs repo up to date and it gets people used to doing stuff to the specs repo but It's uh non-contentious I’m not a huge fan of it just because I would like to do a bigger change but I understand the value in taking the wins we can get and that might be the only one we can get.
 
**Brent Allsop**
 Yeah, Micah mentioned that that takes away the contention but that just pushes it over to whoever accepts that pull request into the spec right?
 
**Micah**
 sorry I meant it takes away the contention about changing the eip process is all like it's a small change to the process itself which is unlikely to get a lot of negative pushback whereas if we try to do what I would like I suspect like matt indicated everybody's gonna disagree with it and we might gain nothing by trying to do too much of once.
 
**Pooja**
 That's right uh yeah I mean I am in very much agreement with Micah’s proposal about uh having the spec section submitted as a pull request and that's how we make changes so like this idea looks good to me but yeah obviously I’ll be curious to know what other people think.
 
**Brent**
 So that would be a pull request against a python a spec running python spec which doesn't exist that would depend on that existing right is that what you're talking about?
 
**Pooja**
 Yeah lightclient is already working on that right now and I have shared the full request that is submitted to eth1.ospec repository. So there was this another idea of like when we are talking about network upgrade and network upgrade process there was another thought around the kind of for differentiating the category of the proposals right so there are proposals for protocol changes and there are some for future changes is there any particular thought on like how to deal with that because it was brought into attention like it sometimes it takes time for any change that is dependent upon an upgrade to come and include that improvement proposal and by the time we are on the upgrade that proposal may have been superseded by something else or may not be valid or something else came up so is there a way we can deal with this kind of situation what do people think generally?
 
**Lightclient**
 Are you referring to the debate on eip 3074?
 
**Pooja**
 Yeah and accountability yeah?
 
**Lightclient**
I mean i still like very much in the camp that there just needs to be a little bit more leadership in at the core layer in terms of i know that's crazy thing to say but and i'm not asking for like a dictator or something to say this is what ethereum is because i say it is i'm just i think that there are already like informal leaders who have ideas of things that you know we should be doing and working for i think like Vitalik is a has been a great leader of Ethereum he generally has a list of things that he thinks is important for the protocol to do and we kind of like see those things manifest as time goes on like we are seeing him talk about these things like extending the address space to 32 bytes state expert these are all things that are kind of on his list and i think it would be would be good if we had people a working group who spent time and tried to build out saying this is like kind of informal path for ethereum and here is like how we kind of like want this road map to happen because otherwise you end up with teams like quilt working on this idea eip3074 which is a very useful change to make to protocol right now and then we i don't want to say blindsided but we didn't really take into account these
things that were like theoretically on the roadmap five to ten years in the future like quantum resistance and fully removing eoa’s and so now we're kind of in this deadlock where until someone actually does some research and thinks about well how can we move away from eoa’s and actually have smart contracts in the protocol may be how could we move away from this sec p256k1 curve there's nothing that we can really do because people can always just kind of like sit back and say oh there's these changes in the future that may not be compatible so i think that if we had a little bit more leadership and have a little bit more responsibility delegated to people for like certain areas as in you know you are kind of the people who are in charge of looking into these types of things improving the UX of Ethereum improving state of Ethereum and we like informally have a lot of this stuff but nothing is defined there's no there's zero structure around these things.
 
**Pooja**
 yeah I think that is what what we can do as a group here in this eipip meeting like can define a structure I was looking into like older proposals and I found that the abstraction of transaction that was originally you know written by Vitalik that is also still in draft status right now so there are these are important proposals these are good proposals but they get lost maybe because we do not have a process defined for how to deal with these kinds of proposals similar similar thing was also there for some of the networking layer proposals, proposals are implemented they are being you know deployed in a client and they are being used but they are still in like older status I mean maybe because of author forgot to create a pull request but I believe sometimes it is included in upgrade and sometimes it is not so that's a lot of confusion around these proposals that's fine but as a group I’m thinking if we can do something about it or maybe can define because we have like great minds here all the eip editors and people who are actually involved into processes are here so can we think of something.
 
**Micah**
 It's a very hard problem this has been solved in traditional business but the way it's solved is a way that kind of goes against the spirit of ethereum which is why that same solution doesn't work um like you know traditional company you would just have..
 
 
**Brent**
When you say it solved in business you mean hierarchical business the guy at the top makes a decision and everyone goes in line?
 
 
**Micah**
Right yes like in a very simplified version usually there's a lot more delegation involved so you have someone at the top who is doing very broad strokes directions yeah it's definitely hierarchical.
 
**Brent**
 and then you know there's disagreement people go to the next level and the next level solves the disagreement?
 
**Micah**
Yeah so if you get into a deadlock specifically you can escalate up and have somebody call and even if that person doesn't have actual authority like the structure is flat just having a tiebreaker like having someone who just makes a call often is very valuable doesn't even matter what the call is more often than not like you just have a business decision that needs to be made it doesn't actually matter what's decision is made it just a decision needs to be made and Ethereum struggles with making decisions we saw this with product proof of work it's like the canonical example of not being able to make a decision and resulting in massive amounts of
engineering waste because just because we couldn't actually decide on what to do whereas in a traditional company you know you'd have someone would have made a call like you know long before you spend thousands of engineering hours on both sides someone would have just been like we're doing this or we're not doing this that's it doesn't even matter like again it doesn't actually matter whether you do it or not what matters is that a decision is made that is more important so I think the to cut myself off I think the solution
we need is a way to make decisions on contentious topics that isn't just like do nothing, like do nothing is currently the strategy for resolving contention.
 
**Brent**
 so if you had a petition system say we want to let's pick something controversial like recover some funds hundreds of millions of dollars of funds lost in the wallet and you build up a petition that describes the change that's going to happen and then you start getting people signing Vitalik says yes I support this and other people start supporting that and then we have diff, of course, a ton of people that dislike that and so they create a competing camp and people also sign and support and but anyway the bottom line you guys recognize I’m just talking about.
 
**Micah**
We tried this before in the past with like the dow fork for example people tried all sorts of polls and
just like sentiment analysis.
 
**Brent**
 the poll is completely opposite of what canonizer all a poll does is measure disagreement and canonizer is completely different than that. 
 
**Micah**
so yeah so yes so the issue often is that we get into a stalemate where everybody knows what everybody else's position is like at least within the courthouse like there's definitely within the community there is lots of misinformation and lots of uncertainty and lots of understanding within the core devs at least we can usually get to a place where everybody understands everybody else's position there's just like there's some core premise that people just fundamentally agree on like some like kind of root belief system sometimes it's a belief system sometimes it's just like a disagreement in style like just I was raised this way and this was more comfortable for me versus I was raised this way and this is more comfortable for me and those are the ones that I think we really struggle with is when it's not that we don't understand each other's positions it's that we find where we disagree and then we just get stuck and we don't have like both sides and I say this all the time in the coredevs call where both sides recognize each other's position and it's just someone just needs to make a call like that’s all like there's no like we caneventually get to that under point of understanding we just can't actually get past it.
 
**Brent**
Right but there's no formal way to track both sides claim there are so many people that are good gonna do this we're gonna fork but that's obvious they have no clue how many people are really on that side oh yeah so rigorous measure of and you can never track all that needs to be seriously measured so if you can see that 75 of all of the core devs and everyone are clearly on board and the noisy people that are against it and saying there's going to be a fork if you can see that then making those decisions become it can become a decision if you see 75 percent people are on board and 25 percent people aren't versus everyone just polarizing says there's going to be a fork and yelling and there's going to be four can you do this.
 
**Micah**
I don't think the core devs actually listen that much to people who yell and scream fork I think there are a few core devs who do but the impression I get is that most of them are pretty ambivalent like most of them seem to be in the general camp of forks are an acceptable form of governance if two groups disagree strongly enough forking is the appropriate way to deal with that situation and that's okay there's definitely people in the community that disagree very strongly with this like they do not think fortunately.
 
**Brent**
Yeah we'll never accomplish anything for constantly forking into smaller fiefdoms.
 
**Micah**
Yeah so i think the idea the idea is is that in most cases people aren't willing to fork over a thing like you have to be pretty big and significant like the dao was an example of a significant enough disagreement that caused an actual fork for pretty much everything else it's not enough to fork over like Prague pow as an again as an example I don't think whichever way it went we people would have actually forked over it like I think people complained and claimed they would but I think in the end like as we saw at least with the way it went people didn't fork despite threatening to and vice versa I think if we would have implemented it I don't think it would have actually forked.
 
**William Schwab**
Prague brings in an interesting mechanic also because contentious forks that involve something that's perceived as an economic blow to miners further incentivizes a fork so even if the community at large might not support it the mining community might I wouldn't say arbitrarily but I would say uh our I would say the mining community is capable of making a decision that's largely independent of the rest of the ecosystem sentiment if they feel like they're defending their own that their own holdings so I know and Prague gets a bit funny that way I’m trying to predict exactly what would have happened uh but I  do agree with all of your points there.
 
**Micah**
 when I say fork I specifically mean a fork where there are actual users on both sides of the chain a fork where it's just a bunch of miners who just go off and do their own thing and no one actually uses it that happens every single time we have okay every hard fork there are miners who forget to upgrade and they just keep mining the old chain for quite a while sometimes um like that is very normal and what specifically a contentious fork I think of like etc is the only one that Ethereums have i understand you actually have a significant user base that exits with I’m not just you know miners trying to sell their tokens or whatever.
 
**William**
Yeah  i understand.
 
**Pooja**
So that also brings me to a point where I wanted to bring it up about the fork identifier right that is this proposal is a network layer proposal and I know that is already implemented in geth so someone please help me understand that so  I have not a complete understanding of it is if it is implemented in all the clients or just get only I know for sure that is there in the geth but is it helping miners like getting on the right chain if that is included with the latest version of geth when it is ready for any network upgrade?
 
**Micah**
which do you have a link to what you're referring to?
 
**Pooja**
 yeah I’m just gonna share them here it's eip2124 and I’m sure so uh the proposal is in the last call we had invited the author to explain about the proposal and there is a very good video on peep and eip about this proposal explaining how it is going to help identify the right chain because they don't have just chain id they also provide an identifier for every upgrade so that may be very helpful for miners to you know to find the correct one.
 
**Micah**
 oh yeah I see uh no so this wouldn't help with miners forking off during every hard fork this is basically just to the way the gossip network works you basically just kind of broadcast out and talk to everybody and you try to find people that are on the same chain as you, it would be I think if I understand it correctly they're basically just trying to make it so you can segregate and so when you open up a channel to talk to somebody you can very quickly identify oh you're not the person I’m interested in talking to I want to talk to because I’m you know following this other fork than you are so that way if something like ETH BTH happens um you don't have people you know still gossiping with each other it's just basically it's a network bandwidth saving thing more or less performance improvement I don't think it'll have any visible effect on the ecosystem if I’m understanding it correctly also this simple summary is too long.
 
**Pooja**
so yeah I was wondering like if there is any such proposal which are there for improvement of network layer they are generally I have not seen most of them in upgrades I was going through the history of upgrades and looking into the Proposals I found one I think there was one eip8 that was accepted in homestead but other
than that no other proposals are there okay if I followed all of them then.
 
 
**Micah**
so I think there's two reasons for that one network changes are actually pretty rare we don't change the network protocol very often and two they can kind of have because they're versions and you could the clients can be on different versions it's not actually critically necessary for everybody to like come to agreement like it is for core eips and so like usually it's Felix and the geth team who you know talks about something they propose an eip and then you'll see they actually are a handful of network eips it's just like because they don't need to go to final they usually just get forgotten once they get close and so I suspect a number of these are actually maybe not maybe these are all really new.
 
**Pooja**
Yeah I mean like it would be good to have them as finals as well like I know there are quite a few version of Eip 64 then we went to 65 and at present, we are at 66. so we have differences we know that one is superseded by the other right so I think sorting them out would be no I wouldn't say superseded like you you can have a client that speaks only 64. Talk to a client speak 64 and 65 geth i believe is actually going to
drop 63 and lower soon and then they won't be able to talk to people who are not on 64 or higher if they remember correctly so yeah so we definitely should get eip 64 needs 65 out of draft like they should be final I
Think because I think they're in production now.
 
**Pooja**
Right and same for 66 that is there in the review for a while.
 
**Micah**
I don't know does anyone know 66 has been deployed?
 
**Lightclient**
 I'm pretty sure yeah.
 
**Trenton Van Epps**
I'm pretty sure geth has it released and there's slowly deprecating uh 64 and 65. all right they've announced sometime this year when they're going to stop supporting it or removing it.
 
**Micah**
Oh is it 64 or 65 they're dropping? So we should definitely get all those merged and moved up talk to Felix is probably the best person to talk to they definitely understand the protocol and like if you wanted to just rope someone in and say hey can just here's a list of Eips can you tell me which of these should we move to final Felix is probably the one to be able to answer that easily.
 
**Pooja**
 yeah right I will reach out to him this week and we'll create pull requests for at least which are in like draft and they need to be moved but for the review one, I will request the author to move it. all right so the bottom line is like I was just trying to understand for these proposals like there are three questions three open questions as per my understanding like one um are we planning to have like code proposals going the same way as it is going for now for the network upgrade irrespective of if it is a protocol change or a feature change let's come with the same process and the next one was for net network upgrade proposals network layer proposals can we do anything about it or it's just that we will be reaching out to author because these are not very frequent we shouldn't be worried or bothered much about it?
 
**Micah**
I’m fine with the network just following this same process as core I think it's just a matter of
they're just infrequent and so that and they don't need to follow the process like there's nothing forcing them to
like with all core devs and so I think it's just a matter of you know just we need to be proactive.
 
**Pooja**
and their inclusion in any upgrade does it have any significance should we or
should we not?
 
**Micah**
 they're disassociated with hard forks so they can be released by clients independent of any sort of hard fork so we don't need to track it for hard fork coordination or anything.
 
**Pooja**
Right yeah i just found only one network layer proposal which went into the first upgrade I believe and after that it was never there cool i'll make a note of that thank you. 
 
**Micah**
 I think that one is actually you're talking about ep8 right. I think it was needed before homestead so I don't think it was actually included with homestead it was just every client needs to implement this before homestead goes live.
 
**Pooja**
 I know I think I saw it in the list of Proposals.
 
**Micah**
 did it actually you know did it actually go live with homestead it is there in the meta eip for Homestead okay that was before my time so I’ll take your word.
 
**Pooja**(new eip editors-31:48)
For it all right I think this topic might need more discussion so we'll get back on this maybe in the next meeting we'll have some more thoughts around it and try to document whatever we have discussed in this meeting and we'll take it from there any question or last comment before we move on to the next item okay uh moving on the next item. is a new eip erc editors in training progress um I know we have William here on the call and there was some discussion in the discord channel as well anyone would like to give any update on how we are doing on it or like is there any challenge people are facing that might need attention?
 
**William**
my largest issue is the lack of more hours in the day currently if we could hard fork today and increase the hours all right that being said I guess on a more serious note I have not put in very many hours this last month I am hoping that the future does yield me a bit more time for that there were a few things sort of extended waiting for me this month that being said it is something I’m keeping an eye on and if I see that consistently that i don't have the time to dedicate to it I’ll probably withdraw from the position and just to allow someone more productive than me.
 
**Pooja**
Uh, it's actually uh like um I would suggest that do not withdraw it yet we need people it doesn't matter that like you know you're giving one hour.
 
**William**
yeah just to be clear I am still trying. Right if i see that it's just like you know I would not have pretty much anything concrete I could point to from the last month for instance so look if I see that that is consistently the case so I’d probably put some effort in trying to find someone else to try and come in I can do that anyway truth does.
 
**Pooja**
Right in the meanwhile, I was just talking to Lightclient and we were thinking of having a recording on how editing works maybe I can have Micah both on a call may be in an episode of people where we can record how the process work and explain it that might be helpful for new people like what all tiny details that they might have to look into. yeah, any other suggestion that we can create some resources for new people getting on board.
 
**William**
To be honest as weird as this sounds lightclient if you are open to having I guess I don't have a better term for this than like a ride-along or something like that if you're about to do some eiping or anything like that that actually doesn't sound very good and you'd be willing to have me kind of tag along or something like that i think 
 
**Trenton**
I think that's the perfect term if you know what rid a long means.
 
**William**
 it's like one of those where I said it and then I was like well.
 
**Trenton**
Maybe better context really would be pair programming.
 
**Lightclient**
Yeah uh, I think Pooja  mentioned something like that that would probably be a good thing to do I just need to figure out uh yeah maybe we can huddle together after this call and figure out a good time to do maybe one hour every week or two.
 
**Trenton**
 I'd love to join that too actually since some of.
 
**Lightclient**
 You weren't invited I’m sorry(laughing).
 
**Micah**
 Eip is a very private thing Trent.
 
**Lightclient**
 Yeah, all these open source repos. 
 
**Lightclient**
Yeah we can let's talk after this and find a time that works for us just to do an hour or so a little less a little more every week or so and then yeah should get our feet wet.
 
**Pooja**(Jason RPC spec drop-36:19)
 right yeah we were thinking about it like maybe meanwhile if we can record something on like ama kind of this frequently asked questions that people have around or get in touch with all these people I know Trent you have also volunteered to do that and William is there and there was another guy I don't know he's not in the meeting today so we'll uh check with him too and anyone else interested to generally learn how does this process work because we would want more and more people to join this is something that needs attention because more like proposals are stuck because it's not being reviewed not like a core proposal they are moving faster but for erc's definitely we need some more help maybe we can come up with something more concrete in the next meeting. All right uh moving on to the next item is Jason rpc api spec progress update I believe Alita you mentioned in the last meeting that you would like to go ahead and provide an update every meeting about what's going on in there.
 
**Alita Moore**
Yeah so basically in the past week we have gotten through most of what I mentioned in the last issue I guess I didn't I was too busy to fill it out for this time but are there any endpoints that are particularly important for us to focus on over the next two weeks?
 
**MIcah**
 Uh, the eip1559s if they're not done yet.
 
**Alita**
 okay uh, do you know offhand what those ones are?
 
**Lightclient**
 I wouldn't actually say the 1559 ones because right now we are we've kept two separate implementations of the spec and the one that's in the eth1 specs repo has the 1559 ones and is kind of the
coordination point and I’m just like keeping those updated for now until the fork passes but um yeah we'll transition away from that after the fork passes so it's not there's not like a strong need at this exact moment to get them.
 
**Micah**
 why do you think we should not use this process for London?
 
**Lightclient**
Uh it was just talking with Ted I mean we are using this process it's just which specs are we using and I’m would rather them not like focus on the one that's apache 2 from ethereum classic and focus on the cco version it's just that like the apache 2 version is you know not as complete as what we're going to want eventually but good enough for clients like we're still using it as the coordination point for clients to figure out what is going into London but long term like the work that all of our work should be going towards the cco version.
 
**Alita**
Speaking of which that's going to be delayed probably until this weekend because I have been very busy so yeah but I did promise that for today so um that's a bit of an update but yeah I will have um pr finished and I mean I’m probably just gonna merge it if that's okay with you all I mean I guess you know you all can review it but I don't know it's gonna be a long pr so I guess Micah likes to read long PR’s but just let me know.
 
**Micah**
 Contrary to popular belief I do not actually like reading long PR’s.
 
**Alita**
There's like essentially if there if anything comes up where there's like specific endpoints that need to be doing that need doing um let me know but otherwise based off what lightclients said and micah said um I’m probably just gonna kind of prioritize based off of you know what is best for myself and for the person working who's actually doing the work here um which is to me that like they don't have or jared doesn't have a lot of experience yet and so I’m trying to keep it somewhat simple um to kind of like guide that learning curve but um there's a lot of progress we've been doing things and there's also a major discussion right now about the format which is like kind of blocking us actually which is a little bit frustrating because like I think it's less important than getting things out you know what I mean like i think it's easier to go back and like reformat than it is to get somebody else on to do this so it makes more sense to me to just kind of like bite the bullet until we can figure this out as far as formatting and just go with whatever we have right now but what do you all think about that?
 
**Micah**
 Momentum is hard to change and so if we pick a format it's and we want to change it later I worry that it will be difficult to actually make that change as we've seen with the eip process we struggle to change it because people are used to one way and then it's very hard to convince them that something else will improve their experience if they just get over the hump of adjusting.
 
**Alita**
Okay so maybe we'll do it internally then I just really don't want to slow down anything I want to keep things moving as fast as they possibly can because otherwise, you're not going to make the august deadline we're already very much so I mean I already am pretty confident that we're not going to make it but if we slow down because of the formatting thing that we are definitely not going to and so.
 
**Lightclient**
 I mean what's this why are things slowing down why can't we just figure out the formatting and then continue on.
 
**Alita**
 well it's because until the formatting is figured out we can't open any more PR's and so we can't get client people we can't get clients reviewing and stuff so in other words, my point is that the formatting is like a very high priority right now um I’m going to schedule a call with lightclient and Tomas for this weekend to figure this out if any if anybody else is interested in being on that please let me know and I will add you but yeah it's like it is essentially it's saying as we have like the raw information but we can't deliver and if you can't deliver then you just have a bunch of work in progress and then we just get to like I don't know I mean it's just it's not a very efficient like pipeline that we have going on right now.
 
**MIcah**
So I think it sounds like the solution is we need to resolve the formatting thing quickly is there anything we can do to expedite the solution?
 
**Alita**
 the best thing I can think of is just this weekend we schedule a call and get through it on that call like basically we just call until we figure it out so yeah it was supposed to be this past weekend but I had a crisis at work and that's resolved now so I will follow up with it but.
 
**Lightclient**
 I mean Tomasz not available asynchronously at all?
 
**Alita**
 I guess he is yeah I can also um message him. 
 
**Lightclient**
If you just ask him to chat in the jason rpc specs discord channel then.
 
**Alita**
Yeah, I think he's a little I think he tends to be a little bit unresponsive because he's very busy  I’m not totally sure uh but he tends to be a little bit slow at times and so I don't know I think a call would be more productive but what we could what I’ll do is I'll do an async as well as schedule a call just so that we hit both avenues and then we can just cancel the call if the async works.
 
**Lightclient**
 sounds good feel free to send me a link to the meeting and time.
 
**Pooja** (cononical source for eip-43:57)
cool so the next item is a canonical source for eips so I don't know uh brent if you may have any update.
 
**Brent**
Yeah that's a time issue for me I need to fork myself but I haven't got it's still on my list of things to do but haven't done anything recently so gotta push it again.
 
**Pooja**
 right uh like uh do you want me to keep it on recording meeting or should we take it off and one you have.
 
**Brent**
 yeah  let's try it at least one more meeting and i'll try and get something before the next meeting.
 
**Pooja**(review action items-44:30)
 all right no worries okay uh so now we are on the last item it's review action items from the previous meeting um there are a couple of tasks that were like coming on from this meeting I just want to quickly have a like if there is any update the one is eip draft banner um are we done with that task or how is it going.
 
**Alita**
 Oh yeah, this one I have um unfortunately not finish this one I don't know maybe I’m gonna see if somebody else wants to just because I’m like I mean I can do it uh like I will get to Its kind of like how what's the priority of this item but maybe Jerry could do it I don't know I does anyone else know css because I do have like a kind of like a rough framework for it.
 
**Pooja**
 i think if we can open it for the community I mean if we have like a bandwidth issue we should create an issue and share it in our discord we have so many people from like you know developers community as well who are looking to contribute so if there is a way they can also contribute that would help us like speed up the task and yeah I mean I know you have worked on it so if you're around they can always reach out to you if that's okay with you.
 
**Alita**
 Yeah, of course, that would be great I think just posting a thing saying hey are you interested in this, and then just reach out to Alita if you are and then I can give them what I have right now um I’m sure that there is not I’m sure it won't take that long for whoever ends up picking it up but I am very bandwidth-constrained right now and so that's resulting in unreasonable delays.
 
**Pooja**
 all right so I’ll take on it.  I will create an issue and share it with people on discord and everywhere else uh the next uh task that we discussed sometimes ago uh was a boat tracking inactivity period that is issue 73 I saw Jared responding on that but unfortunately he's not there wondering uh if you have if you may have any update on that. 
 
**Alita**
what is this again sorry but are you talking to me?
 
**Pooja**
 Yeah, it is issue number 73 I see your comment like you would be able to help Jared working on this task it's about bot tracking inactivity period for eips.ethereum.org so they can move the proposals to the appropriate status if they are no more like you know inactivity for a very long time and that withdrawn status or so.
 
**Alita**
 So, in this case, I don't know too much about what's happening right now I do know that Jared is working on it and I do know that he can reach out to me with questions but I do not have a status I think Jared has been working very hard on the jason rpc stuff and so it's feasible that he and he's also been moving recently and so that's feasible that he's been unable to get to it um depending on the like on the priority of this I might recommend handing off to someone else I can you know guide and train whoever honestly but yeah I mean I' not totally sure uh I think maybe follow up with Jared asynchronously to see if he's done any work on it.
 
**Pooja**
 cool no worries I can follow up with him too all right I am now looking into the last meeting notes to see if we have any action items there and this stations number one anything that wants to be on ethereum standard needs to go through if you can github repository I believe that is related to erc process that we discussed in the last meeting Alita to investigate a bot exclusion to eip1 my understanding is this is done Alita can you
confirm that please.
 
**Alita**
 Yeah that's done.
 
**Pooja**
 Thank you eip1 changes to only require two editors to approve but this is also completed correct I believe both are interrelated that both are related to eip1 the json rpc api is back in either one as duplicated internally until after london I believe we discussed this today lifeline brought it up there are some changes and the last one is change the name of eth 1 api's repo after london is shipped that's a decision no action item on anyone. All right so that's all from the agenda item anyone has anything else to share with us or maybe bring it up we made it on time nice all right thank you, everyone, for joining today I hope to see you all in two weeks on July 14th have a good day evening everyone cheers.
