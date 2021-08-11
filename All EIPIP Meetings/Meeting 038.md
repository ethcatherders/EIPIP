# EIPIP Meeting 38 Notes
### Meeting Date/Time: Wednesday, July 28, 2021, at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/79)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=0zHXZhxs7IA)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION ITEMS

**ACTION 38.1**:  Pooja will  consider a feature update to the present eip bot as a task list and ask Alita to provide her feedback on ETA for completion and if she requires any additional people.


## AGENDA

## 1. Evolving EIP process

**Pooja Ranjan**: Welcome to EIPIP meeting 38. Agenda shared in the chat. The first item on the agenda is evolving the eip process, I have added it  considering we discussed it in bits and pieces in past meetings. So now we have a consensus specification. I think some work is being put in by the quilt team and with respect to much do we see any changes in the core eap process.In general so just wanted to bring it up. Maybe Macah if you would like to add some  thought on how we can improve it.

**Micah Zoltu**: Really quick before we get started. If Tim has to leave early. Is there anything we want to move to the front of the list to make sure we get his feedback on.

### Core EIP - changes wrt to the [Consensus Specification](https://github.com/ethereum/eth1.0-specs#consensus-specification-work-in-progress) & the Merge 

**Pooja Ranjan**: In my opinion yes first this item like core EIP processor will be changed so that is something we can use okay.

**Tim Beiko**: I guess maybe a way to make this very concrete. Do we think that the ETH1 spec will be ready for us to use it? As the merge spec says, Micah has an EIP out right now. Do we think yeah that's what  basically are we gonna start using the consensus spec after the  merge or do we think we can actually use that the specter merge and possibly move over Micah’s eip as part of that or you know alongside that yeah!

**Micah Zoltu**: If this was more of a normal fork. I might say yeah but I think because the merge is so complicated  where we also have this pretty mistake thing.I would say let's  plan to not worry about it. Okay and we'll see the speed at which we finish the spec and if it happens in the next couple months and we talk with Danny and we're able to interoperate with their spec then maybe it makes sense. I think because of how complicated the merger is going to be. It might just cause us more pain.

**Tim Beiko**:  Got it and one one option is also say we get to merge test nets with the eip. We can then almost backfill it into the spec right.So maybe it's not maybe it's not what we use to implement the merge but maybe it's kind of ready by the time the merge hits maintenance where there might be several months lag.

**Micah Zoltu**: Yeah that would be a pretty good outcome, I think for the spec.

**Pooja Ranjan**: All right so if I understand correctly we may be expecting some changes in the process in terms. We may not be going by the eip process in general but  not for the entire set of the proposal just for this pack part. We can manage it with the help of pull requests and the rest of the details can be added to the eip we have 3675.

**Micah Zoltu**:  Yeah and we should keep assuming 3675 is what we are going to use and share with the clients and iterate on over the next couple of months.

**Pooja Ranjan**:  Oh! That's great. All right, that's about core eip. I am iot sure if we have any more clarity at this point of time. Yeah if anyone would like to add anything otherwise we can move on to the interface one

### [Interface EIP]( https://github.com/ethereum-cat-herders/EIPIP/issues/7) 

**Pooja Rajan**: Okay similar to core EIP, I know there is some work which is even being put in for the interface EIP. We did discuss yesterday within the meeting that eip editors training meeting in general. How do we see interface eip in future. Right now I see quite a lot
eip which are in draft status and review we just have a handful of. I think seven or eight eips as finance so do we want to keep interface eips as it is or we do have to deprecate that in future.

**Micah Zoltu**:  I feel we can just keep them as they are and have the understanding that there will be no more RPC eips with that means.

**Pooja Rajan**:  Whatever is interacting and reviewed they do not need to move forward and we can just move them to withdrawn status or just leave it as it is. I don't know.

**Brent Allsop**: It would be nice to clean them up eventually.
 
**Micah Zoltu**: I assume the RPC eips are probably final at this point. I don't know where they are. 

**Brent Allsop**: There's a mix.

**Pooja Ranjan**:  : Okay,share the link in chat. Yeah that's what I am wondering if these proposals,if we are assuming that they are not supposed to move forward to any further
status let's move it to withdrawn and we will make a statement . We have other banners for
different proposals. We can have a banner for this particular category written here that these proposals are not supposed to move any further and we can be using the specs repository for any more interface eips that make sense.

**Tim Beiko**:  Yeah I think it does, I mean a lot of them . There's a bunch of weird ones. 

