#  EIP IP Meeting 5 Notes
##  Meeting Date/Time: Wednesday 11 March at 14:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/8)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=MrJAHvyrg04)
### Moderator: Hudson Jameson
### Notes: Jim Bennett

----

## SUMMARY
This meeting including a presentation from Sam Richards, a web developer at the EF, about migrating EIP information to the Ethereum.org website. Discussions incuding improving or replacing the bot that helps manage EIPs, as well as conversations about changing EIP 1. 

**Hudson Jameson**
Hi, everyone. Thanks for joining. And today let's jump right into the agenda.

## AGENDA

# 1. 1. Migrating EIP content to ethereum.org - proposal discussion

First up is a proposal by Sam to migrate EIP content to ethereum.org. So, Sam, do you want to go over what this proposal is, and then we can discuss it?

**Sam Richards**           
For sure. Hello, everybody. My first time here. I'll just introduce myself quickly. My name is Sam. I am a web developer at the Ethereum Foundation. I mostly focus on Ethereum.org, which is primarily on this education improving on-boarding, particularly for developers entering the ecosystem. Previously, I've just worked at various web agencies, doing a lot of SEO and user testing and web design. So this is an exciting area for me to help out the Ethereum community.

So what I was asking about in Telegram, and why I wanted to chat with you guys, it's really not so much about changing any of the EIP process per se. It's focused on whether there is an opportunity to increase exposure and overall awareness of the EIP process and EIP content. I linked out to  a GitHub issue, which shows a lot of the context of where this proposal started. And it's really just around, "Can we improve SEO and discoverability of the existing EIP website?" I think it's an excellent resource for people to find a specific EIP they're looking for or browse existing ones and see what their current status is.

The TL/DR is just that website does not rank at all. If you search any given EIP, it probably won't be on the top two pages. So the thought we had was, "Well, what can we do to improve that?"

What we've tried so far is just a lot of optimizing meta tags on that site to be more targeted in terms of the keywords that it's going for. And we've also added links from the core Ethereum.org domain in the footer, for instance, on various resource pages to try to push organic traffic that way and signal to Google and all the other search crawler bots of the Web to let them know this website exists and is important and is valuable. So far, that really hasn't accomplished much.

So the proposal I'm putting forward is that we keep the existing EIP repository as is, because it's great for what it does, but mirror or migrate that content so that with every new EIP that's merged, we could set up an automated process that would push that to a page on Ethereum.org. I listed out the reasons why I think that's cool and exciting, but the main ones are really increasing exposure and awareness and discoverability of EIP content and growing awareness of the process itself. And hopefully to just increase the UX of that experience for people trying to learn and read about content.

Some background on that - with Ethereum.org, we fortunately do have the resources. We're currently working with a contract designer to roll out some design updates to that site. We are actively working on features such as site search that exists. And I think there's a lot of those aspects and feature development that we could benefit from if we were to merge two of these sites together.

So what I'm looking for from you folks are what your overall thoughts on this proposal are, what information you might like to know, what concerns or doubts or questions you have. And also, what are my blind spots? Because I'm coming at this from a very particular angle. I'm sure I have a somewhat biased opinion, given that I'm already working on this website. So I'm looking for as much feedback as possible on what we think of this and how we might go forward or how I might gather additional input from the community. So with that, I don't know how these meetings work, but I would open it up to questions.

**Tim Beiko**
My general feedback is that this is a great idea. I have some specific implementation detail questions. But conceptually, highlighting EIPs on Ethereum.org feels like an all-around win.

In terms of specifics, is it too much to move all the EIPs website to Ethereum.org? Or do you want to have a page Ethereum.org that explains the TL/DR of what EIPs are, and then link out to the actual EIP web site? I can see a case for both, because it's a bit of information overload to go on the EIPs website. So maybe if you have a one-page explainer and then perhaps, like the newest EIPs or the EIPs associated with the upcoming upgrade or something like that, a subset of them that's curated? That's a bit harder to do because you need to curate them somehow. But it seems like it might just be more valuable, because this way, people aren't just looking at a list of 150 EIPs without any context.

**Sam Richards**             
Totally. That's a great question. And the short answer is both. Whether or not we do decide to migrate the EIP content to Ethereum.org, I absolutely think on Ethereum.org, we should have a beginner's introduction to how changes to the protocol happen and explain the EIP system. I think that's something we can and should accomplish regardless. And then I would probably envision that resource after an introduction, probably linking to the most common standards.

**Tim Beiko**             
Yeah, I think that would be really good. And maybe the intro page - I think Ethereum.org links to a bunch of videos that talk about this. So maybe linking to a few of those and whatnot, and giving some feedback on what it is and then provide the option to dive into the details.

**James Hancock**             
I've been talking to Sam a little bit about this and definitely support doing all of this. This may sound extreme, but I would rather replace the EIPs page entirely and redoing that and having having it be done. And the reason comes from a practical sense. For example, I tried a proposal to change the header to add a champion's field to the EIP. A barrier to that is someone needs to then update the EIP site to be able to render it. But we haven't had anyone to do that historically, so we've just said, "I guess no one's gonna be able to do that." So not having people behind the web side is holding back the updating-the-EIP process side, and in general, it just isn't really very usable. And without people who are focused on usability, it won't ever get anywhere.

