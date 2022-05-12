# EIPIP Meeting 55 Notes
### Meeting Date/Time: Wednesday, May 4, 2022, at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/130)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=aqJCBdfgx2c)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION/DECISION  ITEMS

**ACTION 55.1**: Collect feedback from the Core Devs for making Diif in Python 
**ACTION 55.2**:  Collect more info on Pandapip1’s comment
**ACTION 55.3**: Jose will create pull requests in EIP bot Github. 

 
—------------------
## AGENDA

**Pooja Ranjan** [0:01](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=01s): Welcome to EIPIP meeting 55. I have shared an agenda in chat.

## 1. Core EIPs in an Executable Spec World [Proposal](https://notes.ethereum.org/@timbeiko/executable-eips) and [Discussion](https://ethereum-magicians.org/t/core-eips-in-an-executable-spec-world/8640)

**Pooja Ranjan** [0:05](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=05s): The first item listed here is core eips in an executable spec world. We have added the proposal to the agenda. So this item is under discussion for the past few meetings now and there has been some async communication also. It can be found in the fem link which was added to the agenda in the last meeting. 

**Micah Zoltu** [0:30](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=30s): we can wait for Sam.

**Pooja Ranjan** [0:35](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=35s): That's right that's right. Sam I think he said he will be joining and today we are expecting oh Greg is also there but looks like he's

**Micah Zoltu** [0:48](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=48s): Greg's also missing. Let's come back to this one after some of the others.

**Pooja Ranjan** [0:54](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=54s): That make sense, we can move on to the number two and we hope that Sam in the meanwhile will join. Also Greg will be back too.

## 2. Discussion items from different Issues. Ref: [Comment](https://github.com/ethereum-cat-herders/EIPIP/issues/130#issuecomment-1113283663)

**Pooja Ranjan** [1:03](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=63s): So the item number two added here is discussion items from different issues. This is added on the request of a community. Contributor Panda eip1 though he could not join the meeting today. He did mention that he will be following the recording and the list that we have here is of open issues and pull requests at different ethereum repositories based on his priority. What he thinks will be of priority. I am gonna just read them and maybe eip editors or anyone who is working on these issues if they have any updates. They can share it or maybe propose any possible solution. The first one that is a bug currently and is of higher priority it seems updating workflow files should use stricter rules and the issue link. 

Here is eip bot issue number 79. So this issue I mean this particular item, I think we discussed it earlier. I see a lot of like comments going on. Anyone has any update there or would like to add anything on that. All right I think this is about the two editors' issues right. Currently only one editor can add or remove any of the existing eip editors and we discussed in one of the earlier meetings that we should have at least two editors or more approval needed for making this function work. I am not sure if we have got this done. Yeah. 

**Micah Zoltu** [2:54](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=174s): I always need someone to do it a lot of these are. I think find them we just someone has to simply take the time to do them.

**Pooja Ranjan** [3:03](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=183s): That's right, I am also expecting some more people to join today. Maybe one of them may be able to help out with this. Though we already have someone also looking into issues. We can find the comment there. Okay definitely we know that this is one of the highest priority items so if
 someone is available to work on that we will make this off one of the highest priority item to
look into .

**Jose** [3:31](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=211s): I will comment about it when we go to the eip boat section in the agenda, seeing that it is the next one.

**Pooja Ranjan** [3:41](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=221s): Okay that sounds good. Mike I am just curious, do you want me to go through all the items listed here or is there anything that we can pick up particularly? I mean  I am happy to read. Let's just go through it. The next one is cannot delete files in asset folders, so again this is already added to the eip bot repository. I am expecting Jose if you may have any updates on that. You can probably share it and if not then whoever will be joining to look into these issues maybe look at it at higher priority.

The next sub item listed here is eip 5069 eip editor apprentice handbook in eip form so recently we have noted this new pull request number is 5069. This  user has documented a hack md file created by me where I have collected all the information related to how we can have new eip auditors on board. He is trying to make it as a meta proposal and he has put it into a template that is available for creating any eip. I am curious to hear what are the thoughts of eip editors here.

**Micah Zoltu** [5:16](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=316s): My thoughts are the same as always with meta and informational eips. I feel like they should go somewhere else but as always I think I am alone in that and so if one of the other editors wants to merge I won't stop them.

**Gcolvin** [5:35](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=335s): There was a really long discussion of that which I didn't participate in. I am sorry about Amsterdam and preparing for Amsterdam and recovering from Amsterdam took up all my time but eips and ercs have been in the same repository and used the same numbering for so long. I don't see any hope of changing that yeah so I don't know

**Micah Zoltu** [6:05](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=365s): I don't think this proposes a change that doesn't.

**Gcolvin** [6:09](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=369s): I have really lost track. They need to be divided in some way just because there are so many possibilities for ercs so there's lots of them and there's just a lot fewer core eips and a lot fewer people who are competent to really understand them and well like myself.  They're the only ones i'm interested in reviewing.

