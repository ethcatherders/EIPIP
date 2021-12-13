# EIPIP Meeting 42 Notes
### Meeting Date/Time: Wednesday, Oct 20	, 2021, at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/87)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=7FXF-dRVgj0)
### Moderator: Hudson Jameson
### Notes: Avishek Kumar

----

## ACTION ITEMS

**ACTION 42.1**:  Plan a PEEPanEIP with Sam Wilson

**ACTION 42.2**: Update EIP-1 to mark “Stagnant” as another terminal state.

**ACTION 42.3**: Run a bot for “Issues” in EIP GitHub

**ACTION 42.4**: Update PR to update the list of EIP authors in EIP-1  

---

## 1. Post-merge will core cover execution and consensus, or do we plan to categorize EIPs based on what they touch? ref: [Discord](https://discordapp.com/channels/595666850260713488/746566142700814426/895319748378779719)

**Pooja Ranjan**: Welcome to EIPIP meeting 42 and I have shared the agenda in the chat. The first item listed here is post merge will core cover execution and consensus or do we plan to categorize eips based on what they touch so eip process after the merge is something that people are interested to learn about. I have picked up this agenda item
from the eip editing channel though I find some responses there later on but not sure if there is any general agreement. We discuss and come to a workable solution to most of the challenges related to eips statuses and the process, so I wonder what people of this group
imagine the eip process after the merge to be.

**Tim Beiko**:  I was curious about his thoughts but I can share mine and what I have been trying to advocate for. So I think eips are really good because they provide kind of an English description of the changes. Especially I am just focusing on quarry ips right now and I think there's a lot of value in like when there's a change to be able to bundle it with an eip number so say you know eip 1559 is this change transaction fee market eip 2929. Does this change the gas cost prices and so on? I think that's like a really valuable property like for example now if you look at the Altair  upgrade. There isn't eips for each of the changes and it's kind of hard to like explain what all the changes do.So that being said eips are also not a great place to actually have the technical specifications for the changes for a bunch of reasons and like clients has gone on to this before but it's just, it's hard because like you don't have all the entire specifications so you have to provide a lot of context and what not and the cool team has been working on an executable specification for the execution layer. So I guess a long way of saying what I would like us to do is to keep core eips as a way to describe the changes that's at a high level both on the execution and consensus layer. But then not necessarily use them to have the actual technical implementation inside. So that this way you could say an upgrade of the execution layer or the consensus layer has eips x y and z and the eips all have a link to a PR in the respective spec and that PR is basically what the actual technical changes. So that's what I would like to see. I don't think it's been fully like
decided yet. I don't think it will be fully decided before the merge actually happens but right after the merge I suspect is when we start working on the actual beacon chain fork is when 
we'll probably look at that.

**Pooja Ranjan**: That's interesting, yeah I mean I generally agree with what you are saying. I just have one concern or maybe a question there, when we are talking about keeping it in a separate pull request. Will that be a part of the main ethereum repository or would that be a part of the individual's repository?

**Tim Beiko**: So it would be a PR I guess from the individual's fork onto the main ethereum repository and then when it gets merged I guess when it gets accepted into a hard fork or something like the PR would always be on the main repository. Right it's just opened by someone else and I guess if it gets accepted into a hard fork then the PR gets merged into the main branch.

**Pooja Ranjan**: All right maybe I am missing something here but if I understand for a proposal to be merged maybe even as a draft.It has to have no external links so the first time when proposal is being proposed as a pull request to eip repository, it will be individuals but it gets accepted and then for further changes there will be a link within the eip for the
technical specification.

**Tim Beiko**:  Yes yeah so I guess we would have links for that.

**Pooja Ranjan**: All right I got it.

**Micah Zoltu**: So I am not a fan of that strategy as Iam sure no one's surprised at. I prefer the strategy that I think. Sam is planning on the execution specs repo once it's ready. Will have the human readable content in it and so the entire process can be done in the specs repo.

**Tim Beiko**: already we have that I think in the consensus specs repo. They already have the human readable version as well.

**Micah Zoltu**: No they don't embed. Where do they have that?