**Hudson Jameson**               
I agree. And I think that this is a great idea as long as we have redirects from the old EIP site to the new one, because that's heavily linked out. We also need to separate the translation effort from the overall proposal that you put there, because the translation project is a big effort. However, we should design the new site so that it could easily be translatable. So maybe integrate Crowdin, but don't use it until we want to use it. We could maybe do both at the same time. That's more for the next meeting's discussion. I guess once this is more fleshed out, but I know you were probably looking for an up-or-down before this was more fleshed out. I'm guessing.

**Sam Richards**           
Yeah. And I would definitely be looking for you folks on some guidance around what next steps would be. I'd be happy to put together a more formal proposal. At this point, I thought I could just link to the GitHub issues so you guys can see the discussion and get some context. But yeah, definitely open to ideas on where to go from there.

**Tim Beiko**               
I think one thing we want to do as a next step - a more formal proposal is really good, but just getting the buying from the EIP editors, there's the Gitter EIP Channel, and I think they are all people who will have good opinions on this stuff.

**Hudson Jameson**            
And a lot of them don't even visit that some of the time. So I'm gonna talk to the editors, because I'm an editor, and I could just reach out to them as well. We should also go to that Gitter repo and post to see who responds. But I'll also reach out to people.

**Sam Richards**                
Yeah, that seems like a great idea. And I have chatted with a couple like Hudson, I know we've talked about this. I did have a call with Nick Johnson, who had some skeptic points that he brought up but was overall not opposed to it. But I definitely agree it's worthwhile just getting everyone's input on it.

**Hudson Jameson**            
The other thing is, would you reuse Nick Johnson's bot and improve on it or completely scrap it? Do you know?

**Sam Richards**               
So at least a start, my thought would be to not touch or change that aspect of the process. I think that we can keep as an isolated piece of the system, if you will. The way that I'd imagine, at least initially, implementing this is any time in an EIP document is merged into the EIP repo, we have Travis or some automated GtHub bot watcher just grab that same markdown file and copy it over into the Ethereum.org website repo, which is also primarily generated from markdown content. So I'm definitely open to helping out in improving that bot. I've heard there have been some issues with it, but I think that could be its own stand-alone initiative.

**Hudson Jameson**                 
I think the bot needs to be improved importantly because I think it shouldn't be its own stand-alone initiative. And the reason for that is it whenever you submit an EIP - so if I'm writing an EIP, and I have it on and it's just a brand new, fresh EIP pull request, the bot checks the header file for compliance, and then if it's compliant, it shifts it to Draft. And then if you get further along in the process and editors approve of it, then it gets put to Accepted, or whatever the next step is. But it always checks that header file. So if you're gonna make a bot that does that anyway, I think reusing and upgrading his would probably be a faster and better process. Because then we'd have two bots going that we'd have to upgrade simultaneously whenever something new happened with the header file. It's already grabbing and converting it to markdown, so most of the work's already done on that bot.

**Sam Richards**               
I see. Okay, yeah, that sounds fair.

**Hudson Jameson**               
It's putting it in a Jekyll file, but you can do whatever you want with it. In fact, once we would probably have the bot push to both sites until we switch over. And then once we switch over, we'll just disable the bot for the old site. And we can get Nick Johnson's approval for all this.

**Brent Allsop**              
Sorry, I'm kind of clueless, but when you say "old site,"" are you talking about eips.ethereum.org?

**Hudson Jameson**  
Yes, exactly.

**Sam Richards**
We're already calling it the old site. It's the current site.

**Brent Allsop**                  
Yeah. I just don't think there should be two of those. Because when I first tried to figure out what EIPs were, it's hard to find where the official stuff is.

**Hudson Jameson**             
Not two of them. I should have been more specific. I don't want to end one site until the next one's up. But otherwise, overall, it's sounding like everyone's for this. If you flesh it out a little bit more, Sam, then we can pick apart the pieces, maybe set up a different Telegram group of people who are super interested in doing this, so it could move along faster than these EIP IP meetings. That's that's my suggested next step -  formalize and then connect with us. You're in the EIP IP Telegram group, right?

**Sam Richards**               
I am, correct.

**Hudson Jameson**             
Yeah. Just tell us when the next step's done, and we can set up another Telegram room and get some of us who want to be super involved in any website meetings that would be dealing with this, because it sounds like this would flood into the Ethereum.org meetings that happen with part of the community, right?

**Sam Richards**                  
Right. And we are moving towards monthly community calls, so I'd be happy to share that info with all you guys.

**Hudson Jameson**                 
Okay. Anyone else have comments on this?

**William Schwab**              
Yeah, I do, actually. The new site is also to supersede GitHub, or are EIPs are still being submitted in GitHub?

**Hudson Jameson**
Not supersede GitHub from my understanding.

**William Schwab**                 
Okay, we're only talking about the old EIP site on Ethereum.org.

**Hudson Jameson**
Exactly.

**William Schwab**
Okay. Just wanted to have that clear. Great.

