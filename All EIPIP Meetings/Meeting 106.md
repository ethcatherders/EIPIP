# EIPIP Meeting 106 Notes
### Meeting Date/Time: July 03, 2024 at 17:30 UTC
### Meeting Duration: 60 minutes
### [GitHub Agenda Page](https://github.com/ethcatherders/EIPIP/issues/340)
### [Audio/Video of the meeting](https://youtu.be/PKkJNqcozhw)
### Moderator: Pooja Ranjan
### Notes: Alen(Santhosh)

## Summary <!-- omit in toc -->
Summary | Description
-|-
106.1 | **ethereum/EIPs#8590**: Waiting on @lightclient 's approval.
106.2 | **ethereum/EIPs#8634** Was waiting on 3rd editor's approval. @xinbenlv approved it and is merged.
106.3 | **ethereum/ERCs#473** Keep the issue open. It could be a good Issue to be worked on by someone willing to make open-source contribution.
106.4 | **ethereum/ERCs#243** Keep the issue open. Need to be worked on.
106.5 | **Security issues with ERC-20 and ERCs in general. Ref:** #340, @Dexaran provided an overview of the issue and proposed solutions.
106.6 | **Blockers to merge a Pull Request:** Waiting for Editor Consensus: Many pull requests are pending agreement among the editors.
106.7 | **Blockers to merge a Pull Request:** Waiting for Author Review: Some proposals require the original authors to review and approve changes.
106.8 | **Blockers to merge a Pull Request:** Draft Status: Some EIPs are still in draft form and need further development before they can be merged.
106.9 | **Blockers to merge a Pull Request:** CI Tests Pending: Several proposals are waiting for Continuous Integration (CI) tests to pass.
106.10 | **Blockers to merge a Pull Request:** Client devs are looking for 'Draft` PRs to be merged sooner to move the discussion to the FEM page rather than on the PR itself.
106.11 | **Blockers to merge a Pull Request:** @SamWilsn agreed to the idea of merging Draft PRs & @xinbenlv also recommended the same for ERC proposals
106.12 | **Estd. timeline for merging Draft proposals** @SamWilsn demoed a tool that can help identify the open PRs to the editor in order of last engaged with the author. This will help get an estimated timeline by which the PR will be reviewed by an editor. The idea is to add this tool to the eips.ethereum.org. Editors will look into open PRs added to the agenda and merge them.
106.13 | **Estd. timeline for merging Draft proposals** Also, the group discussed merging the Draft PR with a minimum requirement. Most of the editing reviews will be done when the EIP is moved to Review status.

**Pooja Ranjan**
* Welcome to EIPIP meeting 106. This is issue number 340 on. It considers Ethereum Cat Herders GitHub repositories on agenda. We have some open issues and pull requests to take a look by the editors. And then we will look into some other discussion topics suggested on the agenda by, different users and authors will take a look at the monthly insight and, few other updates from earlier meetings.
* So starting with the first item, that is edits to Final Proposal. I see we are waiting on Editors decision. The PR number is 8590. 

# Update EIP-4788: specify the timestamp for 4788 ethereum/EIPs#8590 [Editor's decision] [0:49](https://youtu.be/PKkJNqcozhw)
**Sam**
* Yeah I'm okay merging this it does it require 

**Pooja Ranjan**
* We are waiting. because. Oh yeah, I think lightclient was not on the call last time and we could not decide on that. So do we want to? yeah. 

**Sam**
* Yeah, I don't think we can do anything about it. Okay. perfect. 

**Pooja Ranjan**
* Let me make a note of it so I can ping lightclients separately to maybe take a 

# Update EIP-1: Allow links to portal-network-specs ethereum/EIPs#8634 [1:34](https://youtu.be/PKkJNqcozhw?t=94)
**Pooja Ranjan**
* Okay. 8590. I see, next few PRs are already merged, so let's move on to the next, not merged, PR, which is 8634 on EIP 

**Pooja Ranjan**
* And the blocker here is again it seems like okay. Third approver. Okay. I don't know. Victor, could you approve this? Can you maybe take a look? And I think it requires three editors approval 

**Sam**
* Yeah. And we could also do a call for input if we really, really want to. Wait. Didn't we already do a call for input on this or did we not? 

**Pooja Ranjan**
* I think my bad. It was my responsibility and I missed on that part. No we did not do call for input for this one. 

**Victor**
* So, you know, my position. I think this is a general thing that we should approve. 

**Sam**
* All right then. Yeah. So you've approved it. It's good to go. 

# Resolve the EIP-7212 migration Ref: Comment [2:43](https://youtu.be/PKkJNqcozhw?t=163)
**Pooja Ranjan**
* Okay, great. So the next one is a miscellaneous issues and that may require attention. And the first one is oh wow. So resolve the EIP 721 to migration. Can we move it to the later part. I know it's going to be a little bigger. And we do not see the proposal on the call. So can we move it to the later and look into other stuff 

# Node.js actions are deprecated ethereum/ERCs#473 [3:04](https://youtu.be/PKkJNqcozhw?t=184)
**Pooja Ranjan**
* Yep. Okay. Cool. the next one is NodeJS action, a deprecated PR on ERC repository 473. I'm not sure if it is a genuine one or kind of spamming. 

