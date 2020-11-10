# EIPIP Meeting 19 Notes
### Meeting Date/Time: Wednesday, Oct 21, 2020, at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/36)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=k9rTZTkne3g&feature=youtu.be)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION ITEMS

**ACTION 19.1**: Edson will share a Medium post on EIP editors.
 
**ACTION 19.2**: Move agenda items 4-6 from  previous meeting and Agenda Item 3 from this meeting to the next meeting on November 4, 2020.

## AGENDA

## 1. Onboarding EIP editors - expectation guidelines.

**Pooja**: Hello everyone this is EIPIP meeting 19. I am going to share the agenda in the Chat. So the first item on the agenda today is onboarding eip editor. This was to set the expectation and gulide line for the editors that we are planning to onboard and we have limited number of editor and numbers of open pull request are way too many for few editors to handle. so edson conducted some survey,Edson do you want to go ahead and take it away

**Edson**: Yeah so results from the survey is the time commitment required for new editors would be 0 to 5 hours a week so relatively small that is one hour per working day at most. Our minimum requirement would be someone who is already reviewing eips,someone who understands what a standard it is and understands what content should be worked
out and what a standard is here and someone who understands ethereum to an intermediate level and is a good mediator for continious conversation. So the tasks that would be expected
just so we could let them know for new editors would be that making sure that the eips are well
formed and technically complete. Reviewing eips for proper grammar and structure,if it is related to ethereum and then picking up pears that are not merged automatically by the other major part. So for recommendations, I think the only  one is like when it was client for the eip editor.

**Pooja**: Yeah! I see a few of comments I have linked it, like maybe in one of the previous agenda that you wanted to discuss. Some points like should that be auto created reference implementation and client as requirement. Oh! sorry is it something related to a different topic?

**Micah**: Yeah that's a different topic

**Pooja**: okay, my bad. Do you hoping to you know get these things with the expectations and the responsibilities would it be possible to get it documented somewhere
or maybe have complete file or how do you want to see it ?

**Micah**: Can you explain it?

**Pooja**: okay , So I was mentioning like we should try to document all these things. I am not sure if eip-1 would be the good place to document all these things or do we want to keep it in Hacom. What is general opinion here?

## 2. EIP repository scope and editor duties

**Edson**:To document it like we could write an article maybe and requirements for your eip editors or put it in a repository somewhere.

**Pooja**: So, repository somewhere or maybe in the eip-1.

**Edson**: I mean I am not quite sure if it belongs in the eip-1.I am not sure if it belongs in the eip
repository at all. Like requirements for editors as always 

**Micah**: My vote is not in the eip's repository. 

**Edson**: I mean I could write a quick article on it on medium and then we could refer people new people to that.

**Chloethedev**: Yeah I feel like as long as there is an article somewhere that people can know what the information is that should be fine personally.

**Pooja**: Okay, I do not have any strong feeling that where it should go but yeah I agree like as long as information is available and people are able to access it, it is fine. But you know the reach would I  mean like it is my personal thought again, which is like the reach would be increase if we have mentioned even the link of the article that you are writing or mention it somewhere which is easily accessible to community. and that somewhere most of the time
comes to my mind is eip1. Like just mention it that eip author's responsibilities or the expectations are mentioned in this document, just link back to the document medium document whatever you publish.

**Edson**: Yeah, so what I was thinking is eip-1 is for any one thinking of writing an eip. The people that it would apply to eip editors but their responsibilities are would be just the editors themselves and not just editors but new editors. So, it is a very small amount of people. So at the moment they become an editor, we can just send them like personally that link to that repository article.

**Pooja**: Yeah makes sense.

**Edson**: Did you want to get to the comments from that from the agenda.

**Pooja**: Okay.

**Edson**: So these were brought up in the survey. There were not things that I thought of different suggestions that people had, for the eip themselves and let me open it up. It should be a reference implementation be made as a requirement. There should there be a tagging system. The eip should include use cases. The eip should include pros and cons. So, these are a small selection of suggestions that other people had made throughout the survey. we wanted to discuss it, Greg was saying that those suggestions can fit into or the already existing format. If that was the case may be we could include them under those sections within the eip-1. Saying
these are optional like suggested. Like you can include a set of use cases within the motivation section and stuff like that.

