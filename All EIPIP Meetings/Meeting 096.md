# EIPIP Meeting #96
### Meeting Date/Time: December 13, 2023 at 16:00 UTC
### Meeting Duration: 60 mins
### [GitHub Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/300) 
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=poqOUTvvaoc)
### Moderator: Pooja Ranjan
### Notes: Meenakshi  Singh
### Next Meeting Date/Time: January 3, 2023 at 15:00 UTC
____
## 1. EIP Process Standardization

**Pooja Ranjan** [0:00](https://www.youtube.com/watch?v=poqOUTvvaoc&t=0s): Welcome to EIPIP meeting 96 this is issue number 300 on EIPIP GitHub repository. For discussion today we have on agenda EIP process standardization some issues and Pull Requests those are new and people would like to discuss perhaps there would be information on Call for Iinput. And we'll have insights on our monthly EIPs ERCs status reporting. 

### Updates on pending tasks for repo split

So starting with the first item which is updates on Pending task for repo split. I wonder if we have any update on the list there and is it the correct list that we are still going to follow. I don't see Panda on the call. I wonder if anyone else has any update? Very well. We can get update from Panda Async. Moving on to the next topic which is Web Page Rendering. In the past meeting we had quite a few discussion on how do we want to see the web page rendering. And I know Sam Wilson has been working on that. So Sam if you would like to take it from here and share how are we seeing this web page rendering and what is the approach we taking here?

### Web Page Rendering

**Sam Wilson** [1:26](https://www.youtube.com/watch?v=poqOUTvvaoc&t=86s): Sure so I've been working on getting EIP review but to work for working groups I haven't changed anything about the rendering of my prototype yet.

**Pooja Ranjan** [1:38](https://www.youtube.com/watch?v=poqOUTvvaoc&t=98s): I'm assuming that we are in a position to have all three of them being reflected on the same domain maybe with some complexities on UI side.


**Sam Wilson** [1:52](https://www.youtube.com/watch?v=poqOUTvvaoc&t=112s): I still think it's possible I haven't worked on it.

**Pooja Ranjan** [1:56](https://www.youtube.com/watch?v=poqOUTvvaoc&t=116s): Okay. Before we move on is there any other question on web page rendering? Very well. We can follow the updates in following meeting and also on the Ehereum  Cat Herders, EIP editors, Discord Channel, if people have thoughts suggestions and would like to learn more about it. 

### Need a process for moving/cloning EIPs as RIPs and how they are numbered.

**Pooja Ranjan** [2:21](https://www.youtube.com/watch?v=poqOUTvvaoc&t=141s): There is this next item which is need a process for moving cloning EIPS as RIPs and how they are numbered. So basically it is here for discussion suggested by Andrew and Associate editor. Let me give a bit of context here. So one of the proposal which was pursuing as a EIP has now been moved to RIPs GitHub repository and the question here is whether that RIP contain the same number that was allocated as an EIP or it should be allowed to have a new number. And we are hoping to see a process in place wonder what editors thinks here.

**Sam Wilson** [3:14](https://www.youtube.com/watch?v=poqOUTvvaoc&t=194s): So if we're moving it in the same way we moved ERC's. I think it's probably fine to leave like a placeholder on the EIPs repository that redirects but I'm not even sure if we've ever discussed for whether we're adding our RIPs to the EIPs process.


**Pooja Ranjan** [3:37](https://www.youtube.com/watch?v=poqOUTvvaoc&t=217s): I would agree this is a discussion that's worth having here. But just for some more context here as we know that there is a repository which is Ethereum/ RIPs. And the proposal under discussion here is the pull request number 5 in this repository. I just shared the link here (https://github.com/ethereum/RIPs/pull/5). Yeah so the idea here is to
move this proposal under RIP category because it seems that it would be adapted by the L2 projects rather than the being deployed on the ethereum mainnet. However the category mentioned here is core which I think is not the appropriate one. I'm open to open this platform to maybe discuss what do people think generally about considering RIPs or the involvement in the RIPs process.


**Sam Wilson** [4:52](https://www.youtube.com/watch?v=poqOUTvvaoc&t=292s): So I'm in favour of making a like Layer 2 working group. I don't think we should pull them in until we have a more formal process for working groups. But yeah generally I'm in favour of it.



**Pooja Ranjan** [5:15](https://www.youtube.com/watch?v=poqOUTvvaoc&t=315s): Just for some context here like historically proposals have moved from one type or category to another type and category. And we try to retain the same number also when the migration happened from the EIP ERC Repo split. All the ERCs moved to a different GitHub repository retained the same number. So in my mind I feel like it would make sense to keep the history of the Proposal even if the proposal is being moved from EIP repository to RIPs repository. It should contain the same  number. Just to have the history of it draft and review because the proposal is getting into the last call although there is no Clarity on like the last call process. I'm hoping that RIP team will discuss it internally. And it will be communicated unless someone from the team would like to share here. I mean join the EIPIP meeting and would like to share it here. But yeah any other editor has any thought, please share.


**Gcolvin** [6:18](https://www.youtube.com/watch?v=poqOUTvvaoc&t=378s): A few things Their meeting is at the same time as ours so that makes causes some troubles with coordination. I think clearly we need to keep the numbers series such that there's no conflicting numbers or there'll be just total confusion. And for last call I think a working group is pretty much in charge of their statuses. So if they want there to be a last call there can be a last call but if they want a different sequence of statuses. And requirements for moving between statuses that's not the editor's business. ust as for the core working group I don't think they want there to be a last call. It's not really relevant to their process. And it's not for us to dictate their process. And the other thing I heard go by is that I think clearly core is not appropriate. Core proposals are specifically those that are going onto the ethereum mainnet and Layer 2 there are multiple Nets that are Layer 2. So they'll have to decide. I don't know what to call them but they're not core.  Yeah Layer 2 is probably their category. 


**Pooja Ranjan** [8:11](https://www.youtube.com/watch?v=poqOUTvvaoc&t=491s): Or maybe RIP just like we have a standard track interface ERC core. We can have standard track RIP that may be able to Define their proposals. But I also feel that core may not be appropriate. And just to respond to the meeting conflict. We are trying to avoid that just like today's meeting has been planned at 1600 UTC in order to avoid the conflict. I have added the alternate meeting time in the agenda. We can perhaps get to there by the end of this meeting. So we should never be in the  conflict with that meeting. Yeah.


**Gcolvin** [8:51](https://www.youtube.com/watch?v=poqOUTvvaoc&t=531s): Am I right that we're leaving basically leaving the status field up to them. 


**Pooja Ranjan** [8:58](https://www.youtube.com/watch?v=poqOUTvvaoc&t=538s): Of course yeah! I mean I can see that it is mentioned on the pull request number 5 on RIPs Github repository that the proposal is in last call and they have mentioned status as last call. But there is no last call deadline added.

**Gcolvin** [9:17](https://www.youtube.com/watch?v=poqOUTvvaoc&t=557s): I mean, I haven't had time to look at any of this. I am essentially 6 months behind in the work I'm doing for our startup. And I'll probably remain 6 months behind for another year. But it's just real important that working groups that are actually organized like the core working group is and like this working group wants to be have complete control of their own process. 

**Pooja Ranjan** [10:01](https://www.youtube.com/watch?v=poqOUTvvaoc&t=601s): Sure we'll continue to follow the meetings and we'll be able to share more updates and upcoming meeting about RIPs. But in general from this discussion taking it that people are open to have a working group as RIP and the numbering process should be a part of for the EIP ERC numbering which I think is being maintained as of now as well. Anyone has any other thought to add on it before we move on. 

**Gcolvin** [10:37](https://www.youtube.com/watch?v=poqOUTvvaoc&t=637s): Is there any tooling issue with that Sam?


**Sam** [10:43](https://www.youtube.com/watch?v=poqOUTvvaoc&t=643s): With them having their own statuses that was that's the plan yeah.

**Gcolvin** [10:47](https://www.youtube.com/watch?v=poqOUTvvaoc&t=647s): Yeah and with the
numbering.


**Sam** [10:50](https://www.youtube.com/watch?v=poqOUTvvaoc&t=650s): So the numbering there's some oddness like I'm going to have to special case this EIP because they moved it but other than that it should be fine.

**Gcolvin** [11:02](https://www.youtube.com/watch?v=poqOUTvvaoc&t=662s): Going forward it's not a problem as groups come in to just.

**Sam** [11:07](https://www.youtube.com/watch?v=poqOUTvvaoc&t=667s): Yeah. Try to make it all as automatic as possible. So that if somebody comes in we can effectively click a button make a repo in GitHub and and it's ready to run so.

**Gcolvin** [11:19](https://www.youtube.com/watch?v=poqOUTvvaoc&t=679s): Okay so we're all in agreement that we don't want proposals to have the same number confuse everyone.

**Sam** [11:29](https://www.youtube.com/watch?v=poqOUTvvaoc&t=589s): So there is some ambiguity about that. So Matt wanted to just have a completely separate numbering scheme for RIPs. Tim suggested something interesting which is that each working group should take the lowest available slot greater than the biggest number in that working group. And that would make RIPs fill in the holes of. Anyways it's we can talk about this on Discord there's just a few options. But yes I want each working group to have like the same numbering space.


**Gcolvin** [12:00](https://www.youtube.com/watch?v=poqOUTvvaoc&t=720s): I'm bringing it up now because I can't follow everything that goes by in Discord. I have something like 15 channels that come. Yeah I have to prioritize the ones that I'm paid to follow. 


**Sam** [12:15](https://www.youtube.com/watch?v=poqOUTvvaoc&t=735s): So there will only ever be one EIP1.23 and there won't be an RIP 123. It'll just be unique. But there's some some details that need to be worked out.

**Gcolvin** [12:24](https://www.youtube.com/watch?v=poqOUTvvaoc&t=744s): Because RFC's come in the IETF spans a huge range of working groups covering a huge range of Technology but RFC's come in and they just get numbered as they come in. So there's never any confusion about the RFC number. Something is RFC number something no matter what it's about I just.

**Sam** [13:03](https://www.youtube.com/watch?v=poqOUTvvaoc&t=783s): I think we'll preserve that.

**Gcolvin** [13:07](https://www.youtube.com/watch?v=poqOUTvvaoc&t=787s): Okay I don't care how it happens with the tooling. I just don't want documents in our system to have two different documents to have the same number.


## 2. Discuss Open Issues/PRs, and other topics

**Pooja Ranjan** [13:22](https://www.youtube.com/watch?v=poqOUTvvaoc&t=802s): That makes sense.  okay very well. Let's move on to the next one which is discuss open issues, pull request and other topics. I have listed a few open PR here which I believe are the edits to final proposals. We can quickly take a look into each one of them the first one is on  ERC side I'm sharing the link here in the chat. It is for ERC 1046. It's about fixing typo. The other two are also about fixing typo. And I think they are from the same authors. So yeah what do people think about merging this just keep in mind. It is final proposal.


**Sam** [14:19](https://www.youtube.com/watch?v=poqOUTvvaoc&t=859s): Yeah, I can look through these after as long as they're all minor edits. I don't see a problem. Does anybody object to fixing spelling mistakes in finally EIPs. 

**Gcolvin** [14:32](https://www.youtube.com/watch?v=poqOUTvvaoc&t=872s): These keep coming around and we just don't have an Arata process. You want some indication that you change things. Some changes are bigger than others. ERC 20 came by with a bunch of dead links and its Earls with fixes to them. And there were some others and we've just been missing an Arata and that seems just like a section at the bottom of changes. And for typos it could be as simple as an entry that says on such and such a date. We fixed a number of typos and here's the PR number. 


**Ahmad Bitar** [15:35](https://www.youtube.com/watch?v=poqOUTvvaoc&t=935s): I believe the next topic would would help with this but my question or my comment here would be that I'm seeing a lot of new external contributors who are trying to I think this was pointed out by Dan
to me. People are trying to fix typos and EIPs to form airdrops. So my question here would be is it okay if we allow this should the editor group allow this? I don't know that's my question? So this has come up like before.


**Sam** [16:28](https://www.youtube.com/watch?v=poqOUTvvaoc&t=988s): So if they're contributing meaningful changes what like this spelling mistake. One that I'm going through right now looks like they're actually fixing legitimate grammar and spelling mistakes. I'm okay merging it and if they happen to get an airdrop for it. Then that's a good incentive to fix spelling mistakes but if somebody's like reformatting stuff or like doing minor changes just to get a commit in and it isn't like actually useful then I'd be less inclined to merge.

**Ahmad Bitar** [17:01](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1021s): Makes sense.

**Gcolvin** [17:04](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1024s): But we need  some way in the document some aratus section that indicates that on a certain date things did change. We have the GitHub that you know. We do have Source control which is good but we can't expect the reader of a document to go into the resource control system. We need the reader of a document to know that this version has changed.

**Ahmad Bitar** [17:36](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1056s): The next topic is actually addressing exactly that okay.

### Add EIP: Versioning Scheme for EIPs #8034

**Pooja Ranjan** [17:44](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1064s): All right. So yeah I mean I also had listed this as a separate topic for discussion like specify condition under which final EIPs can be updated. We can perhaps get there and try to identify the points that we would like to be document. And where we would like to be document all of them. And if that's okay we can perhaps move on to the next PR which is EIPs PR number 8034 about Versioning Schemes for EIPs. And we are joined by Dan and Ahmad to maybe talk about it. So yeah please go ahead and share about this new proposal. 


**Dan** [18:28](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1108s): Hi everyone my name is Dan. Just a quick background for people that might not know me. I joined the EF testing team in this year in April. Working alongside Spencer who's also in Nicole and Mario Vega and I'm mainly working on tests for the EVM and infrastructure in order to help execute those tests in the in the best possible way. So one thing that crossed my mind while working on this infrastructure is it is quite difficult to track changes EIPs and this is something that Greg just mentioned right now. It's not only software testers it's also other members of the community who are reading EIP online. And so I was talking to Ahmad Bitar about this while we discussed testing infrastructure and Ahmad suggested that we introduce a Versioning Scheme for EIPs. And it was music to my ears. And I basically set about like writing down how this could look. And so Ahmad and I have been working on this idea about introducing basically semantic Versioning Scheme that is mainly based on an EIP specification section. So like a major minor patch scheme and Patch would exactly fit into what Greg just mentioned with like arata. So like if it was a typo fix you can bump bump the patch version but you know that there's been no serious change to the EIP. Then the minor version would be responsible for if there's any new. So the other two the minor and major I should say sorry are really correspond to the specification section. So the minor section would be whether there's been new input or new part of the specification which require additional implementation on clients or additional tests to cover that. And the major version would be reserved for breaking changes to the specification. So if implementation just needs to change and it's not compatible with the previous version or tests need to be updated because of that then you'd have to bump the major version that's the basic idea. I'm very happy to share my screen if you want and give a bit more input but yeah.



**Sam** [20:47](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1247s): So I have two questions so the first is when do you envision this being used is this like a pre-final thing or a post-final thing?


**Dan** [20:58](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1258s):  Okay so I think this actually closely ties to the status of the EIP and this is actually a comment that Pooja made in Tim's like meta EIP eth_ magicians thread that essentially as soon as you submit the PR status draft until other people are working on imp implementations but as soon as another team is working on implementation then it would be worth moving it to review. And as soon as  you move to review you have to bump the major version to one and after that you have to follow the versioning scheme before that it doesn't really matter so much. But as soon as implementation has begun then it's worth following a versioning scheme. So everyone is can be on the same page. So that if you're trying to compare different implementations you know exactly which status each implementation is based on a VIP.

**Sam** [21:58](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1318s):  All right and and so who do you propose enforces these rules like this doesn't seem like something we could automate. So this would be something editors have to check?


**Dan** [22:09](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1329s):  I think we can automate it up to a point so I think Github actions could. So I mean I can, share the I don't  know maybe it's just distracting to share the link now. I can share it later. But essentially I would propose that there's a new version metadata field in the header of standard track EIPs and then secondly there's a change log section added. And I think it's quite difficult to write tooling that catches this exactly that a version that a new change log line has been added. And that this version matches the version in the header but I think you could get something quite close but definitely EIP editors would have to be more attentive to this.


**Sam** [22:55](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1375s):  Yeah so I think it'd be fairly easy to you know require that every time you change the EIP. Once it's in review you have to bump you have to change the version in some way and add a change log line like that's that's easy to automate. I'm more concerned about how do we determine if it's going to be a minor patch or or major version? Obviously in the correct order. So that part is either going to be on authors or editors to enforce that. And that requires kind of a deeper understanding of the EIP. And I'm concerned that that might be too much technical requirement but I'm if we're okay with it being like author provided. Then maybe we could do something like this.


**Dan** [23:38](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1418s):  I think the author should be responsible for bumping this and I think they have a good feeling for whether this would affect their implementation or not. Of course there will be ambiguous cases as there quite often not the entire Essence is captured in the specification as precisely as you might want it as doesn't implement it.  But I think in general it should work out quite well. And of course no one's perfect so I mean of course it can can also be mistakes and we can retroactively correct that.

**Sam** [24:11](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1451s): All right and I guess my final question is could we do something where you have to put like minor patch or major in your commit message and then it just automatically renders that in the document. 


**Dan** [24:26](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1466s): That would be fantastic. Yeah not that's not in the proposal at the moment but that's a good idea.


**Ahmad Bitar** [24:36](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1476s): Okay I would just like to add other like we spoke about. I would like to add like elaborate on the  reasoning behind the importance of this. Because I do understand the additional overhead to both authors and editors that this will bring but the benefits that this would bring to both the implementers and that testers or the ones who are implementing the tests are outweigh the overhead. That's my belief as there was a lot of instances where we would be surprised that a spec in a certain EIP had changed. I'm speaking as a core Dev who has suffered from this right. We were just surprised that something changed in an EIP. And we were not aware of that change and we looked at the EIP multiple times. We just did not notice that change because there isn't really a way where change the changes are listed right what with the EIP that we are proposing not only there is a version that is in specified in the metadata of the EIP but also there is also a change set or like a list of changes that happens on the EIP. So it specifies in this version this change happened. It would make that both the implementers and testers life way easier where they would be able to know okay this change requires my attention or this change does not look like it requires my attention right because it's just like a lingual change or a typo fix or a spelling  check right something like that.

**Sam** [26:42](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1602s): Yeah I definitely see the value in this I don't need to be convinced that this would be useful for people. I just also don't want to do the work of implementing it. So I yeah it's definitely something we can think about. yeah I think it's a good idea I'm just not sure if we'll have the bandwidth to implement it for a while.


**Gcolvin** [27:06](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1626s): Yeah a couple things one this is what Github is for. So yeah you do have a record in a GitHub of things that are changing. And generally if there's a change in the specification section it's suspicious and should be looked at and changes in other sections should not require any change to the testing/ And two this seems like something that's specific to the core working groups process. And could be handled by the core working group adding a field to the header that they maintain for the purpose. So that it's not an imposition on the editors at all if the core contributors fail to maintain the header. The core contributors fail to use the header the way they're supposed to. It's a problem among the core developers because I don't even know that review is part of their stages right now. I think Dan is not here today. I don't think but I think he had a last he described it there was a different set of stages that are relevant to the Core working Group having to do with where it was in the testing Process.

**Ahmad Bitar** [28:44](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1724s): So I would say we can all agree for example that when an EIP reaches the final stage. And it lands on mainnet. That means that there shouldn't be any changes in the specifications especially. Or a bump in the major or minor versions. And only there could be patches to fix spelling mistakes. And this would address the concern where we like are final EIPs mutable like they can be semi immutable in a way that they can have certain changes but not minor or major changes right. They can have spelling changes, grammar fixes Etc. But not changes to the spec Itself. And I do see that this should and it makes sense to be maintained by the authors or the working group. But in my opinion it is important that the editors also are aware of this mechanic. Because the editors especially like if they are aware of this mechanic they will be able to push changes to PRs. For example spelling fixes Etc or grammar or proper English fixes to the PR without bumping the major or the minor version. And then the testers wouldn't have to recheck the PR that the EIP sorry not the PR  the EIP for important spec changes right. And and like have to see
if they have to rewrite test or change the tests. And at the same time when an Spec change happens both the testers and implementers would be in the no as soon as it lands that there has been a spec change.  

**Gcolvin** [31:05](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1865s): Well if the spec fails to describe the behavior of the mainnet it's wrong. And there has to be an Arata. So again we have to agree on just what the arata look like. If the change is not to the specification section then it should not affect the testing. If it is to the specification section it probably does but the editors are probably not competent to say whether it does. So it's sort of a lot to ask of the editors to look at a change to the specifications section and decide for sure whether it's a normative change or.

**Ahmad Bitar** [32:03](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1923s): Not no yeah that totally makes sense. What I meant is if the editor wish to fix something in the grammar or in the spelling they can do. So even to the specification section without alarming the working group about this change. And there can be just a small patch in the patch version bump where you can just up that number by one. And mention in the change set under the EIP that there was this small spell fix or grammar fix right which would be like.


**Gcolvin** [32:52](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1972s): It still seems like that's what the proper use of Github is for?


**Ahmad Bitar** [32:58](https://www.youtube.com/watch?v=poqOUTvvaoc&t=1978s): I mean the thing is as Dan pointed out out like right now they check the testing team checks the comet. Hash of that specific EIP I'm not sure if they check the check sum of the MD file or the commit hash but either one would change if there's even a one letter change in the EIP whereas if so even a single letter or a spelling check change would require the testing team. Okay we need to change that check sum that we keep checking. Or we need to change that Comet hash
that we are checking for this specific EIP. Whereas if there is this versioning scheme. They would just look at the major and minor. And if they haven't changed then there is no worry and they don't have to check anything but if the minor or major changed. Then they would be get involved right.

**Gcolvin** [34:12](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2052s): I just don't want it to be the editor's job to make.

**Ahmad Bitar** [34:16](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2056s): It's not, I’m not saying it is again. I'm not saying the editors are gonna be involved in anything I'm just saying that this will facilitate for the editors to do their job in an easy way without affecting the working groups operations right.

**Gcolvin** [34:32](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2072s): I think the working groups are perfectly free to add fields to the header for purposes like this.


**Ahmad Bitar** [34:41](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2081s): So the EIP that me and Dan are are proposing are is not only adding a Field to the header but also proposing that at the bottom of the EIP there is like a history of the changes. How does everyone in here feel about adding that?

**Gcolvin** [35:07](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2107s): I guess that's up to the working group again. 

**Sam** [35:17](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2117s): So working groups don't exist yet. So if we want to like think about this either we do it today. Before we have working groups or we do it after we have working groups. And today I just don't think we have the bandwidth to work on this right now. Whether we want to or not and after working groups. I think that's be the time to think about this but like it's either going to be me or Panda pip implementing the tooling for this and you've convinced me that this is a reasonably good idea. And then Greg will get your list of changes your Arata table. And I think that'll be great.

**Ahmad Bitar** [35:57](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2157s): One thing that also I want to bring attention is that this EIP does not go retroactively into older EIPs and apply this and try to enforce this it will only enforce this in on newer EIPs. So there is no worry in that sense I believe.

**Dan** [36:26](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2186s): The idea would this it would be from when this this IPA gets accepted then any upcoming edits to or pull requests on existing EIPs would then introduce a change log and the version.

**Ahmad Bitar** [36:43](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2203s): My question to Sam is if you or Panda don't feel that you have the time to implement the checks. Would you like someone else to help implement them.

**Sam** [36:57](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2217s): That would be great! Yeah if you'd like you we can make a group on Discord or Telegram and we can coordinate that if 


**Ahmad Bitar** [37:07](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2227s): I'm not sure. I have the expertise but I will see what I can do. 

**Sam** [37:15](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2235s): We can talk about it and I don't want to forget about this. I think this is a reasonable way to solve Greg's like arata table. And I think notifying people of important changes is also a good idea. So I'm on board with this it's just it's probably going to take a while. 

**Ahmad Bitar** [37:32](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2252s): Cool.


**Sam** [37:33](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2253s): Are you guys in the EIP editing Discord Channel or?

**Dan** [37:42](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2262s): Not yet okay.


**Ahmad Bitar** [37:45](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2265s): I think I am in the R&D right.


**Sam** [37:50](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2270s): Anywhere yeah just just add me on there and we can set something up.


**Ahmad Bitar** [37:54](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2274s): Okay I'll add you.

**Dan** [37:57](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2277s):  Yeah also happy to help out for tooling or trying to find someone who has the expertise to do it. 

**Pooja Ranjan** [38:07](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2287s): Awesome! Thank you so much for sharing this EIP. I am hoping that this is definitely going to be helpful. As I can clearly see the use case with the core EIPs. However I feel like it will be useful for networking and interface as well. I'm not sure if it would be useful for ERC Github Repository but when this is a proposal a standard it can be adapted by other Github repositories. If they would like to but I suppose Victor had some ideas on the ERC side and yeah just wanted to give a few minutes to Victor if he would like to share anything on the same context.

**Victor** [38:47](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2327s): About providing support for versioning?

**Pooja** [38:51](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2331s): That's right. Yeah. 


**Victor** [38:53](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2333s): Yeah I think we haven't officially talked about this but we've seen a lot of ERC's that either has Arata needs for change like what we see notoriously ERC 712 or an versioning as well like we have seen that for V1 V2 V3. And so we were talking about that but so far we haven't like proposed any specific
solution to it. I think what Dan brought is something that inspires and then shows that across the board there's needed for just the kind of thing. And I think speaking of versioning there's also this concept introduced in it which is called best current practice. I think for things like ERCs that a lot of time needs backward compatibility as opposed to EIP usually go in after half work. Best current practice is something that I think could be evaluated but yeah again I think will take it to the broader forum and solicit feedback from people. 


**Pooja Ranjan** [40:11](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2411s): Thank you so much. On this okay so I'm hoping just for notes taker this will be in discussion people may discuss it on Discord and of course there is a fellowship of eth magician link for further  discussion if people have thoughts ideas suggestions. And if they are open to help us with tooling please feel free to chime in there and we hope to get this proposal implemented in the best way. Whenever it is possible moving ahead I think we have a few call for input open here.
Sam if you would quickly like to run through those proposals and where we are on results because I see that dates have already passed for all of these.


**Sam** [40:59](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2459s): Yeah so the big one that needs input from people. And I don't feel closing and I don't feel comfortable deciding until people say what they think about it.  Dexoran wanted to remove external implementations from ERC20. So he wanted to remove the links to consensus and open Zeppelin's repositories. I like have the suggestion of moving the reference implementation into our repository since they are MIT licensed and we're allowed to do that. So this is issue 287 and if you could either tell me now what your opinion is or comment on it that would be great. 


**Victor** [41:47](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2507s): This is for ERC20 right. So there's two things here for one I think it's generally good who have a reference implementation. And I'm actually okay that they are being cited rather than they are included in our asset. I'm fine either way. I want to give author more. I for giving Freedom that said ERC20.
Specifically I think it's a very widely adopted widely cited ERCs and as a historical documents obviously ERC haven't been following any of latest many of the latest requirement for format. And I'm I need we need a much bigger justification to change it especially the content when
there's no mistake there.

**Sam** [42:47](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2567s): All right so to be clear out of the three options remove them. Move them into our repository and leave them as is.
You would like to leave them as is. 

**Victor** [42:56](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2576s): Yeah I until otherwise convinced I strongly favor leaving the methes.

**Sam** [43.02](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2582s): All right how
about you Greg and Matt.


**Gcolvin** [43:11](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2591s):  There it is I didn't follow all of that we had an older PR just fixing a bunch of dead links this is. Are these links dead at this point or?

**Sam** [43:30](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2610s): No they're live.

***Gcolvin** [43:31](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2611s): They're live so there's no big hurry on this that the document is still totally useful. 

**Sam** [43:41](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2621s): Yes the concern is that we are unfairly giving traffic to these implementations as opposed to like a neutral like
Destination.

**Gcolvin** [43:53](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2633s):  What’s unfair here?

**Sam** [43:55](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2635s): There are you know dozens sorry just to be clear these aren't My Views. These are just the views of Dexrann are in but that were unfairly favoring open Zeppelin and consensus over other implementations that might exist so they're getting unfair traffic because the official Source links to their website instead of not. 

**Gcolvin** [44:21](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2661s): I generally be in favor of of moving it just so far is you know having a canonical Source. It's not going to go away as long as that doesn't amount to a normative change.


**Sam** [44:38](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2678s): So to be clear the files would be copied so literally the exact same files that they link to now just in our repository. So okay out of the three options remove the links entirely, leave them the same or move them your choice is to.

**Gcolvin** [44:56](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2696s): I'd love to see it moved and in general I'd love to see all the broken links in ERC20 fixed. Because it's a very important standard and with broken links it's it's much harder to understand And when the links are fixable they should be fixed we have a PR that's just been hanging out for quite a while on that.

**Sam** [45:23](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2723s): All right 
and Matt what do you think?

**Matt** [45:30](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2730s): Yeah I'm pretty indifferent on the options I think if I had a very slight hearing in One Direction. I Would probably just delete the links but I really quite indifferent.

**Sam** [45:45](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2745s): All right I'll add your comments and then I can close out this call for input the next one is ERC 1271. They want to update the security consideration section. They have a what I consider to be a legitimate security consideration they want to add but it is a final ERC and this is issue 291. If you guys could leave your comments on here otherwise I will be closing it by the end of today. And then finally we have Dax Ran's in  informational EIP describing flaws in ERC 20 this is kind of like a kind of equivalent to a CVVE he wants to add an EIP that says like transfer is proven transfer is bad and has some flaws and he wants people to know about it. So this is issue 293 on ethereum cat herters EIPIP again. If you could leave your comments on here, I'll be closing it probably by the end of day today that's about it. Thanks.


### Changes to Final proposals,  Update 1271

**Pooja Ranjan** [46:54](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2814s): thank you Sam for that and I think the next item here is changes to final proposals. And we are joined by to discuss update ERC 1271. Howy if you would maybe like to provide a little bit of background and then yeah what are the changes that you're hoping to get here.


**Howy** [47:18](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2838s): Yeah so background I'm a smart contract engineer Alchemy. First of all I don't think I should be leading this. I don't have enough information and I'm not like an author of 1271 or something. So like some background information is that we found some weird HKS with 1271 which kind of constitutes like a vulnerability on our end like we're just trying to patch some of our smart smart contracts as well as as part of like the disclosure process. Just want to follow up on what this looks like. But yeah I'm not sure like who should be taking this issue but I'm actually just here to listen.


**Pooja Ranjan** [48:07](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2887s):Got it I don't see Frangie on the call but I believe it was a recommendation coming from Victor. Victor,  I wonder if you have anything to add  here. I don't know if you. 

**Victor** [48:20](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2900s): So how can you clarify which vulnerability are you talking about there.

**Sam** [48:25](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2905s): I just keep when this call is recorded.

**Howy** [48:29](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2909s): Yeah prefer not to share too many details but it's regarding a replay.

**Sam** [48:39](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2919s): Oh yeah I think that I was the one the telegram right.


**Howy** [48:46](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2926s):That is there's a telegram group about this.

**Victor** [48:49](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2929s): Okay yeah I think this is not the best venue for that conversation but I can follow up with you on the telegram.


**Sam** [48:57](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2937s): Well I think it is a good venue for deciding how we want to deal with these in general. It doesn't matter that this security vulnerability is or isn't real. How do we want to deal with security vulnerabilities in general .

**Victor** [49:11](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2951s): Oh yeah that's right yeah. We can talk about that in general the editorial.


**Howy** [49:27](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2967s): Sounds good. So sounds like we'll take this offline thanks Victor and Sam.


**Sam** [49:35](https://www.youtube.com/watch?v=poqOUTvvaoc&t=2975s):Yes I think just to quickly try to get some answers from people here. Do we want to update a final EIP so that it shows a security Vulnerability yes or no? All right I'll call you out by name. Matt, do we want to update an EIP with a security vulnerability that was discovered after it went to final?


**Lightclient** [50:16](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3016s): Probably not.

**Sam** [50:19](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3019s): All right. Victor?


**Victor** [50:22](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3022s): So just to clarify if we are talking about core EIP and then we realize core EIP has security caveats. I'm to start to think about cases and this specific situation is ERC's or so I think we will treat them differently right. For core EIPs did we ever have like security issues is after they they finalized and half work? I couldn't recall on.


**Sam** [51:10](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3070s): I'm not sure. 

**Pooja Ranjan** [51:14](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3074s): I'm not 100% sure but I think with one of the proposals we had to change like one very minus pack. After the upgrade but I'm not sure if that was related to security or not. 


**Victor** [51:30](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3090s): And for the ERC 1271 that they discovered or they happen to encounter it. I have not I have not learned that I need to look into what kind of security issue they are. I think generally security issues need to be point out the best forum is a question. I would be okay of a informational EIP but in these two specific cases I wouldn't like fully associate that with the security flaw like for example if we one of things that ERC 1271  Introduced that. For sometime they haven't talked about for applying chain ID into the signature. Or applying the contracts being signed into the signature and then over the course of discussion oh yeah one 712 over the course of discussion they realized this could be attack surface now that there would be let's say fork of Etc right when the when the merge happens that was an attack surface. And situation like that. And so they started suggesting adding those and then it usually comes in with as a new ERC saying hey in addition to 722 the Says 12. You have to add these new domains so it's adding on top of it it's rather not saying hey if you forget this you can this is security flaw. And likewise for the one that Dex rann has been talking about circulating the idea ERc 1271. If you send something into a contract that doesn't respond well it could get locked there. And that's more of a common sense rather than a security slot I would say because you can do the same for just sending native eth and so in these two situation. I haven't seen a strong need for updating existing final ERC's but I'm all for encouraging people suggesting their own ERC. It's just that either you propose your own ERC or you propose a Single separated informational ERC's but what Dexron did was doing both. And then I think that needs additional Justification. 


**Sam** [54:15](https://www.youtube.com/watch?v=poqOUTvvaoc&t=s): All right so on this like to sum up your feeling so far for this particular case it depends on the severity of the security vulnerability and in General you'd prefer an informational EIP but there are cases where you'd update the the final EIP.


**Victor** [54:33](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3273s): I haven't seen a I would be open to updating final EIP with things like Arrata and says there's security vulnerability you really need to change but I haven't seen a real case so far. Yet that justify such an import change so I would be waiting for it when that comes in and then discuss that.


**Sam** [54:57](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3297s): Okay as a president great and sorry just because we're running on short on time Greg how do you feel about updating 1271 with a security vulnerability that we're not going to discuss on the call.


**Gcolvin** [55:10](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3310s): I don't have an opinion at this point.


**Sam** [55:15](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3315s): All right thanks.



**Pooja Ranjan** [55:18](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3318s): Sam do you think it would be a good idea to maybe you know the conditions that we are trying to specify here for final EIPs can be updated come we can come up with call for input. And we can collect the responses from editors who may or may not be on the call asynchronously and we can perhaps in one of the future meetings list them all for people to Follow.


**Sam** [55:41](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3341s): Yeah. 


**Pooja Ranjan** [55:43](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3343s): Sounds good. All right we are close to an hour mark and I hope we have covered most of the topics that we wanted to cover. We have added the website link for EIPs insight. Then we can find three different tabs for EIPs ERCs and RIPS. RIPS do not have any proposal as of now. For ERCs we have two proposals moved to the last call. And three proposals move to the final status. And yeah before we end of this meeting, I would like to check with the members here participants here what do we feel about skipping one week that means the next meetings. The next scheduled meeting and move the meeting to the odd week that means to January 3rd. And that way we will never be in conflict with rollup or EOF meeting is my understanding.

**Sam** [56:47](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3407s): I'm fine with that. I have nothing on the opposite weeks.


**Pooja Ranjan** [56:53](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3413s):  Perfect and any preference on time 1400 or 1500 what do we want to go ahead with?


**Sam** [57:01](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3421s):  Oh what's the current time like not today's but the normal time.

**Pooja Ranjan** [57:04](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3424s): So 1400 is 900 a.m. when All Core Dev Calls happens and 1500 is like 10 a.m eastern time.

**Sam** [57:13](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3433s):  I'd prefer 1500 but I know I'm a late sleeper. 

**Pooja Ranjan** [57:17](https://www.youtube.com/watch?v=poqOUTvvaoc&t=3437s):  So all right. Yeah so we can keep the 1500 it was earlier as well but because of call conflicts we were trying to move here and there. And so let's try to have the next meeting scheduled on January 3rd at 1500 UTC. All right with that I thank everyone to join today's call. And see everyone in the New Year. In the meantime we can continue discussing things on Discord Channel. Have a great rest of the day everyone.

## Attendees

* Pooja Ranjan
* Dan (Danceratopz)
* Gcolvin
* Howy
* Lightclient
* Spemcer-tb
* Sam
* Ahmad Bitar