**Pooja Ranjan**: In that case I will create an issue to look for someone who can at least first create a banner that we are not moving the status of interface eips. We should be using the spec repository for any further eips in this category and then eventually I will try to reach out to different authors and create pull requests to move these proposals into withdrawn status.

**Micah Zoltu**: So there are a few interface eips that are not actually json RPC, so I think the category still needs to stay until we find a home for the rest of them.

**Tim Beiko**:  Yeah there is a bunch of weird things like renaming up codes. I don't  know what wallet permission system is?

**Micah Zoltu**: So, there's a subset. It's json rpc stuff that can be removed or marked as abandoned or withdrawn or stagnant or whatever but there will still be an interface category and there will still be eips in it which means we can't just blanket put a banner on. I don't think or if we need to make sure it's very clear that the banner only applies to json rpc.

**Tim Beiko**: Yeah there's stuff like that you know the trace specification like there's a bunch of.
 I guess they are interface eips.

**Pooja Ranjan**: okay in that case it looks like first we need to separate the eips which are non-json rpc eips and then the withdrawn stage status could be applied for only those are json rpc specific eips and for the rest of it. We can just have a banner that no more json rpc eips  can be found here or unusable here that has to be used with the specs depository and for the rest of the interface eips. This is good to go. I am not very sure what I mean. I am particular. I am not sure that I would be able to differentiate all of them. Maybe I have to reach out to or if anyone here in the group knows so I can share a list and we can add it.

**Tim Beiko**: Pretty much anything that mentions like east underscore  in the title is jsonrpc. or if it says jstrpc in the title like if you  take care of those two classes of things that get rid of like 95%

**Pooja Ranjan**: Great I will first prepare that list and then will get reviewed with one of the editors and then will create an issue and work with help of the community to start working on this type of particular  category of eips.

### [Networking EIP](https://eips.ethereum.org/networking)

**Pooja Ranjan**: All right moving on to the networking eips so I talk to a few authors and have created respective pull requests to move these proposals into the right status. I think there are only a few left in the review status and draft 86 have created a good request today to move it to the last call. Other two Danny  responded by saying that it depends upon the get
the team and I know Micah also has said that. So I have left a note for Felix and am waiting for his response. The eip is in draft I am not sure. I left some  comments for Peter. We will wait for his response if not it can be superseded because we are moving ahead with
each 66. Does it make sense to move it with the superseded with 66.

**Micah**: No for two reasons, one I think we dropped superseded because it's too opinionated and  two I believe e66 actually depends on e65 and so technically let me verify that. I am pretty sure yeah e66 depend it requires  e65 requires e64. So technically we shouldn't even have moved 66 to the last call or to review because 65 and 64 are still draft. Those ones should be moved at least at the same time if not first.

**Lightclient**: Does 66 depend on 65?

**Pooja Ranjan**: Yeah they mention it in the proposal.

**Micah Zoltu**: Yep it's a hard requirement and

**Pooja Ranjan**:  Okay  so what I can do is like I can create a full request to move it to review status for 64 and 65 and maybe then ask the author to approve it. We have  already created requests  for 66 to move to the last call we have 14 days. We will try to sort this
issue within this period of time before moving it into the final status. That is about 1459. They know about the discovery by DNS. I think Felix would be the best person to comment on it. okay I will check with him one more time. All right I think this particular category seems to be in very good shape like this is under control. Proposals are mostly in the right or appropriate status. There are very few proposals in fact and it is manageable good to know that.

### ERCs - revisiting to access the need for process change

**Pooja Ranjan**: About the last category years erc a few months back we decided to leave 
as it is and revisit after a few months to see if this needs a process change. Just wanted to have a quick check with the group like do we still feel that the way it is moving is fine. We can just use the github labels to address erc's or the process that we discussed earlier. Should we try implementing it?

**Micah Zoltu**: I still would like to get rid of ercs out of the eip's repo.

**Pooja Ranjan**: I love your determination Micah. So you know earlier, we discussed that
We will be waiting for some more time to see how poor eips move ahead. If we are moving into the quarry completely it is out of the eip repository. Then we may not be moving erc's but as it looks like. We will still have four eips in the github repository as it is just a part of it is taken out of the github repository. So I think  the changes that we discussed earlier for erc's
makes sense. Especially in terms of taking their numbers and the process like having a separate repo and process to be followed similar to eip but managed separately.