**Pooja**: I think I personally have seen these things in some of the eips but I have not reviewed. So,I mean not looked into too many. Micah, you have any thought on that.

**Micah**: I think the idea with that is like already you can include those things in motivation, that is the appropriate place to include  much of use cases and we have advised people on that at the moment in eip-1users. It is not clear enough to users, what the different sections mean and what is appropriate for them.So we often as editors end up having to kind of walk people through okay. This is what goes in the abstract. This is what goes the motivation etc. So anything we can do to  help users  to get it right at the first time without an editor having to jump in and tell them how to do. It is valuable whether this is valuable enough. I am fine with it. Like I don't have a problem with adding it. I think in general though.We do need to get better descriptions in the eip-1 because as they are written right now. Users are not understanding it and like people who read eip-1,walk away not really understanding what goes in each section. So,this would help with that. This not the whole problem but it is at least part of it. So, I am in favor. Again, this is nothing new and nothing is really changing. It is just more of an easier education things.

**Pooja**: Right so, like Edson would you want to take a tab on it, like open a pull request with specifying these things. I mean these are already there but in the specific categories may be. 

**Edson**: Yeah, I can write a pull request.

**Pooja**:okay

**Micah**: what were the other ones so one of them was the one I was commenting on specifically was the motivation of use cases one. What were the other, I think two or three.


**Edson**: A reference implementation

**Micah**: oh! yeah that was true yeah that one was for me, at the moment people, I have noticed are using the implementation section as a way to basically advertise their product. They are trying, basically people are using eips as an advertising thing. Like they the belief is  lots of ethereum users are reading eips. So, if I go and create an eip that documents my app, then I can put a link to my app in that eip and people will learn about my app and I really want to get away from that. So the way I have been handling it, is telling people, hey try not to link just put code
directly in this repo do not link out textual recompose.The argument. I generally make to users is that we want to make sure that the eips reposotory never gets 404 links and all that stuff
but really what it comes down to is. we do not want to open the doors for turning eips into a place to advertise.It is a huge amount of work for us. Like I would say well over half the eips I review. In my opinion do not need to be standards. They just are someone documenting their
on the earpiece repo and so it is a big burden on the editors to constantly be dealing with that. So,anything we can do to make it more clear that hey this is not a section where you go link to your app, this is a section where you put code is kind of what I was going for.To play devil's advocate since the other people who don't like this idea are not here. I will try to represent the best I can.
Their argument is that the implementations first of all try and write the spec. It is very useful to be able to go and look at someone else who has written the spec and so in those cases a link out to a third third-party repository can be very valuable .And oftentimes those repositories are much bigger than as reasonable to put in line in the eip or even as like in the assets directory. So by constraining that the implementation section to reference implementation specifically and requiring the people in line their code. We're making it harder for people to kind of provide code samples that other future developers can follow.

**Pooja**: On this topic specifically I would like to make a mention here. The Cat Herders has  started peep and eep series that is dedicated to eip. We discuss about proposal,the very first episode of that is about creating an eip.I mean like kind matter he has described certain use cases when to do's or not to do's and when you think that you should come up. Like making a pull request to propose that as an eip. Like you should not be just one case specific. As Micah mentioned that it was just one app specific but you should be very sure of that  is equally applicable to many other applications. So I think I am not sure if it is appropriate to make a mention of that we can probably put a link of that and people can go and watch that because in that like Client has explained a lot of stuff which would be very helpful when you are creating an eip for the first time. 

