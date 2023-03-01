# EIPIP Meeting 75 Notes
### Meeting Date/Time: Wednesday, February 22, 2023, at 16:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/213)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=UE6MOvSXuJM)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION/DECISION  ITEMS

**ACTION 75.1**:   
—------------------
## AGENDA

## 1. Discuss Open Issues/PRs, and other topics

**Pooja Ranjan** [0:00](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=00s): Thank you everyone for joining EAP IP meeting 75.I have shared an agenda in the chat we are going to discuss open issues and pull requests. We will continue some discussions from the past meeting followed by EIP insight and EIP editing office hour updates but before we get into the agenda item. We are joined by one new EIP editor who has recently joined the team. So I would open the floor for him to provide an introduction if that's okay.

**Gajinder** [0:47](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=47s): Thank you Pooja, so basically I am a CL that I've been involved with Load star primarily and as well as I also work for ethereum.js. So I have a little bit I have a deeper understanding of Cl clients and I'm getting a little bit more understanding of the Year client so I'm sort of able to see a little bit more picture of the entire landscape and hopefully I can contribute.

**Pooja Ranjan** [1:24](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=84s): Awesome we're happy to have you likewise. All right so we can go ahead and start with the discussion and issues listed on the agenda we have collected from the EIP GitHub repository as well as from the Discord channel.

