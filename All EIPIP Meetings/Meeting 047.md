# EIPIP Meeting 47 Notes
### Meeting Date/Time: Wednesday, January 12, 2022, at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/101)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=66fO36vzGUY)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## ACTION ITEMS

**ACTION 47.1**: Shashank will work on documenting the EIP bot improvement contribution guidelines.

**ACTION 47.2**: Pooja will check with William Entriken or ask him to join the next meeting to elaborate on comments.
 

## AGENDA

# 1. EIPs repository spam Ref: [Comment](https://discordapp.com/channels/916516304972824576/916713912970412103/930316673200848968)

**Pooja Ranjan**: All right welcome to the ethereum, proposals improvement process meeting eipip meeting 47. We have the agenda shared and the first item listed here is eip's repository spam. We briefly discussed this concern in the last meeting.  Micah pointed out as a concern and how it can be addressed. It was also brought up by Sam Wilson in the ethereum R&D discord and  the last message from Micah on ECH discord suggested to be added to eipip meeting and to be discussed. So Micah if you would like to briefly talk about the issue.

**Micah Zoltu**: So I realised the other day that the majority of my time doing eip editing is
actually just dealing with administrative stuff like reporting spammers and closing tickets that they create and closing deleting comments when they leave them. This is a job that I think pretty much anyone could do like it doesn't. It's not terribly hard to learn to identify the spam. The spammers are not particularly ingenious.  They seem to be in a hurry. Their accounts are very obvious and so it's a relatively simple process to just go through and delete their message if possible and close their issue if they opened it closer to PR. If they opened it leave it leave a comment if there's confusion by actual editors or authors about the
the spammers and then report them to github and  think if someone was doing that along with a couple other little administrative tasks like categorising like putting labels on things or mentioning people as needed like mentioning appropriate people. I could in theory unsubscribe from the eips repository and just get the mentions at that point which would lower the burden greatly and lowering the burden is a Micah and is a good thing because it makes it more likely micah will stick around for a long time and so if we can find someone to fill that role perhaps someone who is interested in getting involved in the process but doesn't have like the deep technical background to do. The editing itself might be a good opportunity for somebody.

**Pooja Ranjan**: That makes total sense just wondering if we have anyone from the present meeting who would be interested because my understanding is this can only be done by someone who has access to delete messages.

**Micah Zoltu**: Yeah so the hardest part is finding someone that is trusted enough to do this. Trust being hard to come by on the internet, if we can solve that problem then I feel like We just need to find someone who's interested and meets that trust requirement.

**Shashank Yalamanchi**: Yeah so what we can do is that maybe not directly trust someone just assign. Someone to figure out what the spam issues or pr's are and then tag someone
who can actually delete it and then see how active they are and depending on that maybe. We can give them access or something like that. Does that make sense? If that's fine I guess to begin with.

**Micah Zoltu**: Yes I am trying to think of how much that would probably help I mean again that would get to get us to the point where we at least can like the editors themselves can actually stop unsubscribe from the eips repo which would be really nice yes yes because the
the repository is very spammy and a lot of. It is stuff that the editors don't actually need to respond to it's just people like updating their own PR's and what not and know you get a
notification every time and it's, if we just had one person whose job was to kind of go through all of that and then mention people as necessary. I can include you're right it can include mentioning someone to say hey spammer please delete.

**Shashank Yalamanchi**: Yeah I have been kind of doing that for the past week tagging Pooja. You may be like, sorry Matt, sometimes if i find a spam comment  what you can also do is maybe you know just tag. maybe you puja or matt and at the end of the week you can take up that responsibility and delete those because you should. You might not  be effective for you to spend time daily deleting these issues or pr's because they are spam by default. They require as much less attention as it is needed by the eip editors so it can be done at the end of the week or maybe end of the month whatever or like a fortnight one whatever works for you, a good first step maybe.