**Pooja Ranjan**              
If you feel it like that, Sam, to get more visibility and get more off feedback on this, we would love to include that in our newsletter to share with the community to get more feedback about this process. And then probably again share the proposal. I'm gonna share that, too.

**Sam Richards**                    
Yeah, thank you. That'd be great. I think the more eyes on it and input, the better.

**James Hancock**              
As I've been thinking about things that would be really big value-adds that it could offer in particular around the EIP-centric process in highlighting where things are as far as the EFI -  something that was has been requested from the community recently is a visual way of seeing the EIPs going through the process. We don't really have a way to do that at the moment.

**Hudson Jameson**              
Oh, like a little map or something at the top of the EIP page, maybe even a little animation that's SVG or something like that that goes from Draft and has an arrow pointing to the next step, but that next step is yellow or something. I'm kind of visualizing it. I'll have off to write it down in MSPaint or Photoshop or something.

**James Hancock**               
Even more specifically on the EFI, things that are eligible for inclusion and where they are in that process and then seeing it. And seeing where things are and what the next steps are so we don't get another "Oh, this EIP's in what status? Nobody knew."

**Hudson Jameson**                
Yeah, the biggest hurdle with changing the EIP process that then gets reflected on eips.ethereum.org is the fact that Nick Johnson's bot doesn't have documentation. So only those who really dive in know how to do anything with it. But if we upgrade the bit and fork it, make it better and then have documentation with it, someone like me or James or someone with Python knowledge could go in and do it.

**Brent Allsop**              
Yeah, I took a stab at that. Gave up pretty fast.

**James Hancock**     
I do know a little bit of Python, so I could actually help with that. I'm not amazing at it, but my old life was a Python life.

**Hudson Jameson**            
Sam, who's on the ethereum.org team that does Python? Do you do it?

**Sam Richards**         
It's been a few years, but I would be happy to take a look. I mean, that's part of this investigation. I assume, like you said, it sounds better to work off the existing bot, improving that and add functionality to copy over this content to Ethereum.org. So it's definitely something that I could help look into.

**Hudson Jameson**                 
And real quick, just for my knowledge, is this a Jekyll-based site, or is this something completely proprietary? What's it doing?

**Sam Richards**               
Ethereum.org?

**Hudson Jameson**             
Yes. And then also what the EIP site would be, since I'm guessing it's more of an extension of it than a whole new thing.

**Sam Richards**                 
I believe the current EIP site is a Jekyll.

**Hudson Jameson**            
It is. I mean, sorry, I meant if there's a new one being created.

**Sam Richards**                  
No. So ethereum.org is a ViewPro site, so it's based off of GIS, but it's very similar to Jekyll in the sense that it it's a statically-generated website. So from markdown source files, it will create and build actual HTML output. So the fortunate piece of that is that they're very compatible together and could work well without too many surprises.

**Hudson Jameson**                
Okay. Sounds good. Any other comments or questions? All right. Thanks so much, Sam. We'll do the next steps I talked about earlier, and thanks so much for bringing this up. This is gonna be a really good change for every everything.

**Sam Richards**  
Awesome. Yeah. Thank you for the feedback, guys. I'll try to get a more phone formal proposal to you guys at some point next week.

# 2. Code of conduct ref. Ethereum Cat Herders: Code of Conduct

**Hudson Jameson**                  
Great. Agenda item two is the code of conduct referring to the Ethereum Cat Herders code of conduct. I didn't make this agenda item. Could someone tell me if this is a change to the ECH stuff or if this is a thing for the CoreDevs?

**Pooja Ranjan**              
I have added that. It is actually a carryover from the past two meetings that we were trying to come up with the code of conduct for general Ethereum platform - the Gitter or the other telegram platform. It is just a carryover and it was initiated by Dano, but I don't see him again in this meeting. So if anybody else has any update on it on how to proceed on that we can go ahead, discuss it, are maybe in the next meeting, bring it to the agenda.

**James Hancock**               
Mine is less on doing a code of conduct in porting over and figuring out what ports over. But I do think it would be good to have some guidelines written around how GitHub works that doesn't exactly work well. There are certain things that GitHub can do that we've had normal expectations around how to manage those features. That's because it wasn't made to do the EIP repository's kind of work. It was made to be a code repository. So some examples would be it would be good if it was a norm for EIP editors not to approve their own EIPs to Draft. Or it would be good that other editors don't change people's pull requests and don't edit them on behalf of other people without permission. Because technically you can, because usually you're in a code environment, but this is a standards environment. So there I think there are certain things like that it would be good to clarify.

**Hudson Jameson**                 
I completely agree with James, and I'm saying that if the person who made this part of the agenda is referring to making a code of conduct for discussing EIPs within the repo. I think that should be low priority, because most of it's civil and most of it is outside of the EIP repo into Ethereum magicians where they have their own spoken or unspoken code of conduct, and they referee that. So, yeah, that should be low priority, in my opinion, except for James's idea. But that's less of a code of conduct and more of an instruction guide. I'd say. Right, James?

**James Hancock**                  
Yeah, It's expectation and standards.

**Pooja Ranjan**               
Okay, So I'll get in touch with Dano and with James, and we'll try to work on this agenda item and see where does it go. So we can probably move on to the next agenda item.

# 3. Progress on change in EIP status and repo cleanup