**Pooja Ranjan** [6:44](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=404s): Well this particular proposal is not related to eip and erc. Probably we can discuss it when we go back to item number one. We were waiting for some more participants to join so we skipped it but this particular proposal is about how to onboard eip editors.

**Gcolvin** [7:05](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=425s): I got lost while I was pouring my coffee so we'll come back to that. I am sorry.

**Pooja Ranjan** [7:10](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=430s): Not a problem so yeah if there are any other thoughts on like do we need this kind of meta proposal or first of all do we need this as a proposal because this was just a hack empty file that we were sharing earlier yeah and if we want to like kind of formalise that we may use some kind of eip and if that at all it has to be an eip. Should it be informational meta so yeah

**Gcolvin** [7:36](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=456s): It didn't used to be that formal but there was simply some discussion among existing editors and a consensus reach that a new person should join and it was loose enough that I recall simply adding macaw out of frustration that there didn't seem to be any other editors but me for a while. So it'd be good to tighten it up a little but I think there should be some consensus of all the existing editors. It doesn't have to be a big deal or a formal thing.

**Pooja Ranjan** [8:19](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=499s): Wondering if anyone else has any thoughts. I don't see sam on the call but yeah lifeline if you may have any thoughts on this. Yes Tim please go ahead. I am not sure if the lifeline is okay? Okay he's using text. Please go ahead Tim.

**Tim Beiko** [8:47](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=527s): Yeah, is this about essentially this is about adding another eip editor or this whole erc?

**Pooja Ranjan** [8:57](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=537s):
so this is about adding an eip editor. The proposal here is like whatever hack md file that we were referring to earlier where it is documented how we are doing this, the internship program, how we are running it and the steps that we are following to onboard an editor. He is just proposing to have these things publicly available not in the form of hack md but in the form of eip, which may be stored on the eip repository. So I am just curious to understand what people think about this particular proposal.

**Tim Beiko** [9:30](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=570s): I don't have a strong opinion but it feels a bit weird as an eip but yeah I am not sure why I can articulate why it just feels. I guess because it's like a process thing and not like a actual ethereum thing but it's a very strong opinion .

**Pooja Ranjan** [10:00](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=600s): Right yeah and and this proposal is proposed as a meta eip which is again for all process thing though I am also not able to comprehend it completely. This user has used my document and he reached out to me that it is fine to have him added as an author. Obviously if you are doing the leg work if you are championing a proposal you have to be a co-author of that. Maybe we can wait for review comments from other people like other editors because it is already added as a pull request. We can expect something going forward. All right we can move on I suppose.

The next one here is forced usage of the included licence file and they have added an issue on ethereum eaps repository wondering if anyone has started.

**Micah Zoltu** [10:59](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=659s): I have comments on it already.

**Pooja Ranjan** [11:07](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=667s): Okay so a few meetings ago, we mentioned that if there are anything that people would like to be discussed in eipip meeting. They can probably list it here on the eip's repository issue section because we are strongly discouraging people to create an issue for eip's discussion. So all the issues here are listed from there feel free to drop a comment over there on the issue that is linked. If you have any opinion, strong weak whatever but whatever can help us close these issues faster.  Similarly I see there is another issue created that is for automatic redirection of old type urls.

**Gcolvin** [12:02](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=722s): I am not using issues. I keep getting confused on just how to introduce an eip especially core eips because we have a section on the magicians where discussions of core eips go but in general  you may want to introduce discussion of an eip before you've actually introduced one with a PR and asked for a number and so you get in this loop where you can't start the discussion of a core eip with a number until you have a pr with a number. So you wind up in this loop and the issues made. It is possible to get started on a discussion with a number that you knew was going to be assigned and start the discussion in the correct place in the magicians.

**Micah Zoltu** [13:16](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=796s): So you can definitely start a discussion in the magicians forum. You're correct. you won't get a number. Is there a reason you need a number to start talking about it?

**Gcolvin** [13:28](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=808s): Look at the core section of the eips and I think the all there includes the number or somehow related to it so you can't really get something started there until you get an eip number it's not cause I believe there's

**Micah Zoltu** [13:51](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=831s): I don't believe anything stops you from creating without a number and so you should be able to and then I am pretty confident that we fixed it. So you now can edit infinitely like you're no longer limited to only be able to edit within the first like 10 minutes or whatever so you should be able to just create create it with a description as a title fill it in talk about it and then once
you get a number you can go back and edit the title to include the number. 

**Gcolvin** [14:11](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=851s): So where do you put your initial draft of the eip before you're ready to actually. You know actually make a pr on the repo.

**Micah Zoltu** [14:28](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=868s): Ethereum magician's thread that you create just like in the original post . We fixed the issue that you brought up that you couldn't edit. I agree with you that it was definitely not acceptable um so that should be fixed.

**Gcolvin** [14:39](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=879s): So you should be able to iterate it on it right in there at this point okay so that's been fixed

