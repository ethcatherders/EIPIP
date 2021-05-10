# EIP Improvement Process Call #32 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, May 5, 2021 at 15:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://youtu.be/cHmjk4tn7GI) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/67) <!-- omit in toc -->
### Moderator: Pooja Ranjan <!-- omit in toc -->
### Notes: Shane Lightowler <!-- omit in toc -->

----

# Summary <!-- omit in toc -->

## Decisions Made <!-- omit in toc -->
**31.1** | ERC authors must go to the EIP repo to assign themselves a number.

## Actions <!-- omit in toc -->

Action Item | Description
-|-
**31.1** | Tim to speak to the EF about the use of trademark for Ethereum.
**31.2** | Pooja to provide access for Alita to the JSON RPC repo.
**31.3** | Pooja to write a summary / background for Tim re: ERC bot so that he can speak to EF devops about a new repo.

---

# Contents <!-- omit in toc -->

- [1. Progress on ERCs repo](#1-Progress-on-ERCs-repo)
- [2. Should we care about people making statements regarding trademarks in Informational EIPs?](#2-Should-we-care-about-people-making-statements-regarding-trademarks-in-Informational-EIPs?)
- [3. Progress on JSON RPC API spec in Eth1.0 repo](#3-Progress-on-JSON-RPC-API-spec-in-Eth1.0-repo)
- [4. Progress on 'canonical source for EIPs'](#4-Progress-on-'canonical-source-for-EIPs')
- [5. Progress on EIP GitHub repo action bot](#5-Progress-on-EIP-GitHub-repo-action-bot)
- [6. Progress on ERCs repo](#6-Progress-on-ERCs-repo)
- [7. Review action items from the previous meeting](#7-Review-action-items-from-the-previous-meeting)
- [Annex](#annex)
  - [Attendees](#attendees)
  - [Next Call](#next-call)

---


# 1. Progress on ERCs repo

Video | [0:00](https://youtu.be/cHmjk4tn7GI)
-|-

Lightclient was not on the call so this section was initially skipped.

# 2. Should we care about people making statements regarding trademarks in Informational EIPs?

Video | [0:31](https://youtu.be/cHmjk4tn7GI?t=31)
-|-

Micah Zoltu - Someone is creating an informational EIP to propose an appropriate term to describe the Etheruem mainnet. We want to clean up the nomenclature.

There's one section in the EIP that mentions that the term Ethereum is trademarked by the Ethereum Foundation. Am uncomfortable with 'legal stuff' being in EIPs. What do others think?

Tim Beiko - Yes, this felt a big red flag. The EF has tried to not use the trademark except to defend against scams. The biggest use case for the trademark is for taking down scam youtube accounts. The EF needs to own the trademark for this purpose. It seems weird to impart how the EF uses their trademark in an EIP.

Micah - Quote re wording in the CIP: 
> even though the name of the network is ethereum mainnet which is what the cip is about it will be necessary for your application it may that may be critical here it may be necessary for your application to show this as ethereum a little r circled mainnet and include a note ethereum as a registered trademark of ethereum foundation elsewhere for more information on your obligations on mentioned ethereum trademark c and then it references the uspto registration number and the note at the bottom of the terms of use page.

They're not saying you must use the trademark.

Tim - No project mentions the ethereum trademark that I know of. I wouldn't include it.

Micah - I'm weakly against it, the author wants to include it. I will leave it to another editor to merge, unless they remove it. That feels a bad way of doing governance though as it will sit there for a long time.

Tim - I can ask the EF what they think about it. They may not want to make a public comment however.

## Actions

- **32.1**—Tim to speak to the EF about the use of trademark for Ethereum.

# 3. Progress on JSON RPC API spec in Eth1.0 repo

Video | [6:38](https://youtu.be/cHmjk4tn7GI?t=398)
-|-

Alita - There is progress on this. I spoke with Tomasz about my involvement, and he does seem to be recommending me to be doing the project, but its not clear that I'm officially doing it. I dont want to waste time if th  unclear. I am blocked because I need reassurance that I am the one working on it.

We are drafting up all of the JSON RPCs and prioritising the ones to be done first (eg ones pertaining to EIP 1559). I posted this on ETH Magicians.

It's going ok, but its challenging put too much time in it because Im not sure if Im the official person working on it. Something will be posted soon on github or ECH Medium inviting comment or proposal.

Micah - In this space, if you just start doing something that noone else is doing and do it well, noone will challenge you.

Pooja - I agree! Im working on getting access to the Eth1 specs repo to merge PRs. Please feel free to comment on Alita's PRs. Re: clarity on tasks... suggest raising specific issues in the repo on these.

Alita - If there isnt clarity on what Im supposed to be doing by Friday, Im just going to start. Please can I get access to the JSON RPC repo? I want to be able to create branches off the repo itself. I wouldnt merge without approval. 

## Actions

- **32.2**— Pooja to provide access for Alita to the JSON RPC repo.

# 4. Progress on 'canonical source for EIPs'

Video | [12:54](https://youtu.be/cHmjk4tn7GI?t=774)
-|-

Brent Allsop - Meta EIPs - we need to decide where the home for everything is. Im still trying to figure out what is best for all.

Micah - We should focus initially on getting the ERCs out. If that goes smoothly and well we could then consider other things. But we should focus on that first.

Brent - Do we want to leave EIP 1 and the meta EIPs then?

Micah - For general meta informational EIPs, its fine to leave. EIP 1 is special - if we feels theres a better place for this to live Im ok with that.

Brent - so re: the EIPs on eips.ethereum.org we have tabs for all and for core and meta, but theres also one for ERCs. Do we wnat to leave that?

Micah - In a perfect world wed have the same page layout but pull from 2 different sources. The engineering effort required to do th  probably more difficult thn just having that tab link out.

Brent - yes, have someone maintain a whole ERC repo. Who can do that?

Micah - we've struggled historically to get engineering to work on this. If and when we pull/extract out the ERCs into a spearate repo we'll probably lose them from the 'all' list. We can keep the tab, but the tab will link out to a separate external page.

Brent - There's also talk of moving towards the Eth2 model - get away from ERCs and just have PRs against the python script. Do we wannt to worry about that?

Micah - too far in the future to worry about. Feeling on it seems positive, but the effort involved is significant. I wouldnt plan on it or build around it.

Brent - So we will continue on as planned. If we can find resource to split out ERCs we'll hopefully do that. For the time being we'll keep on working with what we have.

Micah - ERCs will be extracted, it's just a quetion of when.

Tim - we should make it clear on the eips.ethereum network page that this has changed. A problem we have is when we remove specs from previous hard forks they can be difficult to find. We should be clear where th  moving to. Re: changing to match Eth2 specs... I suspect we will keep core EIPs as a way to define the changes.

there'll still be debates about what gets included and what not and it's probably very messy to have those live and just open pr's to this bank and that are not merged so i would not be surprised to have something where you have the python and then once an eip is accepted you just open a pr against the spec and actually update it or you only open a pr per hard fork or something and you say you know th  the changes for london which is kind of what etude does so it doesn't mean that the eips will go away it just means that it's almost closer to the yellow paper going away than the eip repo.

Brent - There'll still be a proposal for EIPs, but there will still be a clear gate ahead of a decision being made, and then once its accepted the PR is done and merged into the spec?

Tim - Something that.

Micah - i think everybody else that i've been talking to is assuming the opposite of what you just said which is that we would just submit pr's against the spec correctly and there would not be anything...

Tim - it's a very naive assumption given the amount of given the ratio between the proposed eips and the merged vips right we have more proposals than we have things that go into hard forks so yeah and to be clear i don't think that's been decided but yeah it feels it would be very weird to have 100 open pr's against the spec and then we picked the top five of those and then the rest just i don't know gets closed or something it seems odd but yeah it's not that 

Micah - out of curiosity what makes that odd to you?

Tim - the fact that there's no i guess artifact after right take ProgPow just to you know take something that didn't get in that's important what do you do with the ProgPow pr after you know it's not in london exactly whereas now you know the eip is still there and i think that's kind of good that there's a long-term artifact to it and that's i guess that's a political one but there's also the case where eip was at 2200 which supersedes in other eips and whatnot so when eips start building off of each other it feels also cleaner to link an actual thing than to link this pr supersedes this pr and whatnotlike it's not 

Micah - this would be for it'd be for core eips only so we don't have to worry too much about these supersedes because we'll just be updating the spec to now say you know before this blocks the spec would say prior to some eip the spike would say th  the rule and then you the ip would make a change to the spec that says if fork block less than x th  the rule else this rule kind of thing umand so we would still retain the history aspect for the the Progpow and similar i mean there's a lot of programs one example there are many here right vips that are proposed and they're reasonable and they're generally good ideas they're well thought out and they deserve to exist but they're not part of ethereum i think that's the class that i think we're talking about here.

For those ones my personal view is i'm not opposed to just leaving them open pr's there is from a management standpoint we have to make sure we don't get the position where we're we can't manage all the opr's but i think with github labels we can handle that pretty easily and just say this this eip is considered for inclusion label would make it so you can filter and see okay what's actually being considered right now instead of all the things and then things that are explicitly were considered but rejected would have maybe another label so you can filter those out easily and so i feel my gut tells me which my gut here is very weak on this but my i weekly feel we can make it so having hundreds or thousands of open pr's is not unmanageable as long as we have a good system in place for managing that

Brent - okay so yeah i'm guess i'm having troubles understanding the difference between what micah and tim are saying it sounds micah both micah and tim want to split apart there's the governance part where things are being proposed and people are trying to get people on board and then there's the bridge when someone something finally gets accepted then a pull request is done and officially makes it into the spec

Micah - so the difference what i'm proposing is that we as soon as someone has an idea for a change to the spec they can open a pr and make that proposal as an official spec change so that is the first step in the official process you can there's idea steps before that where you just you know chat on forums or discord or whatever but once you want to make it official that you want to propose a change you open a pr that actually changes the specification and then that pr may sit open for months or years depending on how long it takes before it actually goes into hard fork and the act of merging is okay hard fork launched kind of thing and so that the merging into the spec means th  what ethereum mainnet is now whereas tim is suggesting that we have some other process for iterating on spec changes that is separate from those prs and the pr step is very close to the end of the process and so you submit a pr perhaps when we decide on fork blocks or when it goes onto a test net or something along those lines

Brent - so you're saying include the proposal and governance part in the pr process it's just you tag them it's not accepted yet or whatever

Micah - yeah they'd have a label that indicates th n't th n't considered for inclusion yet or th n't and part of th  you know matt has oh matt that's your good so is that client matter is that a different matt i don't actually know your last name so matt has argued with me in the past that the eips repo or the ethereum specs repo should specify ethereum maintenance that's the thing that it should be specified not ethereum things and so if we went down this route i think we would be moving towards that world view where eips are not a general thing or this i guess ethereum specs repo it's not a general purpose thing th  specifically the definition for maintenance it is not the definition for things that are mainnet or even the test networks th  specifically the definition for Mainnet

It does create complexity for testnets that's actually didn't really think about until now but if we're doing prs to a specifications repo then and they don't get merged to the specs repo until main net then defining what is rinkaby is no longer trivial it's no longer just oh it's eip155 

Matt Garnett - but if you have branches i mean it's not super nice but you could have branches with the full spec for the test net and then you could have a tracker where it's these are the pr's because they're still going to be kind of eeps but it's these are the pr's that we're adding just so it's an easy place that someone can look and see these are kind of the chains that are being discussed

Micah - so so actually this th  what we're discussing so do you believe there should still be core eeps or should there only be pr's against the spec

Mike - i think they should only be pr's against the spec i think that you know what i've felt after trying to write several eips is that you end up writing the same thing over and over again for you know half of the eep you're trying to describe the situation and you're trying to set up what is mainnet when in reality if they were just pr's against the spec you don't have to do that anymore you just have to say here's the difficult spec and then you can just focus on the rationale

Micah - and the rationale would that be integrated into the spec maybe some sort of commenting system or would that be just the pr description kind of thing is where the rationale lives

Mike - i mean that's a that's a good question i think in the pr is okay because that's how a lot of other governance systems sort of work as far as i'm aware if you look at the rust language how they do rfcs it's all just prs into the rfc repo and the discussions are kind of there i don't know if they have i mean it's different obviously our again rfcs are not quite the same as a consensus definition of what mainnet is i don't think i have a really strong opinion on whether it should be in the pr in a separate document it should wherever it is it should be accessible pretty quickly and it should be documented historically 

Brent - okay i think i've got that i'm going to try and write some of this awesome go ahead 

Micah - just for you brent everything is up in the air no one's decided on anything 

Brent - right so that's what i'm struggling with

Micah - i i appreciate your your struggle and frustration i said i would work under the assumption that we still have core eips we still are doing the eip process as it is today maybe at some point in the future the doubt process will change but for i think your work you can kind of just ignore that the only thing i think that matters for your work is just the ercs are almost certainly going to be split out from the eips that part i'm pretty sure is going to happen and hopefully in the very near future

Brent - okay great yeah that puts a bounding box around what i need to do so okay i'll move forward to that thanks so much for the help

Pooja - yeah so i have i also wanted to give a small suggestion or proposal i don't know that is something coming up in my mind whatever we have been discussin about that may happen in future about managing it through specs using pull requests for updating the specs of the main net i find that very similar to each tool process right so i was wondering we are working on london upgrade right now i know th  not the right audience to kind of decide on anything but i just want to share my thoughts right now we are working on london and we are following the process that we came up last year during a long conversation in this eipip meeting itself but for the next update maybe shanghai before the merge if you are expecting that i think it it's worth giving a shout out that we should try this pr stuff i mean i don't know i do not have any clear picture right now but my my thought would be feature based pull request if somebody wants to add something

Tim - so yeah we can't do that if we're doing shanghai because there is no spec of ethereum one it's something that's possibly being worked on but it's definitely a prerequisite we don't have something to do prs against right now maybe for the merge we could do it and actually that's what they're doing on the e2 side but if shanghai is just a feature fork the odds of having a stack is very low and i wouldn't want to put that as a blocker

Micah - yeah i think unless we hire someone full-time who already has experience with ethereum realistic timeline for getting a full spec written is probably a year even if we hire someone full time i think realistic timeline is probably a year 

Tim - yeah

Micah - and we're basically saying someone needs to write a python client that is specifically written to be readable not to be fast the currently is pi ethereum but it's designed to actually execute relatively quickly and therefore it's harder to read th  a rewrite of a entire ethereum client that is explicitly designed to be readable

Tim - yeah and i think there's a few different people or groups that are somewhat interested on it but i'm not sure they've made that interest public and you know that they're it's more than a hobby so yeah i it's something i i've been spending a bit of time looking on and talking with folks who might be interested but i doubt yeah i think at the in the best of best cases we would get something six ish months from now but that would be too late for you know shanghai if it's a feature fork and possibly for the merge too so

Pooja -  okay i mean yeah that would have been a nice to have feature i mean obviously nice to have process in place but never mind we also have to consider a lot of other constraints along with this process okay so one last thing that i wanted to discuss in this topic particularly about my types i don't want to bring the entire thing here moving off eip1 and all just one thing for this past two upgrades we are having a dot md file for berlin a dot md file for london so what do people in general think about if we create not create if we kind of move the meta files which were for earlier upgrades here or maybe a copy of that no copy wouldn't make sense but yeah i'm moving

Micah - sorry move move them where 

Pooja - to the eth one spec we have network upgrade section in which we are keeping all upgrades we are keeping it for london we are keeping it for berlin and even if we we have i believe there is a file created for us as well so we can move it there 

Micah - are you talking about moving the old hard fork meta eips there is that correct

Pooja - yeah yeah 

Micah - i'm a big fan of that i would love it if someone just sat down and just kind of transcribed the hard fork metas over to eth1 specs and then my preference and th  a weak preference not as strong as that i have in the past my preference would be then we actually remove the them from the ips repository and just replace them with a pointer similar to what we did i believe for i think we did this actually for berlin so if you look at the hard fork the berlin meta eap it just points at ether1 specs repo if we were to move the retroactively move the other ones there i would be in favor of also having them just have a similar pointer just to kind of encourage people and reinforce that eth one specs repo is the place to go for hard fork meta information 

Tim - so the challenge is each one specs repo might not exist in a year so because if we merge so i i'm fine doing that but i would wait basically a year until we have actually harmonized the eth1 specs any two specs repo before doing it because then you'll just end up with a bunch of broken links but i don't mind taking that on once i guess the first thing i feel i need to figure out is how do we merge each one specs any two specs and it's not the most urgent thing right now but i think after london it will it will kind of climb on that list and once we have that you know ethereum specs or whatever then yeah i i wouldn't mind putting a bunch of pointers and adding the past hard forks but right now yeah the links will just be out of date in six to twelve months

Micah - sure so are you arguing that we should not back port the hard forks at all or just we do back then but we don't back link to them

Tim - i think we should back link to them but once we have a backlink that we're fairly comfortable will be stable right so i don't mind so if we have you know eth one or if we link them if we battling them to eth one specs and the eth one specs repo goes away in six months then we have a bunch of broken backlinks we've forgotten about so if we merge eth one eth two specs repo into ethereum specs post merge then we'll have one repo we know is going to stay around and and we can backlink them there and i think that's fine

Pooja - if i understand correct we are ultimately planning to move out everything out of mata i mean meta eip right so anyway we are going to move it out of eips i mean it is repository at the end of the day so if we bring it to the eth one repo right now maybe it will be pulled to the eth2 or wherever we decide to move merging things it will be pulled together 

Tim - but the link from so in the if we do that right now you basically go to all the meta eeps and you say this keep is not not accurate go to these one specs but all those links will break when we do the transition and people are already complaining to me a lot that they don't know where to find the hard fork specs and whatnot so i'd rather everybody knows that the hard fork meta eips are a thing right now and i'd rather just do this transition once than do it twice because now it feels it's messy and nobody knows where to find the london spec or the burning spec and 

Micah - so i feel there's there's three three options here one we do keep all hard fork eips in the eip's repository until we're ready to fully move them all to ethereum 1 specs or eth 2 specs or whatever or we have all of them in eth specs asap and so that is the canonical source or we have what we have right now which is legacy ones are in ethereum.org meta and the new ones are in eth specs i feel the way we have now is kind of the worst of both worlds because there is no canonical place to go to look my i do have a preference that we move the canonical place not to be eips and we start training people on that sooner rather than later but it sounds tim you would rather go back on our decision to drop eips from meta or sorry drop hard fork eips

Tim - so i guess yeah what i what i was advocating for is your third option which when you put it that does sound pretty terrible so yeah in that case yeah i feel the way you framed it i would probably rather move all the yeah all the meta eips to the e1 specs repo but if we were to do that i think we should give we should bring it up on all corners and give people the chance to chime in and whatnot i don't want to just do it overnight and and then you know people are where the hell

Micah - yeah so these these historical eips are a little bit easier i think than london shanghai and berlin because those are new the historical ones aren't changing so it would not be terrible if we had them duplicated at least for a period so we can leave them in the eaps repo as they are now don't touch them and then also have someone go through and transcribe them over to one specs and then we can tell people you know the right place to look for hard fork changes is the eth one specs repo but people who are still going to the old place will still see the old stuff so you'll still see 

Tim - yeah i that what we could also do is add a line at the top of every one of those saying you know this meta eaves are no longer being maintained here you can see this you know in the east one specs repo um

Micah - sure and then if the if that link breaks it's not critical because we still have the spec

Tim - right yeah and we gave we gave you know advanced warning say that that link breaks in a year then there's been advanced warning for a year that you know th  not the right place um

Pooja - right i mean yeah th  th  very similar to what i was having in my mind like we have berlin and in that we will be having everything that was there for homestead meta eip whatever it was uh just that even my type number would not be there but the content will be there and in that we are going to just add a liner that th  now available on homestead md eat one dot oh spec repo

Micah - so yeah if you have if you have someone in mind who wants to go through those hard fork metas and just kind of port them to eth one specs repo i think 

Tim - i can do it 

Pooja - yeah i was also wondering if i can look into that 

Micah - yes they're relatively easy to port i don't think it requires any specialized ethereum core dev knowledge it's pretty straightforward process just kind of time consuming 

Pooja - yeah sure cool so at least we are good on this part so going back to point number four where we are discussing about canonical source of eips ah just to summarize this for brent brent he has to continue working on ignoring this fact which will be coming in future just work on the erc part and extraction of that for new destination of meta eips not all except eip1 we would be moving meta eips a copy of it to the ether dot or spec repository and for other proposals core interface and network we are kind of tabling it maybe we will discuss that in future

Brent - that helps a lot thanks

# 5. Progress on EIP GitHub repo action bot

Video | [41:59](https://youtu.be/cHmjk4tn7GI?t=2519)
-|-

Alita - Overall progress is good. Hopeful that we can activate it soon. 

Micah - More reliable than our existing bot!

Alita - the bot is active on the EIPs repo. Its a stubbed version so it doesnt have the capacity to merge yet. Will in future. Running in prod but not merging. It's still in my own github - needs to be moved to Eth1.

Pooja - to mark this as done we would want to move that to the ethereum github repo.

Micah - we need to we need two things one we need to meet an actual repo in the ethereum organization and two we need a execution key that has a nice spot name not alita 

Pooja - so when you say that repo on ethereum Github do you mean a bot repo wasn't there such a thing earlier there was bought earlier

Micah - i don't think anyone's created a bot repo in ethereum organization but maybe they have and i don't know about it

Pooja - okay maybe i'll make a note of that we might want to get into it so i'll try to get into that 

Micah - just whoever i don't know who actually has rights in the ethereum organization to create new repositories so i don't know who to ask 

Tim - yeah so it's the ef devops team so you know i don't even have the right if somebody can send me just a quick note just giving some context about the bot and whatnot i can get it created 

Pooja - right so with that note i was going to come back on agenda item one that was progress on erc and i believe we need help there i'm not sure if we have this erc bot created yet do it doesn't even have any information on that 

Micah - i think it's the same problem we just need the right people to go and create new repository i don't again i don't know who those people are

Pooja - i was trying to reach a couple of people but i had no luck or maybe tim if you can help us on that we are looking for someone to create repo and get access to micah and lightclient at least so that they can start the initial work and then

Tim - yeah so i guess yeah so it's the ef devops team so the only thing i would need for both repo is just kind you know some background and summary they want to understand why they you know we're creating the repo so if somebody can just send me kind of a quick paragraph that i can copy-paste and give to them that'll that'll help along with the who should be admin on the repo 

Pooja - i'll get in touch with you and i'll provide you the details

## Actions
- **32.3**— Pooja to write a summary / background for Tim re: ERC bot so that he can speak to EF devops about a new repo.

Tim - perfect thanks

Pooja - for erc i'm very clear on that path for bot micah would you want to add anything

Micah - i can let alita probably can describe the bot better than i can so i'll leave that to her

Alita - i'm gonna reach out right now with the description i don't know that so sounds good

Micah - we probably need to bike shed for an hour or two on the name of the bot as well

Pooja - i think i can bring it up in the next meeting.

# 6. Progress on ERCs repo

Video | [47:07](https://youtu.be/cHmjk4tn7GI?t=2827)
-|-


Lightclient - just waiting to get it created

Pooja - okay so i mean if i understand right after it is created we will start moving and we will have to publish a kind of announcement blog mentioning what all changes we are doing with that process and maybe i was wondering if we we should start adding questions and concerns with erc i have been receiving quite a few comments when with nfts and all they they are having some discussion around this versus business standard and also these kind of stuff may be added in future eipip call

# 7. Review action items from the previous meeting

Video | [48:09](https://youtu.be/cHmjk4tn7GI?t=2889)
-|-

Pooja - 

* the first one is create erc repo we are still working on it and i will probably details how's it going
* okay so the next item is update eips.ethereum.org with changes to eip and erc repo i believe we are going to see this in our next one or two meetings so i mean we have to work on that create a boundary for json rpc api spec i'm not sure if we are going to create a bounty right away but i am expecting some kind of write-up on that maybe from a later that would be helpful 
* complete eip report we discussed this today 
* determine pay rates for eip editors i don't know i'm gonna talk to Moloch people for that uh i have a meeting this week so after the conversation maybe if we can get some kind of clear picture in that one funding part i will be happy to share that in the next meeting 
* the next item is 31.6 it's add an erc dictated editor for now i'm considering Lightclient for the editor of erc as he has shown interest on working on that but in future if we need more and more people we'll try to reach out to community so that's all about it and anyone wants to bring up anything

Alita - so there is one thing which is that there is more work to be done with the bot and moving forward i'm kind of awaiting funding for that so that would be one thing to look into i don't know if that's more of an ech meeting thing to talk about though

Pooja - bot funding Alita?

Alita - for continued work beyond the initial merge so the stuff we talked about today that's all gonna be done that's included in the initial implementation but then there's other work transferring over the circle integration to github actions adding some more features to the bot more considerations along those lines

Pooja - i think i could use help here from the eip editors so eip editors whatever we have decided for the first task i believe we have decided on a fixed amount to be for that work to be done and whenever we come up with any kind of enhancement work or nice to have feature that has to be added on eip bar if we can just create an issue maybe in this eipip repo or the ethereum dot eip github wherever and give an estimate of time or you know work needed the feature that has to be added that would be easier for Cat Herders to follow up and you know kind of provide funding funding should not be a problem that is something that we would to cover from the ECH side but getting an estimate of work and how much funding is required would be helpful

Micah - so i think it would be it would be easier for everyone except for the cat herders if it was if we were able to hire someone to kind of work somewhat unboundedly at an hourly rate or something that or salary just because there's a number of kind of small tasks and often in engineering the cost of estimating how long they will take ends up taking more effort than just doing the task and so i'm worried that we would end up wasting more time and money on just doing estimates than we would on just having someone that we could kind of a regular person who would go back to and say hey you got some more work start clocking hours or whatever the process is 

Pooja - so yeah i'm planning to have a request shared this time for next quarter maybe for an on-call engineer one hour per day kind of 20 hours a month or something that so i hope

Micah - yeah something that i think would work much better than trying to figure out how much each project costs just because there's lots of little things that i think we could really benefit from having just an engineer who was somewhat familiar with our process and who we can kind of go back to

Trent - is this specifically related to eip editing or a different set of tasks

Micah - yeah eip stuff it's yeah bots that help us do editing easier make make the bots better improve them there are also things we talked about this whole thing with the ercs or cips we want them to kind of share a numbering system and so someone could write some tooling that makes it so we have a mechanism for getting shared numbers so they don't conflict don't overlap there's miscellaneous stuff that

Trent - one then my next question this work that's already happening micah are you would you consider yourself as a person to do this kind of stuff or are you trying to get other people to

Micah - it is work that is not happening because we don't have we don't currently have anyone we have everyone who does eip editing is an engineer but none of them actually do engineering for the eip editing the last person who did a significant amount i think was nick johnson and that was two or three years ago i'm here with the original bots and since then we basically have you know we have again we have engineers who are editors but not acting as engineers if that makes sense

Trent - okay so but are you proposing that you would be doing this work?

Micah - definitely not. Alita has done workforce previously on the bot she recently wrote and so i would be fine with her being that person or someone else i'm not particularly attached to any one person more care but that there's somebody

Pooja - that was another point of consideration i'm requesting this funding for but i may not be able to understand to whom it has to be disposed or you know when and how much if it is just on a monthly basis we are requesting for 20 hours a month or so we i cannot say for sure that it is secured until it is actually secure but when when a job comes if we keep on posting that th  th  supposed to be done and this has been done in this month that would be really helpful for a lot of us

Micah - yeah i think having an after the fact just what was worked on shouldn't be too big of a problem that's much easier than trying to do estimates of future work 

Trent - yeah just submitting invoice 

Pooja - sounds good to me okay these are all good conversation i'm very happy that we made some good progress today i mean every meeting we do but yes there was a lot of clarity i was i personally was looking for so thank you everyone for joining us today and i hope to see you all in two weeks please keep sharing any thoughts any comments any concern that you would want to bring it up related to process improvement of ethereum ecosystem make a comment on agenda or you can reach out to us all the members of eipip have a good day evening everyone.

---

# Annex

## Attendees 

- Alita Moore
- Brent Allsop
- Mike Garnett
- Micah Zoltu
- Pooja Ranjan
- Tim Beiko
- Trenton Van Epps

## Next Call 

Wednesday, May 19, 2021, 15:00 UTC.