**Hudson Jameson**               
Great. Number three is progress on changing the EIP status and repo cleanup. The first sub-item is Brent's PR change to the status of EIP 3.

**Brent Allsop**           
Yeah, speaking of code of conduct, I did the pull request to change that status, and I had some stuff that I had included in the bottom in detailing some notes of what I was doing, why I was doing it, and whose approval I got and everything, but someone else, I'm not sure who accepted it, but they totally changed all that. Basically, all they did is change the status from Draft to Abandoned. But there was discussion going on that it shouldn't go to Abandoned. But it got accepted in that state. So that was kind of confusing to me, because I didn't have any control over that. They totally overrode my pull requests and basically just changed the status. So I didn't know if if I did it wrong, or if that person really did the right thing, or what is the process.

But anyway, it's been accepted. And the only thing that change is the status changed from Draft to Abandoned. Pooja and I were discussing it shouldn't go to Abandoned because that could be resurrected, but she was saying maybe it should go to superseded, and the original author says, "Yeah, it might be superseded by the 6465 rule stuff, and I tried to do some research on that, and it looks like EIP 150 might be a superseding to that, but anyway I'm just kind of lost there at the moment.

**Hudson Jameson**              
Yeah. And I think part of the reason this is gonna be difficult at first and we might want to put a pause on it, in my opinion, is because if we're redoing rules for EIP 1, what we're gonna end up doing is changing a lot of these statuses and then going back and having to re-justify or at worse, re-change the status again once we come up with a definitive status process. The ones we have right now are probably gonna stay, for the most part, is my guess. But we might need to include, especially for ERCs a better word for one of them and then go through all the EIPs and change it.

So I think that it might be good if, until we get new editors and there's an actual on-boarding process for editors, where that we have some of the expected rules about discussing this with people on a PR, and we have the new EIP 1 stuff that we  wrap up on over the next, hopefully, six months. Because I know these things could go slow sometimes. We might put this on pause, but I want to hear what you think, Brent, because you've been working hard on this, and if you think it's worth it or not.

**Brent Allsop**           
Yeah, that sounds great. Exactly. Because when that happened with that one, I basically put all my work on pause because I want to know the way it's supposed to be done so that I can help do it right. And until we know what that is, I'm definitely okay with waiting.

**Hudson Jameson**              
Yeah, Let's just do that. I'd say anyone else have comments?

**Pooja Ranjan**                
Yeah. This has started from the list of EIPs that we started to clean up. And as per our discussion, it has been mentioned that Martin was the author and Martin said that it should go ut it gets lost in there. So as you are suggesting that we should be working on the new EIP editors, I tried to list of some selection criteria, and I was thinking of creating a Google form that may be distributed among the CoreDevs who would like to be a part of the EIP process and would like to be an EIP editor to support the process. So I have listed some questions here and would love feedback from people and know how we can proceed. This is something of very high priority to get more EIP editors on board. And I'm looking for these steps, the processes that we should be following here.

**Hudson Jameson**                 
Okay. great. And this is for selection criteria. Okay, I had seen this Google sheets before, but it has more stuff now. Great.

**Pooja Ranjan**                      
Yeah. I mean, to the next item on the agenda, I found that there are some EIPs which are in Final Call for about six months or so on. I am interested in finding out how we can get these things moving. How should these EIPs be changed, because I'm not sure if these EIPs listed here in the Final Call are still a valid EIP. That's number one. And if it is, why is it not in the final Accepted state. How we can change the state?

**Hudson Jameson**              
Got it. So I guess the consensus here is to put the cleanup and changing the state on hold and focus on both improving EIP 1 until we're satisfied, and on-boarding new editors and coming up with a process that the old editors agree upon. Not necessarily, but that would make it easier. Because although I technically have ultimate authority from a settings and GitHub and technical perspective to add editors, I'd like to have the buy in from the editors we currently have before doing that.

**Pooja Ranjan**                
Yeah, that sounds like a great idea. So we should be focusing on Ethereum for EIP 1 and on-boarding more EIP editors. So any further ideas on this on-boarding process would be great to have, if not in this meeting, maybe in next meeting, we would like to discuss something on priority.

**Hudson Jameson**        
You mean set up a state of priorities for each thing we're doing?

**Pooja Ranjan**                   
Yeah.

**Hudson Jameson**               
And also, some of them are going to require an order. Most things, in my opinion, are on hold until EIP 1 gets edited. And the reason I'm saying that is, for instance, the EIP bot is gonna have to have new features based on feedback from EIP 1. And the changing and cleanup of the EIPs is gonna have to wait until EIP 1, and the role of editors is something that is in EIP 1, and we'll want to change before we bring on new editors. So I think if we spend the next month or two months focusing on EIP 1 and also getting a clear understanding of how we can approve those PRs that we're gonna talk about in a few agenda items from now, I think that would be valuable.

**Pooja Ranjan**                  
Sounds great.

**Hudson Jameson**            
Other comments?

**James Hancock**
There's one thing I get thoughts on from the group that could be something we do in the shorter term that I have been trying to work on for a while, which is - and I've got buy in from most of the EIP editors at this point - which is that EIPs that haven't been touched for six months should go inactive and having the bot do that automatically, and in fact, having the bot do that for all of the EIPs at once, and then having that be a starting point for a lot of these discussions.