**Micah Zoltu** [14:46](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=886s): Yes if it's not fixed let's let me know i tested it and it worked for me but I may have more permission so it doesn't work for you definitely tell us because it should be fixed. 

**Gcolvin** [14:57](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=897s):okay well if you can do it there and keep editing it to keep it up to date and then remove it and put a link to the actual  draft when the time comes that works very well. thanks.

**Micah Zoltu** [15:13](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=913s): Definitely let me know if it doesn't work right 

**Gcolvin** 15:16](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=916s): I am sure it does it's no big deal. If it doesn't it's it's mechanical.

**Pooja Ranjan** [15:27](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=927s): Yeah we hope that issue is fixed. I see Daniel muted unmuted. Do you have something to add here? I know you are also working on an eip right?
**Daniel** [15:40](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=940s): Yeah I was just going to say I know you can create draft pull requests that you know that might be a way to have a draft but not have it being reviewed or clogging up any kind of processes and you could just point the discussion to that drafted requesting magicians. Until you're ready to make it official but it sounds like that's not the only way to solve this issue.

**Pooja Ranjan** [16:16](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=976s): Right, that is also a very good point because earlier when we used to have drafts. Draft was the only status before it can be moved to the last call now that we have a review as a status. So people can always create the initial pull request as draft and when they are ready keep it in draft and once they are ready, they can move it to review for editor's review. 

**Gcolvin** [16:39](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=999s): Yeah I am just thinking of the ideas that are often vague enough. They're never going to get to an eip and you don't want to clutter up the repo with draft pr's issues used to be a good place to say. I think this might be a good idea for an eip and start a discussion and that's a magician's is a good place for that too.

**Pooja Ranjan** [17:02](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1022s): All right,  okay going back

**Gcolvin** [17:14](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1034s): Plus the whole pr process is difficult enough that the people don't want to have to learn how to do it until they have to.

**Pooja Ranjan** [17:28](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1048s): All right going back to the last item. It was 5056, I know that there are a few comments related to this particular issue that are already available in the link that is provided in the agenda so if anyone has any comment or suggestions to handle this one. Please look into that. No Tim you did not the first item. We are just coming back on it uh because we were waiting for some more people so we thought that we can quickly finish this up. I think we'll take another five minutes or so and we should be going through all these small items and then we'll go back to our item number one again.

The next one is to merge ethereum cat herders into an ethereum org repository. I suppose this is a very big proposal. It's good that we have many people on the call who would love to hear thoughts on this particular item. I know I had a chat. Oh yeah let me first mention this I had a chat with Tim earlier and we were thinking about how to make sure like  we can have a backup of some of the important repos of ethereum categories repository and we did discuss about eipip to be considered one but I am not sure like it was discussed to move all together into ethereum um yeah please go ahead micah sorry for introduction.

**Micah Zoltu** [18:50](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1130s): I don't hold a strong opinion on this either way but I don't see a clear or strong need for it. So for me I don't.Ii would like to see more on why this would be beneficial like what would we gain from such a move.

**Pooja Ranjan** [19:13](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1153s): Yeah that is an interesting point and I would love to hear more thought on that though I could not 
connect with this person like to have a long chat. He said that his availability will be more in the next two weeks. He has some exams so maybe when he's around or if we have more information on that we can probably bring it back. But yeah if anyone has any kind of opinion like whether it should be or it should not be. They can definitely comment on the issue that is listed here and I find a few more items, three more items that are already listed here and one of them is a bug which is again eip bot. I think we can cover that in the next item it is eip issue number 77. So we can probably discuss it over there. Okay all right so in the essence of time and now that.

## 1. Core EIPs in an Executable Spec World [Proposal](https://notes.ethereum.org/@timbeiko/executable-eips) and [Discussion](https://ethereum-magicians.org/t/core-eips-in-an-executable-spec-world/8640)

**Pooja Ranjan** [20:19](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1219s): We have a lot of people here to discuss item number one. Maybe we can go back to the item. Though we didn't have Sam on the call yet. I am not sure if he'll be able to make it though. We have left a message for him, so let me go back to item number one and see what we have since the last. As I was mentioning that we have been discussing this item for the past few meetings and we have a lot of discussion, so if anyone is interested they can go back and refer to the recording of earlier meetings. From the last meeting it seems like uh greg colvin has some concerns and we kind of discussed what is the current situation with the python specs as well as with the people who will be able to understand the yellow ethereum yellow paper. It looks like current availability of resources such as that moving towards having diff to python specs is comparatively better because we have more audiences who can probably understand python than who can understand the current yellow paper but because Greg was not there last time. So we wanted to bring it up again to the meeting today,so yeah feel free to share your thoughts opinion concerns

**Gcolvin** [21:37](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1297s): Me yeah I spent a fair amount of time with Sam Wilson going over that kind of view 615. Just as an example because it's fairly long and brought home. Some of my concerns, sort of the central concern is just that python is a bad language for declarative specifications and you know 615 as an algorithm for instance, for validation but the specification is almost entirely declarative. If you look at the wasm specification, it's a hundred some pages of totally declarative specification. It has a very short algorithm at the end for validation but it specifically said that's not part of the specification. So having python code for implementing a spec doesn't work as the spec itself.

