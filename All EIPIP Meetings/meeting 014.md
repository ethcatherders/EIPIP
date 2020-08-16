# EIPIP Call 14 Notes

### Meeting Date/Time: Wednesday 2020/8/12 at 14:00 UTC
### Meeting Duration:  1 hr
### [GitHub Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/26)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=mkz9eJ3GDTI)
### Moderator: Hudson Jameson
### Notes: Alita Moore

-----------------------------

# Contents

- [1. Network Upgrade Process](#1-Network-Upgrade-Process)   
- [2. Constraining the EIP repository scope](#2-Constraining-the-EIP-repository-scope)   
- [3. Explore the idea of working groups](#3-Explore-the-diea-of-working-groups)    
- [4. New EIP validator](#4-New-EIP-validator)   
- [5. Onboarding EIP editors](#5-Onboarding-EIP-editors)   
- [6. Discussion on Muir Glacier postmortem report PR-2809 and Network upgrade postmortem template PR-2810](#6-Discussion-on-Muir-Glacier-postmortem-report-PR-2809-and-Network-upgrade-postmortem-template-PR-2810)   

----------------------------
# Summary

## Decisions Made:

Decision Item | Description
-|-
**45.1.1** |Revisit the topic on how to handle contentious topics on a later call / with James |
**45.1.2** |Postpone "contraining the EIP repository scope" until next meeting (or until james is present) |
**45.1.3** |summary of lightclient's working group argument:
        the problem is..
            eips are low quality
            lack of incentive to disagree in the eip chain
        a working group is...
            an organized groups that work together on a single topic with a set roadmap of goals
        the working group would impact ethereum by..
            adding a responsible party for mistakes and increasing overall quality
        A good example of a working group..
            is the 1x ethereum group |
**45.1.4** |The survey has been sent out, and awaiting responses |
**45.1.5** |the eth spec repo should have stuff about hardfork coordination, network upgrads, list of eips connected to mainnet, the yellow paper, and postmortems / retrospectives on network upgrades. |
**45.1.6** |Pickup on the yellow paper discussion in the next meeting |

# Action items

Action Item | Description
-|-
**45.2.1** |Hudson and Micah to discuss with the other editors about the working groups idea |
**45.2.2** |Hudson and lightclient to bring the validator to the coredevs for validation before merging to EIP repo |
**45.2.3** |Lightclient to investigate the triaging permissions with Hudson |


# 1. Network Upgrade process
Video | (0:00)[https://youtu.be/mkz9eJ3GDTI]

(Hudson) - all right let's get started on the eipip meeting number 14. the first agenda item is the network upgrade process um we usually talk about that with um james but he's not going to be here today but we do have a note from edson uh a proposal from him for the network upgrade process uh it's in a github gist and a comment at the bottom of the agenda page so um edson if you want to just kind of go through that it looks really interesting feel free to take it away

(Edson) - um should I share my screen 

(Hudson) - yeah that'd be helpful 

(Edson) - all right can you see 

(Hudson) - yes I can 

(Edson) - all right so um I just started a brainstorm a list of statuses i'll start with that um so these are just possible solutions for a hard four coordination process I separated it into two categories like what the statuses are and how to move from one status to the next um these are just ideas something that we can discuss on to see whether we should move forward or not but i'll start with the statuses uh one's eligible for inclusion so this opens the discussion for the hard work uh implementation; the decision to implement them in clients before testing. after the implementation is done they could be motioned to do testing: to have the eip tested to be a test net or just state net tests fuzzing etc or combination of these um once that the next step is staged which is the decision for it to actually go into mainnet which includes deciding what date to put it on so once it's decided both it's included and the date has been set then it's staged; deployed as that date is passed it's live; and rejected is during any of these if it doesn't pass from once that next the EIP is rejected um meaning the EIP isn't going to be eligible for mainnet. any questions about the first one? 

(Brent) - Yeah I'm just wondering does rejected like.. for example i'm imagining um progpow and a lot of people wanted would want something like that to move to reject it but um anyway i'm just wondering what some of the thoughts are how things like that would be determined?

(Edson) - yeah um so for here it's just the status is not really how it's determined but that could be a good way to figure that out oh the next one uh I just simplified it so it's into three sentiment and gathering sentiment from community for the demand of the EIP so this is um should the EIP be implemented first then refinement the EIP is implemented and tested so testing and implementation are in the same step um and then it's done when the spec is final made final and then deployment the time for release is chosen and the eip is released. so it's the same as the previous except um a lot of the statuses are put together it's a three then on stage same as rejected this is stage one stage two stage three on stage eip's withdrawal from consideration into a hard work. Any questions about this one? 

(Hudson) - um these four that you're going through these groups of four.. these are all they're usually not complementary these are options right 

(Edson) - yeah 

(Hudson) - okay perfect 

(Edson) - well I mean you can if you like one from one we get included in another 

(Hudson) - that makes sense yeah yeah definitely mix and match but like for the moment they're separated like it's just this idea stage yeah yeah yeah um yeah yeah go ahead 

(Pooja) - uh no I was uh I was just going to ask like these statuses that you have mentioned here is going to be statuses attached to EIPs right? I mean um similar to like eip process or how we are planning to like um put them in that 

(Edson) - this is for hard fork coordination 

(Pooja) - I get that part but my question here is like an eip that would be undergoing the process of eip in first place and maybe at the same time parallelly it will also be moving across the process of hard fork coordination so the status is that is generally mentioned in the header of an eip are these statistics of hard for coordination would also be added in addition to the eip status or how are we planning to consider this?

(Edson) - uh I think we should have this conversation another time um because I think we already discussed it, right? we weren't gonna include the status and the um in the EIP but maybe included into meta EIP um but we could add another header um specifically for corey

(Pooja) - okay uh um sorry I didn't mean to interrupt and please uh go ahead and maybe at the end of this proposal I would like to uh you know mention my uh like another counter proposal which is like different from statuses where I i prefer to call them as a stages so please first let's continue this; sorry of interruption.

(Edson) - yeah I mean like here I call it stage so instead of statuses stages whatever um it's just kind of uh the steps in the eip process I mean hard fork creation process um so here's the third one eligible estimated here we estimate a schedule for the or we define the scope for the EIP for so how long it looks like you might take um and then develop public review public reviews another synonym for auditing testing final request of changes public review we can have things like auditing I mean it applies stuff like that final approval uh the EIP is frozen it has to be frozen for it to be in final approval and then has to be approved for mainnet final release the ap is live and mainnet and maintenance we monitor the EIP to see if um if it is working as I expected and um yeah for a period of time it might be a couple months or something any questions about that? okay, the next one, eligible algebra for consideration; uh functional satisfying the EIP works as expected; it's implemented; it's working secure there's proof that the EIP poses no security threats meaning it's well tested and deployed status meaning the ap is live on mainnet so these are the things that are updated after each of these so after testing is done then you add that it is secure versus here you're in testing when you start testing you here you're secure after you're done testing functional you're functional after you're done implementing. any questions about that? All right uh what do you think about all of them like compared one to the other?

(Hudson) - I like the first one the best, I think maybe adding maintenance to it would be cool. I would need to think on all of it more though but just my initial reaction is that I like the first grouping

(Alita) - I think that the first two items in the first one could be combined 

(Edson) - any other thoughts?

(Pooja) - I also like the first one more because it is more like in it's closer to the eip process itself but I would prefer calling it a stages to differentiate between the state and stage when we are considering efi however uh I am not as I mentioned my reservation earlier as well like i'm not very much comfortable having it all together in a separate repository but the process-wise number one looks good to me.

(Chloe) - Personally, I think number one looks good as well. With number two having the stages I think it could also be helpful just to know like um like for example what elita was saying about how a number one and two could be uh together so maybe stage one it could be number one and two uh stage two could be like uh testing and staging and then maybe stage three could be deploying or then or rejection would be the other. you know whether or not the option happens but either way I think stage one and then maybe adding the stages in that way 

(Edson) - I guess so it's looking like a combination between the first one and then elements from other ones like maintenance using staging to differentiate how where it is. it would be great if um james was here get his feedback too 

(Hudson) - do we want to save the next part for when james gets back for him to review this and then for us to have a full discussion I only say that because otherwise we might have this whole discussion again the next meeting if he's one of the primary people we need opinions from on this.

(Pooja) - yeah I would agree 

(Hudson) - what do you think, edson ?

(Edson) - yeah I could take the feedback and create a fifth option and then wait until james is here to continue discussing 

(Hudson) - cool and then uh pooja you had something about this though was that like directly related to this did you want to say that now or at the end of the meeting or I think I can share that i'm gonna share a link in the chat itself and if 

(Alita) - so I have a quick um sorry go ahead i'm sorry I didn't mean to interrupt

(Pooja) - so yeah that is just another proposal but maybe in a different from a different perspective like I mentioned that I wanted it to keep it closer towards the network I mean the present eip process so this is again another proposal for network upgrade but in a different format so here I have tried to specify the I mean try to put it in the form of eip it's coming up from the eip that was proposed last year for that time process when we were doing schedule base but now since we have changed the process and we are doing more eip based so i've tried to change the process based on the efi and i'm just anybody has to say something i'm sorry 

(Hudson) - oh no this is good I like that you did this and edson thank you for your document too that's very helpful 

(Brent) - yeah edson could you put a link to that document in the chat I haven't seen that yet 

(Hudson) - it's the last comment in the agenda too if you want to if you need to reference it later 

(Brent) - in the agenda okay cool thanks 

(Hudson) - so um for the document you just posted Pooja um I think um this is a tough one because we're I we created a test repo for putting things and this is something we can just go and delete if we decide we want to change it later but for the moment we did create a repo for uh called eth 1.0 dash specs for specifications like efi and other like a summary of the eips that go into network upgrades and just kind of that sort of thing um so proposing an eip..

(Pooja) - so uh just uh just so I mean like be a little i'm just trying to be a little flexible here uh I have uh actually mark a specific section where i'm talking about github repository and in that in the comment section I have mentioned that if we are planning to have another repo we can put this thing in that repo.

(Hudson) - oh okay okay I i was I was looking at this the wrong way okay that makes sense 

(Pooja) - so uh the process what I was trying to put here is like trying to define the preconditions for the eips to be considered as as an efi so I mentioned to precondition it has to be a core eip and it would not be applicable for any other the statuses can be anything from draft to final because we have seen that there the eips as soon as they enter into the you know as a pr form people have started considering it for efi because we want to be like you know just with the speed to not delay the upgrade because of any particular eip so those are the preconditions and the proposal can be uh I mean like I have I have mentioned these like different stages proposal, socializing, and reviewing of an eip. so one thing that I i was trying to be flexible here is like once uh an eip is created; what I mean here by eip is created is by the pull request that is being created in the eip repo and at the same time. if people want to it to be considered for efi they can go ahead and create an issue, I personally mentioned here as eipip repository but if we have another test repo it can be replaced by the test repo and whatever is suggested here the repository can be changed but my uh thought process was like we should be following the eip numbering process because at the end of the day the eip has to be has to be having a specific number and that is defined by the pull request number that is there in the eip repo. other than the regular processes I have mentioned one another new point here is socializing of an eip like earlier socializing was just by uh you know having a magician thread discuss it in ac getter but there is this new proposal that uh I mentioned in previous cathodes meeting and we would like to have others feedback as well. although I shared it with few editors earlier and we received some good feedback on that it is about a video series on eip where we would discuss some eips; this is because sometimes all core devs author has this thing in mind that a ct call is not good enough to explain the eip and even if we do, it takes uh it takes most of the acd call time and we don't get to explain the eip the way it should be. so having a 30 minutes kind of uh, you know thing for spec dedicated to that eip would be a good reference point and it would be helpful in socializing that eip with community other than that there are some review process steps and I have suggested a tracker board for the stages that I was mentioning earlier like these efi can be tracked with the tracker board my suggestion was for eipip repo but i'm okay with changing it to test repo and the stages that proposed except as uh accepted it's very much similar to what edson has already proposed maybe one or two terms here and there and on top of that mention some conditions in which an eip can be moved from one stage to another if it is under the list of efi so that's the whole process if anybody has any question comment?

(Hudson) - I think this is great um I need to look at it more before I give further feedback 

(Pooja) - yeah sure

(Alita) - Pooja, do you mind uh relinking?

(Pooja) - you want me to share it again on the chat?

(Alita) - yes, thank you.

(Hudson) - okay well looks like we can probably um go on from there. um unless anyone else had any other comments on edson or Pooja's things. I think lightclient had was supposed to come up with ideas 

(Lightclient) - Yeah I was gonna say that you know I spent some time thinking about this and I you know after a little bit I just realized that I don't have enough context and I don't feel like I can really give a good um proposal on how to actually upgrade the network because I think you know it's important to come up with the organizational flow of how this happens and I think you guys have done like a really good job with that but you know that's something that we can definitely come to consensus on some points to me like the most difficult problem. how can we make how can we get for developers to agree on making something happen and how can we have the community buy into some sort of road map for ethereum and to me these are like really difficult problems because um something that you know someone thinks is a good idea a core developer may not think it's a good idea or they don't have the bandwidth to implement and so like my struggle with trying to come up with something is how do we kind of overcome this and I don't really have a good answer to it and I think like really the only things that I can think of is that it's just you know one we need to avoid any sort of chain split at all cost even if you know uh it's I don't I mean I don't know I didn't I don't know how to define a minority that says this is okay to just change split a ten percent of community thinks it's bad. But let's say you know in the instance of prague pow this was something that was just um you know hotly debated amongst the community and so we wanted to avoid a chain split there so I think that was important even if even if people thought the eip was like technically sound and maybe it was good for the network I think it's important because I think that it would be pretty devastating for d5. I don't even know what it means to have a chain split with e5 anymore I think that's like one thing that we really need to avoid and the second is that there are things that are coming in the future that are going to be um that are going to be very contentious like proof of stake and sharding and stateless but to me I think that as long as we have a more formal definition of what like the ethereum roadmap is like what people are buying into then it's okay for us to make these decisions and we don't have something like that written down formally but I think that anyone who's been in the community long enough has been aware that ethereum is moving to proof of stake and if we're going to have a shorty and these are things that will happen on this network and if someone's supposed to change someone splits a chain but this is what they've kind of implicitly agreed upon um by being a part of this network so for those sorts of things like we kind of have this like this we should have a more formal definition of what this roadmap is what our principles of ethereum are that way we can say yes this is a contentious upgrade but this is what you bought into this is what we've been saying we want to do for five years 

(Hudson) - yeah that was kind of like 

(Lightclient) - yeah, I was just wrapping up; that's like really what I had thought about it I think I don't have a good answer I just think that still just you know the summation of the thought that had on that topic 

(Hudson) - okay I guess I really like that direction because it makes it a little bit more clearly defined what the community's values are like you said I don't know if it's in the scope for eipip only because we already have so much on our plate and a lot of the defining whether something the reasoning behind if something should be chain split or to avoid it is something that's more in a procedural and not only not even procedural that's the wrong word it's in a um I guess non-procedural thing where it's like that's decided based on people running nodes and even deeper than that that's decided like a direction on that is decided based on the procedure we don't need a procedure to decide the direction of a chain split I guess is what i'm trying to say does that make sense 

(Lightclient) - yeah I agree I mean I think that this is not something that falls under the authority of the eipip group. I think I don't know how to you know build this collective community roadmap we already have some sort of implicit one but you know to have a little more formal one to point to in the event that we have these contentious network upgrades in the next two to three years 

(Alita) - so one uh idea I would like to throw out there is if we had so okay eipip is focused on the drafting process and then if you had a separate um I think maybe even is what the efi is; i'll be honest i'm not 100% clear on that but if you have a separate process for the actual implementation of something once it's proven to be technically sound, it would be potentially beneficial of the eipip group to define at what point it changes from a drafting process to an implementation process which I think is what you're talking about. 

(Lightclient) - I think the whole network upgrade process is just like completely separate from the drafting process. maybe there's some you know back and forth behavior where we start to implement something and realize that something the eip needs to be updated but to me like everything that's been discussed before this is all about um you know how can we I mean like we're implicitly saying like we have these statuses or these stages and we can just go from stage to stage to stage but i'm just trying to point out that my question is like how do we actually figure out how to go from implementation to you know thing and I don't think that it's right to say just because i've implemented something in every client and it's technically okay that you know we should have some sort of like um some sort of you know very rigorous definition that because I implemented it because it's in these clients we can ship it I think that there needs to be more um I think there needs to be more people uh who are formally defined as you know being accountable for the changes to the network we kind of implicitly have that you know with the go ethereum team but they need to be accountable that these changes are going to be good for the network and they need to have rationale why those changes are good early if they're going to say if they're going to keep us a change they need to have rationale why it's not a good change to the network and these are these are things that like go beyond just you know having stages and you know the organizational flow of it 

(Edson) - so that was the next part I excluded; which, is how  you move from one stage to the next um so that it it should deal with like should eaps get in versus are they typically sound because that's the issue we've been having with the past contentious eips that yes they're technically sound but like yeah is the is it like ethical to include that or is are they is it okay to include from philosophical perspective um is there actual consensus for it to be included so there's no hard fork no chain split I mean um so that's probably something we should consider outside of the statuses but I think having statuses defined or stages defined is a good first step the next step would be how you move from one stage to the next

(Brent) - yeah also just my opinion you guys know my point of view on this but everything light client is talking about is critically important and he's basically talking about building and tracking consensus in the large community at scale and that's exactly what canonizer is designed to do so in other words when an eip comes up someone can start a topic on that eip and it starts out like a petition everyone starts signing the petition and he and if he can prove that there's a lot of people on board with that eip then you know it's not going to be consent contentious and if someone else has a different point of view they can create a competing camp and the community can organize around that the camp statements can change dynamically unlike a petition a petition can't change once the first person signs it but these are designed to be changed and modified and negotiate and build and track consensus and so you can track in a large community how much consensus there is and if you can then basically we it doesn't need to be formalized or defined or anything you can just see yep we have 90 of everyone all and well we have different ways to canonize things you can can I eventually will have the ability to canonize things based on miners based on eip are based on how much people can vote their ether will have quadratic ether canonizer algorithms anyway just my opinion

(Alita) - what i'm hearing is that the general eip drafting process and implementation process could do with a sort of separation between the whole consensus problem as well as the general drafting problem. Which, maybe we should draft up something like for each step; uh, like having a parallel consensus protocol that's being followed. 

(Lightclient) - I think that this is a good conversation maybe we should continue it with james here 

(Hudson) - yeah that's why I keep thinking I wish james was here 

(Lightclient) - yeah i'm happy to box it up right now

(Hudson) - okay, if anyone has a lot of comments we can time box it alita did you have was your point um responded to?

14.1.1 | Video | (30:18)[https://youtu.be/mkz9eJ3GDTI?t=1815]

    Revisit the topic on how to handle contentious topics on a later call / with James

(Alita) - yep!

# 2. Constraining the EIP repository scope

Video | (30:18)[https://youtu.be/mkz9eJ3GDTI?t=1818]

(Hudson) - I did check a message real quick so I wasn't listening. sorry, uh okay, so um next up would be constraining the eip repository scope which we kind of just we kind of were back and forth on that a little bit um 

(Pooja) - yeah I think we can skip that yeah it makes sense to wait for james

14.1.2 | Video | (30:21)[https://youtu.be/mkz9eJ3GDTI?t=1821]

    Postpone "contraining the EIP repository scope" until next meeting (or until james is present)

 (Pooja) - and since lightclient is here so we can go to the next agenda item we would like to use 
 
 (Hudson) - yeah yeah this one is on um uh working groups, exploring the idea of working groups and there is a link if you click on it to um a chart and a comment from light client so yeah i'd like kind if you want to just do a summary of that real quick 
 
 # 3. Explore the diea of working groups
 
 Video | (30:40)[https://youtu.be/mkz9eJ3GDTI?t=1844]

 (Lightclient) - yeah so I guess first before I you know talk about working groups rather than you know coming up with a solution in search of a problem I thought I would share like what I view as some of the things in the eip process and just you know the the repository that I think are problems right now and I think there's like two main ones and the first one is that I think the proposals are generally low quality you know there's a not a lot of effort is put into a lot of these these proposals they're usually hacked together and then it's just kind of left up to editors to guide these people who are really not even that enfranchised into being a part of the process they've just decided to make a pull request in two hours they've written something so they really haven't even read one they don't they're not um they're not trying to make like a really quality technical document I think this creates a cycle where proposals are low quality and so the people involved in the eip process the editors are not incentivized to really take the time to make the proposals better and to really guide those people because um there's just a lot of low quality and so them not being enfranchised to be a part of the more part of the process leads to more low quality so I think that's a that's a cycle that's happening right now on the eip or pod story the second thing is I think that there's not a lot of people who are willing to make you know unpopular decisions in in the eip repository to reach the goals of having higher quality eips or to have more informative eips rather than changes and I think that uh instead you know everything is just accepted in the repository because that's the path of least resistance for for the editors to do and so I think that you know these two together just creating like a situation where the eip repository is not something that people in the community are super proud to be a part of or to uh to have so it you know if we're not proud of the eip repository this isn't you know like a status very strong technical document then less people are like willing to contribute and so we're having this problem where we hardly get people to be editors because this isn't like a prestigious you know role to be playing and I think that we can fix that I feel like working groups I feel like you know adding some sort of additional hierarchy to the eip process would be helpful and to me like I feel like working groups is something that pretty much every standard organization in the world has and it's something that ethereum can implement into the eip repository and so in that comment I just you know shared a couple of just like very you know generic working potential working groups that I think could add value and you know we can you know talk you know all day about you know what how should we structure the working groups what working group should there be like what are their roles and responsibilities at the end of the day I think that you know in order to improve the overall quality we just need to be giving more people ownership of the repository and you know by giving people ownership of the repository we can make them accountable for the changes and so if we have a working if we have a working group around you know the eip process like we kind of have here then you know we need to be held accountable for making the process better we should have some sort of some people who are in charge of um you know the the actual or like um you know infrastructure behind the eip website like what happens if uh we make a change to the continuous integration suite like I made a change uh last week that hudson you you merged and I didn't realize I made a mistake on removing some quotes from a hard fork meta and that caused the titles to be uh to to be erased and so like we change we fixed it in a pr but there's no one who's really accountable as far as I can tell for these sorts of changes you know this is my mistake but there wasn't you know a group of people going through this pr to make sure that it's all sound so I think that having these working groups it and you know we can do this in a very very lightweight way it doesn't have to be very overbearing but just having more people involved in the process and emphasizing them I think that's going to improve the quality overall of the entire you know process
 
 (Hudson) - Yeah I think that's some good thoughts um I think starting small on that is definitely important so having just a few working groups to start on a specific things is kind of a trial and also utilizing github's um triage permission level at the repository uh would be good to start with to get people like used to using the repository and like um i'll put the link in the chat but there's something called a triage level permission set where you can contributors can proactively manage issues and pull requests without right access so that and also there's maintain which is project managers you need to manage the repository without access to sensitive or destructive acts actions so that that'll be nice so that people can't just like sneak in and do a ton of stuff with right privileges at first if we don't trust them or if they need like time to get adjusted 
 
 (Lightclient) - and honestly i'm not even sure if you know the working groups are people who should have write access to the eip repository um they can sure but to me it's almost like they're going to aid the editors if the editor's job is not to technically validate so it shouldn't be to technically validate every eip you know there's so many different aspects of ethereum you can have someone who really understands the evm and it shouldn't be their job to also understand like all the toe different token interfaces in depth and like how they should be working together and I think a great working group would be some sort of interface working group where you have a couple of people who really understand these and they should play a role in commenting on the in the eip repository they don't actually have to have the write permissions but they just need to say hey this is our working group has goals this is our roadmap we wanted to design tokens and that are you know where can you propose does or does not fall kind of like within what we're working on so this is like our feedback for you so I can improve this and the eip editors can come in and see that okay the working group there's comments on us they either I think this is like a go or a no-go I can just go ahead and make sure that everything is like syntactically correct and I can just merge this 
 
 (Hudson) - that's all the comments I had 
 
 (Alita) - so to clarify is your primary suggestion that we have um sort of panels of experts per se uh and or auditors to verify um changes that are made to a certain like category of eip 
 
 (Lightclient) - I think that the way that you describe it there is more of a reactive way and I would rather the eip or the EIP work groups be more of an active playing active role in the process rather than saying welcome to the working group you're going to just review eips that come in I think that they need to actively be playing a role and say this is the working group for interfaces these are our goals as a working group we're going to design eips that meet these goals if other eips from the community come in we're going to be a place that can help give them feedback or help direct them to the right you know to to eips and efforts that are more aligned with what the goals of the network are this isn't stopping anyone from coming up with their own eip and implementing it but I think that there's already this input these implicit working groups there's you know there's different like levels of how like formally defined they are we have the one x working group and they have their sets of goals they're working towards um and so they should they should be being held accountable for that in the eip process I think it's it's weird that you know 1x is such an important upgrade to ethereum but it's not mentioned in the the eip repository anywhere.
 
14.1.3 | Video | (39:03)[https://youtu.be/mkz9eJ3GDTI?t=2343]

    summary of lightclient's working group argument:
        the problem is..
            eips are low quality
            lack of incentive to disagree in the eip chain
        a working group is...
            an organized groups that work together on a single topic with a set roadmap of goals
        the working group would impact ethereum by..
            adding a responsible party for mistakes and increasing overall quality
        A good example of a working group..
            is the 1x ethereum group

 (Hudson) - okay anyone else have comments on that? okay let me find the agenda because I clicked off of it to get to that comment where is it 
 
 (Lightclient) - well I guess my last question is how do how do we make something like this happen how do we I mean you're the only editor I guess mike is here but yeah I don't think he has his voice on so you're really the only editor here who can kind of make these sorts of decisions 
 
 (Hudson) - yeah uh I don't have an answer I wish I did um now that mike is an editor come to me and micah and we can start to relay this idea and maybe if you or someone you know wants to be like the first guinea pig for this type of thing then that would be helpful so if you have if the plan's there and we have someone who could be a guinea pig then we can go to the me and micah can go to the eip editor's channel and pitch the idea I think that's probably the best way to do it 
 
 (Lightclient) - okay i'm happy to be a guinea pig i'll write something a little bit more formal for you 
 
 (Hudson) - it doesn't even have to be too long uh but um yeah just what whatever you want to make it more uh like official that you want to contribute for sure that'd be great 
 
 (Lightclient) - okay thanks oh james showed up hey james 
 
14.2.1 | Video | [40:00](https://youtu.be/mkz9eJ3GDTI?t=2400)

    Hudson and Micah to discuss with the other editors about the working groups idea

 (James) - I did sorry i'm very late I thought it was in 15 minutes 
 
 (Hudson) - no problem um okay standard format uh so which oh one oh i'm on agenda 13. what am I doing my life is a mess okay now i'm back we are we are now going to item number four new eip validator
 
 # 4. New EIP validator
 Video | [40:50](https://youtu.be/mkz9eJ3GDTI?t=2400)

  (Lightclient) - the eip validator was integrated 
  
  (Hudson) - oh congrats thank you light client um here's the validator eippr it's in that comment uh and like client for those who don't know what the eip validator is can you tell us more about what that means and what you accomplished?
  
  (Lightclient) - sure so the EIP validator is part of the system that runs every time you submit a pull request to eip repository and what it does is it's checking to make sure that the eip is syntactically valid so make sure that the ip number is there make sure that the status is one of the known statuses with the categories from the known categories all these things and there's some other things that i'm hoping to add into it like it's going to make sure that all of the uh headers from the eip1 are being respected and these sorts of things so the first version that that was kind of about parody with the old eip validator that was written in ruby this has been merged into the eip repository.
  
  (Hudson) - awesome anyone have comments on that 
  
  (James) - thank you because we've needed that for a long for updated so it is very awesome for you of you to do that
  
  (Hudson) - yeah it's greatly appreciated I have one question while we're on the topic I know that micah had requested that the withdrawn status be added to the validator and I wanted to make sure that we're on the same page of adding that because I know this is kind of mixing the newer statuses with the older statuses 
  
  (Hudson) - um is withdrawn in eip1 I forgot 
  
  (Lightclient) - I don't think it is
  
  (Hudson) - um I don't know then what do other people think
  
  (James) - I think we should uh present the statuses the new ones for the EIP process to the core devs meeting get final approval there and then start adding it to the eip repo 
  
  (Lightclient) - I also think that's probably the best way to do it instead of going and just you know hoping it'll happen
  
  (Hudson) - yeah I guess put a pin in it and we will um come back and pull that pin out later when we talk to the core devs or something 
  
14.2.2 | Video | [43:17](https://youtu.be/mkz9eJ3GDTI?t=2597)

    Hudson and lightclient to bring the validator to the coredevs for validation before merging to EIP repo

(Hudson) - all right anybody else have um anything on that one okay onboarding eip editors

# 5. Onboarding EIP editors
Video | [43:33](https://youtu.be/mkz9eJ3GDTI?t=2613)

(Hudson) - um that would be a survey to set expectations of an eip editor and triaging permissions.. um so the for the survey I think that's edson right

(Edson) - uh survey has been sent out uh we should wait two weeks for the responses 

14.1.4

    The survey has been sent out, and awaiting responses

(Hudson) - and then the triaging permission I alluded to this a little bit ago with my get my github link that I posted um but there are permissions we need to explore when onboarding new editors to get like junior editors to um have like the triaging permission or a lower permission than write privilege in order to kind of get up to speed on eips and monitor them and stuff like that 

(Lightclient) - i'm also happy to give me take that if you need someone to make sure it's working okay 

(Hudson) - awesome yeah that'd be cool um let me make a note of that real quick um lightclient.. cool I will talk to the other editors about that okay so the next item is discussion on mere glacier postmortem report pr2809 and network upgrade post mortem template pr2810

14.2.3

    Lightclient to investigate the triaging permissions with Hudson

# 6. Discussion on Muir Glacier postmortem report PR-2809 and Network upgrade postmortem template PR-2810
Video | [44:59](https://youtu.be/mkz9eJ3GDTI?t=2699)

 (Hudson) - um those are both in the eips repo I think that's pooja on both of those um 
 
 (Pooja) - yeah I don't have much update on that other than that thank you to light client and micah for at least resolving vbr past bots for that and i'm happy to move the pr I mean and close or reopen or whatever is required in the future to get this listed somewhere as an informational eip 
 
 (Hudson) - cool and if we do ever move a lot of the stuff to a new repo would we just move this one as well or 
 
 (James) - uh I would think the postmortems and launches stuff should go in that should go on the new repo 
 
 (Hudson) - yeah um and we should actually talk more about that because I want to make sure everyone's on the same page the repo was created I don't know if we ever fully decided as a group what goes in there so my understanding was that things that involved efi like updates to efi and also um reports on network upgrades so I guess these postmortems would count in that would go into that new repo but what do people think is that a good idea or 
 
 (James) - i'd agree but i'd also be interested in hearing more from you guys 
 
 (Hudson) - yeah because they're eips right they're informational eips that pooja has worked on and I wouldn't want to merge this and then suddenly move it or move it and then want to bring it back or anything like that 
 
 (Pooja) - just one concern that I have mentioned earlier about the about the storage format like if we are planning to store it in form of eip if not then it is fine with me uh because i'm not sure if we decided on the format of it and if we are planning to decide it in some of the EIP format I am concerned about the number system for this
 
 (Hudson) - ah yes I see so that might need to be that can actually be decided between you and james and anyone else who wants to be in that discussion outside of the call the numbering system because if that's solved and then we can move it out of the eip repo that would make it so that there are less eips in the repo that have to be dealt with by editors and they can move to that new repository that's just dealt with by james and whoever else is you know admins in that repository the new one 
 
 (james) - and I i even though we're moving eips over I don't think they I don't imagine them being moved as in the same format or as eips because we have an opportunity to optimize the format for the specific case of what we're doing outside of the eip process like I think a lot of what we've done is somewhat uh like held in at least by formatting and content by the limits of the eip process previously so we have an opportunity to make it to improve on that and then micah had also said in chat that uh he suggests I want everything that is specific to maintenance to be in that new repository mainnet and ethereum operations such as coordination etc
 
 (Hudson) - that's that's a good point micah what we ended up doing and I think I might have posted this before you got here but where is it um oh maybe I didn't post it but there is a repository for eth 1.0 specs right now and the reason we're calling it that if you go to ethereum and i'll also post this link and you type in the word specs and search uh so if you um do this second link I posted you'll see all the specs there's eth 2.0 specs stateless ethereum specs and then eth 1.0 specs and i'm hoping that 1.0 and 2.0 will get merged at some point but um i'm not positive that'll happen immediately and I think there's someone outside i'm going to check on that real quick i'll be back y'all can continue 
 
 (Pooja) - so if I understand it correct um unlike for this these instead I will be using it as network upgrade or maybe uh retrast retrospective that we decided in the previous meeting uh like retrospective report dot md am I correct to understand this 
 
 (James) - uh I'm not totally.. I mean you're you're right that it will be different i'm not totally sure what it will be yet I think we should take some time and it'd be great to get uh in the issues on the repo if you have I idea this that would be a good place to add the network upgrade suggestions or other sorts of things for how to handle this movie forward I don't know what it will look like immediately but it will be something I hope different 
 
 (Pooja) - got it thank you I just want to make a comment I don't know how much you guys talked about the naming convention here but I think that you know each 1.0 specs is very different from these 2.0 specs repository unless someone is planning to go back in and and rewrite the yellow paper in some sort of spec format it seems uh it's kind of weird to use that as a coordination repo
 
 (Alita) - um so I was actually planning on editing the yellow papers uh is that something that you wanted to coordinate offline 
 
 (Lightclient) - uh I mean I guess I just think that the uh the yellow paper should probably live in eth 1.0 specs now because the east 2.0 spectrum repository has all the specifications required to implement these two clients but for eth one we don't necessarily have that that's kind of the most of the yellow paper 
 
 (James) - I like having everything that you need to write in each one client be in eth one specs and that would include all of the a list of all of the eips that are currently active on mainnet and the yellow paper 
 
 (Lightclient) - I guess you know the weird thing is that the eth two specs repository doesn't you know they don't have the concept of eips the item so I don't know what the proper way of like integrating the idea of incremental changes like that that need to be backwards compatible to a specs repo I think this is mostly like shutting at this point but i'm just trying to say that if we're gonna have a spec repo it should probably all be all inclusive including the yellow paper 
 
 (James) - i'm fine with that and eth2 hasn't figured out how they'll update the spec I they haven't had a vips ii eth2 quote-unquote yet so they're on the other side of this for us but uh that but that didn't really make much sense but yeah I would agree that it should be inclusive of things like the the current state of ethereum and all you need to do to do a client 
 
 14.1.5 | Video | [53:40](https://youtu.be/mkz9eJ3GDTI?t=3220)

    the eth spec repo should have stuff about hardfork coordination, network upgrads, list of eips connected to mainnet, the yellow paper, and postmortems / retrospectives on network upgrades.

 (James) - so just to review if we take the stuff we've talked about being on the on the eth specs repo it would be hard fork coordination, network upgrades, eips that are list like a list of vips that are connected to mainnet, the yellow paper, and postmortems and retrospectives on network upgrades, 
 
 (Hudson) - hmm by the way i'm back hey 
 
 (james) - lightclient suggested that we also do the yellow paper if we're if it's going to be in ethereum specs that it should be inclusive of all things that require to make a client including the yellow 
 
 (Hudson) - maybe.. it'd be kind of weird to move it from its current repo but like coordination for updating the yellow paper could definitely go in the eth1 specs repo as my thinking initially 
 
 (Lightclient) - I guess my thinking was just looking at how eth two-spec repo is modeled and everything in eth two specs repo essentially defines how to write eth two clients so if we have eth one o specs repo where it only has some like new upgrades that seems like it doesn't follow the you know
 
 (Hudson) - for this one it doesn't have to because eth 2.0 had the the benefit of being able to start fresh whereas our stuff um you know has a lot of baggage from other repos and a lot of history so like moving like the light client the yellow paper file out of the old repo would erase all of that previous pull requests that people have to reference and you know branches and things like that for different like byzantium upgrade and stuff like that so i'm just i'm more worried about the collateral damage of moving the file itself into the repo but referencing it from the repo I think would be appropriate 
 
 (Lightclient) - yeah I mean we can figure out whatever the right way to do it is I just don't think that you know baggage should stop us from making a cohesive spec presence 
 
 (Hudson) - yeah of course and we would we would definitely put like yellow paper as a part of this go here to look at the yellow paper and go here to coordinate it kind of a thing like direct people on the read me that's more what I was thinking but if you had something more in depth then we can definitely see about that 
 
 (Lightclient) - I mean in the ideal world someone would rewrite the yellow paper and the same sort of format the pythonic format that these two spec is in but you know that's a huge task 
 
 (Hudson) - that'd be awesome though you're right 
 
 (James) - that'd be so cool 
 
 (Hudson) - uh okay I think we're out of time actually so we might wrap this up here um um for now let's let's pick up on the yellow paper talk for next time
 
 14.1.6 | Video | [57:20](https://youtu.be/mkz9eJ3GDTI?t=3440)

    Pickup on the yellow paper discussion in the next meeting

  (Hudson) - or in the chat and were there any final things people wanted to throw out since we didn't get through much of the agenda before we go that would you know they've been waiting to get an update on or wanted some feedback on before we go 
  
  (James) - uh feel free to make issues in the specs repo about the specs repo or suggestions and things like that that'll be a place where discussion can start happening around it
  
  (Hudson) - all right hey thanks everyone a lot of good stuff was brought uh here today i'm i'm really really happy about the progress uh see y'all in two weeks


# Attendees
- Alita Moore
- Hudson Jameson
- Pooja
- Brent Allsop
- Lightclient
- Jaye Harril
- Chloe
- Edson Ayllon
- Mallach
- James

# Next Meeting Date/Time
Wednesday, August 26th, 2020