**Micah Zoltu**: I mean realistically, I will probably delete them as soon as I notice the dimensions which are fine with me. I am trying to find a good exampleI  wanted to one second let me see if I can find a eips. I wanna do a screen share and just show you guys what the process is for the reporting and how to identify them if anyone happens to know a recent spammer.

**Sam Wilson**:  There's a lucid 36 guy.

**Micah Zoltu**: Yeah okay can you pull this up and I am sure you can see that and it's a thing you see on github. Okay, so this guy for example so my usual process is, so right off the bat. They almost never fill anything in here. If they do something feels named for the description or their comment. It will be just like a link to somewhere else or another eip or sometimes they get particularly clever and they copy and paste someone else's submission and so you do have to look out for those. But if you go and click on the user lucid36 here, one of the indicators is their new account so this account is actually older than most of them. 
Just like they just started committing this week. So this green heat map here will always be shifted to the right for spam accounts. If you are not sure you can also look through their activity and you will notice a couple of odd one. They will contribute to a lot of ethereum and cryptocurrency related things and if you click through on them or look at what they do they just spam pull request approvals or reviews. For example this guy just reviewed you know from 12 different or six different ethereum or cryptocurrency related things they just did a bunch of reviews in a day you know. If you again just dig through, you will see they recreate a lot of repositories. Again this is fairly abnormal for a real human to create massive prosperity not always.

These are just each one of these like another little red flag that you can look out for and then if you really want to check you can look for. If they posted an issue or a commit or a pr and you will probably notice that they look like the same thing that they posted in the theory eips like this person is just posting addresses or hashes or something in the my ether wallet repository. I think this is obvious. This person and then their friend here are just spamming anyway so I just do a quick glance. This usually takes you know I only spend Ii don't know 30 seconds or so on it after you have done a few of these. You start to notice the pattern and then click this block or report button here. Actually I took that back then after verifying that I went back to this page. If it is a comment or a new pr or a new issue. You can click the dot dot dot and report content here in this drop down and I will take you over to github's report feature to do  and there you go. 

Okay, so you just go down. I would like to report abusive content or behaviour. I want to report spam or users disrupting me or my organisation's experience on github. This user disrupted my organisation's experience on github and then down here. you have to type
words or else it will fail and so spam issue creation. I think it's a pr creation. Pull request creation something like that hit send and then finally that'll go off to github and then finally you go back to the pr question and close it. If it was opened or in this case if you don't have
the ability close just mention Micah and say hey it's the spam please close it and that's it. Move on to the next one.

We get maybe 5 to 10 a day of these. I think this is off top of my head. Maybe that's way
off. I don't know but it feels like 5 or 10 a day. They are just tedious like it's one of those things that you see a notification or email that just is annoying. There's two other problems if they do the spam pr review, so a lot of people these same spammers will just go through and those review a bunch of pr's and they'll say approved or reviewed or comment or whatever. This has two problems one is confusing to authors because authors think or someone reviewed my pr but this person did not review theirs or they just are spamming the repo with approvals.

The second issue is there's no dot dot dot next to approvals only on comments and so as you can see on this line. There's no like dot dot report so this is where you have to actually open them up, go into their account and then you click block a report on the left and then report abuse here and that takes you back to the same page.

 The last and final problem is that the irony here bugs me. Github will only yet let you report people at a certain rate and then you get rate limited for reporting people and they tell you to stop and so if you have a spammer that has two accounts you can outpace your, one account that is reporting them and so you have to go create a like second account, just so you can keep up and report all of them. I have only run into this usually if I fall behind. The spammers aren't that bad that they get to the point where I get very limited but github does rate limit you after about three and then you have to wait an hour or so before you get cleared to do more. So if someone could do that and like I said just if you don't have delete access just mention me. I try for comments, I try to delete them because you can actually delete them. You cannot delete pr review comments but you can delete like regular comments if you're an admin and so for their comments. I try to delete them if they leave a review. I usually just report it unless the author is confused by it. If the author says something in response I will usually have comments saying that's just a spammer please ignore but otherwise yeah just message me and so I can close the issue or delete the comment. Does that make sense to everybody?