**Tim Beiko** [22:50](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1370s): Well we already have that for the beacon chain though like we kind of have a counterexample that it does work great and I mean Sam's stack works to implement ethereum basically all the way to constantinople now, so I guess I am not sure what I am not sure understand what you mean but like it doesn't work to implement the spec.

**Gcolvin** [23:17](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1397s): If you have a reference implementation, yes other teams can basically port the reference implementation but you can specify things without writing the code. You write declarative specification and then any code that implements that specification is satisfactory and if you're using a procedural language like python the port is relatively straightforward. If you're using a non-procedural language. I guess haskell you basically have to reverse engineer a declarative specification from the python and then implement it from that.

**Tim Beiko** [24:08](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1448s): And is that are there any clients for whom that would be the case

**Gcolvin** [24:14](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1454s): We went back to 615 and to go from the algorithm to the spec you just wouldn't get there. The spec provides you know rules on how you must write your code and you know in order for the code to be safe. You must follow certain rules, the stack must be laid out in a certain way, things like that and the yellow paper can specify things declaratively because it uses fairly ordinary mathematics. The mathematics it uses is really pretty easy um topolous and set theory.

**Tim Beiko** [25:06](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1506s): So you're saying it's not possible to say specify something like eip 6150 615 in an executable spec in python if that is that right.

**Gcolvin** [25:20](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1520s): I wouldn't know how to do it. I don't write python very well at all. I know I can put together simple scripts and struggle through the beacon chain code but languages we have for doing declarative specification are basically english maths and that's about it for our team. There's formal languages that people use but they're gonna be even harder than python english generally works pretty well and eventually that winds up in the yellow paper

**Tim Beiko** [26:03](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1563s): Right but I think that one of the challenges when we talked about this was about cordevs with english. Martin being brought up is like it leads to a bunch of eips being underspecified right like whereas if you have to actually work through like a full implementation. You by definition have to specify it in code and then the question of like you know python versus other programming languages. I think it is a bit orthogonal to that but I think from when we presented Sam's work on our core devs. There was a pretty strong consensus that having a spec which is in code provides less ambiguity and one of the annoying things for client developers is when a new eip comes in and it's just underspecified and they actually have to 
figure out what the author of the eip intended based on the kind of their English or declarative specification which doesn't have everything.

**Gcolvin** [27:01](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1621s): Yeah I understand I worked with a couple of you know formal analysis experts to go through that and get it as correct as possible and off to the side we did have some. You know some formal specifications but they wouldn't help. Most of the core developers either partly if we want to do this,  I would want to have a person or small team of persons who's willing to work with people doing core proposals to help produce this python. It wasn't clear to me whether this was a full implementation of the client. So you could actually test it. Is it a full implementation, yeah it is okay. Then we get the hassle that the initial implementation is likely to be in some other client.You know work I do would probably be either in the c++
client or the go client so I might have a pr on a you know complete implementation but it's not going to be the python client especially if i'm doing performance work on geth or something it's it's going to be irrelevant to python um but there

**Tim Beiko** [28:31](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1711s): I think there's two things there so it's like sure a pr that improves death performance that's not like a consensus change right like it's a it could be.

**Micah Zoltu** [28:41](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1721s): Gas engulfing for example you need to know what. We're not going to use the python client for figuring out how much gasoline should cost.

**Tim Beiko** [28:49](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1729s): Not sure but I mean you're going to need to use it if you're pricing gas for upgrades. you're going to need to check multiple clients anyways right? So it's feels like there's kind of a weird gap where like yes you know like you may choose to implement something and go first because you're more comfortable there.The base you team would tell you the same thing about java
But I think the question is then what does the full specification get written in which is different from the actual client implementation and I think the goal here is we can have the full specification written in python rather than like english or pseudocode basically which is kind of the case today.

**Gcolvin** [29:36](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1776s): I have got  eips in progress which are declarative English, which once it's worked out will be a complete specification. You don't need any code for that specification to be complete. It's English so that's problematic but using a formal specification language is also problematic. Wasm solves it by having both english and formal spec and a promise that the two of them mean exactly the same thing and that it took some very good people to do that. They don't have a reference implementation as far as some eips. I currently have on the table the reference implementation will almost certainly be and go because I would want have been and would
I want to continue working with Martin in the caf client and or the turbo caf client, so by the time I am done I have a working tested implementation and then if I am told oh you have to port this to python. I am going to  put a year of work into this go and I don't really know how to write python very well and so I am sorry. What am I supposed to do to learn python, well enough to do this? No I can't.

