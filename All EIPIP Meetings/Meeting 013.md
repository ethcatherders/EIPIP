# EIP Improvement Process Call #13 Notes
### Meeting Date/Time: July 29, 2020, at 15:00 UTC
### Meeting Duration: 1 hr
### [Audio/Video of the meeting](https://youtu.be/8dxGtomafP4)
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/25)
### Moderator: James Hancock
### Notes: Pooja Ranjan

----

# Summary

## Decisions / Action items

Decision Item | Description
---|---
**13.1** | Hudson, James will coordinate to create a separate repo in Ethereum GitHub to place network upgrade related stuff.  
**13.2** | Hudson and Lightclient will look into triaging permisssion. James will help with the list of people to be added.  
**13.3** | Lightclient will work on validator and bot stuff. Alita volunteered to help. 
**13.4** | Alita will look into better formatting of EIP-1. 
**13.5** | Muir Glacier postmortem upgrade report and template -  take more time to think about this and talk it on the telegram and then in the next meeting make a more final decision on wether to keep it in EIP repo or a separate repo to be created for network upgrade related EIPs. 
**13.6** | "What you would like to see in a repository like network upgrade?" We should write up the naming question and post in the telegram, post meeting.
**13.7** | Standard citation format to the footer of all EIPs - It’s just fine to merge. 


---

# 1. [Network upgrade process ](https://github.com/ethereum-cat-herders/EIPIP/issues/25#issuecomment-664792653)