- [Allow including both an email and a GitHub username](https://github.com/ethereum/EIPs/issues/6510) ethereum/EIPs#6510

**Pooja Ranjan** [1:43](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=103s): The points for discussion number one here are allowed including both an email and a GitHub username. I think this was proposed by Panda peep, so Panda if you would like to explain and we can collect editors' feedback on this one.

**Gavin John** [1:57](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=117s):I mean there was someone that tried to do it. It seems like a somewhat reasonable request so I just created an issue for it.

**Pooja Ranjan** [2:07](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=127s): All right in that case if anyone has any objection if not then. 

**Gavin John** [2:12](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=132s): The only issue would be that all the CI that parses the author field would have to be updated but that shouldn't be too hard to update your reg access.

**Sam** [2:26](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=146s): Yeah just a little bit of work is not too bad so if we want to do it we can. So what's the advantage of doing it just makes it easier.

**Gavin John** [2:38](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=158s): Well so that there could be a link to the authentication which is GitHub and also a link for contact which is email.

**Sam** [2:47](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=167s): Right I mean the current recommendation is just to repeat from your example here my name once with email and once with GitHub so I guess the advantage is what you would have a single author entry with both as opposed to two. 

**Gavin John** [2:59](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=179s): Yeah
it shows up in the meta twice. 

**Sam** [3:04](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=184s): Yeah and so the meta tags and Well I guess just the meta tags and RSS could benefit from it being one author item correct okay.

**Gavin John** [3:18](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=198s): yeah I guess I'm in favour of this. We can make that change. 

**Gavin John** [3:25](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=205s): Seems minor enough that we can probably merge it without  my client here. I don't think there's any reason why one would object. We are the two people that would be most impacted by it and we just said yes.

**Sam** [3:40](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=00s): Do you want to do a username then email email the username or both.

**Gavin John** [3:45](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=225s): What is the order the eip1 has it in. Right now

**Pooja Ranjan** [3:50](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=230s): I think We are adding the first email. 
**Sam** [3:56](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=236s): Sure yeah sure that works yeah. We can keep it in the order that's specified here. Okay I'll make the changes to Eip.

**Pooja Ranjan** [4:07](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=247s):
That would be awesome and it is going to also make my life easier because I sometimes have a hard time reaching out to authors with just the GitHub name.

**Sam** [4:17](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=257s): So this would be optional right so yeah so right now yeah okay

**Pooja Ranjan** [4:26](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=264s):
very well and has any different thought or if fine 

- [Replace requires with a bibliography ethereum/EIPs#6509](https://github.com/ethereum/EIPs/issues/6509)	

**Pooja Ranjan** [4:32](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=272s): We can move on with the next item. Okay I think the next item is also proposed by Panda Peep. It is about replacing requirements with a bibliography section. I see there are some comments by Sam Panda or Sam anyone would like to provide an overview.

**Govin John** [4:53](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=293s): Which issue is this again. 

**Pooja Ranjan** [4:59](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=299s): 6509

**Govin John** [5:00](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=300s): Oh yeah that basically in order to get listed on Google Scholar. You need to have a proper bibliography and I think, what we can do pretty easily without much effort. Especially now that we're switching to the new build system or hopefully we'll end up switching to the new build system. we can then have a new entry in the Preamble that basically it's like required in fact. It could literally be a yaml list of Erp names but that also accepts external Banks such as dois etc etc etc and then it would generate a bibliography at the bottom before, right after the or perhaps before the copyright section.

**Sam** [5:55](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=355s): Yes I think generating a bibliography is the correct thing to do. I mean we need to do it anyway because of the CSL Jason stuff. My only complaint here is I don't think we should get rid of the requirement because it's like 90% of references are going to be to other EIPs. 

**Gavin John** [6:17](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=377s):
I'm suggesting we use a Wiki data like thing for eips. Yeah lets you just use a string identifier in fact it could be like literally EIP colon Erp number here

**Sam** [6:31](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=391s): Okay and then for like dois and other stuff it would be like a full Json thing.

**Gavin John** [6:37](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=397s): And then for doing I'm pretty sure for Di's. You can just do the DOI equivalent okay. Yeah and for Wicked data Wiki WD colon Wiki data 

**Sam** [6:47](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=407s): Yes I guess for me if we want to go ahead with this. I'd like to see a couple examples of what a preamble would look like following this format. Yeah just throw them in the issue and we can we can talk about them.

**Pooja Ranjan** [7:02](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=422s): All right, I'm not sure.  I'll think of earlier we were using a bibliography before at least for EIP1. I don't know if anyone has any background on this. Okay never mind, we can go ahead with the present proposal. So I think the suggestion here is to add the specs there in the issue section and it would be discussed further.

**Sam** [7:32](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=452s): Sounds about right.

- [Add draft background image to draft EIPs ethereum/EIPs#6479](https://github.com/ethereum/EIPs/issues/6479)

**Pooja Ranjan** [7:34](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=454s): Thank you. Moving on the third item here that is also proposed by Panda Peep and it is about draft background image to draft EIP the issue number is 6479.

**Gavin John** [7:49](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=469s): I think that we are flying through this. I think the consensus was that yes this is fine.

**Sam** [7:58](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=478s): Yep Yeah I think it's just a draft or last call or whatever and just make a watermark out of it.

**Pooja Ranjan** [8:08](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=488s): All right I thought that it is important to make a mention in this meeting because this is kind of a public awareness as well. Also if people aren't following issues diligently then they would be at least aware of it and if there are any concerns they can definitely go back and add their thoughts in the issue that we are discussing here.

- Discuss policy to add a champion or co-author to an EIP

**Pooja Ranjan** [8:31](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=511s): Okay moving on to the next one is a discussion policy to add a champion or co-authors to an EIP. So this item has been added from ECH Discord. So the latest discussion on adding Champion EIP editors and other users have already shared their thoughts and we do have some text added in eip1, defining the role of champion however it will be a good idea to revisit and possibly make changes if needed. So yeah, if any editor would like to share thoughts and share again like what should be the criteria for adding as a champion or as an author here.

**Gavin John** [9:12](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=552s): I really want the adoptable thing to get merged likes it's the easiest thing ever it's a flag others can say yeah if it exaggerates then anyone can just take it off up where we left it off with and if authors don't want it, they can just say no. We'd rather it just stay segment

**Pooja Ranjan** [9:36](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=576s): I think that was the idea initially that's author resists that they wanted to be stagnant. The alternative is someone can start a new PR with almost a similar proposal and mention that it is you know kind of un stagnanting that particular proposal there.

**Gavin John** [9:54](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=594s): But I was specifically suggesting adding a preamble entry so that the EIP number gets kept.

**Pooja Ranjan** [10:01](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=601s): Oh Well that was the biggest blocker So,l yeah if you want to pull out any EIP from statement status I'm just sharing the information that I am carrying from the past the idea was. It should include author's permission to keep the number if they are willing to understand it then only the same number will be kept on the proposal otherwise if the author decides not to un stagnant that and someone else decides to come up with a new proposal with the entire like a copy pasting the entire content. The EIP number would not be the same, it has to be a new one. 

**Gavin John** [10:42](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=642s): That's what I'm suggesting. The adoptable field would literally be authors saying basically giving their approval in advance of its stagnating like we give our approval to whoever wants to pick 
this up. It's not something that's by default it requires an authority authors to give approval but it's just that the approval is given at the beginning of the process when the authors are reachable rather than at the end of the process where the authors will be clearly unreachable since the proposals of distagnant. 

**Pooja Ranjan** [11:19](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=679s): Yeah that makes a lot of sense so do we want to add any field there or any specific comment on what the proposal is?

**Sam** [11:25](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=685s): So I think that was fairly against this one. So I don't think we can discuss it without him here. 

**Pooja Ranjan** [11:32](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=692s): Okay we can bend it. I wonder if anyone else has any thoughts on it. So definitely We're not gonna make any decision in absence of Matt. So, we can at least collect thoughts if people have any differences.

**Sam** 11:47](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=707s): I don't have a problem with what you were doing. Panda likes adding yourself as an author to Eips that you want to see pushed through like as long as you can.

**Gavin John** [11:56](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=716s): Yeah I think that uses an existing process but which requires author approval. 

**Sam** [12:02](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=722s): Yeah Yeah we're just like Matt was complaining about it and I don't see a problem with it. I think it's fine if you want to do that.

**Gavin John** [12:08](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=728s): Especially considering I'm straight up rewriting all the EIP. Like taking their paragraph basically removing all of it and inserting a new one.

**Pooja Ranjan** [12:27](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=747s): Yes please go ahead. 

**Sam** [12:29](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=749s): Oh yeah I was just saying like yeah I think what you're doing is fine. I think that is the best we can do today without adoptable and I don't think we need to but I don't think we can discuss adoptable without Matt. 

**Pooja Ranjan** [12:46](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=766s): All right. Fair enough I'm gonna bring this up in the next meeting. I hope Matt joins then.

- Moving away from Jekyll. Discuss the options available

**Pooja Ranjan** [12:57](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=777s): Yeah now we can move on to the next item which is kind of information. It's more of an
announcement that probably invites a Viewpoint though. It is really not that of a concern of the community at large because mainly it is related to the Dev worker who is going behind the scene and the one who is doing most of the thing has proposed this. So it is about moving away from Jekyll. As many of us know that the present EIP tooling requires Ruby and at present. We don't have many contributors of Ruby or Ruby experts to support the infrastructure. So Pana PEEPanEIP editors who are mainly maintaining this has a suggestion to move out of this so Panda if you would like to give more background to this and what where we are at the at the moment

**Gavin John** [13:50](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=830s): So I've got a completely working website. We could switch literally right now. So I'm gonna put the link in the chat so this is using the entire workflow. So the GitHub actions think that that will automatically build it and I have sent it to this website right now. Since it's on my Fork of the repo so the things that would need to be happen is first the PR that adds this needs to be merged and then secondly secondly in the settings GitHub Pages needs to be switched to the action based workflow instead of the branch based works though and then the URL needs to be set to eips.etherium.org. But as you can see I have a working website here. I think it looks pretty good so far all the feedback I've received after says it looks pretty good.
It has all the features of the previous website plus this nice little search feature I added. It's in JavaScript script so we can add so and in fact the actual code will be on the eip's repository so changes to the website can be even managed by straight up using the EIP review bot. Additionally actually I think that's it well I mean obviously it's JavaScript and we have at the very least I know JavaScript and I also know Sam knows a little bit of JavaScript.

**Sam** [15:42](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=942s):  I can neither confirm nor deny that.

**Pooja Ranjan** [15:48](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=948s): That is a tank but I am happy to share here again that we are  recently joined  by an editor who 
basically worked in ethereum JavaScript. So I'm hoping that we would have a bit more extended support on the JavaScript side.

**Gajinder** [16:06](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=966s): Yeah guys I can support wherever I can.

**Pooja Ranjan** [16:15](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=975s): So can you please once again like to summarise what is needed here. Do we need consensus on switching from all the editors?

**Gavin John** [16:25](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=985s): 
 yeah I think we just need consensus from all the editors. So this is a radar.

**Pooja Ranjan** [16:31](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=991s): Okay awesome. I was just about to ask if we have a PR so the PR number here is 6518. I don't see Matt on the call, I don't see Victor on the call. So we'll keep it open for some time and let's try to collect more support there.

**Sam** [16:54](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1014s): Yeah no this looks amazing besides not being able to click on the search bar. Oh I was able to click on it that time it's really weird. But yeah I know it's great, like good job on this.

**Gavin John** [17:06](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1026s): Thank you. 

**Pooja Ranjan** [17:10](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1030s): Really nice looking website. Thank you so much all right so now that we have the pull request as well.

- [Agenda request: PR #6483 #215](https://github.com/ethereum-cat-herders/EIPIP/issues/215)

**Pooja Ranjan** [17:20]](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1040s): Let's move on to the next item which is in agenda request. Okay so this is from the issue that was added on eipip GitHub repository and the number here is 215. So the proposal requested this issue to be considered for this call. But I know that it was being blocked by one of the editors yeah and I think he would like to mention Panda why  you think it should be blocked at the present state.

**Gavin John** [17:58](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1078s): Which issue number is this again what is the issue number again

**Sam** [18:23](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1103s): All right it's in chat so 6483 is the pull request and eipip 215 is the wrong repository. Yeah it's the filter again search one that four percent. 

**Gavin John** [18:40](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1120s): The only thing I was blocking was that I would like to have seen that split into two different PR'S. Additionally the website rewrite just does all of that already.

**Sam** [18:58](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1138s): Maybe the correct approach here is to ask full descent to take a look at your rewrite and see if it solves. The same problems and just explicitly ask them to take a look at it that would probably solve any kind of problem. I don't know the frustration with the process. Yeah so I would just pick him and be like hey you know what do you think like we've been working on a rewrite over here would love to get your feedback on it. see if it solves the same problems and we'll just see what happens after that I mean I can even do that if you want.

**Gavin John** [19:36](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1176s):  I would definitely like you to at least review the website.

**Sam** [19:42](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1182s):  Yes I know hey I've taken a look. I've left comments.

**Gavin John** [19:46](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1186s): And I've changed up the files since then and also modified about 550 EIP

**Sam** [19:52](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1192s): Now I will take another look don't worry.

- [EIP authors feedback](https://bit.ly/EIPProcessFeedback)

**Pooja Ranjan** [19:59](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1199s): And to address the kind of frustration that can bring to anyone with the present process or with the dynamic process that we are trying to follow here is we are sharing  this feedback form for EIP authors that is our next agenda item. So far we have received responses from only ERC category authors. so please core interface networking informational or meta authors if you have documented a proposal for ethereum repository consider responding to the survey this is just a feedback form less than five questions I believe. It is just to collect your present thought in the process and also if you have any suggestions that we could probably bring up in future eip meeting for consideration of changes.

**Gavin John** [20:54](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1254s):  I'm not sure that networking eips are a thing anymore. I know they're technically still a thing but

**Pooja Ranjan** [21:02](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1262s):  I can say it for one  for sure that is clwp.

**Gavin John** [21:10](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1270s): okay fair enough but I am not sure who's reviewing that.

**Pooja Ranjan** [21:15](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1275s): Yeah mostly because that is neither a part of the upgrade and also that is not a very popular ERC category but they are still in existence at least for now. But yeah we do have common authors. Authors who are contributing into core EIP are generally authors who are contributing to the networking and interface category of proposals and apart from that we do have a lot of ERC authors. So please take out time less than two minutes it would take and respond to this. Let us know what you think is not right thing for you and you would like that to be changed

## 2. Discussion continued from earlier meetings

**Pooja Ranjan** [21:59](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1319s): Okay  moving on to item number two that is discussion continued from the earlier Meetings.

- Adding CL dev as EIP Editor & new ERC Editor

**Pooja Ranjan** [22:06](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1326s):  The first one here is adding CL devs as EIPP editor and a new ERC editor. We met our new core EIP editor. We are recently joined by another ERC editor who is Victor. People have seen him raving ERC category proposals on EIP repository for over six months. I believe now so yeah he is very much familiar with the process but unfortunately he is not here today. He had some power issues or so but we hope to have him in future meetings. Thank you both of you for joining us and helping out with the EIP process

- Thoughts on Asia Pacific (APAC) friendly call time on an infrequent recurring period such as once every 4 meetings?

**Pooja Ranjan** [22:53](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1373s): The next item listed here is thoughts on Asia Pacific APAC friendly times on infrequent recurring periods. Yeah any thoughts if people may have on this one.

**Sam** [23:09](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1389s):  I'm down. So I probably wouldn't even notice. Yeah I don't think we get 100% participation on this call. Anyways, I think it'd be totally fine to add another one that is at a different time slot. We might get different editors showing up so.

**Pooja Ranjan** [23:30](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1410s):  I mean it is I feel like it is useful or helpful when people know that what time that meeting is going to happen so instead of having it at different time can we try to move it to the Asia Pacific obviously friendly time zone which is not that bad and that could be the time when we have other client meetings will that be a good idea.

**Gavin John** [23:58](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1438s): Obviously it depends on what time it is.

**Pooja Ranjan** [24:01](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1441s): That is 1400 UTC. I'm so sorry. So my question here is does 1400 UTC sounds like a perfect timing? because right yeah the same day just the time at 1400 UTC so you know most of the CL Dev the Elder meeting most of them are at 1400 UTC and we know that we have participants throughout the globe. So they are participating at that time.

**Sam** [24:34](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1474s): Didn't we used to have it at that time and then we moved it.

**Gavin John** [24:37](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1477s): So yes this is so that would be 9 A.M Eastern. 

**Pooja Ranjan** [24:43](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1483s): That is right and that would be 9 A.M for a couple of weeks only. Just a reminder March is right there.

**Gavin John** [24:52](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1492s): I think that would be fine for me and I ended up being a few minutes late but I don't think that will derail things too much. 

**Sam** [25:06](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1500s): I mean I'm okay moving around. we can try it. If it doesn't work for us or we get less less participation we can move it back.

**Gavin John** [25:15](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1515s): And if maybe we can also do the rotation.

**Pooja Ranjan** [25:23](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1523s): Rotation is something that I'm a little carry off but I don't know because you know when we  go out and spread the message that join the meeting. we generally try to give them a sense of time like when we are doing it earlier. It was 1500 UTC since we started, then we moved to 14 then people suggested 1600 and here we are going back again to 1400. which I think is a good idea but when it comes to rotation what is the alternate time suggested here. 

**Gavin John** [25:58](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1558s): 1400 UTC is fine. Awesome because that would also work for. I think that is also fine by the newly joined editor because he is also from Asia Pacific and what about you Greg. Greg is that fine with you too. I just wanted to come up with something.

**Gcolvin** [26:26](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1586s): Yeah no problem.

**Pooja Ranjan** [26:28](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1588s): Awesome thank you. Then I'm gonna add that in the summary of the meeting today so we are trying to switch it to 1400 UTC and I'll make the changes on protocol calendars so people who aren't available in this meeting today may be able to notice it through the calendar.

**Gcolvin** [26;50](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1610s): Wait wait wait  1400 that's 10 a.m Eastern. 

**Pooja Ranjan** [26:55](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1615s): It's going to 9am. Right now it is nine but it's going to be 10 a.m in a week's time or so because we are close to March. 

**Gcolvin** [27:06](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1626s): We are going to have DST gone.

**Pooja Ranjan** [27:11](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1631s): Oh no it is not going to happen . Implementor  call is at 15:00 UTC.

**Gavin John** [27:16](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1636s): So UTC does not care about daylight savings. Okay yeah good. Okay that'll be completely fine I will not actually be late then.

**Gcolvin** [27:33](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1653s): I'm confused.

**Sam** [27:35](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1655s): So right now eipip is after the eof implementers call. We want to move it to an hour before EOS and then they'll both shift the same amount when during daylight savings. 

**Gcolvin** [27:46](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1666s): that's fine perfect 

**Pooja Ranjan** [27:59](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1679s): All right, so I will try to have the next meeting at 1400 UTC I'll try to make announcement as much as possible update the calendar and also update the agenda for the next meeting.

- [Add EIP-6269: Full EVM Equivalence ethereum/EIPs#6269](https://github.com/ethereum/EIPs/pull/6269)

**Pooja Ranjan** [28:09](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1689s): Moving on to the next item here, that is a pull request number that is 6269 for pull EVM equivalence.

**Gavin John** [28:25](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1705s):  So I think the issue here comes down to what building meta versus information will mean because I interpret meta to be literally. Basically definitions like because in my opinion you can't ignore a definition. you have to choose one but at the same time you're not beholden to any specific definition. so it could be informational basically we need to have a fine line between meta and informational.

**Sam** [28:56](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1736s):  So a meta EIP would be something like in this specific instance If This Were a meta EIP it would be an EIP changing the process to not allow people to use this term unless it conforms with the definition. So it's a meta EIP describing the EIP process. Informational is just here is a definition for a term feel free to use it. If you want.

**Gavin John** [29:18](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1758s):  Eip1 never says that meta actually has to deal with the EIP process itself. That's what I'm saying
things you can't ignore.

**Sam** [29:27](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1767s):  yeah in this case it would effectively be a change to the list of things editors have to check. 

**Gavin John** [29:33](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1773s):  Oh then absolutely it should be informational but then at the same time wouldn't that mean that the deprecated self-destruct tip should also be information or not matter.

**Sam** [29:43](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1783s):  yes

**Pooja Ranjan** [29:44](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1784s):  
I agree 

**Gavin John** [29:45](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1785s):  okay then should we change that. 

**Sam** [29:49](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1789s):  No it's final 

**Pooja Ranjan** [29:51](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1040s):  So yeah I mean it's going. It's already in the announcement now.

**Govin John** [29:55](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1795s):  Iregular State cases are things that editors can do.

**Sam** [29:59](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1799s):  Yeah no I'd rather not. I don't think it's a problem that it's meta.

**Pooja Ranjan** [30:03](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1803s):  I think the other Advantage with that being in meta right now could be like you know we are going to see a lot of changes coming up with respect to self-destruct. This is just an announcement. I agree that it looks more informational at this point of time but there are chances that it could serve as a matter of and we should see some. You know some more proposals coming down the line for the support of that.

**sam** [30:31](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1831s):  Absolutely I think the base issue with this EIP is that I don't think we should put definitions in the Eips repository unless they're also associated with a technical specification. I think that what you're describing is exactly what information is now what I believe. The informational eips
were meant to be right and I don't think we should have them. Why not if they are standardised? they wouldn't be? it's not something that needs to be standardised like the Eips repository is not a dictionary. It's not an encyclopaedia. It's a list of standards and changes to improve ethereum right like that's in the name.

**Gavin John** [31:16](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1876s):  What is the standard if it's not a definition for something. 

**Sam** [31:17](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1877s):  Yes but it's not technically definite. It's not a standard for a  piece of technology. You can build a proposal just exactly .
 	
**Gavin John** [31:27](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1887s):  Here's a definition for a piece of technology you can build it is. 

**Sam** [31:32](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1892s):  But it's not a definition for a term that you can use to describe a particular type of Technology.

**Gavin John** [31:37](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1897s): Same thing with a lot of erc's not you can think of token as perhaps an adjective that can describe
the smart contract there's.

**Sam** [31:49](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1909s):  Right but there's no definition for a token. We have a  Eip 20 defines a standard that uses the word token but we don't have a separate informational EIP that just defines the word token.

**Gavin John** [32:02](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1922s):  Okay fair enough. 

**Sam** [32:06](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1926s): I would have no problem if you forget it was a full descent that was doing this one. I don't remember who was doing this one but if they were making a standard that's  this is you know the interfaces you need to Define this is the architecture for an L2 that is fully evm equivalent. This is the definition of fully evm equivalent and that would be a perfect place to Define it but on its own without some kind of a technical system that it's describing it's. It's pointless to standardise the term because like the reason they're doing this as far as I can tell is so that marketing teams can point to it and be like hey my evm is fully evm equivalent according to this particular EIP and that's just going to turn into a war that I don't want to touch with the EIP process. I don't want to get into like is this you know L2 actually fully evm equivalent or not yeah 

**Gavin John** [32:58](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1978s):  Okay How about it if it describes something that was eip X evm compliant or something like that. Specific head and each number on the term.

**Sam** [33:16](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=1996s): I mean if you were to do that then you could say okay reading that Eip. does it provide enough information for an implementer to create an interoperable  implementation of a fully evm equivalent lab L2. 

**Gavin John** [33:36](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2016s):  With the links it provides yes it does.

**Sam** [33:38](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2018s): Yeah then maybe okay. it's just defining terms is not something I want to get into but if it has enough technical information that you could implement it  then maybe I could be convinced.

**Gavin John** [33:54](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2034s): It links to the things that actually need to be satisfied in order for the term to apply.

**Sam** [34:01](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2041s): Okay well maybe I'll give it another read. Yeah maybe it deserves more of a chance than I've been giving it.

**pooja Ranjan** [34:11](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2051s):  And maybe just to I think if I'm getting it to write on Sam's Point even I would be more happy
to have it added when it is supported by one of the or technical specifications. I do not mean a technical specification in general but I mean a proposal which is 2982. The serenity phase zero when it went into the informational category was blocked in the beginning for so many reasons I don't want to get there but it actually defines many things that people would be interested to learn about and there are proposals which are using these terms and this proposal is ultimately getting referred to. If the present Proposal with a 6269. The full evm equivalence contains this kind of element then it would make more sense to have it added in the ethereum repository rather than a promotional tool for any other project to say that we are fully evm equivalent. Okay so we do have this item added in the pull request form that is 6269. I think we'll try to say if we get any consensus on the pull request and if it is merged. if not then we'll bring it up in the next meeting.

**Sam** [35:50](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2150s): Sounds good 

- [New contract interface and EIPs should be required to include a privacy considerations section ethereum/EIPs#5682](https://github.com/ethereum/EIPs/issues/5682)

**Pooja Ranjan** [35:53](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2153):  All right moving ahead the next one is an issue number is 5682 new contract interface and EIP should be required to include a privacy consideration section.

**Gavin john** [36:09](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2169s): Again I think we should just replace it with a consideration section and privacy and security subsections. 

**Pooja Ranjan** [36:21](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2181s): Okay all right I think we had some discussion in the last meeting because we did not have any consensus on this. It was supposed to be brought back here again.

**Gavin John** [36:41](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2201s): I mean I'm in favour of including privacy considerations. I just think that if we are going to have a bunch of consideration sections then they should be organised to consider different types of considerations.

**Pooja Ranjan** [37:00](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2220s): Okay if I get it right and if I'm not missing this point. I think Matt was not in favour of this proposal and we did not have enough time to discuss it last time.

**Sam** [37:14](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2234s): I'm also not in favour of it.

**Pooja Ranjan** [37:18](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2238s): okay so we have a tie here. I can see Victor left some comments. He seems to be in favour of it with certain options and Matt is unavailable and given sensitive in favour so what

**Sam** [37:35](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2255s): Like to be clear. I think including privacy concerns in the EIP is great. I just don't think they necessitate or deserve their own section. If somebody wants their subsection.  

**Gavin John** [37:55](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2275s): Right now that's not allowed.

**Sam** [37:58](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2278s):  so why isn't privacy a subsection of security? Maybe I'm not understanding that part.

**Gavin John** [38:06](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2286s): Because you can have something that's not a security issue but that leaks privacy right then that makes it. It's not necessary to inject windows ethereum. It's not a suggestion. It's not a security issue to do that but it allows for fingerprinting.

**Sam** [38:32](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2312s): Right and then by being fingerprinted that's a security issue. All privacy issues are a subset of security. Sorry all privacy issues are in a subsection of security issues. There I don't think there are any privacy issues that aren't security issues. 

**Gavin John** [38:51](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2331s): Nonetheless I think we can definitely distinguish them into two categories based on the leads information about the user and can be used and does not leak information about the user. I think that is definitely something that could be done.

**Sam** [39:19](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2359s): Yeah I don't know. I guess if this is going to keep coming up over and over again on the eipips. I guess I'd be okay with an optional privacy consideration section at the same level as security considerations. If people want to include it

**Gavin John** [39:44](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2384s):  What do you think of making a subsection?

**Sam** [39:46](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2386s): Well I just don't have a section called considerations because I know people are going to abuse it.

**Gavin John** [39:52](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2392s): Well except I there are good reasons to abuse it. If it's hey you shouldn't use this effects y z  that's not related to security or privacy then that deserves to be in there.

**Sam**[40:10](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2410s): Oh no
I know what  people are actually going to do. If they're going to take like motivation content and put it in there. They're going to take rationale content and they're going to put it in there. Its people are just going to put it in the wrong section. They already do and it's just gonna be worse.

**Gavin John** [40:27](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2427s): Maybe if we update the EIP template to. Yeah I like it if it's clear what the section is about. I think that issue can be mitigated. Maybe it's something like implementation considerations.

**Sam** [40:51](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2451s): I feel like that's what it used to be called a long time ago but I might be wrong or at least that this discussion came up before. Our privacy considerations really are implementation. Well yeah I mean there might be considerations that aren't necessarily for implementers they might be on the user side or or something like that I don't know when using the CIP.

**Pooja Ranjan** [41:21](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2481s): Okay I think here are two things, we are trying to discuss when we are trying to move an EAP into like you know final status. We are trying to provide a standard that could be used by any other application developer or project developer to have it. Implemented so the implementation or the consideration that we should like to have it over. There should be for the implementers only not for the end users. The project could be providing the take consideration or any other consideration that they may have for implementers if there are any considerations. They are generally provided in security concentration if that is related to security. Otherwise privacy concentration. They might want to give it a thought on how many of those kinds of proposals. Do we receive and do we really need to have privacy consideration for a room in the EIP Repository?

**Sam** [42:21](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2541s): I don't think we do but that's just me

**Gavin John** [42:27](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2547s): I think it would be okay at the very least I would be in  favour of adding an OP  if the compromise is adding an optional second level privacy consideration section then yeah we can go ahead and do it.

**Pooja Ranjan** [42:52](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2572s): I'm open to not bringing it up again because we have brought it for two weeks. I mean two meetings consecutively but  maybe we can take it from the pull request and try to collect more consensus from editors and people over there because this is something which is sounding like we don't have a consensus and we do have to do additional editors missing on the meeting. Is that okay?

**Gavin John** [43:22](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2602s):  I think it is definitely the case that we do not have consensus on that.

**Pooja Ranjan** [43:29](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2609s): Okay for this one I am going to add that it will be discussed in the repository to collect more feedback and we'll see what is the final decision and go there.

- Change requested for Final EIPs

**Pooja Ranjan** [43:42]](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2622s): Moving on to the next sub item which is a change requested for final EIPs, though we know
that we do not encourage making any changes to any eips which are into final status.The way are still getting some requests. I have added two pull requests here. The first one is 6330 which is to update 5192 and the other one is 6314. 

- [Update EIP-5192: Change name to "Lockable tokens" ethereum/EIPs#6330](https://github.com/ethereum/EIPs/pull/6330)

**Pooja Ranjan** [44:11](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2651s): Let's  talk about 6330 what people think.

**Gavin John** [44:17](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2657s): I mean it doesn't work well. It changes the spec but it doesn't like to significantly change. This back there are some wording things and it changes the title. I don't want to encourage it but this seems a really minor change.

**Sam** [44:40](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2680s): To me it's a final EIP it shouldn't change.

**Pooja Ranjan** [44:45](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2685s): If it helps it is coming from the author.

**Gavin John** [44:54](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2694s): I think it makes sense for clarity purposes to try to get rid of the word soulbound. 

**Sam** [45:04](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2704s): The argument here is that these aren't really soul-bound tokens. 

**Gavin John** [45:09](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2709s): The argument here is that literally The soul bound doesn't make much sense to use anymore because people have stopped using the term foreign.

**Pooja Ranjan** [45:24](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2724s): I just noticed this on my back. So here the proposal is to change the name of the proposal. All together when it turned out to be a funnel proposal.

**Sam** [45:34](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2734s): Yeah exactly 

**Pooja Ranjan** [45:35](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2735s): Oh that's not a good idea.

**Sam** [45:37](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2737s): Yeah I think  this is final, we shouldn't change it.

**Gavin John** [45:45](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2745s): And the thing I'm told about is the fact that it would actually change the citation. So it would actually change the name and basically any citations to. It would disappear but I don't think people cite eips anyway.

**Sam** [46:04](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2764s): Not yet. Yeah I don't know like I said this isn't a soul-bound NFT. As far as my understanding of soulbound goes , it's also finally IP. So personally I just think it's final. it doesn't change we move on.

**Gavin John** [46:29](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2789s): Yeah I'd say as per the current criteria it probably shouldn't be merged but at the same time I think that the current criteria are flawed. This is clearly a backwards compatible change. This is changing only the name and removing the word soulbound.

**Pooja Ranjan** [46:58](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2818s): I don't think that it's gonna be liked by many other people after an EIP gets into final status. We are changing the name because that is something which is highly noticeable and it may not leave a good impression that  was not supposed to be soul bound. we should not have allowed it to move to the final status in the first place.

**Gavin John** [47:23](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2843s):  So I think the best that's fair enough but at the same time I as as previously mentioned I feel like final status altogether should be there to demonstrate how much the standard can change
animal and I also would like standards to be able to change a little bit more while they're in final not the actual specification that should never change but clarification should always be something that can be done.

**Pooja Ranjan** [48:04](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2884s): Yeah, there have been some sentences that are changing in the documentation. Could have been fine but changing the title altogether is not gonna reflect well on us. I mean  if there are implementers for this particular eip. There could be one or two or at the  Max five projects implemented. So we are restricting damage for five projects instead of  re-announcing to the world that this is something that is possible even after an EIP gets into final status. They can request for the name change there.

**Gcolvin** [48:43](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2923s): The final is final if there's an error there can be an Errata otherwise there's no reason to touch.

**Sam** [48:51](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2931s): It does fall under errata.

**Gcolvin** [48:58](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2938s): I don't know.

**Sam** [49:00](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2940s): Okay well I think that's what we're discussing. 

**Gcolvin** [49:01](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2941s): it doesn't sound like it does but the author is not present. I don't think so. 

**Sam** [49:08](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2948s): No the author is the one making the change.

**Gcolvin** [49:15](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2955s): We can discuss it with the author on the pr or elsewhere.

- [Update EIP-1559: Remove empty test cases ethereum/EIPs#6314](https://github.com/ethereum/EIPs/pull/6314)

**Pooja Ranjan** [49:24](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2964s): Sounds good. Okay, we can probably discuss the next PR which is PR number 6314ur and it is to request changes to one of the most popular EIP eip 1559 and it's about removing empty test cases.

**Gavin John** [49:49](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=2989s): So yeah there is literally a test cases section with the word to do in it. Capital all caps that's literally the content of the test cases section. Yeah 1559 so I think what happened is that
Cascades are mandatory for core eips and they just forgot to do them but I would argue that it's probably worth just removing them just because it looks bad to have to do it.

**Pooja Ranjan** [50:27](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3027s): I mean we cannot deny that there were cases because we are talking about eip1559. However we would not have added the link because at that time there was this policy of not adding links outside the repository. So yeah I'm kind of okay I don't know what other people think of removing this to-do section.

**Gavin John** [50:47](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3047s): This seems like enough it's rather right this is an error. There should not be a to-do in a final EIP.

**Sam** [50:57](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3057s): If we can link to the actual tests that'd be better but I'm also okay with removing that.

**Gavin John** [51:01](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3061s): But now we should just remove it.

**Sam** [51:05](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3065s): Yeah I'm fine with that.

**Pooja Ranjan** [51:06](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3066s): Okay so do we need any author's permission here.

**Sam** [51:12](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3072s):  I don't think so.

**Pooja Ranjan** [51:17](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3077s): Okay, so we are agreeing to merge 6314. All right we have five minutes more we already have yeah please go ahead

**Gavin John** [51:28](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3088s): I guess we could discuss 74712 final changes.

**Pooja Ranjan** [51:39](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3099s): Oh I'm sorry, it is not listed. can you please help us with the number pull request number.

**Gavin John** [51:47](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3107s): Let's see 5457. This thing so this was one where I think oh and it said this PR is updated. so what
What happened was that 712 due to an Erp W bug got actually merged with two specification sections without anyone knowing and merged as final with two specification sections that are mutually incompatible.

**Sam** [52:26](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3146s): Wait I thought we merged the one that fixed that or did we not oh God. We didn't.

**Pooja Ranjan** [52:45](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3165s): So what is the proposal here are we suggesting to merge it because I heard you're mentioning it's out of date. Yeah if the current pull request is good to be merged or should we just simply close it.

**Gavin John** [52:56](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3176s): I'm just gonna actually manually go into the PR and fix it for the authors of this PR. If I can find where the second specification section begins. There we are okay so now I believe it is up to date. So there were two errors, one there were two specification sections that should not have been that. There was an additional specification section that shouldn't have been there and some stuff left over from the forking of the original ethereum design messages at eip. I argue that this is backwards compatible because there's nothing that could have claimed to
implement 712 could have because there's nothing that could have implemented it. So it's backwards compatible because there is nothing to be backwards compatible with.

**Sam** [54:13](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3253s): I don't think backwards compatibility is the gold standard for this. If someone were to write eip1559 let's say and completely had the wrong calculation in it from what all the clients made the Eip would have to be updated to match what the clients implemented. It's not backwards compatibility is nice and but it is not necessary

- [Update EIP-712: Fix eth_signTypedData definition ethereum/EIPs#5457](https://github.com/ethereum/EIPs/pull/5457)

**Sam** [54:35](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3275s): So we
should just take whatever the correct 712 is and put it in there.

**Gavin John** [54:44](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3284s): I believe I have updated that PR to do the correct 7110. All right. 

**Sam** [54:49](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3289s): And that was 5457. 

**Gavin John** [54:59](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3299s): Yes

**Sam** [55:03](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3303s): All right so all I need is author approval now. Right?

**Gavin John** [55:09](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3309s): It has been needing author approval for months now. I think it is safe to say that all the authors have gone AWOL. all right

**Sam** [55:17](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3317s): So I don't know what to do with that.

**Pooja Ranjan** [55:18](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3318s): It's just a minute. I think I have some background here. There was one cat herders William Schwab who has been working with Ramco for some time to push this proposal towards the final status I think  we can probably have reached out to him to reach to Remco to  if we need any kind of permission there because I think this proposal was in stagnant for a very long time. I mean if that's okay otherwise if people agree that it should be merged right away. I'm open to that as well. I'm not a hard stopper here.

**Gavin John** [55:57](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3357s): Actually I from the looks of it. It looks like there's even some more stuff that needs changing. Yeah this is it's hard to it's hard to know what's correct here and what's not correct because 
I'm still seeing even though I removed the duplicate specification section. I'm still seeing some ethereum signed message stuff which should not be in there.

**Pooja Ranjan** [56:28](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3388s): I think the either one would like to close this one and the changes that you think is and bought and then should be getting in come up with a new proposal or new pull request for that. Okay we are at times so I think this could be left here. we can leave this conversation and we'll try to look into this pull request number 5457. Maybe it can be reviewed again and see if we get response from authors and if writers are confident that this is in good shape to be merged. we'll take it from there.

## 3. EIPs Insight - Monthly EIPs status reporting.

**Pooja Ranjan** [57:27](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3447s): Okay yep thank you. All right  we are at a time I just quickly wanted to share about the month's update for eips inside link is added to the agenda. We have vipsinsite.com February 2023. This provides us the information with all the proposals which we have moved from one status to another statuses and in the month of February we have received three final eips
and a lot more changes going on in the EIP repositories you may check out the link added here.

## 4. EIP Editing Office Hour

**Pooja Ranjan** [58:09](https://www.youtube.com/watch?v=UE6MOvSXuJM&t=3489s): And we have added recording to EIP editing office hours for people who are interested in learning about the EIP documentation process or if they have any questions related to their pull requests. They are always invited to join this so they can have a conversation directly with the EIP editor and we will try to help more proposal towards the Final Destination having said  that's all include from the agenda item for today we hope to see everyone in two weeks but the meeting time would be at 1400 UTC and the date would be March 8 2023. Thank you everyone for joining us today. Have a good one everyone take care yeah all right



 ---------------------------------------
# Attendees

* Gavin John
* Gcolvin
* Pooja Ranjan
* Sam Wilson
* Light Client

# Date for Next Meeting: 8 March 2022 at 1400 UTC.