**Tim Beiko**: I thought they pulled it up.

**Micah Zoltu**: So they have the annotated specs.

**Tim Beiko**: Yeah like what they have is notation. They are human readable right ?

**Tim Beiko**: Yeah but those are, they are good if you are reading the spec
and you are trying to understand what it does.They are bad if you are trying to reason about things the way you know, like when we have discussions about including eips. I think those are a pretty bad format because they don't walk you through like what's the rationale? what
you know? What basically benefits does this bring? What are the trade-offs and I think  eips are great for that like a really good self-contained document.

**Micah Zoltu**: Is that content that needs to survive a long period of time.

**Tim Beiko**: I think so.

**Micah Zoltu**: And why is that like someone in five years when they are looking at the specs. Why do they care?

**Tim Beiko**: I think the value is like it also helps like the time it was proposed. Yeah it helps to encapsulate the changes in. Like a really valuable way, like I do not know I found like I have struggled to like explain alternative people more than I struggle to explain say like
Berlin because it's not quite as easy to say hey there were these three changes brought in and like at a high level here's. what many of them do. so I don't know what it feels like. It may be just for non-technical people like me but it does feel more legitimate.

**Micah Zoltu**: I agree the information is useful, Mike and what I am contesting here is how often are you explaining to people what was in the homestead.  Like you don't you talk to people about what's in berlin because Berlin. Just happened or what's in the merge or Altair because it's very recent but no one cares what happened in homestead other than like the people who are implementing it and need to have a client that can travel through homestead
and everyone else is completely. Oblivious and doesn't care like regular humans like not engineers don't need that history long term. The reason I think it matters how permanent the information needs to be is because I think for certain types of content. We don't need a really rigid long-term, like standardization process, like we just need a place for information to be and that place can be somewhere that's more transient where transit in here might mean a year or something but it doesn't need to be like 10 years.

**Tim Beiko**: Right I guess the other thing is, I am not sure how much this is like valued here but I think eips are really well understood by the community and they're like easy to point to and for people to like hatch onto whereas like even now that we have moved say the hard fork specs to like the specs repo. I still get I had literally vitalik asking me for the meta eip for London right then being like well where is the eip? So I think there's a really high cost when we move away from these systems. like people just you know are used to them and it's not to say that we shouldn't do it but yeah I don't know. I am a bit cautious of moving it away from eips all together but it's not a hill. I might agree to try to die on it. I won't fully die I will lose an army

**Micah Zoltu**: This is the hill. I am willing to lose an arm, maybe a foot. So I agree with you that change is hard and people will resist it no matter what it is? Like pretty much anything you change, people resist. you change the color of the facebook logo and people throw a fit like it's doesn't matter what it is or how significant it is or how significant it is and so I agree
that if we do a change people will push back on it and we should consider that to some extent. I wish that people would stop using eips. I think this is this is one of the things that I dream maybe one day we can get to a place where people that aren't implementing specifications don't use eips for anything like no one who's using a web browser goes and looks at the w3c specs like they are incredibly technical and they are impossible for anyone to read regular people go look at like and even regular developers go look at canius.com or whatever like they go to other places to get that high level information. They don't go to the specification like rfc see the same thing people who go to rfcs are people who are trying to implement an rfc compliant thing and that is it no one else looks rfcs and I think this is where I end up in conflict with a lot of people on the ap eips is because I want the ips to be that I want them to be a technical specification designed for a very select group of people I am not that we want to exclude anybody but just like the target audience is a very small set of people. The people that are implementing  things on ethereum directly and they need this strict specification to look at and then we have all that other stuff like that regular people go and look at somewhere else. I think I am kind of alone on this. I think everybody else would just rather the eips repo just be this monolithic thing where as the source of all information for ethereum. I think my problem with that is a I don't really like monolithic things I like things that are very targeted but separately we just don't have the manpower to manage a repository that grows outside of the scope that it currently has if we had more manpower than I think I would push back less hard. Because as we extend the the audience the target,
audience it gets harder and harder to maintain things and you get more and more people trying to get involved and contribute and it just becomes really hard whereas if you keep it very constrained say look this is targeted at these you know 30 people and that's who we're going for you know. We are not targeting everybody else then like the management of it is much smaller because there's less people throwing things in at it. There's less people reading it. Less people debating you know what we should do for different things. So I don't know, maybe if we can somehow figure out a way to get more like people involved in the process at a low level we could expand the target audience and not suffer as much.