**Micah**: The more we can educate users the better. But there is also the separate problem of users, who are educated but ignore the rules in order to try to advertise their product. Those are the ones that I am kind of more interested for this particular reference implementation thing I am trying to make it. So, it is very hard for  such people to be able to use eips as an advertising channel. Mainly because as an editor most I believe all the editors have agreed that we do not want to get in the business of deciding what is worth while as an eip and what is not. So, by removing the opportunity for someone to use eips as a means of advertisement. We do not have to then decide okay this is valuable as an eip or this is just an advertisement. There are lot of eips are kind of borderline where it is like I think this is really just an advertisement for an app. But I mean the user can make an argument and now we are getting into the debate of okay is there argument sound is it  a good argument. Whereas if we just made it so they could not advertise. Then all those people would kind of just go away and they wouldn't even try to fight us
because even if they did get an eip created. It wouldn't help them advertise and so I guess there's two problems: one people writing eips don't know how to write good eips and I think the peep and eip is episode that you talked about. It is great for that improving eip-1. It is great for that the separate problem getting advertise people out of eips who are just trying to advertise. I think it is not going to be solved just by education. I think we need to think other solutions for it.

**Pooja**: I think maybe some kind of guidelines, I mean like ofcourse these are the guidelines,but there should be some rules like may be criteria defined, like in what cases there are high chances of it getting not accepted that is not formally announced anywhere or it is not listed. Is it something that can be considered?

**Micah**: So at the moment basically the only thing that gets you kicked out of the eip's repo is if it is not technically sound like it is very cut and dry. There is no wiggle room for editors making an opinionated decisions. It is just like, does this meet the technical requirements of an eip? Yes, okay it is an eip. Historically the editors have all and I actually agree with this that
editors have all been very hesitant to introduce any judgment calls by the editors. Like we have tried very hard to make it. So all the editors, our only job is just make sure things are technically sound, make sure they're written correctly, make sure the grammar is right, make sure the bot passes, make sure that spelling is good make sure that the things are in the right sections etc. so this is why we don't have any fuzzy rules. All our rules are very clear-cut.This is  why I would like a rule that is clear-cut that makes it you cannot link to your personal repo in any eip. Like I said they are downsizing this, it means that for the limited use cases. People cannot  link to repo's and so if we want to stick to our hard-line instances. We need to choose we want to allow people to link to personal repo's and project repo's in the eip or do we want to say no external linking at all. Do you have to include everything in the eip or do we want to break our historic position of editors do not make opinionated decisions. I think there are three possible path forward that I can say.

**Pooja**: I can see one thing that you have mentioned that mentioning their personal eip. I mean github repo that is there in most of the genuine cases because while working on some project they came across. Something that is again sent to the eip repo as a pull request. So it is
going to be linked back in most of the cases. So, I am not sure if that can be a hard rule but in my opinion like editors should have all the powers to make rules. It is not that if they are taking a step back who is going to do that. I understand this is a community project but somebody has to like step up and take these responsibilities to set rules.

**Micah**:So I agree things would go way smoother if that was the case. However historically both this all core devs has this exact same problem where everybody is very hesitant to give anyone else the power to set rules and enforce rules. So,I am not confident that would go over well. I do agree with you though things would go way better if we had like an authority figure
or figures who just said no. I do not accept and I do not need to give you a reason or at least I do not need to convince you of my reason I should say but yeah that is. It would be very hard sell I think.

**Chloethedev**: I am curious, I am sorry so, what is the issue of just being no linking external code in the repo. I mean I understand it would be more difficult for certain projects but then could not those projects just write out hey like I understand that like having a link would make it easier
but you know it seems like yeah what is the main issue against I guess.

**Micah**: As I understand it and again I am trying to represent people who are not here so, it is best if we get it from them once. They are around but my understanding of their issue is that they are concerned that there are some eips when implemented are very complicated, particularly core eips where implementing a core eip like a reference implementation. May be likethat is reference implementation. It is like an entire repository of stuff and like the eip is implemented you know all over that repository like especially evm changes. You know there is not just like one line. Somewhere where it is like oh here is the evm change and it is like here's the entire evm and here are the 12 different places in that giant code base that we touch with this eip and so reference implementations for those are very difficult. Whereas if you're just linking to geth then it all of a sudden becomes much easier you can just say hey here's the guest repo they have implemented it here are the 15 files that you want to look at if you want to check to see you know the places that this touches uh whereas a reference implementation was like okay go write another client it is kind of the replica yeah the reference implementation.