**Hudson Jameson**                
Interesting. So explain your thoughts behind it being a starting point for this stuff.

**James Hancock**              
Because if the bot came in and changed my EIP to abandoned, I might be upset if I haven't abandoned it. But there's a lot of stuff that just kind of disappears and a lot of people that aren't even around anymore and hard to find. So going into each EIP and trying to figure out the status of each one is gonna be a ton of work. And some of that will more directly lead to something, and then some could be just lost into trying to find someone who never even cared about it anymore.

So if we have the first step be a everything that's older than six months that hasn't been touched gets moved to inactive, then anyone that cares about their status can say, "Oh, well, actually..." And then it makes room for people to interact with the process and have that be a standard moving forward, where if something doesn't happen on an EIP for six months, it gets moved to inactive. That isn't a value judgment; it's a part of the process, and it can always be moved to wherever else it ends up going.

**Hudson Jameson**                     
Yeah, that sounds really good. Is that active currently in EIP 1? I'm blanking on that.

**Pooja Ranjan**             
I don't think so.

**James Hancock**                
It isn't.

**Hudson Jameson**             
Okay, so we can't do that step until EIP 1 is changed, right?

**James Hancock**              
That one part of EIP 1.. I'm not sure if a complete overhaul of EIP 1 would be needed, but just adding in one status that all the EIP editors agree with feels like an easier thing to do than trying to change some of these other things.

**Hudson Jameson**               
Yeah, and we can change EIP 1 incrementally. That's another thing to kind of discuss if we need a PR to overhaul a lot of aspects, a bunch of PRs to overhaul various aspects, or a combination. But I agree with you that this change can be put in, and then whoever wants to get used to the bot, this could be their first task to be able to get the bot to make everything inactive or something like that.

**James Hancock**               
Yep. And a community bounty for that, I think, would be how I've been thinking of a good way to have that happen.

**Hudson Jameson**             
Yeah, we could do. Ah, we could do a GitCoin grant specifically for this EIP initiative. Let's add that to the agenda for next time, because I need to flesh out that idea in my head. But whoever's taking notes, let's add that to the agenda next time.

Who has comments?

**Edson Ayllon**             
It might be good to announce that to current stakeholders in EIPs, current editors, authors, before it's executed. But other than that, it's a good idea.

**Hudson Jameson**                 
Yeah, it sounds like James talked to them, and if they like it, then we need to have at least a three-week discussion on the PR about it and try to advertise it on Twitter and Reddit. But that's more for procedural stuff. It's probably gonna get approved, but it would be unwise for us to just assume that we should go in and improve it without a Last Call phase and without a few other things.

So the big thing is these decisions that we make about EIP 1 and other stuff - most things need to go into Last Call, including EIP 1. So that's just gonna be a slowdown variable. Other comments?

**Brent Allsop**            
Yeah, I think that'd be great. It especially clean up the main Ethereum.org site, because there's a lot of Abandoned ones on there. That's a lot of noise. Makes it hard to read anything on that page not knowing what's active and what's inactive.

**Pooja Ranjan**               
I may have a question over here maybe to James. We are stopping the cleanup process for now. So when this bot is gonna change them to all inactive, what would be the next step then? Do we need to reach out to the editors of all the inactive ones and then start working from there? How's it going to affect the entire process?

**James Hancock**               
The next step for that, I would say, is when we do it, we have a "reach-out-to-here" if you have any thoughts or want to talk about any EIP that you've written. So that anyone who says, "Oh, hey, I want to x," and have some people on the other side of that be there to help them do whatever it is that they want to do with their EIP.

**Pooja Ranjan**
Okay, is there any role for the Telegram group that is there for a change of status to accept as a draft that has recently been created?

**James Hancock**                 
I'm not sure I understand your question.

**Pooja Ranjan**              
I'm talking about the telegram group that talks about EIPs.

**James Hancock**                
The merge-to-draft one that I made?

**Pooja Ranjan**                 
Yes, that's what I'm referring to. Is it something that is playing any significant role here? I'm asking this question because I may have been the one of authors whose EIP is there, and it is inactive for the past six months. I'm kind of lost as to where to move it. I submitted the PR; there was some discussion going on, and I have to flesh it more and then move it to Draft. So what is the next step for people like me?

**Hudson Jameson**                  
You can try to merge it. The bot should do something automatically. I'm not familiar enough with the bot to know, but I know drafts get automatically added as a draft. But are you trying to get it to Accepted?

**Pooja Ranjan**              
No, no. To draft.

**Hudson Jameson**           
Is it a PR or an issue?

**Pooja Ranjan**                 
It is PR 1925.

**Hudson Jameson**                  
Let me go to it and see what's up. Oh, it's closed.

**Pooja Ranjan**                
Oh, no. I may have been missing the EIP number, but that's fine. I'm gonna take it offline with James and you.

**Hudson Jameson**    
Okay, that sounds good.