**Sam**
* It's legitimate. Like okay, we do need to, we do need to update our things. Eventually they'll stop working. when GitHub drops support for the old NodeJS. but we don't need to do anything until then. 

**Pooja Ranjan**
* So is there any message that we can communicate to this, user like, are we gonna look into it? Or if it has to be looked after some time, we can just let them know. I think they are also pointing towards, pull request. That is, 202 for send sorry, collateralized NFT. 

**Sam**
* Yeah. So this isn't blocking anything. It's just annoying. Yeah. 

**Pooja Ranjan**
* Okay. So we can just let it open. Let it be open there. 

**Sam**
* Yeah, I'll get around to it eventually. So 

**Pooja Ranjan**
* Perfect. 

**Victor**
* Something that, Ethereum Cat Herders, could help. Let's say someone who is interested in helping out could actually try to, fork the fork it and test it that they can deprecate the 16, and the Node.js 16
* And get it work and then come back with a PR that you can approve rather than waiting for your bandwidth to open up to do it on your own, and also a good training for them. Do you think this is the kind of task, or do you think this is. 

**Sam**
* Oh yeah, absolutely. This is this should be trivial. literally just changing a 16 to a 20 somewhere. 

**Pooja Ranjan**
* So I don't know if this can be rewarded and created as an issue then some. Maybe we can give it to some new contributors. 

**Sam**
* Yep. Yeah. 

**Pooja Ranjan**
* Okay. Yeah. Please share that link so I can share it with the team as well. Perfect. thank you, Victor, for the suggestion It's helpful. 

**Victor**
* I will say this is open up for public contributions PRs. Welcome. 

**Pooja Ranjan**
* Yes, of course. That's why we want a public issue so people can like look into that. We will share the issue and people can look into that. Whoever is available may be able to work. 

# Fix assets redirect ethereum/ERCs#243 [5:35](https://youtu.be/PKkJNqcozhw?t=335)
**Pooja Ranjan**
* The next one is fixed assets redirect. Seems like a genuine one. And it is. Yeah,  Of course, some conversation ongoing, except for the last one. Seems like a spam. 

**Sam**
* It is. 

**Pooja Ranjan**
* Can it be closed? And, I think, GitHub has already, but why? GitHub has, already commented that it could be closed 

**Sam**
* Oh, yeah. It's just our stale bot doing that. 

**Pooja Ranjan**
* Yep,

**Sam**
* It's fine. 

**Pooja Ranjan**
* Okay, so what is the next step here? 

**Sam**
* There's a couple ways forward for this. So, if we want to just continue on with the repositories we have now, we need to do something, to, like, further separate the EIPs and ERCs websites. and once we do that, then this will, like, fall out and be fixed. the other option is we convince me to finish, working groups and we just switch over to that. And that will also not have this problem. 

**Pooja Ranjan**
* Okay. 

**Victor**
* I mean, which which specific, context that you're discussing about the this thing. 

**Sam**
* Like the issue number. It's 243 on the ERCs repository 

**Victor**
* Assets redirect. 

**Sam**
* Yeah, yeah. So when you link to an asset, in the markdown file right now, you have to link to it with, like, EIP in the, name. but when, like, so, like, but you have to put it in the ERCs folder and it's very confusing for people. 

**Victor**
* I see okay. No further questions. 

**Pooja Ranjan**
* Okay. So I think, both 

**Pooja Ranjan**
* Suggested next steps may take time. So this issue I see it's being open and staying there for quite some time. I would definitely encourage you, Samuelson, to maybe take out time and work on the the working group page that you were creating for rendering all these proposals. It would be nice. 

**Sam**
* So that's more a question of like, do we as the editors want to move to that? not it's not really up to me to work on it at this point. It's do are we making that change? And if so, we can we can do that. 

**Victor**
* Two options are all great, but it would take time. The third option is actually enable the real link. Right. If, if like I saw that it's SCC 2 Dash v2. If it's a legitimate external link, like they don't even need to put a PDF into our repository unnecessarily. 

**Sam**
* Right? 

**Victor**
* So yeah, if we approve external link. But these things we don't need to wait for that. So yeah, then I'm using that as an argument that we should be more flexible in in external link 

**Sam**
* Yeah I understand. 

**Pooja Ranjan**
* Going back to Sam's question, I think Sam, the main blocker there was like, what kind of working group we are planning to have? And, I think the conflict was on like, should working group be based on repositories or not? I think there were two proposals, one by you, one by me. And, this was the main point of conflict, I suppose.
* Do we want to take it on right here, right now, or is it something that I should add explicitly on the agenda for the next meeting? And maybe invite editors to make a decision on. 

**Sam**
* Yeah, I think we need to do this, like with a writeup and, like have people make a decision because I don't think we're going to get everybody on the call to talk about it ever. So. 

**Pooja Ranjan**
* Okay. That sounds good 

**Pooja Ranjan**
* We can look into some writeup and maybe ask, start asking questions around, try to collect some thoughts from editors as well as other people from the community, and we'll try to put it together. Sorry for the delay. 