**Tim Beiko**: So I guess I kind of agreeI 100% agree with the fact that limited by the number of people, limits the amount of things we can do if that's really the main constraint. I think that's a solvable problem and I am conscious that we have tried to solve this problem before with mixed success but we have also tried harder things on ethereum. I am also pretty sympathetic to your point of like no one cares after and what not. I think I would be kind of fully on board with your vision if we have a better process defined for them. How do we actually talk about stuff and decide on stuff when we are doing it. Right and that's you know yeah.

**Micah Zoltu**: I think personally I really like just as an engineer who uses github all the time
like most of my days on github or it used to be at least. I really like prs and I like using pr's
as the place where people discuss things and talk about things I find them because the code is right there. It's like close to go by and once the pr is merged it kind of just goes away and you can still reference it like if you want to refer back to discussions or whatever you can but I do like that personally. I don't know if it's a perfect fit here because I think pr start to fall apart when you get a large number of people involved in the discussion process unless you have like someone shepherding like the the first post and making sure that it's always up
to date with the latest conversation but I think no matter what we need a shepherd for every change and so the question just is where is the shepherd maintaining the current documentation for the change itself. So not the specification but where they documented those things like the rationale, the motivation and as people are contributing to the discussion you know. They add things like when I was doing 2718 people would
if i saw a question come up like more than once I would just add it to the rationale and so you need somebody there. Doing that step like making sure that this contains the latest information for1559. I felt you did a great job with that with your hackmd article like it had a huge number all the links to all the relevant materials that you know people could easily find everything I really liked that personally I don't know why everybody seems to hate that
process but I thought it was great.

**Tim Beiko**: Right, it's like I agree with you I think in theory and then I just like to think of all the practical steps and like hiccups to getting there and it seems like it's harder.

**Micah Zoltu**: Yeah I am currently debating  with Nick on this on the eips repo where we have the eips repo and it has a process. Creating a new process for a thing is hard, so it's much easier to just shoehorn your thing into an existing process. So it's like oh there's a process right there that's related to ethereum. I will just jam my thing in there and just kind
squeeze it until it fits and I totally recognize why people do that because of setting up. A new change control process thing is a ton of work and lots of you know figuring out the details. It's  complicated. I just worry so much that if everybody jammed once because what I have noticed is once someone jams their thing into the eip process then they come back like they force it to fit in there and it kind of fits. You can jam it in it maybe fits and then like a month one or two people do that and a couple months passed and then those people are like we should make the apd process work better for these things right and by making it work better for these things it works less well for the thing it was originally designed for which is corey abs and so each new thing that gets shoehorned in is bringing in people that want to change the process to fit their thing better which means it doesn't fit the thing it was personally designed for as well and so I think that's my worry of the whole shoehorning and I am constantly arguing people on the aps repo about this like three or four times a week at least
about someone. You know wanting to change the process because it doesn't fit their thing
and I don't have a good solution other than hey go build your own process which isn't a good solution it sucks.

**Pooja Ranjan**: well I don't think that we are going to get a solution right away today in this call for everything but yeah I think in improving the process we have we have covered a long
distance and educating people like how do we work and now that with some new changes
coming in maybe if we try to define the process early on would be helpful for other people while I agree to both Micah and Tim suggestion about seeing eip repository in a different way but I think or that's that's workable for core eips and there are a ton of people who are there using erc's as well so, if ercs are there,processes are there, standards are there it will be cluttered. We just have to try to clean it up and uh with the help of some of the bots that have been designed recently to you know help us with the process. I think we are in a process of cleanup and if I look at the stats today out of about 400 proposals that exist in eip
repositories. 200 are stagnant so, we did some part of it and we are trying to clean up step by step and come up with a clear and concise list of proposals that are good and irrelevant and as per the like people looking into the history may not everyone be interested. Looking into the history but some students especially like I interact with a lot of college students and I
have seen when they are trying to learn something they try to dig inside say for example account abstraction the latest proposal that vitalik proposed so when one of my students he was looking into that proposal he tried to look into all earlier proposals that were written for a counter abstraction they may not have been in like the final status but it did help so I think keeping history for these is useful and helpful for new people getting onboard and yes we might want to improve the process do some cleanup and give it a good look.