**James Hancock**              
Just to give my thoughts on that, I created that the channel as a kind of a test to see what happened. The hope was that if we get all of the PR drafts into one place, then the EIP editors would have an easy way of finding it. I don't know if anyone here knows this. Maybe I should give background on the Telegram announcement group I made.

**Pooja Ranjan**               
So do you want to publicize this? Of course it is in the AllCoreDevs meeting, so people would know about it, but is it something that you're looking forward to getting it publicized? Or is it something that needs to be not very open to the public? What is the idea there?

**James Hancock**              
Publicized.

**Pooja Ranjan**    
Okay.

**James Hancock**               
if someone wants their EIP, their pull request to be put there, I'd be happy to to help get it to there.

The idea was to collect all of the drafts, all of the request for merge of drafts into one place so that they don't get lost in all the other places where the [arc?] is right now. It's kind of hard for all the EIP editors to find them. So my thought was, if we remove his much friction around that as possible to where EIP editors can just click, look, approve, and merge as being an easier way to help some of this process move along.

**Pooja Ranjan**  
Yeah, that basically answers my initial questions. Thank you so much.

**Hudson Jameson**
Right. Any other comments on that?

**James Hancock**             
And if people have feedback on that or a way I could do that better, or just general thoughts, I also would like to hear that.

**Hudson Jameson**              
Great. So the next item is selection criteria for an EIP editor. We went over that a little bit. That's just basically Pooja looking over that section of the Google doc and leaving comments, right?

**Pooja Ranjan**               
Yeah, that's correct.

**Hudson Jameson**                    
Any other comments on that? Okay, change status of EIP 233 and 2378 which is the upgrade meta EIP. And the EFI from meta to informational.

**Pooja Ranjan**               
I can give some background on that. This is coming from the EIP Gitter discussion. Somebody there suggested that they're not willing to accept an update to EIP 1,because there seems to be not enough information, and I do agree to that. Meta EIP 233 is kind of a template that is provided for all the upgrade meta going forward from Istanbul. Before that, we did not have this kind of template.

Again, the 2378, that is the EIP for EFI that lists all the EIPs that have been eligible for inclusion. So we think that it is something that should not be labeled as meta EIP, because "meta" makes it mandatory to be followed, but informational just makes it optional. So if it is good for EIPs that we are following right now. But EIP 233, we are trying to follow. My thought is that it's good to keep it as informational, and that was what was coming up in the EIP Gitter, but I would love to hear from other people what they think.

**Hudson Jameson**        
I think those should be in active status. I think the active status was made for ones that are going to be living documents that are changed, including EIP 1.

**Pooja Ranjan**                
That sounds good, too.

**James Hancock**              
Yes, and the hard fork meta one, the ideal for me would be for all of the information in those to go to EIP 1, because that's where that information should be. The actual registry of what is EFI and what isn't and where their status is would be an active EIP.

**Hudson Jameson**             
So the formal process for hard forks, that EIP, you want the whole thing transferred into EIP 1? Or do you want a reference in EIP 1 to it?

**James Hancock**   
So I've already done a PR to write the contents of what a hard fork is and all that stuff into EIP 1. What we would leave there would be the template. Or we could move the template into EIP 1. I see value in having any information all be put into one place, so we all know exactly where the single source of truth is for everything. EIP related. Fragmenting it out means people won't be able to find it.

**Hudson Jameson**                 
Yes. I need to think about it more, but initially I agree with you that having definitions, especially, for what some terminology means, should be in EIP 1 if it's very important, like hard fork/network upgrade. But then the template itself, because it's a little bulky, might need to stay in 233. And then we can just say we'll go to 233 to see the template.

**James Hancock**              
Yep. Yeah, something like that.

**Hudson Jameson**                 
Great.

The next time just says "next steps," and we already talked about that a little bit. Sam's next steps are to make the plans a little more formal, get more information on it, and then talk to us in Telegram and make another Telegram channel for people who really want to help, potentially make a GitCoin grant. Once that's more formalized in the next meeting, we can talk about specific steps like the GitCoin grant and stuff like that. And then put a pause on cleaning up the EIP repo and then additionally working on getting editor buy-in for some of these steps while we do changes to EIP 1. So that's how I understand what the next steps are for between now and two weeks from now.

What about y'all?

**Pooja Ranjan**                
Yeah, that was more specific to Agenda item #3, but yeah, that covers it all. So we're good.

# 4. Survey on the EIP process (target audience - core devs)

**Hudson Jameson**           
Great. All right. So item number four - survey on EIP process target audience to CoreDevs.

**Edson Ayllon**                 
Yeah, I can talk about that. These meetings, they're called "Improvement Process for EIPs." "Improvement" just kind of assumes it was changed in a positive way.

There are two fundamental ways to do that. You could either move towards something like a goal or set of values, or move away from something. Moving towards is usually called goal-setting; moving away is called problem solving. And then there's alternatives to that where you set up a system that solves problems automatically or a set of conditions that create a produced result automatically.

In the first meeting, Hudson started by asking frustrations from the group. I think that's good. That's a good way to identify problems to start solving them. A good idea would be texting that to more stakeholders. And an Easy, quick way to do that is with simple survey. So I was suggesting that we create a Google form and send it out to CoreDevs, EIP editors and past authors. It's just to get a general feel for what the state is currently for the EIP process and things that could be improved on, problems that could be solved. My suggestion would be just two questions: What are your current frustrations with the EIP process and what are your current fears with the EIP process. That would be a good indicator of what could be solved.