**Victor**
* I actually find that you're not conflicting each other. Actually like we can have a higher level, let's say governance group and or repository group, and then any other people who want to collaborate can form topic group, which could be like subset within a repository or across different repositories. Doesn't matter it is a topic that people want to collaborate. So I don't see that it has to conflict. These two proposals can coexist actually, and can combine. 

**Pooja Ranjan**
* Very well. Let's try to add some more thoughts to the proposals and if possible, we can come up with a writeup and see, where we go with this one. Okay. Yeah I think I can do that, Sam. Perfect. Yeah. 
* Cool. okay, let's move on. The next one is, and the next one is closed, of course. So we move on to issue number 8718. The issue has been deleted. Perfect. Thank you. And 8717. Oh, wow. Sam, looks like you have already bought it. All of them. 
* Perfect. Thank you so much. so that's all about it. let me check the last one if it has gone as well. Yes. So I don't see the call for input. Deadline has reached for the only call for input. That is number 343. so, yeah, perhaps we can move to the next section. And we are also joined by Dexron. 

# Security issues with ERC-20 and ERCs in general. Ref: Comment [11:59](https://youtu.be/PKkJNqcozhw?t=719)
**Pooja Ranjan**
* So the first item on other discussions is security issues with ERC 20 and ERC in general. Dexron has added some comment to this agenda, and I would like to invite you to maybe give some background and, yeah, share your specific questions. How we can help you. 

**Dex**
* Hello, everyone. today I'm here with Dario. Dario works for iOS support. He also implements the Ethereum Virtual machine in its smart contracts as well. So whatever we are going to discuss here is also relevant for your community. 
* So I would like to start with a summary of the history of the problem that I am going to discuss, because it's quite long. so we have an ERC 20 standard in Ethereum. It was developed in 2015. At that time, there was a call stack depth bug in Ethereum Virtual Machine. So in order to make token not affected by this bug, there were two transferring methods implemented in 
* ERC 20 one is designed to transfer tokens to externally on addresses, and the other is used to deposit tokens to smart contracts. In 2016, the call stack depth bug was fixed, but ERC 20 specification was not upgraded. Obviously. And then 2017, I was researching the ERC 20 and I discovered that it lacks error handling 
* If you use a method designed for transferring tokens between externally entendres to send tokens to a smart contract, then instead of getting an error, you will successfully deliver the tokens to the smart contract, but it will not be recognized as a deposit as a recipient contract and you will effectively lose your money. I have reported this problem in the 
* ERC 20 in the ERC 20 finalization thread on GitHub. You can still find one comment there. Uh. However, Fabian Vogelsteller replied that they are finalizing ERC 20. Anyways, in 2017 I have created an alternative token standard ERC 2 to 3, which was designed to solve this problem. 
* And in 2019, there were about 2 million of dollars worth of ERC 20 tokens lost because of this issue that I discovered and reported in 2023, I wrote a script that calculates the amount of lost tokens, and after the result of the script, it was possible to conclude that there 
* Are at least 80 millions of dollars worth of ERC 20 tokens lost to this issue that I reported seven years ago. At this point, I was trying to escalate this problem. In 2023, you may remember my proposals, and my general proposal was to add this description of the problem to the 
* ERC 20 Security Considerations section in the text of the ERC 20. if I remember correctly, at, some of the EIP editors calls, my proposal was voted out by Greg Colvin, when he stated that the problems of, money losses caused by the design of ERC 20 standard must be described 
* Somewhere outside of the ERC 20 standard text, and I was told to create an informational EIP to describe this problem of ERC 20. I have created one, but it was subsequently rejected by EIP editors. I don't know the reason, but we can find it on the GitHub. It's still there 
* So here we are right now. Currently it's 2024. Yesterday I ran my script again, to calculate the amount of lost tokens. And, as of today, there are another 20 millions of dollars worth of ERC 20 tokens lost which were not lost on, 
* 25th August 2023. so if we will take this, amount as a key performance indicator of the Greg Calvin's idea of how to handle the problems of, disclosures in EIPs, then this idea quite failed because, people keeps losing money 
* To well-known issuers. It was reported 7 years ago. so now let me explain what is done wrong. Once I know those requirements that I'm going to highlight are not my personal invention. I did some research on the evolution of C++ programming language standards, and I found
* some documents that describe the workflow of ISO C++ Committee. and, this is a practice adopted by this project, one of the largest project with largest development histories. I think it's quite good to link. So the first one, exposure in order to solve a problem in a standard, the problem must be clearly communicated to the implementers. It is very important not only to communicate the problem itself, but the severity of the problem as well. Because people tend to treat known issues as something they don't need to worry about. I have a great example here 
* For you. in 2023, I reported to Openzeppelin that the pure implementation of ERC 20 in the code is prone to this problem that I described. And, at the same time, it fits in critical security vulnerability criteria in the Openzeppelin bug bounty page 
* They replied that even though it does fit in critical security vulnerability, no bug bounty will be paid, obviously. And, this is because it is a known issue and it is reported long time ago, so they are not going to do anything about it. if ERC 20 standard itself will not 
* Change. So in fact, they have a known critical security flaw in their contracts. And people keep losing money because of this, but they place a secure label on the smart contract repository as if everything is good and you can observe it. It's still there. so we need to make it very clear for the implementers that a pure ERC 20 implementation will 
* Inevitably cause their users to lose money. As a result, they need to implement a sort of modifications of on top of the base standard to prevent this. And this is more than possible. And here comes the second requirement to solve the standard problem according to ISO C++ committee document 
* Alternatives. If we are stating that there is a problem in the standard, then in every place where the problem is mentioned and in my opinion it must be mentioned in every place where ERC 20 is mentioned on Ethereum resources, there must be a list of actions that the implementers can take to either mitigated 
* Solve it or avoid it. Unfortunately, it's not possible to solve the problem for ERC 20 tokens, especially the existing ones, but it is possible to implement a number of modifications to the transfer function that would prevent it. And in newly created versions of ERC 20 tokens, it is possible to mitigate like 
* 80% of the damage that it can take, it can inflict to the users. It is also possible to avoid this issue by using alternative standards. And here comes the third requirement to solve the standard problem upgrading processes. If one standard must be replaced by another one, then the upgrading 
* Process must be coordinated. Currently in  process there is no such thing as coordination of an upgrading process. There are no tools for this and as a result, we didn't see any major standard upgrade like, ERC 20 is the first standard that emerged in Ethereum, it has 
* A problem that fits in critical security vulnerability criteria, according to Openzeppelin bug bounty, and it sells the mainly used one and also of an alternative token standard. So from my side I'm working on ERC 7417 and I'm trying to change the paradigm one 
* Token, one contract. where if there is a UCC token on Ethereum every other utility token that you can find is a scam. So with ERC 7417, there will be one version of each token in each standard. And effectively, there will be ERC 20, Usdc, there will 
* Be ERC 223 Usdc created by a special contract. yes. I will, add the link to the documents and the comments. after this call. Thank you for the reminder. so I will continue on the upgrading processes 
* Description. as an author of the ERC 23 standard, I am developing an upgrading process that will allow the ERC 20 and ERC 22 to 3 tokens to be converted from one to another. But imagine that you are the implementer, 
* And if there is one standard that everyone uses and it is supported by most of the exchanges, and the ERC 20 is supported by all of the exchanges, and it's the only standard that supported by exchange. It is supported by wallets. Then why would you consider any alternatives? what can be the arguments to convince you as an 
* Implementer to even start thinking of using any alternatives? I had some discussions with the implementers. I can also provide the links and the best argument for the implementers can be written in the text of this exact EIP. So everything that is written outside of the text 
* Of the EIP is treated as someone's opinion, and not a valid argument to start doing something for the implementer. This is important to understand. And, one note, regarding Greg Colvin's proposal, if some object is particularly dangerous, then the danger warning is normally placed on that object. for example, there are some dangerous household chemicals, like bleach.
* And you can place a warning message, don't drink bleach on a bottle of Coca-Cola and pretend that you did great job warning people about the dangers of drinking bleach. If bleach is not designed for drinking, then you place a don't drink this message on the bottle of bleach 
* To warn the people. And this kind of explains why Greg Colvin's proposal doesn't work, and why we have the an extra 20 millions of dollars lost after the implementation of this proposal. And, now I would like to propose something that, in my opinion, can solve the problem. Or at atleast, reduce the damage to the ecosystem. 
* So the first proposal I would like to revive the ERC 20 vulnerability disclosure EIP that I was working on and finalize it. We can revise the old one. I can write a new one. It doesn't matter, really. And we need to add the warning to the security consideration section of ERC 20 text. As I initially proposed, currently a year passed, 20 millions of dollars are lost. I think it's time to change the strategy. 