**Tim Beiko**: Yeah and I think realistically. This is gonna be a high focus after the merge. At least once the merge is done code wise I think it's gonna be hard to get input from like actual engineers and folks from like danny until the merge is a bit farther along even like personally it's. I know this is important because we need to do it. But it's like obviously less
important than the merge and so it just falls to the bottom of my priority list every week. Relative to just whatever thing related to the merges so I think once we are in a spot where the code is mostly stable and we're kind of going to main nets then people will have much more mental bandwidth to deal with this and we'll also be forced to deal with it. Because basically we're going to need to start planning the withdrawals for afterwards

**Pooja Ranjan**: I think  sooner I mean I understand your priority list here like getting into merge specs in place but I think the sooner we start discussing on the process better it would be for us because as for now we have just one proposal that kind of describe the changes what we are expecting how we are going to switch from proof of work to proof of stake that is very good but in case we are trying to have some more features or something to be added. If we keep getting them as like you know proposals as eips and we have a place particular place for that would be good for people to follow because they would not feel the friction like something has changed it would be same but if it start thinking about right at
the point when merge is there. I think it would be a little late for that.

**Tim Beiko**: I agree it's not optimal but I just think it's not realistic to expect a ton of feedback before it emerges much farther along so that's just.

**Tim Beiko**:  I think folks probably like me and Danny can start looking at it. It just feels like there is little appetite from like actual engineers to discuss this and maybe I don't know. Once we get to a spot where like the cordless calls are pretty empty again because like you
know we are done with the merge and people are just saying that they fixed it as bugs. That's maybe a good signal that we should start and bring it up.

**Pooja Ranjan**: Yeah I agree. I mean  as I said that it's not going to be decided today only but I just wanted to start discussion so we hope to get it discussed at some point.

**Tim Beiko**: I think one thing that could be valuable and is maybe getting like sam to present the executable spec on an alcor devs once he feels it's like in a reasonable spot
so that I suspect like most people on all core devs don't even know that's been worked on. I was thinking about that maybe if we can peep it absolutely but if we can also do like a five ten minutes on all corners. I think it just catches different audiences but like absolutely we should have even and maybe like a sort of teaser on all core devs or something where he can just kind of give a high level overview and then invite people to come there.

**Pooja Ranjan**: I will try to show you something real soon. All right I think we are close to
like  half of the meeting so let's just move on unless someone has some last thought to go on with on this topic.

**Micah Zoltu**: Only comment for me just to close it out is if you guys do want to try to devise a new system. I would be happy to be involved in whatever that process is so feel free to
invite me to things if you think that would be valuable.

## 2. Remove updated from EIP-1 Ref: [Issue](https://github.com/ethereum/EIPs/issues/4384)  

**Pooja Ranjan**: All right so moving on to the next item listed here is removed from eip1. Like line has just started this issue and I saw some comment from Micah but I am not
sure if there is any reference to any pull request. The link is added to the agenda so this   update is there in eip1 but it's not being used. It is about the last updated I think it is redundant because github will give us the last date of updating that proposal so it is not something that an eip author should keep on adding every time he is updating his proposal.

**Micah Zoltu**: Sorry can you put a link to the agenda  in zoom since I was late I missed it
That way I can find these things you're referring to.

**Pooja Ranjan**: Okay Okay I just shared the link of the issue and I am also sharing the link of the agenda here. 

**Micah zoltu**: So for that one we just need to have two pr's out we need to merge one of them.

**Lightclient**: Just turn Alex's pr and two ready for review without  Alex green.