**Hudson Jameson**              
Sounds good to me. I don't see a downside. We might want to add, "Do you want to be involved in the EIP Improvement Process group?" And I would like to get background information for each person that is submitting a survey, and I don't mean super extensive. What I mean is like, "What role are you in the community?" which would be, like, EIP editor, EIP writer, community member, CoreDev, ERC writer, and then reference if they have written an EIP what's an example of an EIP they've written, and then a name. And the reason for that would be to rank, so someone who's never interacted with the EIP process, we want to take their opinions lighter than someone who has, I think. But I'll defer to Edson on that because I think you have more experience on that.

**Edson Ayllon**                
I think that's a good idea. Weighting them by past experience with the process would be very valuable for that kind of survey.

**James Hancock**               
I think it's a great idea as well.

**Hudson Jameson**            
And I can advertise it across stuff, as well as everybody else on the call. And we could put it in the newsletter and the cat herders Twitter, and then I could have the Ethereum account retweet it.

**Edson Ayllon**            
Yeah, I can help make this survey or make the form. I would need help with who to send it out to, as well as everything you just mentioned, which is great.

**Pooja Ranjan**          
I'll try to help out with the process, too.

**Hudson Jameson**                 
cool. I think those Google surveys can get converted to a CSV or a Google sheet that you can then share with people.

**Edson Ayllon**                 
I think so.

# 5. Update on proposed changes to EIP 1

**Hudson Jameson**             
Okay, perfect. Next up. Update on proposed changes to EIP 1 to reduce dependence on AllCoreDevs. That's a PR by Bryant Fubuloubu.

"During the great ProgPoW debates of 2019-2020, it became clear that the approval of CoreDevs for EIPs to move forward in the process..."

Okay. So this is just someone seeking comments for an EIP. He should have really put this on an Ethereum magicians post. I might suggest that as a comment, since this is a process improvement that's on a technical level. Well, I guess it's political too. I don't know. What do you all think?

**James Hancock**               
I don't know.

**Hudson Jameson**
Yeah, I'll have to look at this more. We can just skip this one and bring it up at the first of the meeting next time.

**Pooja Ranjan**                   
I have a question here. While creating this agenda item, I was trying to gather information on the topic that was under discussion and some of the other problems. So is it something that we should be continuing in future? Or is it something that can be dropped? Because I thought that these are some improvements suggested to EIP 1, and we give it a look in a big group and discuss something about it. If it's something good that we should be continuing, or we can just skip this part.

**Hudson Jameson**             
I think for the purposes of our meetings and improvements, we should skip it. I think this goes too deep in the weeds right now for what we're trying to do.

**Pooja Ranjan**        
Sure. I'll take care of that.

**Hudson Jameson**                  
Okay. The next item is "change hard fork to network upgrade." That's Tim.

**Tim Beiko**                  
Yeah. I haven't gotten much feedback on this, except overall, I think people were generally favorable for it.
spk_0                 

**Hudson Jameson**  
I like the idea as long as the first time "network upgrade" is mentioned in any document, it has "AKA hard fork" in parentheses.

**Tim Beiko**                  
Why? I would kind of disagree. I feel we had this conversation last time on the call, but it feels like a hard fork is a potential result of an upgrade, but they don't all lead to hard forks. I don't see them as synonyms.

**Hudson Jameson**              
Oh, I saw them as synonyms. Because in my opinion, on a technical level, anytime the network upgrades, there is always a hard fork because there is always a split in the network, even if it's for a second. And there's always at least one block mined on the other chain. And so that means the other chain continued on for X amount of time.

**Tim Beiko**                 
Yeah, that's right. I mean, I don't really have a strong opinion to that level of detail.

**James Hancock**              
I was on your side of "technically, it is a hard fork," but I came over to Tim's side and the way of always calling it upgrades. And part of the reasoning that got me was that while there's a technical definition of hard fork, there's a community expectation, and I see it all the time that a hard fork means there's a community split happening or a new coin is being made, which hasn't happened with any of the upgrades. So specifically, in Bitcoin culture, a hard fork means that there is a community split.

**Hudson Jameson**                
I think the definition is changing over time. I need it look into it and convince myself of that change is here or not yet. But yeah, great points. I'll personally think about it more. Other thoughts?

**Tim Beiko**            
I think, Hudson, if you listen to the recording of the call two calls ago where we discussed the PR, I think you'll get a lot more nuance.

**Hudson Jameson**         
Sounds good. Let's go to adding a table of contents to EIP 1, and then I think we should skip six and seven.  that what's the usual way to go about this? Because I've missed enough meetings that, um I don't know.

**Pooja Ranjan**  
That's fine. Most of the action items have been already been covered.

**Hudson Jameson**                 
Great. Go ahead, James.

**James Hancock**                 
It's a PR. It's in there, but I don't know the path of getting it. It's an EIP 1 that doesn't have a clear way of getting it into a state that it gets merged.

**Hudson Jameson**              
Is it just making a table of contents and that's it?