**Micah Zoltu**: If we think that we will see a switch over to the f1 specs like the python specification within the next 12 months then I can probably be swayed to give up on getting erc's out because when that happens I will just stop paying attention to the eips repository. I think for me the issue is I am not confident that within the next 12 months. We will be off of the eip's repository. Does anyone have inside information that I am not privy to that would help convince me.

**Lighclient**: I mean we will have a spec written within the next 12 months and it's a matter of for people wanting to switch to it and I think they will but it's not given

**Micah Zoltu**: Where would one go to follow along with the progress of that

**Pooja**: The eth 1.0 specs repository. I think the link is there in the consensus specification I mentioned in this particular item.

**Micah Zoltu**: Oh is it just being written right there?

**Pooja Ranjan**: Okay in the meanwhile I am just wondering. I know now that we are having this meeting of eips and editors and training. So we are trying to cover more and more eips as well as erc's. I mean review at least. I don't know if we can add triaging permission to more of the reviewers with that help.

**Micah Zoltu**: We can't give triage permissions because  the ethereum organization is not
the latest version.

**Tim Beiko**: We don't pay for github enterprise and you need github enterprise for that I am sure.

**Pooja Rajan**: I am surprised because in the ethereum cat herders get help. It works. 

**Tim Beiko**: I tried and I asked her devops team. I don't know that's you can give triage
permission in any cat herders repo.

**Pooja Ranjan**:  That's right

**Tim Beiko**: I mean let me try .

**Micah Zoltu**: In  the ethereum organization?

**Pooja Ranjan**: No cat herder is out of ethereum organization but I am saying that I am also I mean like ethereum cat herder is also is not a paid version of github

**Tim Beiko**: Yeah Yeah. So which repo this is for the eth1 specs right.

**Pooja Ranjan**:  No it is for eip

**Tim Beiko**:  Oh okay let me try

**Micah**: So I think the issue here is there's a difference, there's multiple versions of github. There's github ,paid github, private and there's legacy github private and then there's github enterprise and there's legacy versions of github enterprise. I am guessing cat herders are on just the traditional public repo whereas the ethereum organization. I think it's like one of the older.

**Tim Beiko**: Oh well I think the thing is we are maybe not an enterprise but probably a paid plan. We are probably like in this weird mello.We are an organization but not an enterprise. Okay there's a team plan so I wouldn't be surprised if we were on the team plan. So we get the worst of both worlds.

**Micah**:  Yeah I think I don't think you guys are on the team plan because the team plan
is what a new thing. Right? I believe you guys are basically grandfather the ethereum organization is grandfathered on a plan that no longer exists like you cannot get this plan anymore yeah and I don't want to leave because leaving would change the pricing model
Significantly.

**Tim Beiko**:  I just checked on the eips repo. I don't even have access to see who's in admin and see the roles.

**Pooja Ranjan**: Okay notice then in that case Yeah I was just wondering because I found that lightline added to some full request that it is an erc and it was really easy to sort it out.
so I was wondering if I can also contribute or other people who are trying to understand the eip editing part maybe. Just because this is the primary thing. We can do it without too much effort but no worries. Okay so that sums up the evolving eip process.

##  2. [EIPs site rendering issue](https://discordapp.com/channels/595666850260713488/746566142700814426/869490362895454248) with linking to other EIP

**Pooja Ranjan**: Agenda item listed here on eip's site rendering issue. I think this was
discovered in the eip 3675. Michael also left some comments. I left the first comment because when I was trying to read out the file that was giving me a 404 error. So I suggested to move out the anchor part but it seems there was some rendering issue not sure if it has been solved or someone needs to look into it.

**Micah Zoltu**: I just made some changes recently. Have you checked since then?

**Pooja Ranjan**: Not today morning, I checked last night.

**Micah Zoltu**: I think he made some changes today to try to get the anchors working. So I am probably worth checking again.

**Pooja Rajan**: All right then it sounds good yeah. Because I was trying to understand like
why is it missing and when I am seeing why they're doing 404 ahead to me but that's all good.  I will look into it again.

##  3. EIP-bot

**Pooja Ranjan**:  The next item is eip bot. Alita mentioned in the comment that she may not be able to attend the meeting today. But she left some updates on work she has been putting in for eip bought a few issues. I have highlighted earlier was a proper representation of eip that eip dash whatever the number is I think that would be a good practice to let  people know that whenever we are referring to eip that is something that we need to do
and my assumption is it is fixed because for another pull request I got it in a better format. So we considered it done. I am not too sure about the next item if a user gets a specific message about why a pull request failed checks. Because if I look into the list of pull requests right now. Most of them are red cross that means they are failing the vote check at some point but  I am not sure if I am receiving a specific message about what has failed. I mean why it failed and how I can fix it to get the green check.

