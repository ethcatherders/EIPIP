# EIPIP Meeting 50 Notes
## Meeting Date/Time: Wednesday 23 February 2022 at 15:00 UTC
### Meeting Duration: 1/2 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/110)
### [Audio/Video of the meeting](https://youtu.be/htwlb08kueg)
### Moderator: ****Pooja Ranjan****
### Notes: Stefan Wüst

----
## ACTION ITEMS

**ACTION 50.1**: Formal onboarding of William Schwab and Sam Wilson as EIP editors [04:30](https://www.youtube.com/watch?v=htwlb08kueg&t=4m30s)
**ACTION 50.2**: Pooja will get in touch with Andrew in order to remove EIP-1706 from the yellow paper [08:10](https://www.youtube.com/watch?v=htwlb08kueg&t=8m10s)
**ACTION 50.3**: Shashank will create an Issue to fix the validator check -> Field: Withdraw reason [23:32](https://www.youtube.com/watch?v=htwlb08kueg&t=23m32s)

**Pooja Ranjan**  00:00
Welcome to EIPIP meeting 50. I have just shared the agenda in the chat.

## AGENDA ##
## 1. EIP Editor onboarding

**Pooja Ranjan**
The first item listed here is EIP editor onboarding. So for the past few months we have been running this EIP editors apprenticeship program to onboard few more reviewers to help out with the EIP editing process. Especially on the standard track ERC proposals and the good news is we have received good responses and possible candidates who have been contributing on the standard track core and ERC proposals.
In the last meeting micah brought up that we can discuss onboarding of these candidates because some of them have been contributing for quite a few months now i know we have discussed this in the past but i suppose we can probably agree on the candidate name and decide on the next steps

**Micah Zoltu**
Like i said last time i would love to get some more editors formally on board

**Pooja Ranjan**
Right i totally agree and i know like client you have been facilitating these meetings and from my experience one of the name is prominent over there that is william schwab so i would like to propose him to be like formally onboarded and if you have any thoughts suggestions recommendation on that

**Micah Zoltu**
Sounds great to me. As far as i can tell william is a human and does not immediately appear to be a bad person so that's all my texts

**Pooja Ranjan**
yeah right he is human for sure i haven't met him in person but i have seen his face sometimes in some meetings so i can vouch for that.
Oh well in the past like how we did the onboarding process was we tried to get some accesses in the EIP github repository for the EIP editor to be working now but i understand now many things have changed since then so i would be looking into what would be the minimum requirement what would be the like minimum steps that we need to formally on board these people and if there is any action item for me that i need to talk to someone i'll be happy to do that

**Micah Zoltu**
just the person just needs to submit a pull request to add their name to the i'll find link but there's a file that has which editors have rights to approve we don't they submit a pr to that and then the current existing editors will review it and approve it and that's it

**Pooja Ranjan**
that sounds simple so i don't see any action item on my part my part except we need to communicate it to william schwab maybe to get his name added so he can also start getting notifications okay let's begin with this and i know there is another name sam wilson he has recently started getting more involved and he has been looking into core as well as ERC's as well what do people think do we need to start for that as well right now or we can probably wait for a couple of more months

**Micah Zoltu**
sam also does a good job of pretending to be human and also does a good job at pretending to be a good person so i'm fine with that
if you can reach out to both of them assuming that's okay with sam as well i know maybe we should interpret matt silent as he really doesn't like sam very much
so if you can reach out to william and sam and have them go to that link and submit a pr to add their names to or their github panels rather to any one of those any one or more of those lines they're interested in helping with then the editors will review it and if everybody's agreeing in agreement it'll get merged and then from that point on they will be able to approve prs and then the prs will be auto merged on that approval doesn't require me or matt anymore

**Pooja Ranjan**
well that sounds good to me as well i will reach out to both of them and the process seems simple as of now i do not see any other action item not on my part and not on like a devops part so let's begin with this and if there is an issue or kind of not having consensus which i doubt highly doubt then we will bring this topic in the next meeting.
Any final comment before we move on?
I'll let them know.

## 2. YP fix, remove EIP-1706

**Pooja Ranjan**
the next item listed here is a yellow paper fix remove EIP 1706. so this item has been picked from the discord chat where exits suggested that yellow paper should be updated someone and someone from the community brought up that a proposal eip1706 is added there which is currently now in withdrawn status. this sounds fair to me just wanted to bring up to here if there is any different thought and a question may be who can update it or if anyone from the group is willing to pick it up

**Micah Zoltu**
i actually have no idea how to update the yellow paper

**Pooja Ranjan**
if i remember correctly for one of the core proposals which was supposed to be updated i mean like i know that was a merged in clients and the yellow paper was updated for that andrew from the erigon team had created some pull requests i remember just because he mentioned this in the in one of the meetings so probably he may be the right person but yeah i'm not sure.
anyone else has any you know ideas or thoughts around how these things work or really people being updated

**lightclient**
i think it's just a matter of downloading the required latex infrastructure for your computer and then making the change
i'm not sure who merges those though actually when i think about it.

**Pooja Ranjan**
okay i just remember the proposal number i think it was 3607 which is now in final status that was the proposal which was supposed to update the yellow paper as well to bring some changes. okay maybe just a simple question: Is it okay if i reach out to andrew and follow up with him to get this thing updated or anyone from the EIP editors would like to own this task?

**lightclient**
i think it's fine to talk to engine

**Micah Zoltu**
i do not want to own this task

**Pooja Ranjan**
In this case both are the right answers thank you so much well okay fine i i will get in touch with andrew and try to get this thing updated but i assume that there is no no like contradiction on eip1706 to be removed from there because the current status of this proposal is withdrawn

all right i now see sam wilson on the call welcome sam and we just missed you as we were discussing. for you to be a future EIP editor and as an action item probably for you from the first item EIP editor onboarding is if you are interested and if you want to contribute as an EIP editor micah has shared a link in which you might want to create a pull request to get your name added so you start getting the pings for every pull request that comes into the EIP github repository

**Sam Wilson**
great okay that's in the the agenda or?

**Pooja Ranjan**
i think it was in the chat i'm gonna bring it again because you joined recently so you might have missed that link

**Micah Zoltu**
add your name to any one of those lines and join us in hell

**Sam Wilson**
sounds fun

**Pooja Ranjan**
The more the merrier i hope you guys will have a good time there

## 3. EIP bot issues

**Pooja Ranjan**
all right moving on to the next item it's EIP but issues update i have added to the link to the EIP part github repository though i haven't seen any new changes or pull requests over there but we have shashank on the call so i'm not sure shashank if you have any update to share on the EIP bad sides please feel free

**Shashank Yalamanchi**
yeah so i see that the ip portions are only mentioning the bot that is related to what alita created but you also have the EIP validator board and it also has a couple of issues you know open so i'm not sure if we are also including these in the agendas to talk about yeah clarification?

**Pooja Ranjan**
oh yeah sorry my bad going forward i will be also adding about eipv issues as well so yeah if you have any update please

**Shashank Yalamanchi**
sure so i i noticed that alpha key has already picked up couple of issues and he's trying to work on the the EIP EIP hyphen bolt so i'm i'm thinking of picking up the ip validator bot end of resolve couple of issues i m i do have some questions regarding one or two issues i'm not sure if we are open to if the follower is open to ask questions regarding that will that be fine?

**Pooja Ranjan**
i hope so we have editors here so i hope your question should be answered here yeah

**Shashank Yalamanchi**
so i think the main the main one is that discussion regarding you know have we formed the consensus around that we should have the discussions to pointing to etheremagicians because i saw comments again on the EIP eipv issue that was raised some account named arachnid commented and also micah was a part of that discussion

**Micah Zoltu**
yeah i believe we are every i believe everybody who is an active editor is an agreement this of course is a very different set of people than all the people in the world and we are not in agreement with all the people in the world and i think we are agreement with all the active editors

**Shashank Yalamanchi**
all right all right so i think so regarding that what would happen to the issues that or the EIPs that didn't have discussion between the previous like so have we have a thought off..

**Micah Zoltu**
sorry we don't plan we don't currently have any plans to migrate existing issues so existing issues that already have or sorry existing EIPs that already are using github or twitter or reddit or whatever for their discussion we'll continue to have that for the time being this would only be validating the new EIPs going forward

**Shashank Yalamanchi**
okay so so the new ips also include the current pull requests that haven't been merged would that be correct in the assumption

**Micah Zoltu**
yeah so any non-final EIP would probably fall under this rule if there's an EIP that has a whole lot of discussion already in a different place we it's probably fine but i would say we can just override when that happens like there might be one or two that are going to get grandfathered in and we can have one of the admins which would be manorai override in that case
for the sake of the bot i would say have the bot very the sake of the bot have the bot be all be very strict so if if there is an EIP that is getting checked by the bot which should be any EIP that is currently has a pull request against it then have the bot validate that

**Shashank Yalamanchi**
okay so i think in one of the issue axic already mentioned a solution his suggestion was to ignore he said two rules one is basically ignore it for anything marked final superseded or abandoned and the second rule was add an explicit exclusion list for EIPs that is a way to disable this check for a set of EIPs and include those which are missing it currently but are merged 

**Micah Zoltu**
i'm also okay with either of those solutions okay those those solutions that alex proposed are more robust than the one i proposed the one i proposed is very easy so it depends if you if you feel you have the time and capacity to implement alex's solutions i do think those are better if we have to choose between doing nothing and doing my solution then i would pick my solution 

**Shashank Yalamanchi**
sure make sense okay that's there so matt there was this issue opened called remove updated will it be fine if i share my screen so it's easy for everyone? i kind of didn't understand this EIP should not be allowed in with updated so when i open this issue it points to this one

**Micah Zoltu**
yeah so there there is a very constrained set of fields that are allowed in the header and updated is not one of them and so i don't know if the validator currently validates that there are no extraneous fields i don't think it does but it should so the validator should when it's checking should make sure that there are no fields in the header besides the ones that are official fields

**Shashank Yalamanchi**
Got it. yeah i think that'll wait thank you

**Pooja Ranjan**
yeah i think that is from the one of the recent pull requests it's a new proposal fairly new proposal that had that additional fee and we were wondering like it would be nice to have the part validating it and i should not auto merge that

**Shashank Yalamanchi**
and we currently only ask the EIP authors to follow the specific fields that are that are like in the given in the ip1 spec right or are they allowed to add any additional sections

**Micah Zoltu**
no so the sections and the header fields should all match what is in the spec within a section things are a little more loose but the top level section so things that start with two pound signs and then everything in the header which is between those three dashes those are very very strict and the more we can get the bot to check those two sets of things the better right now the editors basically manually read and check to see there's no extra sections and there's no extra header fields but we very often miss

**Shashank Yalamanchi**
okay i just remembered there was i think two other yet two other issues that i'd like to discuss one was there was this issue pulled pulled by x i see that's that's to kind of check whether these links within the EIPs are matching correctly or not. are you guys aware about this issue?

**Micah Zoltu**
yeah so there's another thing that would be great to have the validator check doesn't currently but the EIPs should always be in the form EIP dash and then some number of numbers not starting with a zero so like the the reg x would be EIP dash and then any number of numbers first one not being zero recorded so one through nine followed by slash d plus or anyway so anytime there's a link to another EIP and this is the tricky part is going to be identifying where there's a link to an EIP that's a little more complicated but any time there is a link to any another EIP it should use sorry anytime there's another a reference to another EIP it should use that form and it should be hyperlinked using relative pass so dot slash EIP dash number number number dot md it would be awesome if the the bot could catch all of the places that's broken. again this is one of those things that if there's an easy solution that catches 90% that's better than no solution so don't if you decide you wanted to follow up on this don't get bogged down trying to get it perfect. maybe the simple solution is to just look for the common ones like the one alex mentioned here so he lists a set of common formats maybe just search for those formats and fix them only don't worry about trying to find every single EIP mention. also i think that Pooja may remember in a recent meeting we discussed whether we should always use the EIP and not ERC did we come to a conclusion on that

**Pooja Ranjan**
yeah we have updated the eip1 for that so for there the number is like EIP-20
in a similar context if i may ask to look into the EIP number seven zero six shashank while you are sharing screen would it be possible for you to go to eips.ethereum.org and just take out the eap1706?
So here when we see into look into the withdrawal reason i see the format is not working i remember that this thing was working earlier but it seems like something has broken. anyone has any i idea like why is it not reflecting the correct i mean why is it not properly structured not that one, withdrawal reason.

**Micah Zoltu**
my guess is because that isn't that's the header isn't rendered with marked markdown render. if i just had to take the wild guess and because of that it's not rendering properly so the place for someone who's interested in tackling this issue, the place to check would be github.com/ethereum/eips and then under i want to say under underscore layouts is where it's going to be or maybe index.html anyways in in that repository is where all this the rendering happens. yeah okay so if you i'll drop a link. if you go there to that link is pasted you can see it's escaping the withdrawal reason and so fixing this is not going to be simple i suspect.

**Pooja Ranjan**
is withdrawn reason a valid field maybe that is the reason

**Micah Zoltu**
no it's always a valid field it was we added it not terribly long ago

**Pooja Ranjan**
i remember discussion on this but i wasn't sure that this is the case i didn't see i probably didn't see this withdrawal reason in any other withdrawn EIPs

**Micah Zoltu**
there we go all right so so fixing it is going to be a pain the the fundamental issue is that it's not it's not marked down we could make the withdrawal reason mark down but i don't know how to do that so this would be a research project to figure out how the github markdown or how the jekyll which i believe is marked out the renderer we're using how does jekyll render stuff and how do you tell it to render some set of text as markdown.

**Pooja Ranjan**
all right maybe in the sense of time this the best next step for this would be kind of creating an issue and maybe then we can explore the reason and if we get there then probably the team can look into fixing it

**Micah Zoltu**
yeah so definitely create an issue for it it is a bug it's just i'm guessing it's going to be more difficult to solve than most of the other problems we have and so i would recommend prioritizing other things over it since it's relatively minor

**Pooja Ranjan**
sounds fair.

**Shashank Yalamanchi**
yeah that will be it i guess thank you

**Pooja Ranjan**
thank you shashank if you can also like just create an issue for the bug that we just discussed for eip1706 that would be nice all right thank you

## 4. Execution specs

**Pooja Ranjan**
moving on the next item is execution specs i know sam has another meeting and he just left i'm not sure if we have anyone else on this call has any update on execution specs right now maybe going forward i will try to keep it in earlier items so we can get to there.

## 5. EIPs Insight

**Pooja Ranjan**
The next item listed here is a EIP's insight. The link to the EIP insight is added in the agenda as of now we have four new proposals and the latest one which was also discussed in the all core dev meeting is eip4788 that is beacon state route in the EVM that is one of the most discussed proposal and possibly will be getting a place in shanghai not decided yet but it is under discussion.
Other than that we have three proposals moved to final and four proposals are moved to review status. The new proposal those have been added to the review status is ap four three nine nine a supply and difficulty opcode which is there for the march and there is this another proposal 4803 limit transaction gas limit. this proposal is also a core proposal and it is not supposed to be a part of any upgrade that has to be implemented in the client asynchronously so yeah that's another one to look into. i mentioned it in the last call there is one proposal that recently changed, it's a type from informational to standard track, that is eip2098 and rest all information are added on the EIPs insight document that is added to the agenda

## 6. EIP editor apprenticeship meeting

**Pooja Ranjan**
next item is EIP editors apprenticeship meeting the video link is missing here but the video is published we had this meeting yesterday and we discussed about a proposal that is currently in a draft form as in pull request the number is 4505 the authors of the proposal were also present in the meeting and they had some questions we tried to when like the ap editors tried to answer that talking about this particular pull request i i remember reading a comment about the proposed standards so it appears that there is similar standard available not in EIPs category but i was just wondering out of curiosity - i understand that it would not be possible for us to like make sure that everything that is coming up new, especially in the ERC category, we would be able to validate if there is something existing already in some form of standard. just wondering if any EIP editor has thought about, how do we make sure that a standard here is not like earlier added to the repository i mean

**Micah Zoltu**
it's a hard problem the best chance we have at that is that when the when editor goes to review it they're the most likely ones who will have seen something similar before and they can like if they notice that this is a duplicate or something similar to another one, they'll at least i will usually tell the person hey this looks a lot like EIP blah blah blah i'm going to check that out before merging this. that being said it is okay like people are allowed to submit duplicates, in fact if there's a strong enough disagreement between two parties about how he should move forward one of the recommendations for resolution that we we give people is that they should both just create their own EIP and operate separately. and such in such case those EIPs will be duplicates of each other basically so yeah so there's no fully automated solution for this that i can think of that doesn't involve like designing a revolutionary artificial intelligence and so i think just best guess of editors or best effort of editors is all we've got

**Pooja Ranjan**
that's yeah probably the right solution and i'm sorry i i suppose i'm set the wrong pull request number the correct one is 4671 i have shared the link in the chat here.
okay that sounds fair and that would be the recommendation for new editors looking into it they have finished potatoes looking into these proposals.

## 7. Other discussion topics

**Pooja Ranjan**
the next item listed here is other topics other discussion topics which are referred here and i think these are the items suggested by william in trichen he did make some pull requests and i see that that is mush now and i'm not sure in one of the past meetings or to an earlier communication to me he did mention that he would probably want to come up to these meetings and talk about the rest of the issues that he has added though i don't see him on the call so i'm gonna drop it for now and maybe we will bring it back whenever he is available or he would especially request for bringing this back to the discussion.

## 8. Review action items from the previous meeting

**Pooja Ranjan**
Going for the review action items from the previous meeting, i know there was this one that i'm supposed to talk to FEM team about the limited editing window i have pinged the theme but i'm waiting for response probably because of ETH denver people were really busy there so and most of them are traveling so i'm not sure they did they got the chance to look into it but i will try to follow up with them again and hopefully we should have something in the next meeting to share with the people.
That's all on the items listed here. Anyone has anything to bring up or any new discussion points for the upcoming meetings?

**Micah Zoltu**
Nothing for me

**Pooja Ranjan**
if there's nothing then probably we can assume this is going to be one of the shorter call. well thank you everyone and as usual i would request the people if there is any question or any concern related to EIP, EIP process or anything in general that might require editor's attention, please feel free to add in the comment section of agenda for the next meeting so we can bring it to the discussion.
Thank you everyone for joining, have a good day everyone!

# Attendees

* Ben
* lightclient
* Micah Zoltu
* Pooja Ranjan(Host)
* Sam Wilson
* Shashank Yalamanchi

# Date for Next Meeting: March 9 2022 at 1500 UTC