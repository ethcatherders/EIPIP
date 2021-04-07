# EIPIP Meeting 29 Notes
## Meeting Date/Time: Wednesday 24 March at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/57)
### [Audio/Video of the meeting](https://youtu.be/CD3LCpeQX8w)
### Moderator: Pooja Ranjan
### Notes: Alita Moore

----
## DECISION ITEMS

**DECISION 1**: CFI (draft), Devnet (review), and the main-net phase in last call; EIPs will be marked as final only if it is deployed on the mainnet 

**DECISION 2**: split editorship between ERC and EIP, split out to seperate repos

**DECISION 3**: Allow bot to fail if it was going to merge (to be turned on at a later date)

**DECISION 4**: Define JSON RPC in specs repo

**DECISION 5**: Create a new repository that's just for interfaces instead of migrating to eth2 specs repo

## ACTION ITEMS

**ACTION 1**: decide on numbering system between ERC and EIP

**ACTION 2**: Create issue on EIPIP repo to seperate ERC and EIP repos -- with description for EIP bot requirements

----

# 1. Network upgrade process review
Video | [0:20](https://youtu.be/CD3LCpeQX8w?t=20)

**Pooja** - welcome to eipip meeting 29. the first item on the agenda is network upgrade process review and some proposed changes to the status of core eip uh this item we discussed in the previous meeting and um with the present model uh i'm trying to propose some changes in the status of core eip so in the last meeting i shared this diagram that is uh that is a link is provided in the agenda itself that suggests that if we can have the change of the status for mainnet phase and make the testing green light or public test net to be in review or the last call status 

**Tim** - so basically just to make sure i understand when something is being tested that it absolutely has to be in review or last call right 

**Pooja** - right so the last uh meeting we discussed that generally the last call is suggested to be for 14 days only so there were one con there was one correction that i recommended that instead of having the last call for 14 days we can mention it as a minimum of 14 days that was point number one and the point number two when we are sending it on public test net then we mention it to be on the last call and until uh it reaches on the public test net let it be in review status 

**Tim** - i think that makes a lot of sense 

**Pooja** - and um and eip will be considered final only if it is deployed on mainnet for the proposals which are actually being considered to be deployed on the mainnet via network upgrade because the standardization process for eip and network are different now so there can be some core proposals who would be reaching to the final status but may not be ever being deployed on the main net so we wanted to keep this on agenda for this meeting as well so that people should know about it and if anyone has any other thought feel free to share 

**Micah** - just to reiterate again this is not not an eip issue this is a core dev issue 

**Pooja** - right but what uh i'm suggesting here is like if we are planning something and document it we can at least reach out to the core devs or maybe the author of the eip uh suggesting that this is this is the process and if we go by this that would be like really helpful for everybody nobody can say that we weren't aware that the proposal is in this status and it is going in the upgrade and something like that that happened for one particular proposal

**Micah** - yeah i do think that taking off my eip editor hat putting on a wannabe core dev hat i think that anything that is um proposed for like for mainnet should be in review by the time it gets there like we don't want eips that are still under active development by their authors to be proposed like you should be confident enough in your your eip that you think you're done at least you might not actually be done but you think you're done before you bring it to the core devs and waste their time with it 

**Pooja** - right so uh by bringing it to the core devs do you mean the consider for inclusion phase because uh my understanding is even if it is in draft for computer consider for inclusion it must be in review when it is approved if a coder says that okay this is general consensus we can think about it then it should be in review or 

**Micah** - i mean it's fine i'm okay i'm personally okay with cfi being in draft because mainly just because we don't want people to waste a huge amount of time before they get just like a general consensus from the dev core devs saying yes this is an interesting thing to us and to me cfi is basically the core dev saying yes this this is interesting to us go go finish it now and come back to us when it's ready for us to look at for implementation right and so for cfi i'm okay with draft personally just again like if the core devs of saying no we're not interested i don't want people to waste a huge amount of time getting something to review which requires getting past micah which is a huge pain in the ass um if this is going to be immediately rejected by the core devs it would be nice if people get just like uh like there's a bunch of core eips you know where people craft them and then they go through a huge amount of effort to get it past me and then they finally get it past me and then they take the core devs and the core devs immediately just shoot it down and say no we're never doing that and this is just a big waste of time for that that author 

**Pooja** - right and tim has suggested here in the chat cfi for draft network upgrade for review and test net block chosen for the last call yes that is exactly what we are planning here

**Hudson** - that sounds good to me uh by the way sorry about that i actually can be here today everyone was very quick so i can make it

Decision 1

    cfi for draft, network upgrade for review, and the main-net phase in last call; EIPs will be marked as final only if it is deployed on the mainnet 

**Pooja** - thank you for joining hudson okay uh so uh let's let's keep it uh for the notes taker uh uh the suggestions here uh cfi for draft network upgrade for review and test net block chosen that is actually the main net phase um in the last call and it will be marked as final only on um when it is deployed on the main net and we will share this information with the coder as well hope there should not be any objection 

# 2. Should ERCs be moved to a separate repo?
Video | [6:35](https://youtu.be/CD3LCpeQX8w?t=395)

**Pooja** - okay moving on the next item on the agenda is should erc's be moved to a separate repo so there has been this discussion around eips and ercs should be in different repos we discussed it briefly in the previous meeting and i saw some conversation on the ethereum discord channel as well so uh maybe lightclient or micah if anyone would like to take a lead and talk more about it

**Lightclient** - i can say something briefly i posted on the discord channel uh based on the conversation for the last eipip meeting we kind of talked about how ercs just don't fit very well within the eip repository and there's a lot of disjoint responsibilities over there those eips you know i personally feel like i'm not a very good person to to be editing and reviewing a lot of the ercs and i think there's people in the community who would be really great at that but they're really not suited very well for you know review core aps you know for that reason in other reasons you know we talked in the last meeting about what if we had what if we took the ercs and we put them in their own separate repository and i had just posted on discord asking like what does it take who whose approval do we need to get to make that happen i'm happy to do the work i i don't think it's gonna be too difficult uh to me the biggest question mark would be there's a lot of permalinks out there that point to the you know the github pages we can redirect the eips.ethereum.org website all the ercs can be redirected to their correct page but we can't redirect the github page my proposal to resolve that is just replace every erc with uh a stub that just says this has been moved to the erc repository here's the new link and so that would just add an extra uh level of indirection for anyone trying to access it directly on github i don't think that's like a showstopper 

**Micah** - what's the proposed numbering system 

**Lightclient** - i think the numbering system would you know we'd have to have some way of and you know my look the lowest tech that i can think of is just a google sheet that we share with editors and that's going to increase the burden a little bit because instead of just looking at the pr number we would have to go look at the sheet to see the next available number but i think that i don't want to do something where we like multiply ercs by 10. i think that that's that that that's just asking for problems in the future but uh i think it's worth it in the long run just to make it a little bit harder to assign a number because it's going to be a lot less work for core editors uh who don't have to review ercs and then we can really bring on more people to edit ercs and actually build you know kind of a community around just that aspect because there's a lot of people who are only interested in the application level of ethereum and they have no interest in eips at all 

**Micah** - i suppose once we create the if we migrate the ips into a similar file structure then if someone tries to create a pr and create a file with a matching name it'll immediately get flagged and blocked so we don't even need to keep a separate document i think right

**Lightclient** - if the bot had a like an overview of both repos 

**Micah** - no i mean like if if we take erc20 for example and just copy it or cut it out of the eips repo paste it in the erc's repo sure there is now an erc20 in that repo and so if someone tries to create erc20 it'll just immediately show up as they're deleting the old one which is very obvious 

**Lightclient** - sure i'm more worried about assigning new numbers though because there's no way to know if you know 3502 has been assigned as an erc yet 

**Micah** - uh right so as soon as they um as soon as someone like editor comes in and says oh your pr number is 20. so use erc20 the user will then try to create erc20 realize conflict send a message to the auth the editor saying hey there's a conflict what should i do no the editor then just says i'll use 19 instead or whatever 

**Lightclient** - if it's published in the erc repo there would be no corresponding file on eip repo 

**Tim** - yeah can we just add like some padding can we just say i don't know you add like 5 000 to the number so if it's pr20 then you're erc or i don't know 5 000 might be too low 

**Lightclient** - but i just feel like we're not gonna you know leave the eip system in five thousand i mean that's yeah i mean that's only five thousand eips away that's 

**Micah** - are you are you worried about there being an eip 5000 and an erc 5000 to me that seems fine um you don't need them to be actually exclusive 

**Lightclient** - i mean if we don't need to be mutually exclusive why not start erc's over is that where you're playing yeah because 

**Tim** - but then you're going to conflict with the current ercs i think if you take a number that's bigger than the last eip right now then you you make sure that there's no conflict right 

**Micah** - yes but the the total number of ercs that are actually like draft or higher is on the order of maybe hundreds i think i'll check while i talk but i think that long term you're going to end up with more simplicity if you just continue to use the pr number numbering scheme and you just deal with those 100 or so conflicts if they come up and keep in mind that there's a very good chance they won't come up because you know every single pr increments that number but only a small handful of those are actually new ercs and so um i think that you'll just end up with a small number of conflicts like so when someone comes along and does pr20 if pr20 happens to be a new erc not someone updating an existing rc then they'd have a conflict and then we'd do a one-off fix for that one say i'll use 19 instead 19 is free 

**Pooja** - i have a suggestion i don't know how much it will be helpful but i was wondering like not all pr number is an eip so um what if we add an additional step for the ercs just asking them to create a pull request stating that i have requested for i have created a pull request in erc repository for whatever proposal he or she has and just refer the pull request number here and use that as erc number there so in that way there is never going to be a conflict and it will not disturb any of the process other than it will be an additional step for an author to just create one issue for request here at the eip github repository 

**Lightclient** - i would prefer that the eap like if we were going to separate them i would rather have it truly separated but i do kind of like the idea where i mean we can artificially bump a repository up to a specific you know issue or request number and you know theoretically we could have a repo ethereum slash um numbers i don't know what you would call that but you know you could just say if you're going to open an erc or eip you have to go open an issue to you know claim a number that kind of removes the burden from the editors i don't really like the idea of going allowing people to you know start claiming like single and double-digit erc numbers that were eips and i just i don't really like the idea of having a erc conflict with an eip number that to me just seems like we're asking for it you know especially because this is this is something that's going to be changed and it's already difficult enough to convey changes in the eip process to the broader community and so people start seeing oh wow there is you know eip 3102 and there's erc 3102 i think that's just asking for confusion 

**Hudson** - yeah and like the the precedent we've set is that ercs are eips up to now so changing that precedent would be a task it's not impossible but like maybe taking this in steps so like the first step would be finding someone who even wants to be an erc editor and then have them start doing erc editing in the main repo and then getting the resources meaning funding and people's time to split out the repo that would be a whole different discussion so i think i guess all that to say we're kind of getting into the weeds today when really the main decisions to be made are maybe if it's worth it to split it out in the first place like from the repo because i'm not convinced that they shouldn't all be in one repo um but i guess what's the benefit of splitting it out into two repos just like clarity 

**Bret** - one additional thought i had in since we're talking about splitting ercs from core dev uh eips um is there's all my understanding is that micah and lightclient get harassed with a bunch of people trying to do stuff that isn't related to either one of those and if we it and the key is we need an editor for erc's and we and and and maybe we could have a miscellaneous so we have three different locations we have a miscellaneous for all the other stuff and we have and and maybe we could just say we want to push in that direction and we want to find an editor for miscellaneous stuff and we want to find the editor for ercs but eips are just for cores anyway just a thought because if i i believe you instead of telling people what not to do tell them a better thing to do so if people that there's a lot of people that want to do that if they had a place where they could put stuff that would take some pressure off the editors i would think 

**Hudson** - yeah a lot of this is about taking pressure off the editors who aren't like either aren't equipped or don't want to handle ercs like they'd rather do eips and so if that's one of the main goals and sorry about the background noise by the way if that's one of the main goals i don't know if we should split it out at all right now or maybe just decide that later 

**Lightclient** - i think that it's it is more than just making things easier for editors i also really think that it can help increase community participation there's so few people in the ethereum community who have the overview where they can understand both ercs and core eips it didn't generally tens of people you know are at dap level developers or they're kind of core level developers and there's a lot of noise in the eip repository with both of these things and being an editor having notifications on seeing the noise it's hot can be tough for me to keep up even though this is like a responsibility that i signed up for if i was just a community member who wanted to follow the latest and greatest core developments the latest and greatest you know erc developments that would be hard and i think that if we split it up that would generally just allow this kind of natural boundary that already exists for people to like really begin to be more involved in that process without actually having a role just you know tracking what's happening and uh you know being a part of the um the governance process on both of those sides 

**Micah** - just to get it out there so there's only a few hundred i would say total eips and a portion of that is erc's and so when it comes to numbering schemes if we just use the pr number like we do with the erps that use it for ercs as well except for be the erc repo it will be very rare that we actually run into a conflict and when we do we can just handle that conflict individually and i think overall that will be the least amount of work for erc editors in general um just because conflicts are rare and when they happen they're very easy to resolve and that way the numbering scheme for the common case is very simple let's just use the pr number like we do now 

**Hudson** - so you're saying there we will they will start with erc one and then skip 20.

**Micah** - yeah so we'll start with the erc1 and there's like a 99 chance we'll skip 20 naturally because that's just how the numbering system works it is not uh incrementally increasing like eip you know 20 exists and 55 exists and nothing in between the two exists um as yeah we start with erc one and then there would be an erc you know maybe 35 and maybe erc 72 assuming the pattern is similar to eips and every now and then there'll be a conflict but it'll be very rare i'm guessing one or two total 

**Hudson** - i think it's going to be confusing because generally people will associate lower number with earlier in the history of ethereum so if there's erc 5 they're going to think it came before erc20 etc so like if there's a standard that like improves on erc20 or replaces the erc20 but it was erc7 i i just can see most people getting confused 

**Pooja** - I would agree to that so if we have to start this like we should be starting from this point onwards not going to the back number that would be my first suggestion and uh using the same like you know getting the pr number would be a better idea it would not ever let us to any kind of conflict because it's just an request that is there an empty kind of just mentioning that there is a relevant erc that people can go and refer to if they want to

**Micah** - so the other option is we could just write a little bot that just turns through the first 5000 issue numbers and do github repo 

**Lightclient** - the problem is then you still have this issue where you you can end up with er eips and ercs with duplicate numbers and so i really feel like they should be mutually exclusive uh.. i i just think that we've already said this precedent that ercs and eips are kind of very similar they're in the same repos they have different numbers and it's going to be hard enough to try and tell everyone hey this is a totally different thing now ercs are their own thing there's you know maybe in the future they can have the numbers could conflict but i just think in the in the beginning i really don't think it's that much extra work there's you know i think there's two good ways to do it we can either have a spreadsheet where an editor you know spends 30 seconds and goes and puts the number in when they assign it or we can have a canonical repo ethereum slash numbers where people can create an issue and they post the link to the issue and say this is my eip number because i went and this was the next number i got in the repository and and so i think there are good ways to solve this issue of you know making them mutually exclusive it just only puts a small amount of extra burden on the process and it creates it makes things so much simpler for people who are trying to follow it without knowing every detail 

**Tim** - so could maybe a way to do that be like you split the repo but within the same actual github repository so you create two different top level folders one for eip and one for ercs and then at the top level you maintain a list of numbers so like at least this way yeah they're always in sync

**Micah** - the problem with that is you don't solve the one of the bigger problems which is email notifications like i i'm currently subscribed to all the eips repo so that way anytime someone comes in with a new um pr i notice it and if we add them in one then i still get all the erc ones and on the escalator it still gets all the eip ones 

**Tim** - is there a way we could automate this list that like keep tracks of the different it's almost like whenever there's a merged pr you want to update the list with that number or something 

**Micah** - i mean you can set up like a github um github action that fires web hook anytime a pr is made and you can even set it up to automatically do the numbering so get the humans out of the numbering system of course that requires engineering effort and that is something we are very short on in this group

**Lightclient** - yeah i mean definitely we can have bots do this this is a very simple thing to have written obviously it has to be written i don't think we have the time to specifically do it at this exact moment but that's what i'm saying i think that you know starting with a spreadsheet and then eventually having someone go in and turn that into a part of the merge bot that would be back to the same level of effort required or less 

**Pooja** - i don't know if github repository supports uh with the help of label i mean like if we start labeling it as erc in the beginning if somebody is creating a pull request and that helps like um with the notification that you're receiving i'm not sure that by the way 

**Lightclient** - it doesn't help with the notification unfortunately 

Decision 2

  split editorship between ERC and EIP, split out to seperate repos

Action 1

  decide on numbering system between ERC and EIP

**Hudson** - so just to go over what we've kind of decided we definitely want to split editorship into eip versus erc um we are heavily leaning if not pretty much decided they should be split out by repo what we're stuck on is once they're split out by repo how to do the numbering is that is that kind of a good summary.. okay so i think a better option would be for people to come up with proposals when we make an issue in the eipip repo or like uh where's the stuff discussed there's an eipip repo yeah so um i can make an issue for that and put it in here uh it's like ethereum dash cat dash herder slash e-i-p-i-p and github um i think that's good and then we can move on to other stuff unless someone wants has like a final thoughts on this 

**Micah** - only final thought is if we're going to do this for erc should we also do it for interface and network or not ercs are the biggest problem but the same basically the essentially the exact same problem exists for all the different categories it's just much more muted for the other ones 

**Pooja** - that was there in my mind thanks for putting it um i think 

**Hudon** - it's we should try out with erc's and learn from that and then split it out further if well i don't know maybe doing it all at once would work but i don't think there's very many how many interface and networking eips are there i don't think there's that many that 

**Tim** - it would we yeah and i think we want to keep the networking alongside the core eaps because it is like the same set of folks who end up reviewing and implementing both 

**Micah** - yeah i agree i tend to agree with that core and networking are very tightly related interface is a different set of people so like metamask and basically all the wallet providers care a whole lot about the interface section as do core developers as do dap developers and so um interface is like it's a very appropriate name it is the interface between all three layers and they care about all three very much um so maybe that one pulling it out just again so we can have people can don't have to get the core eips if they just care about interface stuff 

**Lightclient** - sure i think erc's are a good place to start the number of non-erc or core eips is incredibly small 

Action 2

  Create issue on EIPIP repo to seperate ERC and EIP repos -- with description for EIP bot requirements

**Micah** - i'm good with starting with erc and see how it goes 

**Pooja** - so i think i'd say i think i think that was background noise i think uh um we have to create an issue on eipip get our repository stating that we would like to start with erc to be in a separate repository and then maybe i don't know if alita just mentioned in the chat if we can have some documentation of the requirement for both bot that we discussed if that has to be done with the help of bot 

**Hudson** - um oh did we did anyone discuss about losing like historical hit like history between behind like the older eips and stuff would we just close all the previous prs and issues and they'd still be in the eip repo or would they be deleted 

**Lightclient** - they would definitely still be there i assume that the discussion threads for old ercs if they're pointed to issues will probably just you know stay as issues in the eip repository and then you know over time there'll just be so few that are actually actively discussed

**Hudson** - got it okay 

**Pooja** - okay so does it make sense to bring it back in the next meeting to discuss further on this topic do we keep it [yeah]

# 3. Progress on EIP GitHub repo action bot.
Video | [29:37](https://youtu.be/CD3LCpeQX8w?t=1777)

**Pooja** - so moving ahead uh the next item on the agenda is progress on the eip github ripple action part uh i believe alita is working on that and there is an issue uh for collecting some uh you know requirements for the bot that is issue number 59 in the same repository alita if you would like to provide some more update on it 

**Alita** - sure so right now um the bot is waiting on i forget who exactly but basically we're waiting on transferring the exact bot to a ethereum controlled repo um it's currently in a private repo um the actual merge bot like where it's used um on the main eip repo is not merged yet um i think that there's a small change that needs to be made um and we're still trying to figure out like manual stuff um for the eip bot itself the from stuff we discussed last week um our last meeting um i have implemented like the testing framework for it um and then i have created a new issue for okay so i have interfaced like the eip merge bot in its own repo so that way we can more easily managed it i have built the test framework and i have created a issue for collecting information on more features um required for the bot i think that sums it up does anybody have any other comments or questions?

**Hudson** - uh great job and um did we i don't see it written anywhere how much the cad herders are paying for this and i want that like down somewhere so we know how much to pay you for your work uh is that somewhere 

**Lightclient** - 200,000

**Alita** - yeah it was like a million [Laughter] no no i actually created a funding um request in the cat herders and that references the video that um like got me started on it which was seven thousand usd; um so and then for future funding um like because because i'm considering getting it up and running with like the features that were initially requested and like transferring over including the testing included in the 7000; um just because i don't know i want to make sure it's good um but any future uh like features and stuff i will make um like the idea behind the requirements document is to get everything in one place so then we can create a like a thorough proposal for funding um to get those in place as well 

**Pooja** - there was an issue actually it was a response somewhere in the eip github repository itself uh in which we kind of calculated like how much the work is required and how much should be the funding maybe i would share that link but yes that was somewhere around 7 000 so yeah that's fine 

**Hudson** - um other than that um do you need help getting it into a neutral repo like ethereum

**Alita** - yeah you could transfer over and then um well actually i have two requests can i please be made a um contributor to the eips repo because it would be nice to be able to branch off of that because i'm probably making changes to the um bot once once it's put in um like if i want to change the version or something on it um and then but yeah so then we also need to transfer the current bot which is alita-moore/EIP-bot which i can link um that one needs to be moved to an ethereum control repo which i would like to be made an admin on so that way i can have some like ease of editing stuff 

**Hudson** - that all sounds good to me um so just to be clear we don't have contributor access on the eips repo the three roles we have are read write and admin um because we are on an old github plan that's cheaper for us so would you need write permissions to read clone and push to the repository and manage issues in pull requests or would you need admin to also change settings 

**Alita** - i don't know if i need admin 

**Micah** - just write 

**Hudson** - okay put your username in the zoom chat if you're not on mobile and i'll make you write permissions right now and then message me on discord and we'll in the next few days uh get that transferred 

**Pooja** - just one last comment from the camera side like uh uh do let us know whenever everything is done like when bot is merged and when we have to make the payments so just uh gives us a heads-up um

**Alita** - i mean i submitted the funding request um the bot is like i guess mostly done i have some like polishing to do i don't know if we want to wait for that to be done um i know i'm waiting on a final review from micah um like essentially it's kind of a continuous process so i don't know if there's if there's a clear line in the sand um like in my opinion it feels like the initial task was done and i'm just polishing right now um what do you think or you all think 

**Hudson** - my opinion would be after micah's final review if that if he says it's all good and there's no last-minute fixes that were part of the initial set of either requirements or expectations then i'd say we can pay out then with the expectation that for we don't pay anymore for you actually installing it because i think that was part of the initial stuff right

**Alita** - oh yeah for sure, um yeah 

**Hudson** - okay then yeah that sounds good after micah gives the okay i say we can we can fund it what do you think micah 

**Micah** - the last i looked i think i was we were waiting on that manual trigger that we found getting that set up and there is something else i think it was mentioned in the issue um are those two things set up now like we have the ability to manually trigger and what was the other one 

**Alita** - speaking of which the manual trigger that you mentioned i don't necessarily know that's gonna work i'm trying to find a workaround for it um but 

**Micah** - what's the problem, what's the gist of the problem like the one sentence version 

**Alita** - you can only run it on a branch not a pr

**Micah** - i think oh but this particular bot needs to know the pr because it's gonna merge i see well that's annoying um okay and the do you remember what the other one was 

**Alita** - um let me read your message here i thought there i thought there was one other thing oh yeah that the other one's done it was talking about not referencing master so um yeah the bot on its own separate repo has a versioning system and um it's using the version so that's easy 

**Micah** - uh just send an at mention me in the pr so i can it gets added to my inbox which will cause me to then look at it and i can do it final review

**Alita** - done um and then as far as the the manual thing goes i mean there are definitely solutions it's kind of hard to do that async so maybe we can have a call or something like today or tomorrow 

**Micah** - and what i'd what i ultimately really like is a way that we can um dip our feet in with it and migrate to it slowly and so we can basically test to make sure it's doing what we think it should do and then once we've validated that it's doing everything we think it should do in the production environment then we flip it flip the switch and turn the old one off the new one on i'm just a bit hesitant to have them both running specifically because my current process is if i see the bot auto merge something i completely ignore the email from github and so if the bot goes crazy and just auto merges everything just as a pathological example it may be a very long time before anyone notices 

**Alita** - okay um i will implement some way of do manual like the one okay maybe what if we just 

Decision 3

    Allow bot to fail if it was going to merge (to be turned on at a later date)

**Micah** - what if we just have the bot set up to always run but take away its ability to merge and then just have it when it runs it will just do like a green red or yellow in the ci section like you know how the ci at the bottom says green green red or yellow if we can just have it go green or red then i'll at least see did the the bot think it wanted to merge or to think that it shouldn't merge then we can do run that for like a week or two and then if it looks like it's correctly going green and correctly going red at the appropriate times then we'll flip the switch and if and actually enable merges and if not we can fix whatever bugs 

**Alita** - that sounds great to me 

**Pooja** - do we need any kind of conclusion for this any kind of what documentation 

**Micah** - i mean documentation is always nice but at the same time um i would rather Alita spend her time on more useful tasks given there's like maybe three people that actually ever use it 

**Pooja** - yeah that's fine i i was just wondering like if it if it is needed at all 

**Alita** - um so there is some documentation on the bot like the code itself um i mean it's well commented and everything i fully intend on doing um like a full test suite for it just because i mean i want it to be scalable but um like essentially what kind of documentation are you referencing 

**Pooja** - i know i was just mentioning that if any kind of documentation is needed for people to refer um maybe in future if they have to fix anything or something like that 

**Alita** - yeah the bot itself is written in a way that's readable um with clear documentation on contributing 

**Pooja** - so i think that's good oh cool okay uh so in the sense of time should we move ahead with next agenda if everyone is funnier okay 

# 4. The EIP standardization process
Video | [40:57](https://youtu.be/CD3LCpeQX8w?t=2457)

**Pooja** - uh the next item is the the eip standardization process uh so we had this um meeting for eip1474 or that was basically for rpc standards for ethereum um jason rpc standards and two things uh were proposed in the meeting one like this standard this proposal particularly is never going to achieve a final status because there is always going to be room for some improvement so should it follow the normal eip standardization process or should it be granted some kind of special uh access or maybe you know um going with a special status maybe living or there was another proposal of converting it to a meta eip because it would be kind of template for every client to implement in the way they want to because not every client's implementation for json rpc standards are exactly the same so it's difficult to document that in the proposal as an implementation section and people were looking for thought of eip editors on this like how do they want to proceed with this particular proposal 

**Micah** - my personal preference is take this opportunity to try out um a specification system closer to like what eth2 has where we have a repository that defines a specification and then pr's to that repository is the change control process and then when a pr is merged the repository just shows the latest version um i feel like that works really well for documents that tend to live over time that being said i don't actually think the json rpc should be a living document at all like i very much think that when you deploy or when you standardize on something you should really not be changing that standard on people like that's how you end up with the browser hell of circa year 2000 to 2015. like standards should stick around and be very very rigid because that's what makes them useful is the um so i have two minds on it one i think there are much better systems for living documents than the ap process and i encourage people to try them and two i don't actually think this is necessarily a good use case for a living document and i know those two things conflict like 100

**Pooja** - so the meta question here is like this proposal or proposals like this should it be a part of erp at all 

**Micah** - so json rpc specifically definitely needs to be specced out somewhere like it needs to be documented currently it's documented in five different places and is documented poorly and the people who own the documentation are not necessarily the people who care about the the specification and so um it's not great the current situation 1474 if i remember correctly tries to move all of it into an eip kind of wholesale at once which i have spoken out weekly on uh like loosely against that saying that it should really be multiple eips let me verify that one four seven four isn't back to one thing enough

**Lightclient** - what's the canonical place for the rpc standard right now 

**Micah** - yeah so i think if you're gonna use the eips repo i think the proper way to use the eips repo for this sort of thing would be to have each endpoint each method be a separate eip and then maybe any eip for the overarching this is how ethereum json rpc is defined i don't think trying to have this one monolithic eip that then just mutates over time does anybody any good because then you have immutable standard and mutable standards are not standards so therefore they're not useful as a standard um again i would this is a good up i i still think this is a good opportunity though to try other things besides eaps like there are currently there's basically other than this eip there's no work that's been done historically or very little on standardizing interfaces there's some but not a whole lot and so unlike core eips moving out of the earpiece repo i don't think would be hard and so i'm going you know trying something new like a like eth2 is doing with a github repo that it just has prs against it maybe is a better solution 

**Pooja** - so we are now joined by eric swan so eric we were discussing about the proposal excellent 

**Eric** - sounds uh like an interesting proposal how much of it did you catch i caught the i caught the very tail end i think so uh the suggestion that uh we may want to do something like h2 is doing and having a pr dedicated to the json rpc interface that accepts prs 

**Micah** - yeah so basically have a github repo that contains the specification and then the change control process would just be prs against that repository and the entire that is the entire change control process so pr would want to submit if they want to submit a change gets reviewed by however many people that pr lives for a reason amount of time to make sure there's time for people to get feedback on it and then when the pr is merged that's when it's final or that's when it's standardized 

**Eric** - uh well i'll be damned if that's not the most pragmatic thing i've heard 

**Lightclient** - it's almost like we should do that for core development too 

**Micah** - i agree they are used for everything 

**Pooja** - so while you're talking about having it in form of pr and a repository what are the thoughts on having it on eth1.org repository 

Decision 4

    Define JSON RPC specs in specs repo

**Micah** - i'm fine with that i think that's a great place for it to live and this would be a good opportunity to try to kind of start using eth10 specs repository for this exact sort of thing and then maybe one day we can enter then if this works successfully i can dream at night about how one day the uh core dev change control process goes through the same system and eth1 specs repo

**Lightclient** - just imagine we'll be putting prs into the yellow paper for hard fork changes 

**Micah** - well hopefully it's worded better than the yellow paper 

**Tim** - so about the eth1 specs i was talking with Danny i think yesterday or today before when the merge happens those repos should merge too um and the eth2 specs repo is like much i guess more uh much bigger it has more content than the eth1 specs repo so i suspect in the next like i don't know six months or maybe a year the ethonospex repo will probably get merged into the eth2 specs repo and and given like the scope of both uh the east one would be this one that moves over um yeah so i just want to point that out it might be kind of on its way out and i mean most things would still be useful in the like i guess it would be called the eth specs repo at that point or whatever but like the the merged version of the eth1 and e2 specs repos 

**Micah** - so perhaps if we do this do it in the eth2 specs repo and just deal with the fact that it's kind of a misnomer for six to 12 months

**Tim** - yeah and moving the eth0 specs repo is not long uh you know i could probably do it in a day but i think it's

**Micah** - you know yeah the moving the pr is the hard part like if we do do this pr change control process um then like it's nice to have the pr's living in the right place from the beginning 

**Tim** - yeah yeah yeah sorry yeah that's what i meant it's like almost we should move the eth1 specs repo before we do this right

**Micah** - um but then yeah out of curiosity how would how do the eth2 devs feel about just renaming that repo like this week to eth specs and we just move everything over there over the next months um they feel very possessive of it right now

**Tim** - so i guess my fear is like or my perception of their fear is maybe i i don't know i think danny ryan is the one who would want to ask about it like i'm curious i'm just looking at the commit history right now and it's like danny ryan and and xiaowei are like 80 percent of the commits and i guess proto is like you know number three a distant third but like yeah shaway and danny ryan are really like the biggest committers so i think just asking the two of them is probably yeah good approach um 

**micah** - okay anyone want to volunteer

**Tim** - to yeah i don't mind asking i don't mind asking i guess what um what i would would be useful to know along with the ask is like what are the specific changes we'd want to do you know um because that'll be the hard part if i tell them can i move five markdown files over i suspect they'll say yes if i tell them can we change how you handle pr's uh i suspect they'll say maybe and this is the hard conversation 

**Micah** - right right and that's a that's why you just you know you show up and say oh do you mind if i can cut in front of you and then you're holding like one thing and so as they say yes you're like okay bring over the carts 

**Tim** - so i you know i think it yeah maybe the best way to go is like for us to and us i feel like i'm putting work on other people than myself right now but like um yeah till i kind of write down what we want and then bring all of that to them um rather than just like can we merge the two repos which is a bit disingenuous 

**Micah** - so short term i think what i would imagining is the hard-fork coordination for the application layer would move over so london berlin shanghai etc and then potentially if everybody's in agreement on jason rpc we'd try to talk to the jason rpc group to make sure they're also on board with something like this and if so then the other thing would move over would be like basically the interface layer so the application layer interface which probably will also include the application consensus layer interfaces like the ones that communicate back and forth from each other um some of those are already in the eth two specs repo so however they have it laid out maybe we could kind of merge in with that again assuming everybody is on board with this general idea um eric does this general idea sound good to you not quite sure how much sarcasm there was in your statement earlier

**Eric** - uh none whatsoever i think i think this will be well received because one of the main concerns uh that have been raised during the um uh like json rpc groups uh meetings is that like like it particularly from the client teams they're like wait you're saying that like we're going to be held up by the eip process to like create or change methods they're like forget it so i think they will be very receptive to this idea 

**Tim** - we talked a bit earlier about splitting up the eip repo for notification spam i feel like if we merge the eth1 specs eth2 specs and json rpc all together then we are back you know xiaowei doesn't want to hear about new json rpc calls and people in yeah working group don't want to hear about yeah deposit contract changes yeah that's very valid it's a 

**Micah** - good point yeah so uh fallback suggestion then would be um i don't know ethereum interface specs repo or something yeah 

**Tim** - i think i feel like there's i don't know maybe it makes sense to actually keep them separate for now and have yeah one for the json rpc which is like the interface e1 and e2 and then after the merge we can merge eth1 into eth2 and then and and then you know there won't be any more changes to each one after right like or whatever changes they'll be they'll be across the merged clients right they won't be just across eth1

**Micah** - um only minor note on that is i would name it interface not json rpc um at some point we might bring in other other protocols like grpc if artem gets his way or we have rest for the consensus application layer i think they use rest for their communication and it feels like all those things should go in this repo like this is the repo for how various pieces of the system talk to each other essentially yeah that's what i'm imagining at least 

**Eric** - so are we are we thinking that rpc methods that are implemented by say just wallets like wallet at ethereum chain and so on would also go in this repo 

**Micah** - that is in my head that's what i'm imagining um because that that still is an interface which is between dap and wallet right and you've got the interface between wallet and client you've got the interface between application client and consensus client you have the interfacing condenser client and wallets like each we could split each of those connections out but i worry that we'll end up with people being confused especially since there's some overlap like the um dap wallet and wallet clients application client interfaces are very similar like they share a lot and so splitting it apart into like one repo per like pair of things um feels like that's not quite the right solution and so that's why i'm thinking one repo for all of it open to other ideas though 

**Eric** - yeah no i think uh i think that makes sense

Decision 5

    Create a new repository that's just for interfaces instead of migrating to eth2 specs repo

**Pooja** - okay to conclude for this uh particular item like we have to wait for some time and maybe when we are getting more clarity on how to merge with the each one and e2 spec as the ethereum spec repository then we will uh proceed with uh like creating a pull request there and having that living there on that repository itself 

**Micah** - uh you're talking about the for the eth1 specs merge 

**Pooja** - uh yeah because i understand that we are not planning to have the json rpc spec on the eth one spec repository so uh it will be created on the eth2 only directly there 

**Micah** - uh no no so the the current thinking for tim's feedback long ago we've pivoted very rapidly uh the current thinking is now have a new repository that is just for interfaces basically 

**Pooja** - oh sorry sorry uh yeah i got it no i i just messed with yeah okay uh so we have just a few more minutes left eric uh do you have any more questions 

**Eric** - i don't uh at this point i really appreciate that uh you guys decided to talk about this and uh i think the solution sounds good 

# 6. Progres on cannonical source of EIPs
Video | [56:46](https://youtu.be/CD3LCpeQX8w?t=3406)

**Pooja** - great thank you for joining us and we have just couple of minutes left here for this particular call i wanted to quickly check with brent if he has any update on canonical source of erp that he has been working on 

**Brent** - okay yeah yeah we have made a little bit of progress we got one of our engineers got the jekyll system running on his personal system and now we're moving that to a public system and once we get that up and running then we'll have a staging area where we can stage proposed changes so don't have a lot of time but we're making some progress 

**Pooja** - sounds good um so i know many people have to drop now to join the other call and we have almost had the time so thank you everyone for joining us today see you all in next uh two week on april 7th and the timing will be 15 1500 utc will be back on our uh usual timing thank you everyone for joining thanks see you later thanks 

# Attendees

* Pooja Ranjan
* Hudson Jameson
* Brent Allsop
* Micah Zoltu
* Lightclient
* Erik Marks
* Alita Moore

# Date for Next Meeting: April 7th at 1500 UTC
