# 1. EIP Improvement Process Call #12 Notes
Meeting Date/Time: Wednesday, July 15, 2020 at 15:00 UTC  
Meeting Duration: 1 hr  
[Audio/Video of the meeting](https://www.youtube.com/watch?v=5PSQDT1nr2E)  
[Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/23)  
Moderator: Pooja Ranjan  
Notes: Alita Moore  

## 1.1. Decisions Made

Decision Item | Description
---|---
**12.1** | Edson will make a survey to the current editors on the expectations from an editor (time-commitment, qualifications)
**12.2** | James wil look into the necessary permissions and how to setup users with triaging capabilities
**12.3** | A process for removing editors and criteria for removing editors is a future item to discuss
**12.4** | Link to the live EFI document through EIP 1 rather than continuously updating EIP 1; EIP 1 can be used as a hub for statuses instead.
**12.5** | Remove emergency EIP process item until such time that it becomes pertinent


# 2. [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/23#issue-655857894)


1. Onboarding EIP editors, new EIP validator and suggestions.
2. Separation of EIP process and hard-fork coordination
3. Discuss the EIP-1 Brainstorming Document.
    3.a Goals Outcomes
    3.b What we are not doing.
    3.c EIPs TODO
4. Clarifications for how a precompile address is decided.
5. Emergency communication document and checklist
6. EIPIP project board.
7. Postmortem format feedback
8. Review action items from previous meeting

---

# 3. Onboarding EIP editors, new EIP validator and suggestions

Video | [0:00](https://youtu.be/5PSQDT1nr2E)

(Pooja) - Welcome everyone, this is EIPIP meeting 12; we have shared the agenda in the chat, and it is available on the ethereum cat hearders EIPIP repo. So the first item on the agenda is onboarding EIP editors, new EIP validators, and suggestions.

(James Hancock) - Pooja, can you make it so that I can record? Or give me permissions for that, or someone who has permissions is able to record.

(Pooja) - I think that it is automatically recorded and going into the cloud.

(James Hancock) - It doesn't s-- oh it does it is recording. Okay, good.

(Pooja) - So once it is done, I will download and upload it to the cathearders youtube channel where it is always shared with the community

(James Hancock) - Okay. You can continue; I'm sorry for interrupting. 

(Pooja) - that's alright. So we can start discussing about onboarding EIP editors; if people have thought about it; like what should be the criteria, then mabe we can define some outline. e.g. if we have to invite participation from the community or from the people who are activily involved with submitting EIP or creating EIPs and if they would be interested in joining as an EIP editor. What are the guidelines for them on what would be the criteria that we as a group can think of that would invite their participation?

(Alita Moore) - I think Ethereum involvement would be a good criteria 

(James Hancock) - Yeah, actively invovled in ethereum seems...

(Pooja) - So I was thinking that maybe we can give some kind of of a number to that; as a simple example for that is that they might have subimtted a few EIPs if they want to be an EIP editor. If we can give it a number; it would be helpful to quantify the number of EIPs someone has commented on for example.

(Chloe) - A comment here, to understand exactly what would be looked for. Are there specifications that you would want someone to have if they want to edit EIPs? Is it a job that anyone can do whom wants to take part; or is it the case that someone would need certain requirements to even get started?

(James Hancock) - The... So talking about at least... well... two parts that we can talk about historically what they've done and then we can talk about what they should do, or what they could do. A big one historically, the merging of EIP (merging drafts), which requires... uhm, having the formatting done correctly and an, and an, and an understanding of github. So that they can do the githubby things. Something else that they do, into the chat, so the other thing they do is they merge drafts, and the other one is they determine if the PR changes a radda. What I mean by that is let's say someone like Mike find something that's not really clearly articulated in a currently existing standard for an EIP and makes a PR saying that 'this' better describes what the EIP was saying. The EIP editor will need to be able to tell if that is a substanstial change enough to warrant either changing the draft status, changing the status of it, or if it's really just a change in wording, then it really doesn't need to go through any other process, and it is merged without changing the status.

(Chloe) -  Okay, that makes sense; there's probably a lot of different things for people to understand or learn like you were saying that some parts of that might be learning and understanding github, understanding the ethereum community and what's need; so I guess maybe it'd be helpful if there was some kind of generalized.. I don't want to call it a course, but some kind of learning platform that people who think being and editor is something they're interested in, then it's a location to learn what about github you'd need to know, what about the ethereum community that you'd need to know, and maybe there could be a way to onboard new editors to be like "okay, this is what you get started, this is what you'd need to know, this is who you talk to kind of thing"

(Pooja) - sometimes that we talked about this mentorship program, like uh something like kind of providing community education to the many people whom are interested in community for protocol improvement. You know, and providing checks and so on. A mentorship program is a very good idea if we can invite our current EIP editors and kind of having a session with them, documenting the highlights from those sessions as a general guideline for people to understand what is actually required for this posisiton. The problem that we've faced sometime back was that PRs were stacking up so fast that they couldn't be reviewed and so they couldn't be merged. So we are discussing increasing the number of EIP editors to solve this problem. So having a good palce to start is a good idea.

(Edson) - I think we should start with people who are already involved in the rpocess; they would need the least amount of education. And I think each current editor has either many EIPs or they've commented on EIP PRs

(Alita) - We could do a nomination system where already existing editors can nominate others. In this case you would need to be involved in Ethereum to be nominated.

(Matt) - Yeah, I feel like the most difficult part is how do we nominate or possibly deteremine who can be an editor because there's not a clear path. There's already a lot of people contributing, but it's not clear how they can go from a contributor role to an editor role. I don't think we need to be spending time to onboard those people because they're already invovled, but there just needs to be a clear specification of what needs to become to become an editor.

(James) - And we should make it clear what the expectations for being an editor is.

(Matt) - Sure.

(Pooja) - As a group, can we come up with certain points like the expectation that we are trying to set for these people whom want to get invovled? Then maybe if someone is nominating somebody, other people should be able to relate the qualifications of a person with their fit in the EIP editor role. What do people think about defining those rules? For example, a criteria like someone who's been submitting PRs for adding new EIPs again and again; like they have 5 PRs merged or 5 existing EIPs and active participation in EIPIP channel, they are available certain hours a week or something like that.

(James) - I think too that there's kind of two routes to do this. Both should be done, but I'm not sure about the order. Expectations of an EIP editor, or requirements of something that should be written. Maybe it should go into EIP 1 or a draft EIP 1. Which, would talk about what an editor does, the expectations for an editor, it could even be good to say this many hours a week is a good target of what we want from an editor. Like is the role of an editor a 5 hour a week job or do we think about it as a 2 hour a week job; they'd be able to spend 2 hours a week and be able to get whatever needs to be done done between them.

(Edson) - A way to do that is to ask existing editors. I don't think any are on the call but Hudson, Astic aren't here (asks James if he's an editor, James says no).

   (James) - I was asked earlier and I fell into the position of hardforked coordinator editor, but it was a little weird to be doing both of those thing.

(Edson) - Ya, so we can ask Gregg or any of the other editor for their input; what they do, and what their opinion of what they think is good as a requirement. Also, who would be qualified to do what they're currently doing.

(James) - Yeah.. Could you do a survey like you did before?

(Edson) - Yeah, I can make a survey.

(Pooj) - The hard part here is that this role is a volunteer role. So people whom are actively invovled and whom care about the community and are actively involved must be volunteering. Recently I brought up this topic because we received some interest from the EIPIP gitter channel. Someone expressed interest, and I have seen him actively involved and he's been doing PRs actively. I was confused who he should speak to him. It would be very helpful to have the basic criteria for this. We should document these things, because information is very limited at this point in time.

(James) - Previously, there hadn't been a new one for a long time. I know this kind of anecdotally, but I feel like I can represent it pretty well for what Hudson had told me. They told me that after doing some work in the EIP repositories, someone asked to be an editor, and the current editors sat down and thought about it, and they approved the request. They then just made the person an editor.

(Brent) - Gregg had posted that he supports Mika being a new editor. 

(James) - Yeah, so the big ones are actively participate and comment on PRs in the EIPIP repository. Because if you're actively doing that, and you're helping process or review PRs, even if you're not an editor, you can still review a PR and tell what needs to be done for it to be merged and things like that. The other thing is that Matt and I put on the agenda the idea of having a smaller group of less permissions that can do certain things.

(Matt) - Yeha, I put a contributor sheet on Github which is just for triaging issues. I think that would be very helpful for people whom are interested in getting started going down a path for becoming and EIP editor in the future. But it kind of just gets in the way to have to be in the gitter channel constantly. If you think that it's good, and you think it can be merged by an editor. I think that if people have a triage permission, they can just add on labels for a pull request, so an editor can come in and see what could be ready to be merged. Maybe something that's been abandoned and closed and wouldn't required write permissions to merge it to the repository. I don't really see any harm from having people there and having a tighter feedback loop. If they're adding labels that aren't making any sense, then they can removed quickly, and they wouldn't be doing any harm to the repository itself.

(James) - Yeah, and how do we turn said thing on?

(Matt) - I think it's pretty straight forward if you go to the github organization settings and then you add someone as a triage-contributor, it's somewhat has permissions to do that, and I could probably walk through it.

(James) - Okay, we can talk later. I propose that anyone whom wants to become a triager, and then we just make them it. If there's an issue with how they triage then we figure out how to address or remove them. So a process for removing people whom aren't being active or things like that. So it'd be easy to say yes to anyone that asks, and think of ways to weed people out whom aren't being helpful.

(Matt) - Yeah, if they're consistently being helpful then that makes them a pretty good potential EIP editor.

(James) - Definetely, because they'll see that and actively be commenting on PRs. That would allow the current EIP editors if they need more EIP editors and then if the person who's interested fits then it can be a mixture if the EIP editors want to nomiate people or people want to apply, we should allow both to be happening. As to maximize the number of people helping.

(Pooja) - Anymore parts on this topic? As I understand it we will be collecting feedback from the EIP editors about what we should have as an expectation for those to be nominated as an EIP editor. The triage thing about sorting out the issues can be very helpful, but I'm not very clear about the permissions of who can give that or how it can be done.

(Matt) - It's anyone who has control over the Ethereum organization or the repository.

(James) - The Ethereum foundation has permission over the EIP repository. The EIPs are pretty much the editors, but the foundation has the widest permissions.

(Pooja) - In that case, anyone who's currently associated with the Ethereum foundation directly, they can do that and it would be good to have a list of people who we can reach out to or as a reference for other people.

(James) - Sort of, I wouldn't say anyone at the foundation can do it. There's probably only a small group of people whom would actually be able to add owners to the EIP repository. Including the EIP editors are able to do that. Let's add a task to me to follow up on how to give people permissions for being a triager.

(Pooja) - Yeah, that would be great.

(James) - So I can follow up on that, and I possibly I can get permissions to be allowed to do that. And we can start that as a good first step.

(Pooja) - Right, we can note it down for the action items. 

(James) - Yep, and Edson if you can work on a quick survey that we can send to the editors which includes how much do you spend being an editor a week, how much time should the role take, what experience and we can brainstorm questions for a little bit.

(Brent) - Yeah, well what might be a good criteria to indicate someone as qualified for that

(James) - Yeah that's a good question for the editors

(Pooja) - Right, so do we have any more questions or comments on this topic?

(Matt) - I have a question; we talked about building a criteria for what it means to be an editor, and then what kind of work do we expect the editor to do, but if they're not meeting those expectations then we haven't really talked about what happens to them. Is the editor ... list or is it something that with enough feedback they'd be able to be removed from 

(James) - Is (unknown name) still an editor

(Pooja) - Who?

(James) - Ofrey was an editor I believe

(Pooja) - He's no anymore

(James) - But I think he removed himself because of the fiasco that happened earlier. I do think that we need to think of something like that, and the best suggestion I've thought of is to make it based on activity. So if you're not active for a certain amount of time (commenting and merging PRs, basically) you just get automatically get removed or you at least can be removed. Like you're flagged for removal if you haven't done anything for say 6 months.

(Pooja) - We can add that to the criteria and expectations; I have seen the history of it, like () was one of the editors when he was part of Ethereum, but after he left he was also removed from the editors list. So it can be kept up to date depending on who is still active.

(James) - Yeah, I'd say that a mechanism for one to passively remove editors whom aren't contributing so it's an easy way to someone who's moved onto another project or actively in the Ethereum developer space that it probably doesn't make sense for them to be an editor. But going through the politcs and drama of having to figure out how to remove that person is kind of a lot. So one, having some kind of activity threshold of if you're this active, and it could be very low, then have a second process for if the EIP editors feel like someone is misbehaving. This hasn't really happened for us but it definetely happened for the Ethereum classic community. Which was a really interesting case study about what to do, have EIP editors have a process for removing someone who's innapropriately using their editor capabilities.

(Edson) - I think, say someone is doing something unethical, I think it can be moved to majority vote of the current editors. So we just assume majority will behave altruistically.

(James) - Yeah, maybe even a super majority would be fine. Some process that one of those two kind of things. To have that, I think the list would be maintained a pretty high quality.

(Pooja) - Alright, we have pretty good first step here, connecting a survey from the EIP editors; to get an expectation set for the onboarding editors. Then also having a criteria for when to remove people from the list. So we are almost halfway through the meeting, so I think we should timebox this and move on to the next item.

(James) - I'd just like to ask Matt one more question; are there things you're thinking about in regards to a process for removing people?

(Matt) - I mean, my general thoughts right now is that we are trying to scale and EIP editor list of about 8 to maybe the teens or 20 tops, so I don't think too much process is needed. I think a majority or super majority is fine, I don't know how often the EIP editors should meet. Maybe they should meet quarterly to discuss if people should be removed or not

(James) - Ah yeah, that's a good idea. We should add that. I'd be happy to host that. Yeah, so attendance to the meetings is actually a good requirement.

(Matt) - One last thing, if you all have any ideas on requirements please message us that directly on the EIP validator. I'm trying to create a list of things that need to be implemented.

(James) - I have a document where I wrote out a few of them; do you know where that is Pooja?

(Pooja) - I think it's in 2 blues, maybe it's linked

(James) - on the notes for the previous meeting?

(pooja) - No, on today's agenda item number 3

(James) - Oh yeah

(James) - I just put it in the notes, let's schedule something to go over that because I think that'd be a good call to have.

(Edson) - One last comment: I was thinking about this when I wrote the article for the road-map. Say because we are currently still editing the process in the EIPs themselves. If we were to onboard people now, they would be learning the old process, and they'll have to learn the new process very quickly so they'd be doing one thing and then doing another. It might be better to wait until the new process is flushed out and matured before we have people learn how to become an editor and be onboarded was my first thought.

(James) - Yeah, that's a good point.

(Pooja) - I think this will take some time to shape up properly so by the time we are into the new process this thing should be ready. I am hoping it would be ready publicly and it wouldn't be a problem for EIP editors. Moreover the people we are trying to consider here as an editor are actively invovled so it would be a good transition for them also to be onboarded for this process. That's just my thought, though.

(James) - Mika for example would be totally fine. Being able to handle that, Matt would be totally fine to be able to handle that. The new statuses are I think getting pretty solid. Those are the, I think, the biggest ones. It'd be good to have some of that be settled before we really push through this, that's a good point so thanks for bringing that up Edson.
## 3.1. Decisions

- *12.1*- Edson will make a survey to the current editors on the expectations from an editor (time-commitment, qualifications)
- *12.2*- James wil look into the necessary permissions and how to setup users with triaging capabilities
- *12.3* - A process for removing editors and criteria for removing editors is a future item to discuss

# 4. Separation of EIP process and hard-fork coordination

Video | [29:30](https://youtu.be/5PSQDT1nr2E)

(Pooja) - So moving on, the next item is the seperation of the EIP process and the hard-fork coordination. There's some progress in previous meetings about seperating EIP, like we are now having clarity on the EIP process as well as the statuses that we should be referring in the new process. James, would you like to take over from here, and let us know how we should take care of hard-fork coordination and how would we form to split it as a seperate process.

(James) - So the first step in seperating it would be accepting into EIP 1 the new statuses and the transitions between them. And then a lot of work in changing the statuses for the EIPs that currently exist, for updates on the hardfork coordination process, we on the allcoredevs side, we've taken a hiatus about talking about Berlin. If we're working on Berlin then it means to focus on working on client diversity and handling some of the pressures on client developers and other stategies to help prevent burnout and just put client development and put them into a better mindspace. Especially ones that have majority .. share. So the process that we've gotten to so far is to have things get into the eligible for inclusion and that gets applied on the allcoredev calls and people apply to various EIPs we discuss and then through rough consensus they move to that bucket. Then the next stage is they are then implemented into some kind of yolo testnet, which means that all of our clients have to build some implementation of it, but that doesn't mean it's finalized or that it's in the state that it'll go onto mainnet. But it's at least in the state to where they'll see what it's like to run it in a real-world sort of setting on the testnet. I'm kind of waiting to see what happens next because I don't want to prescribe the process, I want to let the process evolve and to have a lot of emergent properties that showed up. And so progress on what happens next after that I think will resume when we restart talking about Berlin. But then recording those steps and then defining them a littl better is the process for.. like the first couple steps that need to be fleshed out more need to be documented more and then decided if they go into EIP 1 or a seperate EIP 1. So that's the update for the status of those two and next steps for all of them. Are there any questions or things about that? I've read an awful lot of information.

(Pooja) - I have one question and maybe concern; so the current EIP 1 talks about the current EIP process that includes the current EIP process as well as the hard-fork process because they're merged together. So let's say for exmaple in the future we want to update the EIP 1 with the seperation of this process what do you think about documenting that in the way of two seperate processes that define it clearly and then we do it. We have seen it for the EIP process, like I saw it very effective and easy for people to grasp it. So how do you feel about having this thing layed out for hardfork coordination plus the status or the term for the status and then we go ahead and update it for EIP 1.

(James) - Are you saying to update EIP 1 with the hardfork or the new hardfork coordination goals? This at the same time that we do the status updates?

(Pooja) - yes; I was wondering if we bring all these three things together and then go ahead and update EIP 1 it would add clarity to people to understand. Otherwise, I'm working people may go blank. Like "fine this is the EIP process, these are the terms, but what about hardforks because it is missing that. It was there earlier but now it's earlier". So I'm suggesting we can get all of these three things together?

(James) - I don't know if the preference is for it to be in EIP 1 or for it to have its own EIP. I mean the hard-fork coordination side or the network upgrade path / pipeline. And the way of tracking it? One is that it's not totally finished, so waiting... I wouldn't want to wait to add the statuses, to update the standardization process in statuses. I wouldn't want to wait for the network upgrade process to be fully specified. Because that will take an unknown amount of time.

(Pooja) - Okay, so if we are not very sure about if both have to be, because I was thinking of a place ot be documented, and at this time we can see EIP 1 as the place of the documentation of every processes related to EIP. But they'd be favoring the hard-fork process into some other seperate documents, I think I clearly understand what you mean by going ahead with the statuses.

(Edson) - I think there's nothign wrong in opening a new EIP for those; seeing as how you can link to it in EIP 1, it doens't have to be included directly. But it also doesn't have to be excluded.

(James) - Yeah, that's a good point. We also have a project board for EIPIPs so it's a good thing to also link to it in the EIP. So yeah, that makes sense, does anyone else have thoughts about if it should go in EIP 1 or start as its own EIP and think about what happens after that?

(Edson) - So we're talking about the hard-fork coordination process, right? 

(James) - Yes

(Pooja) - Well my initial thought is that we should have both of them in EIP 1 but if people have a strong recommendation of keeping it seperate (the network upgrading process) then I'd be fine with it just being referred to in EIP 1. I have no reservations.

(Matt) - I kind of find it strange that EIP 1 has this special status that allows it to be continuously updated over time. My preference is to keep the EIP that's been accepted and then if there's substanstial changes it can be updated. But we're already kind of past that precedence, so I think it's okay.

(James) - Yeah, it's pretty at least helpful for the EIPIP process, and then if EIP 1 has that status, then for the EFI list, having that be something that's updatable without needing to make changes to the numbering makes a lot of sense because it's acting as a registry.

(Matt) - I guess like why would we want to have a list of EIPs that are eligible for inclusion. Why can we not generate this case on their statuses? Why do we need an EIP to update it as a tracker. I think this is something that can be built on top of the list of EIPs

(James) - If it were through statuses, then we are connecting again the network upgrade process and the EIP standardization process. So have we seen the new list of EIP statuses? 

(Matt) - I don't think so, no.

(Pooja) - I think that we may have to connect it at some point in time, so I find this suggestion to be quite useful because we would be looking for some kind of connector being these two processes and being able to seperate it. So EFI is maybe a good one.

(James) - Yeah, so from just the way we've done it so far it's been helpful because someone comes to a meeting and says I want this EIP to be EFI and then we change and add it to the list of current EFI EIPs and that process has worked pretty smoothly. If the statuses include information on its inclusion in a hardfork or into mainnet, then we start connecting the world again that we're trying to seperate.

(Matt) - So what's the status of the EIP that's being considered as EFI.

(Edson) - So EFI isn't an EIP status. It's a status for hardfork coordination, which is in a process for each EIP. So EFI is only applicable to core EIPs whom are under consideration for hardfork.

(Matt) - So the EIPs that have been considered for a possible hard-fork. Do they have to be EFI.

(Edson) - Usually, yes.

(James) - But it could be really any stage. If something was in a final standards page and they wanted to be able to bring it EFI they totally could. So there isn't one status that is required to be there.

(Edson) - So what we're trying to do is externalize the decision making so that it's not part of drafting EIPs itself. What EIPs are included? So, the EIP repos that have options for inclusion in some hardfork that's seperate from any political or controversial position; just to have it exist and be formalized and then the hardfork coordination process can deal with the decision making on whether the EIP should be implemented not really what or how it is.

(Matt) - So what is the argument against having a status that says EFI, that's basically just denoting it's in a pretty stable place and people saying it could be included in a hardfork eventually.

(Edson) - EFI is only applicable to a few EIPs, it wouldn't be applicable to ERCs for example. So we'd be creating a status that's unique. If we were creating a unique status it wouldn't apply to every single EIP. That would increase confusion and complexity of the statuses.

(James) - Another example of where it would have shown up historically. Prog-pow could have been put into a final stage and said this is what the proposal is, and it could be final. As far as the standard. But it doesn't need to be marked as being inelligible for inclusion.

(Matt) - So having these statuses does not mean it has or can be implemented in a hardfork?

(James) - No, it means that the standard is that this proposal is state of the art and any changes beyond fixing typos beyond typos should be done as a new EIPIP.

(Edson) - So for example, in political systems they have a process for drafting bills and then they have a seperate process for including them into law if that makes sense.

(James) - Let me share my screen. Can you make it so that I can share my screen, Pooja? (talks about host stuff of the call).. I have here in the hackmd link that's in the chat there if you scroll down to the EIP status defintion 3 to version 2, at the top you'll see two diagrams. The top one is the one we've settled on. And at any point in the draft review last call final stage something could apply to being included for a hardfork. Then, that would be considered in some other kind of flow. But this flow works for all different EIP types, which is nice, and it's clearly seperated as the EIP standardization process and not a what's going to go into mainnet or not. So another example of where this has come up is Greg's EIP on static jumps. Because it's in EFI, but the current standard is not likely to be the one that'll go into mainnet. But the proposal that Greg had could very easily go into a final stage and say this is the proposal that Greg does and then it could be deteremined seperately if that is the standard that wants to be implemented. There's a few other restrictions that the core devleopers are considering that are above and beyond Greg's EIP; but i've noticed that stuff gets kind of stuck on the what it will look like when it's connected to what's going to go onto mainnet and then it bogs a lot of these things down.

(Matt) - Yeah, I know you guys have thought a lot about this. So I'll think about it on my own, but that generally makes a lot of sense.

(James) - Yeah, and I appreciate the questions and critical questions on that. Because we can't adequately define how we've made decisions when we need to be remaking and rethinking them.

(Pooja) - I'm sorry about the screen-sharing issue. Nex ttime I'll get it fixed before we start the metting.

(Edson) - ONe final comment about that, I think that currently the hardfork meta EIP is its own EIP seperate from EIP 1 and EFI tracker is its own EIP seperate from EIP 1, so it looks like all all hard-fork coordination EIPs are their own EIP. SO that's another reason for why I'm inclined to giving some EIP the hardfork coordination process.

(Alita) - Are you saying that we should merge all those different standards?

(Edson) - So the new hardfork coordination process I think that we should create its own EIP and so when we update it we can supercede it. But for the new statuses we should make a PR for the EIP 1.

(Pooja) - Yeah, I think it would make sense, I remeber this conversation in one fo the previous meetings that we requested that EIp 1 should not be updated so freqeuntly. Historically the hardfork process has changed, so it makes sense that we provide a link to the EFI process is explained and add it to EIP 1 instead of adding it directly to EIP 1. Any more questions or comments on this topic? We are almost at the end of the meeting.

(James) - I think it would be good to have the EIP written for the network coordination, the network upgrade process before we do the EIP 1 for statuses. That actually make more sense. So the next step is to actually make an EIP for documenting the network upgrade status as it stands. That's better so I'm glad we didn't do the other way that I think about it.

(Pooja) - So we can add it as an action item for now, and we can see in the next meeting if we are done with that, then people can go ahead and create the PR for updating EIP 1

## 4.1. Decisions

- *12.4* - Link to the live EFI document through EIP 1 rather than continuously updating EIP 1; EIP 1 can be used as a hub for statuses instead.

# 5. Discuss the EIP-1 Brainstorming Document. 

Video | [50:29](https://youtu.be/5PSQDT1nr2E?t=3029)

(Pooja) - So we have very few minutes left, what topic would we like to pick up quickly? There is one emergency communcations document, adn I'm not sure William are you in the call?

(William) - yeah, I'm here

(Pooja) - Can you quickly walk us through this?

(William) - Okay, I know I'm up against time so I'll try and keep this as brief as possible. I also was not by the last meeting so I odn't know what was discussed there, but the idea of trying to raise an emergency coms team was raised in teh cat hearders so I responded to that. In the meantime, what Pooja arranged was  alittle bit of a team, and what I've been working on has been trying to basically assemble a document tha tboth defines what a state of emergency is for the ethereum protocol platform. Not even exactly sure what terminology to use. And what woul dbe done in such a case. I've also been thinking about how a COMs team would work. This is really the early stages, and I've been doing some twitter polls on what people think an emergency is. At this point, I have two overreaching definitions. Either it's something that makes the network innaccessible or soething that compromises the integrity of the transactions being recorde don teh document: past present or future. Those are both very general but there's a lot of things that you can sort of get into both of those; either or both. So the question is, first of all I'm not sure this is an EIPIP thing, I'm not sure how much this is actually related to teh EIP process if we would need to draft and EIP on teh states of the emergency or what the correct protocol is for handling a state of emergency on what they would want from an innitiative like this. Even if that wuld mean kind fo broadening the scope to something else and just general feedback. 

(Pooja) - So this thing was discussed inthe previous meeting saying that it makes sense that there should be a group that would be proactive in an emergency situation that might come up during a network upgrade or otherwise; so we picked that up from there although I know that cat hearders have already been doing that. I listed it in the agenda this time, adn if people would like to see it again we can bring it back. As yo umentioned, maybe in teh form of and EIP or something else btu if not then I'm happy to keep it on the agenda and continue the discussion with teh cat hearders.

(James) - I would have to think more about it being an EIP or not, but it would fit as an informational EIP.

(Pooja) - My concern here is that this emergency com thing and this document and the checklist that we are tlaking about; I am a little conservative about sharing it with too many people. This document should be with a group of people whom are actively taking responsibility of it and maybe reaching out to the stakeholders at the time of emergency. Even in an informational EIP it would be quite public.

(Alita) - I think there should be an avenue to initiate or get in contact with those who can get more.

(James) - As long as we're not listing out more people in teh informational EIP, like if you document the process, and maybe shephard a few people whom want ot know more about it.

(William) - In other words the EIP should be process; a contact list shouldn't be part of an EIP, especially because that's not something to be set in stone and would mutate with time. So what we would be looking for in an EIP would be some sort of codefication of process but not the specific contacts. It would probably suffice to say major stakeholder or something vague like that instead of providiing contact information

(Pooja) - It would make sense to create a checklist kind of thing at the time said situation emerges. And maybe adding some way to contact people whom are actively involved with the script.

(William) - So it sounds like this should probably be pulled off of the EIPIP agenda and then maybe at such a time when we're ready to submit an EIP it would maybe come back again as an item. Does that sound about right?

(Pooja) - Sounds good to me

(James) - I'd also ask some editors about what they think; I'd recommend that, and everything else sounds good.

## 5.1. Decisions
- *12.5* - Remove emergency EIP process item until such time that it becomes pertinent

# 6. Various Final Topics

Video | [56:08](https://youtu.be/5PSQDT1nr2E)

## 6.1. EIPIP project board
 
(Pooja) - Okay, so we are almost at time but I want to share a couple of things here. We have created this EIP project code, the link is available in the agenda. Everyone can go ahead and look adn check that out. We'd love to have feedback.

(James) - It's so good!

(Pooja) - Thank you ^_^. so we would like to keep it as up to date with the tasks that we are completing, we could then let people go back and see all that we have achieved with this group. Which, would be a great informational sharing platform that would encourage others to be a part of this community whom care about developing Ethereum. There's one last thing that I would like to quickly share about one thing. In the previous call we shared the upgrade post-mortem. But the thing that we did not share was the general template. I'm sharing the link in the chat if people can give it a look, and if they have any feedback or comment, feel free to let us know. Traditionally we have more time to discuss anything else. Anyone else who'd like to discuss something, please speak freely.

...

(James) - Looks good to me, but I'm biased

(Pooja) - (laughing) yeah, we worked together on that; so yeah, we would like to hear more feedback from people and maybe again we will stop at this point and have the cat hearders have some kind of discussion about this kind of EIP. I'm planning to start an ETH magician post about it.

## 6.2. Clarifications for how a precompile address is decided

(Edson) - It might be good to open a PR and then change the EIP number

(Pooja) - That's a good suggestion

(Edson) - Then change the file name to the EIP and then the EIP number

## 6.3. Postmortem format feedback 

(Pooja) - That makes sense; yeah we can do that. I've also shared the link of the previos post-mortem update that we shared in the previous meeting about the new glaciars. We are ready to share it with the AllCoreDevs; when Berlin is back, and we are talking about upgrades. That's all from the agenda that we can cover today. Anything else anybody would want to share? Okay, then I think we are good to go today; thank you everyone for joining the meeting today, I'll see you guys in two weeks on July 30th.


---

# 7. Annex

## 7.1. Attendees

- Alita Moore
- Edson Ayllon
- Pooja Ranjan
- Chloe Lewis
- William Schwab
- Edson Ayllon
- Matt

## 7.2. Next Call

Wednesday, July 30, 2020, 15:00 UTC.