**Chloethedev**: Yeah that makes sense guess like the issues that you were proposing of people or teams trying to simply use the repo as advertisement and I would assume that is not something that usually happens from client teams or sort from corey eip. So could core eips have a specific distinction of allowing or links or just to keep things the way it is and then just have
other like all other eips not allow links would that be a way just to kind of okay well you know what these more complicated. Eips we are going to allow links still but try something different with or this new way of doing things with other eips potentially.

**Micah**: That could potentially help I think that there are situations where an eip is complicated enough to probably warrant its own you know linking out to separate repo and it is not a core eip those are definitely much less common.I think I am not against that what you just suggested again playing devil's advocate i think the argument is we are now adding more complexity into
our process because now we have to draw a line between what is core and what is not and there  have been examples recently in the past, where it's kind of blurry sometimes what's the core eip and what is not. Then like what if someone's linking out to a fork of death and because it's not implemented in gaff yet such as their fork but whether that fork ends up being you know another ethereum client or another ethereum network. Like you know turbo gas for example. is that part of ethereum network it doesn't actually sync with the ethereum network right now fully. I don't think but they are also not you know building for tron or something yet there are ethereum clients that are forked from geth that are building for tron should we allow them to link like it is just I think  there is going to be a fear and pushback of like where do we draw the line because now we have. We are the arbiters of what is an official client and historically no one has named any
official clients like geth is the most popular but there is open ethereum there is another mine. There is bessu, there is turbogeth and the line there is very blurry of okay where do we draw the line who is allowed to do this and who is not. Again I am not against what you suggested I just that  what a problem I can see coming up potentially.

**Chloethedev**: Well that makes a lot of sense thank you.

**Pooja**: Will it make sense to kind of mention this thing . Like in this particular group this eip group what we are trying to do is kind of improve the process which is ongoing. We discuss about some of the issues and we brainstorm potential solutions and try to come up with solution but the implementation part in my mind would not be effective if we are not getting support from
everybody and if they are not willing to accept the decisions that are being made or the proposals actually is not decision. The proposals that are like going out from this meeting. So, will it make sense to kind of guard the all-core devs sentiment on this part like how good it is to define certain rules like so far there are not hard lines now we want to define hard lines is it something that is acceptable then this particular group can come up with certain rules and we can share it with them to get collectors.

**Micah**: If I pretend to be james for a moment, I will  say that putting my james hat on I think james would say we are trying really hard to separate eips from the core devs.They are a user of the eips repo but they are not special they are not authoritative they like basically we do not need to get permission from the core devs do anything? The eip is not a coordinated thing it is a totally separate entity, separate people managing it.

**Pooja**: Totally get it

 **Micah**: So just again I suspect that's what james would say if he was here.

**Pooja**: Yeah I know. I am getting the point here. So in that case in my mind it feels like you know the eip author should be like the group the people who should be like making rules and we the cat headers or the eip group can support to get it enforced. Like we should list it out. Okay I see that Greg has referred to some of the comments. I mean like related to the rules and responsibilities of eip editors. 

**Micah**: Now before  we move on what was the third item Edson.

**Edson**: Pros and cons and let me go back to 

**Micah**: Sorry I just want to make sure we finish this before we move on that is all yes go over everything.

**Pooja**: use cases pros and cons and reference implementation and one more thing was tagging system.

**Edson**: So greg said that eip is already tagged with labels.

**Micah**:yeah I do not think that is the same thing

**Edson**: yeah, so for tags I do not know what would be added so like tagging implies that multiple tags could be applied to the to a single eip and then it would be used to filter. May be like in the eip website. Then pros and cons you could we can may be suggest that for the motivation section

**Micah**: So as far as those two very good. I think I am liking a little bit.

**Edson**: We can hear you

**Micah**: So the pros and cons i'm fine with. Again i feel like that something goes motivation we should make eip1 better and encourage people to put that sort of content in the motivation section on the abstract not in the simple summary, not the specification.

**Edson**: Yeah I agree what about a tagging system

**Micah**: I am not against the tagging system personally. I worry that what is a tag and what is not and which things get tagged with which things is going to be complicated and I do not know if it is worth it like my personal opinion is people should really, only be reading final eips like too many people read drafty eips and there are relatively few final eips. So like I do not know if we have enough final eips  to warrant having a mechanism for filtering them yet and for draft eips I would rather people just like get them out of draft.

