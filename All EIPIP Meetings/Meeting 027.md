
# EIPIP Meeting 27 Notes
### Meeting Date/Time: Wednesday, February 24, 2021, at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/54)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=nyW-5Y3elOs&feature=youtu.be)
### Moderator: Hudson Jameson
### Notes: Avishek Kumar

----

## ACTION ITEMS

**ACTION 27.1**: Pooja will ask Alita More to get in touch with Micah in regards to progress on EIP GitHub repo action bot
 
**ACTION 27.2**: Hudson will connect with Jame about the oasis JSON RPC stuff

## AGENDA

## 1. Progress on EIP GitHub repo action bot

**Hudson Jameson**: Okay so, hello everyone and welcome to EIPIP meeting number 27.The first item on the agenda is the EIP Github repo action bot. Pooja you said you have a small
update because I don't think Alita is here.

**Pooja Ranjan**: Yeah considering the issue with the present EIP  bot the eipip group
discussed to address this by possibly  having another bot and Ethereum Cat Herders are funding the effort and Alita Moore from the team is working on it. I guess she made some progress as far as I know she had some questions related to testing but unfortunately I don't see her on the call today. So maybe I would ask her to get in touch with  Micah if that is fine
and yes we can get it done like offline.

**Hudson Jameson**: okay sounds good,

## 2. Progress on the content for [Eth1.0 spec repo.](https://github.com/ethereum/eth1.0-specs) with useful information.

**Hudson Jameson**:  All right uh the next item is progress on the content for the
Eth 1.0 spec repo including JSON RPC and Network Upgrade pages.

**Pooja Ranjan**: We are trying to add some useful resources to ethereum 1.0 spec repo. I believe James is  taking care of that. Maybe adding the previous network upgrades and some effects. I have just one small update on the JSON RPC side that ECH is organizing a PEEPanEIP meeting for eip 1474 remote procedure call specification on march 17th with Eric Marks and Mauris W. where we are trying to provide the overview of the proposal and how the implementation is done. Because many people have questions on that particular proposal.
Helping out with this JSOM RPC spec, if people are interested please feel free to join us
on march 17th.

**Hudson Jameson**: All right great 

## 3. Relationship between eth1 and eth2 specs

**Hudson Jameson**:  Item number three is the relationship between ETH 1 and ETH 2 specs.
I  think that's something that Danny put on the agenda and wanted to talk about today with the merge coming up things like that. So Danny if you want to kind of talk about what you had in mind for the discussion today and we can chime in.

**Danny**: So as you know largely we have done specification writing in an independent
repo called the Eth2.0 spec repo. and moving forward, we are beginning to write specs that have a tighter relationship to existing specifications things that we normally call Eth1
specifications and just for some context the way that we are currently writing specifications
and currently protecting things is essentially take Eth1subtract out proof of work,  add Eth2 as consensus layer and you have specifications.Obviously we did 2982 at the end of last year which was met with some contention from eip editors as
to whether that actually made sense to tie like the Eth2.0 specs repo into the eips that way in an
informational spec. I just want to pick your brains get some advice get some thoughts on how
best to do this because the specifications moving forward look like modifications to the consensus layer proof of statements layer specifications in the ETH 2 repo and linking somehow into the application layer specifications which is largely like what we call ETH 1 largely exists in eips.I know there is also the yellow paper. I know there is also ETH 1 of specs repo on releases. There are a lot of moving parts and it's not clear how to. It is clear in my mind how to link them together technically but not necessarily practically from like a specification and maintenance
standpoint. So I just wanted to see if you all had any ideas. I don't suspect we would necessarily decide today but I just wanted to put it out there.

**Hudson Jameson**:  So I guess my first thought is, what is the way that we can do this that best signifies that this is a single ethereum because I think that's really important to make sure that we do not frame this well.It is already kind of a I think misnomer might be the right word that
ETH 2 is like totally separate from Eth1 or like is a whole new thing and Eth1's deprecated more so than this merge that we are kind of developing a new narrative for. So,I think that is an important aspect. I also think that it might be hard to answer how it should come together until we figure out how best to organize eth1 stuff and get that complete. Because from last I heard and someone might be able to answer me the yellow paper is not updated. The eips repo is still looking for more editors and the ethos spec repo still doesn't have all of the things it wanted. It includes previous network upgrade information and some other stuff like the JSON RPC spec.

**Danny**: Help me understand the ETH1 spec repo is primarily what it does. It takes like a bunding of eips and says like this is essentially a release and specifies them as such.