**Micah Zoltu**: So I think all eips will have a red check right now ?

**Pooja Ranjan**: Yes actually it is.

**Micah Zoltu**: Yeah I think it is as soon as it can get a green check it merges like that's how the merge works basically.

**Pooja Ranajan**: Oh so it's not possible to get a great change before that because I remember when this was the case for earlier bot.

**Micah Zoltu**: The current bot you cannot green check. The green check means your merge
basically, if you have passed the check mark. It will say like two of four or three or four or one of four or four or five something like that. In theory you can get something, Some information out of that or if you click on one and then scroll to the bottom of the pull request. You can see which checks are failing which ones are passing. If the failing check is travis ci
that means there's something the user probably needs to do. There's something wrong with the actual eip like it's got a spelling error or it's malformed something like that. If it's one of the other ones it's just the waiting for the waiting for approval basically.

**Pooja Ranjan**: That makes sense but it it is not able to pinpoint what is wrong like
when I was into such a situation I took help of you guys pointed me that I should
add a dash between eip and the eip number and I got a green check but that was
with the earlier bot and I don't know I mean is there a way that.

**Micah Zoltu**: Yeah, so yes right now it is definitely not easy for end users to understand what the problem is usually as editors. We look and see what the problem is and then tell them in a comment. It would be great if the bot could comment on the  ipsl for on the pull request itself saying hey you need to fix this thing even better. Would be if it offered suggestions on how to fix it like for the spelling errors. The bot could just offer an online suggestion but all this requires engineering effort. I think we have to build something.

**Pooja Ranjan** : Yeah right. I was just wondering if this can be considered as a feature update to the present eip bot.

**Micah Zoltu**: it's a reasonably sized task depending on how good you want to make it. Especially getting the travis stuff out. Because it requires some integration the other direction
which is complicated,so it's not a small task.

**Pooja Ranjan**: Got it okay. So we will consider this in that task list but we will have to ask Alita  and also give her some feedback on this. How long or if she would like to have more people engage working on this or whatever. We will talk to her also. The next item is metrics. I mean the sub item is metrics. I'm wondering if there is a way to collect the metrics of how many proposals are being proposed if not new proposals let it be pull requests or issues coming up every month or every week. How many
gets the reviews comments and how many gets closed or any kind of metrics is it possible to
collect data with the help of github or maybe we can design a part with that.

**Micah Zoltu**: Definitely possible but again requires engineering effort. 

**Pooja Ranjan**: So this is not currently possible with the help of github.

**Micah Zoltu**: They may so if you go to the insights tab in github.It's like github insider pulse , so if you go to the repository and then go to the insights tab at the top.They have some kind of basic high-level stuff. I am not sure if that's quite what you're looking for. The things you list that I don't think are included in. They're very high level.

**Pooja Ranjan**: Yeah I see that too but these are just as you mentioned it's very very high
level, multiple requests or people request something like that. Okay then maybe first we need to determine what kind of metrics could be helpful to understand like how, when we are getting the request from the community and then to see if this is helpful and if not then maybe look into the part well. 

**Micah Zoltu**: As you can say, somehow I fell into fourth place on the eips repo.

**Pooja Ranjan**: that is surprising 

**Micah Zoltu**: very sad day

**Pooja Ranjan**: Yeah that is surprising because I know you and lifeline keep on commenting on most of all of the pull requests not sure of the issues but yes.

**Micah Zoltu**: Well this is for commits not for comments.

**Pooja Ranjan**: Okay So I keep this open as well I will check with Alita on this and we will
try to see if we can get a list of metrics that can be helpful and then probably try to put in some work in this. 

## 4. New EIP/ERC editors (in-training) progress

**Pooja Ranjan** : Moving on the next item is eip erc editors in training progress meeting. So we had this meeting yesterday and we covered I think over five proposals so reviewed and they left comments there. Thank you likeline for conducting these sessions. James Hancock also joined us yesterday. So we now are getting more and more people
involved learning the process and I hope that with this rate if we keep on working we would be in a position to decrease the number of at least pulled requests first under 10 and then we'll start considering the issues section.