**Edson**: Yeah I think that's fair so tagging would be more beneficial if we had a lot an overwhelming amount of eips especially in final. I will make the prta p1and then it could be reviewed.

**Pooja**: Yeah I think by making this new people will get to know like what should be added more in their proposal in the pull request. so that's about it and the next item in this was also
referring open issues. okay on the expectation guideline. There was already a pull request open
as a role of editors in eip process. I am not sure did you also consider that while considering the expectations for eip editors.

**Edson**: I am sorry I could not really hear you did you.can you read that.

**Pooja**: Okay, so there is the next topic which is on the agenda item first about the expectation
of responsibilities of eip editors. There was also an open pull request talking about these things.
uh i think it is 1467 pull request 1467 role of editors in eip process, just wanted to bring it to your attention while documenting the expectation if this can be considered as well.
okay anything more on agenda item one on onboarding eip editors I think we came up with two decisions one Edson would be writing up a medium post on eip editor's expectations and responsibilities and he would be also opening up a request for what more could be added. When we are proposing an eip. okay so the next item is a eip repository scope and editor's duties talking about it.

**Edson**: Just one thing, before we move on. I am looking through the issue and it is saying that eip editors assign numbers. I do not think that is actually true. We should probably update the eip-1 with that. 

**Pooja**: I think  I have seen some comments of Greg on that part, he mentioned that it is
actually the role of editor but most of the time author  does by themselves. They do it like. I do not know I have found that bot does not give it a pass. If we do not add the eip number or something like that I am not sure. 

**Edson**:So the eip number right now is determined by the pull request number 

**Pooja**: Right 

**Edson**: Which is not in the eip one but that is how it is done.  I think we should update eip1 to reflect that because right that is not actually a role of the editors right now. They just suggest using the pr number.

**Micah**: I think that is the opposite the editors if I remember correctly. I need to read it again but I remember correctly the editors choose whatever number they want, it just so happens that the editors has  right now to choose the pr number.

 **Pooja**: Yeah, I think and this is also mentioned in eip-1. The current eip-1 that mentions it is
clearly that it is the responsibility of an editor to provide the pr number, I mean the eip number to any pull request. so yeah it is completely up to them.

**Edson**: Because I was looking through the core devs chat and they had suggested that. I think they had decided that the eip number is the pull request number.

**Pooja**: Generally it is that but if editor wishes to give some other number which is open and yeah they can.

**Edson**: Has that happened?

**Micah**: Yeah a couple times has happened where something other than the pull request number was used. One of one time it was because someone was trying to squat and so we
punished them by giving them a different number like they're trying to squat on a particular pr number and the way they did it was they spammed. The eips repo with a bunch of issues to bump the number up to what they wanted and then they took number they wanted. We just said no and we gave them something different and that made them very sad and that made us very happy.

**Pooja**: Yeah so I think that that does not need to change. I mean that will still be considered
under the responsibility of an editor to provide the eip number even if it is the same as the pull request number.

**Edson**: I mean generally like so i think it's the exception where the eip editor changes the number. But most cases, the eip number is the forcast cost number and I do not usually see authors asking permission from the editors for that in that case.

**Micah**: Yeah currently that is the case the vast majority of eips are just the pull request number because it is easy. We have also given people like if they start with a an issue and like we recommend they do. They start with an issue as an idea, they flesh it out a little bit and they
create a draft. Sometimes we will let them use their issue number instead just because like maybe they have already referenced it or they have already talked about it. What is the advantage of codifying that or solidifying that?  okay is there a problem with the current
system.

**Edson**: I guess like the biggest benefit would be to new. New authors because it is not anywhere in the eip-1 but that is the way it is done.

**Micah**: So, you are saying we could save the editors some effort. Like right now author creates an eip. They put tpd and the eip number. Editor just immediately posts a comment saying “change this to the pr number”. We are saying we could avoid that step, if the author is just did put the eip. Sorry if the author is filled in on the first draft

**Edson**: Yeah exactly.

**Pooja**: well on the contrary I believe that keeping it with the editors will help. Prevent some squatting thing as well. Right so if we don't do that and if we allow the editors to just choose the pr number then I am not sure if we would be able to stop that.