**Hudson Jameson**: That is part of it. Yes so it used to be when you go to the eip repo. You would be different. You would have meta eips for like homestead and all those other ones and that would really conflict a standards process with a release process including stuff like having final and eips mean it is enough work when you are talking about quarry eips. So we have changed up some of the terminology and also tried to separate out the standards from the non-standard stuff including network upgrades to make it a little bit easier. I think Micah was a big driver of that. So he might be able to give him a little more color as to why  that happened.

**Danny**: Great, interesting so in my mind and maybe not in the mind of everyone but what we call each one is more like in this and in a merged world each one minus proof of work is like the
application layer and ease two is the kind of consensus layer. The cradle for the application layer and maybe the linkage is actually between these two spec repos in that when there is a
merge there is kind of things are released in tandem where the application layer is at this point and the consensus layers at this point.They are tied together through essentially on the
consensus layer. There is like a function call under the application layer but it might be very clean. There might be more than one tie and it might be dirty and we might just kind of
see how it lands. So that is one possibility and to so tie them through these two repos instead of
through the eips like I tried at the end of last year. But I am definitely open to thoughts and
ideas here.

**Micah Zoltu**: So my initial thought with the process that would result in the least change to the process would be that anything that needs to happen for the merge that would go into an ETH 1 client would go through eip process so any changes that each one clients need to make
prior to the merge and then once the  merge happens at that point any changes to either ETH1
clients or ETH 2 clients would go through the eip process. So basically the ETH 2 clients would join the eip process as of until the merge. 

**Danny**: Yeah, right I see that so in that sense the ETH 2 specs become something like the yellow paper as in like the foundation before it started and it can still be maintained in random
but its relative stuff needs should probably go through the eip process.

**Btrent Allsop**: Does these two have an improvement proposal process?

**Danny**: No it's quick and dirty. Kind of by design things move very quickly and rapidly and we do have kind of rough consensus in the specs repo and what gets built by clients and released
but the plan is certainly to refine that into a point in which it unifies with ETH 1 development process at the merge so it does not have a formal process. Right now and that's also one of the reasons I am chatting here is that it certainly should have an affordable process at some point in his life time and that is certainly at or before the merge.

**Micah Zoltu**: Just to be clear I am not missing it. 
**Hudson Jameson**: I think Micah might have a delay going ahead Pooja.

**Pooja Ranjan**: Okay so from where I was  looking at this ETH1 and ETH 2 merge process. I consider this to be in  three phases. If we divided that would be helpful for both of us from the ETH 1 client perspective and maybe from ETH 2 client perspective. Something is pre-merge stage hypothetically like if this merge has to happen like in like next 15 months by the summer of 2022.  So we have this pre-merge phase so we have to work on the proposals that is needed
for ETH 2 much later on preparing for the merge would be like the next stage and post merge. So from my understanding at least one of the ETH1 upgrade we are seeing that is definitely before the merge okay  and if we consider that to happen before August we might want to focus on the proposal sites like which proposal would be if at all that would be needed for the eat to merge and then for while preparing for the ETH2 whatever proposal we could not consider. They and we find that these are useful and that would be needed or maybe helping out in like
whatever the shifting of the brain from ETH 1 to ETH 2 would be required we can look into that. The third part of the post merge is something from my perspective that is more important for researchers to figure out what is needed in ETH 1 client at the end of the day and this will drive the first and the second phases. So what I was trying to mention here is like if we would like to consider this much process and  not the process of the overall ethereum chain running but what we are expecting from the ethereum 1.0 client. Maybe we have to figure out what ETH 2 needs from us as that was mentioned in the last encoder .

**Danny**: Yeah and so, there's two parallel things happening here. There is the practical standpoint of like communication and coordination between these two pieces of software and then there is also how do we write it down and where do we write it down. There is interplay there. Certainly Tim and I and others are going to work on the the practical component of like
what actually we plan on producing a  document the next week or so that says like these are all the things that actually need to happen at least from the best of our understanding. Right now we have a relatively clear path on how to begin to integrate those onto the consensus layer side on the on ETH 2 side in terms of specifications and then we need to think about how to integrate
them on the other side and I think  you know a number of these things can show up as eips but contextually the eips needs. So like for example the change of the difficulty opcode that is you know essentially like bricked in a proof-of-state context and you need to decide that what it returns in that context because there is legacy contracts that use it but if we just write an eip that says brick the difficulty opcode. It needs the context of proof of stake otherwise it looks like a pretty silly eip and so at  that point I mean we can point back to ETH 2.0 specs repo but which works but there's also. I do not know we need to figure out that process and MIcah are you back.

