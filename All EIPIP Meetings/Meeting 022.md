# EIPIP Meeting 22 Notes
### Meeting Date/Time: Wednessday 2 December at 15:00 UTC
### Meeting Duration: 1 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/43)
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=FUEaz9YrP0g&feature=youtu.be)
### Moderator: Pooja Ranjan
### Notes: Avishek Kumar

----

## DECISION ITEMS

**DECISION 22.1**: People on the call agreed that there should be stronger rule for discussion to. A PR will be created to add this in EIP-1 after the next meeting if no strong opinion otherwise.
**DECISION 22.2**: Will be discussed in the next meeting when  James will join.
**DECISION 22.3**: Bring back to the next meeting when Micah is present.
**DECISION 22.4**: Cat Herders will start reaching EIP authors to change the status of the EIP. 
**DECISION 22.5**: Brent would continue looking into it.
**DECISION 22.6**: Publishing will be holded till Edson gets word with James on where to publish. 

## ACTION ITEMS

**ACTION 22.1**: Edsom will contact James to decide where to publish the EIP status blog.

## 1. [Stronger rules for discussion-url](https://github.com/ethereum/EIPs/issues/2967)

**Pooja**: Welcome to eipip meeting 22. The first item on agenda is stronger 	rules for discussion url . When you click the 	link that is coming from the issue that was created sometimes back 	by exec. We wanted to pick up some of the other issues that are 	there in the eips ripple. So the first one is a stronger rules for 	discussion. So far we have been recommending ethereum magician forum 	for discussion for any of the proposals but it's just a 	recommendation. Do we have thoughts on should it be recommendation 	or should it be you know a little more stronger than recommendation. 	 	

**Light Client**: I am all in favor of it. I am happy to have it stronger than a recommendation. I am happy for your requirement. 	
	
**Pooja**: I think there would be two questions related to it. Number one what 	is the ideal place for discussion tool and number two would be a 	strongest recommendation for that so. Are we on the same page about 	the discussion to place that it has to be fellowship of ethereum 	magician that looks good to me but yeah.
	
**Light Client**: Yeah I mean that is my preference. I think that having it 	available for people to use. The issues is also okay that way if for 	some reason they don't want to create an account on another website. 	They can use github which they already need to be having an account 	on. I think that we could disallow ease research. I think that is 	not really ,the appropriate place for eip discussions anyways. So I 	think that just a preference of the magicians but a requirement that 	it is either east magicians or the eip repository issue. That is 	what I would say.
	
**Pooja**: With the eip repository issue. The one downside that I see is like when the eip is merged. It is generally recommended to close that 	issue but with it magician there is nothing as like you know closing 	the issue and that is open forever, so how do we want to like you 	know, what is suggested here is like you know we should be adding it 	to eip1 and you know adding a recommendation or may be the stronger 	version of recommendation. Is it something that we would like to 	create a pull request saying that the discussion took place. Is a 	fellowship of a theory magician or .
	
**Light Client**: I would like that.
	
**Pooja**: okay, then we can add that. As you know I mean I am not sure if we 	should add that as you know one of the outcomes of this meeting 	today because we have less participants . Will mention it as what 	the present group think and if there is no strong opposition then 	we'll try to create a pull request to update that. sounds 	reasonable?
	
**Light Client**: Yep sounds good.
	
## 2. [Handling Retroactive Changes](https://github.com/ethereum/eth1.0-specs/issues/12)	
	
**Pooja**: 	Okay the next item is handling retroactive changes. It is coming 	from the at one dot, oh specs I think like client you have created 	an issue about that eip261 is the example cited here.
	
**Light Client**: Yeah I am not sure if this is the right. Group to discuss 	this with but I am but I say I am curious to your thoughts even if 	it is not there is the cip the ip2681. I guess whatever yeah 2681. 	This is basically changing the transaction. The validity 	requirements of a transaction retroactively up until we this was 	agreed on in the last all-court devs. It was theoretically possible 	to have an account whose once is incredibly high something that 	could be represented in you know an arbitrary length integer and 	what was decided on the call is that we would have a stricter 	requirement and set a max max cap of for an account nods to be two 	or sorry two to the 64 minus one. 	
	So 	it is the highest that nodes can be and this is something that as of 	when this was decided upon last week and I assume it is still true 	today. There are no accounts who are even close to that and so the 	decision was to make this
	happen 	retroactively meaning that we would just say this is actually how it 	always was from genesis that way. We do not have to really include 	this in a fork it is. We are just saying that it is going to have 	always been thought of as true
	because 	there was nothing that invalidated it up until now. I do not know 	what the correct way to handle this is in terms of documenting the 	change because the ethereum you know improvement proposals. This is 	that's kind of the document that describes ethereum but it is not 	the not exactly the full specification but neither is this e1 specs 	repo. It kind of seems like the yellow paper is the main 	specification and so I do not know if anyone has any thoughts or 	comments of what the appropriate method for documenting a change 	like this is.
		