**Edson**: We could all, we could also just specify any. If you want these things aren't allowed like inflating opening issues to get a specific number opening a pr with that's empty for a specific number.

**Pooja**: Yeah and that's how.

**Micah**:  I am ambivalent if other people feel strongly, I  don't care that much. 

**Pooja**: My thought is it should be with the eip editor itself? Like they should have authority of like. We are giving everything to the eip editor. We are saying that they are the boss and they would look into everything. So the the like top most thing is the number that it is referred with but that is again me.

**Micah**: Is anyone else here? Edson repeating himself. I think  either he is lagging or I am lagging. I cannot tell which.
 
**Edson**: Right now I hear,  no one talking so, I can may be try to rejoin. I should be using headphones so this should not be an echo.

**Micah**: That is not an echo, it is like you will say something and then like may be a minute
later I will hear you say the exact same thing again and it's only you i'm not hearing it from anyone else.

**Edson**: Let me try rejoining okay. 

**Micah**: Sorry I already rejoined it didn't fix. So may be that will fix.

**Pooja**: Any other thought on this proposal on eip number and peer number.

**Micah**: Like i said I am ambivalent , I can go either way I think that right now the editor telling someonewhat the number to use is by far the easy easiest part of the job.

**Pooja**: I do .

**Micah**: So it is very minor  to me to have to tell people hey like it is just you know triple backs back take suggestion type in the number. Triple back tick like it is super easy for me super, easy for the author and so that is why I do not really care like there are so many more time consuming
problems when as an editor that one is easy.

**Pooja**: Okay so i'm not sure like we should mark it as like decision item or should we just keep it open for one more meeting and share it outside this group present group to get some more response on that. If general opinion is it does not matter. I am fine with that.
 
**Edson**: So, here is,  can you hear,

**Pooja**: Yeah,better.

**Edson**: So, here is the thing for when I was first looking at the eip repo. So i thought that you needed to have a number first to even create a pr, which was an understanding on my part. until I did research like oh the pr numbers. The pr number is the eip number so.I was thinking of contacting the eip editor. Just to get an eip number, just to open the pr because most eips it is the file name is the eip number. So, it would be weird to open a pr with the file name that does and not that is just empty.

**Pooja**: I think that is what is traditionally done. We just open a pull request with the file name
and later on we add the eip number to it and it accepts. It like it works that way. I do not know.

**Micah**: So for an author, I think that the situation is going to be basically the same because 

**Pooja**: We can't hear you.

**Micah**:  Yeah pretty ! I am pretty sure, I am liking. I will try to just listen and type up. I have some importance.

**Pooja**: Okay so do we have something like some consensus here, before we move on or do we want to keep it open for one more meeting and then decide on this part.

**Edson**: I think it is fine so like all, I was suggesting is may be specifying the eip-1.  Typically the eip number is the pr number, because right now it looks like editors are writing the eip number for every single eip. 

**Pooja**: So, like as far as I remember it is already mentioned in there but not all the time that you just do that. Like in my case, I have made three four pull requests, so for a couple of files when it was not getting I bought pass. So like Ken suggested me, Micah suggested then I went ahead and I corrected it tried the wrote the eip number and it then started showing me the green check. So it was fine by me.

**Edson**: I mean I have not checked recently but unless I remember it was not mentioned
in eap-1.
**Pooja**: Okay, anyone has any anything uh concluding on this topic . Okay, then in that case like I would like to keep it open. Like may be add it only this point before you go ahead and
make couple requests for changing thisparticular point like the eip number would be provided. Would be added by the author itself and it does not come in the  responsibility of eip editors. Just
this point and let's  have some more opinion on it. If people think that it is not very important thing and like it can go and all the authors should go ahead and do that will be added in the pull requester one the one you are creating for.

**Edson**: I will make two separate pull requests.

**Pooja**:  So make sense yeah that makes sense then it would not be dependent upon whatever you are trying to make pull requests.

**Edson**: Yeah exactly 

## 4. [Micah has too much power](https://github.com/ethereum-cat-herders/EIPIP/issues/36#issuecomment-707494164)