**Micah Zoltu**: Yeah I am back so just to be clear  what I  proposed before I got disconnected was not necessarily my preference.Just that was the process that was closest to what we have today. Regarding your question on linking to ETH  2 specs repo so I have a pretty strong policy as anyone who watches the eips repo would know against linking outside of ETH 2 repo and the reason for that is because for any sort of long-lived document repository links will all eventually
404. any lengths that are outside of your page is going to 404 and with a single editor. I cannot keep up with the thousand things of 404 every day that being said I also recognize that it is unreasonable to say okay. You need to define all of these two specs in the eip's repository like that's insane and so I don't have a great solution. I think we might just have to accept that we are going to have broken links at some point and that we make an exception in this one case. I wish there was a better answer right?

**Danny**: Yeah I mean in terms of  maintenance and if we presume that the merge happens and the eco specs become canonical consensus for state consensus specs and are used in mainnet ethereum. There is less of a chance I mean there is definitely a chance that links break
but if we're pointing to like specific releases on that repo. You know those that are maintaining
the two spectrum those that are maintaining relative eips become certainly have more of an overlap and so there's probably less chance that it becomes like kind of an external repo that just or an external link that just dies but I agree with you that there's a fundamentally kind of an issue there and makes it relevant yeah. So I mean one other and this one other potential way to do this. No, I didn't think about it. Does the eip refill linked to the yellow paper.

**Micah Zoltu**: No for basically the same reason I mean the type of the class of problems
that I am worried about with ETH 2 specs repo is less. What if ETH 2 specs when we don't go to these two. It is more like what happens when Github starts centering people and everybody moves to Gitlab and now ETH 2 specs is not Github.com. ETH 2 specs and then six months later they joined the bandwagon. We moved to some random dark web onion yeah so again in this one case maybe this is a special case it's worth. It is  going forward like long term and this gets back to saying that I don't necessarily think the eips process is the best process for use to. It might be better and would address this if instead of having an eip process that then adjusts a spec that lives somewhere else like right now the eip process kind of technically adjusts the yellow paper. Since you guys already have all your stuff in Github it might make more sense
to have your change control process b pull requests against that. So that way it's all in one place and right and I was thinking about that.

**Danny**: Maybe crosslinks yeah maybe the eip core specs or corey ips end up being
application layer query eips and the consensus ends up being like a slightly different
process or at least lives in a slightly different place. Tell me this and I believe I know the
answer but the sum total of core eips on or at least like deployed core eips is not the entire ethereum protocol right? It assumes the yellow paper and then its modifications on top.

**Micah Zoltu**: Okay, optimistically yes I think it assumes yellow paper. Yeah and some other stuff mixed in that wasn't documented.

**Danny**: Yeah I understand if there was a more maintained yellow paper and somebody doing that would  change the way the relationship is like the eip core and the ethernet vector repo and stuff or is that do you consider just kind of independent at this point?

**Micah Zoltu**: I would like that like I would love it if instead of the yellow paper we had a specs repo like you guys have for ETH 2 and we had it for ETH 1 and actually documented the current protocol fully and then from there we could then do PRs against that as either as part of the eip process or just replace the eip process with direct PR’s to the spec. The reason I haven't pushed on that or even proposed really is because that's a pretty big change and it is hard enough getting you know one op code removed nonetheless changing the entire process.

**Danny**: So I recommend you speak with Paul. I can't remember his last
name. Paul has a lot of familiarity with the wasm spec which has a written spec and a
accompanying code spec that like kind of line by line is very literally an implementation of the
written spec and he is talking about doing that for the yellow paper and updating yellow paper
and such a executable spec along with a written spec might change the way the possibilities
are doing here. Obviously there are a lot of unknowns there one will be done two who's maintaining it. You know all of that  but it might be worthwhile for one of you all to reach out to Paul to get a handle on what he is attempting to do and whether that's relevant to the eip stuff. So, let's do this so we can talk about this as much as you all want to but I will say I won't drop an eip like we did at the end of last year without chatting with you all  and as the specs are written on ETH 2.0  side. We are trying to formalize how to do the same on ETH 1.0 side. I will keep the conversation open so we can end up in a reasonable place with as few brittle links as possible.

**Hudson Jameson**: Yeah if I had my way today and we had to make a decision. I would go
with what I think what Micah called the easy path or the path that like we're kind of set up for
today which is the merge ETH 2 repo. Does the spec all the way up to the merge and then they start filing the eips after that sounds like what we're set up for today.

