# EIP	 Improvement process call #33 Notes

Meeting Date/Time: Wednesday, May 19, 2021, at 15:00 UTC

Meeting duration: 1 hr

[Audio/video of the 
meeting](https://youtu.be/BJ7X3csL9vc)

[Agenda](https://github.com/ethere-cat-herders/EIPIP/issues/69)

   Moderator: Pooja Ranjan


   Notes: Darkfire-rain

## Summary
### Decisions Made

   Progress on Eip github repo bot still need work on some actions 

## 1. Statements regarding trademarks (0:00)
**Pooja:** welcome to eipip meeting 33 i'm pooja ranjan so the first item on the agenda is statements regarding trademark i have added this item from the last meeting there was some discussion this is in continuation to that wondering if there is any word on it and another question is should it be on the agenda anymore so i i don't see tim here but micah light client if you guys have any word on that

**Micah:** i do not have any insight beyond what's in the discussion on the api belief

## Should external links be allowed in eips? (1:45) 

**Pooja:** right okay.  so i'll keep it open  if we get something by the end of this meeting today that's fine and if we don't have to put it on the agenda anymore i'll remove it so let's move on the next item should external link be allowed in the eip so this has been coming up here and there and in some cases of eip as well as in some cases of ercs because we have active editors in this meeting it will be good to hear some thoughts that may be helpful for authors who are pushing proposals like when we are talking about external inc or what is the definition that we want to put in that's nber one and nber two if there is any reference link would that be referencing things client implementation i'm referring to particularly would that be counted as an external link as well

**Micah:** so  so that just for some back stories in case someone's watching this afterwards the eip editors there's very few of us and we're very resource constrained so time constrained and it's very easy to implement rules that are very strict such as no external links that's an easy rule if you see an external link you just say no whereas external links that are the other the other two options are just allow all external links the problem with that is is we found that people often use eips as a form of advertising sort of where they have a product they're trying to build and they create an eip that defines their product and then they link to their product over and over and over in their in eip and so if we allow all external links we
end up with a nber of vips that end up have following that pattern and there's a worry at least for me that if we continue to allow that behavior then we're going to get going to get
Overrun by these people that are looking to advertise and in the middle ground of course is to
use some sort of judgment like the editors would use judgment say okay this is an acceptable
link that's not an acceptable link the problem with that one is due to the limited resource available to eip editors time wise it's very very time consing to do case-by-case judgments like that for one because just just the mental effort of making a judgment is hard they have following you have to see what it goes to you know try to gauge what's the quality of the sources and then on top of that you have to deal with people to say well you let someone else
include an external link why can't i have my external link and you have to fight people on it  so historically i've been going with the just no external links rule and i was very rigid on it and just said if there's an external link not allowed one exception the one exception i've let through is rfc links so rfcs are a standard by another standard standards organization and they are very stable over time they've shown throughout history like they've lasted decades and we already have them all over the place in the afp's repo recently though there's been a lot of
pushback on that and so i think the culmination of all that pushback is we're going to go
with the other option which is to let editors put whatever they want in their eips and we'll just see how bad it gets we have some long-term ideas for how to address that problem like such as switching eips repo like getting rid of it or getting rid of four eips in favor of a concrete specification that is updated via pull requests  in such situations there's much less room for people to put external links and they make much less sense and so this problem might just go away on its own if we can ever achieve that it's also possible that my fears will not be borne out and there will be a handful of people that use eips for advertising but they'll be few and far between so i think unless someone feels otherwise i think that's more or less where we're at

**Pooja:** so when you say for advertising i mean i am considering that is not the case with the poor proposal that in case of erc's right so can we have a kind of fine line between
the eips and ercs here like when we are talking about ethere client implementation we can
have certain rules and we can define the external links over there and when we are talking about erc's kind of proposals then we we may or may not allow the link from the particular github repository i mean if that's that's just a proposal what do other editors think on them 

## 3. ERCs (5:30)

### Progress on making a repo   (5:30)
**Micah:** so once we get erc's and eips split apart then i start caring far less about what the erc's repo does and i'm totally fine with a separate set of rules there as long as they're
kind of together it feels easier to have one set of rules rather than have a step two sets of rules in the past we've had kind of separate rules for ercs versus eips and it led to a lot of confusion for users because you had this kind of branching like okay if you're this kind of vip then you need to follow these rules if you're this kind of vip and follow those rules and we have strived to kind of condense those into one path like the whole thing with having draft review last call final we used to have that branch a lot more based on the ip type and i think that just led to a lot of confusion for users and so i have a weak preference for not having different rules until we have the systems actually split apart which hopefully is soon but i can  could be convinced away from that if other people feel strongly

**Edson:**   i think there should be some sort of consistency so if we do start branching off we should really think about the intention behind it and the benefit there would be versu keeping things unified

### Erc editors (6:45)

**Hudson:** i think there should be flexibility that the eip editors can pick and choose
which links to do but i i do hear the concern about the time constraints so i don't think we should declare that right now i think if we get More once the eip and erc repos are split apart and once we've hired more eip and erc editors then i think it would be good to say the eip or erc editors whichever rule sets they have can define if something's being too much advertisy or if something is  the link is not applicable to an eip or an erc i think giving that that structure that's kind of in my opinion kind of part of the scope of an eip editor is to
make sure it's you know the specs are clean and don't deviate too far from necessary links

**Edson:** i think in general links can bring utility obviously they could put links in the discussion to selection but those get lost  yeah i mean it would have utility in the in the case where someone is has done external research this is the one included in the ap to blow it and they just link to it as a reference like  i think having evidence like additional evidence to
uh support an eip is beneficial like you said having  just links that are advertisements or product i don't think that's desirable for the aps repo so i like i can see the benefit of it but
i do think that it needs some policing that makes sense

**Hudson:** i guess one example that i think of is like an erc to say we want to improve erc we want to improve the token standard erc20 so i need to link to these four papers that talk about quote attacks on erc20 like where would that fall micah would that be because that sounds like something that would be justification within the eip for the eip or the sorry for the erc to get
Approved

**Micah:** so i tell people one of two things or both usually one is that the eips are specifications and standards this is not the right they're not the right place to argue a point so like when you define a standard you say okay these are the rules somewhere else you can convince someone you should follow rules a instead of rules be  and this is kind of just the just the rules bit not the argents  the motivation section obviously speaks against this  and i'm and often the motivation section is where the most conflict comes in is because people want to use the motivation section for like a to put forth like a big argent for why this should happen and my personal opinion is for a standard repo  that's not really this not really appropriate place to argue for your thing the standard repo's job is to define a thing not to say whether the thing is good or bad or to assign more moral value to it it's just to define it
and that being said a lot of people want to use the ap's eip process for more than just standardization they want to use it for like consensus building and discussion and argents
and you know putting forth the why and i think that's where a lot of the conflict comes from is the question of is the ips repo a standard repo like is it just a place to store standards and
Specifications or is this a place for like kind of more broad discussion and more broad
like information storage if that makes Sense

**Lightclient:** i feel like one of the reasons that that is so prevalent is it there isn't a great way of building consensus and arguing for standards outside of the eve yes there's the discussion to form but you can have the same you can have different people ask the same question you know every month and you have hundreds of posts to go through it's not really the latest and greatest of the thinking of the author and there's no good mechanism to have that and so
it's kind of the only it's you know i i feel like in her ideal world there would be no motivation it would be purely a spec and there would be a group of people working on the
standardization i want to think about ercs mainly because i think that eips we kind of already have that for court heaps this is a bit of an all-core devs call we have general agendas of things that we want and so there's a lot of work on the specification outside of it there's
i think a lot less need for the motivation but for ercs there's no group that's sort of thinking what does the community need in terms of standards that's going to improve the interoperability and make ethere better it's just mainly projects who think oh i need to extend nfts in this way for my project maybe other people benefit from that let me
throw in 15 links to my project

**Brent:** yeah you guys are talking about consensus building that's exact
and having smaries of all the discussions that going onand tracking the people's latest greatest current thought that's exactly What canonizer is kind of designed to do you create a camp that's a petition that you want to build consensus around and people that agree with you can like basically sign the petition and the petition can constantly improve and anyone who disagrees with that can create a competing camp and all of that kind of stuff is designed to be handled at canada just fyi 

### Erc editors
**Hudson:** so have you discussed with some of the eip authors about using canonizer

**Brent:** yeah a little bit and i've been trying to reach out and recruit them to help do that but they just think i'm  just shilling my our product and stuff like that it's hard to communicate that canonizer can do that and that's what canonizer is for it's a consensus building and
tracking tool but got it okay but but i feel like it's More

Lightclient: i feel like it's more than just building consensus it's it's to me that's the approach right now is more reactive you know people come out and they say hey maybe this is a good standard and then everybody reacts to standard to try and say oh is this good or bad
where i think we need i'm talking again about erc's i think things need to be more proactive
in terms of ercs these are things that we think in the future you know some group of people who do a lot of smart contract development these are things that we think can improve interoperability let's work together and try and build standards around this rather than and there always needs to be an avenue for outside submissions and this is exactly how rfcs work
generally there's groups of people who are working together on standards that's going to improve improve the internet improve software in general and there's always
the ability for outsiders to submit things and then once that circle and work together and we kind of have that with core eaps there's clearly this all core devs call that's happening every two weeks and there's core developers who are thinking you know what in terms of where we want to go with the core protocol what sort of use do we need okay well there's a ddos attack that's possible we want to go to stateless so let's introduce access list of these things and
build leaps around that and that makes sense but we have nothing like that for er cs
there's no group of people thinking hey you know we really need to build out this erc 721 standard this is really big and important let's work together and figure out how to do that

**Pooja:**  i think we we went a little like on the other item of the agenda so let's first conclude this one and then we'll go to the ercs in general that is listed as the next item so if i understand correct as for now the general consensus is around let
 they would want to add in the proposal for both eids and erc when we have a separate process set for erc if and then then maybe we will discuss on that part but for now it seems like we are in consensus to allow them to put whatever in the proposal even i was looking into eip one it says that you know  like i if i may read each efp that is referenced in an it must be accompanied by a relative link for the first time if it is referenced and may be accompanied by a link on subsequent references so i don't see any hard and fast rule mentioned in there as such and i hope people are in agreement to let it be like that  if i'm missing on anything please  correct me

**Hudson:** that sounds right to me i i just wanted to add at the end though that as we hire on eip and erc editors getting their opinion and getting their bandwidth and  seeing how they want to do this i think it's a good thing to revisit in the future  so it doesn't have to be something that's like in stone

**Pooja:** right yeah obviously so yeah my main like  intent here was to get some clarity here so there is no change whatever is mentioned here as  eip1 as of now and we will revisit
on this topic later on so moving on the next item on the agenda is erc so we have been discussing this erc and erp this is on the agenda for past few meetings and there are a lot of back and forth all these discussions can be found on the issue that is a link is provided in the item as for the last meeting we were discussing to reach to the right person to comments there could be some new options that can be explored so yeah i'm opening the floor for anyone who would like to speak to this i i saw some comments from a latest comment from lifeline that you had some different thoughts maybe you would want to

**Lightclient:** yeah i was just thinking in turn i hadn't really thought about it in this way before but if we move to becoming more spec driven and and for the core development then i think that's going to mostly remove the need for each for core eeps and so then at that point you know what is the eip repository doing and so i was thinking maybe it doesn't make sense to split out the erc's at that point maybe it makes sense to just let the er erc sort of take over the eip repository because otherwise we risk you know splitting out ercs and then Moving to spectr and development without eips and now we're re directing everyone who wants to look at ercs to a different repo i think that's going to be problematic

**Micah:** i agree with the caveat that my my caveat only on the time frames so i'm concerned that we might not actually move to spec driven core development for you
know three to five years and we're good means we're suffering with erc eip combination for three to five years or however long it takes

**Lightclient:** yeah i i i just don't know how long it's going to take to to have some service back i wish that there was a way that that could be prioritized

**MIcah**: yeah i think there are people who hire Someone

**Lightclient:**  yeah i mean i you know we have a full ethere implementation in python the trinity client and it's really a matter of removing the software engineering from it to make it a great client and then making it into more of a very readable format for specification and i would love to move to the future where we don't have a front we don't fracture this the consensus test across multiple repos we just have you know the ethernet specs repo we have a testing folder and that has all the test vectors because i think the e2 has really done a great job with how they have written the spec as code and they have the test vectors in the same repo that they can actually run against the spec and if we can get to that point that's going to be huge

**Micah:**   yeah i agree with the the trajectory i think that started the trinity client is very reasonable because it's probably the closest client to something that's written that is what we want  but i suspect there's still a whole lot of work to take out all the optimizations
basically we're basically saying trinity and make it not work as an actual why there's in favor of readability

**Tim:** yeah there's two many i think i've been chatting with different people about this over the past few months there's like two Approaches you can do one is you take trinity and
you simplify it and then the other approach is you take the yellow paper and you transcribe it in python or you know some readable like yeah like or you don't need to transcribe it line but you know you kind of rewrite the yellow paper in python mu you know i i think the challenge for either of those is finding people who want to do that one and two who whose purpose
is to actually help with the kind of eip and eth1 specs process so there's some folks who are
you know looking at rewriting the yellow paper for example but they're more interested in just analysis and and not necessarily the eip process  yeah there's and there's obviously kind of the the trinity team who has written the python client but i don't think they're interested in kind of adopting it to be more respect  if anyone knows like an engineer who would like to make that kind of their focus like write a python spec for ethere either based on trinity or
on the yellow paper  yeah i i i can probably help coordinate funding you're you know like getting some reviews on it and whatnot but it seems like finding a person who wants to do this work who has the skill to do it and whose main motivation is the eip process and not like some tangent where it might end up being useful to the eip process no so i think yeah he's he's looking at kind of rewriting the yellow paper in python  but he wants to stick to the yellow paper as closely as possible  so i you know the okay the two options are you know we wait for paul's work we see you know how how close or far that is from from what we do and maybe it's quite easy to refactor that  then the other option is you take trinity and you just start from that  but yeah i i i suspect paul's direction is like coordinated with what we want but it's not the exact same thing yeah  yeah

**Lightclient:** i might float this idea with some people depending i'm curious to see what
the the apprenticeship program yields in terms of people because i'm seeing a wide range some people are saying they have 10 years of experience software Engineering and they're kind of newer to ethere and so they might have there might be some people who have good python skills and goals yeah back and forth implementing in a simple way where you don't need to do because you know a lot of ethere isn't the most complicated thing in the world but i think that especially when it comes to how to layout the database and efficiently do a lot of things it becomes problematic and they don't have to do that it might be an interesting project yeah
 
  **Tim:** that's true  yeah that's so i thinki can keep an eye on what they're up to
yeah did you make sense at all you work with in the same office as piper right now right  yeah yeah that would be that would be really valuable if somebody from that batch would get on it and it might be also like a slightly so one of piper's concerns with that program is you know like how much people can like actually help these you know onboard new people to the to the process but this feels like it might be kind of distinct enough from like core development that you if we can get different folks to help with reviews and whatnot

**Pooja:** so coming back to the question here how when what is the time period that we
see here with this migration considering we get people to write aspects for ethere and we will eventually move on to the you know pr based system that we are talking about if we talk about this eips and erc how how long is the period that we think that switch is going to
happen like if it is more than a year  in my mind it's worth considering have a separate repo
if that is a kind of issue for many people but if it is like less than that then we can let it be what do people think on this

**MIcah:** i think that if we had someone on staff right now who was a competence engineer knows python understands eap or ethere protocol i'd say six months before for a full migration more realistically probably much longer because we need to find someone and the person they find there's a good chance they will either not to be an expert at python or not be an expert at ethere probably the latter and so a lot to learn on the way and then  so i
would asse like optimistically like a year pessimistically three he's all random guesses 

**Tim:** yeah i a year is my i'd say realistic estimate like the time that we do it you know i can see everything goes well and we have you know like a and drafted it by the end of the smer be like the the the distance between eighty percent done and 100 done is probably another couple months and then kind of switching the process over is probably another couple months  and then you know cordes will be busy with the merge in the meantime so  yeah i i think a year is like things go reasonably well  yeah three i don't know three years to be
seen almost like we just don't do it right like i yeah 

**Pooja;** so considering a year like do we like have the need of erc
People as of now is the question that we might want to answer here because if they do then we would want to progress in that direction getting a rep created and like process set up

**Micah:** i'm weakly in favor still of splitting them out just because of the uncertainty

**Lightclient:** i think i'm i've walked back a little bit and i i would rather wait a few months
And see if anything begins to materialize because i would hate to get down that path
where there's clearly an end in sight and we've already done quite a bit of work to
move and redirect things i don't i don't really think there's a huge benefit of
going three to six more months with erc's out of the repository versus in

**Pooja:**  yeah i think for the time being i mean if this is like general agreement then
for the time being we can start using making use of obviously the tags available in
github although it's not gonna help us with the notifications that we are receiving but
that would be something we can look into and work for the time being and if people would like to revisit it after some time

**Micah:**  we need to hire a tiebreaker someone who's not like client or me

**Pooja:** if we want to push a thing we need to have a champion for that like if we want to have an erc repo we want to have a maintainer of that repo and like we need to have people owning the responsibility if the task can be done being an eap i mean having it in the eip repo and that can be managed is fine but if we have someone pushing it then in my mind it will make sense to move in the direction even if we start looking for people who can actually create a repo and we do not have any maintainer that would be again an issue at the end of the day


**Hudson:**  yeah i think not having any rc editor right now that would kind of be a weird reason to start the move before we have any rc editor right

**Micah:**  well it's kind of making it official that we don't have any rc orders we already don't have any rc editor it's just they currently just sit as opi our yeah

**Hudson:** Yeah i don't have an opinion otherwise i'd be the tiebreaker this time but yeah i don't have an opinion

**Lightclient:** i don't think this decision should stop us from continuing to search for people to
become part of the erc process and i'm happy when we find people to do that to help work with them to you know get them in a place where they can do it all on their own i just i'm not going to be a great eoc editor because i don't write smart contracts and i don't interact With things in the dap level

**Hudson:** well the good news is we are exploring funding options pooja and i and we've made a lot of progress on that i don't think that's in the agenda and i don't know how much we want to say yet about where we're getting funding but we're what's it's moving along

**William:** cool yeah actually in a similar thing the reason why i joined today is  i've been doing some work with magicians and  the idea was floated to maybe have me move towards the rsd editing so  i came in a bit late i missed a bunch of the conversation but it sounds like that would be really relevant right now  i like this is like a really really really fresh idea it's not really scoped out in any way shape or form but if there's any information i could offer with that i'd be happy to you might smart contact someone reading that yeah i do i do write smart contracts

**Hudson:** oh cool okay yeah you've told me that before i don't know why i asked again
but i guess if everyone else didn't know yeah the smart contracts so  if that's the case i'd be okay with you being like a and training editor if you decide to go that path i'd be in favor oh cool

**Lightclient:** i mean i can't say i have like the best grasp of like exactly what would be in
Scope as an editor also so like i mean i definitely am not looking for any kind of streamlined decision process on that just it'd probably be good if i signaled that there might be something like that like you know living

**Pooja:** so  yeah i see and it's comment on that issue proposing william to be an erc editor and i have also received a couple of more interest on the ech discord people mentioning that they are interested to contribute as eip and erc editors  we will keep looking into this
like as i always mentioned it to people that the best place to start with will be the eip
github repo and   as like can't also mention that if they have any questions it would be i mean like he is available you can always go and ask for that but the question that we started with is still here do we need a repo at this point should we think about it or should we drop it considering erc editor is a second thing that they will keep doing it in parliament

Micah: all right go ahead i was gonna say i've won several recent bouts against that so i'm
okay with losing this one 

**Light client:** my ego thanks you

**Micah:** you're welcome 

### Open issues being used as standards erc-223

**Pooja:** thank you i mean i i wanted to have a clarity on this part because many things like are dependent on it so if we are clear that we are gonna have these things like as it is for
now and maybe we would revisit it after three months then we can start looking into it
but again this is one thing that we were looking into another point that was mentioned today
and it is like a very important the process of erc there are a lot of things that's not like streamlined people are not getting proper attention there is something that we might want to do in that direction as for now eip one is the reference for both eips and ercs maybe we would want to add some more text focus on erc that would be helpful for people to follow along
 having said that i have listed a erc standard of in the like sub item it's eic223 that is
an open issue i did not i could not find any pull request for that but i find that is being used as a standard for many other projects and many other proposals this is a situation that i don't know how we we should handle that if a proposal which is not and not listed on eips.ethere.com should we call them as an erc or should we not because i think the clarification on usage of terms is also important for people to understand what is a standard
for ethere and what is just any issue that is randomly moving around
	
**Lightclient:** i think things that define specifications that the application layer should be referred to as erc https://github.com/ethere-cat-herders/EIPIP/issues/69

**Pooja:** do we want to wait for any  standard to follow the standardization process that was defined i think  nine months or so ago like this is the process that every proposal has to undergo eips and ercs to be called as a standard and when that is added as in a standard
it is available for community to use although community can use even if it is in the form of pull request or issue but it's i feel it's important that we should give some clarity to them when we are actually calling it as a standard because i don't want that people should write something in their own report that i have seen an example that that is there in their personality and they are calling it yeah this business

**Lightclient:** so i tell people that until you reach final you are not a standard you're just
An idea for a standard  and the reason for that is because we've frequently run into this
problem in the past of people going out and implementing things before the standardization process finishes  erc20 being the canonical example of that where you know we had th ico boom and 10 million tokens were created on the erc20 standard before it was finished and  we all regret it now because the erc20 standard is terrible because it was just like a first draft basically and then everyone implemented the first draft and then people came and reviewed it we're like hey this is not good we have these problems this problem this problem this problem we need all these other features and this is not great but we're stuck with it and so i try to strongly encourage people don't go implementing these yeah like just because something's in the eip repo implement it like it has not been reviewed it has not been vetted there's not agreement on it until it reaches final  of course i can't stop people from doing things that
are bad ideas so it still happens Anyways

**Gary:**  yeah i i mean i agree i just feel like we need you know more leadership and more
authority around the erc process because they're it's really just a free-for-all at the moment and there's no cohesive plan or goals to move to and to things that or like people want to address if we had a strong leadership group who was helping shepherd standards and the erc20 standard there's two ways to go about it one you can do things you know slightly more
closed source that way you don't even have the issue of people seeing what these standards
are before they reach a more thought out position obviously there's issues with this and you know we could still do it in the open but just not have it become even a draft drc until it gets to a point where some people within this group have seen it and have done some betting on it that way we can kind of avoid some of these scenarios where people just implement the first draft or we can just keep doing as is and i think we're going to keep running into the same issues that we ran into the past where people put whatever they want out there and we have very fractured ecosystem of interface standards


**Edson:** yeah i mean i think generally there's been pushback against anything closed
Source when it comes to ethere at least that's my understanding from their earlier
all-chord eps calls before ours became consistently streamed another thing is say the committee of erc people reviewing your c's i think we should start off with just having erc editors and as there becomes more erc editors they can be the committee because we don't have like core developers that are separate from eIp editors right now the only people reviewing them are the erc editors which apparently we we don't Have any  so i think we should start off there and then if they want to do their own call that's that's on them adding
bandwidth to themselves but

**Lightclient**: the issue is that being an editor is very different from being you know a person who's helping try and shepherd and lead standards just being an editor is just doing doing editorial tasks these are things that most people can do is just a little bit of training saying this is what an eap is what it isn't whereas looking for people to come in and say here are the problems that we se interacting with applications in ethere here are some ideas of
standards that we should try and flesh out to improve that and you know it's been six years of ercs and we still don't really have any people who are kind of coming forward so i think it's
sort of on us to try and help facilitate and build that out because it doesn't appear to be naturally occurring 

**Edson**: yeah in that case i think the easiest way is to have funding for that kind of
Initiative and then seek out people that are willing to do that

**Micah**: i think what you want is basically like platform architects more or less

**Lightclient** yeah the issue is that i don't think that money is something that's going to
do any good particularly for earthy editors since they could easily just write the next hot token
and you know make a few million dollars i think that the only thing that we could offer is you know the prestige of being a part of a really important process in ethere

**Micah** it's only a million dollars not a few Million

**William**:  i don't think i agree with that either i mean i mean i'm in the app level dev personally and i mean yes i could put an erc20 contract  i have no interest and like you know i did not make any dog tokens  i have no interest in doing anything of that particular ilke  i i think also the point that you mentioned before lite client about shepherding is important i think would also really play into funding  something that i think would probably
be more important for the ercs than the corey ips is it having  people of a capacity that are more shepherding than necessarily critiquing  a lot of the erc's these personally that i've looked at just literally need help like maybe to explain to people what needs to change or to help them especially if english is not their first language  through the process of even getting a like legible flesh out erc and then to maybe shepherd them a little bit through the process  i believe that that is well geared for a nber of people who probably
would not necessarily be in the position to launch like you know the next hot er c20 token anyway and i also to get back to what i was saying before i wouldn't underestimate the goodwill of people who are in the space for the right reasons

**Micah** i think if i understand what labour land is getting actually talked about before
it's it's this weird intersection where you have people who are passionate about the work
and no matter how much you pay them is not going to change whether they work so you got people like me for example who i i don't get paid but for some reasons unbeknownst to anyone i continue to help out and put forth almost all my effort into ethere  and then you have people that are motivated financially and if you're motivated financially and you're Capable in this space there are more profitable things to do and so we're kind of
looking for specifically that set of people who are interested in making ethere better
and then of those people the question is is how many of them need financial motivation on top of that like will that push them over the fence and maybe there's a lot i don't know

**William**: especially for the innovating position what i'm trying to argue is that i do think that that would be useful i mean choose myself as an example  financial motivation in my personal case i'd say it's not why i'm in the space and there's a lot of things i do do for free but it's definitely a lot easier for me when there is financial kickback for me 

**edson**: i mentioned finance because people that are competent they are i mean they're they're probably already busy right so having like finances like as an extra incentive they'll probably put more priority over during the work

**Lightclient**:i'm just thinking in terms of you know if we're trying to build great standards to create interoperability between the most important projects to me that means you need to get buy-in from the developers at uniswap you need banter you need these people who you know it's not it they're not going to be swayed by okay we'll give you 5 000 whatever they're not going to be swayed by some money to participate in that and yeah there are a lot of roles and important jobs that can be done by people who aren't necessarily meeting big d5 projects
but it can't be a group of outsiders just fully leading these standards because it needs to be the people who are going to be using the standards of the highest level need to feel that they're you know part of the process and that they're able to contribute what they think things should be so potentially go ahead

**Micah**: i can imagine like the people who the the paid editors or paid reviewers or paid curators whatever we call them  reaching out to those other groups for soliciting feedback so i think trent has been doing this lately  for forget one five five nine or three seventy four one or two and so just those people who are kind of the paid workforce of eips or the paid
curators or whatever whatever you're not calling them i i think having them can allow us to
interact and integrate with those big projects  so i can appreciate what william's saying i think

**Lightclient** yeah i think yeah i think i agree i think that if we have if we have a group of people who are helping shepherd the process and they are able to create you know good channels of communication between those teams basically that's we're looking for i think there's a good chance yeah i was going to say something very very similar to micah

**William**: awesome i think there's a good chance that would be the direction

**Pooja**: so there is another suggestion in the
chat would it make sense to have an
integral standard organization or a
smart contract standards body

**Micah**i think that's kind of what your fees Are right in in theory yes  the enp process i think was meant to be kind of like a standards bodies like iso or rfc or whatever  or wc3 or w3c  it's just not quite as functional as them it's all a little more dysfunctional at the Moment

**Lightclient**: i think some i think something that could be really beneficial for the erc process is just to create a separate initial stage before people open prs and start writing out their ercs if they could just if there was a call where people could come and you know it was 30 minutes an hour and they could just give a five minute pitch of their idea and someone could just stamp it like this is not an erc and just here and you know that they want to go ahead and make a pr and really persistent shirt i'm all for allowing this but i think that would stop a lot of people from coming in and just making whatever years they want to and it's also like at the first point of contact that we can start you know understanding what what are the needs of people what sort of things and have synergy with other proposals because oftentimes
you'll have two similar proposals from different teams that don't really Communicate and there's no great mechanism other than just creating each to see what other people are
thinking and wanting to do

**William**: i'm curious to who would leverage that Service  there's a part of me that i i don't mean this to be discouraging but there's definitely a part of me that feels like  it would be very helpful for the people there for the right Reasons and then it would probably also inspire kind of a wave of low effort  like the kind of low effort low quality crowd that shows up when they can like think they get someone else to do the work like you know i i'd anticipate
being on a certain percentage of calls with that involve like okay so can you write me an erc where you can make a contract with a token and it's worth a thousand dai always or something like that  but it would be helpful for other people also and it could be the cynical vision is not correct here

**Pooja**: i think in the essence of time i would like to smarize this particular item but before that i want to make a mention of it the fellowship of adidas magician on that team that they are looking into some or the other like you know process related stuff with respect to ercs maybe  catalyst can also contribute to that and in that case we can look into a proper
process not as if not an organization Maybe focusing more on process we'll try to discuss it in this meeting because we consider this as a process improvement meeting we'll bring it there but now like the example that we that i just mentioned about erc223 i believe the general agreement is until that is a standard we should not call it as a standard that can be
something that people are free to refer to but that should not be called it as a general standard

**Micah** yeah with a little minor adjustment to that i think we should actively discourage people from  running off with like drafts and saying okay it's standard i'm going to go implant it like actively discourage that because it has caused much problems over the years

**Lightclient** how can we actively discourage that though because right now you know once it become once it goes on to the live website there's just nothing that we can really do people you know no matter what we say people are gonna do it because it has a nber in front of it and it's on an official Website and that's why i think that there needs to be a stage before to try and help stop or at least get a more fleshed out version before it becomes live

**Micah**: yeah so in the past what i've done is ihave back when i was doing erc stuff  i
Just would when people start i see people referring to it and just tell them this is not a standard do not implement this like or implement at your own peril like this is subject to change and make that very clear and That kind of helps at least a little bit i'm not suggesting that we go out and start like camp actively campaigning just when people approach us and say hey i'm looking for a standard on this don't send them a link to a thing without a like warning labe that says this is not a standard yet but maybe in the future this will be a standard you could help participate by joining in the discussion

**Edson** and that should be sufficient but i think this is an issue that's other standards centers organizations have where they it's it's clearly in draft and then people start implementing implementations for it anyways like in javascript there was decorators which  some projects in react started using but they needed like special libraries to use it and i think angular is used uses decorators even though the the spec was still being fleshed out and wasn't in final state  but they i i guess the javascripts as standards they they're willing to do that just just to keep the process transparent but yeah i think for the give up i'm not sure there's anything we could do other than write text and like it requires text before it's in draft but in the in the spectr vote it literally could be as simple as having a warning banner
 
**Micah**:i like that i
like warning better on the ap's repo for
anything that's not final yet
says beware this is not final yet this
is in this stage if you want to learn
more about what that stage means click
Here

**Pooja:** is that something doable like can we do it on the presentation

**Micah**: okay yeah it should just be somebody someone who knows css and html basically just needs to submit a pr to the eips repo in on the one of the templates i don't know which one 

   **Pooja**: does anyone from the present group is willing to own i know a little you are very much familiar with eips github is that something that you would want to own i mean i understand you have other tasks as well but   i am asking if there is someone who can own this it's fine then we'll look into it later 

**Alta**: yeah i mean do you mind kind of reviewing a little bit on what it entails that wasn't paying 100 attention

**Micah**i just say some html and css to put a little warning banner on the top of any non-final eips in the main web page and the code for that lives in the ips Repo

**Alta**yeah i mean that's something i could do for sure oh yeah i could send you an example so like something like that

## 4. Progress on JSON rpc api spec in eth1 repo

**Pooja** i know we have only four minutes left so i wanted to discuss about erc editors like what are the things that we are planning to do but just in in essence of time i want to
touch up on any other item quickly that people would want to share i see there is this item json rpc Api spec is it something that we would want to have it on agenda on a regular basis because i know there are a lot of work going on in the background 

**Alta**:  yeah i mean i think having a follow-up on that is good i guess kind of one pertinent thing to bring up is i created a bunch of issues and a project on the  on the eth1 specs repo so if you want to see like the progress of the of the project  which is essentially zero right now  then you can check there but it's underway  things are starting to ramp up more now that we've kind of come to a conclusion on how things are going to get done  and i'm just kind of going to soon i am the person and getting you know more focused work anyway	

**Tim:**  sorry yeah about the open pr for the
15291
 i saw so matt or
you had two like basically typo
comments but aside from that if i commit
those in
 is there anything else we're missing
before we can merge this

**Lightclient**: i think it would look good to me okay i mean we can make changes in the future right but

**Tim**: yeah okay so i'll commit those two suggestions and i'll merge it so we can actually share that to people
 
**Micah**: i still think we should rename the file before we merge it personally but i'm not going to die on the hill

**Alta**: so i reverted the the renaming but  the the important thing to recognize with the renaming is that like i'm going to be completely revamping like i'm going to be splitting everything up into like different files and stuff like that's the next step  so it's pointless but

**Lightclient** well i would caution against you know how you're going to proceed on this because if you're going to start doing a lot of work on the spec i think that work should be done from scratch so that we can license the cco because it is apache2 license and if we just continue using this as a base then we're going to put a lot of work into an apache 2 Project

**Micah**: yeah it's it's annoying but i agree with that this time just copying the spec was kind of

**Lightclient**: you know to get the ball rolling asap and have a spec for 1559 stuff but for the future work i think that the first step is to yeah i don't know i don't think it's i mean it's a spec and so it's not going to look that much different than it kind of is already but if you're going to write from scratch i reckon just doing your best to write it out from you know clean and then we can license it cco

**Tim**: is there a way that so i i just merged it is there a way to host like to have like a hosted version of the spec basically that we can link in the in the region

**Light client** yeah it's it's a i think you probably saw the link that i had put in a pr or something where you could pull up a full dashboard for it i think it's just a matter of connecting
with the rights that helps people at the ef to get a domain set up and then have continuous integration to deploy it Okay

**Pooja**; so i see over 100 issues that was created yesterday on eat one dot post by people i personally feel that's a good way of keeping track of all the tasks that that is being put in but it was funny to receive more than 100 notification in like 10 minutes thank you for all great work you're doing here

**Lightclient**: yeah i'm not sure if i'm the only one but i would prefer these to vet in a single issue because i think we should be cognizant that there are people watching these repos and it's in that's a lot of notifications for just some people beginning and i don't want to discourage people from watching the spectr repo this is really important today 

**Tim**: yeah i would kind of agree if there's a way so it's not only the one time notifications
and now it's done like it might just be too much of a pain to change it but it's also like the kind of order of magnitude difference between like everything else and that so it's like kind of hard now to find you know any other issue in the ethos factory oh there's not a ton now 
but yeah you know i don't think it's   worth necessarily closing the 145 issues because that'll just take a bunch of time but yeah i think in in the future if we could try to like group stuff and yeah have a smaller total nber that would be that would be good

**Micah** i i just agree with both i think that the it's a one-time cost to get all those dishes created but it gives us a lot more clean tracking on progress and allows us to distribute tasks and distribute work more easily okay  and we just apply labels to them too if we need to filter

**Alta**: yeah is like in the case that we want someone to get on board because i'm not fulfilling so if you want somebody else go faster  be it's a lot easier to just kind of assign tasks and delegate

**Pooja** right so initially i thought that there was some issue with the bot or something like that but later on i realized these are these are all issues yeah if that can be bunched i mean  i also feel that it would be better but now that is there let's let's keep it let's use it for the purpose of tracking okay we are already like on time anything anyone wants to cover i know there is another can called source of eips that is listed for today's and eip gets a bar so  anyone wants to speak on either item maybe we can go a couple of more minutes and then we'll conclude the meeting i don't have anything significant on canonical erp ids okay
 
**Micah** does anyone hear ruby experts we got the github notification from dependabot saying we've got a security issue we need to address but i don't know readable enough to analyze it

**Lightclient**: i mean it looks like it's just about being a version of some of the gems it seems benign to me you think we should just merge it and pray yeah i call it i said i think we should
just go ahead and merge and make sure that the site builds properly i can't i mean it looks like it's just a minor chain it's a minor version increment so i can't imagine it's going to break anything but if it does we'll just quickly revert It you want your hands clean i see that's right hold my hands clean of this impending Doom 

**Micah**: when it turns out the defender pot is injecting a back door into the aps repository i don't want to be held responsible

## 6. Progress on EIP GitHub repo action bot

**Pooja** okay okay so the last item i believe there were some action items from the earlier meeting and tim you have created some pull requests for that i want to say something about the 

**Tim**: oh yeah so yeah thanks for reminding me  i put a pull request in the east one specs repo with all of the previous hard forks basically  i basically copied over the eeps into that i didn't want to merge it until you know people had a chance to look it basically com so it copies the text from the e the only change i made is i link back to the actual eep  so i added a kind of metadata link field for every one of them linking the eep

**Pooja**: thank you  so yeah we are already over time and thank you everyone for joining
uh we hope to continue this discussion On some of the topics that we started today but we may not get on the conclusion hope to see you all in two weeks from now thank you for joining today have a great one thanks everyone congratulations matt

### **Next meeting**

Wednesday, August 4th at 1500 UTC

## Attendees
Pooja ranjan
LIght client	
Trenton van epps
Spore_Druid_bray
Brent allsop
Light client
Alta moore
Edson ayllon
Micah
Hudson jameson
Tim beiko 
William schwab
Gary schute
	