**Sam**
* May I interrupt for a second? Yeah. So I think the prime example of why we can't or won't do that is I believe that your EIP 223 has a security flaw in it, which is that if you send tokens to a counterfactually deployed contract, there is no way to know, ahead of time and the account will be locked and those tokens will be lost. So obviously the only way to fix that would be to require a signed message from any account that, you're transferring to. So I want to put that warning into your EIP. 

**Dex**
* Well, I would say that this is not a problem of my token standard. This is a problem of how Ethereum treats addresses. For example, here is Daru from EOS and in EOS, addresses do not exist before you do some special actions. So it basically has some built in naming rights. And this is not a problem of a token standard. This is a problem of how Ethereum creates addresses.

**Sam**
* On Ethereum 223 can't detect counterfactually deployed contracts. And so they the tokens might be lost. So that is a security problem. And now I believe that should be added to your EIP. So how do I add that to your EIP in our process or in the process that you're describing. 

**Dex**
* Wait a minute.why would you think that this is a security problem of my standard? my standard is a copy paste logic of the Ether. And, do we add it to the description of how Azure works? 

**Sam**
* Sorry, your EIP is a copy paste description of what, the logic of 

**Sam**
* 2223 is based on the logic of ether, the native currency of Ethereum. 

**Sam**
* So it's still a problem though. Like you can still lose tokens by sending to an address that is eventually becomes a contract. 

**Dex**
* Yes, it's obviously a problem. Yeah, I agree fully that it's a problem. But this is the problem of Ethereum the sender. This is a problem of address generation, not the transferring method. It's a different problem. Yes it is a problem but different problem. 

**Sam**
* So I think what I'm trying to say is that any process that we create for modifying final EIPs needs to be able to account for these kind of disagreements and needs a way to resolve these disagreements. That doesn't rely on editors being experts on what's a protocol problem vs a standard problem. 