**Danny**: Yeah I would say barring some other decision or like reasonable path that
emerges or maybe reformulation of eip stuff then I think that by default  would make sense. The one well the one problem is there's like there's two major things we want to do with the Beacon chain one is merge the ethereum application layer into it and the other is charting iterative work on the consensus layer after the merge that didn't include sharding would probably be pretty simply to be able to be done in eips but post that but in addition to that there's the the sharding work which would be a little bit more major scaffolding work and might be more difficult to do in the context of an eip but we can  address that when we get there,

**Micah Zoltu**: I suppose. We can just call it ETH 3 and I think what we want to. I  think a good goal for when we are figuring this out though is to make sure that ETH 2 stuff feels comfortable rolling into eips. Trying to figure out the best way to say this like right we don't want this to be
a hindrance. I guess like let's say oh yes a little.

**Danny**: Yeah, as I said it the doing an eip kind of specifying qualitatively and quantitatively to a certain extent.  What a modification that would be done to ETH 2 spectrum quote is reasonable but at the same time we're going to do an accompanying PR  in ETH 3 expect repo
becauses there's an executable specification that builds tests and so there are even if we move in to do iterative work in the eip stuff. It will always be accompanied  at least for the foreseeable future with executable spec modifications which so then we are maintaining things in two places
which isn't crazy.  I mean that's the idea of the elevator is that you are maintaining things in two places. Micah I am  sorry I think you are like lagging but what would you say.

**Micah Zoltu**: Oh! sorry I was just saying I am not a fan of maintaining information in two places.

**Brent Allsop**: Yeah my understanding of the yellow paper is that it's a user-readable version of what's in the eips combined with ETH 2 spec or I mean the ETH 1 spec in the eips and then if you combine that together that's the canonical definition of ether and all the yellow paper is a user-readable stuff and in my understanding it's a type of wiki system where people can contribute but it never is up to date and some of the new stuff right gets accepted in eips and so it should be recognized as not canonical but up to date as much as possible right.

**Danny**: So I mean in that sense it might go to that end . If we do want to maintain this thing. The executable you spec in a different place to be able to build tests then that would point to potentially not doing the iterative eip thing and having a different change process more closely to those.

**Micah Zoltu**: Yeah then that would lead to that other thing. I suggested where we have eips
would be for changes to the ETH 1 clients even after the merge. So like the application layer as you called it and then you guys would have a separate process likely a pull request process for changes to the consensus of course then we there's still that interconnect and i think we just might have to live with crosslinks forever unless at some point. In the future we can have just an ethereum specs repo that has executable code for application and consensus layer which would be awesome. But I don't know how realistic that is and so we should probably have a plan for that doesn't happen.

**Hudson Jameson**: This would also be a good opportunity for those who want to do this I am
not in that camp but I know people have been yelling about this for a while to separate the eip's repo between ercs and eips so there would be a new repo. I don't know were you a proponent
of that Micah I forgot.

**Micah Zoltu**: I think I am the only proponent. I believe I am just loud enough about it. It
sounds like 10 people.

**Hudson Jameson**:  okay that might be it but I think that this would be the only opportunity. If we were to do this after merge to separate the eips repo between ercs and eips
and then that new fresh start would enable us to do all ETH 2 and 1 related core consensus application protocol work and one repo and then erc's in the other.

**Mica Zholtu**: Yeah I would love that very much because I could just quit reading ercs and they would stop hating my life. 

**Danny**: You don't want to read the new upgradeable smart contract protocol.

**Mica Zholtu**: Oh my god I do not want to read the latest upgradeable smart contract protocol
or the 10th latest or whatever. We are up to the one problem you might run into is that I suspect if we do this what will happen is no one will be an editor for the air sees repo like the only reason I am an editor for. It is because it's currently bundled in and I feel obliged to respond to them as soon as you split it off. I literally will just stop reviewing the rsds entirely because I hate them and I will only review core eips and then I suspect no one will take up this dead. I am okay with this but just be aware of what will likely happen.

**Hudson Jameson**: Yeah that makes sense. Okay so it sounds like where we are at is if
default happens and we don't have more of these meetings as things get closer. It would
be spec repo or the specification repo for eth2 continues on and then they start doing eips after the merge and then we figure out something for sharding later. 

**MicahZoltu**: Yeah, I would say the default should be that application layer does eips and
this layer does  whatever their process is probably pull requests and then if  someone comes
up with a reason not to do that then we have a backup plan or at the merge have these two specs go to eyepiece, I guess the secondary.

**Danny**: The release of a merge fork or merge release would be a 1.0 release tied to a 2.0 release and showing the connection between the two essentially like the modifications to the application layer and the modifications to the consensus layer.

**Hudson Jameson**: Yeah and you know looking at it like I am thinking about what changes we have to the consensus layer currently in ETH 1 world and there's not many is going to be that many in ETH 2.