**Shashank Yalamanchi**: Sure I do have a doubt Micah, so I do have a doubt so let's say if I go ahead and I mention to you that this is a spam. Do you also would like to have an explanation as to why I consider this as spam so that makes it easier for you.

**Micah Zoltu**: No I would just say, I am guessing that I will recognize it right away as spam and like I will probably still double check at least at first.  But if I disagree with you that is spam or whoever mentions me if I disagree that is spam. I will probably leave a comment saying I don't know about this. But I am guessing like I said I have gone through enough of these that at this point it takes me about 10 seconds to identify someone as a spammer or not. Every now and then they do something new and clever and it makes me a little bit longer like one guy actually had a pro account. They were spamming with meaning they paid github money to spam repositories and that caught me off guard because that was the first time I saw a pro spam. Right? I still end up being a spammer but I spent a lot more time digging into that one than I do most of them but yeah like I said most of them. I can  recognize right away and so the goal here is to make it. So I can hope is that we can get to a point where I can unsubscribe from github and instead just get mentions because right now I am watching this repository for all activity and I think I am the only person that does that and so I am the only person that sees you know half the stuff that comes through.

**Pooja Ranjan**: Well this is certainly helpful, it's not only that people who are like one of us, who are actively involved in these eips repositories can tag you or the other eip editors to flag these spams but anyone listening to this call can do that. So thank you so
much Micah for screen sharing and explaining the process. How it can be actually reported
and just for record Shashank I do not have edit access or delete access so I can also  just forward it to eip editor so it's better to mention it to eip editors only. I mean to make a mention of that right now.

**Micah Zoltu**: It might make more sense just to mention and link me like in ethereum cat
headers or ethernet ep editing channel. That way we don't need to further add more spam on top of their spam to people's pr's and whatnot.

**Pooja Ranjan**: That makes sense because it will again increase our github notification

**Shashank Yalamanchi**: Yeah I think that would be better, yeah maybe on the discord server. It will be better, yeah it's not sure.
**Micah Zoltu**: Yeah so anyone who notices one just mentioned me and then if things are going smoothly. I will unsubscribe and be happy.

**Pooja Ranjan**: Well that sounds like a great plan to move ahead. I just hope that it should not be spamming but I hope that this is going to be very helpful because these people are not. Just creating spam but they are ultimately harming the innocent people who believe in them by looking at their github uh you know colours on screen that they have contributed to some of the repositories.

All right let's move on to the next issue listed here unless anyone has any final comment to add. cool

# 2. Discuss & document process to merge EIP bot PRs

**Pooja Ranjan**: So the next item listed here is the discussion and document process to merge eip bot pull requests. The present eip bot was developed in 2021 thanks to Alita Moore for working on it. I know the eip editors have helped a lot to improve the process of
eip standardisation in a year and half. In the past 18 months and even at ECH we are trying to engage more contributors to work on eip bot as we know that shashank has been working with Alita and looking into the issues which are reported in eip bots issues but we are trying to make the process more community contributor based like people should be finding it very
easy to come forward and help us with any issue to make it more manageable. I suppose he has some thoughts on documentation and processes that he would like to share.

**Shashank Yalamanchi**: Yeah so I was thinking so currently I don't find any documentation or process as to how one should be contributing eip bot or also how does the eip part even work, so maybe having a documentation in place of the process of contribution and the understanding of how the eip bot is working at a code level. Maybe adding more comments or having or having a general spec for the eip bot would make sense, so that any dev who wants to contribute to the eip bot can just loop in and look at the documentation and start contributing so that improves the process of me or elite or some other main contributor to the eip. What not having to be present at all times to communicate and you know dispense information. It will become easier for the devs who are trying to contribute from the contribution point of view if that makes sense.