**Dex**
* Yeah, and this is the next thing that I was going to discuss. I have a perfect, perfect. Yeah. I recall that we had a discussion a year ago regarding whether EIP editors are supposed to make these actions and act as security experts to determine whether something is a security problem or not. I would propose that, there can be a simple rule if something caused a verifiable loss of funds, after a certain amount, like 10,000 of dollars, then, it can be added to the security consideration section. We don't know if this is a security vulnerability or flaw or something else.
* If something has caused a verifiable loss of money that can be detect by simply going through transaction history and open blockchain explorers, then it can be added to the security consideration section or the corresponding EIP. I think that the EIP editors can do this without any specific requirements for the security skills. And going through the blockchain history and reviewing if something was lost is not that specific. And if something caused the loss of money after there is a precedent, you add it to the security considerations.
* So if the situation that you are describing here will happen to ERC 23 tokens once it happened, we can add it to the security considerations. 

**Sam**
* And is there is there a particular dollar value you're suggesting, or could it be one way? 

**Dex**
* Sorry, I didn't understand the question. Oh, sorry. 

**Sam**
* Is like, is there a particular dollar value that you're looking for, or can it be as small as one way? 

**Dex**
* I think it must be something like anti-spam, because, if you will put, $1, then someone can artificially throw $1 worth of assets in this situation, and nobody will sacrifice 10,000 of dollars for this to bloat the specification. And add the problems that naturally never happens. So I think it must be smaller than $1 dollar and, a little bit higher than something that an average person can sacrifice to gain a competitive advantage in the process. 

**Sam**
* So you're saying like you're kind of describing we put a price on getting a competitive advantage or. 

**Dex**
* In theory, we can do it as little as $1 per, but it will not be representative. You will bloat the specification with, issues that you as editors have to handle, but it's up to you. I am just proposing a way of how we determine if something is a security issue or not. In theory, even if you lose $2, it's an issue. The question is, if it is worth your editors time to investigate small issues, or you need to focus on something else if you will be investigating all the issues, it's fine for me. 

**Sam**
* I'm just anyways, like, is at the end of your, like, discussion, or do you have more to say? I don't want to cut it too much 

**Dex**
* Yeah, I had three proposals. So the first one is to revive the old vulnerability or security flaw description EIP that I was writing, and add something to the security consideration section of ERC 20. Implement this rule of how we can add new security considerations based on loss money. And, I'm here to ask for feedbacks, because it seems that I'm championing the solution of ERC 20 problem. So I'm here to hear feedbacks and, maybe some else ideas of, what else can I do to facilitate the solution and how else I can contact like this. Thank you. 

**Sam**
* Thanks for coming I appreciate it. I think you did a really good job, like articulating the problem. And it's good to have a record of that in our recording. so thank you. as for, like, I think the problem is more that there's like a missing layer in ERC governance or in Ethereum standards governance. So we deal with documents, right? Like we, just make sure they follow a certain rule and such. And then, we try to be as objective as possible. Uh 

**Sam**
* Which is kind of different from other standards bodies like the C++ standards body or W3C or, or any of the other ones who are generally a bit more opinionated. and I think we're missing this kind of, opinionated layer that sits above the documents so in the core development world, that's all core devs. So for example, like I can make an EIP that I don't know, sends all of the ether to my address and get it through all of the document stages, get it to final. but that doesn't mean anything. It just means that the document can't be edited anymore. there's this layer above EIP, all core devs that kind of manages, what they're implementing and what they're not implementing.
* That layer is missing for ERC development. And, obviously it's hard to kind of envision one existing there. Just because there's so many different competing actors and such. and I think it'd be very hard to say, like, you know, you better not implement ERC 20 anymore or else will find you or will like, so I think that's the problem is that we don't have this kind of, opinionated governance layer. And it's not necessarily that, something that we can solve at our, you know, document centric layer, but I'm definitely open to other opinions on that. 

**Dex**
* Okay. So I will say that I, disagree with your vision of where the problem lies because if you can make a proposal to change the protocol of Ethereum, it's up to implementers to decide and it's up to the keepers of consensus to adopt it or not. But, here we are talking about something that, community implementers will look on and you are not providing them with sufficient information to make a proper choice. You are silencing the problems. you are not intentionally silencing the problems, I think. But, the problems that exist for years and caused severe damage to the customers, are not highlighted. They are hidden from the implementers.
* And when me, I'm a security auditor, I own a security auditing company. When I am stating that there is a problem in the standard, they are treating it as if it is my auditor's opinion It's it's not my opinion already. It is discovered, it is discussed. It is documented. It's not an opinion already. It is a fact. We can verify it by transaction history. And this needs to be included in the documentation. And you are governing the documentation.
* So that's why I came here to make some proposals of what can we change on the documentation governance level so that we security auditors on the social level will gain a proper argument to convince the implementers who are too lazy to do the research themselves, to make a proper choice. 