**Danny**: Yeah difficulty bombs yeah I mean if somebody wants to propose a difficulty bomb then that would like validator rewards would like drop to zero or something like that  those validations the idea is to have very few right like I think that there's a lot more moving pieces
in the proof-of-stake mechanism than the work mechanism and so I would expect certainly over the next 12 months some refinement. There's some refinement expected to go out this summer. So I can't say for sure but that would be great if it was largely stable and then we can get back to application layer modifications.

**Hudson Jameson**:  yeah yeah i don't know. Okay and I hope more people as things get closer to the merge will get more involved in a meeting like this. Yeah because I think we just need more think people thinking on this for different ideas and yeah it's unfortunate there wasn't as many people on today, but  let's definitely bring this up again at a future eipip meeting and hopefully by then we'll have a few other things solved like more editors onboarded.Things will be cleaned up a bit more so that I mean hope I am hopeful but there's no indication that's happening but I am still hopeful that we'll have more editors and things like that so we can have things cleaned up a little more and like have a better clear distinction and what the ETH1 point of spec repo becomes.

**Danny**:  Okay, we are moving forward on some 2.0 merge specs that begin to kind of dictate some of the changes in the ETH1 layer and we'll kind of just have them written down and We will figure out over the next handful of months where to formally write them down.

**Hudson Jameson**: Yeah another default is going to be the linking between the ETH1 eips like the difficulty opcode stuff and linking that to reasoning at an ETH 2 repo that's like I think that is what has to happen. I can not think of an alternative unless we start including more documentation in the eip repo itself.

**Micah Zoltu**: Yeah I am not a fan of that either I would say for Danny just as much as possible. Limit the cross links like try to where it's reasonable try to include the information necessary in the ip itself like don't just be like this hash code now like try as much as possible to actually specify as much as you can and then maybe have like one link for additional information to the reader.

**Danny**: That I can provide the context verbally like the in the context of an merge a movement to prove mistake like this is a modification of the difficulty op code to be this instead of the previous proof-of-work context and I can say that all verbally I don't have to even point to an external link but it is at least contextualized by something that is not in the eip repo.

**Micah Zoltu**: Yeah I am willing to let it slide in this case because this is special. The reason I  have this personal rule is because I get ercs that have just like links to people's personal Github
accounts and they are like go here for all the details of this spec.

**Danny**: Yeah okay

**Hudson Jameson**: Yep that sounds good

**Danny**: That all seems reasonable and I will attempt to be very reasonable as we move
forward and I will keep the dialogue open.

**Hudson Jameson**: Yeah Micah I like how you say this is an exception like this isn't a huge deal like being two's like what's the question. 

**Micah Zoltu**: I guess I will let you because I like you. 

**Hudson Jameson**: It is one time this is one time.

**Danny**: Yeah I would not let anyone know that you compromised here. 
**Micah Zoltu**:  I am sure it is gonna end up all over the internet. I am sure on twitter it will be like oh Micah is being unfair unfairly he's friends.

**Danny**: Micah lets people do external links now and it's going to be a free-for-all.

**Micah Zoltu**: Oh my god i'm already in my life.

**Hudson Jameson**: Yeah get your hexagon upgrade contracts ready for your external links anyways.

**Brent Allsop**: Yeah I just have a personal opinion on fear of external con links and 401 errors to me everything should be done in a weekly leaderless way like for example right now. We have got eip.ethereum.org and ethereum.org slash eips and we are proposing moving the ethereum.org eips over to eips.ethereum.org and that's going to break a few links and so I  would like to take on the responsibility to track down those links and get them fixed ourselves because Micah mentioned the bottleneck process.He can't keep up with all the links and keep them all fixed but if you put it on the leaderless bottom-up way so when someone moves a page
they should be able to go out and find all the links and make the changes from that end. So that
we're not bottlenecked by anything and everything can be done by anyone but anyway just a
thought.

**Danny**: Yeah I mean I am  like it in theory impressions when I detail distribution on who fixes links.

**Micah Zoltu**: Yeah  it gives me one idea though in theory eip specs repo. Yet ETH 2 specs repo is currently a Github repository right. Likes with markdown files in Github hypothetically. We could include it as a sub module and the eips repo and that way we can link internally.

**Danny**: Right,  an eip that modified the consensus layer could also modify. Would actually modify like actually do the code modification as well is implemented.

**Micah Zoltu**: Right yeah and that's like what part of why I am a little meh on it i mean some modules in general are a bit hellish to maintain and deal with well.

**Hudson Jameson**: It's not impossible because they we have that for each 1.0 with the jello
paper.  if or was it the beige know that the jello paper or the beige paper.