**Edson**: okay make sense. Okay so are we good to move on. oh my god we are okay
so there are a few other topics that we have to touch today. I am not sure like  we would be able
to get on all of them but there is one topic which was suggested by Mika. About the Mika has too much power. Is it something that we would want to discuss now? I see that mika has written a like big comment about it . Also, Greg responded to that at this point of time only exec subtacular Greg and Mika are working on it. My hope is with having more editors on board this problem
can be solved. I mean I have no problem having Mika so much of power but it is like on his part he is getting a lot of work to do. A lot of responsibility on him. So I believe that having more adidas will help now. The biggest question would be like, how do we invite people to be you know considered for eip editor. one suggestion we have like client as the Edison mentioned but what
are the other ways how we can invite people.

**Edson**: Yeah I agree . I think it might just be a side effect of there not being many active editors. I think what micah can do in those situations is just tag the currently active editors to mediate the rest of the discussion.

**Pooja**: So, yeah historically a selection of editor was a simple, like complete the present editor they select somebody and that person is now auditor and they can start taking up responsibility but I think we can I mean if it is okay with the group. We can make. As you know  tweet about it asking for inviting for adjectives and let's see if people who are from the community and they are interested. It is just that they are not aware of like we are looking for more editors if they show up then we can pass along the names or if there are any other suggestions of how we can invite these people because we need more than one ofcourse.

**Edson**: Yeah i mean we could start with looking at who is already active in the eip repo.

**Pooja**: Okay 


**Edson**: May be we could  ask current core developers. Since they already have an understanding of thing like ethereum. They should like a at least an intermediate ,if not advanced
understanding of ethereum.

**Pooja**: Yeah, totally agree like historically those people are editors. They have done this responsibility in past so if someone is interested now we can possibly invite them.

**Edson**: Yeah like I think I would be comfortable awaiting anyone from geth, anyone from
netherline, anyone from a baesu, Just any anyone from there would it be a good candidate or like the rest of the clients.

**Micah**: I suspect the problem is going to be time availability. Like my understanding is the  developers are all currently way overworked.

**Pooja**: so in that case maybe uh this document  that edson specifying what is the expectation five hours a week but may be I am not sure if they are comfortable or like taking out
time and doing it. It  is not  hard to you know check with them. May be we can make an announcement and see what is the response we are getting.

**Edson**: Yeah so the the time requirement was minimum zero to five hours. So I mean even one hour a week  is fine as long like one hour of work for eip repos. I do not think it takes much time to review eips because it's mostly just approving or specifying why it is not approved.

**Pooja**: I don't know may be Micah is the best person.

**Micah**: The most time-consuming part is teaching. The most time-consuming part is teaching
people how to write good standards, like most most people do not or it does not come naturally too.

**Edson**: So may be we should put more time into education.

**Alita**: What if we created like an online course or something like in.

**Micah**: I am definitely a fan of educated people more. The thing I worry about is that the
people won't go educate themselves, before they create an eip and then  like should are we supposed to just be like, if someone shows up writes in the eipp and it is bad. Am I supposed to just say go go take this course and come back or should I okay I feel that is a little bit rude but I mean at the same time I do not have infinite time so that may be the only option I have.

**Edson**: Yeah, So I was thinking that write an entire course but  there could be  say there is something that they mis wrote or some something that they have that is not  meaning the requirements of a specification instead of writing it out entirely. You could summarize it and then link to an external source that says read this to understand really what I am saying. 

**Alita**: You could also  like say create a core or let me just think about like a documentation for how it works and then you can just reference that documentation whenever you have a problem
with that documentation having like the full explanation regarding the problem itself that is like relatively common or whatever that might be easier.

**Chloethedev**: Yeah if you personally if it was a course. I mean you can call it like a course or
documentation or whatever it is but I think having you know the editor being able to link just like you know not having to teach because I feel like all the teaching that you're doing like is probably
could have been put into a course. Anyways probably notice you . So, you know if there was this like place people to go to for Michael. can just be like okay well I mean you're way off base you know start here. I think that might just streamline the process potentially a little bit easier.