**Pooja Ranjan**
* Well, thank you, Dex. Thank you. Sam, I hear the main problem is about the governance layer here at Sam. Very well. Put it out. We do not have, some some place where we decide or maybe can make a decision on what would go in or not. The standard repository that we are having right now is open and open for all. 
* As much as I understand the concern and I share the concern as well Dex. I am not very, very much confident that we have a solution right away, but we can definitely consider those three proposals that you have proposed today under consideration and would try to work on that. However, as you have also mentioned in the issue itself, the document shared by Sam Wilson about, you know, brainstorming for security disclosure, as we say, that this EIP process or the ERC is those are available on the standard, are mostly author driven.
* We definitely can help them understand the issue. But adding such warning, has not been accepted so far. I'm just trying to explore if there are any other venue where we can add it without, disturbing the current, organization or the template that we are following for proposal.
* I do not have a straightforward, next step for you, but what we can do is like if you want to, like, as you have already championed 2 to 3, and it is there for us now, if you want to propose something new, we can maybe increase discussion on that side. Or if you think we should involve more parties, maybe some application developer who would like to support the idea of getting, this thing documented in either EIP one or ERC 20. I am open to have a specific discussion on this if you would want to. 

**Dex**
* Well, I'm not here to propose something new. I'm here to state that what was already proposed and rejected was the proper version because, I made a proposal. Greg Colvin voted it out and made another proposal. His proposal doesn't work. We can identify it by the amount of lost money. And it's time to change the strategy, in my opinion. And, I'm here to basically ask if it is worth to revive this EIP that I was working on a year ago. And if, in the light of new events. 

**Pooja Ranjan**
* Can you tell the number of the EIP you are mentioning here? If it is not 223,

**Dex**
* I can find it. I'm not sure right now. I will find it and attach it in the comment thread alongside the documents that I mentioned. 

**Pooja Ranjan**
* Of course. yeah, that I think would be a good, start again for bringing  this conversation back if it is backed by a proposal, already, either in draft or stagnant status, even if it is there, we can perhaps start making discussion on that. But, the main blocker is, main blocker with not updating ERC 20 is when a proposal moved to final status. We do not want to make any changes to that. And if we have something new, we can perhaps make room for that. But we want to avoid updating ERC 20 as much as possible. 

**Dex**
* Yeah. But, the problem here is that, you do not allow EIPs to go to the implementations before it reaches final state. And, bugs and problems are normally described and discovered during the testing state. So in your system, you don't have a room for testing. Proposal reached final. And at that time it becomes immutable. And only at this time and your issue can be discovered when it is already immutable. 

**Sam**
* Well, so last call would be the time to start implementing an EIP and then reporting any issues while you implement it. 

**Pooja Ranjan**
* Yeah, I understand we do not have like proper testing, devnet and public testnet kind of thing as we have it for core proposals. That's not existing for ERC, and that's why we have been stating it as a standard and authors should implement on their own risk. What we are trying to provide here is to make sure the standard that a user wants to make available for the community has proper template, has proper checklist, and they have done their due diligence. They have documented their specs. In a way, it should be useful by any other implementer to implement in the project EIP editors may not be able to verify whether this has been tested 100% or not. 

**Dex**
* Yeah, understand. But, the problem here is, why is the security consideration section immutable? I understand why the specification is immutable. You can change the standard which is already in use. It will break the compatibility with already existing solutions. But, security considerations can be append only. 

**Pooja Ranjan**
* That's a fair point. All right. I think, security consideration is definitely for implementers support. So they should be aware of what what are the things that they should be mindful of. I hear your, thoughts over there may not have, again, may not have immediate solution for that, but I would highly recommend you to come back with the proposal that you have, anywhere. Even if it is in stagnant status. We can perhaps bring it back and start talking about it and see if that would be helpful. 

**Dex**
* All right. Thank you. We will revive this proposal, and I will attach the link to the comments. 

**Pooja Ranjan**
* If you could add it that would be nice to have. We can perhaps take a look. And if that is like something in the stagnant status already and you want to revive it, please make a new PR to bring it back to active status. We will take it into EIP editing Office Server to make sure that proposal is merged as active and then we can start discussing it actively on its Fellowship of Ethereum Edition page to see what we can do next. Very well. That was a big chunk of, our discussion today. I know we have a few other items to go over. and there was also a request from 721 team to see what we do about it. like, we know that there are two proposals.
* One is 721 to in our GitHub repository, and there is the other one, 7212 to in EP GitHub repository to add some context, when we made the split of EIP and ERC, we moved all the ERC s out of the EIP GitHub repository to the ERC GitHub repository. And 7212 was one of those proposals, which was moved to the repo GitHub repository. And here the status shown was moved. Now the proposal 7212 is in final status as per RIP. GitHub repository. And they are also trying to push the proposal to the final status on EIP GitHub repository. That has brought some confusion and this is being done because proposal 7212 is being considered for Pectra upgrade.
* I think, people are getting confused, whether they can have the same number on both repositories.
* I would be curious to hear thoughts of editors, and we should keep it in mind that the number allocation process is uniform across all these repositories. So far we have only one number existing in one repository. We do not have duplicates of that. 

**Sam**
* I'll put up a call for input for it. 