**Micah Zoltu**: So I will push back slightly on that with any given project. The act of
Writing documentation is quite time consuming and so you have to weigh the benefit of the documentation. Does it outweigh the cost of writing it for some many projects that definitely I
wasted like because you get you know 10x, 100x effort versus payoff. So if you have some piece of code that's likely to be interact with by hundreds or thousands of developers then having documentation is critically important because it allows one person to help inform
thousands of others. If you have a piece of code that is worked on by two people very often. The active writing documentation takes far longer than just having those two people talk to each other and so the thing that I would be curious about before we sink a significant amount of time into documentation is do.We think that the eip bot is going to attract a significant number of contributors and authors or do we think that it's probably just going to be one or two people.

**Shashank Yalamanchi**: I think that would depend on how much do we want to automate a stuff using the eip not  right because if there are too many tasks being added or being pending on the eip bot then maybe having that documentation or maybe a basic documentation in place not a maybe detailed one just a basic as to how the eip bot is kind of working like what are the workflows and stuff like that. Would it make sense?

**Sam Wilson**: Something minimal like contributor guidelines or yep okay. Because maybe how to get involved would be a very worthwhile section writing without going into much technical depth.

**Shashank Yalamanchi**: Sure, because I think most of the open source projects do have some sort of contribution guidelines right? SoI  think that would be a good first step.

**Micah Zoltu**: I am assuming you want something more than what's in the readme there
that is linked.

**Shashank Yalamanchi**: I was just initially wondering if  a dev is trying to read and trying to
contribute, maybe having this basic understanding of like okay what's the code exactly doing but that makes sense because it actually takes a lot of time to write the whole documentation. So yeah maybe just the contribution guidelines would be sufficient I suppose

**Sam Wilson**: Yeah so from a quick scheme of the readme maybe just like a statement that you know it's open to contribute contributions from anybody and like that kind of thing, I am not sure.

**Pooja Ranjan**:  Well the idea is to decentralise the work. I know today Shashank, yesterday Alita was working on it today. Also she is contributing but we are trying to decentralise the contribution and I think  this contribution guideline is like what if people find an open  issue how they would want to respond to it. Obviously if they would look into the readme that is already existing, will give a brief idea of what this depository is all about and it would be just nice to have a small contribution guideline that may not consume a lot of time.

**Shashank Yalamanchi**: Already wrote that contribution guideline. But I am still not sure as to what exactly eip bot is doing. When does it trigger? Why does it trigger? What's the end goal of the eip bot?  What is it currently trying to do? Right, like what does the pipeline of the eip bot look like? Is what I'm trying to get at?

**Miah Zoltu**: So right now, we currently have two bots and that definitely doesn't help with
clarity. Actually I think we have three or four bots. Technically I can appreciate there being  some value in just having an outline of what roles the different bots have. Why do we have multiple bots instead of what is the general high-level process for the bots? It is a type of documentation that's a little bit easier to write than like more formal documentation it's more
just a descriptive high level overview. Yeah I can, that might be a good task for Alita if we think we're going to get multiple editors.

**Shashank Yalamanchi**: Not just that, maybe all the contributors might not be available all the time,so tomorrow if I leave or Alita, someone else leaves or someone just wants to join in, yeah.

**Micah Zoltu**: The solution we have had in the past to that problem is just to write a new bot.

**Pooja Ranjan**: well we have spent a decent amount in the past 18 months on these. Like you know, improving processes if we can improve the process by adding some documentation. Like adding some effort and documentation. So we do not have to rewrite the bot again. I suppose that would be helpful for example yesterday in the eip editors internship meeting. There was this guy who came up with a new proposal or new set of codes which was again I believe is a set of improvement in the present eip but I understand that he may not be very clear about how it actually works, so I obviously have pointed him out to Alita and Shashank. But I suppose that it would be useful. Yeah Shashank if you have anything on that particular script too.

**Shashank Yalamanchi**: Are matching to the original eip1.Framework or sorry template
and now the another issue is the  board that arita wrote isn't typescript right automatically running on javascript so now another another confusion is should we add should we merge these boards or should we keep the parts upright should we add another flow so this just
complicates the task of adding new bots. so I was saying yeah so basically I and Alita agree on the point that there should be a single code base for the bot and we shouldn't be having multiple bots because that just increases the complexity of maintaining all those individual bots and like now you have to reach out to the authors of the bot to understand like what's going on and it just becomes too complicated. so having a single bot in a single code base makes sense instead of having multiple bots maybe.