**Micah Zoltu** [31:14](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1874s): I think that's going to be true no matter what language you choose so anything we choose there will be a set of people who do not know it. So if we choose python there's a lot of people who don't know the python features. Go to some people who don't know, go if we choose if there's going to be some people who don't know F. I think that is an unsolvable problem like the fundamental kind of underpinning of what you're getting at and that leaves us the question okay so which do we choose and we can we could choose a formal something you know r or whatever it is or something. It can be formally specified the reason for python. I think it is just that it is the most likely language that most people will be able to know or figure out. I mean there's a reason people use it for teaching right because it's relatively simple and not too complicated and doesn't have a lot of weird edge cases. I mean it's not a perfect language. I don't use it for example but it's not hard and so I i think that i mean my argument here is basically that we're not someone's going to be unhappy in this case it's you and
probably some other people as well. I am sure there's other people that don't want to write in python but I feel like this is kind of optimising for the least total unhappiness across the core dev space .

**Gcolvin** [32:23](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1943s): No you're not getting it. I am sorry.

**Micah Zoltu** [32:28](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=1948s): Well so then there's I think there's the other aspect. we're saying I do agree with which is that a declarative specification would be better. I agree the problem is that getting someone to write and maintain a full declarative formal specification for ethereum is hard. The yellow paper was supposed to be that and it was totally under maintained, no one could read it. I shouldn't say no one, many people struggled to read it and we want something that's approachable and accessible and so we have to make it. So the choice the question is is do we make a sacrifice in. We were sacrificing what you said. Declarative is better but we're sacrificing that in order to increase accessibility and approachability and simplicity and things that people are more likely to be familiar with and again I want to make clear I do agree with you that.
Something formal would be better if we had infinite resources and we didn't have to worry about  ramp up time and onboarding time for new eip authors stuff  that and so i think it's python is just kind of an  optimization for lowest common denominator I guess you could say 

**Gcolvin** [33:37](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2017s): It’s worse than that. I have eips that cannot be expressed in python, an algorithm for validating that code follows certain rules. Can be written but reverse engineering rules out of the algorithm would be very difficult stating the rules in an english statement.

**Micah Zoltu** [33:59](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2039s): Right my information would be to write the rules in english or whatever you're familiar with you can write them in the eip. I don't think it is limited to only having the python. It's just it must have at least the python and so you could write your eip perhaps initially without any of the python. You'd author it. Get it as a draft. You might not allow it to go to the reviewer last call without the python implementation. But I definitely would accept a draft without a python implementation and so you can, you know, write it in something you're familiar with and have a declarative all that and then maybe as a later step once  you know you kind of sold some people on it. Someone can come in and help you or actually do the python implementation. So that it satisfies the requirement of it has to have the python update that's my thinking um may have other thoughts on that though because process wise.

**Sam Wilson** [34:47](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2087s): Yeah that lines up with what i am kind of imagining

**Micah Zoltu** [34:55](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2095s):.
does it make sense to have a pr that doesn't actually change the executable spec

**Sam Wilson** [35:00](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2100s): As long as I mean as long as we. Okay because there's a couple ways you could do it right? You could do it so that you just make the markdown file and don't make any changes whatsoever to the executable spec. You could make the markdown file and change the dock strings of the relevant functions which I think doesn't really require knowing much python. Just enough to be able to find where you want to make the change and I think you know having different levels of. I don't know where the line should be drawn maybe zero python is probably the best option but yeah there's different places you could draw

**Gcolvin** [35:44](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2144s): I can't do this. It's just but one thing so I could look I could show up with an eip that uses english and
you know whatever seems appropriate to present the idea clearly enough that it can be implemented. I might at some point and I might not do it until I first get it to cfi. Then finish off a complete working implementation in one of the clients and damn that's a lot of work already and there needs to be a complete implementation. If you're doing something that's supposed to improve performance you need to show. It does prove performance in the important clients at that point you've done a lot of work and then you're told you've got this go code. You have the c++ code. Oh! you have this java code and before it can be any ip. You must translate this code to python and it's just. No, that's too much work. Well I think the other team doesn't really if another team who is the python team says don't worry, we're the python team now we'll work with you to finish off the spec. But it really seems up to the core devs themselves whether respect is ready for them to implement whether they really need this. It's not really for the eip editors to decide what the core devs need that the original concept was, you know pretty much that the core devs are operating independently enough of this process um that it's up to them what what they find acceptable

**Micah Zoltu** [37:47](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2267s): So I think that part of the reason that things came about is the frustration from the core devs that we have a lot of core eips that are under-specified. We don't find that people implement them in different ways because they're written in English and so this is an attempt to solve that problem.

**Gcolvin** [38:03](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2283s): Fine I can just withdraw some eyepiece or ask for a lot of help.