**Micah Zoltu**: I will do it. sorry Alex you were overruled.

**Lightclient**: All right, I did it. It shouldn't auto emerge now maybe like it look at. Oh no it changes something other than an eip file

**Pooja Ranjan**: we will be coming to that admin issue as well like that is there in my agenda list today but before that I also want to go through this one so do we consider that                                                                                              number two remove updated from eip1 like salt.

**Micah Zoltu**: Yeah I think we just literally need to click the merge button on this which I am  about to do

## 3. Progress update on moving to Stagnant by [bot]Ref: [eip-bot](https://github.com/ethereum/EIP-Bot)

**Pooja Ranjan**: Okay cool so uh next one is some of the changes that I was wondering how to deal with and that's why I have listed them here with this eip bot. Like as I mentioned earlier 200 proposals have been moved to stagnant so far in the month of september and
october. So I am looking for some of the guideline to understand and may be able to educate
people on that the status changes from stagnant the present eip one suggests that it has to go back to draft. Do we want to always go back to draft or is it okay if we can update it to review or is it okay to go back to the last status say for example one proposal was in last call
but it was the last call for over six months. The ip author did not do anything and now it has been moved to stagnant. What do people think about when this proposal has to be pulled out. Should it go back to draft review or it can go to last call.

**Micah Zoltu**: So if someone has, I think I would rather people go to review first ,so I don't have a good reason for that to think about it. I just want to make sure that people are getting the appropriate eyes and they are just skipping ahead to the end in hopes that no one will actually look at their thing

**Pooja Ranjan**:  Right and with the last call here is like I mean I was thinking that if a proposal was in the last call. Now it has been moved to stanley. It can be allowed to go back to last call but that would be the day one again 14 days so it will get the enough review period of time

**Micah Zoltu**: So I guess realistically if someone wants to go straight from nothing to
last call. I don't actually have an argument against that like if you're so confident in your
thing that you think that you don't need anyone else to look at before it's done. I guess you could just go straight to the last call like I can't think of a good reason to force people to iterate through the steps like the more I think about it so I guess.  Yeah I don't have any good argument for forcing people to go through the steps.

**Pooja Ranjan**: Yeah that sounds fair to me as well. We might want to add some text to eip when describing these changes. Yeah lightclient do you have any thoughts or do you think it is fair to go back to the original status.

**Lightclient**: I don't really mind that much. I would prefer slightly to go to draft to review but if they really want to go to the last call that's also okay.

**Pooja Ranjan**: Sure yeah I agree I mean we want people should be around for the proposal to move it and we don't want the process to be a hurdle for them to like move their
proposals. All right I will make a note of that the next one is I think we discussed it yesterday in the eip editors apprenticeship meeting it's like when an author is making a pull request
to change the status.  would it require editor's permission or should the bot design. It should
be auto merge like we thought I would like. I have  suggested that it should be auto  merged because the author is there.

**Alita More** : is it like if the if it's created by the author

**Pooja Ranjan**: So actually I saw this one example. I think  the proposal was 1523 so it said that the barter left a message that it is auto merging but it never merged. So I guess there is some bug you might want to look into later.

**Alita More**: All right we'll do

**Pooja Ranjan**: I suppose Lightclient has also created an issue in the eip part repository. So, you might get some reference on that. Okay the next one is if moving the proposal is impossible for any reason say for example eip 3403 partial removal of refunds. We know that there is another proposal that went into one of the earlier upgrades and this is never going to go through. Now this has been moved to stagnant, so we would want this proposal to be out of repository not stay in the stagnant  forever. So the next course of action could be to move
it to withdrawal and withdrawn I don't know if the author would be around to do the thing. So I was wondering about what could be the other way so we make a cleanup here without the author's involvement if someone creates a pull request and the author  approves it. It's fair enough if not an eip editor can do it. 

**Micah Zoltu**: Sorry I was trying to merge that what's the short version of what you just said. 


**Pooja Ranjan**: so for a proposal which is no longer. we know that is no longer in the system. What do we do with that if they are standing in stagnant status?