**Pooja Ranjan**
* That would be nice. Yeah. And yeah another point that is for consideration here is the precompiled address is different in EIP 7212 and EIP 7212. So we should highlight that as well. That means the specs are not 100% exact same. They have one minor change and that change is in specs section. Well thank you Sam. I think that is also up for all core dev meeting. So if you could create the call for input, we can also share it with people. there, core developers, people, if they have anything to add, although this call for input is specifically for editors, but we can definitely collect their thoughts as well. Okay, couple of other items.
* This I think we can perhaps skip it because we don't see too many editors here, but we can get into the other one. 

# Discuss blockers to merge a Pull Request [42:55](https://youtu.be/PKkJNqcozhw?t=2575)
**Pooja Ranjan**
* Okay. Discuss blockers to merge a pull request. So the last week I was in, ezmerelda and event, in California, and I got a chance to talk to Tim Baker as well. And we were discussing the issues that EIP, um team think that they have these issues with the EIP editors, like where they would need support from EIP editors. 
* So, we looked into, the PR blockers. It seems like on a broader level, we have like four different kind of PR blockers. Number one is waiting for editor number two waiting for author. Third, we have lot of open PR which are into draft status but haven't been merged. There are a few of course, more which are based on CI test pending. 
* So there were two issues that I think this group may be able to support. One PRs which are waiting for editor and second PR which are made for new drafts on the discord channel of R&D. Also, we have received one PR, suggested by one of the developer, and he is having this question like, what should I do to get this proposal merge as draft? 
* My question to editors here would be like, can we think of a some, maybe an estimated timeline for merging draft proposals? 
* But when we are, suggesting this timeline, we should keep it in mind that draft proposals are very basic. It need not be 100% like correct, because for that we have the review status. But if we can come up with certain timeline that way, it will help us reduce the number of open pull requests as well as it will give the confidence to, core developers who are trying to make a proposal for consideration in network upgrade, that they are there. I see I noticed some of the PRS which are in draft status have also been moved to stagnant, but I try to list out some of them which are out there. Please, share your thoughts on how we can minimize, this wait time. 

**Sam**
* Sure. So, one idea that my partner Nicki had, who wasn't here to present it, unfortunately. But since it came up, I'm going to talk about it anyways is this, it is a, rust tool that pulls the repository and puts all of the pull requests into the order that they require attention by an editor. The algorithm is basically like, find the oldest author interaction, that is after an editor interaction and then sort by oldest first. 
* So this can kind of give you an idea of when your pull request is due to be reviewed, like how many things are in front of you. and it also makes it a lot easier for editors to, find stuff to work on instead of having to go through the whole list. 
* So this is one idea we had to kind of a give authors an idea of how long they're going to be waiting. And, b make it easier for editors to find out what to work on. yeah. So that's kind of one idea, I guess. 

**Pooja Ranjan**
* It's pretty interesting, like how we can implement this, what support we can provide that this tool is made available for, either on the EIP repository for editors to maybe take a look into. 

**Sam**
* Yeah. So the my end goal is to have this as part of the build so that every time, you know, somebody publishes the website, it'll update this and kind of just let you know how many things are in front of you. 

**Pooja Ranjan**
* That would be awesome to have. So you did mention that it would be a part of build and someone publishes on their website. by that, would it mean that people may need to look into EIPs.thereum.org to get a feel of how long is the wait time or is it something? Okay. Perfect. Sorry, Victor. You were saying something? 

**Victor**
* Oh, no. I like this idea a lot. I think, having this information will help, at least give a, give an estimation for how long it would take for them to to approve But also, I think in general, having, a statistic published like average time get from one place. I know that, EIP insight already have that information. Maybe we can also publish that to get a general kind of estimates but for what?
* Sam says like for one specific EIP instead of, in addition to, publish, like what other EIPS are out there waiting for attention? we can have a very good estimate unless we have there is a there is a expectation of, let's say, Q or ordering or scheduling of who is going to work on them. Right? Even if this EIP could be in the queue, some other, like EIP editors or other people might be focusing on other EIPs, not yours. Which means you can wait longer, right? So how do we figure out which one to schedule? Which one to prioritize? Is there any ever a prioritization approach? I think that's a question I have. Like how should we what's your opinion on that? 

**Pooja Ranjan**
* I think it is prioritized by date. Like if I understand that 

**Sam**
* Correct. Sam. So in this tool. yeah. So it so okay for editors in general, I would very much recommend just picking the oldest EIP and trying to get that one merged. And if you're blocked on the author, move to the next oldest one and don't prioritize in any way other than that, because it gives the, the appearance of, you know, non-neutrality, but that's just me. I'm not going to force anybody to do that. the tool, specifically does it based on the oldest author interaction. 
* So that's like a commit, a comment, an edit, like any of those things. So the oldest interaction by an author of the EIP, that is after, the most recent interaction by an editor, and that's how this list is prioritized. 

**Victor**
* I agree with your approach. I think that's actually a good way, at least for the pure editing part 

**Sam**
* Yeah, exactly. It just means, like the oldest, the people have been waiting the longest, get interacted with first. 

**Pooja Ranjan**
* That would be awesome to have because as I was mentioning earlier, I have seen some of the proposals which are in their draft status and has been moved to stagnant because the wait time was a little bit over than expected. 