**James Hancock**                  
It's a table of contents, and I added the stuff from the hard fork meta EIP about hard forks and I changed them to network upgrades, so some of those could be split out, which has been on my to-do list. Just like the general path, it doesn't make sense to make an EIP to make up some of these changes. Or I would say we shouldn't do that. But then what do we do?

**Hudson Jameson**            
I see there's a description in the conversation, a section for the EIP centric model. The thing I would take issue with is - the EIP centric model ,is that well defined yet? Because have we even gone through it once, technically?

**James Hancock**                
The parts that are well defined, I included.

**Hudson Jameson**            
Okay. I almost wouldn't define the EIP-centric model in EIP 1. Rather, I would link to ideas around it until it's more fleshed out, and it's gone through an iteration or two, because then we'll have to just go back in and change it. And if we're down to EIP 1, then it'll be complicated.

**James Hancock**                
Yep. The reasoning for why I moved it into EIP 1 was that [unclear- Alex?] recommended that before I merged the draft that I move it into EIP 1. So that's where this kind of limbo started happening.

**Hudson Jameson**               
Okay, maybe split this out so that the EIP-centric model is its own PR and the other two stay in because the other two are not controversial at all, from what I can see. It's just porting content.

**Pooja Ranjan**                  
I have something here to say that I discussed in one of the meetings. That was related to the EIP-centric model itself. I was trying to encourage people here to add this process because the EIP-centric model is the model that we are going to do for Berlin. I'm not sure if we're going to continue or do a change, because for Istanbul, they did something something else. And it is highly probable that we should come up with some new or better alternative for taking this upgrade forward.

So my suggestion was to add a motivation section in the meta EIP of an upgrade, and in that we explained the process that is being followed for that particular upgrade. Because Ethereum is something one of a kind. We keep experimenting, and every time going back to EIP 1 and changing may not be a good idea, but what we can do to make this constant information available to the community is we keep it adding on the meta EIP for an upgrade in that we mention the process that we follow, and if it's changed, we don't have to go back and change EIP 1.

**Hudson Jameson**                  
Okay, so you're saying EIP 1 should include maybe a reference to the EIP that's an informational EIP. I guess this way would be that EIP 1 says the phrase "EIP-centric model" for the chart that has the hard forks, maybe?

**Pooja Ranjan**               
No. James's EIP already proposes something in which they are categorizing all the upgrades that have been done in Ethereum so far. I think I saw that they are also going to add meta EIP for Berlin that is coming up. And in that meta EIP of Berlin, we just mentioned the number of the meta EIP there, saying that for Berlin, we're gonna list all the things that will go into the upgrade.

So my suggestion here is when we are creating this meta EIP for Berlin, we should add a section of motivation which was missing in all of the previous upgrades but was present in the Muir Glacier, it was really a good thing to explain why we're doing it, how we're doing it and everything in one place. Because for every upgrade, the community will go to the meta EIP of that upgrade. That is the center of information for one particular upgrade. And EIP 1 will contain the name of that upgrade plus the meta before that upgrade. So we will not have to change it every time. We will just keep on adding as we go.

**Hudson Jameson**              
Sounds good to me.

**James Hancock**                   
I would I would rather work on getting a process for keeping EIP 1 up to date. So part of that, I would push back on.

**Pooja Ranjan**               
One concern here is that if we do that, then the previous thing would get lost somewhere.

**James Hancock**             
The reason I don't want to necessarily have EIPs that have part of the history of things is because there is a certain loyalty to the process that happens, and I saw this in the ETC repos around the ECIPs, where there was a lot of discussion about whether or not something should happen. But a lot of the people had strong feelings because of the process and not actually from looking critically. They were so strong on the idea of immutability that they didn't have a critical discussion about the topic at hand. They were talking about a meta version of the thing of the meta version, and it just became really an intractable way to have some of these conversations.

**Hudson Jameson**              
Interesting. Ok, I'll need to think about that more. I'll leave a comment today on that EIP that you             made.

**James Hancock**  
Yeah, and I got the feedback from Muir Glacier - his is from the from the EIP  editors - that that information shouldn't be there. It should be in EIP 1. My whole like context about why I proposed Muir Glacier, the feedback I received was that's irregular and not normal to how the process should go. So I'm not saying that we should do either one. It's like we should decide when we should be doing.

**Pooja Ranjan**                     
We should keep this information condensed somewhere, because I think that the information about the upgrade that we did for Istanbul is lost. It's very difficult to find it anywhere. It's not mentioned in the meta EIP of the upgrade or in EIP 1. And if we keep on changing, we are never going to get the history of that.


**Hudson Jameson**                  
I see both sides. Let's discuss it again.

The meeting is already over time. Thanks everyone for coming. We will meet again in on the 25th. Nothing's going on then that I know of, because all the conferences are canceled forever. So we will see all in two weeks. Thank you. Bye.

# Attendees

* Anett Rolikova
* Brent Allsop
* Hudson Jameson
* Guthl
* James Hancock
* Jim Bennett
* Pooja Ranjan
* Sam Richards
* Tim Beiko
* Wei Tang
* William Schwab

# Date for Next Meeting: 25 March 2020 at 1400 UTC.
