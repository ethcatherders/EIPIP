# EIPIP Meeting 54 Notes
### Meeting Date/Time: Wednesday, April 21, 2022, at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/125)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=4hii6hcYL3M&)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION ITEMS

**ACTION 54.1**: Keep “Core EIPs in an Executable Spec World” discussion on the agenda for the next meeting. Collect community feedback.
 
**ACTION 54.2**:  Sam Wilson will make a pull request to update EIP-1 for discouraging the word "standard" in EIP titles.

 
—------------------
## AGENDA

**Pooja Ranjan** [0:01](https://www.youtube.com/watch?v=4hii6hcYL3M&t=01s):  welcome to EIPIP meeting 54. I have shared an agenda in the chat for people to refer to.

## 1. Core EIPs in an Executable Spec World [Proposal](https://notes.ethereum.org/@timbeiko/executable-eips) and [Discussion](https://ethereum-magicians.org/t/core-eips-in-an-executable-spec-world/8640)

**Pooja Ranjan** [0:06](https://www.youtube.com/watch?v=4hii6hcYL3M&t=06s): The first item that we have for today is core eips in an executable spec world. So this was proposed a few weeks ago by Tim Beiko. There is a proposal and the link is added to the agenda. We can check it out and this has been under discussion for the past few weeks. In the last meeting Greg shared some concern for people having to learn python to be able to contribute to the execution specs but we were short on time to continue this discussion. Hence I have added it for today's discussion so yeah if there are any thoughts.

**Sam Wilson** [0:51](https://www.youtube.com/watch?v=4hii6hcYL3M&t=51s): Sure so Greg and I had a discussion after I think it was the last  EIPIP meeting. You know how python fits into the eip process and how it's not really a great fit for all types of eips. So, one thing we were considering and I don't want to speak too much for Greg but  is possibly allowing a diff against the yellow paper or the python spec in the eips that might be one path forwards. I don't know how anybody else feels about that but that's basically the only update that's happened since uh the last time we spoke about this.

**Pooja Ranjan** [1:38](https://www.youtube.com/watch?v=4hii6hcYL3M&t=98s): Right I see there are a few questions that uh those are being discussed one is about the eip number i think there are some certain suggestions for that and then some improvements that could be made with the help of bot. So if you can maybe summarise what is the proposal on on like higher level and the way we are trying to move forward.

**Sam Wilson** [2:01](https://www.youtube.com/watch?v=4hii6hcYL3M&t=121s): Oh sure, I mean at a high level I guess the idea would be to change the eip process so that instead of it being an english test text description. We would first start by splitting the eip process into two parts core eips and non-core eips. Core eips would live in the execution specs repo. Well so this is my proposal. It's slightly different than Tim's but mostly the same but in my proposal you would split the core eips and put them into the execution specs repository and then the eip numbering proposal I had. There was basically that if you have an eip that spans multiple, each eip number would encode whether it's a core eip or an erc or a consensus layer eip. So you'd have some extra information in the eip number and then you could use
that information to find out where you need to look for the eip and then the eips would live. Either the consensus layer specs repository, the execution layer specs repository or in some erc specs repository and the reason why we want to. Well I am proposing we split it up like that is to keep the standards close to the code that defines them. Yeah I don't know if that's helpful or not but that's kind of the summary of the eip numbering change.

**Micah Zoltu** [3:26](https://www.youtube.com/watch?v=4hii6hcYL3M&t=206s): Do we have to retain numbering between when we make the switch? can we start over from one?
I would like to keep one application to inspect what we gain by keeping it.  I was worried there's a lot of complexity in keeping it long term and if we could just have a different numbering system that seems easier.

**Sam Wilson** [3:52](https://www.youtube.com/watch?v=4hii6hcYL3M&t=232s): I don't feel super strongly about it. I think I would like to keep the eip numbers like and just have a legacy set and then a future set but I don't really care that much. I think my biggest concern is about how we're actually going. Are we going to put execution specs into the eip process or not ? And I think that's a much bigger question than how we're going to number the eips.

**Micah Zoltu**:  Sure

**Pooja Ranjan** [4:18](https://www.youtube.com/watch?v=4hii6hcYL3M&t=258s): Yeah I think we first need to a list of the questions that we want to be answered first in order to progress in that direction because it seems to me like there are too many things that we want to address at the same time and we are not clear on which path we want to go.

**Sam Wilson** [4:36](https://www.youtube.com/watch?v=4hii6hcYL3M&t=276s): All right I mean I guess the the biggest question is do we make a diff to the python spec a mandatory
part of core eips and then everything else is kind of secondary to that.

**Pooja Ranjan** [4:53](https://www.youtube.com/watch?v=4hii6hcYL3M&t=293s): Micah do you have any thoughts on that making diff to the python spec to exist.

**Micah Zoltu** [5:00](https://www.youtube.com/watch?v=4hii6hcYL3M&t=300s): No, I have no problem with python specs. i would like my personal desire would be that execution spec repo handles everything and that is both the actual technical spec and the human ruble stuff.  I liked the way Sam proposed it previously which is just the markdown files in there. So I think Sam and I are mostly aligned at this point. Would you agree with that Sam?

**Sam Wilson** [5:28](https://www.youtube.com/watch?v=4hii6hcYL3M&t=328s):  I think so.

**Pooja Ranjan** [5:30](https://www.youtube.com/watch?v=4hii6hcYL3M&t=330s): I have one more curious question here. So  we are talking about having execution specs for core eips only. So what do you guys think about having just for core eips there? And  for rest all of the eips including interface and networking eip following the same process as they are doing right now. Or are we planning to have uh networking and interface be a part of execution specs?

**Micah Zoltu** [5:58](https://www.youtube.com/watch?v=4hii6hcYL3M&t=358s): I don't believe there's any current plan to move any of those into execution specs. One can imagine the networking probably being the next reasonable thing the interface stuff in terms of json rpc has kind of already moved out of the eip's repo so that's already on its way out to another system

**Pooja Ranjan** [6:20](https://www.youtube.com/watch?v=4hii6hcYL3M&t=380s): I have seen a couple of interface proposals. I suppose for the exec consensus layer specs.

**Micah Zoltu** [6:30](https://www.youtube.com/watch?v=4hii6hcYL3M&t=390s): I have argued on those issues. So it is part of the reason we need to settle on something is because the consensus layer does need a place to do their change control process in some way and some people want to merge that with the eip process, some people want to keep it separate and then things get even more complicated complicated when you have some change set that includes both execution and consensus layer changes where you keep that document and so that one people are kind of pushing into the eip's repo at the moment,  not a huge fan of that I would keep it out. But I acknowledge there's not really another place to put it at the moment.

**Pooja Ranjan** [7:13](https://www.youtube.com/watch?v=4hii6hcYL3M&t=433s): So if I understand correct at the moment for execution layer specs interface proposals are already
moved out of the present eip depository however for consensus layer.

**MIcah Zoltu** [7:27](https://www.youtube.com/watch?v=4hii6hcYL3M&t=447s): Json rpc stuff is moved out.

**Pooja Ranjan** [7:29](https://www.youtube.com/watch?v=4hii6hcYL3M&t=449s): Only json rpc. Okay 

**Micah Zoltu** [7:30](https://www.youtube.com/watch?v=4hii6hcYL3M&t=450s): Yeah so the interface and theory includes other things though not much that json rpc is the bulk of it.  But hypothetically there are other things that fall into that category.

**Pooja Ranjan** [7:43](https://www.youtube.com/watch?v=4hii6hcYL3M&t=463s):  Right, so giving the benefit of doubt there is still room for interface and networking eip with erc eips process.

**Micah Zoltu** [7:56](https://www.youtube.com/watch?v=4hii6hcYL3M&t=476s): I guess I mean I don't. So yes I mean that I am not sure the eip process is ideal for either of those just like the execution executable spec. I think it is a better solution to the problem of coming to consensus around specification. I think the same is true for the networking stuff. I think the networking stuff would be better off if there was, you know, a canonical document that ideally was computer readable similar to the fusion stack. It would be like the networking spec and that had some sort of change control process built into it. Again just like the execution executable spec that's being built however,  We do not have that today and we're not there today and so since the eip process is basically the only change control process we have at the moment, everything is dumped into it and that includes networking which I don't think
is a good fit and historically an interface which I also don't think was a great fit. So yeah like it's one of those things like we have nothing better it's not it's not a great solution but it's a solution that exists

**Pooja Ranjan** [9:05](https://www.youtube.com/watch?v=4hii6hcYL3M&t=545s): Well it looks like that earlier we were in a position where we were thinking of moving eip and erc
separately. Now we are trying to pull out just the core eips from the existing change control process.

**Micah Zoltu** [9:22](https://www.youtube.com/watch?v=4hii6hcYL3M&t=562s): Yes at the moment we are only working towards pulling out core eips because with through the execution specs and again we we have already sort of pulled out the json rpc stuff which is the majority of interface and hopefully one day in the distant future when we have infinite engineering resources. We'll also pull out the networking stuff.

**Pooja Ranjan** [9:44](https://www.youtube.com/watch?v=4hii6hcYL3M&t=584s): All right, well this is good at least we are very clear on this part that we are not going to change the entire change control process. The proposal is just for limited to core eips only at the moment whenever we get a chance to update the networking and other interface eips will look into that so this is clear this is really good and now if we discussed two proposals I think not two distinct proposals somewhere overlapping. So yeah in that I mean on those two proposals the point of disagreement was including diff to python spec. I don't know if I am not an editor nor a developer but from where I am looking at it. It looks like because we have this yellow paper written only in python spec. Right now that is available with us it seems like a fair compromise but yeah if you guys have any other thoughts on that.

**Sam Wilson** [10:46](https://www.youtube.com/watch?v=4hii6hcYL3M&t=646s): So Greg did bring up the point that we do also have the yellow paper so we could theoretically use diffs against yellow paper as also an acceptable way of specifying things,but yeah.

**Micah Zoltu** [11:00](https://www.youtube.com/watch?v=4hii6hcYL3M&t=660s):  For the listeners the primary argument against that is the number of people who can functionally read the yellow paper is like 10. The number of people who can functionally read python is you know millions maybe not millions hundreds of thousands.This in terms of notation and general understanding within the developer community python is just significantly higher than the mass notation that the yellow paper uses like it's basically it's more accessible like the python is far more accessible than mathematics.

**Sam Wilson** [11:36](https://www.youtube.com/watch?v=4hii6hcYL3M&t=696s): Greg's not here. Is he? Okay so his argument against that would be that the yellow paper is currently poorly written and if we devoted as much time to maintaining the yellow paper as we are to the python specs. We would have a much more accessible yellow paper.

**Micah Zoltu** [11:54](https://www.youtube.com/watch?v=4hii6hcYL3M&t=714s): I would be curious if that is true. I am not convinced if I imagine myself rewriting the yellow paper to be more accessible. I would find myself ending a python or something along those lines. I don't see a path it doesn't take you to just use python or just use typescript or whatever.

**Sam Wilson** [12:14](https://www.youtube.com/watch?v=4hii6hcYL3M&t=734s): I mean so if I were to do it, you know with infinite engineering resources I think doing it in a formal spec language would be like ideal like something like k or daphne or whatever and that you know you could actually use that to formally verify code and that would be the best option um but no one knows those languages and they're not accessible.

**Micah Zoltu** [12:41](https://www.youtube.com/watch?v=4hii6hcYL3M&t=461s): Yeah right so if I can be convinced. I think that writing in something that can be formally verified has significant value. I do not think it solves the accessibility problem at all. So yellow paper is either accessible nor formally verifiable and the python spec is accessible but not formally verifiable and so I would say that strictly better and then there's a third option which is formally verifiable but not accessible and I can see a strong argument that is a path that one would want to take over non-verifiable but accessible and in a perfect theoretical future somewhere rainbows unicorns. We find something that is both accessible and formally verifiable.

**Sam Wilson** [13:24](https://www.youtube.com/watch?v=4hii6hcYL3M&t=804s): And I think you know the possibility of you knowing how to take off. I am pretending to be Greg  here personally. I think you know there's no reason not to use python in the meantime until we find something that satisfies both accessibility and formal verification. 

**Micah Zoltu** [13:46](https://www.youtube.com/watch?v=4hii6hcYL3M&t=826s): If you had to pick between accessible but not formally verifiable or formerly verifiable but not accessible. Is it immediately obvious to you which of those is better or is that something that you would see are good either way like are you in the fence.

**Sam Wilson** [14:05](https://www.youtube.com/watch?v=4hii6hcYL3M&t=845s):  I would say I am on the fence about it. Like from a theoretical point but I can't make the formally verifiable spec so obviously I am going to work on the accessible spec.

**Micah Zoltu** [14:18](https://www.youtube.com/watch?v=4hii6hcYL3M&t=858s): There were two people that you let's say you finished the actual spec and at the same time in parallel Greg finished the formerly verifiable spec. Which one I would choose?

**Sam Wilson** [14:31](https://www.youtube.com/watch?v=4hii6hcYL3M&t=871s): Definitely the formally verifiable one for me yeah

**Micah Zoltu** you think so okay

**Sam Wilson** [14:37](https://www.youtube.com/watch?v=4hii6hcYL3M&t=877s): But I don't think we're ever gonna get that 

**Micah Zoltu** [14:39](https://www.youtube.com/watch?v=4hii6hcYL3M&t=879s): So if anyone out there listening wants to devote a massive amount of engineering time to write a formally verifiable specification for ethereum it's a desirable thing apparently.

**Sam Wilson** [14:51](https://www.youtube.com/watch?v=4hii6hcYL3M&t=891s): Yeah yeah and I mean we have the foundations of the evm and k already somewhere so that might be a good place to start but there's a lot more than that. Yeah I don't think we're

**Sam Wilson** [15:05](https://www.youtube.com/watch?v=4hii6hcYL3M&t=905s): I am sorry it's very confusing because your zoom icon is Pooja's zoom icon and I don't know what's going on with that and it's funny really. Yeah it doesn't switch. It's just he's pushing, so you know if somebody wants to come along and have that ready then I will gladly support switching to it but in the meantime the yellow paper I think is the most useless. An idealised yellow paper I would be much more supportive of using the eip process and obviously I am very supportive of using the python spec in the eip process.

**Pooja Ranjan** [15:45](https://www.youtube.com/watch?v=4hii6hcYL3M&t=945s): So it looks like we are at a point where we have executable specs in python and may be looking for someone who can write specs informally. Formally verifiable specs can be written with the help of yellow paper.

**Micah Zoltu** [16:04](https://www.youtube.com/watch?v=4hii6hcYL3M&t=964s):  Yes but just to be clear that is a monumental task and so while I put it out there if someone like has a background in this and really wants to get involved in ethereum. This is maybe a place but this is like a very big eth. This is definitely not a small little thing. We need someone to help out a little bit this is like we need someone to dedicate two or three years of their life to build this thing

**Pooja Ranjan** [16:30](https://www.youtube.com/watch?v=4hii6hcYL3M&t=990s): Well I think this particular argument gives us some flexibility to go ahead with whatever is available as of now because I understand this execution table spec is being written for over six months and now we are at a place where we are assuming that we will be finishing up with all the upgrades and we'll be reaching a point where we can migrate the process I mean like bring the query ids to this process but if we start today for with yellow paper it will take another  six months to one year down the line.

**Micah Zoltu** [17:02](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1022s): I would say more than  to get formally verifiable. I mean I am definitely not an expert in that area but I would guess years of engineering effort.

**Pooja Ranjan** [17:16](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1036s): 
It's unfortunate that Greg is not here and I am really a little hesitant on coming to a a general agreement. When we know that we have someone who has a different thought. Maybe we can bring it up in the next meeting. But from today's discussion it looks like moving in the direction of python spec. I mean a diff to python spec is probably a good approach at this point anything anyone would like to add on or if there is. I don't know how to put it ? Maybe
 kind of call to action that we can do from the community looking for people who can start working on it or maybe voting kind of collecting some general opinion on what is the preferable. I know we have limited people on the call and we get to hear what they think about but in general if people are looking for getting more opinions we can do that the categories can look into that part but yeah.

**Sam Wilson** [18:30](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1110s): I mean all I can say is you know. I am gonna keep working on the spec well along with the other people who have been volunteering on it and if it becomes useful for the ap process I think we should adopt it but.

**Pooja Ranjan** [18:50](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1130s):  I think working on this executable spec is a very good idea and we should continue doing that. Thank you for you and  your team and so many other contributors who are working on this and maybe we can share the recording of it with some other people and if needed collect some more opinion from different editors and we'll also share it with the client teams if they have any preferences and we'll try to bring it up in the next meeting. Let's see if Greg will be able to join in the next meeting. Maybe we can have a consensus then probably will focus on which particular process to be adopting because I understand we have almost two proposals here. Sounds good to everyone. All right, thank you. 

## 2. Should we discourage the word "standard" in EIP titles and descriptions? Ref: [Issue](https://github.com/ethereum/EIPs/issues/5009)

**Pooja Ranjan** [19:52](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1192s): All right uh moving ahead the next item listed here is should we discourage the word standard in eip titles and descriptions. I have added the issue so this is collected from the eip github repository where we are asking people to add issues which can be discussed in eipip meeting brought in front of eip editors so sam has created this issue and I already see
comments from mike and sam going on not sure if there are different opinions but yes I am if you would like to talk a  bit more about that .

**Sam Wilson** [20:25](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1225s): Sure as an eip editor, I find it incredibly annoying that the word standard shows up in the title of every single standard that's proposed. So I would like to just add a note that we discourage the worst standard in eip titles and descriptions.

**Micah Zoltu** [20:37](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1237s): Can I support that. Yeah I mean you create a pr. I will approve it and then I guess if you create a pr I'll thumbs up it because our approval stuff is kind of broken free eip1.

**Pooja Ranjan** [20:53](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1253s): That's right, yeah so this is basically a proposal to amendment to eip1 and yeah this sounds like a
fair ask. Yeah thank you Micah for suggesting a solution here. Okay let's see if any other eip editors may have different opinions. They may respond to the pull request and we can take it from there.

## 3. EIP [bot Issues](https://github.com/ethereum/EIP-Bot/issues) and [eipv Issues](https://github.com/ethereum/eipv/issues) updates, an agreement on the process to merge & close issues

**Pooja Ranjan** [21:21](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1281s): The next item listed here is eip bot issues and eipv issue updates and agreement on the process to merge and close. So now ethereum cathedrals have been looking into some issues at eip bot github repository and eipv repository. We have Jose on the call who has been looking into these issues and he has been trying to close the issue, so we are looking for a proper process or maybe kind of agreement on how we proceed in that direction. Earlier it was Alita
and she had  the access to maybe close and merge pull requests everything else but now it
is limited um i would pass it on to Jose for his concerns and opinion thoughts whatever he ever observed so far.

**Jose** [22:08](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1328s): Thank you yes each issue 58 and issue 53, they are pretty much the same. Comments could be written in the repos, so you guys can agree on it or not. Issue 55 is a complete modification of the copyedited capacitive of the bot is basically the list for this action has been pretty much close up. There is just one pending issue about the pdf file and I haven't said that this morning. Oh I don't know if this afternoon depends. Panda Pit just comment that basically or maybe we use we just can split this issue and queue one that includes the all the actions already pretty much agree and the other one to open the discussion for the pdf file.Greg was not liking the idea but well I guess that if we just create separate action. We will be able to talk about it and to get an agreement and the last but not least signs. The last call two issues were
closed. Issue 60 and issue 61 that's pretty much about it.

**Micah Zoltu** [24:02](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1442s): I do agree that uh it looks like this enhancements um issue number 55 should be split up into multiple smaller issues that are more targeted so we can discuss them separately.

**Sam Wilson** [24:13](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1453s): Yeah I think actually one per uh numbered item in the comment that I posted would probably be the most appropriate.

**Micah Zoltu** [24:24](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1464s): Yeah I weakened it good 

**Sam Wilson** [24:25](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1465s): I can do that if there's no objections

**Micah Zoltu** [24:33](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1473s): 
none for me i would i would like see it also makes it a little more consumable for new people that are trying to help out allows them to make something easy and tackle it and feel a sense of accomplishment

**Sam Wilson** [24:45](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1485s): 
It's an excellent point yeah so i'll do that i'll split all that up into like 11 or 12 different issues and then we can discuss in the various threads does that work for you. I am assuming Jose but i'm not sure 

**Jose** [25:00](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1500s): Yeah that's fine. Thank you, please also take a look in between 58 a.m and 53.They are pretty much the same. So we can just close one and leave one open as to take that action.

**Micah Zoltu** [25:20](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1520s): 
58 and 63 you say are the same?

**Jose** [25:24](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1524s): 53 53 cta that's the one about the adding or populating the co-owner's file with the editors. Just together they're very very much the same .

**Micah Zoltu** [25:43](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1543s): Is the code owner I see that and then five three is editor approvals required for ambiguous prs is that correct.

**Jose** [25:52](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1552s): Yes when you see the discussion till the end. There was some comments and agreement to basically just
do the same.

**Micah Zoltu** [26:05](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1565s): I see okay yeah I am a little bit behind on . Maybe it's a good segue anything else on the topic

**Jose** [26:26](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1586s):
that's cool for me thank you

**Micah Zoltu** [26:32](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1592s): I am just going to use this as a segue to get into something that's not on the agenda but before we move into the insights and differentiation stuff. I am like two weeks behind on eip editing. I have got my inbox has like 200 emails in it that I need to go through. We could really use a full-time editor. I think Sam does once a week which is definitely helpful like Matt has been maybe once every couple of weeks and that's basically it. I think and so if anyone out there wants to become an eip editor. It's definitely useful. I am finding myself getting burnt out and so and I don't want to put the eip editing situation back to where it was before. I showed up which was that eips would sit open for like a year with no one touching them and we had a backlog of 500 or a thousand prs. I want to avoid that but at the same time I have a lot of other things that I am working on and the eip editing is probably the ones that I end up. Putting off the most and more lately, they haven't put enough more and more. So call out there to anyone who wants to become an ea editor please just start editing and start providing feedback.

**Sam Wilson** [27:59](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1679s):  Make a pr if you want to. The eip one I think is right .

**Micah Zoltu** [28:06](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1686s): Hi everyone there's the file.

**Sam Wilson** [28:09](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1689s): Yeah that one. I think Daniel raised his hand too.

**Daniel Tedesco** [28:18](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1698s):
Yeah hi Micah thanks for that call out and it's something that I am thinking about. I am still  very new and I am something that I am curious about is the like what is the onboarding process for eip editors because I see there's kind of a note about the responsibilities of
editors in eip1 at the bottom and you know I have seen that I have started coming to some of these meetings but I am thinking about you know what is the formal onboarding process like because I think that clarity will help me figure out what I need to learn to get up to speed and also provide clarity on what it would actually detail.

**Micah Zoltu** [29:12](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1752s): So it's a very informal process to basically show up on eips and review them to make sure they follow the rules in the ip1  and follow the template. You can see if you  want to go above and beyond you could go back and look through comments that I have put for example on other people's effects to get an idea of the types of things I look for and the types of things that I follow. I am the same thing with sam or light clients or any other editors. Just kind of if you wanted to look through see what other people are doing but yeah basically just comment on
people's pull requests and say hey fix this and  these things need to be changed. Eth cetera the job itself, the day-to-day of the job is basically just making sure people's proposals are. You know follow a general standardised format and style and so eips are consistent across each other. The kind of more philosophical side of it is and this is maybe just me, so take this next part with a grain of salt.

**Sam Wilson** [30:21](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1821s): Before you continue mike I just want to say like I think the actual technical formal process for becoming an eip editor is making a pull request against that bots file.

**Micah Zoltu** [30:31](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1831s): Yeah that's true, so the bare minimum if you want to be an editor. Make a pull request against the boss file that is being said. Generally we probably won't approve of you unless we've seen you do some editing in advance. So step one is going to build up a reputation within the either community which is very small as someone who is helpful and actually adds value and then step two is adding your name to the list and I will send you a link a pr and add your name to that list or add your github handle to that list and then again assuming you have built up a minor reputation amongst editors as someone who has been helpful and useful. Then we'll approve and you'll now be an editor. It's a very simple process. As far as like
philosophy the one thing that I am a little bit worried about and has probably the number one thing that has kept me from stepping down is that I really want the eip process to be incredibly neutral and this is starting to come up in some of the discussions that we are seeing but one of the ways that I worry and in the past we have lost this for a period of period of a couple of years. I don't want it to be an old boys club where if you happen to know some, know the right people you get your eip has merged and if you don't know the right people you can't get your eip merged and so it was like this for a while where you know if you knew somebody like you knew one of the editors you could ping them out of band and say hey can you merge my eip and that set of people was also given a privileged position where they could just write whatever they wanted in the fb and no one questioned them. So I want to make sure that the eip process remains as neutral as possible and as open to anyone who wants to contribute as possible so that means that someone comes in they submit a pr they're treated equally whether they're a core dev that's been around since the beginning of ethereum or there's someone new into the ecosystem that just wants to help contribute and so that's the harder part of the job because it does entail you know telling some of the old guard. No you need to follow the same rules as everybody else and it also does entail a lot of helping people who have no idea what they're doing learn to contribute meaningfully.

**Daniel Tedesco** [32:50](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1970s): That's very helpful helpful.

**Micah Zoltu** [32:53](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1973s): Make some contributions, comment on things and give people feedback.

**Pooja Ranjan** [33:04](https://www.youtube.com/watch?v=4hii6hcYL3M&t=1984s): I have shared the link of a handbook that contains the information that is not available on eip1 but is a kind of rough process that is being followed around eip editing or documenting an eip or even if needed for reviewing for the proposal, so you may follow that and there is a section how we can onboard an apprentice to be formally added as an eip editor. There you will find the link that micah has already shared in the chat here

**Daniel Tedesco** [33:46](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2026s):
Great thanks a lot. Yeah I haven't seen this doc before I'll take a close look at it. And yeah appreciate the advice on how to get started and kind of build a trust in the community and a profile of someone who might be a good editor. I see the path and and what it entails more clearly now thanks a lot.

**Micah Zoltu** [34:22]{https://www.youtube.com/watch?v=4hii6hcYL3M&t=2062s):
and to be clear the bar is really low for building that trust uh basically just show up and be helpful and useful. You know for a extended period of time like someone we want to avoid as we've had in the past people show up to help out with ending and they like help out for a week and then they disappear in every scene again and so we do want a little bit of a track record just someone who continues to show up and doesn't get burnt out after a week but beyond that there's no really no hard requirements. It's just you know if you're helpful and useful and you're providing good feedback and even you mistake sometimes that's fine.Just like as long as you're showing you know capacity to learn and whatnot the bar really is pretty low.

**Daniel Tedesco** [35:06](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2106s): Sounds great, Yeah I'm the thing that intimidates me is my technical capability but it sounds like a lot of the work doesn't even require that much  technical knowledge  It's just there's a lot of rules to edit the eip so that they're just understandable to the community.

**Micah Zoltu** [35:37](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2137s): Yeah the technical knowledge. Isn't it's we generally want to have someone on the eai editors that is active and has deep technical knowledge but not everybody needs to have that significant value someone can add without any technical knowledge. Just like you know basic grammar checking and formatting and style and you know making sure the rules are followed things like that like things that you really you don't even like it's helpful to know what ethereum
is but technically you don't need to rule. So yeah don't feel intimidated if you're not like an ethereum expert. I think  we have a lot of ethereum experts as editors is because these are people who have tried to make changes to ethereum and gotten frustrated that there weren't the editors and so they joined uh it's not because editors need to be ethereum experts such as experts happen to be the class of people who generally stumbles into the eip process

**Daniel Tedesco** [36:35](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2195s): Sounds great thanks yeah and I appreciate the encouragement. I will  give some of this a try hopefully and be consistent about it.

**Pooja Ranjan** [36:52](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2212s):
Thanks to you Daniel and thank you Micah. On the same topic I have one question
for you maybe for Micah and other eip editors. I see some of the pull requests are open on eipv github. I'm wondering whether we are waiting on something or who needs to approve and get it merged. I'm gonna share the link here.

**MIcah Zoltu** [37:18](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2238s): Eipv was most  recently written by Matt and so Matt would be an ideal person yeah. I mean ideally we'd have more people. I don't actually know anyone other than that who would be qualified to link something different.

**Pooja Ranjan** [37:43](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2263s):
no no actually my question is like now that eipv is moved from Matt's personal repository to
ethereum repository. So I am assuming that now all I mean like obviously you and whoever has this accessibility as an admin for these repository may be able to merge it.

**Micah Zoltu** [38:01](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2281s): Oh so yeah so I don't know who has  admin rights. Is it just ethereum eipv? Right, I can check to see if I do. Alll right I'm checking to see if I have rights to edit stuff. Again sorry. Oh yeah I appear to be on some sort of team that being said I know nothing about rust so I wouldn't usefully be able to merge anything or review anything. I can click a button to to merge but we should definitely have someone else actually read code and changes not me.

**Pooja Ranjan** [39:01](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2341s):
Okay and for the eip bot  how comfortable you are for merging pull request over there

**Micah Zoltu** [39:09](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2349s):
um same thing the one difference is eip bot I actually see I  know the language is written in but I don't actually know anything about the bot itself ideally elita would approve and merge.I
don't know if she's still around though if we don't have anybody I can click the button but again it'd be good to get someone reviewing who is actually understands it in a perfect world for any code base you want at least two people and who get who are both familiar with the code base um to so that way when one person submits change the other person can read it and confirm this is valuable if we don't have that. Ican click the button but I can't commit to doing more than just clicking the button.

**Pooja Ranjan** [39:51](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2391s): No I get it. I was just trying to figure out how we can move forward in the absence of anyone being like a key person who may or may not be around. I know Alita is still around. She sometimes shows up in one of the meetings so maybe we can take help of her for now but
I'm just trying to explore the best way in which we can manage this without you knowing.

**Micah Zoltu** [40:21](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2421s): Sure for the eipv changes so pr number 46. I can merge. I can review and merge that one probably. I'll re-review it and then for number 44. I think we're just basically waiting to get a general agreement but if Alex and I are the only two participating then I can just merge it. Eip I can handle these too the volume is small enough um but don't rely on me for that in the future

**Pooja Ranjan** [41:05](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2465s):
right but if okay. How do people think about having these issues and pull requests even discussed in the eib ip meeting like you said that number 44 is waiting for general
agreement i don't know it's been open since .

**Micah Zoltu** [41:21](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2481s): Yeah we should talk about it, we should have more people here.

**Pooja Ranjan** [41:24](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2484s): of course then I'll start adding it to the discussion items. All right, that's helpful. I was curious how to manage these two depositories because they are not piling up with issues and we don't want to end up in a bad situation there. All right, anything else on this topic. okay if not then probably we can go ahead with the next item. I see a comment from jose sooner than later bart would need additional coding to be merged that's right uh we are trying to figure out a way how to get these codes be merged 

## 4. [EIPs Insight](https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/) - Monthly EIPs status reporting.

**Pooja Ranjan** [42:16](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2536s): All right moving on to the next item. It is eip's insight monthly report nothing much has changed since the last meeting except we have got one new erc category proposal added as draft. The number is a eip4955 vendor-specific metadata extension for non-punchable tokens. There is one small non-normative change to a funnel eip 721 other than that there is one eip
which is in the last call and the last call is ending on 24th april. The eip is eip 1967 standard proxy storage slots, so people if you are listening and if you have any question comment concern related to this particular proposal please reach out to the authors or participate in the discussion at discussion tool link this proposal will be marked final very soon because its last call is ending in next four days. In this month um eip insight I have added the an additional chart to represent the different categories of eips since august 2021 because that's when they started collecting data individually so now we can see how many core erc networking and interface eips are being proposed as new eip and when they are merged I'm considering the data only if it is merged . If it is still in the open pull request form or the data will not be reflected here so that's one new thing and if people want to have different kind of data if looking for any other stats that can be added please let us know in either in the agenda item comment or reach out to me so that's all on eip status reporting.

## 5. EIP editor apprenticeship meeting

**Pooja Ranjan** [44:25](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2665s): Next item is eip editors apprenticeship meeting. This week the meeting was postponed because of dev connect so we are going to have this meeting two weeks from now but a day before on tuesday.

## 6. Review action items from the [previous meeting](https://github.com/ethereum-cat-herders/EIPIP/blob/d65074c7849efe475edd11918850314473114406/All%20EIPIP%20Meetings/Meeting%20053.md)

**Pooja Ranjan** [44:42](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2682s): The last item for discussion today is looking into action items from the previous meeting. Just trying to pull out the notes here. Okay have ci update the creation date of an eip to the date. It was first merged into the eip repo. I remember having this discussion but I'm not sure if we did anything about it. Does anyone remember like what was needed here

**Micah Zoltu** [45:19](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2719s): Yeah, which one was this?

**Pooja Ranjan** [45:22](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2722s):  53.1 okay let me share the meeting notes so it is about um we discussed about the mention of creation date of an eip

**Micah Zoltu** [45:33](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2733s): Nothing I don't think anybody's done anything about that.

**Pooja Ranjan** [45:40](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2740s): Yeah right so i mean i'm just blanking on what was the action item if there was any. Do we need to create an issue in the eip bot?

**Micah Zoltu** [45:52](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2752s):
yes the empire would be where this would go so that would be. I think the next step yes would be to create an issue in the effort repo to automatically add the creation date when a new draft is merged.

**Sam Wilson** [46:10](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2771s): YeahI I will do that as part of splitting up issue 55.

**Pooja Ranjan** [46:17](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2777s): That would be great. Okay the next action is update the bot not to touch eip1. How is that gonna work?

**Micah Zoltu** [46:29](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2789s): I'm gonna do this again. Someone needs to do it if there's not an issue in the eip bot repo. Someone should create one. Actually , this isn't the bot repo already I think.

**Jose** [46:49](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2809s): I'm just  going to add that eip1 if I don't remember well. was any other living for every eip that was the company when they exact 

**Micah Zoltu** [47:05](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2825s): Yeah eip one is the only living eip so something that's updated all living eips or eip1 both would work come okay 

**Jose** [47:13](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2835s):
Excellent, yeah that's true. 

**Pooja Ranjan** [47:19](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2839s):
tokay and the last one is update bought to have minimum two eip authors approval before merge.

**Micah Zoltu** [47:26](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2846s): Specifically that should be added uh you should add the word eip1 to that.

**Pooja Ranjan** [47:31](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2851s): Right got it.  Okay update bot to have minimum two eipod authors approval before the merge of eip1 pull request. Right?

**Micah Zoltu** [47:44](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2864s): Yeah,really before immersion of ambiguous forecast. I think we already have an issue with this. So that one that doesn't need to be an action item. It's basically just need to wait for someone
to write the code to do it. There's no action right now, we're just waiting for someone to write code.

**Pooja Ranjan** [48:09](https://www.youtube.com/watch?v=4hii6hcYL3M&t=2889s): Okay okay maybe I will look into it and revisit these items next meeting. Hopefully it will be done closed by the time but yeah we'll revisit it and I think that's all that concludes the meeting for today. Anything else anyone would like to bring up for today's discussion. Well we made quite good progress. Now we are at some clarity with executable specs and core eip process. Now we are looking into some general consensus. Maybe we will be able to discuss it further in the next meeting and look into the proper path for moving in the direction of pulling out core eips or leaving it in the same repository, so maybe we'll have a decision not decision general consensus as I say in the next meeting. So we made quite a good progress and yeah that's all I think I have to share with you guys today. Thank you everyone for joining and see you all in two weeks. Thank you.

---------------------------------------
## Attendees

* Micah Zoltu
* Pooja Ranjan
* Sam Wilson
* Daniel Tedesco
* Fireflies
* Jose

## Date for Next Meeting: 4 May 2022 at 1500 UTC.