**Sam**
* Do you mean, like stale or do you? Oh, oh, you mean like the IP was merged as a draft and then it wasn't merged? No, those are the worst I try to so my editing routine is look through the recently closed things and unclosed, the ones that were, that haven't been reviewed yet. 

**Pooja Ranjan**
* Yeah. So I have tried to, maybe, share a list here on the agenda, which are some of the open, proposals for new core EIP and networking and interface. Perhaps I'm not very confident that all of them are core, but definitely I have taken all of them from the EIP GitHub repository.
*  And it would be nice if someone can maybe take time and may be able to merge. Some of them has received some attention, some inputs from editors, and they all of them have a number, but they aren't merged yet 
* So if on the draft level, we can just make sure that, the proposal is abiding by the template, the EIP template, they receive, the, real number and it can be merged. So these people can talk a little bit more about it, and we can get into in-depth review when the status is proposed to be changed to review. 

**Sam**
* Sure I can take a look through these. 

**Pooja Ranjan**
* Okay. Perfect. I think that would definitely help. providing some confidence to the core development team, that EIP process is not completely broken. Editors are there. They are reviewing it. Just that the number of proposals or pull requests for review are a little more than than the number of editors we have here to review all these proposals. 

**Sam**
* And, if I'm being completely honest, I don't review EIPs anymore. I kind of hope that Matt and Gajender, do those. I haven't done any EIP in quite some time. 

**Pooja Ranjan**
* That's not bad. Even, like, we have two people to maybe take a look into EIP. So I'm unfortunately I'm not seeing them on the call today. So we'll try to talk to each one of them as well. if they can follow the same norm and may be able to merge, these proposals are not get involved with reviewing because the main issue that was highlighted to me, when it gets on to review on the pull request, most of the conversation are there on the PR itself, and they are not being captured on the Fellowship of Ethereum magician. That way some people may lose some context. 
* So it is a suggestion that we should merge the proposal as draft. So whenever they are having some discussion, it would be moved to the Fellowship of Ethereum magician. Not on the initial draft pull request. 

**Sam**
* Yeah, that's a good, good point. 

**Victor**
* And also, Sam, I, some of the ERCs I like to merge, but I saw that you already have some comments and we're waiting for authors to, to kind of come back.
* I wonder if some of those, comments could actually be given after, the merger of drafts, because a lot of authors need them to be published as drafts. and then sometimes it's just, very basic grammatical change that doesn't affect the understanding and completeness of the draft. For it to get feedback, I wonder if it's okay if I go ahead and. Yeah, wait, why are they waiting for them to come back with the with an update for as as long as I haven't marked it as, request changes. 

**Sam**
* Like as long as like there's the three ways to reply, right? There's approve, there's comment and there's request changes So as long as they haven't request changed on something you can like approve it if you want. I won't be mad. 

**Victor**
* Yeah. So okay. So as long as it's not a request for math, right. If it's just like suggest the change, that's fine. Right. Yeah. 

**Sam**
* Exactly. Like if it's not the red icon, you're good to go. 

**Victor**
* Okay. Yeah. Makes sense. I think that's some of them. Seems, well, ever since Matt doesn't want me to ping people to say hi. Are you still working on this? Because, of course, that also, reset the timer for the for the bot, which is, I think Matt's ask is reasonable. I like yeah, that's another consideration. Let it stale or let or approve it. 

**Pooja Ranjan**
* Yeah. We can perhaps discuss some of the, options how to, bring them back, for discussion and things like that. I have a couple of more points which we wanted to discuss from the meeting. there. but in the essence of time, we may want to move it to the next meeting.
* From this meeting, for note takers, if I can conclude it in a way that we are open to the idea of merging the initial draft as soon as possible, I know the number allocation is done within 24 hours. And if we can just try to merge, draft proposals within a week's time at the max, definitely. Before next quarter, call our next developers call, ACDC or ACDC. that would be helpful. And the same thing can be applied on ERC side as well. We would try to move most of the discussion out of the GitHub repository. We'll try to push it on to the Fellowship of Ethereum Magician page. Whatever suggestions recommendations we have for authors. 
* All right. I know it's about time. So, I wouldn't go through all of the details of the EIPs Insights. We have added a link. we have some changes seen in the month of June, not major changes coming up in July, because today is just 3rd of July. People may take a look at it. And, yeah, I think that would be all. 
* Yes. I think there was this, make a call for input for, PR number 8390 was there, which I was supposed to do. Unfortunately, I did not do it. maybe I'll try to do it this week. 
* Anything else anyone would like to share add for the next, agenda item? 
* Very well. Well, thank you everyone for joining us today. I know some people got some resolution get to the next step, but we will try to solve issues as we are getting it. We definitely have our next step. We are open to bring up anything in the next meeting. If if anyone has any thoughts, new ideas that they would want to share or discuss with editors. 
* So once again, thank you everyone for taking out time for this meeting. I would welcome all of you to share your thoughts comments in the Eth Cat Herders Discord channel on the EIP Editors Channel, you can always share your thoughts there and, add any item for the next meeting as well. All right. Thank you everyone. Have a good one.



---------

## Date and Time for the next meeting

July 17, 2024 at 14:00 UTC

---------
## Attendees

* Pooja Ranjan
* Sam
* Akash
* Zainan Victor Zhou
* Dario
* Dex