Video | [0:10](https://youtu.be/8dxGtomafP4?t=10)
-|-

**James**: Hey welcome to the EIPIP meeting 13, the agenda is in the Ethereum cat herders repository under the issues number 25. This is also being live streamed is it on the Ethereum cat herders live stream. I thank you all for coming, we just had a really good session with the magician's about the EIPIP meetings that I recommend people to watch if you want to know more about the meta process of how we EIPIP came together. Let's just go right into the agenda which I saw the first thing that was there was moved up is the network upgrade process which you had a note on that you wanted to talk about that first, Edson. Do you want to introduce that?

**Edson**: Yeah so it's something that way you started with the status of the the network upgrade process, we never actually finished that before we started talking about  on boarding and updating the EIP template. One thing I wanted to suggest for writing out a new process is like one method of creating solutions which is you’ve  the idea and then you have to validate the idea. Something using creative process is creating multiple different solutions before the call. so for hardfork process there can be multiple different ways in which happen it can happen. once we have a selection of things to choose from we can evaluate them and then break it apart and see what works and why and maybe construction combined solutions to have a better solution that we would have gotten had we just got on with the first thing we thought of.

**James**: I like that.

**Edson**:  So the process is pretty simple it's just instead of just creating one solution we create say 10 different processes we can choose from, quickly present them on the call and then as a group evaluate them to make sense to create one process that we can decide on. 

**James**: I've had one of my mind and I've been I just need to write down but I mean I feel like it would be better if there was more than just myself cuz there are others that are interested in writing out. Let’s say we scheduled for doing it for the next EIPIP meeting, is there some other people that want to draft even just roughed ideas on how it works together?

**Edson**: I can draft one.

**James**: Sweet! We don’t have to work together but come together to discuss, if that makes sense?

**Edson**: That make sense like having prepared beforehand and then discuss it as a group.

**James**: Someone else on the call have a comment.

**Lightclient**: I can also draft some ideas. 

**James**: A couple things I would propose in this  when talking about the network of your process is that we release it before we do the EIP status changes and that'll be its own separate EIP. I think we talked about and cemented more on recently.

**Lightclient**:  why do you think it should come before the changes and the EIP process?

**James**:  because if we remove the hardfork coordination part from the EIP process and then like accepted is no longer a status, then there's an opportunity for community backlash because how would you put things in the mainnet. I think it would be easier to have that defined in some way even if it's not fully defined. I don't think we wanted to find it all out, but we should at least have an EIP that we can point to people saying oh yeah well we separated it and here is the proposal for the other part not just we separated and nothing and there isn't anything.

**Lightclient**: ok

**Hudson**: I think that sounds really good. The separation is needed and we agreed on it previously but having it explicit once we make the changes even when it is in basic form is important. 

**Lightclient**:  I'm not sure if this is the right point to bring the stuff but I was just coming off if you want to talk about another time but I had a comment on the agenda that I feel like there should be a status for a state-of-the-art for mainnet EIP and if we have additional EIP to describe what the network upgrade process is and how it’s not tied to roles of the editors on the repositories then that sort of become like a book keeping duty for the editors to change the EIP status to state-of-the-art on mainnet once it’s like is actually included in the hard fork.
Micah has rebuttal this point that his general view is that the EIP repository is not just focused for Ethereum, it’s more focused for any Ethereum like thing, if another project that they're using EVM, maybe they want to have a finalized EIP that they’re using that’s not ever going to make it on the mainnet Ethereum.  where I am coming from a different point of view where I feel like EIP repositories are for Ethereum and if other parties want to use that then they should develop their own procedures for maintaining what standards they have.

**Hudson**:  yeah I'm with you on that. the every major evm chain has their own version of EIPs, so I don’t   see why anyone would eat from other chains would even want to. No one from other chains has even asked to use our repo, so I don't see the point there.

**Edson**:  I think so from my understanding I'm looking at other like smart contract platforms they actually do use EIP repo but they use like erc's. the other version of erc20 is based on the EIP 20 and then they have a version of non fungible tokens that was taken from the EIP repo, but as far as standards go usually standards are platform-agnostic just another Industries and they exist there to be, like you know like experiments exist and then you can reproduce them kind of some other standards.

**Lightclient**:  It’s difficult with Ethereum, this is different paradigm, if I have an upgrade for tcp  then we can still negotiate our protocol using like an older version tcp potentially.
where with Ethereum, once we make a network upgrade everyone is on, there is no way that O can say that I’m using the old version of Ethereum, that’s just a completely different fork of it. I feel like that should be represented within the process, even if it is just the book keeping, then there is actual selection of the EIPs in the totally separate discussion. 

**James**: The definition of what is Ethereum is what is mainnet, should be kept track of somewhere and how the best way to do that I'm not totally sure but the only think it's worth something should keep on keep on the agenda and we keep bringing up until we figure out the best way to do it.

**Edson**: One thing we can do is say we define the number if you don't exactly know what they will end up being. we could just create a new header and tracks that doesn't compromise that way it doesn't have to be tracks manually. I mean obviously you got the better but you could be could have another section and the EIP website that just tracks mainnet and then I would simplify it for people who are trying to create a new client, so they have somewhere to look at in addition to the yellow paper. 

**Hudson**: Light client made the point that the there would be overhead for editors to go in and merge those changes all the time, so I think that a good in between would be having those hard fork processes as separate EIPs but have them be inactive status so what that means is there never needs to be editor input in order for it to be merged. an active EIP can continually be edited and merged without consent of the editors, is how we can frame it. Right now in active EIP that's not the case because like I think for example I think EIP-1 is an active EIP, like that’s the status. but if we make it so that we can just have these active  EIPs to be able to be changed whenever except for EIP-1, I think that would be okay.

**Edson**:  we had already proposed that so I think EFI we're going to make active, Lightclient was saying, we should just have the status and instead of creating a new EIP.

**Hudson**: Oh! I see.

**James**: Light client talked about how we can make a permission that there are there's a group that could do tags and edit tags and we could make it so there is a group that would be able to edit that field that isn't EIP editors, so that was so if it's bookkeeping then we can have permission for bookkeepers that aren’t EIP editors.

**Lightclient**:  I feel like the overhead on editors is pre-spawn and if we're not doing the network upgrade that often and this really not that mean to go into it should be pretty quick for them to see, okay this is mainnet, this was included in the hard fork yes, we’re going to update the status for that. 

**James**: Yeah!

**Hudson**: Cool!
 
**Lightclient**:  Also I really don't like the idea of the active EIPs, I think EIPs should be static standards and I feel like this is sort of a tooling problem like the reason why we are having this Active EFI is because we don’t have a better place to put it. I don’t see why we can’t have this as part of the EIPs.ethereum  websites where someone is modifying the repo. I don't see any reason why I don't see any difference between having an EFI EIP that’s active all the time vs. having on a website somewhere. Because the network upgrade process is already different from the EIPs process so having an active EIP as a registry is just trying to hack something into a standard process that live outside of it.

**Hudson**: So your proposal is to have a separate repo with the hardfork process, right?

**Lightclient**: I don't really care how it's done, it could be a separate repo it could be a separate folder in the EIPs repo could be formed, whatever. I just don't think that the registry EIPs make a lot of sense. It does feel hacky sometimes, what were you saying Pooja?

**Pooja**: So, if I may break this question into two parts, like there is one part about active status and another part is about EFI. we are talking about EFI EIP to be in the activity status. so I believe that for Active status we are clear that the status is required, not only for EFI EIP but for EIP-1and possibly we would have a couple of more EIPs that may require kind of a status. And for EFI, I think if it is just about maintaining a list, I partially agree to Lightclient’s saying that it can be maintained separately but since this is everything related to protocol, I feel that if we give EFI the status of an EIP that would help people understand more the level of importance of that list and the protocols that are there.

**Edson**: I think that something to consider with EFI, if it is active it won't actually track what's deployed what will track was the point is in EIP that is a hard Fork EIP where it tracks to the hardfork names like Muir Glacier, what EIPs are included. That would be its own EIP which you can look up and see what's I guess what's Cannon to Ethereum and mainnet, and then EFI would  just be tracking what’s currently being discussed.  so things may go into EFI and things may leave EFI.

**Pooja**: Right,  whatever goes under the mainnet deployment that is separately listed in the hardfork meta for that upgrade but EIPs those are currently under consideration, we do not have any specific place to list those EIPs which may or may not be going into the hardfork.

**James**: Listening to Lightclient, I am actually more on the on the page of having it be separated cuz it it would be, so for example I sometimes hesitate making PRs because it inflates. If I make a ton of little changes then I moved us the EIP number of 100 for doing tiny things repo, whereas doing it in a separate repos.  then I would just be a lot more comfortable making changes all the time. Pretty much all but the EIP-1, the Meta EIP is related to the hard fork stuff and the registry things. I don't know I just I think I have maybe been a little bit too having a attitude of we only have what we have and how to work with what we have versus stepping outside of that a little bit and this is what actually making me think? Hudson, what are your thought if you had like a separate Network upgrade repo, is that crazy. 

**Hudson**: No, actually I think that’s a good idea. I think it’s cool also because you can start on that before we even finish the EIPIP stuff .

**James**: Yeah and like I'm hesitant to be an EIP editor cuz I feel like it's kind of a conflict of interest. if I'm doing the network upgrade process I shouldn't also be over the EIP process so then it would be a really easy for me just get started working on the network upgrade stuff, and be an admin there but not in the EIP Part, so their separation.

**Hudson**:  Yeah I like that idea, anyone else have the comments on that? I think Chloe had something on the chat, hi we can have it as a subsection of the it repo but I guess the one issue there would be we would have to give different GitHub level permissions to James potentially mess with other stuff. We don't trust James but he could get malicious suddenly and mess with other stuff within the IP repo you know grow a mustache twirl it in train tracks that whole deal so we don't want them messing around in there :)