**Micah Zoltu**: What do you mean no longer to go in the system

**Pooja Ranjan**: So there are a couple of proposals, for example eip  2070 which was mata e prepared for I guess Berlin or London. I know that it's not gonna go ahead so it's better to be withdrawn, that is  we know the author maybe we can reach but there are few more proposals. There was one for partial removal of refunds eip3403. We know that there is some other proposal that went into the final upgrade so this would never pull through and we don't want to leave it stagnant forever. Is it fair that someone creates a pull request?

**Micah Zoltu**: Why don't we want to leave it stagnant forever. I thought that was the whole
point of stagnant is a place, we can dump things that are abandoned or the author no longer
seems to care about.

**Pooja Ranjan**: Because there is a better proposal that actually went into it and it was
proposed by the same author.

**Micah Zoltu**: Yeah I am like I still think there's value in. So I am not a fan of doing anything with other people's eips and so we have two options, we have currently it's our current process is either allow it to fall on stagnant just due to no one touching it for six months or two months or whatever it is or ask the offer author to withdrawn like we don't have a process for any other terminal states besides those two and I treat them like mentally is fairly. Similarly, are you saying that you want to delete the eip or just move it some new way?

**Pooja Ranjan**: Oh no I was wondering  like the proposal that has a hope that it can be pulled back  should stay in withdrawn as long as author wants to but there are certain proposals which personally I feel is no hope for them to ever get added to the final repository because that was an intermittent proposal and something better was proposed during the same cycle and the better one went into the upgrade so we know that the older version is never gonna go through

**Micah Zoltu**: So the two questions I or one question will comment on. What would you like to see them with ? Do you want them deleted from the repository or do you want a new status?

**Pooja Ranjan**: Maybe withdrawn because that is the only terminal status we have got here. It is just that this time with John is not by the author. It has to be with the permission of eip editors. I am just proposing this.

**Micah Zoltu**: So my concern is that  deciding which eips are never possible and which are not is challenging. At best for example  this proposal 3403 partial removal of refunds like maybe the authors feel that there is still a chance for that just with a little bit of tweaks or whatever. Similarly like when eip1559 went out. We had several counter proposals that people created and yeah well 1559 one could argue kind of it won some the the authors of those may feel like you know they want to try this again in six months or a year or whatever maybe they are waiting for 1559 to fail so they can bring their thing back in and so I am very hesitant as an editor to get into the business of deciding whose eips are no longer relevant and who's aren't. Like I would rather the author make that decision and if the author makes that decision they can move it withdrawn and within alex's change they'll be with withdrawal reason and they can say we decided to go with eipx xx instead this is no longer relevant. That being said like I am perfectly fine with stagnant being terminal like if it we can just update the ip1 or the picture or whatever to just say you know  stagnant can be terminal like
it's okay if things stay stagnant forever because there will be a lot of stuff that isn't stagnant forever.

**Pooja Ranjan**:  I hear you. Yeah there was this another proposal that was also in my mind like 2593 which was escalator free market change for eat 1.0 now that 1559 is there so I was considering that it may not go through but hearing your thoughts it is possible and yeah an author may decide at this at some point that he would want to bring it back okay. So I see one more plus one on stagnant forever. So maybe we would like to make these changes on eip 1. I will keep it open for at least one or two more meetings. These changes that we are discussing today for eip1 and then after a few rounds of discussion maybe. We will update the eip1. Does that sound reasonable?

**Alita More**: Yeah I am also okay with just if you want to create a pr against eip1. We can have discussions there asynchronously if you prefer that yeah that may speed up the process make sense.

**Pooja Ranjan**: All right and the last one here on the list was about moving the proposal, if there is a necessity but eip author or champion isn't actively involved. I know Micah you
suggested someone getting involved from the eip editor apprenticeship program to look into that and we kind of discussed that yesterday in the eip operating apprenticeship program but
 the concern here is we might want to have authors' approval to be added as a  champion or co-author for the proposal and if we are not yet not getting the author's response at all, what is the solution?