**Pooja**: 	Yeah I think this item we can bring it back when we have you know 	more people. I mean right set of people to answer this. Thing I mean 	it is coming from network upgrade repository . So, my thought was 	James presence would have helped you .
	
**Light	Client**: Yeah that is what I figured too that sounds good. 	
	
## 3. [Implementation section](https://github.com/ethereum/EIPs/issues/2940)

**Pooja**: 	Yep, moving on the next item is Implementation section. This is 	again coming up from the eip repo issue.
	It 	talks about like, should we have implementation section in the eips. 	I do not know if people have thoughts on it.
	
**Light Client**: I think Micah is probably the biggest proponent for making this not making eips not have the implementation 	section. So, it is kind of unfortunate to not discuss that with him. 	I like i probably are both on the side of possibly having it. I 	think there are some cases where it makes sense to have an 	implementation section in the cases where it is you know some sort 	of erc. I think that those are the best cases for having an 	implementation section and the core changes were the implementation 	section links to a change in a client. I think those are the less 	good cases for it.
	
**Pooja**: 	Right I wish Micah has joined the call but due to some outage power 	outage in his location he would not be able to make the call today. 	so let's move it to the next meeting. I just heard from Hudson also 	unfortunately he is also not able to make the meeting today. I am 	wondering should we continue with the rest of the items? what do we have here?
	
## 5. Single source of truth for EIP

**Light Client**: Is there anything we feel like we can make decisive action 	on without Hudson, Mica or James?
	
**Brent Allsop**: Yeah just the next item eip repo cleanup that is the one I 	am working on right?
	
**Pooja**: 	Right I was about to say that. 	
	
**Brent Allsop**: Yeah the only update I have is let's see pull up my 	notes here. I have I am trying to get a hold of William Entrekin 	because he's done some work and made some progress on this. But I 	can not get him to respond. So I am also gonna try and contact Sam 	Richards or Josh Stark. I have not done that yet but plan on 	reaching out to any of those and if anyone else has any information 	of who at the ethereum foundation or the ownership that owns that 	website that might be able to help me or or give me access ,so we 	can try and make some improvements there if anyone has any more 	information. Anyway that is work in progress, I am continuing to 	work on that. That's all I had. 	
	
**Pooja**: So I believe , you are talking about a single source of truth right?
	
**Brent Allsop**: Right, yeah! There is right now there is eips.ethereum.org 	and there is also ethereum.org/eips and they are sort of like copies 	of each other but we should have one or the other and William and 	Tradekin has done some research and found one is by far used the 	most and so we are talking moving towards that one, but anyway there 	is some other cleanup that needs to be done but so yeah.
	
 **Pooja**: So I believe exec also had some thoughts on that about single source 	of truth for eip's repo and that we did earlier.
	
**Brent Allsop**: Okay, that is good I will try and reach out to him too 	cool thanks.
	
## 4. EIP repo clean up.

**Pooja**: 	Okay so one another item is eip repo cleanup. The intention behind 	adding this was like we were
	looking 	into proposals to you know kind of filter out? which are in draft ? 	which are in steel ? I know most of the eips have been if they are 	still they have been removed or marked still with the help of both, 	but there are still some eips which are therefor you know more than 	longer duration that it needs to be in the state of last call . So 	would it be the right time to look into the proposals again and 	reach out to the authors. What is a general thought here?
	
**Brent Allsop**: I thought we were going to wait until Ii guess do we have 	a well-defined set of states that the eip can be and I thought we 	were just waiting until we had that well-defined state. Then once we 	have that state then we are going to start contacting all the 	authors to. See if we can push things along.
	
