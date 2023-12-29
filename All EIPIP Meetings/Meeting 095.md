# EIPIP Meeting 95
### Meeting Date/Time: November 29, 2023 at 16:00 UTC
### Meeting Duration: 65 mins
### [GitHub Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/297) 
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=qgcphJxvVDs)
### Moderator: Pooja Ranjan
### Notes: Meenakshi  Singh
### Next Meeting Date/Time: Dec 13, 2023 at 16:00 UTC
____


| Agenda  | Summary |
| --------| -------- |
| 1.      |  Update RIP Editors to EIP-1 and Pooja will update Reviewer's sheet |
| 2 . |Maintain EIP-1 as Purpose and Guideline documents. Add links to specific Meta EIP/ERC/RIP to refer to the community to learn more.|
| 3. | @poojaranjan- proposed to begin with 4 WG and circle back in 2-3 months|
| 4. | @xinbenlev- volunteered to create ERC WG|
| 5. | Sam Wilson discussed eips.fyi |


## 1. EIP Process Standardization

**Pooja Ranjan** [0:00](https://www.youtube.com/watch?v=qgcphJxvVDs&t=0s): Welcome to EIPIP meeting 95. This is issue number 297 on EIP GitHub repository. In the past few days I have received multiple queries on EIP ERC repo split. And on how Robos the current feedback loop is between researcher and authors. And also for those building applications and infrastructure. We can use some more clarity on evolving process. This week Ethereum Cat Herdders published a PEEPanEIP video on EIP 5069 with the editor Sam Wilson. Where Sam has explained a high level proposal of working group which we will be hearing more in this meeting and perhaps collect editors' thoughts on this to decide what are the next steps on that. And some of us here may also know that we are also looking for a rough consensus on how we would like to render ethereum standard. We need one website for all standards or we may need multiple websites one for each GitHub repository. And yeah what is the best approach here? I'm hoping to get a resolution on that as well. We also have some issues and PR’s and also call for inputs added for today's agenda. That's on High level what we can discuss here in today's meeting hoping we get enough time to discuss all of them. So I have been redirecting people to follow the EIP meeting to learn and contribute to decision making of the EIP process. As we can see there are a few new participants on the call for them and for everyone following this call later. I would like to begin this call today with a brief high level overview of where we are and perhaps  share my vision also to see how we are taking it forward. 

### High-level overview of EIP - ERC - RIP repositories & standardization

**Pooja Ranjan** [1:59](https://www.youtube.com/watch?v=qgcphJxvVDs&t=119s): So I have added the first item here as high level overview and that is a presentation. So let me quickly share my screen. So this is like we are going to just talk about EIP ERC and RIP standardization. So what we had in the past is like one unified website eips.ethereum.org. We had one repo which is ethereum/eips and we have set of editors called EIP editors. Although there was a split in having EIP and ERC editors. We had unified tooling eipw, eth-bot and other Bots. And data analytics with EIPs insight. Why we made this split because there were too many ERCs with there were too many PRSs getting on ethereum EIPs repo which was not very convenient for people who have subscribed to that. And also coredevs wanted to have their say on EIP process especially which is directed towards the core EIPs and this would also lead to an opportunity for ERC Community to evolve. So what we can expect here is like we have a unified website. I know there is a discussion on that as I mentioned earlier like would we have one or more but assuming for now that we have one website. And we can have independent GitHub repos for like EIPs we can have ethereums/eips . For ERC’s we can have etherum/ercs and similarly for RIPs we might need EIP ERC and RIP editors. And of course customized tooling and unified data analytics website for that. So as most of us may know that at present our EIPs are basically divided into type and category the definition for all these are available on EIP 1. Meta is basically for decision making and process information are for other informations that are provided and a standard track contains code networking interface and ERC. All of those were earlier registered to the ethereum/eips github repository. And when we look at a proposal when we look at it EIP that is basically divided into two parts one is called Preamble in which we have like some standard set of information provided which in most of the cases are unique. Sometimes they are overlap but in most of the cases are unique and those are being helpful for tooling websites those are available. This body structure is what actually defines the EIPs. And I hope that we can perhaps make changes on the body structure. So this header, the Preamble header, is already defined on EIP 1. people can take a look at it. And it sounds like this is like fair list of headers which we can
have on every set of proposals and like on every GitHub irrespective of type and categories. these are the set of statuses except idea because idea is not trackable under any repository we have seven statuses. My hope would be to have standard statuses except the statuses could be defined by the working group or who would want to move onto certain status depending upon their independent criteria. And this is like the high level structure of how we move around EIPs.  EIPs go under draft review last call and final this is the standard moving statuses. And then we have other defined an EIP 1 again. So we recently saw the EIP ERC repo split. It happened in October about a month ago. what changed there is like earlier we had this EIPs GitHub repository but we kept the type and category same. What I would like to see in future is like we make minimal changes and see where we land up. So now we have two GitHub repositories one is EIPs and another one is ERCs all under the github.com/ethereum. What we have here is like meta and informational again that is there with EIPs repository. And under standard track we have interface networking and core. We have moved the ERC section out to the ERC repository. however there are certain interface level proposals which are also used by ERC. So people would like to discuss  that on the ERC repositories as well. So we have kept this category for ERC's as well. And we will have meta and informational of course needed for it. So this is the present Repo split status. And with the status is because it is a clone like the ERC repository is a clone of EIPs repository. And we have been doing well with the moving ahead with the same statuses that we decided earlier for EIPs. There is no change as such no noted change as such. now people may observe that we have an addition of RIPs. A new repository has been created.  So what I am hoping to see here is like an addition of an additional category called RIPs under the standard track. this will not disturb our current framework and like you know whatever the earlier EIPs were there we do not have to make any changes for them. Again will have almost the similar status type but of course the RIP developers may decide on when to move from one status to the another status. So now our GitHub structure looks something like this we have GitHub/ethereum and under that we will have three repositories EIPs ERCs and RIPs. Now we can have meta and informational common for all of them except we have specific categories added for different repository. And this is like for EIPs it is mostly for protocol client teams. This is for application projects and this is for layer 2 projects. Now when we have Github repository separated. We understand what type and category proposals we get in. It is important to have editors. We do have editors for EIP and erc's but I am not aware of RIP editors. It would be really helpful for authors to get the list of RIP editors. Maybe we can work on that. and we will share. I think it's Ansgar and Carl mostly. Okay then I will go ahead and update the editor sheet and have them added over there. 


 ### Working Group GitHub: https://github.com/eips-wg , Rendered: https://eips.fyi/

**Pooja Ranjan** [8:51](https://www.youtube.com/watch?v=qgcphJxvVDs&t=531s): So we talked about working group. Working group is has been proposed in this EIPIP meeting for past few of few times. And it seems to be really helpful. So I'm hoping the working group will be with respect to repository. So we have three different repository EIPs, ERCs and RIPs. So we will have working group accordingly. And as we can see that there are already meetings going on for core working group, most of the things can be decided the proposals can be decided on All Core Dev meeting. However the governance will be something that can be taken care on in the EIPIP meeting which we can talk later on. As of now we do have all wallet Dev meeting for wallet related proposals. And we have All ERC Dev meeting for ERC related proposal. And similarly we are aware of Roll Call meetings that goes on for rollup developers. So this can be the RIP working group. And who would be like participating on these working group? And what this working group will be doing more on that? We will get to that but first take a look at the website. For users who are looking EIPs from a distance they see the website like this All, Core,  Networking, Interface, ERC, Meta and Informational. I would hope that this would not change for users for looking from the distance and We will just add the RIP here. And if we take a look it would not matter much because the first thing that if we click on each of the tab what we see is this thing the number the title and the author and depending upon the status. What may change is the inside of it. The .md file may change. For this particular section the Preamble we hope that it could be consistent and there should not be a problem with that but the table of content will be controlled by the working group. So let's go back to this the structure of the EIP again. The Preamble we can perhaps maintain to have it consistent all over the repository. And this body structure could be decided by the working group. So for example, if people do not want to include test cases or reference implementation as a part of their EIP or they would like to add for example upgrade name for core EIPs they can make the modification in this body structure of the EIP. And that can be updated into the template file that we have for every EIPs. So the Preamble will remain constant and the working group will decide the content of it. Now let's take a look at the Governance side of it like EIP ERC and RIP. I'm hoping that all should be governed with the help of like this group meeting at EIPIP level. So for governance again it would be based on the GitHub repositories that we have. And if people want like if this working group people want that they would perhaps have their separate Sub Working Group. For example for ERC they can have ERC NFT group they can have ERC SBT soulbound token group. And similarly for core they can have core EL, core CL if it is decided by the working group that's totally optional. And what working group will do I know Sam has a lot with the charter. And I hope that we will cover that right after this presentation to understand how he wants to look at the working group. But on a high level as per my understanding what I have added here is like a working group will be consisting the GitHub Repo Editor, the Editor Associate and reviewers that will be added with the help of Charter. That we will learn more about it. And what they will do is like they can control the template of each of the repository like what to include what not to include. And they will also decide on the status criteria when to move from one status to another status. They can do a micro level governance over there. They can accept reject Pull Request if they want to include final proposal in or not kind of thing.  And of course they have independent meeting they can perhaps discuss those proposals in the respective developers meetings to make decision on them. I have added an example over here like what can be the criteria. So for General if we say that okay a draft when proposal is  proposed by a PULL request for review when that is ready.  And for last called generally that is 14 days but it varies in case of core proposal. So this is just one example. So if we want to be more specific about it we can perhaps go for core in interface networking informational or depending upon whatever the category of the Proposal is. We can perhaps decide the status. What will remain constant irrespective of GitHub repository. I hope to see like unique proposal number allocation right now. What we are doing is EIP number is being allocated both for EIP and ERC maintained by a Google sheet among the EIP editors. They coordinate there and they add the numbers and that could be Extended to RIPs as well. If we would like to coordinate here. I'm hoping to see it same over there. Then again we can just live
with 1eips.ethereum.org . I know we have this thing added for agenda for the discussion. If people don't agree fair enough it's just a proposal. And we can have almost a uniform tooling Bots data analytics and everything else. For micro level governance as I mentioned we can perhaps use EIPIP meeting and we can have like call for inputs discussion final EIP discussion. And any coordination related to tooling is needed we can perhaps do that. So we already have covered like we would love to see Preamble common status common tooling common and everything else there are certain EIPs which are going to be uniform EIP-1, EIP 5757, EIP 5069, and am aware that people are willing to have ERC1 and RIP1 kind of thing. But I hoping that if we can have one of the proposal as EIP-1. I will explain it later why we needed one and it would be really nice to have. So for having just EIP-1 what needs to be appended. If we take a look at the current EIP-1 this is how it looks like the table of content. So this contains the information of  how EIP should be written. So these are the highlighted areas where I think it could be a part where we can append it. For example this is like a special requirement for core EIP.  There are two ways to go about it either we can move these special requirements or anything specific to any particular type of per category in their respective read .md file.  Or else we can make it a standard and have it added over here. Why I am hoping to have only one EIP-1 because if we have ERC1 it would be mostly a duplicate of that. so most of the contents will remain same. But we will change very Minor Details. So it would be really nice to see either everything added to EIP 1 back link to where whatever respective repository readme file is or add these specific things to the respective readme file. So EIP format and template. So here we can add like okay for if you are proposing an RIP the template is available at riptemplate.md and we can back link over there that's one way of it. So here simply this is limited to core only it can be either moved to the readme or if we have any specific for any other type and category we can perhaps add that. bottom line is we do not need to exactly copy paste too much. We can perhaps move data depending upon the consensus we get here by the EIP editors to make sure that we have only one EIP-1. I have added this as an example of like if we want to have a the EIP status decided based on the type and category there are very few changes either we can add these changes to respective readme file or update on the EIP-1 itself. I know this will not contain all of them. So I have also added this thing here for people to leave comment and feedback that is reviewers sheet that we are maintaining for active EIP reviewer and ERC reviewers. I'm going to add RIP reviewers here as well for people to refer to but if people have thoughts we can perhaps add it over here. So I did mention that, why we need to have only one EIP 1. So as of now we see EIP-1 is also available on ERC GitHub repository. So when we are looking at tooling it will be like duplicating the same thing. okay EIP one is here from the EIP GitHub repository and it is again here from the another GitHub repository which are there for ERC's. So for that purpose my hope is to have only one EIP-1. And yeah, I just wanted to uh share this and maybe open to questions if there are any? I know, I see a lot of comments here but yeah if anyone has anything to add share agree disagree? Yeah. 


**Sam Wilson** [18:43](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1123s): I think that's a great summary of where we are right now. That's awesome, thanks for putting that together. Sure yeah.

**Victor Zhou** [18:52](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1132s): Pooja that's  wonderful. I really appreciate the effort of putting it is much more clearer. I do have a few clarification question that I like to maybe leave on the comments were asked on the spot  but what is the best way to further the discussion on this.

**Pooja Ranjan** [19:17](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1157s): I mean if there are questions that you think that more editors input would be required. We can perhaps take it here. We can spend another four five minutes to finish up this thing. And then we'll jump into the uh working group concept otherwise I'm happy to respond uh both the slides as well as the the Google sheet that I have shared are on comment mode you can add it over there and we can respond to it there .


**Victor Zhou** [19:39](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1179s): Yeah cool. I think one of the first question I have is that if we are going to have ERC meta and EIP meta and I'm assuming based on meta's policy with regarding they will be imposed specifically within that repository. I'm a big fan of having a one unified website but also in that website. Do we plan to show or how do we differentiate it is a meta for ERC or it is a meta for EIP. And also EIP-1 in your proposal which I'm also in support of the being one EIP-1 for all. How do you show an EIP matter  that is applying to all these repositories.


**Pooja Ranjan** [20:32](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1232s): Yeah that's true. So as I was sharing this rendering here. It can be managed. For example here we have categorized based on the type and category. So Meta and informational are here. As you can see, EIP-1 is added on both the repository as meta. The number one is being duplicate here. So say for example we decide on a process for ERC. And we make a meta for that particular ERC that will be shown here as well. On whatever it is, it does not matter which repository you are saving. If you are creating a meta for a process it could be displayed.


**Victor** [21:16](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1276s): I mean can they is that intention that's a different report will have their own policy making for example like I mentioned some core deps really want to have consider for inclusion. And it will appear on the EIP side of a meta policy as.


**Pooja Ranjan** [21:35](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1295s): Yeah that's right.


**Victor** [21:40](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1300s):  Okay. I understand that. Thanks for that. Awesome work I will continue to ask clarification offline with you and also maybe comment on I'm really appreciate that this is very clear.

**Pooja Ranjan** [22:03](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1323s): Thank you so much. I see a lot of comment over here any specific comment that we can perhaps respond to. I see yeah. Some people are in favor of EIP-1. That is good thing to have. 

**Tim Beiko** [22:21](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1341s): Yeah I was just saying if so EIP-1 is like extremely hard to get changed. So like I think in terms of just practicality if you want to it might be just much simpler to say like adding your link in EIP-1 to another either ERC or RIP and having the process defined there where it's linked in EIP-1 but then you don't need to actually bug everybody involved in EIP-1. Every time you want to change them. So you can have just a section that says you know for descriptions of the RIP process the RIP1234 or whatever link it in EIP-1. So it's easy to find but then the authors of RIP1234 are the ones that need to be involved every time there's a change rather than all the authors of EIP one. Because that can just be much slower.


**Pooja Ranjan** [23:15](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1395s): Yeah that's pretty much I'm trying to advocate here. As you can see I have tried to put it together like the generalized what we can add onto EIP-1. So if we are having status defined on EIP-1 we can just add a sentence over here, please refer to respective readme files of EIPs, ERC's and RIPs and here this eips.md or whatever it is sitting there for readme file for respective repository we can link it back. And people will be making changes at there and it would not reflect I mean people don't have to update EIP-1 again and again. 

**Tim Beiko** [23:48](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1428s): Yeah that makes sense.


**Pooja Ranjan** [23:52](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1432s): Very well. All right. So I think if this is helpful we can perhaps go ahead and try to take a look into the working group that is being proposed by Sam Wilson. I have also added the GitHub link and how Sam would like to see it rendering on eips.fyi . Sam if you would like to take it from here and maybe explain a little bit more on the concept of working group how we can perhaps manage it from there.

**Sam Wilson** [24:19](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1459s): Sure so out of everybody here who's already looked at eip.fyi . If it's low I will run through it quickly and if not I will just skip it. All right I will assume nobody has looked at it okay.So the general idea I've been going on with this is that. So people want their own processes for their own like groups of proposals Core Devs. You know want to have want to get rid of last call and have a considered for inclusion and you know ERC devs like having last call. So that the approach that we took
originally on this is to just split the repositories and let them evolve separately but Greg objected to having separate organizations. And wanted to keep everything under the EIP editor like umbrella. I kind of agree with that approach because in the end they're all documents. So I've come up with a set of tooling and governance documents that describe working groups. So I will hopefully give people a little run through on what working groups look like. So it's all built. This is all you know running code. Yeah so it looks pretty much the same as uh it used toplease ignore the empty content I just haven't written it yet. But yeah so this is built using a completely new pipeline but it looks exactly the same. You can navigate through your Proposals. They all render you know roughly the same as they used to borrowing a few bugs here and there. But the important part is this so each working group is its own website completely separate from the others. They all get their own subdomain of eips.fyi . So this lets each group evolve separately they can have their own templates. They can have their own rendering system. They can have their own eipw rules everything is completely separate depending on which working group you go into but they all render and look like it is the same website for the most Part. How I get rid of this thing go away go over there perfect okay. So a little bit of run through of the actual codeit's divided into a series of eips-wg repositories and each one of these map to a working group. And then there are some supporting repositories we have a pre processor a registry a theme doesn't really matter what they are. I the important ones here are the registry. So this is how we would assign EIP numbers to new proposals. It's just a big long CSV file in git . We also have the pre-processor which takes our somewhat custom markdown files and turns them into something compatible with Zola which is the renderer I'm using for this. There's an automated script for doing the import from the existing EIPs structure so that's all automated. And we have a theme and some build files not going to go into those. So that's kind of the technical structure of of working groups which may or may not be interesting. I don't really know what you guys care about.  But on the governance side we have kind of this Charter document. So let me actually describe the working groups that I'm envisioning first So eips-wg-eips that is the working group concerned with the process of EIPs. So right now we have meta so that's what this is. eips-wg-core is stuff concerning the core Network so networking uh core proposals that kind of thing eips-wg-erc is exactly the same as what it is today. And eips-wg wallet would be a new working group concerned with JSON RPC and related proposals. This one is obviously new and it's kind of coming out of my work with all wallet devs. The other people who would be interested in probably becoming working groups or maybe the NFT community. And RIPs would probably be another working group. I just haven't created repositories for them. Yet I'd also like to say I probably should have said this earlier. This is all prototype it hasn't been approved by anybody, this is just throwing it out there for your consideration. Yeah so going into the charter so each working group will have a charter and the charter describes the scope of documents that that Charter is responsible for. It describes the statuses that uh proposals in that working group move through. and it describes the Preamble. So you know header-like withdrawal reason those kind of things and then you define the sections and stuff of the body. So each working group gets to Define their own Charter like this. These Charters all go into the  eips-wg-eips repository. So to your question earlier Victor there wouldn't be a meta category for each working group. there would just be one meta category for all working groups.and then that keeps everything organized and separate.and then uh there was some discussion in the chat about who gets to approve changes to these documents. So the members of eips-wg-eips again that's the meta working group would be the EIP editors. So any changes to those documents would be approved by EIP editors. changes to any documents and any of the other working groups would be approved by their membership. Each working group's membership would be defined in the charter for that working group. It's down here somewhere so for example in the eips-wg-eips working group it's just defined as the EIP editors. Core for example might say members must have a working client or or something along those lines that's up to each working group. Yeah so that's kind of the overview of what I'm thinking for this. Does anybody have any thoughts on this? Does this seem appealing? Does this seem way too much? Yeah. 


**Victor** [30:34](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1834s): I like the idea that's working groups are the one and then I'm all for having one meta for. It seems if that is the case we need to update the Pooja’s diagram which separate the meta into boxes of each one. So maybe we need to align or clarify that. That said, I think you mentioned that EIP editor will need to approve EIP-1.  And I think in the governance side slide of Pooja's proposal that they will in the future have different ERC editors group and EIP editor group. If that is the case should an ERC have its own ERC 1 or should an ERC has its own kind of ERC major meta. So that they can impose policy separately. So that would be my question.


**Sam Wilson** [31:32](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1892s): So in this design there wouldn't be ERC editors there would be one group called The EIP editors that handles like defining the policies and everything. and then each working group has members. So you'd be a member of the ERC working group. And those members get to manage their own Proposals.

**Victor** [31:52](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1912s): I see. That's great. I find that in this context EIP editors applies to all the entire thing. and then if we still call it kind of felt that EIP has two meanings in this context right now. Either it covers ERC or it doesn't cover ERC's. So maybe it would be good for us to kind of give it a name to so that people won't be confused that this applies to everything thing. And also editor Supply to everything. it seems or maybe we can just call what's in the EIP repository the core EIPs and then we always used it.

**Sam Wilson** [32:37](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1957s): Yeah. So EIP editors would be as defined in EIP 5069. So it would be like the governance file like the list in EIP-1 right now. And then ERC working group members would be the other term. So editors would be one term and members would be the other term.


**VIctor** [32:57](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1977s): Okay. That makes sense. 


**Juan Caballero** [33:01](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1981s): Could we maybe have a soft expectation or a cultural expectation that each working group have one EIP editor on it. Just to make sure the two layers stay aligned.


**Sam Wilson** [33:15](https://www.youtube.com/watch?v=qgcphJxvVDs&t=1995s): Yeah so I think this is like way out in like the future I haven't thought too much about this but my current loose plan is that each working group starts with just one EIP editor on it. And then that EIP editor can choose to add members as they say see fit.

**Victor** [33:33](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2013s): Makes sense.

**Juan Caballero** [33:34](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2014s): Just to make sure I understood the presentation right. The pre-processor and the Zola publication. That's all built into the CI of each working group's repo. So if you Fork if you clone one for RIPs. They just automatically get an RIP Pipeline and they also get to use the number picker and all that.


**Sam Wilson** [34:04](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2044s): Yeah so
there's one so each repository has a GitHub action that proxies to a common GitHub action for all working groups. And then you clone the template, you change your a few like placeholders with the name of your working group and then you're all set to go.



**Juan Caballero** [34:30](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2070s): Followup question how quickly could this be approved. I love this can we just use it. Is there any reason not to just use it?

**Sam Wilson** [34:40](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2080s): So there are some technical things left to be done. The number picker  isn't built yet EIP review bot isn't modified to work with this. And I haven't written enough governance documents yet. uh so there's that and then we have to get Buy in from the rest of the editors. Which is kind of why I  think we're presenting it today.

**Juan Caballero** [35:02](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2102s): Okay. I volunteer to help with the government's documents if I don't know if there's Buy in on this enough Buy in on this call to to keep going.

**Pooja Ranjan** [35:19](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2119s): It will be interesting to hear thoughts from other editors on the call like what do uh people think generally about going in the direction

**Lightclient** [35:37](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2137s): I mean I think all of this looks very nice my only comment maybe is do we need all this process? Like we're creating kind of a complicated structure with lots of documents and procedures and I don't feel like we're. I don't feel like it's as important right now. We're not. I don't feel like we're getting overwhelmed with you know lots of people doing things that's not progressing forward where we need to put structure in place to put them on Rails. I feel like more we're spending a lot of time on process and less time on just editing things. 

**Sam Wilson** [36:22](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2182s): So, I 100% agree with you there. Okay so I agree that we have way too much process. There are currently seven EIP editors and we spend an hour every two weeks plus whatever time editing and like this has been my full-time job. Just making this prototype for like two weeks we spend way too much time on process for how many people are actually doing editing. But I think on the flip side we also have groups that are coming and starting to self-govern. And it'd be nice to preserve their documents in the same way that we preserve core documents. So that's kind of the tension that I'm feeling right now.

**Pooja Ranjan** [37:07](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2227s):And I feel like when when we have these documents in place. I understand that it seems like too much of work because there is something changing here. If we create these documents there would be other groups which will be like you know helped and maybe using these documents for their references. As I mentioned in the beginning of the call that I have been approached by few groups to maybe understand how they can make contribution. I'm happy to mention here like we have been joined by a couple of members of 4337 group here to maybe see how they would be helpful to make contribution to the EIP process. And how to make sure the researchers comments are being Incorporated by EIP author. So there are a lot of things we are having it in different places. What we are trying to do put them together in form of documents. So in future if anybody would want to do something we can just refer to them towards these documents. So it's one time effort in my mind. 


**Lightclient** [38:04](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2284s): What do you mean people who want to do something? 

**Pooja Ranjan** [38:09](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2289s): Say for example there are a few people at ethereum cat Herders Discord. We have integrated a channel especially for 4337 people like there are multiple EIPs with respect to that particular proposal and some curve related proposals. So if they want to make sure that their proposals are getting in they are getting proper feedback and including the feedbacks from researcher and they would like to incorporate that in their EIP to make it a standard to be followed by other projects. They know the process we can just direct towards them they write guide to follow and share their proposal to us for EIP or ERC or RIP editors right.

**Lightclient** [38:51](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2331s): I mean I don't really see how this working group process does anything to affect that. Like these could be three completely separate things and they could just say hey we want to do this curve and then someone in the Discord could say oh yeah you should make an RIP. Llike there's no need to develop this process around all these things if that's what we're trying to solve.

**Pooja Ranjan** [39:12](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2352s): That is one example working group is there to Define what people want of that particular group and categories. For example core people want to have their different set of proposals. I have been informed about another proposal for core which is called versioning EIPs kind of thing. We do not have the presentation group here today but perhaps we will have it in future EIPIP meeting. So if people want to have their own design for Core Group they decide the working Core group will decide what they want to put in on their side of proposals. Similarly for ERC if 4337 wants to contribute to ERC related working group they can do that. So this Charter is just trying to Define an outline for for these working group. Now working group will take care of the responsibility of what they want to keep it in like their governance process will be managed by themselves.

**Lightclient** [40:07](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2407s): But we could also just let them manage their own process without some kind of overall structure around it which is what I originally wanted to do.

**Pooja Ranjan** [40:21](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2421s): Of course yeah I mean that could be done it's just that we would love to have any sort of documentation if a Core Working Group do not want to have so many processes they can just Define their process wherever they want to. And have it link to EIP-1. So people can follow.


**Sam WIlson** [40:37](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2437s): Well I think what you're saying Matt is that we can do all of this without having the EIP editors sitting on a throne above everybody else right.

**Lightclient** [40:47](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2447s): Yeah I mean if there is need for that structure and I can imagine a world where there is need. Like I can see where in a couple years there are lots of people who are trying to do things. And we need these rails for them that makes sense to me. And so I'm hesitant to say like we shouldn't do this but I also know that right now we don't have as much of this need. And like I am generally wanting to go to something that's simple because I feel like we spend, I mean you said it, we spend a lot of time debating how to do things and less time like actually just doing things. So I would rather come up with a framework that just is extremely straightforward and simple where we don't have to debate things. We stop having this mentality of changing the process like the process is the process and we work and live within it for as long as we can. 

**Sam WIlson** [41:46](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2506s): Yes I think we're on two ends of the spectrum here. So one is like process maximalism which is what these working groups are. And then we could have process minimalism where it's literally just anybody just makes a repository and can track their documents however they want. And I think both are fine but this Middle Ground where we are right now where people obviously aren't happy with what we have. I think we need to get out of that.

**Lightclient** [42:09](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2529s): Yeah and I mean I'm not against process maximalism if the energy the effort required in making the process work is not large.Like I think it's good if it's very clear if there's a lot of processes it's very clear how everything works but I'm afraid of is having very complicated process. it requires many calls. Lots of people to make decisions about things and then we're just creating lots of work. And that makes sense when you have lots and lots of things that you need to figure out and you need that process to work through all of those problems. I'm just saying I don't think that we're there where we have so many problems that we need like very detailed process to solve. And so I don't know is that's a question, is the process that you're coming up with is it something that is sort of can run on its own without lots of like heartbeat calls and management or is it something that is going to need a lot of that?

**Juan** [43:15](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2595s): I mean I could speak just to the wallets I talk to through wallet connect. And Kasa and they see this as a process of opening a PR on the EIP process is the one and only option. Talking to people beforehand is a waste of time peer review doesn't exist. Like I do think that the reason ERC's are kind of messy is that they would benefit from a process to you know some sort of pre- discussion before just opening a PR and making more.


**Lightclient** [43:54](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2634s): This is not going to fix that. I can promise you this will not fix the inability of people reviewing things peer reviewing
things.

**Sam Wilson** [44:03](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2643s): What I do think this will fix on on that note is EIP editors can stay ideologically aligned and working group members can be whatever they want. So we'll be able to get people who aren't aligned with our ethers to review things and define their processes without having to worry about them affecting the guarantees that EIP editors provide.


**Lightclient** [44:31](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2671s): So you're saying you're trying to separate the concerns of EIP editors right now where editors are both sort of dictating this process of standardization. And what the values that are should be held with respect to that as well as the actual process of accepting and reviewing standard proposals as they go through pipeline.

**Sam Wilson** [44:57](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2697s): Exactly. So it's like working group members are technically knowledgeable about their area. And they can review proposals but you know they don't get to decide or influence decisions on whether we allow external links or or whether a DOI is a sufficient way to reference a document. Like we can have our policies about preserving documents for historical purposes. And then your working group members can decide whether a proposal is technically sound and technically sufficient.

**Lightclient** [45:30](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2730s): I mean once this architecture is set up how much work is going to go into process versus just straight reviewing stuff and you know actually doing the thing that the standardization process needs to be doing.


**Sam Wilson** [45:48](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2748s): I think the people were in  EIP editor hats will no longer review documents and the people wearing working group member hats will be reviewing documents and not thinking about process.


**Lightclient** [46:00](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2760s): Do we feel like we have people who are going to wear these working group hats because I think we've tried to get people to review these different types of things? And they don't seem to exist. And so I'm like wondering where they're going to just come from now that we have a name for them.

**Sam WIlson** [46:18](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2778s): So we have Kyle from Brave who's very interested in doing wallet related standardization we have Ansgar and Carl that want to do RIPs. You know we have you who wants to do Core EIPs. So I think there's there's some people at least that are interested.


**Juan** [46:36](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2796s): And Kasa is kind of doing this already like I think a lot of the stuff happening in kasa would be happening in the wallet working group if it already existed to be honest. And there's plenty of reviews.

**Sam Wilson** [46:54](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2814s): I guess that's a good question would Kasa become a working group? Or is there at least a path for that?


**Juan** [47:01](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2821s): I mean Kasa is currently It's sort of currently a grab bag that has a few working groups in it. Some of which could just be the wallet working group and a lot of it is sort of offchain or or multi-chain like non-EVM. So that probably some parts of kasa would still need to not be in here. But I do think that yeah like the RPC stuff a lot of the stuff should be here. And like I said, wallets people you know companies that make wallets even more. So now with 4337 don't really know where to go like there's this confusion about how the broader EIP process could work. And I think it would you know I do think those people exist because all of these wallet companies have Dev teams of like four or five people. And I talk to them a lot through wallet connect. And they have opinions and want to have assumptions in common interfaces in common. They just don't really know how to start. 


**Pooja Ranjan** [48:21](https://www.youtube.com/watch?v=qgcphJxvVDs&t=2901s): So maybe begin the work and see where we are after a couple of months. How about let's start with the concept of working group the four broader working group that I shared in in my presentation slide for Core there would be only one working group which is like core working group. And that will include EIP editors for core and if anyone else wants to be reviewing it they can be added as associate reviewer or maybe the working group member. They can be a part of it managing that particular working group. And most of the decisions making with respect to EIP could be taken care by the code of meeting that we have. Similarly for RIP Ansgar and Carl are already there for taking care of that. I'm happy to have them added as editor or reviewers depending upon if wewould like to add them as editors. We have a certain formalities to be done that can be done like adding them to get the notification of Pull Request and everything think we can perhaps take care of that. And let them be informed about the process how to be added as an editor with the help of 5069 EIP and they can follow that that would be onetime job and they can do that. Similarly for the ERC category we have at the moment two groups those are active one is for all ERC developers meeting that can be one working group and another is wallet developers meeting. So let's begin with these four broader category of working group and maybe get back to to working of more than these in a couple of months. What do people think about It? 

**Juan** [50:11](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3011s): Victor just volunteered in the chat to help.


**Pooja Ranjan** [50:17](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3017s): Oh yeah! Victor is already leading the all ERC developers meeting. I think this meeting happens twice a month at a different time to maybe include every participants from all part of the world. So anyone interested to be a part of that for ERC working group perhaps they can connect with Victor. And join the All ERC developers meeting.


**Sam Wilson** [50:40](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3040s): So is the like action item from this to maybe come up with people who would be interested in participating in the Working Groups.

**Victor** [50:48](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3048s): I think both I think we will need people who are interested and also who other people think they' like to be a peer of like they want to know that if they are committing time other people that they're committing time with are also who they ike to work with. So I like to put up a few names and for you guys to review and if you think good we can go ahead and kind of see if they can make Commitments.

**Pooja Ranjan** [51:17](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3077s): Right so what we need at this point of time people who can review proposals coming up in independent GitHub repository for EIP we have a definite set of EIP editors and Associates. So I'm hoping that will be covered and we will be getting the proposal reviewed as by them. But if those editors and reviewers thinks that there should be a process change they would like to change something here and there from the existing one may be able to document them and then share it in the upcoming EIPIP meeting or maybe document it wherever they do not need approval from anybody else except the EIP editors group over there. Similarly for ERC they can do the exact same thing. We need people who be able to review the ERC proposals we have a bunch of ERC PRS open. I know Sam reviews and Victor also reviews and PandaPIP also reviews but we do have a lot of open PRS. We would like to decrease the number of open PR. So we get people who be able to review let them be added as reviewers editors Associates or working group member. Whatever they want to do but just inform how we can maintain it. Like right now  I have created this Google sheet for people to maybe keep on adding. And then if they are being added as editor we would like to let them be listed in EIP-1 as well. We'll make the changes a step by step. So that would be my number one ask from today's call and the number two ask would be about the web page rendering thing. Is it okay? I see this is very much possible that we can perhaps represent the proposal on eips.ethereum.org we can just add our RIP tab over there. We can list the all RIP thing. The high level representation would be same. There would not be any change to the end user except for the .md file. If any group decides to change from the current format/ current Template. 


**Sam Wilson** [53:19](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3199s): Sounds good.

**Pooja Ranjan** [53:21](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3201s): Okay. So I'm just trying to take a look at at least we should cover on the number one agenda item and there is one other thing left on that is the updates from pending task for repo split if I don't see Panda on the call but we do have Matt.I'm not sure if there is any update for issue number 1 on ERC GitHub repository with respect to migration that people would like to share today.


**Lightclient** [53:52](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3232s): I have not done anything. I don't really know what the latest is?

**Sam Wilson** [53:59](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3239s): I loosened up some EIPW restrictions that were causing problems but that's about all I've done so far. 


**Pooja Ranjan** [54:05](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3245s): And I'm hoping.

**Lightclient** [54:05](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3245s): Yeah is it even working right now in general merging erc's.


**Sam Wilson** [54:12](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3252s): About half of the merge, I don't know why the other half don't.

**Pooja Ranjan** [54:15](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3255s): So there was this one issue that was highlighted in yesterday's meeting Sam if there is anything that needs to be done with respect to some of the pull request not merging automatically. Like can anybody do anything about it. Maybe we can take it with PandaPip. Let's see his response on the Discord Channel if he gets a chance to look into it. Yeah we have about 3 minutes left for this call. Anything from today's discussion that people would like to maybe say that they are strongly opposed and they don't want it. I think the decision so far is Clear. We will be going ahead with I mean I'm just repeating the decision if there is any change people can mention that. Maybe four working group as mentioned we need editors we need associate editors and reviewers and maybe a working group members to be participating for the managing of the pull request coming towards the individual repositories. And one of the biggest thing that I think I would like to get a green light from Matt on this one specific because it seems like Panda and Matt are on the opposite corner of this. So Panda wanted to have a unified website and people from Core devs including Matt wanted to have a different website so it seems like there is a way in which we can perhaps have a unified website but represent their content on on their specific GitHub repository. So should we go ahead with that and we continue doing it?


**Lightclient** [56:16](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3376s): I mean how does it work in what Sam built.


**Sam Wilson** [56:20](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3380s): Each page renders to its own subdomain. So they are separate websites but they all link to each other.


**Lightclient** [56:27](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3387s): But yeah but if I want to update my working group like where does that live?

**Sam Wilson** [56:31](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3391s): In your working group.

**LightClient** [56:33](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3393s): Okay I mean I'm not yeah that sounds fine. I don't think that they should all be on ethereum.org like if I link to an RIP it shouldn't ethereum.org.

**Tim Beiko** [56:44](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3404s): I feel pretty strongly we should have subdomains for each working. I don't know if each working group but at least EIPs ERC's and RIPs and then maybe we have specs that ethereum.org which links to each of them plus the python specs or something. 

**Sam Wilson** [57:04](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3424s): So to be completely transparent I'm actually proposing that we use eips.fyi as the root domain for this not ethereum.org And then we could have specs. ethereum.org or something point to that.


**Tim Beiko** [57:18](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3438s): So we would new keep ethereum.org. basically.

**Sam Wilson** [57:22](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3442s): Yeah it would just be so I have a program that can do the bounce redirects like from new and other than that yeah it just be dead. 


**Lightclient** [57:32](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3452s): Oh why?

**Sam Wilson** [57:33](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3453s): Because like core.ethereum.org is stupid. 

**Tim Beiko** [57:39](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3459s): So no but you just do EIPs and then you do ERC's.


**Sam Wilson** [57:42](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3462s): But yeah but that it doesn't really line up with the rest of what like they're not grouped appropriately. 

**Pooja Ranjan** [57:47](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3467s): Yeah I mean my alternate proposal here was like we keep eips.ethereum.org but we keep tabs. Like right now we have types and categories. So what we are basically doing is adding one more category RIP and we keep it as is being displayed there just add another tab it would not.


**Lightclient** [58:05](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3485s): Yeah I mean that that's what I proposed except the tab just links to another subdomain which is a separate website 

**Pooja Ranjan** [58:12](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3492s): That is also doable. It can be done over there as well redirecting to rips.ethereum.org. 


**Lightclient** [58:21](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3501s): Yeah I mean I don't know we can debate the what to do with the eips.fyi but I think we need also need to solve the problem today. 

**Sam Wilson** [58:31](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3511s): Each working group is going to definitely be its own website in my Approach. Like there there's really no effective way to merge them.

**Lightclient** [58:39](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3519s): I mean but are we going to have working groups that have different that use the same prefix because so far I don't see.

**Sam Wilson** [58:47](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3527s): Any each working group has its own prefix.

**Lightclient** [58:49](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3529s): Yeah so then I don't see a problem with eips.ethereum.org erc's.ethereum.org.

**Sam Wilson** [58:54](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3534s): Yeah but then then you'd have like core.ethereum.org and like.

**Lightclient** [58:59](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3539s): Why core.ethereum ?

**Tim Beiko** [59:01](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3541s): We just eip/core like it is today. We have eips.ethereum.org/core. 

**Sam Wilson** [59:08](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3548s): I mean we could but then they wouldn't be separate websites right. They'd all have to go through the same rendering pipeline at the end.

**Lightclient** [59:13](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3553s): I still don't understand EIPs is core. So why would you need core again.

**Pooja Ranjan** [59:19](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3559s): Because EIPs GitHub repository contains networking interface and core and that also contains like you know meta and informational.


**Lightclient** [59:31](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3571s): But I mean those are all core related proposals.

**Tim Beiko** [59:35](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3575s): But these can be Pages rather than subdomains and then if ERC's have Meta. Meta ERCs you just do erc's.ethereum.org/Meta right. Like we do for core now and I think that would work no.


**Sam Wilson** [59:51](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3591s): No yeah but again they wouldn't be separate websites that's one of the things that Matt you were very strong.

**Tim Beiko** [59:56](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3596s): They would right because they'd be eips.ethereum, you'd have eips.ethereum.org/meta and then ercs.ethereum.org/meta right.

**Sam Wilson** [1:00:05](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3605s): But they can't be rendered to separate websites that way. Like the way GitHub Pages works oh they have to be one website. So you'd have them all render and then you'd have a parent one that renders them all together in one chunk. so they wouldn't be separate.


**Lightclient** [1:00:20](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3620s): So, I mean I don't really understand how exactly you've set it up. So maybe what I'm saying just doesn't make any sense.

**Sam Wilson** [1:00:27](https://www.youtube.com/watch?v=qgcphJxvVDs&t=3627s): So if you look in the chat here like doing specs.ethereum.org/core and specs.ethereum.org/erc's to do that with GitHub Pages they all have to render from one repository.


**Tim Beiko** [1:00:41](https://www.youtube.com/watch?v=qgcphJxvVDs&t=s): Right. But so whatever is in this the same subdomain has to render from the same repository right correct. Yeah so, this means if all the erc's are in the same repo. We can do erc's.ethereum.org that will only render the erc's and then we can have slash / for what for whatever subcategories and then we can do the same thing for EIPs.  So we can do eips.ethereum.org/core and that only renders the core ones within the EIPs repo. So I think if they're all in separate repos that would work where basically.

**Sam Wilson** [1:01:19](https://www.youtube.com/watch?v=qgcphJxvVDs&t=s): Then you'd have like wallets.ethereum.org.

**Tim Beiko** [1:01:22](https://www.youtube.com/watch?v=qgcphJxvVDs&t=s): Rright and that's a good one. 

**Sam Wilson** [1:01:24](https://www.youtube.com/watch?v=qgcphJxvVDs&t=s): That's fine if we want to go that way but yeah.

**Tim Beiko** [1:01:27](https://www.youtube.com/watch?v=qgcphJxvVDs&t=s): Will wallets have their specs? Where do the wallet EIPs live? Will they live in the ERC repo or will they live somewhere else?

**Sam Wilson** [1:01:38](https://www.youtube.com/watch?v=qgcphJxvVDs&t=s): So the repos reflect the governance. So at least in my proposal so if the wallet group is separate from erc's it would be in a separate repository.

**Tim Beiko** [1:0151](https://www.youtube.com/watch?v=qgcphJxvVDs&t=s): I'm also late for something else but.

**Sam Wilson** [1:01:54](https://www.youtube.com/watch?v=qgcphJxvVDs&t=s): All right right so before everybody hops off I just want to go over two calls for input. There's 291 which is adding security considerations to ERC 1271. Please leave your comments on there and there is also removing external reference implementations from ERC 20. That's issue 287 that one's past its deadline but I am unclear of what everybody's opinion is. So please leave comments on there as well. And there's one last one which is 293 and that's merging flaws in ERC 20. Just go leave comments on those. Please thank you. 

**Pooja Ranjan** [1:02:32](https://www.youtube.com/watch?v=qgcphJxvVDs&t=s): Well thank you everyone. We can perhaps continue discussing and if there is any more questions needs to be answered on the Discord async. And yeah thank you everyone for joining us today.



## Attendees

* Pooja Ranjan
* Eric Siu
* Sam Wilson
* James
* Lightclient
* Gajinder
* Victor Zhou
* Juan Caballero
* Tim Beiko
* Maintainer.eth