**Micah Zoltu**: So  ideally we get the current author to like it if they are not interested in doing the champion. Championing themselves like the busy work of fixing things and getting through the review process making changes etc.Then ideally we get the author to sign off on somebody helping them out and so for example you know if there's some. We will William I don't know what he goes by, if he wants to help out that would be a great place to help and he helps someone who is interested in getting involved in core eips to learn the process and everything but they can do it with someone else's idea so they have someone with an idea they want to push through but they don't want to do all the bureaucratic stuff of vip editing they can get help from someone who wants to learn the process so that's the ideal scenario which I think we all agree on if the author is completely unresponsive but we do want to get it pushed through the fallback option is to have find someone who wants to champion it and go through the editorial process to just basically make a clone of it. Make a new eip that says the same thing but with a different set of authors and push that one through and if that one gets pushed through then eventually the other one will go staggered

**Pooja Ranjan**: So  the second option question  the eip would not be the same number correct?

**Micah Zoltu**: Actual champion presumably and so we'll actually make it final and then once it's final then the original one will eventually fade away into stagnant or withdrawn
got it.

**Pooja Ranjan**: Okay let us give some more thought we did discuss yesterday. We had couple of more people joining in the meeting so we are trying to come up with a small group
of volunteers who might want to help us in this process. Maybe we discuss with the eip author try some more time  to it and if not  then maybe that is the ultimate option I suppose

**Micah Zoltu**: Yeah maybe try reaching out to the author on multiple channels like just like
email or discord or github just to see maybe they're simply not getting the messages. I don't know.

**Pooja Ranjan**: Yeah, it makes sense, thank you.

## 4. [EIPs Insight](https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/) - Monthly EIPs status reporting

**Pooja Ranjan**: Okay that's like most of the sections the next one is eip insight. So this is just a monthly report that I have started recently talking about how  we are doing on the eip site up till october 15. There are two new proposals one is account abstraction 4337  and another one is difficulty bomb delay to summer June that is eip 4345. One proposal moved from draft to review is an erc 1581 and about 115 proposals have been moved to stagnant status. We see some efforts are being made to pull out some of the proposals that are good and encouraging that at least people are trying to move their proposal to a decent status.
We are happy with the progress that  we are making with the help of bart and the team eip editors Alita and everyone who are heavily engaged in helping out with this so thank you
everyone.

## 5. The future of "EIP merge bot" - Is it safe to turn it down?

**Pooja Ranjan**: The next item that we have listed here is the future of the eip merge part so we know that there was another bot run by nick johnson and that was not working for a while or we thought that it's a good idea to create our different bot and that's why we have eip bot. I was wondering whether it is safe to turn it down or do we want to have it running.

**Alita More**: I think about the old one you don't. Is this the one with the travis ci that we'll get right now

**Micah**: Yeah I haven't thought about the next run for a while.

**Pooja Ranjan**: But he's still running it. I mean he has still kept it on and he wants to check whether it's safe to turn it down if it is not being used at all and if it is being used it's fine.

**Alita More**:  I think that this is a different one. We have two eip validators and realize one isn't travis. It's in ruby and I don't know if you want to like trans transfer the logic from here over to the other one  or something but regardless.

**Micah Zoltu**: To answer the next question, yes you can turn it off. We do not use it anymore. I believe it's been disconnected from github all right that makes sense to Alita's question. Yes long term it would be nice if we consolidated the bots into one consistent location and ideally one consistent language but I think that's probably not a high priority. It's not for me. Okay sounds good.

**Pooja Ranjan**: All right so this is good like I can inform him to turn it down.

## 6. Admin access to EIP repo to EIP editors?

**Pooja Ranjan**: The next one listed here is admin access to eip repo and a report to eip editor so recently .We have made some I can't say changes it's just that we are trying to represent it correctly like  most active eip editors and we have a new section called emeritus
editors to list all the editors thank you Tim for that suggestion that really helped, I didn't want it to remove the name because it's  good to have history there and I talked to different eip editors which are still as listed as active but  they would want to be removed from there.With that list I think I will be sending one more pull request to update the list. We have received from some of the eip editors  that they no longer want to be a part of active editing . But I was wondering, like the eip github repository there are very few people who have admin access. I suppose Micah you already have the admin access unsure about  access.