**Pooja**: 	Yeah that was the last decision made but now that we are having some 	clarity on statuses and that is already added in eip 1. Sometimes 	backwards.
	
**Brent Allsop**: Okay ,cool yeah so in other words can we start contacting 	eip authors again and start pushing things along.
	
**Pooja**: That is my thought is but if people have different opinions.
	
**Brent Allsop**: Yeah that would be fun to start pushing forward with that. 	Matt if you may have any suggestions
	or 	comment here? I know I mean like the bot is working but if there is 	anything that can be done and would be helpful for the cleanup.
	
**Light Client**: I think the best thing that can be done is to avoid 	commenting on repositories where the bot has marked them as stale. 	In those cases, if we mark if we comment then the timer resets and 	if the bot is going to clean that up, we have to wait again three 	months or whatever the threshold is sort of ought to intervene. So I 	would say if there are issues that you we want to comment on that 	have not had the bot comment or someone else commented after the 	boss did and we wanted to comment and that is okay but if the bot 	has commented no one has responded
		it 	is probably best to just leave those until applause does it 	automatically.
	
**Brent Allsop**: So in other words once the bots commented on them that is 	the final state and we want to leave them there or is there some 	state after that we want to get him to. 	
	
**Light Client**: Yeah there is one more state after that well the bot. I 	think makes two comments it marks something as stale, meaning that 	it has not been interacted with for a period of time. I forget 	whatthe exact time
	is 	and then maybe a week after that it will close it or two weeks or 	something like that it will actually close the issue.
	so 	if someone comments in that intermediate time, it will reset the 	counter all the way back to zero.
	
**Brent Allsop**: Okay so in other words but then once it is closed then it 	is closed.
	
**Light Client**: That is the end 	
	
**Brent Allsop**: That is the goal is. It is cleaned up. okay cool good to 	know thanks for that.
	
**Pooja**: 	So one question I have I mean it is a kind of confusion even if it 	is closed on the github. Repo but the status won't change if it was 	already there in draft in eips.ethereum.org. Will it?
	
**Light Client**: All right that's a good point that is true that is 	something that I guess we will need to have manual intervention for 	now. So I guess that. Yeah I think I was thinking maybe the bot does 	that but it does not yet. Do that it only closes the issue. So the 	things that are actually closed. Would need to be manually moved to 	whatever the preferred inactive stages abandoned or.
	
**Pooja**: 	Yeah so how we started sometimes back was looking into that 	eips.ethereum.org and from there. We picked up eips which are either 	in draft or last call or any other status but final we made a list 	of that and were trying to reach out to author asking if they would 	want to pursue this or not. So even if most of the issues or pull 	requests have been closed by bot marking them, still if we find that 	something is still there in last call. I think that can be a 	starting point for us to reach out to author.
	
**Light Client**: Yeah I agree.
	
**Brent Allsop**: So help it sounded like you were talking about, just 	eips.ethereum.org as if that was different than ethereum.org /eips 	what is I thought those were both built from the eip repository and 	deposited in those two locations via some build process but but are 	those different then is that is my understanding and correct?
	
**Pooja**: 	As per my information the difference there is ethereum.org/eips 	does not list the eips. Which I mean what kind of what category of 	eip it is or what state it is only eips.ethereum.org list that.
	
**Brent Allsop**: Oh okay, I got I will need to do some more research on 	that then thanks.
	
**Pooja**: 	So I think that is one action item we can mark it on cat herders and 	we will restart working on it. We have the sheet maybe we would want 	to clean up more the sheet and fresh it up and start working on it 	again. 
## 6. EIP status blog/document

**Pooja**:  Moving on the next item is eip status block slash document, I 	guess Edson is working on that document and he recently submitted a 	draft . Edson would you like to share and talk more about the talk?
	
**Brent Allsop**: You are on mute and if you are talking.
	
**Pooja**: 	I am not sure him we are not able to hear him but I may have the 	draft let me share the link if people would like to give it a look 	or maybe leave some comment and feedback for that. Sure, I shared 	the link in the chat. So if people have thoughts and comment on the 	article. We are planning to publish it on ethereum cathode is 	blocked. This generally states about what are the current statuses 	that the group agreed upon. It is already documented in eip1. Just 	this explanation of how we are moving along the process of 	standardization.