*Tim Beiko** [38:11](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2291s): I think it's okay to ask for help right? Because in practice this is what everyone who's not a guest dev does today right. They have an eip that they come up with and then they have like a specification which is usually english or some like underspecified format and they usually need to get  help from one of the client teams to like actually implement this in guest or at
at the very least review it or whatnot and I think I see your point that like you for a draft or something it's probably reasonable to not require a full python implementation. My personal line would be for us to move something to cfi. You would probably want to have that and then it's by then you know if we're actually thinking about moving this eip to cfi. Tthere should be somebody who's willing to help you with a python implementation if you can't do it yourself. But it seems  safe for drafts and for discussions. I appreciate that that creates a ton of useless overhead. And we shouldn't impose that on people. But yeah I think  to move
to cfi or at the very least  to move to be included in a hard fork then you make that a hard requirement and other people at that point might might be able to help if  the eip champion
is blocked by that specific task which is the case today for a bunch of eip champions for say the actual say death implementation or other kind of improvement issues.

**Gcolvin** [39:51](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2391s): Well also
the people who are maintaining the python client.

**Tim Beiko** [39:59](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2399s): Sure but you would ideally not dump it all on them. I think it's a bit unsustainable to say. Yeah the people maintaining the spec need to be the one like i think it would be good to have the norm or it's a bit of a broader set of contributors.

**Gcolvin** [40:16](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2416s): Okay well
Again you can write entire specs and depending on the subject of the spec.They often need to be declarative that the specifications are declarative and python is a bad language for doing that. And I remember this discussion years ago on the c+ committee. There was a lot of pressure for us to define it with the formal language.I think z was the popular one at the time and there would have been advantages. The problem was that we would have a specification that very few people in the world could actually read and we decided to go with English ordinary maths such that people could actually read it and there would be some ambiguity so it would be a job. We had a small subcommittee whose job was to disambiguate the English if and when issues arose and  you know in our case we were specifying a language so examples and such would be in that language and when we could specify things in that language. But I don't know if 615 remains an example. There's a validation algorithm but you could slice it off. The proposal and formalists were able to go through it and write complete formal specifications based on the english help me get the english cleaned up and it's a totally adequate formalisation and writing a validation algorithm in python rather than a pseudo c. Fine it would be more readable and it would not be a specification you'd have to reverse engineer. The specification from the python 

**Micah Zoltu** [42:23](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2543s): Definitely for something like 6.5 I definitely don't think that you should remove the specification you have like the english language version. I think the only requirement here is that there is also a python reference implementation functionally like this that does not preclude you from also having you know better stuff. It's not even a declarative language, something in English and something I don't know. Whatever the popular declarative languages are these days like that's acceptable it just also has to have the python reference implementation.

**Gcolvin** [42:53](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2573s): So basically to write that I would have to learn enough python to write what might be a fairly difficult algorithm. Yeah in python and learn to wait a minute and learn how the reference implementation works well. Enough to make a pr even if the pr actually involves fairly
substantial changes to the reference implementation. You're asking an awful lot of people that unless you know unless the executable spec team itself is willing to help when I am working with the geth team when I am working with the c++ team and they think it's good. 
you know a good thing to do or to investigate they help me you know I am not left alone.

**Micah Zoltu** [43:53](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2633s): I suspect that would still be true for the python teams as you put it. I did the reason I don't want to say you will get help is because I want to avoid the trap of saying every single person who wants to draft a queer eip gets a slice of the python team's time. I want to make sure we don't fall into that trap because there's you know hundreds of eips that never make it anywhere and they're terrible and we should not be dedicating resources to those people. There are definitely some eips that are going places and we want them to be included. I don't know. Let's take 1559 as an example because it was very popular for that. It would have been pretty easy to find someone to do the python implementation or help you with it. 615 may also fall into that  bucket. There are a number of people who are interested in that. We just need  one or two of them to know. Help out or the python team may interest themselves and they can help out. I don't think anything precludes you from getting help from people who are familiar with it. I just want to be very careful. We don't promise that because that can lead to worse problems I think .

**Gcolvin** [44:54](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2694s): Well at what stage then? At what stage are the core devs insisting that they have some python before they'll go to cfi.

**Micah Zoltu** [45:08](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2708s): My personal preference on this is that it is acceptable to approach. The core devs with an idea that is you know reasonably well described and ask them does this interest you and if we
push this through you know is that likely to go through or is this going to be something that no one wants to implement and I think it's very reasonable to not have a python implementation for that. I think once you cross that phase I would argue that the next one of the next steps before it gets implemented by all the clients is the python reference implementation again because the idea is we want to make it so it's relatively easy since all the current clients are procedural. It's relatively easy to port python to them and so I think that's why we want somewhere between between the core dev. Say yeah we're interested in that and the coordinates say. Okay we're going to go implement that we want the python implementation and that's my personal preference I am sure other people have other videos

**Tim Beiko** [45:58](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2758s): And so that would be just like process wise that would be after something is cfi so take 615 as an example we could say we consider 615 cfi for the next hard fork as is with just the go implementation but then prior to all the client teams or  in parallel perhaps to all the client teams implementing it and prior to being officially part of the hard fork. Then you make it you have the python implementation and I think this also has the needs property that you get different people who can review the python implementation as things get included in hard forks and that's like a valuable thing Yeah!