**Chloe**: That makes sense.

**James**: I like the idea of separating out explicitly also the signal that they’re separated.

**Hudson**:  Sounds good, I think we should go ahead unless anyone has any objection to doing that. I say we, but that’s really James but if James if you want help obviously to tap me in and other people. I could make a repo, if we need.

**James**: That would make a lot of these easier. That's a good point, thanks for bringing that up. Does that resolve your concerns there?

**Lightclient**: I like it. 

**Hudson**:  I think we can go to the next item, right James? was there anything else on this one?


---
Decision Item | Description
---|---
**13.1** |  Hudson, James  will coordinate to create a separate repo in Ethereum GitHub to place network upgrade related stuff.  


# 2. Onboarding EIP editors
## survey to set expectations of an EIP Editor

Video | [19:15](https://youtu.be/8dxGtomafP4?t=1155)
-|-

**James**: so yeah for the next item onboarding EIP editors, survey. We’ve got about 30 minutes. I'll move through some of these little bit faster survey to set expectations of an EIP editor triaging permissions.

**Edson**:  I created a survey let me bring it up and I'll send a link but it's just three questions I'd like feedback on if I should add or move anything before I send it out ?

**James**: do you want to go for a right now or just have a read through it?

**Edson**: I send the link, I asked what’s expected out of an EIP editor? what is a good requirement for someone to become EIP editor? do you have any recommendations for new EIP editors?

**Chloe**: I'm not sure if it's just me but the first question is showing F?

**Edson**:  it should be correct 

**James**:  I would add how much time do you feel an editor spend a week being an editor.

**Pooja**: Yeah and may be couple of more specific questions. We’re trying to collect information about - when who and how, these three things. if certain criterias are met, we can onboard that person, what are those criterias, we need to define that. we also need to decide on cases when we need to remove any editor, what can be those circumstances, if we can  get this information as well and how is like I mentioned in the previous meeting, also James added that there should be availability for meetings like on a quarterly or monthly, number of hours per month and some general guideline in my mind will be helpful in making it more firm.

**James**: Any other feedback on questions?

**Hudson**:  oh actually hold on I had one and I lost it. I'll talk to you later Edson, I lost it.

**Alita**: I think this covers everything that was discussed everything that was discussed last session, well.



## triaging permission

Video | [22:28](https://youtu.be/8dxGtomafP4?t=10)
-|-

**James**: as far as onboarding with a triage information so let's talk about the triaging permissions group thing. Could you explain what that is Hudson, lightclient?

**Pooja**: The triaging permission here I added coming from the previous meeting where we discuss that possibly you would be looking into adding information to some of the people who are from Ethereum foundation and may be able to kind of label the PRs and that would be helpful for EIP editors. 

**James**: Yeah, and I talked to Hudson  and it  turned into talking to Lightclient and Hudson knows what to do with how to do it.

**Hudson**: If someone can explain me how to do it, I’d be happy to facilitate if we can get like a test repo up. SO, someone can walk me through of what it will do because I'm always reticent to mess with settings on a very important repo.

**lightclient**:  sure so yeah we could do that anytime but the only thing how people do is there going to be able to use the tagging feature to tag information about PR in issues. This will just allow new contributors to do that when you look at the right permission at the repo. You just have to invite someone as collaborator and then I mean right access use data to the triage access.

**Hudson**: Okay, once we figure out who wants to do that I'm happy to do real quick ask the editors if that's okay and then that's so they're not off guard by someone adding tags. And then add persons who should be a tagger. 

**Lightclient**: Sounds good!

**James**:  I think we should call on them the Ethereum bookkeepers.

**Hudson**:  I like tagger cuz it reminds me of people who spray paint illegally.

**James**: That’s pretty good.  Would it be possible for me to be able to add people to that list but not me an EIP editor or can I help with that ?

**Lightclient**: I think it depends on what you're like organizational role in the Ethereum group is on GitHub. I think if you are an owner, you could do that but if you aren't I think you have to have the right access to the EIP repo.

**Hudson**: This is to just do the thing that we were just talking about?

**Lightclient**:  yeah I think someone with the right access to the EIP repo or just people who can add a triage contributor.

**Hudson**: I am a super admin, I can do that.

**James**: I just was wondering if that's something I could help with without becoming having total write access to the repository.

**Hudson**: Oh! Probably not like Lightclient mentioned. 

**James**: Because,  I'd be happy to help. There's a bunch of people here that should be.

**Hudson**: We can just get a list here, that should not be a huge deal. 

**James**: I’ll just collect the list and send them to you.

**Hudson**: Great!

**James**: any last comments on that the triaging permission or group or I'll give it a second for anyone who has final thoughts.


---
Decision Item | Description
---|---
**13.2** |Hudson and Lightclient will look into triaging permisssion. James will help with the list of people to be added.    



# 3. [New EIP validator](https://github.com/lightclient/eipv) and [a suggestion](https://github.com/ethereum-cat-herders/EIPIP/issues/21#issuecomment-651918606) to handle current validator
Video | [26:05](https://youtu.be/8dxGtomafP4?t=1565)
-|-

**James**:   Now we can move on to number 3. This is the new EIP validator and a suggestion to handle current validator. Is that you lightclient?

**Lightclient**:  yeah I don't think there's any major updates from the last meeting I was off for about a week so I'm still working through. I have a list of requirements that I'm trying to get to the validator to reach and if you see anything that you disagree or one other thing that could be added, just ping me or add an issue to that repo and I can have that added. One other thing about that is that a [comment on gitter](https://gitter.im/ethereum/EIPs?at=5f1edfe8a050df43001c0497), I'll just post it here again so people can see. Maybe there's a little bit of confusion between the validator script and the merge bot. Those are two different components. Right now I'm working on the validator that is just going to analyze EIPs to make sure they are conforming to whatever standards we have. Do they have all the section or all the links to other each relative? These sorts of things that editors are currently having to do manually. After that completes, hopefully I can do some more work on the merge bot. Merge bot is what basically manages the state transmission types of changes that it's going to be determined. The author is moved from draft to review and it’s going to automatically accept that rather than forcing like an editor to review it but if they want to obviously remove from review and it's going to finalize then that’s something that they eat better. So all those things are managed by the merge bot. 

**James**: Yeah that's great! I wanted to thank you for looking at that cuz I have wanted some updates to happen but it's just you get someone has to do it like some has to change the code. 

**Lightclient**: I think the merge bot is written by Nick Jhonson. It’s pretty good in general we just need to make some additions to it. The problem with the validator is it just seems to crash in really unhelpful ways and that’s why I am writing it from scratch rather than just working with it. I think the merge bot is a lot more amenable to being updated. 

**Alita**: I’d be happy to help with the merge bot.

**Lightclient**: Great!

**james**: something I'd like the merge bot to be able to do is to have subgroups of permissions. So, if  we had the triagers if we also gave them permission to be able to edit the footer and the mergebot would be able to accept those.

**Lightclient**: That would be cool.  

**James**:  it would be helpful and the tracking things that are currently Ethereum like the whoever is a triagebot making updates to that, it would just be nice if there was another layer of bookkeeping that's possible and have a group that is allowed to make those changes.

**Lightclient**: That’s a really good idea. That’s something I’ve been struggling with because right now, if you have right access to the repo, you can do anything and so this will be a really good way to have to give people a very small amount of access to things. I like that. 

 **James**: Yep. let me pull up the agenda again. any more thoughts or questions on that?

**Pooja**: Just a mention, there is a suggestion from Greg, the link is added on the agenda item. If that could also be considered. 

**James**: I will read it. Is it the link to “a suggestion”

**Pooja**: Right.

**James**:  so I'm seeing a comment from like client 29 days ago, is that the one you're looking at Pooja?

**Pooja**:  It's from Greg, I'm sorry looks like by mistake I put the wrong link, nevermind, I’ll just post the link in the chat. When Lightclient and Alita will be looking into it, may be they could consider that. it's coming up from the previous agenda but we missed to discuss it in the previous meeting. 

I'm sorry it's like “Current validator has a spell check.
It might be good if some things could be handled as warnings -- merge the Draft but let author know there is work to do. Things like wordy abstracts and missing sections.”

**Lightclient**:  yep that's something that the validator that I'm working on,  will do.

**Pooja**: Thank you, I just wanted to bring it to attention. 

**lightclient**: Thanks Pooja!

**James**:  So, is there another point to discuss, Pooja?

**Alita**: Is this like general question, any other points or just for this topic at specific?

**James**: I’d open it up to if you have a comment on something.

**Alita**:  yeah I was considering re-factoring the current EIP-1 in terms of layout I really like the layout of the Improvement proposal from python from JavaScript that you said Edson in the chat.  Regardless, I was thinking of going through refactoring EIP-1 is like a bit of a trap, to give like a different layout cuz the curtain one feels bulky or clunky to me. 

**Edson**: So, I think what Alita is referring to is I posted the process for how JavaScript creates new releases so like ecma 2019-2020 like ES6, on the website I think they have a table with the status and then the description to the status just like in the table format. 

**Alita**: Also, we’ve a bunch of different categories and stuff. Where you could say just the kind of organized columns and say I'm not exactly sure how it would end up looking or if they even feasible. But just in a sense of you can look into a single table and know what are the guidelines, maybe even with spreading out some of the stuff we just so you know Mark down stuff so we can have a linked table that just goes to the document really easily cuz the document is really long so you can have kind of have it nice and spread out. 

**Edson**: The reason I actually brought that up was, this is how they decided to become what is released into Javascript. I was thinking of it as an inspiration for hardfork coordination.
I mean it's up to you guys what you think about reformatting EIP-1. 

**Alota**: Okay, I can also just give it a try, if you don’t like it we don’t have to go with it. I think I’ll be  okay with that too.

**James**:  That sounds good to me, do  you have any thoughts Hudson?

**Hudson**: No, that sounds good.

**James**: better formatting is better. 

**Alita**: Cool!,  I’ll try to get that by the next meeting.

---
Decision Item | Description
---|---
**13.3** |  Lightclient will work on validator and bot stuff.
**13.4** | Alita will look into better formatting of EIP-1. 

# 4. [Standard citation format to the footer of all EIPs](https://github.com/ethereum-cat-herders/EIPIP/issues/25#issuecomment-661506005)

Video | [50:20](https://youtu.be/8dxGtomafP4?t=1000)
-|-

**Pooja**:  James if I may ask for one more item to be covered quickly, I think it can be done quickly. Number 4 - Standard citation format to the footer of all EIPs.

I think this proposal is almost on the final call, so Micah was asking if someone has any objection. That is just about the standardization of footer for all EIPs. People can look at it.

**Edson**: Does it add citations or is it the same citation which one or is the individual ones?

**Pooja**: I think that is about a citation for every EIP that people should be using.

**Edson**: I think it's good. So if it's citations for EIP specifically, I think that is good I think it would be more ethical because if  using work from someone  else copyrighted, I think  you should be referenced or a linked back to the original work. I looked at the PR, it looked like just static text or I wasn't quite sure how is it is it taking part of the section of the EIP and putting in there or is it just one citation for every single EIP? 

**James**: I think it's an edit to the layout the template EIP. So that in the template there would be I don't know.

**Hudson**: I am trying to figure out what the hell this is? I thought it was for the eips.etherum.org.

**Edson**: So this looks like it's for the website for EIPs.

**Hudson**: I might go wrong then. This is what 's confusing me.

**Pooja**: Anyway, I just wanted to bring it to attention so even if people find any thing to be commented on. This is something getting into final stages, feel free to go there and comment on the pull request. 

 **James**: Okay! any other things you'd like covered Pooja in the last minute?

**Pooja**: No, I think I'm done, thank you so much.

Video | [35:25](https://youtu.be/8dxGtomafP4?t=2125)
-|-

**Hudson**: I figured this out, just before we go. This is for EIP.HTML Jekyll layout file. Basically if you go to eips.ethereum.org and you click on the EIP and it gives the header information like the author and stuff and then it gives the content of the EIP. And  at the very bottom all it does  it says please cite this document as IEEE specification for reference formatting to include the author, the EIP number,  the title,  what status it's in and stuff like that and where it's available. So, I think it’s just fine to merge. 

**Edson**: Oh that makes sense, I agree.

**Hudson**: I am just going to put a comment saying this looks good. 

**James**: Thank you!
You all have a great Wednesday, 


---
Decision Item | Description
---|---
**13.7** |  Standard citation format to the footer of all EIPs - It’s just fine to merge. 

# 5. [Constraining the EIP repository scope](https://github.com/ethereum-cat-herders/EIPIP/issues/25#issuecomment-662202920)


Video | [45:05](https://youtu.be/8dxGtomafP4?t=2705)
-|-

**James**: Ha ha ! Okay we got 10 more minutes so let's go over to item 5 Constraining the EIP repository scope.

**Edson**:  I think we already talked about that and hard fork we’re considering creating a new  repo for hard fork coordination to separate that out from EIP repo. Something we can define is an addition to separating stuff defining what’s the scope would be so it would be. We could formally define it as specifications and standards that would include specifications and also include new processes. I guess we would put that in EIP-1 if we were to create a scope.

**James**: And thoughts on what we should call the network upgrade repo? 

**Lightclient**: Upgrade?

**Edson**: Mainnet coordination?

**Hudson**: Which repo again?

**James**: So if we make a network upgrade repo or hardfork coordination repo.

**Edson**: Like Hudson creates a new repo what should it be called?

**Hudson**: Oh that, the one that's in the Ethereum organization. Okay I thought that for some reason I was mixing up the organization repositories.

**James**:  I'd like to open it up to think more about that at the last part of the meeting so I can have some feedback from people before I just run.

**Hudson**: Okay, I'll think about it before the end of the meeting.

**Edson**:  You want to ask like the EF, Hudson, what it should be called?

**Hudson**: Nah! They don’t care. Not that they don’t care about the process I'm just saying as far as naming goes, they don’t care. If a repository needs to be made for whatever official reason, we don't have policies basically it's like to be a good reason that you're making it and it doesn't need to be abandoned but otherwise like naming wise there's not like hard-and-fast policies.

**James**:  Is there anything else left to talk about related making a new repo for the network upgrade process that someone would like to bring up.

**Edson**: Yeah, so we're separating it. We would follow the same rules as the EIP repo. We could divert it but I think just starting it off we just have the same template.

**Hudson**: I don’t think it needs that much structure. I think it should be whoever wants to put stuff in there, have people who want to be in charge of approve it, people like James and there needs to be organization like folder separation, like how the pm repo is separated but like one of them could be like a folder for retrospectives and then there can be a template maybe but that's like similar to eips but it doesn't need to be super super strict unless people want it to be.

**James**: And having an EFI section too.

**Hudson**: Yeah having an EFI subsection, retrospective and maybe not EFI but like what EFI is so like a hardfork policies or stuff like that. I don't know what the wording would be but like that stuff section that has EFI.

**Edson**:  I guess it might be hard to decide what will go into it until we define what the new upgrade process would be. 

**Hudson**: Good point. 

**James**: What I would like to hear from the group here is **what you would like to see in a repository like that** given that we could do whatever we wanted but what would you like to see pie in the sky kind of stuff.  

**Hudson**: I think **we should write up that question in the naming question and post in the telegram post meeting because then we can think about it more** and I'll reply in there.

**James**: That’s a good idea. 

**Pooja**:  One last question on this, this is related to the PR that I’ve already made. If I understand it correct, I’ve to hold on to this one (or two) and when the new repository will be created I’ve to just close and create a new PR over there. And any other suggestion on any of the part of these PRs. I saw one comment from Lightclient that even the template could be an informational one. I am fine with that other that if people have any feedback for this to be added as a PR in the new repository, feel free to add a comment there. 

**James**: Okay, we have about five more minutes the last place I mean review action items from the last meeting.

---
Decision Item | Description
---|---
**13.6** | "What you would like to see in a repository like network upgrade?" We should write up the naming question and post in the telegram, post meeting.


# 6. Discussion on Muir Glacier postmortem report [PR-2809](https://github.com/ethereum/EIPs/pull/2809) and Network upgrade postmortem template [PR-2810](https://github.com/ethereum/EIPs/pull/2810)

Video | [35:25](https://youtu.be/8dxGtomafP4?t=2125)
-|-

**James**:  Moving on to discussion on Muir Glacier postmortem report [PR-2809](https://github.com/ethereum/EIPs/pull/2809)  and network upgrade post-mortem template [PR-2810](https://github.com/ethereum/EIPs/pull/2810)  you want to take that, Pooja?

**Pooja**: So before that there is a comment from Micah, I guess, that is linked to item number 5. So, it's actually related both of them.

**James**:  go ahead Lightclient.

**Lightclient**: I just wanted maybe suggest a different wording than postmortem because I feel like postmortem usually has to do with when something goes wrong and we're writing a summary of what happened where I think this is generally we want to have an EIP that state the stats of the hardfork.

**Pooja**:  Yeah I was more inclined towards marking it as like assessment report of network upgrade or something like that but since traditionally we use the word postmortem, so it was. I’ve no issues in changing the wording.

**Hudson**: I like retrospective, personally.

**James**: That’s a better word for it. 

**Pooja**: Yup, I agree!

**Lightclient**: Are there not already EIPs that are tracking what like the network upgrade will consist of ?

**Edson**: There are, so Micah's suggesting that we just remove all of that from the EIP repo and keep it only standards, which  I think we've already decided in the beginning of the call what we're going to do. We are going to keep, we’re going to create a new repo basically for ... 

**James**: We’re skipping into discussion of Muir Glacier postmortem, so let's finish this number 6 ofcourse and then we'll go back to Micah’s comment. cuz we jumped around a little bit, which is my bad. 
Yeah the retrospective I think it's a better wording in, there's definitely things in your Glacier that went wrong so that's why it was a post-mortem, we can call it a retrospective for all of them that's fine with me.

**Pooja**:  I think, I missed asking this question earlier so changing the name to Network upgrade retrospective of Muir Glacier. There are two proposals, one is for template in general and the other is for Muir Glacier retrospective report. For Muir Glacier, we categorized it as Informational EIP and I documented as that and Micah left some comments over there, feel free to reach them. For this template one  I was wondering should it be information or should it be (if we say it )Meta, it is going to bring a lot of controversy but I was thinking about the EIP 233 which talks about the process to be followed to create a Meta EIP for network upgrade. I was trying to relate.  I'm happy doing either way, looking for some suggestions here. 

**James**: So it sounds like it would be something that fits on hardfork or the Network upgrade repository ?

**Pooja**: Right!

**James**: So, if there was a network upgrade repository that the postmortems on the network upgrade or the retrospectives would fit there. Which I think also solves Micah's concern.

**Hudson**:  Yeah I think it definitely alleviates  a lot for sure.

**Lightclient**: I don't know, I feel like this fits well in the EIPs repository. It doesn’t have to do with the governance at all. This is just purely informational it seems like the exact reason to have an informational EIP that states something that happened.

**Hudson**: Yeah but I think,  I guess the fewer EIPs that are non-standard, the better, is how I like to look at it but that's like more of a personal opinion, I guess.

**lightclient**:  You're staying non-standard as they are not standard?

**Hudson**: No, they are not standards, like with an ‘s’.

**Lightclient**:  I kind of think that we should have more informational EIPs and maybe this isn't the right kind but I feel like Peter has been posting some of the stuff like implementation of Geth, there’s been a lot of talk about how the databases are implemented. I feel like those are things that could be written as Informational EIPs. They are not consensus requirements but they are something to help future developers understand decisions.

**Pooja**: I am totally on that, and that’s the  argument I was trying to give in one of the comments to this PR. According to EIP-1 we have theses three different categories of EIP,  like meta, standard, and  information. Informational section in my mind is created to provide more information and that  is a placeholder for important information and community reference. In my mind I don't find it wrong to be placed in EIP repository but if people agree to have everything related to network upgrade separately, I don’t mind that either. 

**Lightclient**:  I think Micah’s point of view is that he's coming from this place where he believes that the EIPs repository should be generic to the platform and so he doesn't think that should be network upgrade because he believes that there could be finalized EIPs that are not ever going to be used by the Ethereum mainnet, it might be used by a different project. My point of view is that that shouldn’t be a case. This is the Ethereum Improvement Proposal repository, we should be focused on Ethereum related things and so, one of the most important parts about Ethereum is what is on mainnet and information about mainnet. I definitely think the Governance process about what goes to mainnet should be separate from this but I feel like we should have a singular focus on our Ethereum. 

**hudson**: Yeah so that I could go either way. It could be in the hardfork one that the James is creating or it could be in the EIPs but for now since this is already a pull request in the EIPs repo and I just looked over a little more closely and it’s purely informational. well I can see these eventually becoming political as they get more detail, is something I just thought about. So like if someone screws up and then we like the discovery of the problem this client broke this because we have had cases in the past including a pretty major bug where a precompile was incorrectly or there was a idiosyncrasy with a precompile which is a really polite way of saying one of the two clients messed up reading the spec, we don't know which client it was because there was disagreement about what the specs said based on their interpretation of it. So then there was this huge thing and later Yoichi who used to be more active in the EIPs repository wrote up a really long long like article that like a GitHub thing that explained you know if anyone was at fault like who was kind of fault, who wasn't in it. it became a whole deal. so I can see these in the future becoming more controversial and then the not fitting in the EIP Repository.

**James**:  Yep I'm in, I assume where I can see them both, I see both sides, so I don’t want to push them in either direction. 

**Hudson**: We could **take more time to think about this and talk it on the telegram and then in the next meeting make a more final decision**, I guess.

**James**:  yeah that's a good idea.

**Hudson**: Yeah I mean obviously if there’s other comments, I don’t want to stop anybody. 

**Edson**: Yeah I mean there's been a big push to keep the EIP repo purely technical and remove politics whenever possible, it's just some feedback that I’ve been seeing.

**Hudson**: There might be a time when politics need to be involved in a report like this especially if it's going to continuously be written by groups that are not editors and people that are not are like groups like The Cat herders and James and other people who have similar groupings to James's position and what the cat herders do.

**James**: So you’ll just go send all that all the politics and controversy to me. 
**Hudson**: Shipping on your way, one way UPS. 

---
Decision Item | Description
---|---
**13.5** | Take more time to think about this and talk it on the telegram and then in the next meeting make a more final decision on wether to keep it in EIP repo or a separate repo to be created for network upgrade related EIPs. 

# 7. [Explore the idea of working groups](https://github.com/ethereum-cat-herders/EIPIP/issues/25#issuecomment-664579942)

(No discussion)

# 8. [Clarifications for how a precompile address is decided.](https://ethereum-magicians.org/t/proposed-process-for-assigning-opcode-address/4302/3)

(No discussion)

# 9. Discuss the EIP-1 Brainstorming Document
(No discussion)

# 10. Review action items from [previous meeting](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20012.md)

Video | [52:45](https://youtu.be/8dxGtomafP4?t=2340)
-|-

**James**: Great! I’ll review the action Items.

Decision Item | Description | Status
---|---|--
**12.1** | Edson will make a survey to the current editors on the expectations from an editor (time-commitment, qualifications) | He did that.
**12.2** | James wil look into the necessary permissions and how to setup users with triaging capabilities | I talked to Hudson and we talked about it today.
**12.3** | A process for removing editors and criteria for removing editors is a future item to discuss | We did not discuss that today, so we should add that to discuss at a later time. 
**12.4** | Link to the live EFI document through EIP 1 rather than continuously updating EIP 1; EIP 1 can be used as a hub for statuses instead. | James to having a repository for network upgrade coordination. 
**12.5** | Remove emergency comms from EIP IP agenda item until it becomes pertinent | We did that. 

Thank you, everybody!

---

# Annex

## Attendees

- Alita M.
- Brent Allsop
- Edson Ayllon
- Hudson Jameson
- James Hancock
- Lightclient
- Chloethdev
- Pooja Ranjan
- Jaye H. 

## Zoom chat

00:06:54	Pooja Ranjan:	https://github.com/ethereum-cat-herders/EIPIP/issues/25

00:13:23	Jaye Harrill (she/her):	Dropping off, I’ll catch-up via YouTube.

00:22:08	Chloethedev.eth:	I see both points. Could the EIP be set to whatever the standard is for the normal repository and then link to another (new) repository that would stay active? Would that satisfy both issues?

00:22:56	Chloethedev.eth:	Still show the importance by having it in EIP repo like Pooja was saying?

00:26:37	Edson Ayllon:	https://forms.gle/gEnjbnxQhhHdVdWQ6

00:33:34	lightclient:	https://gitter.im/ethereum/EIPs?at=5f1edfe8a050df43001c0497

00:38:23	lightclient:	https://github.com/ethereum-cat-herders/EIPIP/issues/23#issuecomment-657610099

00:38:28	lightclient:	greg's comment ^

00:57:48	James Hancock:	https://github.com/ethereum/EIPs/pull/2738/files

## Next Call

Wednesday, Aug 12, 2020, 15:00 UTC.