**Light Client**: Is this going to get published to the ethereum.org blog or 	is this only going to go on medium.
	
**Pooja**: 	The plan is to put it on ethereum cat herders blog.
	
**Light Client**: Okay 	
	
**Pooja**: 	Yeah I mean because we have access to that only. So if it is 	something that should be on a broader scale. we can probably share 	it or i don't know if there is another suggestion for that or any 	other better place for it to be
	published.
	
**Light Client**: Yeah I am not sure what the right place. Is it just seems 	that you know chain large changes to the theory improvement process. 	Is you know a pretty big change in my opinion.
	
**Brent Allsop**: Sounds good to me.
		
**Pooja**: 	So I am sorry, I did not get it properly. So where I mean would be 	the right place maybe on the github repo of ethereum dot spec.
	
**Light Client**: I do not know about the ethereum specs repo. I would say 	you know these changes are already going into the eips repository. 	You know via eip1 where the change was made and so people who follow 	along there would see that this is happening. so then it's a 	question of how do we announce it what are the right channels
	to 	announce it and I mean.
	
**Brent Allsop**: Did you mention any ethereum.org blog.
	
**Light Client**: I don't know sorry I just cut out perspective. I was 	getting a phone call. I did not hear what he said friends.
	
**Brent Allsop**: Yeah, you mentioned something about an ethereum.org blog
	
**Light Client**: Yeah there I mean there's the ethereum.org blog where they 	post a lot of. You know things that the ethereum foundation is doing 	and that varies from you know updates of guests to informational 	posts about their
	research 	to their grants to protocol related stuff like you know the genesis 	of e2. These are things that they post and so I feel like this is in 	that kind of category of informational things about ethereum that 	they could post on and I do not know you know I do not know who the 	right person as they ask about that is. Probably James Hancock would 	know if that would fit in.
	
**Brent Allsop**: Yeah that is yeah if James Hancock's the best one. we 	should definitely look into that. I think see if we can get it 	posted there.

**Pooja**: 	Right so we will like hold the publishing it on the characteristic 	medium right now, if people have feedback on it, feel free to 	suggest and then I will check with james on this.Okay thank you for 	that suggestion.
	
**Brent Allsop**: So who that sounds like an action item to me. Should I do 	that or do you want to do that pooja or we should wait till we have 	James in the next meeting or.
	
**Pooja**: 	I think Edson would be the right person to do that.It is his blog so 	I am not sure if he is unable to mention atm and talk here but I 	will communicate it to him.

**Brent Allsop**: Okay cool thanks.
	
**Pooja**: 	We will mark it on as an action item to get in touch with james too.
	
## 7. Review action items from the previous meeting

**Brent Allsop**: okay, so the last item from here is a review action item 	from previous meetings and Yeah there are a few things so some 	decision makes an action item needed. Decision mates were funding 	for eip editors on that we had a small discussion in cat herders 	meeting. I would be reaching out to ethereum magician people to 	first you know check with them if they are comfortable for editors 	funding because the idea was if this eip is very much close to the 	fellowship of ethereum magician people. so let them have this 	funding thing for eip editors if at all we would
	like 	to pursue this idea and if not working then cat hurdlers can help 	out with the requesting of fund and distribution as required as 	needed. But I think the the first step here would be to decide if we 	would like to go with this idea of funding. How many editors are 	there and if they are actually interested in being funded. May be in 	one of the future meetings we would like to bring up this as a 	discussion item. Like if we want to pursue that the next decision 	made in the last meeting. Was like client is now an editor 	congratulations and thank you very much nightlife for ofoffering 	your services are gonna data we were looking for more people to help 	out with.
	
**Light Client**: Yeah

**Pooja**: 	Okay, 21.3 states uh discuss issues from the network upgrade 	repository here. We did try but in absence of sufficient people or 	the right set of people here. We could not make any decision we 	would like to bring it up again in the next meeting. The action 	needed was 21.1 contact Nick Johnson about the eip merch bot.
	
**Light Client**: That was done.

**Pooja**: 	Oh it is done okay we can mark it as closed. okay so that's all 	about it.

**Brent Allsop**: So is Nck Johnson then volunteered to be someone that can 	make changes to the merge bot that we request and stuff like that.
	
