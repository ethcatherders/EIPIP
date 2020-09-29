# EIPIP Meeting 16 Notes
### Meeting Date/Time: Wednesday 9th September 2020 at 15:00 UTC
### Meeting Duration: 55 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/30)
### [Audio/Video of the meeting](https://youtu.be/UJmYpFkZGzY)
### Moderator: Pooja Ranjan
### Notes: Alita Moore

## Summary

## Decisions Made:

Decision Item | Description
-|-
**16.1.1** | Propose changes to the EFI process on the EFI github reposoitory / to the README
**16.1.2** | we are at the stage now to begin implementing the new EIP process and migrate the EIP repo to the new ones
**16.1.3** | triaging purchasing requires upgrading the ethereum organization github, Hudson is having a meeting to discuss pros and cons
**16.1.4** | remove the precompile address discussion from agenda / not applicable to EIPIP

Action Item | Description
-|-
**16.2.1** | Change name from EFI to CFI
**16.2.2** | add Edson's transitions to the README without specification on their interactions then update them as necessary
**16.2.3** | Micah to implement relative paths
**16.2.4** | Edson to create document outlining the required criteria and procedure for onboarding EIP editors

Helpful Links | Description
-|-
**16.3.1** | https://gist.github.com/edsonayllon/e9b91a2c3a8e2d4e242cfc236162e106
**16.3.2** | [EIP statuses abandoned vs. withdrawn](https://github.com/ethereum/EIPs/issues/2941)
**16.3.3** | [problems with EIPs by Axic](https://hackmd.io/issXMJfhSCqvlffu3NHxbA)

##

# 1. Network Upgrade repository and process

Video | [0:00](https://youtu.be/UJmYpFkZGzY)

**Hudson** - okay now we're live 

**Pooja** - hello everyone welcome to eipip meeting 16 agenda is in the description box the first item on the agenda is network upgrade repository and process i guess james was working on it james do you have any update on that 

**James** - there's a project board now there's a readme that describes it in gener like generally the principle and then there's a project board with the current state of eips going through the network upgrade process which in which up to this point is um CFI which we're we're proposing to change the name of EFI to CFI which is going from eligible for inclusion to considered for inclusion and then the next step after that is inclusion on a client integration test net like yolo v1 or yolo v2 and that's the process up to this point 

**Pooja** - great uh in previous meetings we also uh were discussing about the process like how we are going to you know move so this project board that we can see there is actually what we are coming up to 

**James** - um what is what do you mean by the question 

**Pooja** - uh like two or three meetings back there were a few proposals on how this uh repository is going to be managed or what it would be the process for network upgrade because i guess we decided sometimes back that it has to be you know proposed in a form of a proposal and add it to eip1 by uh by adding this proposal separately so i was just wondering uh if we have anything decided on the process part do we want to discuss it now or it's just good that they go ahead 

**Edson** - yeah can we discuss it now uh also an update i said the statuses on the our whole devs call there wasn't much feedback there also wasn't any opposition to the new statuses um james you weren't here but uh we discussed a possible set of um phases for the hard fork coordination process i linked it um in the chat i could share it also if you guys want that like i could share my screen

16.3.1 | https://gist.github.com/edsonayllon/e9b91a2c3a8e2d4e242cfc236162e106

**James** - um do we do a video recording of this when we post it yes then yeah sharing your screen will be great 

**Pooja** - just to give you a little background here uh so a few meetings back there was few proposals uh one was presented by edson one was with me and we come up with some kind of uh solution like we can come up with a combination of these things in absence of you we could not come up to a particular decision so that's what we are hoping to achieve today 

**James** - okay 

**Edson** - so here are the different uh options that i came up with and uh the final one we came up with was like a combination of these so this is number five okay so we have them each in stages stage one is eligible stage two is implementation stage three is testing stage four stage so this is stages it's the decision to go to mainnet and then the the date is decided on where the block is deciding them and then stage five is deployed the ap is live so the the date has elapsed and the EIP is live stage six maintenance review monitoring the EIP after it's launched i mean that and seven is just rejected which can happen after after any of these stages okay and do you want me to to go over the other ones or

**Micah** - what's the difference between five and six

**Edson** - yeah that's a good question um so originally one of them had maintenance um i think uh six might be redundant because um once it's deployed then would we say it's deployed or we say it's in maintenance 

**Micah** - i'm okay with either of those it just feels like each of these stages is like has a clear milestone that is achieved and once you cross it you're in the next stage except for those two which both seem to occur at the same time 

**Edson** - yeah um i think like the difference here was before they were just deployed and then we never really saw maintenance before that makes sense like we never made that our priority where um once it's deployed do we keep monitoring it or not 

**James** - when you say monitoring it you um i'm trying to get a sense of if i if i have an eip go in then because they are monitoring mainnet in the chain i don't know if anyone is moderating monitor monitoring the eip or an individual eip if that makes any sense

**Hudson** - yeah i don't think the maintenance makes a lot of sense i think it would just cause more confusion

**James** - uh and there's a little bit of difference i think the teams the that are when you're maintaining mainnet you're not thinking about i'm maintaining an EIP an eip you're just keeping maintenance alive

**Edson** - yeah i was more thinking like maybe a performance like the to like measure EIPs once they're deployed see how they're performing 

**James** - that that would be that would be cool to have a like a review for or a post like a post mortem but not that word the other word retrospective like have a retrospective on eips and see if they do what they're trying to what they said they would do that would be interesting 

**Lightclient** - isn't that just part of the eip like if it's not doing what it says today and that's the shouldn't that be addressed in every stage

**James** - um yeah i the it would be nice to have kind of this um let's see so having some more explicitly let's go back and look at a decision and evaluate it would is kind of an interesting thing for me personally when i've been putting the hard four coordination and work together and such i've worked really hard to not uh be prescriptive about what things might what things will look like later or what things could look like and the the reasoning for that is that hard fork coordination is really not like most other software upgrade processes and the combination of working with multiple clients for ethereum even out even within blockchain ethereum has kind of its own way that that it develops because of the multiple client implementations and then the breadth of node operators and and community members like they and so although i can certainly sit down and think of ways i think it will go and maybe have a good prediction or not i've hesitated on saying this is what it will be like and rather just went with the emergent properties of what is happening as it's happening so for an example is and and this the these stages generally describe what is going to happen um what what does happens or what is going to happen um but i don't know if it's it's necessary to really have it all written out in in such a way yet because like for stage one it's the having an open discussion about if it's gonna be available or not and nine months ago before EFI was thought of i wouldn't have told you that that was the best way for us to to track that step but it it turns out to be to work really well and it emerged from part of the core dev calls there was a little bit of confusion about stuff and so then now we have EFI that came from uh some other proposals and that stuck as something that's working really well and then for stage two implementation i guess where the next step is for clients to implement it but uh we didn't we were having trouble getting clients to merge prs with the eips themselves and there was about two or three months where we were there we were in this weird lull where we had eips that were considered for inclusion EFI at the time but we weren't getting them merged into clients in a way that allowed us to do testing between multiple clients so in that in that time while that was happening uh martin and some others thought hey this you know what would be really great is if we had a test net that was different than any other test net we've ever done and we make sure that it's a test net that no one else is going to deploy on and all it does is sync clients so that clients have something to work towards and something to um to merge into their clients and have everybody agree on what to think this is also around the time where we looked at the uh instead of having make a fork figure out what goes in it we did the version where as eips are ready then they are then they're scheduled to go into a fork like the train model or otherwise that has been said so because we had we when we changed to that model there was the moment of hmm without a deadline it's hard to get people to do stuff or without a solid target so then we went uh we went back and evaluated and then came up with the next stage which is getting your eip into a client integration test net like yolo so i'm sure that so and then so stage three testing of course we need to have testing and fuzz testing but what is what is it what does it look like to have finished that stage or what does it look like the thing that we need to do to make sure that stage is being done hasn't really been established yet and i don't know what it will be but it will be something and then stage four staged is um when something goes on to a test net like a more client used or used test net like robstein or whatever all of those things that's it that's really part of the staging process but what's the decision and timeline and stuff around that i think is yet to really be uh established and i'd rather let i'd rather see what happens with the core devs and then adapt to what is needed on on that and then stage five is the hard fork is up and it's and it's live so i think this does a this does a great job of highlighting the general path of what's going to happen but i wouldn't i wouldn't like to specify how we get from each of those stages and what it needs to be to to go from each of those stages until we are going through them and observe and figure out which are the best which is the best way to work uh as things emerge

**Pooja** - i can also see a table here like the project board is it reasonable to consider that maybe the stages i'm talking about the project board that is available on the ethereum 1.0 spec it says that CFI applied approved test net applied uh is it something that can be considered as stages for network upgrade and that's what we can go ahead with 

**James** - uh yeah because that so that is stage one a and stage one b and then stage two a and stage two b in this in this list that that edson has here and the reason why i had both is because we have discussions like their people propose that it goes from one stage to another and then it's in that stage and then people propose that it goes from one stage to the next and it made sense to track them where as being proposed and accepted into each of those buckets so that is what that's that what is happening

**Pooja** - right uh so from the point of view of documentation is it do we really need to document it i mean like uh in the in one of the previous meetings uh uh there was this document shared by um me i mean i shared it uh in which we tried to document as uh similar to the eip1 but since we are making a new upgrade process for a network upgrade it was just for the other one uh the new one thank you edson so here we have actually tried to document the um process or how we are doing it in a form of a proposal that can be added as a pull request to the new repository and can be saved as a reference point is it something that we still need or we are good with 

**James** - this is i added this to the to to the this is the read me now of the website of the network spec oh yeah i remember sharing it with you

**Pooja** - sorry i missed reading the readme it said 

**James** - maybe just let's go to the specification eth1 specification website uh the github repository can you can you do that edson 

**Edson** - yeah do you know what it's called yeah i'm gonna share the link here on the chat is it where is it yeah 

**Pooja** - so yeah that's right so in this way like the readme already explains whatever we want to do with this particular repository i mean it looks good to me but if there is anything else that we would like to add as we discussed today the stages 

**James** - yeah so this is this i pulled from that document i left out the diagram of the actual stages because i'd like to do that as we go document them right and the network upgrade process or is good for tracking it and then as we move along we can we can clarify and write what the steps are more specifically right yeah so if there are things to be included on this or thoughts for stuff that needs to be included so like some ideas is what is the specification of mainnet do we put that on there um having the specification for yolo putting this do we put that on here um or any other ideas that you guys have feel free to propose and we should discuss

16.1.1 | Video | [17:00](https://youtu.be/UJmYpFkZGzY?t=1021)

    Propose changes to the EFI process on the EFI github reposoitory / to the README

**Pooja** - right and in the issues section i see that uh there is an issue already created for uh discussion on EFI to CFI do we have right set of people where we can discuss about it 

**James** - yes 

**Pooja** - personally i am in favor of changing this like EFI to CFI but if people have other thoughts feel free to share 

**Hudson** - i'm cool with it too it's not a huge deal to me either way 

**Pooja** - i mean i was thinking like eligible sounds more like okay fine you are eligible you are getting into it but CFI sounds more reasonable like consider i mean i found that more reasonable so 

16.2.1 | Video | [18:00](https://youtu.be/UJmYpFkZGzY?t=1082)

    Change name from EFI to CFI

**James** - yeah and it felt like a good time to make a transition of name while we're migrating to eth 1.0 specs to just take and make sure that everything all the terminology is uh like button down and more specific 

**Pooja** - in the chat mike mentioned that he also supports going from EFI to CFI and further he mentions that i also like the stages after stage five and six was combined 

**James** - yeah so i i'd say that we take edson's list with the stages and we can put them into the readme and then leave off uh specifying exactly what or how that the each stage transition is defined and then we'll go back and update them as they're they're happening 

16.2.2 | Video | [18:54](https://youtu.be/UJmYpFkZGzY?t=1134)

    add Edson's transitions to the README without specification on their interactions then update them as necessary

**Edson** - so you're suggesting we just start implementing the stages and then define how to move them once after we go through them once 

**James** - uh to to write that as that is the rough path that is going to happen but not say exactly how like by implementation is a is a the number two is is the rough path is the path that an eip will go through it has to go through implementation 

**Edson** - i mean um i'm sorry i guess there's a stage called implementation so we we just we use these stages right like officially but we don't we we go through them to see how how it works going through each of them 

**James** - yeah i wouldn't even know if i would say we use them as efficiently but more of as a as a guiding post for stuff that will probably happen like the consider for uh like implementation the yolo stuff is the stuff that you track and have for the stages for implementation like the sub stages um i don't know i guess it might be confusing too i'm torn between the giving people an idea of what's going to happen and me or or just uh what's the word like manufacturing a process that it doesn't naturally fit when there's stuff that will and we just don't know what it is yet 

**Edson** - I see what you're saying, so like in terms of like one moving one status to the next i i did write something one of them was just we just keep doing what we're doing now like what we're doing naturally and let's define it later um is that what we're moving towards

**James** - yeah we and we don't have we yeah and we define it later and like for example the the considered for inclusion is pretty it's pretty close to ready to defining and having been gone through enough times to say this is what it's like so as we get things further in the process we'll get more and more settled about this is the this is the right way to do x and this is how we track y um i just want us to get to that point and then figure it out 

**Edson** - okay also um uh i guess like since we have enough we could update EIP1 

**James** - um i would say we update EIP1 to just point to the spec repo at this point and not have any specification of the network upgrade be inside of it yet

**Micah** - I feel like that uh pointer is wrong direction i think network specification is quite dip is not the other way around like to me the eip is a um a primitive that can be referenced by other things it is not a high level construct like fair in my opinion the EIPs are technical specifications only they have no politics there's no opinions it's just this is a technical spec for a thing that someone thought was a good idea and then the uh network upgrade process could then point to those and say hey this is the technical spec that we'll be implementing on this date or whatever um but having eips point to the inclusion process which is much more political feels to me like the wrong direction for that pointer 

**Lightclient** - i feel like it's just metadata so i don't think we have to have any of the upgrade discussion in the eve but if i'm looking at it if it's valuable for me to quickly be able to go to where it's being discussed in terms of governance 

**James** - i can see your point on the on eips pointing to the network upgrade process like individual eips except for maybe the the exception of eip1 saying that we have an effort we have an upgrade process and that to look at it you should go elsewhere 

**Micah** - sure um i guess for me that's more appropriate for the readme than the eip1 like to me eip1 defines this is how you write a spec um whereas the readme is more like this is how you how ethereum works and how we use this repo um but i wouldn't be i wouldn't push back hard against that mta if you want if it was just like you mentioned i think

**James** - yeah i'd be fine with either of those it's the i want to be able to if someone's at the eip repo and thinks how do i find the main how do i find the upgrade process i want them to be able to find the right repository so if that's the readme or if that's the EIP1 or whatever it's less than i think i think the thing that like lion's bringing up and the point of disagreement between us on that is um is the eips repo specifically for ethereum mainnet or does it also include ethereum classic and rsk and all these other things that reference the eip's repo i don't know if that's actually on our agenda um though we have been off and on talking about it for a while

**Lightlcient** - I feel like deep's repo is just for ethereum i think all these other chains have on governance processes or specifications repo 

**James** - even though even though ethereum classic uses eips they also have the eip and their own repo for tracking it so and i agree that it should be specifications and tracking them i do see value in at least having a tag that says this is an eip that's on mainnet 

**Edson** - i see i see micah's point though that if a specification is a specification it can be used by other protocols segregated protocol agnostic if it's well defined like erc several other pro like several other chains have their version of erc now because it was um just defined well and used enough in ethereum 

**Lightclient** - sure but i think that those other chains can spend their time and track what they have launched on their network and we can focus on our network 

**James** - yeah we had we talked about it earlier as even just having it on the eip website like eips.ethereum.org have a tag that track that shows up on eips that are implemented in mainnet but what is implemented in mainnet is tracked in the network 1.0 specs not in some meta-empty or as or as like explicitly even needs to be a field but some some way of of doing that 

**Lightclient** - i mean all i would love is an additional field in the front matter that says i don't know um yeah i don't even know what the name of it would be mainnet status and maybe something like that and then you can plug in whatever its stage is for the upgrade process and then link to whatever that repo is 

**Pooja** - just one point i would like to mention here uh that came up yesterday during a conversation with greg on the eip repo like since we are trying to separate this network upgrade and other proposals there so he was just mentioning it like it was a casual conversation where we were thinking about like should it be called as eips because we are taking out all the core eips and taking it to network repository mostly the leftover would be erc i know this is not very legend and may require a bigger discussion but just wanted to bring this point 

**James** - um i can respond quickly that the it sounds to me that greg is thinking that eips are going to be moving over to the network spec repository but that's not there there won't be any eips in the network spec repository there will just be lists of things that are going into the maintenance but they will be still in the eip repository right so there uh there isn't anything there isn't anything of that type that's moving over um well i just had a thought um i lost it but it'll come back to me 

**Pooja** - i'm sorry i think Micah was saying something 

**Micah** - my fear with adding anything about uh the network upgrade process to a vips is it will encourage people to come over to the EIP repository and debate politics on whether we should include something or not and i really would love to see that all go away and by go away i mean become someone else's problem which means whatever manages the repositories (it's a really big problem with eips) we're trying to define a technical spec and we end up with just like a bunch of people talking about whether this is a good idea or not and i would love to make it so we can just tell them hey this is where we're discussing the technical specification which may or may not go into ethereum may or may not go into any other network it's just a technical spec if you want to discuss whether it should go into ethereum here's where you can go and it allows us to segregate so we can focus on the technical stuff here and we can focus on the politics somewhere else 

**James** - yeah and i and i've seen similar uh interesting things about where we're talking about a specification but then we're really talking about what it would need to be able to launch on the main net but that's not something that needed to be talked about at that stage or focused on so makes it difficult um i saw i remember what i was going to say that i do think we're at the stage where we're ready to start the new ta the new processes for the eip statuses and migrate the eip repo to the new ones

16.1.2 | Video | [29:19](https://youtu.be/UJmYpFkZGzY?t=1759)

    we are at the stage now to begin implementing the new EIP process and migrate the EIP repo to the new ones

**Pooja** - great 

**James** - i had been hesitant before because i wanted to be able to and i had good feedback from this group that we would we should have a place where we can point people to the network upgrade process before we start making changes like removing accepted as the status so now that that we have something and we can point people there i think it's time for us to or i propose that we start implementing the new eip statuses

**Micah** - here if you're according to like uh there's a document floating around somewhere that has them um like withdrawn and stuff 

**James** - yeah uh i see uh a request for comments and changing active to living and those like that diagram yeah 

**Micah** - okay 

16.3.2 | [EIP statuses abandoned vs. withdrawn](https://github.com/ethereum/EIPs/issues/2941)

**Pooja** - there is a pull request i'm sharing in the chat um i think uh that is looking for some more discussion on the status eip statuses abundant versus withdrawn um just wanted to bring it to attention of this group so that may be considered when we actually start implementing the eip statuses. okay so any more thought on this particular topic we are almost 30 minutes past so 

**Edson** - yeah i just want to comment on the repository it looks like people already using that to have their EIP uh considered for inclusion which is good um that the discussion is being moved here and i guess like we could make as many issues as we want so we can actually have discussion here 

**James** - yep and feel free to make issues for like uh things you want to see in the repository or stuff you think we should we should be considering uh we have a lot more space to make issues of any kind we want because we're not inflating efp numbers or interfering with that process

**Pooja** - right that was my biggest worry 

**Micah** - yeah we're almost out

# 2. [Relative vs. Absolute Paths](https://github.com/ethereum-cat-herders/EIPIP/issues/30#issuecomment-682540129)

Video | [32:00](https://youtu.be/UJmYpFkZGzY?t=1921)

**Pooja** - so moving on uh to the next item it is a relative versus absolute path there is a link in the agenda and that leads to some comments by micah so micah would you like to take it over 

**Micah** - uh sure i think uh just to start out is anybody opposed to relative paths everybody i've talked to so far seems for a relative paths and i think it's just a matter of we need to do it but i want to first see if there's anyone opposed is just we want to standardize how uh links are handled and the question is do we do dot slash eip dash one dot md or do we do https call slash slash eips.ethereum.org slash eip slash emp dash one um is anyone opposed to relative if if not we can just skip this whole topic and just do it uh if someone is we can have a more fruitful discussion 

16.2.3 | Video | [32:45](https://youtu.be/UJmYpFkZGzY?t=1965)

    Micah to implement relative paths

**James** - i would say just do it yeah i mean adding that and it's uh so that's something that per that falls to the purview of eip editors more so than other topics that we bring up so just do it 

**Micah** - we can always undo it if we get significant negative feedback as well yep okay we can just i'll just take i'll get a pr out in a couple days next couple days until someone beats me to it um and we can skip that 

# 3. EIP Working groups

Video | [33:15](https://youtu.be/UJmYpFkZGzY?t=1995)

**Pooja** - so moving on the next item is working group but i'm gonna skip that because i see uh there is a comment by liteclient uh in the agenda itself i'm going to read that comment it says that i have no update on working group at this time although i would like eventually have this structure i think the breakout session this week was really effective and for the time being a reasonable solution anybody has any more comment on it otherwise we can move on 

**James** - yeah the breakout room was great we made a lot of progress on the EIP and we should do more often 

**Pooja** - right for people who could not attend uh there is next breakout meeting on september 14th at 1400 utc uh and uh the eips that were not that we could not discuss in the previous meeting would be continued to bid the 

**Micah** - one point of feedback on the breakouts was maybe this was just me and i misread something i went into the breakout session thinking it was just about 2718. it wasn't until i got there that i realized that it was actually about several things um i don't know if i just misread something or if there's a better way to convey it

**James** - that just emerged into happening because we realized before we talk about what would happen with that transaction envelopes understanding what was in yolo was like important to understanding if we should do the one so that just sort of happened on the call but okay and it wasn't like documented as something right okay 

**Micah** - in that case yeah i'm totally fine with it; i do think the breakout rooms for or breakout sessions for specific topics are better than generalized ones because you're more likely to get people to show up if you're talking about one thing whereas if you say we're gonna talk about what they send things and it's hard to get people to dedicate time 

**James** - yeah i would agree with that as well 

**Pooja** - in the next meeting uh along with 2018 we would be discussing about 29.35 for the consideration in yellow but i'm not sure if people add further in the agenda that is available in ethereum pm and if we get time that might be discussed as well 

# 4. EIP triaging permissions

Video | [35:38](https://youtu.be/UJmYpFkZGzY?t=2138)

**Pooja** - moving on uh the next item is eip triaging permissions um as far as i remember uh light client and hudson were working on it do we have any update on that 

**Hudson** - uh no in fact do we still we still want to do that right light client or do we need to figure out what the triaging would even be for before i give the permission set 

**LightClient** - i think we still want to do it i don't think there's anything to um to figure out i think it's pretty straightforward said a github username and then they have the ability to use the tags that alex has come up with on the repo okay i'm going to go ahead and just invite you and give you that permission set awesome okay we'll see how it works out 

**Pooja** - uh i have a question here related to you know not related to the permission but related to some recent bot changes i see that the bot is now able to figure out what are stale what are the processes i'm going to share a link in the chat and with that we could see all the eips that are still is anybody here that may be able to explain more about it this new process on this new bot

**Micah** - sure it's a just a simple github action that if a pr hasn't been commented on for 60 days or more then currently then it will get the stale tag and the bot will comment on it saying hey this is mathematically if you don't do anything and then i think as soon as anyone comments on that pr then the stale tag is removed and the timer starts over if pr has a stale tag for more than a week then it will be closed automatically by the bot so it's just a mechanism to deal with people who create prs and then get feedback and then never respond to it it'll automatically handle those for us

**Pooja** - that's great and i see that it is not only for a state it also works for many other thing like i see uh it also marks as processes if any eip is for process any is for core and something 

**Micah** - i think those are being done by alex manually someone might correct me if i'm wrong there 

**James** - yeah those are those are done by hand

**Pooja** - okay sorry i i got confused i thought that what is also taking care of this yeah 

**Micah** - i cannot wait for the day when a block can automatically do all that stuff that will be a that'll be a some i don't know what it's called like the computers have taken over singularity 

# 5. Onboard EIP editors survey to set expectations of an EIP Editor

Video | [38:40](https://youtu.be/UJmYpFkZGzY?t=2320)

**Pooja** - right okay anymore anything more in this topic okay moving on the next item on the agenda is on boarding eip editor survey to set expectation of an eip editor i think edson 

**Edson** - uh let me pull that up real quick um we only got three responses from eip editors i can go over the generally what they what they're saying um so the time commitment for new editors ie between is about five hours per week to zero hours per week um in that range the tasks that are expected to do uh make sure the eips are formatted their technically complete uh working with authors to get new eips into the repo looking at grammar structure the meaning uh if it's related to ethereum and uh looking at the auto merger bot if in cases it doesn't handle; good requirements for someone to become an eip editor is to already be helping um so anyone could review eaps editors are only needed to merge and someone that understands the difference between a standard and a good idea someone that understands the content that should go into standard and someone who's a good communicator and understands ethereum at least into an intermediate level and can handle contentious discourse and understands github

**Pooja** - great so by this uh just one point i want to mention it again like by the task that has been suggested by the eip editors they want to focus it on uh if it is ethereum related um i don't know if it brings back to our uh conversation that we had sometimes back on like what would be the eip repository should be for maybe i'm not sure maybe we could have it a separate agenda item in one of the future meetings and then would like to discuss 

**Micah** - it would be nice to settle that it's been ongoing when discussion not just between lightclient and I for the one currently having but also like the other day someone put in something to the eips repo which was a specification for a new cryptographic primitive which um like is very general that's like something you would submit as an rfc to some other standardized body but they chose the ethereum repo is ethereum the ip's repo the right place for that like yes ethereum may use that cryptographic primitive at some point but there are definitely better places in my opinion to get feedback on like cryptography stuff than the ips repo so i think answering what is the scope of the ap's repo cover does it cover just ethereum and stuff that's going into ethereum and stuff that's specific to ethereum or does it cover a more broad scope including stuff that goes into that may or may not go into ethereum but is kind of related to the evm and things that run the evm and does it include like cryptography like which is tangentially related to ethereum so just answering that would be nice at some point it's not a super pressing matter though either

**Hudson** - i have a quick update about the triage permission that we were just talking about um it turns out your are we have a legacy github organization at the ethereum organization in github and we would need to upgrade it which would incur cost in order to get the triage permission um i don't know there's some like pros and cons to doing that so i'm gonna have to go over with the ethereum foundation devops team but for right now we can't do the triage permission but i can talk to them uh we're having a meeting tomorrow about it 

16.1.3 | Video | [42:50](https://youtu.be/UJmYpFkZGzY?t=2570)

    triaging purchasing requires upgrading the ethereum organization github, Hudson is having a meeting to discuss pros and cons

**Lightclient** - okay yeah i guess we'll see what the outcome of that is that's surprising that there's a cost because usually the open source stuff on github is free 

**Hudson** - oh no no it's not it's not that it's a paid feature it's that there is there was a when microsoft got github they had this thing so instead of it being github uh paid uh github paid accounts per repository it's now paid per user and there's different names like enterprise and team and stuff and but the old one is just like github business or github paid or something like that and that's the one we're on the new stuff has new features um whether it's free or paid so because this is a paid account in general uh even though there's aspects that are free and a lot of the repo's are free and open um not all the features can be in there until the whole organization is migrated over to the new type of account 

**Lightclient** - very sneaky okay 

**Hudson** - that's all i had for that one 

# 6. Clarifications for how a precompile address is decided

Video | [43:56](https://youtu.be/UJmYpFkZGzY?t=2636)

**Pooja** - okay so uh the next item here is clarification of how a pre-compile address is decided i think this is something uh james was looking into 

**James** - for which part 

**Pooja** - item number six there is a link in the agenda um 

**Hudson** - we decided this a few meetings ago i think and we just said this doesn't need to be on the eipip agendas anymore because it it's just not a not applicable i guess um to what's on an eip 

**Pooja** - oh okay 

**Hudson** - i think i i could be wrong though we'll see if james wants to keep it 

16.1.4 | Video | [44:52](https://youtu.be/UJmYpFkZGzY?t=2692)

    remove the precompile address discussion from agenda / not applicable to EIPIP

**James** - no that we there was some something i wrote at some point that might make it in somewhere but we don't need to keep talking about it; it was it was it was very far down on the list of a very long list that we're finally getting to

**Pooja** - okay maybe uh like in past a few meetings we could not uh answer that or i just somehow 

**Hudson** - yeah i think it was just because james wasn't here to answer and it was his um comment in the thread that was probably it

# 7. Review action items from previous meeting

Video | [45:35](https://youtu.be/UJmYpFkZGzY?t=2735)

**Pooja** - yeah so yeah that's all on the agenda today do people have anything else to talk about in fact i may have something i somehow came across a list uh not a list a document i think it is originally made by axic uh that talks about some of the problems with eip i'm not sure if people would want to have this in some of the future meetings because i find these are related to the process and that that the group is working towards 

**Hudson** - we should see which ones are still applicable, some of these looks like it's still being decided 

16.3.3 | [problems with EIPs by Axic](https://hackmd.io/issXMJfhSCqvlffu3NHxbA)

**Pooja** - uh last item in there like there are some more issues raised by community it actually marks all the eips that are related to the process of eip1 so that list might be something that we could use to

**Hudson** - got it okay cool yeah we can we can put a few at a time as long as we don't overrun the agenda that'd be nice 

**James** - uh any thoughts on if we're ready to start migrating eip1 to having the new statuses we discussed previously i think we are ready for that 

(people agree)

**Pooja** - so i think uh pierre would be required uh i'm not sure gmc would be taking care of that

**James** - i don't know it's a pr to eip1 i don't know what's the best way to start it i just know let's do it 

**Micah** - i think the the one thing that might still be up in the air is axic proposed changing withdrawn to abandoned and then having in a recent field that's separate since there it turns out there's you know a bunch of reasons why any mp may end up no longer being worked on 

**James** - yeah we my so i read through his comment and we we have discussed this previously in march quite a bit but i we had we also had this discussion on eip calls over us over a couple sessions of calls and i i and i feel like we decided on having those both having the withdrawn and the abandoned and we went through a lot of the reasons why and debated them back and forth pretty a lot so i don't know if it's like going back and doing that all over again is worth it at this point 

**Micah** - i definitely don't think it should hold anything up like whatever gets us to the new statuses quicker i'm a thumbs up on 

**James** - yeah like we even had axe on a call on on one of these multiple times and discussed it among a lot of us and the the decision was to keep both of them.. i'm i'm fine restarting the conversation and saying let's reevaluate but i would not want it to stop the migration of the statuses we should start doing that now and if someone wants to change a status then of course they can propose that and we should talk about it but i don't want to hold anything up 

**Pooja** - so how about like about the implementation of statuses like we should uh take it as one of the decision item here and we already have proposed in the all-coordinate meeting we did not see any you know over my dead body kind of opposition are not the not so welcoming uh comment on that so let's start working on it let's keep it as a part of decision item for now and as we go on populating the new network repository we'll make a pull request to eip1 um adding those statuses 

**James** - i mean why wouldn't we just make a pull request now for that adds to the statuses and then work on migrating the eip repo 

**Pooja** - yeah we can do that too but uh i would be happy if we can also add the network repository there in this pull request i mean just the link 

**James** - the eip and micah that that it's that one but without superseded superseded was retracted

**Micah** - excellent 

**James** - i'm still not totally understanding your suggestion pooja 

**Pooja** - oh no uh i'm proposing that as we discussed a few meetings back like when we are adding something to uh the eip1 we try to make it with new uh statuses eip statuses should be there that's number one and number two we wanted to add about the network upgrade repository now that we have repository and it has actually i mean people have actually started populating it so my suggestion was let's have both of them getting into one pull request 

**James** - um i would i would just do the eip statuses and then um i'm i actually like micah's feedback of should it be in a README or should it be any eip1 i think it's good to consider and i wouldn't want to get the conversation muddled between the two of them by having them both in the same pr

**Pooja** - okay i got your point yeah great 

**Micah** - i would not reject a uh either one of those prs uh readme or EIP1.. just so we don't get this lost is there volunteers for doing either of those things either those pr's um like we have the list of statuses and that is already documented in james's document so if he would like to do that otherwise i can take a stab on that and add it to add a pull request to eip1 

**James** - i can do that and then let's add this as an item but for you and i pooja to go over in our call that we do

**Pooja** - sure we'll we'll take it on our call okay the last item here is um and not the item it's actually the review thing about the previous meeting so i am going uh by the decisions made in the last meeting the first one is bring up eip repository scope and triaging permission in the next meeting we discussed it today number two discuss eip repository scope and triaging permission for if the hard fork coordinator is available i think it's repeated so it's both both of the same thing and we did discuss it today number three wait two weeks to discuss onboarding eip editor survey after receiving survey results uh thank you edson for sharing that with us we we did discuss that as well the last one is wait for james to discuss clarification for how a pre-compiled address is decided if i understand it correct that is not something under the eipip group scope so we are dropping it for our future meeting yep so yeah 

**Micah** - i'm assuming that survey the purpose of the survey was to work on onboarding more eip editors if so what are our next steps for that

**Pooja** - right the initial idea was to collect the feedback from the editors and based on that we are going to define the scope timeline i mean the number of hours required and maybe try to come up with a document which which can be referred as a base document whenever we want to onboard any more new editors so uh i'm not sure uh just checking with you first edson because you have the feedback is it something that you would like to take on 

**Edson** - um doing the onboarding

**Pooja** - uh the document uh on onboarding process like for defining this scope uh the duties in what condition an editor can be onboarded and then what if they want they want to or the uh the group decided that they have to be removed from the position something like that would you like to come up with a document 

16.2.4 | Video | [54:24](https://youtu.be/UJmYpFkZGzY?t=3264)

    Edson to create document outlining the required criteria and procedure for onboarding EIP editors

**Edson** - Yeah i can create a document 

**Pooja** - sounds good thank you so i think we can take it for the next meeting or maybe in a meeting one or two meeting from today we can discuss further on the scope and this document that would help on the process of onboarding eip's editor so yeah that's it for today uh thank you everyone for joining us today and uh see you in two weeks the next call is in on september 23rd at 1500 utc

# Participants

- Chloe
- Hudson Jameson
- Micah
- Brent Allsop
- Lightclient
- Edson Ayllon
- James Hancock
- Jim Bennett
- Alita Moore
- Pooja Ranjan

# Date for Next Meeting: 23 September 2020, at 1500 UTC.