**Danny**: Yeah the gel paper is like jello  paper is a k specification of I think primarily the
evm it doesn't have all the cradle components like the stuff but I don't know  if that's actually very maintainable gel paper. Owners claim that it's very maintainable but it's very dense to read in my opinion.

**Micah Zoltu**: All of my code is very maintainable no one else is this.

**Danny**: Yeah I would say encourage one of you to hit up paul D  to hear about what he's working on on like an executable spec accompanying with some yellow paper updates which if we had an executable that kind of both layers then we can start to do some pretty interesting
things maybe and putting that in like the 1 0 spectrum though and there can be some interplay between the two there.

**Husson**: Yeah we just throw money at someone to maintain the yellow paper I think just get it up to speed before the merge.

**Danny**: Yeah you gotta find the right someone.

**Hudson Jameson**: Okay I think we are good with this topic unless anyone has any final stuff
okay well thanks so much thanks for.

**Danny**: Having me I appreciate it.

**Hudson Jameson**: Yeah we will have another one of these eventually bye. Unless you want to stay whatever you want to do i'm out later all right see you

## 4. EIP editors onboarding requests & funding

**Hudson Jameson**: Next up we have eip editors onboarding and requests for funding. I don't have an update for that so we can go to the next thing. Oh actually no we do have an update
for that we have a blog don't we?

**Pooja Ranjan**: Right  so after the release of the blog I became an editor. We have been approached by a few people from the community that are interested in being edited and they have questions on the process part and if this position is compensated etc. I wanted to bring this to the meeting to get clarity on the onboarding process. As how we can screen the application may be whom could we send candidates to or like how do we want to proceed with this
particular onboarding process for eip editors.

**Hudson Jameson**: I think me and Micah and the light client can just talk to them.

**Pooja Ranjan**: Okay  so  like what would be the best place where we can send like any group or I don't know how.

**Hudson Jameson**: How many people are there that came to you?

**Pooja Ranjan**: At least three but those are like coming directly from community what we are doing at the first training part asking them to fill up their onboarding form for ethereum categories so that we can get to know about them a little bit more if they have any association with ethereum or not and some from references etc.
**Hudson Jameson**: Micah where's your preferred place to be discussing with these people like either the eips chat, discord the cat herders chat and discord or a telegram group.What do you like anything in discord is good for me.

**Hudson Jameson**:  okay  Pooja do you have a place that you think would be best maybe the cat herders discord.

**Pooja Ranjan**: Yeah mostly people are showing up in Cat Herder’s discord because that is mentioned in the blog that reach out to cat herders so possibly I would create a separate channel providing access to Mica, light client and you and we will send the candidates over budget.

**Hudson Jameson**: If you make that channel, remind me to turn on notifications for it because I am really bad at that. So in fact I am going to change my notification settings for the cat headers channel after this call because I think they got muted automatically when I joined and I don't want that to happen.

**Pooja Ranjan**: Okay yeah I mean definitely so there is already a channel of eip where Alita is throwing some you know stuff for the boss one but I am gonna do it if we want to have a separate  channel for the api data. So we can continue the discussion over there because everything is going for the eip depot only there.

**Hudson Jameson**: I am okay with having the same channel.

**Pooja Ranjan**: Okay then I will reach out to light client and Micah and get them added over here.

**Micah Zoltu**: So  one question I have maybe someone else can ask of all the applicants is
why in the hell would you want to work for free on eip fees.Anyone who wants that at eips I am
very suspicious of which I know I shouldn't be since I should that would make me suspicious of
me but I am very suspicious of me too. I don't know why you guys trust me.

**Hudson Jameson**: They probably are asking about compensation which isn't happening yet
but if they are still like I am willing to wait for that  or like I will come back when we have compensation that would be fine too.  We can still vet them beforehand or get to know them that's not a negative thing.

**Micah Zoltu**: Yeah sure, if that was if that was someone's answer like why do you want to do this and I said well I need a job I would be totally fine with it. I just worry about anybody who's like oh yeah I would love to do eip editing. Yeah no one says that yeah no no it's just.

**Pooja Ranjan**: Yeah we received these queries like if this job is compensated I already have
informed people that at the moment it is not but we are considering some options to get provide funding to this particular road and yeah obviously if they would want to consider it now or maybe come back later it's fine.

**MIcah Zoltu**: Okay yeah I definitely trust someone who likes money more than I trust someone who doesn't.

**Hudson Jameson**: Nice okay that's good for is that all you need for that item Pooja.

**Pooja Ranjan**: Yeah.

## 5. Single source of truth for EIP