**Gcolvin** [46:45](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2805s): Well so you're saying it's not acceptable to show up with you know with it working in any other
Client

**Tim Beiko** [46:56](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2816s): well you're gonna need to show that. It's a good idea right and if the way for you to do that is showing it working in another client because it's like a performance optimization then like that's kind of the way you convince core devs that this is actually worth doing but I think
from that point up to  before everyone has done it that implemented it then is when you also
need to get it done in python either by doing it yourself at that point.

The next I can do it and again at that point it should be a bit easier to do that because other people should want the eip to also go in the next hard fork and be kind of incentivized for it. Yeah and one of the reasons I guess why I am pushing so hard. I think there is  also a large set of potential core eip champions who are not client devs and for whom  this is much better. I was talking with uni swap yesterday about their eip and they struggle to get it implemented in geths and all these other clients which have nothing to do with the type of code that they usually write. So I think python is much more accessible for all these folks who like to work more at the application layer and have changes. They want to propose back down. So it's not and it's not perfect for anyone but I think having it at this point where you are kind of deciding whether something goes into the hard fork seems rough. The right spot but I agree with Sam in the comments that we can just ask all core devs and see what client developers prefer.

**Gcolvin** [48:35](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2915s): There's nothing wrong with doing it that way. That's a great way to write one if it's the best way for someone to write one but it just seems like it if you don't really need it. If you've already known if you've already implemented another client to then say well fine but you also need to implement it in the reference client. It's just like it was hard enough to do it in one client and unless the core devs are saying no. We must see it in an executable python when really in the past people have been able to work this out and once everything is a consensus on the net. It just doesn't seem to be as big an issue as we're making it to be the quality of the eips coming in is an issue but the core devs are quite free to push back and just say we can't understand the eip well enough for. Whatever reason and having it written in python may or may not help you can write really bad python.

**Pooja Ranjan** [49:56](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=2996s): One other point that I would like to bring up here generally. We consider four at the ,six core eips for any upgrade and considering if we are having even two upgrades in a year and we have one or two proposal which needs help like i have it documented in python that can be provided but I totally agree to Tim's point that we should not be making it a burden to team who are maintaining their specs for python but in my understanding uh this is something doable and if there is any help needed to push a proposal now when it is considered for inclusion so cfi be generally from the process point of view um such as that proposal should be in  review and ideally to have a spec written in python in review status when it is ready to be shared with the code would be good to have but if not I think it's just reference implementation and you can share that with code apps and if it is acceptable then someone may help you out with having that in python and you can proceed from there.

**Gcolvin** [51:03](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3063s): Well the core devs will pull the courthouse and are free to pull anything into cfi and they will pull at just a draft stage if the draft is clear enough. 

**Pooja Ranjan** [51:21](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3081s): Yeah that's right. That's a fair point and that's what gives us this flexibility of if we need to have that documented in python. You can get sufficient help to get it done.

**Gcolvin** [51:35](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3095s): Okay I object, not enough to block yet but I do object. You know eips need to be clear and well written but I don't.. I don't think that just requiring python will necessarily achieve that goal and it puts a big barrier on a lot of people including me.  

**Pooja Ranjan** [52:03](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3123s): Well noted. I think this is a fairly good discussion and that we are trying to discuss both the points. As Tim and Sam I think I read somewhere in the chat that it is good to check with the all code meeting is more what other clients think about it because we try to come up with a decision on  based on general consensus  whatever is good for a big number of people like a majority of people who try to move ahead with that so for now like because we have specs available in python. It seems we are good with there but definitely we can make a final decision after code. What do they think about it?  Anything more to add to this discussion?
Especially related to having it in python and not in python because I know at some point Sam mentioned that if it is so contentious then we can probably drop it and I just don't want to drop it just that before we have  a very very good reason to drop it.

**Gcolvin** [53:12](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3192s): Yeah I think we're finished with it for now.

## 3. EIP [bot Issues](https://github.com/ethereum/EIP-Bot/issues) and [eipv Issues](https://github.com/ethereum/eipv/issues) updates, an agreement on the process to merge & close issues

**Pooja Ranjan** [53:17](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3197s): That's good. I think this is something that cannot be closed in one week or two. Maybe we will have to work on this adjective, so we will come back again on this topic next week. Not this particular one but I know. Tim has joined here and we are also looking for some support on the ethereum process as an overall  help there. So yeah Tim if you would like to take it from here and talk about how we can probably add  more support to existing processes in terms of if we have to move ahead with this execution spec. We'll be looking for more help in eip bot and other sections.

**Tim Beiko** [54:04](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3244s): Yes, so we have Mario today from our team who can probably help with some of these issues. I don't know Mario. Do you want to introduce yourself real quick?

**Mario Havel** [54:15](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3255s): Hey folks I am Maria Havel. I work with ef with demon training vertical support. Yeah and I have been looking into the eip bots. I was listening to the call from January to get some overview about the bots and there are well multiple of them. There are multiple issues and  this eip is in javascript. I am not really experienced with that. The eipv one is in the rest. I might be able to help there. So I will look into it more and and try to try to solve some lowering issues.