## 5. JSON RPC API spec progress update

**Pooja Ranjan**: Okay the next item is json rpc api spec progress. I think Alita left her 
update on the comment that we are nearly done collecting the necessary data to write edge cases and are well into finalized track to begin the client review process. The open rpc spec needs another review from my client. So lifeline if you might want to look into the open rpc specs and she mentioned about a blocker I don't know if someone from here from the group can help it's about finalizing the format for the edge cases in the open rpc spec. This requires that we first merge in previously discussed open rpc. Second and then I will open another discussion on this point. Unfortunately I do not see too much on the call but yeah
anyone  and Micah if you guys have any thoughts or suggestions on it .

**Micah Zoltu**: I think we agreed previously to just move forward with everything except for that and then internally they can use whatever format they want and then before we like to publish it. We will have a discussion and try to figure out what the best format for that is. The impression I got was that no one's really in a rush though to solve that problem.

**Pooja Ranjan**: All right, I will ask Alita to follow the recording and then maybe she can look into it. Maybe in the channel that the discord channel that is created to discuss this open rpc.

## 6. Progress on 'canonical source for EIPs' [WIP doc](https://docs.google.com/document/d/1hUpMQh9gA5z3WSDvXKqU_CS6g3Y0hugJZHDYQdKxot8/edit)
 
**Pooja Ranjan**: Moving on the next item is the progress on canonical source for eips of WIP doc. I see Brent on

**Brent Allsop**:  Yeah I am here. I was able to, I am trying to get my head around the gatsby that  it uses. I have got gatsby installed on my personal machine. I got it up and running but evidently one of the servers is configured with not enough memory. I am working through some problems on how to get that so I haven't got anything to show yet but so I am hoping to be able to understand that system and be able to make changes and then be able to propose changes and show people prototypes and stuff like that but I am still still working on it and so hopefully in the future I will be  able to easily contribute and help a lot of the some of the stuff that we would like to help make on that system so still just learning the system.

** Pooja Rajan**: All right thank you for the update Brent 

## 7. Review action items from the previous meetings

**Pooja Ranjan**: The last item on the agenda is to review action items from the previous meeting. Unfortunately the previous meeting  we did not have the recording it was a very small meeting and we have covered most of the items that we discussed there. Yeah I think we covered almost all of them

### [EIP draft banner](https://discordapp.com/channels/595666850260713488/746566142700814426/849726116980981760)

**Pooja Ranjan**: The sub item is eap draft banner a shout out to felt a discord user who took up this issue and have submitted the pull request which is actually merged right now. We have this banner available on eips.ethereum.org about every proposal like what is the
current status of the proposal and what is the expectation with it. If there is any change expected or people or it is ready for people to use it so thank you so much for submitting the
request for that.

### A bot tracking inactivity period and changing the state of the proposal [Ref issue #73](https://github.com/ethereum-cat-herders/EIPIP/issues/73) 

**Pooja Ranjan**: The another sub item is bot tracking inactivity period and changing
the state of the proposal that is still open. Alita mentioned in the ethereum meeting that she would be looking into this issue and we will try to get it done this month so I will wait for her response to finish it up but there is one thing that I found on a bot's comment, if I remember correctly the agreement was for over 90 days period. Right?  If  any proposal or any pull request is inactive for three months or more then the bot should be sending a message that this will be closed soon. I don't know if I saw somewhere it is two months or something like that so does anyone remember what was the decided period there. Maybe I will go back and check in eip1 because two months seems like a very small duration. Generally any proposal or pull request takes some time for review for people to comment if that is not a very hard proposal. So you might want to keep it open for a little longer if that has.

**Micah Zoltu**:  I am ambivalent about the specific time frames. I don't care.

**Pooja Ranjan**: I mean obviously we would like that if a proposal is here. The champion or the author should be around to push it. We do not want it to be hanging in the pull request
repository for a very very long time. But having said that we should have a decent amount of time provided to notter or the champion to talk about that proposal or any pull requests that they have created. After that part should automatically close. I will look into the specifics one more time and then maybe bring it up in the next meeting.That concludes the item listed here on the agenda. Anyone has anything else that they would like to bring up today. All right we are closing early thank you all for joining us and see you all in two weeks thank you

---------------------------------------
# Attendees

* Lightclient
* Tim Beiko
* Micah Zoltu
* Pooja Ranjan
* Brent Allsop

# Date for Next Meeting: 11 August 2021 at 1500 UTC.