**Light Client**: I do not know, I need to re-look at the discussion that 	happened. I think that the main outcome was just that we were sure 	we were you know. We figured out that for sure, he is the one who 	was running it we figured out where it IS located and he said that 	he could add someone to it. So that they could restart it in the 	case that there were issues which was the main thing, We were 	looking for but nobody really was it. You know Committing to making 	actual changes to it.

**Brent Allsop**: Okay sounds good thanks.
	
## Project board	
		
**Pooja**: 	Okay so I was saying that I want people to look at the project board 	that is there in this repository. I am sharing the link in the chat. 	So when we started this group of eipip the intention was to improve 	the process as well as support the eip repository that is already 	there to clean it up to make the process streamlined and all these 	things. We have made good progress here. We have finished so many 	tasks that we started in the beginning of this year. The group 	started in january 2020 and by the by the end of the year we made 	good progress. So if people have suggestions what other tasks or 	action items. We can consider for this group feel free to add here. 	We are already
	working 	on eip repo cleanup. There were two things I think is missing. We 	sometimes back we talked about having a
	document. 	I am not sure if we have that document for eip editors right with 	roles and responsibilities. Did we miss it out somewhere? Okay I 	will look into that I think it was on somebody's action and we may 	have missed while carrying the meeting notes. So that was there one 	important thing that I find here is define a process for reaching 	consensus on core eips. Is it worth putting in a future meeting 	agenda?
	
**Brent Allsop**: What would that involve in other words. If there is a 	controversy or something like that or what would that involve? 	

**Pooja**: 	My thought is general idea of like we dohave a general process, but 	the unclear part is like how do we reach on consensus like it 	happens in the all core dev meeting but I mean I came across this 	hing like for core proposals consensus are made in all code of 	meetings. Just one person or two person say I mean one client or two 	clients say it is there but there is no defined line so we want.

**Brent Allsop**: Yeah that seems totally ambiguous and confusing and 	expecting people to browse through those notes and everything to try 	and find out what status everyone is on. Anyway my thinking is we 	need to have some definitive source where people can say if you are 	in if you are for this. You sign this petition if you are against 	it. You create an account anyway just in my opinion.I think everyone 	knows my opinion on that but I think that would be a great help if 	if we could say singles and also you have to be able to jump camps 	if you are not onboard. You need to be able to jump off and if you 	are not onboard jump on and track all that rigorously just my 	thoughts.

**Pooja**: 	I think as of now, with the one dot or spec repo we are trying to 	get some clarity on that like if we look into the yellow v2 or v3 	document md file. There we are trying to mention like which client 	is okay with what proposal or they are planning to implement it. 	This may be good as per the core eips are mentioned there but for 	some other eips like networking eips, we do not have that process so 	it never gets clear like if those eips are ever implemented in 	clients on. If at all implemented what all clients have implemented 	or willing to implement. I am not sure if you would like to get 	clarity on these sections as well.

**Brent Allsop**: Yeah that is both of those things are critic. It would be 	great to just have a single source of proof, have a process where 	everyone could know go to a single source and find out what is the 	current state-of-the-art state of that. 	
	
**Light Client**: I am afraid that this may not be the best group to tackle 	that. I think that this is something that it is
	unfortunate 	how the process currently is but you know it is really run by client 	teams and client teams sort of dictates what goes into the protocol 	what does not and I am not sure that we can come up with a process 	for them. The only way we could hope for a process is if we did it 	together with them and you know my experience of working with them 	is that they are really busy and they don't have time to mess with 	this sort of stuff right now.

**Brent Allsop**: Right yeah but basically I am just talking about a 	communication process where all of the teams can like communicate to 	everyone else. What they are and are not implementing and who is on 	board and who is not on board and that kind of stuff.
	
**Pooja**: 	Yeah I mean, I find this as you know an area of opportunity that can 	be the gap can be reached. I understand that client teams may not 	have the kind of bandwidth to document these processes or how to do. 	They think about it but if we get some senses of the decision making 	process. Possibly documenting them and sharing
	them 	with people in the form of blog as we are doing it for statuses of 	eips and others would be helpful but just a thought. 	
	