**Hudson Jameson**: next up single source of truth for eip I forgot what this item was
For.

**Brent Allsop**: Yeah I am working on that,

 **Hudson Jameson: Oh that's the one you mentioned earlier. okay so now
no real big updates there.

**Brent Allsop**: Yeah I integrate last meeting we talked Micah had the idea of removing meta information in the eip repository like eip1 out of the repository and so it included that idea in the proposal that I am doing and the next step I think is to create. so what and we want to move that into eips.ethereum.org and so I think the next step is we need to set up some kind of staging area where we can build a new version of ethereum or eips.ethereum.org and I asked Pooja before the meeting who's responsible for that and sounds like axis is and so I am going to reach out to find out if there already is a stationary grade if not i'll look towards seeing what is required to set one up that and push in that direction but that's just just an update of where I am going. What I am going to do next 

**Hudson Jameson**: Now when you say move out eip1 do you  mean move it out of the repo into a website.

**Brent Allsop**: Well right now we when we made the changes to the eipip process
all of the new updates got made to eip1 and right now that's the canonical set of staging of where the canonical information is and last meeting Micah proposed moving that out of there and moving that someplace on to eip.ethereum.org and so that  and so I added that proposal and I think that's a great idea specifically. Since it  needs to take some of the workload off of eip
editors and stuff like that and so I have assumed that's okay it sounds like you might have a problem with that is the case.

**Hudson Jameson**: I more just want to understand it before I have a problem with it or not um
because like if it's so it wouldn't be a  meta eip anymore it would just be a rule set then.
**Brent Allsop**: Yeah and keep up with and we would define the canonical med eip information somewhere on eip.ethereum.org and that's why I want to set up a staging area where we can move all that and get all that set up and get it because right now it is the eip1 that is the  canonical stuff but we want to get a stationary set up and get everyone on board and say yes
that's sufficient we can switch over from eip1 being the canonical source to this new source when we make it live but  anyway Micah do you have anything you want to tell him about why we would want to do that.

**Micah Zoltu**: I am just trying to keep eip. The efp's repo focused on eip standards
and right now. The eip1 talks about stuff that's not directly related to standardization like why I pulled up real quick so I can remind myself for example right at the top what is an eip rationale
talks about the eip workflow which belongs in a successful eip like this all feels like the workflow probably is fine to stay but  what belongs successfully I  feels more like a tutorial or like a blog post or something that's kind of this isn't a spec. This is just like some helpful information for newcomers and I currently think that type of information is spread out in multiple places and I feel like rather than putting everything more stuff into eip1 instead. We can take some stuff out of the ip1 and have efp1 focus purely on this is, The process like these are the requirements like
it's basically a standard for eips like eip1 becomes an eip in it. I  guess what i'm trying to say is eip1 is a technical standard right now. It is a technical standard with a whole lot of non-standard information like non-normative information in it and I would like to pull out some of that non-normative information and put it somewhere else.

**Hudson Jameson**:  As long as someone is putting something somewhere else I am okay with that so like if we have through a blog or two prepared or an article or what Brent's coming up as long as that's been prepared for when that happens then I think I am okay with it.

**Micah Zoltu**: Yeah the idea is we would take the information that's currently there and then move it over to ethereum.org and then delete it from eip1 after it's moved. so not not that we  delete it first and then maybe later we'll add it somewhere else it's definitely a migration. So  We are moving to a new location.

**Hudson Jameson**: Yeah I am not. I don't have a strong opinion on this like I would probably if I had to choose I would probably keep it the way it was for simplicity but like at the same time I see your points and that sounds good to me. We can also start the thing where it's less opinionated on how to do stuff and more just like you said a technical specification on the process itself.

**Micah Zoltu**: Yeah that's  what I would like looking through it. As an example there's a history section in the eip1 that talks about bitcoin's bip process and that really an ibm doesn't belong in
it like a technical spec for how to build an eip it's like history and it's interesting and it's
useful. Just I feel like the ethereum.org which already has a whole bunch more of that type of information is a better place for it. History and you know stuff like that.

**Hudson Jameson**: Cool okay okay.
**Brent Allsop**: So do you think like the map of states that says what states eips go through. Does that go in there?

**Micah Zoltu**: I think  that's technical  like basically anything that I as an editor would refer to and say hey you're not following the standard point back to eip1 so like if someone tries to go from draft to final. I would point to eip1 and say that's not allowed here. So if it's whereas I am never going to point someone and say hey look at the history and of the bitcoin process like as a reason to reject their eip so if something is like a specification or a standard or like a requirement for the process then I would say eip1 and if it's more just metadata about the
process or description of why we have this or you know where this is the history of it
stuff like that  would be moved over to ethereum.org.