**Micah Zoltu**: I tend to agree with that.

**Pooja Ranjan**: I suppose a decent compromise here would be  if shashank would like to volunteer or one like to work on the documentation part look into the process because  I know he is trying to get involved with the eip bot issues more and more so it would be nice to have him look into the process and documentation that they think might be
useful to add over there unless it is like too big of a task and it is like too much of time consuming.

**Shashank Yalamanchi**: Well I was actually planning on working on that already, so I just wanted to. 

**Pooja Ranjan**: Sorry we keep losing you Shashank, but it looks to me that you are already working on the documentation part, so maybe we can revisit this particular item in the next meeting and see where we are and what else is required to be added. Yeah I can see that I will thank you so much for this. Before we move on to the next item I see a comment here which I think we can address right away about the eipv. It's not a comment actually Micah just shared the link for resources we had discussed about. The placeholder for eipv in the past meetings and I was supposed to work with a third of Devops team to get the right access. Luckily I got a response from jimmy today and he did mention that he would like to bring it up with the devops team and it's very much hopeful that this can be moved to the ethereum repository soon, so that's an update.  Yeah I am happy that at least we are moving in the right direction. All right, anything more on item number two. Okay I see a comment here , so I will submit the draft for you guys to check and see if any changes have to be made. eah that would be nice, thank you Shashank.

# 3. [EIPs Insight](https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/) - Monthly EIPs status reporting

**Pooja Ranjan**: Moving on to item number three it's about eips inside it's a monthly report that we share every month on what's going on the eip editing site.I have shared the report for the month of January so far like up till 12th of January. We have four new proposals added as draft. All these four proposals are of erc categories. There are two proposals which are moved from draft to review and one of those is already moved to review to last call. In total we have three proposals in the last call eip 3448, 3607,and eip 3668. The deadline is 24th and 25th January. So if anyone has any comment concerns related to these proposals or they want any further improvement or any suggestions are there please look into the proposal and join the discussion to link at fellowship of ethere magician. So your concern should be addressed before they finish their last call deadline and if there are no major changes we hope to see these proposals getting into final status very soon. Other than that there was this one proposal 2098 which was moved to stagnant by the part but the author is
very much interested to pursue the proposal. I will suppose it is an informational proposal and this is brought back to a review status. There is one eip one related change or like we have made this small edit to have this consistent documentation of eips in eip1. So eips are generally called eips irrespective of their category so we just try to make sure that the eip1 shows the consistent documentation. There are a couple of final proposals which had minor edits going on. You can check out the entire eip's improvement proposal inside for the month of January to take a look at the details of the eips that's about it.

# 4. EIP editor apprenticeship meeting

**Pooja Ranjan**: The next item is the eip editors apprenticeship meeting. Yesterday we had this meeting and recording was made available. You can find that recording even from the agenda or also it is available on Ethereum Cat Herders on youtube. It's good to see that more new people joined in the last meeting. There was someone who was entrusted into erc related editing, so we hope that these meetings help newcomers to join the community and eventually start contributing in the reviewing process. Anything so far like comment questions.

**Micah Zoltu**: Nope 

**Pooja Ranjan**: all right

# 5. Other discussion topics Ref: [Comment](https://github.com/ethereum-cat-herders/EIPIP/issues/101#issuecomment-1011094223)

**Pooja Ranjan**: I think the next item is going to be a little interesting, so last week we had a meeting with william and trichon the lead author of  eip721. That meeting was so if people are interested to learn about the proposal and some use cases. The recording is available on ethereum cat herders youtube after the discussion. He shared some of the concerns that he initially had when the eip process was evolving and he listed a list of tasks or maybe concerns that he would like the editors team to look into and if that could be helping in improving the present process. I have added the list in the comment section. I don't know if
anyone want to pick up anything specific to discuss. I mean I was looking into it. Some of these things I think are already addressed but yes.