**Light Client**: I guess I think that there are things that we can tackle 	within the eip repository that is that we would be better suited for 	and I mean those are things like trying to have more separation of 	concerns in terms of the types of eips that we have. I know that 	Micah wants to just totally remove erc type eips from the repository 	and see. I think these are things issues that we could really make 	progress on. I am afraid that we would spin our wheels
	a lot and I would have to discuss exactly what we want to do in terms 	of understanding how you know the network	upgrade 	process works and to actually write those documents. But you know my 	experience in being a part of some of those conversations is that it 	is incredibly opaque and trying to write a blog post it is going to 	be hard because there is not much. There is not really a great there 	is not really a process that is followed. It is more just constant 	discussions and a lot of those discussions happen privately within 	the guest team things that we are not privileged to anyways and then 	the results of those conversations are the sorts of things that we 	see bubble up on all core devs. So I do not know if that is the best 	place to spend time working I think there are other things that we 	could do.
		
**Pooja**: 	Yeah I think I am getting there. We do not have to mess with the 	current process. I get that part I mean we could use the time to get 	some areas where we can be actually helpful. 	
		
**Light Client**: So I mean I would love for. You know I would love it if we 	could help make the network upgrade process less opaque and I feel 	like you know six months ago that was something that I also felt 	strongly about
	this 	berlin hard fork a lot you know a lot more with the eip. I have been 	helping champion with Micah. I just realized that this is a really 	complicated process and there is not a process that is really 	followed and we just see that weekend or you know every all core 	devs whenever we try and decide on something. We will circle around 	for an hour and come kind of back to the same point. There is no 	rhyme or reason it is just everybody's trying to do the best that 	they can to think about what's the best to the network.

**Brent Allsop**: So it sounds like to me you are talking about exactly, 	there should be a petition of what someone wants to do and everyone 	that agrees with that could sign that petition and that could be a 	dynamic petition and if
	anyone 	disagrees they could create a competing camp and say I do not like 	that for x y z and people. Just and you measure and so you can 	really track who is on board with what and who is not on board and 	why and what requires to get everyone on board and track that in 	real time in a dynamic petition system. 	
	
**Light Client**: I mean that is essentially what is happening right now in 	all core devs and on discord it is just we do not have the 	formalization of these petitions and I do not think that is 	something that the core does are going to be amenable to in the near 	future. I think they feel you know incredibly overwhelmed with the 	amount of things
	that 	need to happen to the theorem protocol and they don't want to go 	through add additional bureaucracy to decisions that are already 	very hard for them.
	
**Brent Allsop**: No no no no the problem is now they spend hours and hours 	going hashing over and over and over and no one knows any of the 	decisions made. I am saying reduce all that work and just make a 	concise statement on a petition, say I am for doing this who is and 	is not on that and it seems like to me that would
reduce 	everyone's work and communication would all be natural. Anyway just 	a thought.
	
**Light Client**: Yeah I mean you know on paper that sounds amazing and it 	sounds like it will reduce things. But the 	problem is that I think some of the things that are being discussed. 	It is not easy to synthesize into a petition.
	You know the great example is just the work that we have been doing on 	type transactions. The questions that have been coming up are things 	that we did not think about at the previous meeting they were things 	that just you know continue to come upm during the implementation 	phase.
	
**Brent Allsop**: That is why I am talking about a dynamic petition that 	constantly changes and improves because
	you 	have a petition, so you can submit a change in a wiki kind of a way 	and then everyone that is supporting gets notified of those changes 	and if no one objects within 24 hours it goes live and you can 	assume unanimous consensus and that way you can track who is and is 	not on board in real time and it becomes easy and so you constantly 	change that petition. Trying in other words you do negotiation for 	the people that are not on board and
	say 	well if we made this change to the petition, would that get you on 	board and then you submit that to the petition and if no one objects 	then you can assume that everyone that has signed it still agrees 	with that change so
	so 	it is not just a static petition. It is a dynamic petition.
	
**Light Client**: Yeah I mean I hear you are saying. I think that sort of 	happens informally by a discussion on discord and the number of 	people that are involved in those discussions are small enough that 	people generally just have an idea of who is on board and who is not 	on board.

**Brent Allsop**: Yeah it needs to be able to scale so thousands of people 	can be involved inthe process. 	
	
