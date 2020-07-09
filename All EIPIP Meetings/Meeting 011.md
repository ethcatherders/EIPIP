# EIPIP Meeting 11 Notes
### Meeting Date/Time: Wednesday 1 July 2020 at 15:00 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/21)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=wZnsVp0aqBk)
### Moderator: James Hancock
### Notes: Jim Bennett

## Summary


## Actions Required:

Action Item | Description
-|-
 **11.1**        | Introduce EIP 2046 in a future AllCoreDevs call to be considered as an EFI.
**11.2**        | Discuss an emergency communications checklist on the next EIPIP call.
**11.3**        | Pooja to add Jaye Harill to the comms group in the Cat Herders
**11.4**        | Follow up with lightclient on his new validator and the rules.
**11.5**        | Read [this link](https://www.rfc-editor.org/about/independent/#:~:text=To%20post%20an%20Internet%2DDraft,%40rfc%2Deditor.org.) about independent submissions as part of the RFC before the next meeting.
**11.6**       | James to write the precompile discussion item into a PR.
**11.7**       | James to work on doing a document or a PR for the statuses to EIP 1
**11.8**       | Investigate the Cat Herders repo to use the project board for tracking the EIPIP agenda items.
**11.9**       | Figure out who has access to give Edson write access to the Cat Herders repo for the EIPIP project board.



**James Hancock**
Let's start. I'm James Hancock. This is EIPIP meeting 11, with the [agenda on the Cat Herders GitHub.](https://github.com/ethereum-cat-herders/EIPIP/issues/21) We are small today, so we're going to review and go over stuff and perhaps have a short meeting. But thank you all who came. If there's something particular you all want to go over, since we're small enough, I think we can be flexible about what to talk about first, if there's anything that comes to mind.

## 7. Using the Projects feature of Github to organize talking points for future EIPIP meetings.

**Pooja Ranjan**
So yeah, we can start with the idea of the project board. That is something new and interesting that we might need brainstorming over there. So just introduce why and how you thought of it and where you see this going.

**James Hancock**
Okay. You want to talk about your thoughts on this?

**Edson Ayllon**
Yeah, so I was watching you use it for EFI. And it looks like Trello. Sometimes, there's things on the agenda, which we don't get to. As more and more items are added to the agenda, I think it'll add bloat to future agendas, and we might lose items. So I think it's a good way to organize future talking points that we table to future meetings. Or sometimes they have agenda items that - say we want to focus on decision making, but we're also introducing stuff around on-boarding. We still have ideas that we want to keep, but not necessarily address at this moment. And a way to organize them could be using the project's feature and GitHub. So it's more of a way to organize the topics from these meetings.

**Pooja Ranjan**
Yeah, I kind of like the idea, too. Sometimes back, we have used it for creating the post-mortem for constant in poll and the Cat Herders itself. I'm gonna share the [link in the chat](https://github.com/orgs/ethereum-cat-herders/projects/1) here. So yeah, this is a good way to keep track of whatever agenda that we are trying to discuss here, and of any decisions we make, and how we are going to implement that. It would be a good way to keep track of it.

**James Hancock**
Yeah, this has the Cat Herders EIP repo use project boards before? Has it set up for them?

**Pooja Ranjan**
Yeah, when we look into the EIPIP repo, there is a section below project which is empty. At this point of time, I'm going to share the link here again. So there we can kind of sort tasks, plan project, automate workflow and everything is there. So we might have to take what we want to put where, or how we would want to address this.

**James Hancock**
Great. I'd love to see us move forward on this, or at least investigate where to get integrated and such.

**Pooja Ranjan**
So I think up 'til now, how we have been managing is we had this [initial document](https://docs.google.com/document/d/1KzEMD21Joqn7IWk4WnocwraRuo66y7r2w8R9Wml4BN0/edit) of EIPIP where we gathered some idea how we are going to do that. And the extensive report that came up after the EIPIP survey. So that was another reference point. And now we have to collect the main ideas from there and add them as tasks. And then we can keep measuring the progress. We need to keep track of the progress. And if it is closed, we can certainly reach it out to everybody in community as well as the CoreDevs to let them know what the things are.

**James Hancock**
I actually have started using the GitHub project board for managing the hard fork coordination stuff. I have one that I've thought about just making public, but I wanted to make sure it works well before I did that, just to keep track of the stuff that I'm doing. And something that's nice using the GitHub project board is you can tie issues, you can connect an issue to a tile or whatever you call them.

**Pooja Ranjan**
Right.

**James Hancock**
And so you can have an easy way to get to more information and discussion about individual things that's really handy. I'm excited about the possibility there.

**Pooja Ranjan**
Yeah.

**James Hancock**
Let's just go backwards, because Pooja, you copied a [comment from Gitter about separation of the EIP and hard fork coordination,](https://gitter.im/ethereum-cat-herders/community) and I'll just read it out here.

I am and this is from [Jochem Brouwer.](https://github.com/jochem-brouwer)

"I am super concerned that in hard-fork meta's Drafted EIPs get accepted (see the BLS EIP). I am also concerned why it is not a requirement that accepted hard fork EIPs have state test PRs in the ethereum/tests repository. What are the thoughts of this group based upon my concerns?"

The definition of what is accepted is changing. If we go over the new statuses that are being proposed, Accepted isn't even in there. And the reason is that the Accepted status will be part of the network upgrade process. And that will be done separately. So a little bit of high-level where we are currently with that is we have EIPs go through EFI. And then through EFI, they go through implementation, and then they go through the stage of going on a testnet like a YOLO testnet for client and client integration. And then after that is the state test stage. So we're at the point of defining where and how state test requirements for EIPs fits in the pipeline for network upgrades. And so it's a good concern and something that we're actively thinking about. It's actually been easier to process this since we've started separating the EIP process and the hard fork coordination process, because we can be stricter on things like this exactly and have a better process for each one. So that, I've been personally excited about, and I'd like to move forward with getting the new statuses added to EIP 1. Did you guys talk about that last week about having the statuses be moved? Or being merged early, being the first thing that gets merged to EIP 1?

**Pooja Ranjan**
No, not really. That was skipped in your absence, because it's better if the hard fork coordinator should be present. In the same context, I have a question here. It's just for my general understanding. When you mentioned that an EIP has to be EFI and then goes for implementation and then goes for Acceptance in the upgrade meta meta. So, my question is in regards to EIP 2046 and 2565. I understand that 2565 recently has entered into EFI and that we are considering in Berlin dashboard for the next upgrade. Although it is not very much confirmed that it is going or not going depending upon how the progress goes ahead. So for EIP 2046, where do we see that? Is it under EFI or considered for EFI, because I remember some discussion considering it for the Berlin upgrade, but I'm not sure what is the state of it or which state it is in right now.

**James Hancock**
Which one is 2015 again?

**Pooja Ranjan**
It is reduced gas costs for static calls. I know there is some discussion going on.

**James Hancock**
that's what I was thinking. So the update on that is, it's in the same - there hasn't been a lot of work moving that forward. And there's been a lot of other things happening in the CoreDevs, so it's understandable. But the status should be an EFI. And it's also still possible to get in Berlin because the reason EIPs get into hard forks is because they're ready to go in when a hard fork happens, or when a network upgrade happens. And so as that one is ready, then it can be moved. There are is still some outstanding stuff to figure out what's okay. And it'll go on YOLO before I think any of that is even decided.

**Pooja Ranjan**
Ok.

**James Hancock**
There are some things that need to be tested before we could even say we should think about it going in Berlin first. And it's easier to test those having them on YOLO, because then we can test them between different clients. So that's why it's a little bit in a weird place compared to other EIPs. Some EIPs, it's pretty straightforward if or how to do it. And then we kind of move forward on implementations. This one, because it's touching gas costs, it involves repricing gas things which then means we need to make sure that all contracts are still safe on the network. And that's just something someone has to go through, which that step is easier if we have it on YOLO by verifying the effect of the gas costs on all existing contracts is easier having it been merged into YOLO. So that's like an outstanding thing. I don't know if that exactly answers your question.

**Pooja Ranjan**
Yeah, but another question that is linked with this. So in our previous AllCoreDevs meeting, there was this discussion that EIP 2565 is not formally EFI. So does this also need to be formally introduced as EFI in one of the future AllCoreDev meetings?

**James Hancock**
The Merkle Tree Generalized Index. Well, it is a ERC

**Pooja Ranjan**
Oh, I'm sorry, I'm referring to EIP 2046.

**James Hancock**
2046.

**Pooja Ranjan**
I'm going to [share the link.](https://eips.ethereum.org/EIPS/eip-2046)

**James Hancock**
Reduced gas cost for static calls made to precompiles. So is it that it hasn't been added to EFI yet, or that it needs to be?

**Pooja Ranjan**
It hasn't been yet, as far as I remember.

**James Hancock**
And it hasn't been discussed, or it just hasn't been added to the document?

**Pooja Ranjan**
It has been discussed as an EIP but never as an EFI.

**James Hancock**
Yeah, so it still needs to do that.

**Pooja Ranjan**
Okay.

**James Hancock**
It's functionally there already, but it's important that in a call, we bring it up andr motion that it gets into EFI, as that's the the arbiter of what goes on the list goes through the calls. And it's important that we maintain that.

**Pooja Ranjan**
Yeah, maybe in one of the future AllCoreDev calls we will introduce it to be considered an EFI.

**James Hancock**
Yep.

**Pooja Ranjan**
Thank you. That clarifies.

**James Hancock**
And because we've talked about it before, it is possible that it could be made EFI that time. If it was the first time bringing it up, then it's really unusual for something to be added to EFI the first meeting it's discussed.

**Pooja Ranjan**
Got it.

**James Hancock**
Other questions on EFI or stuff like that from people while we're here and free to talk about it?

**Chloethedev.eth**
No questions from me.

**Jaye Harrill**
I don't have questions related to this, but when there's time in this meeting, I'm still sort of new in understanding the process of all this. I'm trying to understand where the process is to bring up certain EIPs into these discussions.

**James Hancock**
The best way is to add a comment on the [EIP meeting agenda.](https://github.com/ethereum-cat-herders/EIPIP/issues/21)

**Jaye Harrill**
Okay, so then it's just added to the next meeting.

**James Hancock**
Yeah. And then it's just added.

**Jaye Harrill**
Got it. Okay. Simple question. Thank you.

**Pooja Ranjan**
Not necessarily in the next meeting. If you do it before the meeting, we could include it in the same meeting itself.

**Jaye Harrill**
Makes sense. Obviously, there's only so much you can fit into a meeting and time. Yeah. This is not a pressing thing. It's just something I was just wondering.

**James Hancock**
Great. It's been nice having your comments on the EIPIP channel. So thank you for joining.

**Jaye Harrill**
Well, when there's suddenly an effort for Ethereum state regenesis, my interest starts to peak. So yeah.

**James Hancock**
It's good that we have you.

**Jaye Harrill**
I call it immutability, but people can call it whatever they want. Yep.

**Pooja Ranjan**
More comments on some other agenda items.

**James Hancock**
Yeah, but I wanted to address [lightclient's comments.](https://github.com/ethereum-cat-herders/EIPIP/issues/21#issuecomment-651918606).

So he mentions:

2. Github allows a special type of contributor with 'triage permissions,' meaning that they don't have write access to the repository, but can label issues and PRs. I think this could be a good on-ramp for contributors to become editors and would minimize the time editors need to click through PRs to see what their status is.

This is great. This would be a great thing to do. I 100% support that. I would say Hudson would agree. I'm not very GitHub literate, to be totally honest. This is a matter of actually knowing how to do it, and having someone who knows how to do it, do it, so I would very much appreciate help on this.

3. It would be good to agree on a specific naming convention for EIPs, since official documents use several different formats.  

This is correct. And it should be updated on EIP 1.

**Jaye Harrill**
If you're looking at naming conventions, is there someone who has a technical writing background involved?

**Edson Ayllon**
At least for different standards, they use letters and then the numbers, no space, or they use letters and the hyphen numbers, or RFC also uses letters, space, and then numbers. So all three of those that they listed are actually fine. It's a matter of just choosing one.

**Jaye Harrill**
That makes sense.

**Pooja Ranjan**
So I remember an incident when I submitted a PR for a specific EIP, which was already existing. And then one of the editors edited my EIP number. I forgot to mention the hyphen between, say, for example, it's EIP 1, so I chose the third one: EIP-space-1, and he corrected it mentioning that no, it needs to be EIP-hyphen-1. So if we consider that as a baseline, I think that needs to be mentioned in EIP 1, and that can be followed.

**Jaye Harrill**
Yeah, I had another question. I'm just looking at the Constantinople post mortem action items. Emergency Comms Team and also Risk Evaluation Rubric were two things that popped up. The thing about the comms team - is there any progress on that? Because I feel like there's a few people in this space would be perfect for that. And certainly, we have some experience with doing emergency comms. And then the risk evaluation, this little note is small, and what is involved in creating that is very, very large. I think it would be better to put that up for opinion in the Eth security chat.

**James Hancock**
For the naming conventions?

**Jaye Harrill**
"Create a rubric for risk evaluation."

**James Hancock**
Oh, yes. Yes.

**Jaye Harrill**
Yes. I don't know that that's - you can have something to base things off of, but that is not going to necessarily cover all your bases. And I know don't know that there's necessarily a way to cover all your bases, but there are certainly things that are doable.

**James Hancock**
Yeah, that would be great to get the list of things. I don't know if there's any progress on a rubric for comms. It ends up being Hudson and I waking up whenever something happens and finding people that need to talk about it. I'm pinging him and pinging everyone until things are resolved.

**Jaye Harrill**
Is there a playbook as to what the checks are to do when that happens, all the checks that need to be need to be done?

**James Hancock**
Not that I'm aware of.

**Pooja Ranjan**
So for that, we have created this [emergency comm process document](https://github.com/ethereum-cat-herders/PM/blob/63d6c017c67ac2188b44f8d9f5293f563a1745cf/Constantinople%20Postmortem%20Report/EmergencyCommTemplate.md), sometimes back during the Constantinople post mortem only. So it suggests that we should be having a list of key audiences, those are going to be, you know, emergency comms members. And we are trying to create this list. Generally, we use this kind of list at the time of upgrade or hard fork to communicate with our key stakeholders to let them know what's going on if something urgent comes up. So that's it, and the other thing was we came up with a list of [preferred channels of communication](https://github.com/ethereum-cat-herders/PM/blob/63d6c017c67ac2188b44f8d9f5293f563a1745cf/Constantinople%20Postmortem%20Report/EmergencyCommTemplate.md#preferred--appropriate-channels-of-communication), because it's important that we should be reaching people, more people and as quickly as possible. So these are the preferred, appropriate channels that we suggested we should be using.

**Jaye Harrill**
That make sense. I'm just quickly looking at this. Certainly understanding the list of who to contact, this is public, so I know that it would have to be a trusted group of people to do that. But I feel like if there's a little bit more direction in this document that that team could be formed. I don't know. It's honestly more of an operations role with someone who can understand how to form something that doesn't provoke worry, but provokes calm, immediate action of the right things rather than a reactionary thing. And so I don't think that's very hard. There's some talented comms people in the space.

**Pooja Ranjan**
Yeah, so if you could put me in touch with them, or maybe if you feel like you could be helpful to add more to this document, but as you mentioned, as information can be sensitive, and we would want to keep it in a closed group, we could work together on that.

**Jaye Harrill**
Yeah, I'd be happy to try and find some people. I'd be happy to be on the team, too. I'm just - there is a process that already exists, and there is already a list of people to contact, so I don't want to change that. I think it's more or less here. All it's really needed is the people to be able to execute on the thing when it's needed and to have the professionalism to work together and say the right things. And I think that could be honestly coordinated through a little Telegram chat that's limited in how many people are in it.

**Pooja Ranjan**
So the executors here are basically the Cat Herders itself. We reach out to the group of people in the Cat Herders, and we reach out to these people. And James is the hard fork coordinator, so we work together. And some people are reached by James, and that's how we have been managing it so far. But yeah, happy to have you on board, too.

**Jaye Harrill**
That makes sense. Emergency comms is something that I have some experience in, so I'd be happy to help, but I think I'd still want to hang back a little bit as I slowly unpack and understand more of the processes. I'm not ready to just jump in and start saying "here are solutions, because that wouldn't be good of me. There's a lot of stuff that has already been built out.

**James Hancock**
And Hudson would be a lot better person to ask about this, because he has more experience doing these kinds of things. But a checklist I think we appreciated as something that we could we could go through, and in the case Hudson isn't available, it would give people the opportunity to still execute on it.

**Jaye Harrill**
Yeah, that'd be amazing. I think a checklist and people to execute on it would be good, I think it wouldn't be a very hard thing to organize. Maybe it's a thing to talk about on the next EIPIP call it with more detail. I'm taking up too much time here. But I just wanted to bring that up. That is that is definitely an area that I feel like I can help right away.

**James Hancock**
Cool.

**Chloethedev.eth**
I think personally, I agree. I feel like the processes that are there work for when things are going well, but even right now with Hudson Jameson being away, I'm sure, James, you are kind of left to do a lot of things that maybe you aren't used to doing. So having processes where those of us that aren't used to helping out might be able to fill in the spots and help out when maybe if you both were away, we'd still be able to get things done.

**James Hancock**
It's been a little eye opening me to me. If I hadn't joined, and Hudson was gone,it'd be really hard right now.

**Chloethedev.eth**
Yeah, exactly.

**Jaye Harrill**
Yeah, I feel like that's an area that could be better patched. But I don't know that I feel confident in leading this as a task, but I certainly feel confident in providing feedback and also help coordinate a team together when we're ready and work on when shit goes down, but at the moment, I just don't have enough of the pieces, and I think the the biggest need is to prioritize it, have a checklist, go through the checklist, and get a list of contacts. If those things are in place, then I know for a fact I can go and organize a group.

**Pooja Ranjan**
There is a group already, the comms group, which is within the Cat Herders itself. Maybe after this meeting, I will be talking to you and adding you to the group.

**Jaye Harrill**
Yeah, I think there's a lot of communication stuff that, you know, it's not always easy and getting people to pay attention is hard.

**Pooja Ranjan**
Agreed.

**Edson Ayllon**
Should we move on to the next topic?

**James Hancock**
Yep. From [lighthouse:](https://github.com/ethereum-cat-herders/EIPIP/issues/21#issuecomment-651918606)

"What are people's thoughts on increasing the strictness of the eip_validator? It seems like the quality of EIPs could be improved quite a bit if more checks occurred before merging. I've started work on a new EIP validator. I plan to make it much stricter than the existing validator and more robust."

And I have been asking for this for a long time. I don't want to jump ahead of everybody, but I'm very excited. The EIP validator is been one of the limiting factors on doing upgrades to the EIP process and the EIP repo. Because any change that affects the validator needs to be made and no one's been able to figure out -  we haven't had anyone to make those changes. So yes, please. Anyone else?

**Chloethedev.eth**
I'd love to hear more, but I'm for it, obviously, from what you're explaining so far. I wouldn't say that I understand exactly the differences about upgrades specifically.

**James Hancock**
Yeah, it'd be good to know more about what he asked me specifically, but we haven't had any upgrades do a validator. So even just making the validator, where someone can know how to upgrade it.

**Chloethedev.eth**
That sounds great in general, for sure.

**James Hancock**
Yeah. There's a bunch of things. There's a bunch of stuff - rules that I'd like to make more strict. So we should bring that up on our next meeting.

**Pooja Ranjan**
Yeah, he mentioned that maybe next meeting, he would be able to join some, just because he wasn't able to make a test meeting, we just threw the items on the agenda.

**James Hancock**
Yep.

Then the last one:

"How can we funnel people working on similar EIPs together? For example, EIP-2549 is related to eth1.x and eth2 witnesses. Those groups may not be at the stage where they are ready to pursue and EIP, but it seems like this will end up being superseded by the eventual EIP from those groups. Funneling independent contributors to existing efforts is a standard practice for RFC contributions."

It would be nice if this was a responsibility to the EIP editors. But adding more responsibility to the EIP editors isn't really a good thing to do until we figure out more about what the responsibility of the EIP editors - like to have more decisions around that. Andso then it's left to people in the community pointing out, or me or Hudson or people being aware enough that when we see things say, "hey, these things should work together." Does anybody else have thoughts on this?

**Edson Ayllon**
I think he is mentioning just working groups. So if we have more people, we can definitely form working groups. People can monitor differences of EIPs.

**James Hancock**
When he lists a independent submissions as part of the RFC, which is something I'm going to read afterwards, but [I'll put this in the chat.](https://www.rfc-editor.org/about/independent/#:~:text=To%20post%20an%20Internet%2DDraft,%40rfc%2Deditor.org.) I think it would be good for us to read about it and bring it up in the next meeting. Unless someone else has comments that they'd like to give.

**Pooja Ranjan**
Yeah, this is a good document. I want to read it and maybe discuss it in the next meeting.

**Edson Ayllon**
So maybe we should read up before or table this to a future meeting.

**James Hancock**
Yeah. I would suggest that.

I'm deciding if we should just read through the agenda or have Pooja present the post mortem that we worked on, and I'm leaning towards having Pooja present the post mortem, and then we can have final thoughts and just close, unless anyone has other ideas.

**Pooja Ranjan**
So if we have to look into the post mortem, we just gave a look to the poll that we did earlier that was in a form of project. But in one of the previous EIPIP meetings, we decided that this kind of information should be made public in the form of an EIP. We can save it as an informational EIP, which is way easier accessible for people rather than finding it in some particular GitHub repository in some projects section. So this is a draft that we have created for the previous Muir Glacier upgrade, and we have tried to provide as much information as possible starting from the upgrade summary section. Like what date, time, block number, and who owns that particular block.  The details from there included a list of the EIPs that were included, but for Muir Glacier, it was just the only one for pushing up the difficulty bomb. So we use that. And this is the sequence of events that took place, the decision making date so that people can go and refer. The thought is to make everything accessible for the community later on to read. And if we come up with some good practices that we would want to continue in the future, some corrective actions like the rubric that we discussed, about how we can prevent anything mess happening or what was the issues we faced and what about that possible suggestions to that...

**James Hancock**
Are you in a position you could share The screen with the document that we're talking about?

**Pooja Ranjan**
I think I can do that. Is it visible now?

**James Hancock**
Yeah, I can see it. Okay.

**Pooja Ranjan**
I also shared the [link in the chat](https://docs.google.com/document/d/1onC1rUqXTI3MNYJRiwhgLS91OaYrVgAlZb0Ri3i4hRE/edit) for people to refer. So we have not submitted it. It's just a draft, and it is staying with us. I wanted to discuss this with you guys to collect some feedback if anything is missing. The two questions I have in mind, I'll just mention it so that if you're giving it a look, or maybe think about it, the discussion section here, what we did is we refer to the eth-magician post that James created for Muir Glaicer upgrade. We did not create any specific eth-magician post to just list the Muir Glacier, because I'm not sure if there is much more discussion needed or if we can just combine both of them. So that was one. And the other thing was at the end of this document, we have also listed the resources. This is not a typical format of an EIP. Do we need to have it? If it is fine to keep it, because I think I have mentioned all the links here already, then we will keep it. Otherwise, we might want to remove it. And yes, please feel free to share your thoughts about this. There's one more thing. We have [this template](https://docs.google.com/document/d/1onC1rUqXTI3MNYJRiwhgLS91OaYrVgAlZb0Ri3i4hRE/edit). This is the general template for future post mortem upgrades. This would also be posted in the form of an informational EIP for people to refer and when we are creating, we'll keep this in mind. I will share the link of this document as well. So feel free to add any comment. Anyone have any questions?

**Chloethedev.eth**
On the second point you made about the resources, just on specifically accessibility. As someone who does have a hard time sometimes navigating through some of these EIPs, I do think it's helpful to have the resources for future post mortems, if that can become something that was normal, I think it could be helpful for people that aren't as used to know what's going on in the community. Then I go kind of figure out more information there. That can also be in the in the blog post as well, potentially. So there's that, too.

**Pooja Ranjan**
Yeah, sure.

**James Hancock**
It would be good to add the blog post to the resources.

**Pooja Ranjan**
Okay. So I have added the blog post here somewhere.  Okay, this was published by the Cat Herders. Okay. I think I missed one published by the Ethereum Foundation, I may have to add that blog post as well. So we try to provide as many links as possible to get into the real conversation and feel like we have not made up anything. Everything is coming up from the discussion. So yeah, I will add those at the bottom as well.

**Chloethedev.eth**
Yeah, for sure. I just know for me, sometimes, the EIPS can get very verbose and very long. And sometimes just scrolling to the bottom and seeing a few very important resources can be helpful. And so for other people that might get into other more technical post mortems, it might just be helpful to have those few key resources at the bottom, as well as all those lists that I'm sure people that are more into those post mortems will go through thoroughly.

**Pooja Ranjan**
Right. So one new thing that we are trying to do here is putting the suggested corrective action in the form of problem and suggestions. One of the comments that was received by one of the client developers was "The testing window planned for this particular upgrade was too short." Maybe because we did Istanbul in December and January it was there. So yeah, certainly, we did not have testing window, and maybe because of that, some miscalculation. The Ropsten had to be delayed for a very, very long time. It came up after 10 days or 11 days after the mainnet, and we should avoid mainnet to upgrade before testnet. So does anybody have any comment on this particular format, the problem in suggestion, or it looks fine, or can we put it in some other form?

**unknown**
I think it looks fine.

**James Hancock**
Great. It's been it's been fun. The last couple of weeks, Pooja and I have been  meeting and writing this out. It's long overdue. So I appreciate the help on making this happen. I think it's important to record this and so we can learn from it.

**Pooja Ranjan**
I'm going to stop sharing now, and we can move on to the next item unless anybody has any more question on it.

**James Hancock**
Anyone have thoughts on the the 2, the TV, or where to put the discussion link? Or what that should be like? The "discussion to" usually goes to a post on the EIP, but in this case, thoughts on what's a good place to put it or if we should have one.

**Pooja Ranjan**
I mean, this was the general format. That's why we use the existing one. But if somebody feels strongly about having a need of a separate discussion pointer, we can create one.

**James Hancock**
Yeah, the other option would be when we create the post mortem, we'd make a post on the Eth Magicians and then link the post mortem into the the post for people to discuss. That's another option. Like have the post mortem be its own topic on Eth Magicians.

**Pooja Ranjan**
Yeah, we can do that, too. So I've also shared the link of the upgrade post mortem template, the Word document, if anybody comes up with any thought that they would like to share later on, feel free to do that.

**James Hancock**
We have 10 more minutes or so to discuss. Anything comes to top of mind?

**Pooja Ranjan**
There was a lot of To Dos, I think.  Do we want to discuss some of those or maybe we can plan?

**James Hancock**
The EIPS To Doo is a pretty big document.

**Pooja Ranjan**
Okay, then we might want to go through the [review action items.](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20010.md) If there's anything pending, we could look into that. So going by the notes of previous meetings, it looks like a bunch of decisions made. James, please go ahead.

**James Hancock**
Yeah.
Decision Item | Description
-|-
**10.1** | EIP number registry may not be a major issue. Discussion can be dropped.
**10.2** | Continue the discussion on adding a mandatory terminology section for EIPs.
**10.3** | Future meetings, discuss onboarding EIP editors.

We talked about that a little bit today. You can have permissions for triage and things which we can have be more open for individuals.

**10.4** | Have use of labels for PRs to EIPs.
**10.5** | Waiting on James to complete the precompile discussion item.

What does that mean exactly?

**Edson Ayllon**
I think that's the precompile - how new precompiles are made.

**James Hancock**
Yeah, I just need to write that and make that into a PR so we can talk about it better.

So we have the new proposed status flow with some idea about the definitions. What are thoughts on on moving forward with that as a first change to EIP 1?

**Edson Ayllon**
So I think that's good. One thing I brought up in the previous meeting was feedback from Artem was that there's less scrutiny moving from one status to another. And that could be because we haven't defined how to move from one status to the other. So we can probably include it with the statuses. We can define how to progress within the statuses or specify that. Make sense?

**James Hancock**
Yeah.

45:12
Yeah, that would be good to add. I added more arrows that are stricter, but we can describe what can move to where and how. That would be a good addition to clarity.

**Edson Ayllon**
Yeah, how is more specifically how you move from one place to the other. Also, we should start defining statuses for the hard fork coordination. And we should also include how to move from one status to the other for that as well, kind of mirroring the EIPs.

**James Hancock**
Yeah, do we want separate statuses for the hard fork coordination process? I was thinking more like steps. So having steps in a flowchart or steps in the - I haven't settled on the best way of tracking where things are in the process.

**Edson Ayllon**
So I was thinking just like project management steps. So there would be, or this is just my initial thoughts because they get feedback, but Eligible for Inclusion is For Consideration, then Implementation, then Testing, then Final Decision, then Deployment. And then through any of these steps where you go from one to the other, there's always the chance to motion to Rejection. So say you go to Test then you can go to Rejection, you know, in implementation, you find something that just the EIP makes something impossible or just messes something up deeply may be rejected before it even goes to testing. But that's just my initial thought.

**James Hancock**
I like having the flow that way. Part of the what we've run into historically is the definition of Accepted is kind of clear in the EIP 1. But the community understanding and even sometimes the core developer understanding of what that means is totally different. So having you go through the process, and at any point, it can be rejected is a good way of kind of managing those expectations, and we should show that visually, when we're defining the process. I like that quite a bit. I'll work on doing a document or a PR for the statuses to EIP 1. You're right that it's time to start more defining the network upgrade process. I would just feel more comfortable if we had some more resolution on the standardization process before I start shifting mental gears into that. That's something I can work on.

**Edson Ayllon**
We could just start opening up a PR to EIP 1. There's nothing stopping us from making future PRs. Yep.

**James Hancock**
Yeah, I've been hesitant to dump into the network process. I'd just like to get this standardization process at least more moving forward before I start diverting efforts. But I'm open to feedback from the group on what's the best way to proceed there.

**Pooja Ranjan**
One of the action items mentioned, or not an action item - it's just a part of the decision is like that there should be a particular place to collect all these kind of definitions that we are planning. There is already a mandatory terminology section for EIP. So we are discussing for putting these statuses as described in EIP. It is something that we should consider for EIPs in general as well. If something new is coming up, we should add this section in an EIP. I'm talking about an EIP template that we create.

**Edson Ayllon**
Yeah, I think we mentioned this in the previous meeting. I had suggested that different standard organizations, they have a section for terminology. It might be good if we simplify to something like, say, definitions as having it mandatory. There may be EIPs that don't really introduce new terms. And then having global terms that are required for each EIP, I don't think is necessary. But some  EIPs may introduce new terminology that would facilitate clarifying to the reader. It brings some value having a definition section.

**James Hancock**
Yeah, I would agree.

**Pooja Ranjan**
I'm not too sure how much value it would add if it is not something that is going to be common. And in most of the EIPs, we can probably go ahead and explain that term in one of the summary sections or somewhere else in the EIP itself. But adding this as a mandatory section for every EIP that is something I'm not sure about, but it doesn't hurt to have something additional as well.

**Edson Ayllon**
So I think it's good as an optional section. I don't think that it needs to be mandatory for every single EIP.

**James Hancock**
Yeah, it would be good to have one in some of them going to EIP 1. We can have definitions that people can use, like the definition of a network upgrade.

**Pooja Ranjan**
Right, that is needed for EIP-1. I understand this point. This section is mandatory for EIP-1. But again, EIP-1 is not any general EIP. It's a kind of documentation that provides a guideline. So for that, having this section, it makes a lot of sense. But making it mandatory, I was not sure. But if it is optional, yeah, perfectly fine.

**James Hancock**
When I've written EIPs, I tried to do this or be mindful of if I'm using terms defining them. So having that be as a best practice, is something else we should consider. Because we have stuff that's required. And then we're starting to also list things as best practices. And that, definitely, we should add to the list of best practices. Or consider doing it. I don't want to decide. I'm getting ahead of myself. We're at the top of the hour. So unless there's some final thoughts, I think it's time to wrap up.

**Pooja Ranjan**
Can we just quickly summarize for the note takers, what are the decision makers and action items.

**James Hancock**
Decision and action items:

1. Look at the Cat Herders to investigate the project board for the EIP repo. I mean the EIP ip repo
2. Follow up with lightclient on his new validator and the rules.
3. James to draft PR for new statuses

**Pooja Ranjan**
Did we decide on any timeline to submit this PR or is it final or we would want to wait? And what do you think about it? The PR for the post mortem update I'm talking about?

**James Hancock**
I don't think we need to decide a timeline. We should meet again and keep talking about it. Then bring it up on the next call.

**Pooja Ranjan**
Okay.

**James Hancock**
And then the next step on that is to  present it on the AllCoreDevs call.

**Pooja Ranjan**
Oh, yeah, of course. I'm not sure for AllCoreDevs, should it be submitted as a PR in the EIP repository or it can be shared just like that?

**James Hancock**
Either. Yeah. Are there outstanding action items that I'm forgetting?

**Pooja Ranjan**
Yeah, and we would like to bring some of the agendas here repeated in the next meeting. We would like to continue the discussion on the rest of the items.

**James Hancock**
Yeah, it'd be great if we could get the agenda put into the project board, or the items in the agenda fleshed out into the project board and use that next meeting as possible.

**Pooja Ranjan**
Yeah. Edson, I would be happy to work with you if you have anything in mind. Or if you would want to give it a stab. If you do that, you can create a PR and we can do that. Or we can discuss it offline and try to create it.

**Edson Ayllon**
Yeah, I tried adding a property for it. I don't have write access to the Cat Herders repo. So this is what's limiting me with that.

**Pooja Ranjan**
And I'm not sure who has the access to give you that access at this point.

**James Hancock**
Yeah, that's that's the day action item. Figure out who has the access.

**Pooja Ranjan**
Yeah, I'll work on it. I will look into it like who has the access. Maybe Hudson or somebody and should have, but I'm not sure of that. But yes, I would be happy to discuss and see if we can work it out. I'm not sure. If you have any idea, James, does it work out with the help of pull requests?

**James Hancock**
It doesn't take your pull requests to add a project board. You need to have write permission. You need a specific kind of write permissions to the to the EIPIP repository. And then you can add them under different permissions.

**Pooja Ranjan**
Okay, we'll look into that.

**James Hancock**
Thank you all for joining. It was a nice kind of relaxed conversation today. Are we good? I appreciate the comments and in all of the value you all bring, and please continue.


# Attendees

* Chloethedev.eth
* Edson Ayllon
* Hudson Jameson
* James Hancock (host)
* Jaye Harrill
* Pooja Ranjan



# Date for Next Meeting: 15 July 2020, at 1400 UTC.