## Add mission statement [ethereum/EIPs#1128](https://github.com/ethereum/EIPs/issues/1128)

**Pooja Ranjan**: Okay the first one is about the mission statement. It seems like the proposal is now stale and closed. Okay I see the last comment from Micah,  yeah if you have
thoughts on that.

**Micah Zoltu**: I am reading it right now to remind myself this is a very long time ago.

**Pooja Ranjan**:  I know this is a last minute entry. I should have added this list earlier. We don't have to discuss all of the things today but I just wanted to share the list so whatever we can cover today would be nice to have 

**Micah Zoltu**: Regarding mission statements. I am fine with them just indicating you know why we do eips. I guess that's fine. I mean that my gen Ialso don't have a strong desire for them at the same time. Like it's not the same where i'm like oh yeah we definitely need a mission statement. It's critical for our success. It's more just if people want a mission statement. I am  totally fine with the first line readme which just says eips are standards.

**Pooja Ranjan**: Right I think a mission statement is very much closer to the problem
statement here like what problem are you actually trying to solve which you think can be a standard and this problem is actually being faced by different applications or you know clients so but I am not sure if there would be something added to the eip and if that would be some general consensus and changes to eip template would be required. Do you have any thoughts on that?

**Micah Zoltu**: Sorry I got distracted reading this thread. Say the question again.

**Pooja Ranjan**: So my understanding is this mission statement should be very close to the
problem statement and if they are trying to mention that okay. This is the generic problem that other projects or dabs may face and this is why it should be considered as a standard then probably it should be added to the eips and if it would be then we might want to update
some of the eip templates maybe something added.

**Micah Zoltu**: So I don't think he's suggesting we add a mission statement to each eip. I think he's saying we add a mission statement to the eip's repository. Am I misunderstanding that I think he wants a mission statement for like github.com/ eips

**Pooja Ranjan**:  Well I think you are right. I was wrong. Yeah it's about to read me that makes sense.

**Micah Zoltu**: And that's where I am satisfied  with what we have in that opening sentence like I don't feel a need to have more but if third parties are finding that is not explanatory enough then that's also okay like I don't mind expanding on it.

**Pooja Ranjan**: Sounds fair. Do you have any thoughts or concerns on this Matt.

**Lightclient**: I am okay with it. I don't think it should go on every eip.

**Pooja Ranjan**: Yeah I totally understand that it was my mistake sorry. All right then we can probably update him and if you would like to add something there he can always come back and make up a request.

##  Rewrite README.md and index.html with a focus on our audience of builders and end users (I will create PR if somebody that cares about this can call me briefly)

**Pooja Ranjan**: All right going on to the next one rewrite readme and index.md with a focus on our audiences of builders and end users. So he obviously suggests that he is willing to take a lead and creating pr.

**Micah Zoltu**:  We have talked before about how currently the readme/ eip1/template/eips repository webpage/ethereum.org all cover the same thing in slightly different ways and with slightly different words and it's confusing and it's not clear who the target audience is for each of them and we have talked about fixing that before and I would still like to fix that  general issue and I think this falls into that. This is I believe more or less the same problem
where we have the readme and eip1and index.html that kind of could just use being rewritten like they have just been mutated over time over and over and over again and they just ended up in an unhealthy place. So I am not against that one. If someone wants to go through it the hard part is finding someone who wants to go through and clean all that up.

**Pooja Ranjan**: That makes sense and as per the comment it looks like he's already
willing to create a pull request for that. So I will communicate that and maybe when he does
if there is anything to be improved or changed or if it's just fine it can be merged.

##  Increase accountability of core EIPs

**Pooja Ranjan**: All right the next one is increase accountability of core eips i mean to me
it is a little unclear like how but I don't know if you guys have any thoughts on it.
yeah i don't know what that means
that's a little weak

