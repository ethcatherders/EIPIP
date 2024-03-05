# EIPIP Meeting 100
### Meeting Date/Time: Wednesday, 14, 2024, at 17:30 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethcatherders/EIPIP/issues/312)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=9GRzvp06Qlg)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----------------------------------------------------------------

## ACTION/DECISION  ITEMS

**ACTION 100.1**: In regards to working Group Charter, Sam shared the [link](https://hackmd.io/@SamWilsn/rk2CG6qqp/edit) to collect feedback and is willing to present it to the editors' group in the upcoming meeting.

**ACTION 100.2**: Sam will merge the PR asap for [ethereum/ERCs#213](https://github.com/ethereum/ERCs/pull/213)

**ACTION 90.3**: Pooja Ranjan will inform the group if there is any success in rendering RIPs. as of date, eips.ethereum.org includes EIPs and RIPs data but does not render RIPs.  Also In parallel, @SamWilsn is working on page rendering based on the working group. The output will contain RIP data as well.

—------------------
## AGENDA

**Pooja Ranjan** [0:00](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=0s): Welcome to EIP IP meeting 100 this is issue number 312 on Ethereum Cat Herders / EIP IP GitHub repository um today on agenda we have some discussion with respect to EIP process standardisation open issues and PR will take a look into call for input and some other discussion continued from the earlier meeting followed by eips insight for the month of February.

# 1. EIP Process Standardization

## Adding "Errata" section for Final EIPs.

- Open a pull request to modify EIP-1 and eip-template.md

**Pooja Ranjan** [0:24](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=24s): So starting with the very first item which was suggested by Greg here it is about adding the Errata section for final EIP. We understand that this discussion came up multiple times in the EIP
meeting but because this was specifically requested to be discussed and made a decision in this meeting. So let me invite Greg to maybe provide some background why he wants that and we can open the floor for editors to share their thoughts over here 

**Greg** [0:28](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=28s): Yeah I'm looking through the agenda item. It's probably not that important; it came up recently on a request  from an author to add a co-author. There was some discussion some discussion of that so
far as even what authorship meant. So there's some disagreement on that but I think it's pretty clear industry wide for publishing that a major contributor to any publication is considered an author and certainly ifa  primary author is saying you know this person is a co-author, then there shouldn't be any real doubt of that and if that person was was left off the list that's an error that should be corrected somehow and in general for instance for a final EIP that's a core EIP. The EIP needs to describe what's actually running on the main net and if it does not describe that then it's an error that needs to be fixed. And for years
the intention has been that we can have Errata and we simply have never gotten around to deciding on just how we want to do that. So I wanted to just settle that. How we do that so we can even have reasonable discussions of whether some requested change is an Errata because it just keeps coming up and I think in the industry it's done in one of two ways, either the document itself is corrected and a footnote is added saying a previous version you know had such and such mistake or the original document is left alone and then there's some sort of footnote or separate something saying, you know this is the correction. The latter way there's an original document in the header, it will say there are Errata and then there's they maintain a separate list of all the Errata  and actually have a link to a version in which shows the version with the merged Errata. We can do it either way I think. Hob would support by creating a fork of that document that's been corrected but it it could be done either way so i' just like to open up a discussion on that one and if we get any consensus on that then there's the particular issue on the PR are to add the missing author Somehow

**Sam** [5:11](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=311s):  So what would the Errata section like to bring over to get commit history.

*Greg** [5:21](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=321s): Well first I guess the first decision is you know what we do we allow for Errata. I think that decision needs to be yes but I don't know if we have consensus on that. 

**Sam** [5:43](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=343s): I think we do allow very limited Errata right now and we use get commit history to track them. so I think you know EIP 1 does say that we're allowed to add clarification and Errata so.

**Greg** [6:04](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=364s): Yeah okay I'd suggest that only normative things need to be fixed if it's not normative then there's no compelling reason to change it but anything normative that's wrong needs to be made right and I guess authors are on the edge as to whether that's normative. But it's important you know even  just a search with the duck or with Google you know we'll find policies for you know for Journal after Journal you know indicating that you need to give credit. Where credit is due it's I think in some cases it's almost a legal thing someone can actually sue  that they were an author and they were not credited. So, if we already have a procedure in which we simply correct the document and the history shows that a correction was made then I think maybe we just need a field in the header pointing back to that commit or or what do we already have a process for.

**Sam** [7:48](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=490s): So I think the process right 

**Gajinder** [7:55](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=497s): Yeah actually the reason that you mentioned that somebody might the reason that we should not be having the author list because people can keep coming back and saying that you know I
8:06
contributed to this but I was left out and it is already always it will always be a bone of contention. So, I think that we should change author to maintenance and we should call it a day instead of opening this Pandora box of allowing the changes to final EIP. 

**Greg** [8:28](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=508s): Well wait a minute the first question is, do we have a process ? do we have a way of making a change for Errata? How do we do that and how do we indicate uh that that's been done.

**Sam** [8:53](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=533s): Yeah so right now we use the call for inputs for that so if somebody wants to make a change to a final EIP. They or  more likely I can make a call for input where we collect editor opinions and then m decide if we're going to allow the modification or not.

**Greg** [9:16}(https://www.youtube.com/watch?v=9GRzvp06Qlg&t=556s): And if we make the modification how do we indicate that something was modified. 

**Sam** [9:23](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=563s): You just modify it and then the changes are shown in the history.

**Greg** [9:30](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=570s): Okay that would make sense to add a field to the header and indicate that it had been modified and give the commit.

**Sam** [9:45](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=585s): So there is a proposal that the testing team brought up recently for EIP versioning and I think that would be a reasonable way to. Yeah sorry I think that would handle reasonably what you're suggesting so you would indicate why you're changing the EIP and then you'd also include either a patch minor or major version number bump. Yeah thank you Pooja and  that would be in the header so you would be able to tell what changed and when.

**Greg** [10:24](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=624s): Okay I'm on a phone now so I can't  easily read the chats there's not much I can't even see the screen outside where I am. It's too bright just so if people are putting things in the chat I can't see them.

**Sam** [10:43](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=643s): I'll put it in Discord for later.

**Greg** [10:46](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=646s): Okay if that's already settled then the issue is whether we can add an author later and I strongly think that if the primary author is saying we missed an author and we need to give this person credit . I cannot see any reason why we would not make the Change.

**Sam** [11:20](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=680s):  So I think this is where Gajinder's objection comes in where if we have authorship as a field and please jump in if I'm misrepresenting your opinions here but if we have authorship as a field then people can always come back and say, oh this person was an author even though they didn't contribute meaningfully to the document and so he's suggesting. We rename the field to maintainers and remove the implication that they authorship credit.

**Greg** [12:04](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=724s): Very often the authors are not they were authors.

**Sam** [12:13](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=733s): Right exactly so we should rename the field so it isn't authors anymore and make it purely just people who have permission to merge PO requests so Gajinder posted in chat. how can one miss an important author all this while the EIP went through to become final.

**Greg** [12:30](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=750-s): If you change that often there are eips, core eips even where the original authors no longer maintain it at all.

**Sam** [12::49](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=769s): Exactly so I think the idea would be to not call them authors anymore.

**Greg**  [12:54](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=774s): So we go in and make a change and say I forget who the authors of vc20 are but I think they've all moved on and if not that one I'm sure you can find a number of eips  even very important ones for which the authors are are have moved on and have no further interest in maintaining the document.

**Gajinder** [13:27](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=807s): Yep so we have such eips where someone is trying to. For example, move them from stagnant to basically draft status and we can't do that. We don't allow them to do that because the original author does not agree to that and the original author also doesn't want to maintain the EIP. So I mean we already have this current behaviour  with regard to the eips that I mean if the final eips anyway don't need maintenance so again it doesn't matter whether the authors have moved on or not and for the eips that have become stagnant if the author is not willing to let somebody else take charge and so they can't really do that so in that case a new IP has to be created. So we already have this process where we force people to float a new EIP if they want to worked on an old EIP and if the previous author is not available or previous author doesn't agree through that 

**Greg** [14:40](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=880s): This gets strange for instance EIP 615. Christian is still an author and he contributed substantial text which is still. There he actually opposed that at this point and I asked if he wanted to be removed as an author and he did not he wanted credit for the text that he contributed even though he no longer wanted the EIP to be accepted by the core devs in the form that it's in now and I don't think it's ever been withdrawn it's simply in probably stagnant status. Yeah regardless that's just a an example where if for instance EOF failed I might very well decide to resurrect that one and would see no reason necessarily to have to give it. A new number just because one of the authors wasn't interested. It's a dicey situation but legally it's much more appropriate to leave the authorship unless that author actually wants to be removed as the Author.
**Sam** [16:52](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1012s):  So just to kind of restate this again the idea would be that we no longer track authorship at all as part of the process and we only track permission to merge Port requests and that would be the  change I think that gender is proposing.

**Greg** [17:07](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1027s): Only the editors have permission to actually Merge.

**Sam** [17:13](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1033s):  So when unless you're changing the Status authors can merge without edit or approval.

**Greg** [17:35](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1035s): This all gets very confusing. Do we if the winds up being conflicts between existing authors then
what.

**Pooja Ranjan** [18:07](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1087s): I think what has been suggested so far I'm just trying to take some excerpts from the discussion here. if there could be confusion between or like disagreement between two authors of the proposal the best way to go forward would be to come up with either a new proposal or just to you know remove the author with obviously the author who is disagreeing can agree to be removed at that point and we can move forward with the proposal. If I understand correctly
people are suggesting here is like we  should not make edits to the proposal when it went into final status. However that's not the case with proposal 615 that is still stagnant can be brought back, it can be resurrected and it can be updated with the author list over there. But uh in case a proposal is finalised. We should not allow updates. However another proposal that came up was a versioning scheme that may allow some of the minar things and if people are open to consider updating this author as Non. It could be a part of that if we want to go ahead with a call for input here to collect points from other editors . They generally think about it and we can perhaps make a decision in the upcoming meeting.

**Greg** [19:44](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1184s):  This seems to be an easy case. The primary author has said basically it was mistake to leave this person off and we want to to add the person to

**Sam** [19:58](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1198s):  So the decision on that particular EIP has been reached and I don't think anything new has come up so let's not reopen discussion on it .

**Greg** [20:08](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1208s): Okay the decision was incorrect and I object strongly to the decision and I had to. I would block the consensus if I could, it is completely unfair to the primary author and to the person the primary author wants to add once. 

**Victor** [20:38](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1238s):  We do this so Greg. I think we should very carefully use our way to our power to draw consensus.
if we are like the minority opinion I think it's okay that we kind of just like how the Supreme Court does. We can just publish in my only opinion but still allow the uh if we feel strong enough but still allow the general editor group to follow the consensus of other people because any time a blocking opinion a blocking ISS anytime if any one of us raise an I an attempt to block consensus it's kind of a damaging to not only our efficiency but also like how we collaborate so I like to say that I agree with you on opinion side. I'm okay to site with you on minority opinions. I am not very comfortable that we are using this to block a Consensus.

**Greg** [21:43](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1308s): I don't know what to say. I read it carefully and the arguments to not give this person credit simply I think they're wrong I absolutely think. They're wrong and I think they set a very bad precedent.  

**Victor** [22:05](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1325s): I agree with you on that yeah I totally agree with you on the fact that I disagree with not giving this person credit and then we pretty much claiming a right of Editor to deny adding new Authors which I don't think is a good idea to begin with but also think.

**Sam** [22:30](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1350s):  It's very sort of jump in here but this call for input was open for 30 days and I'm using my keeper of consensus Powers here we are not reopening this discussion unless we have new arguments that weren't listed on the on the call for.

**Victor** [22:45](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1365s):  I agree with Sam. I would go with that consensus.

**Greg** [22:53](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1373): So this is now
 a policy going forward that we will not correct off.

**Victor** [22:58](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1378s): Then can we say this is not a policy.

**Sam** [23:05](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1385s): No, as far as I know we aren't like precedent based we can decide whatever we want at the time. Yeah 

**Victor** [23:12](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1392s): Okay so I guess I interpret the consensus being without setting a president at this time. We're not adding it unless we see a new argument.

**Greg** [23:24](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1404s): What has been the reaction of the primary author and the person who should be added but especially.

**Sam** [23:42](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1422s): As far as I know they haven't said anything since opening the PO request.

**Greg** [23:47](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1427s): Okay as usual I'm not a lawyer none of us are and CCO might complicate things  but they're I believe their substantial legal precedent about you know failing to give credit to an author. So I don't think there will be any lawsuit in this case but I think we're doing a bad thing and not allowing a primary author to give credit and I'm sorry that I did not notice. I think I was in the discussion early on and then time went by before I noticed discussion had closed off  but so I apologised for that and you know I sit on the edge of whether I should remain an editor. I basically way behind in difficult work on an $18 million startup. So I can only give occasional attention to what's Happening Here. I try and keep an eye on things that are very important to me um of course yeah and you know. 

**Sam** [25:22](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1522s): We don't want to unfairly disadvantage you because of the amount of time You can commit right. I'm hoping that our 30-day windows are sufficient, maybe we need to make them longer I'm not sure.

**Greg** [25:40](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1540s):  Yeah or I need to figure out some way to  know my notification stream.

**sam** [25:48](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1548s):  I can email you like what makes it easiest for you to follow along. I can definitely figure that out.

**Greg** [25:58](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1558s): Yeah  I need to look at the titles to see if there's something discriminating my currently my filter pulls in so many notifications they stack up in the folder to where I have, I think something like 5,000 unread emails of notifications of ethereum related stuff. So, yeah if you're if you're willing if you're willing to keep an eye on things and notify me before they go to final.

**Sam** [26:37](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1597s): yeah just let me know how um we can we can discuss that on Discord or whatever I don't want to take up too. much of everybody's time 

**Greg*** [26:44](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1604s): Mostly I just  try to notice when VIP meetings are when these meetings are coming up and check the agenda and be sure to participate I don't know on this one but I really appreciate if anything that requires consensus does come up at this meeting rather than the consensus happening on the discussion Fred because it's hard even to tell on a discussion thread whether a consensus was reached or the discussion. Just sort of trailed off. So I don't know

**Pooja Ranjan** [27:24](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1620s): 
yeah so yeah I mean for that we have called for input included in EIP meeting every other week whenever we have this meeting so I think that would be a good place to follow up with 
the points where consensus are required.

**Greg** [27:39](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1659s): Yeah I do not know in this case whether it came up at a meeting that I just missed and I don't does the agenda to go out as some sort of separate um email or something.

**Sam** [27:58](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1678s): So currently I publish them on Discord and GitHub. If there's some other way you'd like me to send them I can certainly do that as well.

**Greg** [28:11](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1691s): Unfortunately discord's, mailbox feature is useless it only it keeps track of the last two weeks of messages and so  if I'm away or even just travelling for more than two weeks, I'll come back and it's well here the last two weeks what happened before that well we erased it too bad and just I don't know if Discord even has a good way to say please email me anything that would have gone in that box um so yeah that would help I try to attend all these meetings unless there's a conflict um but I think the only way to actually check the agenda is to  you know look the
day before and that's it's hard to I may have already scheduled a conflict by then so and I don't know if we can reopen this but I really feel strongly that we are doing a big service to these people and I doubt they would go to court but I think doing things this way actually opens up to Legal liability and it's hard to tell because copyright law varies internationally. so the exposure is international and just somebody said something about. It's not for fluffing resumés and it isn't really credible and that's just a wrong argument trying to decide Things based on something that might hypothetically with low probability happen in the future is silly and it's not just about fluffing resumés. It's about giving credit where credit is too and that's just a long established principle in copyright and authorship. 

**Sam** [30:30](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1830s): So Gajinder mentioned in chat that copyright has been given up through CC0.

**Greg** [30:42](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1842s): I am right but only the copyright holders can give that up. so if someone is there with both that person and the primary author basically you open up a different kind of liability where a person can say wait a minute I was an author and I did not release my rights.

**Sam** [31:11](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1871s): Yeah that can happen regardless of whether they're in the list or not. Right like that and there's no restrictions on who can add authors like I can add you to an author and pretend that you released it via CC0 so that we can't use that list as any kind of like legally binding set of contributors.

**Pooja Ranjan** [31:44](https://www.youtube.com/watch ?v=9GRzvp06Qlg&t=733s):  I think we should perhaps consider this as. I mean even if we don't want to quote it as a precedent that we have made this decision this could be an opportunity for new Authors to make sure that whenever they are moving any proposal to a final status. Please be sure that there would not be any further edit. It's not just about authors, it's about any other thing. Authors are definitely important, their contributions are immense towards a standard but this can be an example that can be double triple and no matter how many times you need to be very sure that this is it this is going into final please check it out.

**Greg** [32:25](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1945s): Okay I mean I don't feel strongly enough to block it but I would very much like to reopen the discussion on this. I simply made a wrong decision in my opinion and if we have no way to go back and say we made a wrong decision and we're going to correct ourselves it makes no sense to me.

**Pooja Ranjan** [32:59](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=1979s): I think we can let it rest over here because this was already closed. So as I mentioned if we come up with some new references, new examples. we can perhaps open it or if there are any other new cases about this maybe we can reopen the discussion.

**Greg** [33:21](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2001s): I'd like someone to reach out to the author to see if they're as unhappy as I am or if they're willing to just shug and say well the process is gone and I'll accept the result Simply.

**Pooja Ranjan** [33:42](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2022s):  I hope the author follows the EIP meeting and may be able to reach out to us or may be able to comment on the PR that was open to add some new references for our consideration.

**Greg** [33:58](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=733s): Okay well I will register my extreme unhappiness with the situation, we are doing a disservice to the authors, We're just being unnecessarily rigid and that's a regular complain about us and our process that we're just rigid and bureaucratic and impossible to deal with that Way.

**Pooja Ranjan** [34:39](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2079s):  Right I mean this is decentralised yeah 

**Gajinder** [34:44](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2084s): Maybe even a further Wilder idea would be to not render author SL maintainers on finally EIPS anyway, I mean when can render them on or maybe not even on the other eips because it's about who can push and who can edit and we can just totally remove this tab when we renter it on the website.

**Greg** [35:20](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2120s): The authors can even even release rights under a CCO and so if you leave anyone so one has to credit the authors at some point even even for that CCO to be meaningful and so it may not happen but whenever we do this we set up a situation where an author an actual author this person actually is an author can come back and say I did not release my rights. Yeah I'm with Pooja on this one.

**Sam** [36:07](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2167s):  Let's end discussion on this topic and we can continue with asynchronously.

## Working Group [Charter](https://hackmd.io/@SamWilsn/rk2CG6qqp/edit)

**Sam** [36:12](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2172s):  So next up we have the working group Charter so I posted a link at the top of the chat and I will repost it now. So this is kind of my work in progress draft on what I am going to be showing to editors later to vote on or to rough consensus on whatever the term we want to use and this is  describing how working groups are going to work their General responsibilities kind of the shape of all. I just wanted to bring it up here in case anybody has any early feedback but it's not done yet that's it for that topic.  I'll turn it over to Pooja and you can continue the call 

# 2. Discuss Open Issues/PRs, and other topics

## Merge [Update ERC-1363: Add missing return statement ethereum/ERCs#213 ? Ref](https://github.com/ethereum/ERCs/pull/213)

**Pooja Ranjan** [36:56](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2216s):  So the next one here is about an open PR I believe We made a decision to merge this one in the earlier meeting but it seems to be open and the author is wondering if there is anything to be done from their side can someone maybe take a quick look and see where we are on it. The PR number is ERC 213.

**Sam** [37:24](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2167s):  yeah I think this is fine it's adding comments so I'll just go ahead and Merge. This merge this unless somebody objects. This is a final ERC and it's adding at return annotations to some functions.

**Pooja Ranjan** [37:42](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2262s):  Yeah right I mean it was approved, Yeah it was approved in the last meeting as well.

## Call for Input

**Pooja Ranjan** [37:53](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2273s): Perfect very well, the next here are a couple of call for inputs which have crossed the deadline. Sam if you would like to maybe share more about it and if there are any decision. 

**Sam** [38:09](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2289s):   Definitely so we have 306 and 308. So 306 is for back references from a later EIP to an earlier one. So this would look something like  ERC 223 would have a header in it. That's superb seeds and it would have the value of 20, So it would be like suedes coal and 20 and that would be an ERC 223 and then on the erc20 page we would have a list of all of the things that are claiming to supersede erc20 so this would like improve navigation between proposals that claim to replace one another that's kind of the 30 second summary of this. Yeah, so I guess we'll just do a quick temperature gauge here. How do we feel about these back references? I know Gajinder, you said you are not in favour. 

**Gajinder** [39:15](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2355s):  Yeah I mean as long as the Clutter can be managed, I'm fine with it. I mean if there is so many back references that can clarate.

**Sam** [39:33](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2373s):  All right and Greg do you have any opinion on this right now or would you want to bit more time to look at
it.

**Greg** [39:40](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2380s):  I'm not sure if I completely understand. I'm sorry, I'm on a phone here so it's hard.

**Sam** [39:47](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2387s):  Oh no worries  

**Greg** [39:53](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2393s):  Are we generally not wanting to supersede or are we generally wanting to have superseded. 

**Sam** [40:04](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2404s):  I think that's what we're trying to figure out right now um I'm in favour of it and yeah. 

**Greg** [40:11](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2411s):  I think about  what's on the main net. There's only Errata, it's already on the main net and if there's an upgrade then it's just sort of automatic. that an EIP the core EIP needs to describe what goes on the main net and the appropriate thing I guess is a new EIP. The purpose the main purpose I think of having superseded is so that somebody who's trying to implement it doesn't go in and Implement an older EIP that's no longer the way that we do things a little
less important for erc's but still important. I said last week to write a small web server and started on using one EIP to do it and then notice that it had been superseded and had I done it according to the first EIP. It would not it would not necessarily work because things have changed. So  I can see a need for it but I'm just not quite sure whether we want to do it that way or not for all.

**Sam** [42:07](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2527s):  Right yeah I'll add those to the thread and yeah thank you.

**Greg** [42:15](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2535s):   If you could send me a link to the thread I don't think chats tend to stick around after calls. I may be wrong, I just don't know where to find them.

**Sam** [42:37](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2557s):  Yeah I'll send it on Discord.

**Pooja Ranjan** [42:41](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2561s):  Okay perfect with that perhaps we can move on to the next one or is there anything depending on call for input.

**Sam** [42:50](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2570s):  No, I think that's all of them. I don't think there's any new ones.

**Pooja Ranjan** [42:55](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2575s):  No I don't think so .

**Sam** [42:57](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2577s):  Yeah I think
we're good.

# 3. Other discussions continued or updates from past meetings

- RIP process documentation

**Pooja Ranjan** [43:02](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2582s):  Very well moving on to the next one that is continued or updates from the past meeting. It's about the RIP process and documentation, but I haven't heard back from the RIP team. It seems like they are doing well with what they are doing right now. I have noticed an introduction of another RIP. This month but yeah we might want to hear more from the team whenever they have an opportunity to share about it. 

- Web Page Rendering to include EIPs, ERCs, RIPs

**Pooja Ranjan** [43:33](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2613s):  Apart from that in the last meeting we discussed web page rendering to include EIP, ERC, RIP. I know at this point of time e. ethereum.org includes EIPs and ERCs but they are not able to include the RPS part. Sam also made some progress on a working group on their website and may have missed this. Samp please help me remember that does that include RPS as well. 

**Sam** [44:01](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2641s):  So the working group proposal would include RPS.

**Pooja Ranjan** [44:07](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2647s):   Oh no I'm talking about the rendering of the website.

**Sam** [44:11](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2651s):  Yeah so the the version of the website that I'm working on for. Working groups would render RPS .yeah I haven't really touched anything without working groups yet.

**Pooja Ranjan** [44:25](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2582s):  Right now because  one of our contributors was working on e. ethereum.org and unfortunately we have not seen much progress on sharing RIPS on the page as of now. If there are any change in future we'll we'll keep the group posted about it.

**Sam** [44:47](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2687s):  Sounds good
thank you 

# 4. EIPs Insight - Monthly EIPs status reporting.

- [EIPsInsight.com](https://eipsinsight.com/insight/2024/2)

**Pooja Ranjan** [44:50](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2690s):  Moving on the next one is EIPs insight for the month of February as you can see we have total of eight draft including one in RIP total of six erc's and one new EIP have been added to the repository. We have five total proposals in the review section. There are proposals in last call but most of them are on four side proposals which would be moving towards final when they are finally deployed on the main net but because those are on public testnet. They are in last call and just for people to remember this last call duration for core proposals
are more than 14 days. It's not limited to 14 days it would be whenever they are deployed on the minute. They will be merged as a final proposal. There is one proposal  which is EIP 2070, which was hard Fork meta for Berlin that has been withdrawn and the inclusion
of the information added to this proposal is included in a proposal shared by Tim to include all the missing so that's all about eips insight for this month. I'm quickly taking a look.

# 5. EIP Editing Office Hour

**Pooja Ranjan** [46:13](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2773s): Yeah so for the next  EIP editing office hour, the agenda for meeting 32 has already been added. Its just a request to all authors irrespective of the type and category whether you are an EIP author ERC author or rip author if you are looking for attention of editors  for a PR that has been in the repository for quite some time and it could not PR an attention of editor please add that as a comment to the agenda added over here. We will definitely try to include that in the next meeting which is on coming Tuesday at 16:00 UTC. So it would be on February 20th at 6:00 UTC and yeah that's all about it any other thing anyone would like to quickly
bring up or may perhaps want to add it for the next meeting I'll be happy to add it to the next
Agenda

**Greg** [47:21](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2781s):   If I could back up a little bit on supers seeds. Sam I think is the executable spec at this point considered canonical.

**Sam** [47:40](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2800s): As canonical as anything is you can link to it from EIPs if you want to.

**Greg** [47:47](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2807s):  The point being if someone is setting out to write a client. Then following the executable spec is the way to go as opposed to trying to gather together all of the eips that happen to go into yeah it's.

**Sam** [48:07](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2887s):  Certainly easier.

**Greg** [48:08](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2888s):  Okay it's almost the only way.

**Sam** [48:10](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2890s):  Because the yellow paper has been updated as well at least two the merge yeah. 

**Greg** [48:21](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2901s):  Yeah I didn't see that after the merge there was any commitment to keep that going and even objections to keeping it going a fair number of our developers don't have any mical skills apparently. Nobody wants to spend money on Hing doing an edit or right to just clean up the presentation but anyway. The super seems a bit less important on core eips because they're not where you go. They're not where you go to see what is canonical. The canonical thing to implement if you go back to an older EIP that describes an older chain U it's sort of your bad .

**Sam** [49:19](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2959s):  Yeah this would be more for things like there were two proposals for deprecating self-destruct one was withdrawn and the other was finalised or I think it's in the last call. so you could have a supersedes from the one that's actually going on the network to the withdrawn one if you want it's for like document status

**Greg** [49:45](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2985s):   If he was withdrawn, there was really nothing to supersede.

**Sam** [49:58](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=2998s):  Yeah it would just be to get the link to like from the withdrawn one to the next one kind of thing.

**Greg** [50:05](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=3005s):  That's not available on Github.

**Sam** [50:10](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=3010s):  Not right now I don't think no 

**Greg** [50:16](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=3016s):  He's not even
report I mean as of now.

**Pooja Ranjan** [50:30](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=3030s):  Supered is not a legal status in EIP process but if people really want to share the information of which EIP may have superseded in case the earlier proposal has been withdrawn. We can perhaps add a sentence over there to let people know which is the next EIP they can follow.

**Sam** [50:50](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=3050s): Yeah we have withdrawal reasons for that.

**Greg** [51:01](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=3061s): EIPs are withdrawn make note in the withdrawal of the things withdrawn in favour of a different
proposal.

**Pooja Ranjan** [51:25](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=3085s): Anything else anyone well  thank you everyone for joining us today hope to see you in two weeks have a good rest of the day everyone

**Sam** [51:38](https://www.youtube.com/watch?v=9GRzvp06Qlg&t=3098s): Thanks for hosting talk everybody later.

 ---------------------------------------
# Attendees

* Sam
* Pooja Ranjan
* Gajinder
* Gaudren
* Zainan Victor Zhou

---------------------------------------

# Date for Next Meeting: February 28, 2024 at 17:30 UTC