**MIcah Zoltu**: Yep just me and the like it's just me Jamie Pitts and Nick Johnson 

**Pooja Ranjan**: yeah yeah so I am wondering like not most of the people are heavily
engaged but Light client is so can we consider getting access to the people who are working right now  like i know there are only two three people access Lightclient Micah I see all these
comments I know Greg also expressed interest to get the right access to the current repo. do people think about like any thoughts in favor not favor otherwise.

**Micah Zoltu**: so for Lightclient I am fine with him in access. I think Jamie is probably the one you didn't talk to though similarly okay he contributes fairly regularly not as regularly not as regularly as Matt but regular enough  that I consider him an editor. With Greg I am more on the fence and the reason is because pretty much the only time he interacts with the ips repo is when he's working on his own eyepiece  like he doesn't really do any editing of other people's stuff and I am kind of hesitant to and incentivize  people to kind of get eip access
just so they can merge their own eips and bypass the process. That's my weak feelings if  he wants to get  back to being involved. I am  okay with  that and similar with Nick Johnson like
Nick Johnson was an active editor in the past but isn't anymore again the only time he interacts with the repos with his own stuff that being said Nick. Nick has historically shown a little more restraint and he usually will defer to the other editors and won't audemar like won't merge his own prs for example right so this is my kind of surface thoughts on the subject.

**Pooja Ranjan**: Right for Nick he said that he would be like he would be interested in getting into active editing but his time constraint does not permit him so he would like to be a part of non-active editors for now but Greg showed his interest and he said that I would be interested in getting back into editing but for access. Right now I think let's go ahead with Lightclient and see with like um in a period of time if we get  more attention more work done by more people then we can start involving more one

**Micah Zoltu**: Yeah just um talk to jamie pitts I believe this is the right person

## 7. Review action items from the previous meetings

**Pooja Ranjan**: All right, okay , so that's all about it. We are almost done with the agenda items  we have just  the next meeting sorry for the last meeting  decision or action  items. okay the one thing the part will  show a notice to new issues to make a discussion thread on ethereum magician.I think the bot has started working on that direction but there is one thing
that we wanted to do in issues eip issues which I think still need work on activating the part to clean up the issue section. Maybe Alita whenever you get chance to look into that you might want to consider it

**Alita More**: can you repeat that?

**Pooja Ranjan**: so we have one bot for pull request section of the eip github right that helps with the stagnant proposals and trying to clean it up close them marking them as stale or stagnant. Similarly we would like to have a one for the issues section because we have over 400 issues and I mean I am assuming more than 50 are non active discussion things so if we can have similar part activated and we start closing the issues we will have room for
active discussing issues like real issues that people would like to discuss about all right 

**Alita More**: okay yeah  that one is I can definitely do I will add that to the list

**Pooja Ranjan**: yeah so i think that's all from the last meeting  and yeah that concludes all the items listed here anyone has anything else to bring up today.

**Alita More**:Yeah I am just uh are there any other I am gonna be doing a bug bash with the bots this weekend  and just try to basically get through every single bug , so get your bugs in like if you know of any bugs that aren't  reported yet please report them on the eip repo so I can have you buy repo. So I can just grind through them this weekend.

**Pooja Ranjan**: Awesome okay, later just for your information like here is this one resource he has reached out to me and he might be interested in looking into the erb spot site oh like it as in working on it. yeah not no not completely but you mentioned earlier right so you might be looking for someone so he is interested I will try to get more conversation
and if he fits with you.you're happy to refer to you 

**AlitaMore**: yeah

**Pooja Ranjan**: Okay and I think that's all we have listed on the agenda today. Thank you everyone for joining and yeah hope to see you in two weeks thanks.

---------------------------------------
# Attendees

* Hudson Jameson (Host)
* Tim Beiko
*  Danny
* Micah Zoltu
* Alita More
* Pooja Ranjan
* Brent Allsop

# Date for Next Meeting: 27 October 2021 at 1500 UTC.