**Light Client**:The thing is I do not think that thousands of people will. 	I do not know if they will ever be in this process. I think that 	this is a process that will always be limited to sub 100 people and 	I am not saying it is a scalable. I am not saying this is scalable 	as it is there are things that should be done to improve the system. 	It is you know I just do not know if yeah I do not know what the 	right way to go about that is and I do not think that we can really 	go about it without enfranchising more of the core developers in the 	work there is no way that we can just impose something upon them and 	say here is this great process. We have come up with on our own. It 	has to be something
	they 	really want to take the lead on and I do not think at this point 	that they do once want that.
	
 **Brent Allsop**: That makes sense yeah to me it takes someone who wants to 	do something like violate the state of the chain that critically 	needs to be done that is a hard decision and if someone wants to do 	it, they can start a petition say I want to do this and then people 	can start getting on board say, yes I want to do that and start 	building consensus and and so it is a tool for someone that wants to 	do something to make it change. That is primarily what it is so if 	someone right now I am it seems frustrating to me because especially 	violating changing the state of the blockchain everyone's. Just 	afraid to touch that because they are going to cause a fork and no 	one wants to go there but if we can not do that ethereum's going to 	be stuck in the mud and if someone wants to champion a petition. We 	need to find out a way to formalize that and make that so that we 	can make those kind of decisions on large scales.
	
**Pooja**: 	So I just wanted you know get people's attention to the project 	board to mention that we made good progress. Now if we want to take 	some more tasks that can be added here. So that is I think that is 	that covers all
	four 	items that were discussed if anyone has anything. We could not 	address some of the items today. We would like to bring it back to 	the next meeting. 	
	
**Light Client**: I have two questions, the first one is you know regarding 	sort of the I guess the project board but also just higher level 	what the this group's goals are and I guess I was wondering is this 	a group that expects to carry on in perpetuity are there always 	things that you think that there that will need to be done or the 	script needs to handle or is there kind of an end goal that this 	group wants to get to that says okay. We have achieved what we have 	wanted to achieve and now we are complete.
		
**Brent Allsop**: I mean yeah I think there are two steps number one we 	want to redefine the process so we have a clear defined process then 	what then that is the primary goal but then once that done, my goal 	is is to participate in an ongoing basis. Maybe not as it is as busy 	as we have been but to constantly be working on cleaning up eips and 	reporting back and say what have we and have we not accomplished and 	what eips can be cleaned up and coordinating who is going to try and 	clean up. What I eip to me that is I thought was a long term effort 	.

**Pooja**: 	Yeah I mean my thought process is also very close to what Brent just 	explained like the idea of having this group was to get the process. 	You know improved and if we started with eips because that was the 	area which
	needed 	most attention and that is how we renamed this group as eip but if 	in the process we find that there	are 	certain other areas where help can be provided, it is good it's 	okay we would be happy to do that.

**Light Client**: Yeah I think that one thing that is sort of eip tangential 	that this group could really help a lot on that.I hink would be very helpful is to create a specification for eth1 	in the same vein as the e2 specification
	because 	right now in my mind that's one of the biggest missing pieces of you 	know understanding standards in ethereum 	and understanding the protocol is that there is not no good single 	source for information and if this group could help facilitate 	someone to build that. I think that would be incredibly useful in 	both the aspect of improving. How standards are written and 	understood and improving. How things are discussed in terms of 	network upgrades and the protocol itself.
	
**Pooja**: 	Yeah that sounds good.I think we can start thinking over it as well. 	I mean like the idea and now that we are moving ahead we should 	consider all these sessions where it can be provided and makes 	things better for community to reach out to.
	
**Light Client**: Sounds good see the one other thing was is that and I know 	Edson's not here now but I think he was the one who was leading the 	effort on building some resources to onboard eip editors and so I am 	still willing to go through that to give feedback on it.
	
**Pooja**: Yeah I think I mentioned that we missed it somehow in the process. 	I mean like in from the meeting notes. It is where it was missing 	but I will talk to Edson about it and we'll try to bring it in the 	next api meeting 	
	
**Light Client**: okay
	
**Pooja**: 	okay so, I think that is it for today if anybody has any other 	question or anything? So the next meeting is in two weeks december 	16. Thank you everyone for joining. I hope that we have more people 	to make a decision on the items that we missed today. See you all in 	next two weeks thank you.
	
**Brent 	Allsop**: Thank you.

## Attendies

* Pooja Ranjan
* Brent Allsop
* Jim
* Lightclient
* Edson Allyon


## Next Call - Dec 16, 2020.