**Edson**: I mean like because we we do want more editors but if most of their time is being spent educating. we could just do the education beforehand and then have the editors like back, because like the ultimately like one of the larger goals is just reducing the backlog. but I still think we should add more editors and we should  brainstorm how to onboard more editors.

**Pooja**: I will agree like giving them education.I mean like having some documentation part or
some reference material at least will offload a little bit from the editor's job.

**Edson**: Yeah mike  I see your mic moving but i'm not hearing anything.

**Micah**: Regarding. yeah so I think that we need more there's two reasons:
 one to help keep up with everything like I fall behind frequently and it is hard to catch up andwe still have a backlog of prs that have not been touched for a year because I have not like currently.
I only try to keep up. I do not try to clear the backlog. If we had more editors we could do both. Second thing we need more editors for is so that I do not have so much power and so even if we do solve reduce my workload. I still think we need more editors so that if I decide I don't like informational eips. I don't have the power to unilaterally implement that just because no one else is merging the earpiece and at the moment I do. So because I do not like informational eips are
de facto banned from the repository because I would not merge them and I do not think that I should be have the power to do that. Like without discussion, without agreement like no one agrees with me on this which is my personal opinion. Yet that is effectively what is happening
and I do not like that and so even if we do reduce my workload I still do think we need more editors.

**Edson**: Yeah I agree with that. 

**Pooja**: So yeah I think the best uh way that is like we should try to first finish up with this
document. This is the medium post that Tarzan will be working on. Then we will try to reach out  the co-developers or the people who are heavily engaged in ethereum development. If they would be interested to be. You know editors to be giving some time maybe an hour a day or something like that then we can set expectations and let's see how it turns out to be. But I think that is certainly needed at this time. What happens like it is my experience like as mentioned
as Mika mentioned that when when he says that information eip is not agreeing to it and it is there nobody you know, nobody else is there to either take a decision whether to close it or not move ahead with it or may be merge it. It is there forever and after the bot after three months it will be closed automatically. Nothing can be done about it so we should not just let go any proposal just because nobody is there to attend. There should be a like you know decision before we are going to close a pull request. So I think that is something that you need to be looked into.
Okay so I think this is not something that we can decide right away it is going to take time may be
in next three four meetings we would be in a good position to speak more about it how we are
proceeding and like we are almost time.

## 5. [Review action items from previous meeting](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20018.md)

**Pooja**: I would quickly like to cover a few things which was coming from the action item from the previous meeting. A Lightclient shared a twitter account eip info for tweeting eip updates. I have shared that with James. So,everybody else is interested
they can get in touch with James on this part. There is another item should meta and information eip be part of eip at all. So that was listed here in today's agenda  like eip repositories scope but we could not cover it. It is a long discussion and we could not cover it in this time so. I am going to move it to the next meeting. Pooja will reach out to eip authors to get them to follow the documented network upgrade Mika and I mentioned this in the all called meeting that the author should be creating pull requests to change the status of their proposals which are getting into berlin. Mika reached out to Aragon to tell them that they need to put in comment to eip3000. I am not sure Mika, is it a closed item now?

**Micah**: Yeah that was handled, I told them to add content and they did after like a day and then it covers it.

**Pooja**: Great move agenda item four to six to the next meeting that we tried to cover in this meeting and yeah that is all from the previous meeting. Anything else people would like to cover
today. we are like one minute past the time but yes is something that can be quickly seen. I do not see a Lightclient or James on the call or Hudson. So skipping the triaging permission item but anything else if anybody would like to discuss. Cool so we made good progress we have some
decisions or being you know to do's for us. Thank you all for joining today see you in two weeks November 4th 2020. One more thing like on november 4th the time is going to be changed for the
daylight. People living in the daylight area like est is going to change, so we be sure that the meeting is at 1500 UTC even if it is like change in eurozone.Thank you.

**Edson**: Yeah all right thanks bye.

**Chloethedev**:Thank you very much everyone see you in two weeks.

**Micah**: Thank you.

# Attendees

* Alita Moore
* Chloethedev.eth
* Edson Ayllon
* Micah
* Pooja Ranjan (Host)
* Brent Allsop

# Date for Next Meeting: 04 Novenmber 2020 at 1500 UTC.