**Pooja Ranjan** [54:59](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3304s): Awesome so did you mention that you would be more comfortable with eipv because I know there are a lot of open issues and also some pull requests that need some reviewing before merge.

**Mario Havel** [55:09](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3309s):
Yeah exactly. It's the eip verifier validator right? Yeah well later on so because I am just
much more experienced with rust than with javascript. So it would take me a while to pick up on the other one but I was already looking into this one and  Yeah i'll be glad to contribute.

**Micah Zoltu** [55:39]((https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3339s): So we've been discussing slowly migrating the eipv over to the eip bot however so on the one hand I want to say you know we should be careful about syncing to merge dev effort into eipv. If we're just going to eventually deprecate it. On the other hand we are desperate for help and people and so if we have someone who wants to help and rest is what they want to do then. I would rather keep eipv and not deprecate it and instead get the help if that makes sense.

**Mario Havel** [56:12]((https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3372s): Yeah sure you have to get it. Yeah I mean let me see if I will be able to figure out something there. So what would be the timeline there? When would you imagine to have the eipv duplicated if there are contributions.

**Micah Zoltu** [56:29](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3389s): If there's no contributions to either of them then neither then they will both continue to live on forever. It's we have been working on slowly very slowly adding features to the bot that overlap with eipv until eventually at some dispoint in the distant future eipv could be removed because it's fully handled by the bot. Again though that that process is very slow and I would rather take the help where you can get it and so if  you're passionate about rust and you hate typescript then I would much rather get help on the eipv than nothing for sure and the timeline at our current clip our current pacing is. I don't know many years before we managed to hear the eip

**Mario Havel** [57:13](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3433s): That's great,  yeah I mean I am a bit busy these days. I will probably be able to look into it in the coming weeks and I will reach out to you. I see that you are one of the contributors there and I also actually have in touch with him regularly. So if I have anything I will ask.

**Micah Zoltu** [57:35](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3244s): Yeah I think for eipv you probably want to talk to Matt light client. He's I think he's the one who ordered it originally from ruby, I am not mistaken and so he probably knows it the best. I actually don't speak rust so I would not.

**Mario Havel** [57:53](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3473s): Okay you should be good uh yeah i talked to light clint and amsterdam recently. So yeah I can I will get in touch yeah.
**Pooja Ranjan** [58:07](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3487s): I think that would be a good help in that direction because as Micah mentioned that we were considering that to be converted into typescript probably but now that we are getting some help on rest side, so let's have it what we get there. I know there are a lot of open issues
so it's good that you have already started looking into it and we have someone else Jose on the call who is currently looking into eip bot stuff but I know Jose you have been suggesting a lot of suggestions how to improve that. Yeah if you have anything to add? I know we are out of time but anything quickly if you would like to share 

**Jose** [58:44](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3524s): Yes thank you very quickly issue 78 and issue 80 was created to answer issue 75 and issue 70.I will move them to the pull request as as suggested and I will generally also pull requests for issue 77 and issue 79 which are high priority.

**Pooja Ranjan** [59:15](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3555s): Sounds good. Yeah if you can add pull requests that would give more clarity to eip editors. They too may be able to review it and decide whether that is a good suggestion or that would be a good solution to the issue that is  looking for some help so that would be great. I
I know Sam Wilson has done a great job putting out small issues for bot that can help automate some of the processes. So slowly we would like to also get into taking up those issues. But to begin with we can start from whichever or the higher priority. We are out of time. I am not sure if you'll be able to take any other item listed here. Just quickly I wanted to  mention this to Mario. Mario i'm not sure if you are available on ethereum cat herders discord. If you have not, maybe you would like to join and we will try to have a discussion. You can also discuss it on ethereum rnd eip editing channel but there are also editors available on ethereum cat herders eip editors channel and we can discuss if there is something that I mean that is there for you to answer the editors.

**Mario Havel** [1:00:27](https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3627s):
Yeah I am in discord and I am following here. I  also read that  the editor apprenticeship had a book and I might be able to to help with some editing as well or some feedback for the piece .

**Pooja Ranjan** [1:00:49]https://www.youtube.com/watch?v=aqJCBdfgx2c&t=3649s): Great thank you so much. Thank you Tim for introducing Mario to the group. I hope this will help us a lot because we have been looking for a lot of help to  towards sport so we'll be able to
 move smoothly. Anything anyone would like to bring up today? All right um I will consider that we are good for today but I know we have a few more things that we would like to cover in the upcoming meeting so, thank you everyone for joining us today. Hope to see you in the next two weeks and we can still keep chatting on the discord ethernet and ethereum cat herders. 

---------------------------------------
# Attendees

* Micah Zoltu
* Mario Havel
* Pooja Ranjan
* Sam Wilson
* Daniel Tedesco
* Fireflies
* Jose

## Date for Next Meeting: 18 May 2022 at 1500 UTC.