**Brent Allsop**: I was a little bit unclear on that but I understand that makes a lot more sense.
now okay i'll update the information and keep on moving forward.

**Micah Zoltu**: With that I mean there's the other option and I am not against this not for it. Just to throw it out there which is to just get rid of vip one and just put everything somewhere else.

**Brent Allsop**: Yeah that's kind of the way  I am a huge fan of that initially starting but if we don't want to go that far yet then I would like to know.

**Micah Zoltu**: I am okay with that just I mean it does mean there's just one less place that people have to know to look for things like it consolidates information. So I am not against just one the whole thing out I don't know how other people feel.

**Brent Allsop**: Right but I think we should have a very clear location whether it's eip1 where these are the states eip go through and this is the process you do to migrate from one step to the other. It doesn't need to be any eip1 but if that's where we want but we should if and I was proposing moving that exactly thing so that every time you want so Micah to say you're not following this he would point to wherever that location is and I thought we were removing that
the eip.etherium.org but  maybe.

**Hudson Jameson**: It's entirely possible. I proposed that last time and I have just forgotten and changed my mind that does sound like something I would  say,

**Brent Allsop**: Okay. So which way have you changed your mind and should I back off a little bit on that.

**Micah Zoltu**: No like the more you talk about it, the more I think that would be nice.

**Brent Allsop**: Yeah I  think I like that idea because the eip repository is where we want to
have the ether spec and we eventually want to have that the canonical ether spec stuff and have some kind of automated process  where that's the canonical ether spec and all that meta information should be moved out of that. So that's Like that idea but anyway. So are we still going with completely moving but but again before we make that move. We have got to have the staging area and we have got to have everything built and say this is where we want the new to be new stuff to be and it has to be sufficient for Micah and Hudson and everyone ether and Pooja and everyone make sure we have. Okay yeah everyone's happy with that now.
we can throw the switch so that's why my proposal is we need to start building a staging area
where we can start building that and moving everything out and moving in that direction.

**Hudson Jameson**: Yeah so you're going to make a proposal
for that as next steps I think.

**Brent Allsop**: Yeah that's  that's my proposal here and I am going to start on that next.

**Micah Zoltu**: what are your feelings Hudson do you think just pulling all of eip1 out into
ethereum.org so we have just a single page that just has history and process and everything.

**Hudson Jameson**: Yeah I don't have a strong opinion because like I see the pros and
and a little bit of the cons cause like the cons mainly the number one con in my head is
like it's now in there is now information in two places or more that people have to go look. So I might need to go read a blog, read ethereum.org and read eip1 to get the technical, non-technical and recommended.

**Micah Zoltu**: Right and that would seem to me to argue that we should just pull all of the eip1 out and put it on ethereum.org along with. So all the information is in one place both the process descriptions and the process history and the process metadata etc. If everybody else is finding that I am totally fine with it.

**Brent Allsop**: Okay we can pull it all out that sounds good to me. Okay I am back in that
direction I will I will push in that direction thanks so much for your help just remind me I
said this next week when I say.

**Hudson Jameson**: It's a bad idea.

**Brent Allsop**: Okay well I was wondering if I just didn't hear you right so
thanks.

**Hudson Jameson**: Hey you probably did. I learned the other day my brain is full. I asked them a question and like five minutes later they gave me an answer and I was like oh that answered has pushed out the question and I no longer remember what I asked because
the ants replaced it that's great. So anyways if we're done with that,

## 6. Review action items from the [previous meeting](https://github.com/ethereum-cat-herders/EIPIP/blob/1b814b8f46303c6216c2a33e3c73d48340baa4fd/All%20EIPIP%20Meetings/Meeting%20026.md)

**Hudson Jameson**: The last item is reviewing previous meeting action items so the first one is complete transfer eip bot to github actions that's still ongoing 26.2 is brent to open a prto the eips repo that's still ongoing we just talked about that editor blog to be reviewed and published that happened and then follow up with oasis for the JSON RPC what was the oasis I know about the oasis JSON RPC stuff but who was doing that was that James.  okay so we'll have to get in touch with him about that otherwise I think that's all the meeting items are there. Anything else. okay cool thanks everybody see you all in two weeks

**Brent Allsop**: yep thank you  

**Pooja Ranjan**: Thank you

---------------------------------------
# Attendees

* Hudson Jameson (Host)
*  Danny
* Micah Zoltu
* Pooja Ranjan
* Brent Allsop

# Date for Next Meeting: 10 March 2020 at 1500 UTC.