**Micah Zoltu**: and same thing in the next one i'm not
sure
what i mean by the next one

##  Increase interaction (RSS, email list (yes really))

**Pooja Ranjan**: Yeah the next one I understand is it's increased interaction rss email
list and with the talk I had a feeling that he is looking into that rss feed to be more active and if possible someone can maintain the list of emails who are looking for this. You know the rss fee. I don't know how much it is possible in real life. Is it really possible to have this kind of
list maintained anywhere?

**Micah Zoltu**: We already have an rss feed I believe.

**Pooja Ranjan**: Yeah but I am not sure. I am not subscribed to that so I'm not sure if it is still going out. Is it?

**Micah Zoltu**: I don't know if it breaks. I don't know who maintains it or where it's hosted. I just know it existed at some point.

**Pooja Ranjan**: Okay maybe some research work in this direction can be done if you still find value in maintaining their services feeds and emails. Now that there are so many processors involved and we are trying to provide information on different channels. But yeah I think if people are interested in having feeds. We can always invite them to update it. If it is not being updated

##  Recommend a specific place for discussion that are off topic of EIP repo

**Pooja Ranjan**: Moving on to the next one is to recommend a specific place for discussion that is off topic of eip depot that's something different. So far we have been recommending that this is the right place to discuss everything related to eips. I am not sure what he means. 

**Micah Zoltu**: It's very broad. They mean off topic like where do people go to talk about covid or is there somewhere in between that they're hoping to like what is the specific scoop they're looking for?

**Pooja Ranjan**: Yeah right maybe I can get more clarity from him or I would ask him to maybe join the next meeting or add comments to this agenda and we can bring it up next time as well. Yeah please go ahead.

**Micah Zoltu**: I just agree

**Pooja Ranjan**:  Thank you.

##  Provide platform for EIP discussions, disallow official discussions outside of our platform (avoid link rot)

**Pooja Ranjan**: The next one is provide platform for eip discussions at this allow official
discussion outside of our platform avoid link road, so I think we have made significant process in the past few months on moving the discussion to fellowship of ethereum magician
and making that as an official discussion forum so this I think is actually taken care of.

**Micah Zoltu**: okay

# 6. Review action items from the [previous meeting](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20046.md)

**Pooja Ranjan**: All right I think that's all from the list going back to the agenda items. We have covered almost everything except this last one review action from the previous meetings. So I am quickly looking into it and from the last meetings looks like we have three
action items or decisions make peers to call. All eips in the documentation and not years is for eips but erc category.This has already been merged  number two was continue discussion to move all discussion to and pre-draft to ethereum magicians. Yes we are trying to enforce that moving all of the eips related discussion to link to fellowship of ethereum magician and the third one is to merge Greg's pr for him to receive notification for eips. I suppose that is already done. So that's all from the last meeting and the one I already have updated Pooja will talk to devops and not for an appropriate placeholder. We have shared the information that we received and it should be taken care of. That's all from the items listed here anyone has to bring up anything. Well it was a good meeting and we tried to catch up on things that we left last in december and looks like we have some new tasks and activities to involve more. I am really happy with the progress of eip bot that we are doing recently. I noticed the tag that I suppose bot is providing like as soon as a pull request is created it says that it is about status change. It is about general updates. It looks really nice
and yeah I hope to keep improving the process with the help of this meeting so people who are listening to these calls if you have any questions and concerns reach us. The eip editors and the cat herders teams we are available on ech discord on eip editors channel share your concerns with us and we will try to bring it up in the future meetings. Thank you everyone for joining us today. Hope to see you all in two weeks on January 26th.

**Micah Zoltu**: Thank you

**Pooja Ranjan**: thank you, have a good one everyone, thanks.
 
---------------------------------------
# Attendees

* Micah Zoltu
* Pooja Ranjan
* Sam Wilson
* Lightclient
* Shashank Yalamanchi
* Stefan

# Date for Next Meeting: 26 January 2022 at 1500 UTC.





