# EIP Improvement Process Call #46 Notes  <!-- omit in toc -->
### Meeting Date/Time: Wednesday, Dec 15, 2021 at 15:00 UTC <!-- omit in toc -->
### Meeting Duration: 1 hr <!-- omit in toc -->
### [Audio/Video of the meeting](https://www.youtube.com/watch?v=xEuy8b5cJjU&t=644s) <!-- omit in toc -->
### [Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/98) <!-- omit in toc -->
### Moderator: Pooja Ranjan <!-- omit in toc -->
### Notes: Edson Ayllon <!-- omit in toc -->

----

# Summary <!-- omit in toc -->

## ACTION ITEMS <!-- omit in toc -->
Action Item | Description
-|-
**46.1** | Make PRs to call all EIPs EIPs in the documentation, and not ERCs for EIPs with ERC category.
**46.2** | Continue discussion to move all discussion-to and predrafts to Ethereum Magicians.
**46.3** | Merge Greg's PR for him to recieve notifications for EIPs.

---

# Contents <!-- omit in toc -->

- [1. Discuss a standard for documenting Standard Track EIPs especially "ERC" Category](#1-discuss-a-standard-for-documenting-standard-track-eips-especially-erc-category)
  - [Actions](#actions)
- [2. General consensus to discourage using Issues for "discussion-to" or EIP number](#2-general-consensus-to-discourage-using-issues-for-discussion-to-or-eip-number)
  - [Actions](#actions-1)
- [2. Update eip-bot to add Greg Colvin as reviewer to notify his availability Ref: Discord](#2-update-eip-bot-to-add-greg-colvin-as-reviewer-to-notify-his-availability-ref-discord)
  - [Actions](#actions-2)
- [3. EIPs Insight - Monthly EIPs status reporting.](#3-eips-insight---monthly-eips-status-reporting)
- [4. EIP editor apprenticeship meeting](#4-eip-editor-apprenticeship-meeting)
- [5. Review action items from the previous meeting](#5-review-action-items-from-the-previous-meeting)
- [Annex](#annex)
  - [Attendees](#attendees)
  - [Next Call](#next-call)

---

# 1. Discuss a standard for documenting Standard Track EIPs especially "ERC" Category

Video | [0:00](https://youtu.be/xEuy8b5cJjU)
-|-

This continues a topic from the last meeting. 

In the public, ERC's are prefixed by ERC instead of EIP. For example, many reference ERC-20, but no one says CORE-1559. ERC-20 is listed as EIP-20.

This topic is to standardize standards track equally.

Micah: I convince we have everything prefixed EIP in the documentation. But I don't think we can change outsiders calling ERC EIP's ERC.

Shashank: Do EIP authors already know the difference between ERC and other EIPs? Isn't that sufficient?

Pooja: Yes, there is a common understanding. ERCs are a part of the standard track EIP. It may be a difficult task to convince people to say EIP-20 instead of ERC-20.

Shashank: I see ERC-20 more as a marketing term. I don't see what the exact problem is.

Micah: In our documentation, it's inconsistent. In some places we refer to them as ERCs. Do we still plan on splitting out ERCs onto different repositories? Do we know?

Pooja: Maybe after the merge we can decide this.

Lightclient: I think we're waiting for the execution spec. How people use the execution spec depends on whether we move ERCs into their own repository.

Greg: It seems to happen, ERCs are EIPs through the approval phases. Once they are final, an EIP becomes an ERC.

Micah: If we are going to split ERCs in their own repository. There is value on calling them ERCs now. As for documentation, it doesn't matter much. We can call them EIPs, and let users call them whatever they want.

Pooja: We link ERC-20, but when they click on it, it shows EIP-20. What we can do is update EIP-1, call it EIP-20. Then we can try educating the public on calling them EIPs. 

Micah: I agree making EIP-1 consistent. I'm against educating them to use EIP instead of ERC, as it would be a huge headache. 

Pooja: I can create a pull request to make these changes in EIP-1. 

## Actions

- **46.1** - Make PRs to call all EIPs EIPs in the documentation, and not ERCs for EIPs with ERC category.


# 2. General consensus to discourage using Issues for "discussion-to" or EIP number

Video | [10:32](https://youtu.be/xEuy8b5cJjU?t=632)
-|-

Spam Issues Ref: #4556 and #4554 in the EIP repo.

Pooja has been wanting to have the bot push people to Ethereum Magicians for the discussions-to section.

To address spamming, Pooja proposes having the bot count the EIP number as the first PR to add the EIP. 

Micah: Is it to continue to reinforce what we've been doing? Or take it a step further?

Pooja: The issue is related to the EIP number, which can be done with the issue number or PR number. As less people would use the issues section to start discussion-to.

Micah: Ok, looks like a small change.

Lightclient: Good with me.

Greg: We've been using issues as a way to begin discussion, and begin a number early on, for years. Even before we started. There's no need to change, as we won't run out of numbers.

Micah: The goal is to condense discussion to EthMagicians. Secondly, we would like to use the issues section to discuss issues related to the EIP repo and the process. Currently, we can't, because it's cluttered with people posting their EIPs. 

Greg: The issue should have a link over to the Magicians right away. This is a way it worked for years, and changing it after years, it's not worth the bother. It's better to discuss an EIP that already has a number, than may one day have a number.

Micah: Do you feel there is value in getting a number before you are ready to submit an actual draft? Is that accurate?

Greg: Yes, I'd rather clutter the issues with things that die early, than clutter up the repo with ideas that die.

Pooja: I don't think it's a good practice a proposal that is merged as an EIP, we should refer to it as a pull request. The whole point was to standardize the process more, and follow the recommendation by EIP-1. In EIP-1 it's up to the EIP editors to select one. I think it makes sense that the responsibility is on the editors to provide the number, and not the authors. As for the discussion, we have a lot of open issues, and discussion issues we don't know when to close. The proposal related discussion moving to Ethereum Magicians, we can better use the issues section.

Greg: The magicians discussion has to point to something. If we make it point to a draft, then we start cluttering the repo with drafts that die as bad ideas. The way it works right now works, and it's been working for years. The only hassle is when people keep clicking the number until there's a number they like. If people do it, it's not worth scolding people about. 

MIcah: Why do you think there needs to be something to link back to? Why can't they create an Ethereum Magicians post have the information for discussion.

Greg: Where does the draft go? You want to write-up something that's developed enough to have a discussion. I don't want to write a draft in the repo for that purpose. The discussion may say it's a bad idea.

Lightclient: I think the issue for having 2 places for EIPs. Some issues the EIP exists, it has an EIP number, but it's not in the EIP website, nor the repo.

Greg: If it never makes it into the repo, it's not quite real. People have been doing this for 5 or 6 years now. You can change the advice in EIP-1, so people start doing it that way. But the problem is where to put the large text that people want to discuss.

Micah: Why can't you just put that in the Ethereum Magicians forum?

Greg: You can, but the hassle is you have a discussion that's hard to parse if there's edits. People may create an EIP in their own repo, but not everyone manages their own repo.

Micah: Your point that you don't have an EIP to link to. For us, that's a selling point. We want to make sure that it's not an EIP at that point. It's just an idea. And having that not in the EIPs repo, until it's an EIP. We have problems people calling it an EIP, and not even making it to draft.

Greg: It can get to draft, but if it dies, it's just a dead number. We can change the advice, but trying to enforce it, is not worth the bother.

Pooja: The purpose of the standardization is for everyone to follow. We would like to have the standard we develop to actually be a standard, and not a suggestion.

Greg: I find it difficult to change what I'm doing.

Shashank: If we don't have a standard process, it increases for friction.

Greg: The issue provides a history, without involving EIP editors until it's more substantial. A process slows things down a lot once editors have to manage it. I do see arguments on both sides. From my perspectives, it's hard to change things once it's been some way.

Shashank: I think only 10% of people use issues for discussion now. 

Greg: If I ever write an EIP again, I'm still going to do it the old way.

Pooja: We should start by changing EIP-1. I assume, whatever is there on EIP-1 is a standard. If there are other issues that come along the way, we can revisit on other meetings.

Greg: If we do drop the first pre-draft at the start of the discussion issues, does it keep letting you edit it indefinitely. There's a problem of cluttering the issues. But cluttering the drafts is a worse issue.

Micah: If Ethereum Magicians does have an edit timer, than it is a legit argument. 

Lightclient: I can edit indefinitely. But I don't know if it's because I'm a moderating.

Pooja: I think there is a timer when a post is not editable. However, this can be overriden with moderation help.

Shashank: I was wondering if it would be useful to create a different repo specifically for discussing ideas. Then there's no issue for numbers and drafts.

Pooja: EthMagicians was created for this purpose. If you want to start a discussion, you don't need to have a draft open.

Micah: It does appear there's an edit timer. Could we edit that?

Lightclient: It's an open-source software, we should be able to propose it. The forum is called Discourse. 

Micah: I do agree with Greg, that if there's an edit timer, then it does not make sense to have this idea phase of this discussion. There is value to type up your specification before it's ready to recieve feedback. If We can remove that, I'm back on the camp to having the discussion on EthMagicians.

Greg: Remember, these discussions go on for years. I have EIPs open that have been there for 5 years now. Edit timers are really a hassle.

Pooja: If we can divide it to 2 pieces: Issues for EIP number, and issues for discussion link. Is there consensus that only the PR number to be an EIP number?

Greg: No. The whole advantage of issues is that PRs and issues count up the same number. The benefit is that it has a number when the discussion starts. If people don't have a number to refer to, it's difficult to get it out to the community to discuss to. The only way it's broken is we get a lot of issues. We can't use issues like a normal repo. We have these discussions on our discord threads. We're trying to solve a problem that's just not a big enough problem really.

Pooja: I think in the past, we have made some effort to move the discussion link to EthMagicians. I haven't heard any strong resistance so far. Though I'm open to hear the arguments to going back to issues. Talking about the serial number, once the PR is there, it's the same number from the issue number. I do think it's something that should be provided by an editor. And we shouldn't call it an EIP until it has a draft. We've seen project that claim they implemented an Ethereum proposal, but that proposal doesn't exist in the EIP repo. We can table this discussion for now.

Shashank: If I understand correctly, an EIP author is trying to submit a pre-draft. But the number should only be alloted later.

Pooja: The number should only be assigned once it's submitted as a draft PR.

Shashank: As an easier identification, what's a prefix for that predraft.

Micah: For predraft, we should be soliciting feedback on the idea. But we should not frame it as a standard. The issue is, someone creates an idea that isn't merged, then they tell others to implement this EIP that doesn't exist. If you want to collect wider feedback, you should create a draft. If you just want to get a small pool of people to look at your thing, you should post on EthMagicians.

Shashank: I was asking for a category to automate it.

Micah: I don't think so, draft is the first step. We just need them to follow the rules. I've merged drafts where the body is just TBD. If you're like Greg, and you want to discuss it beforehand, I'm ok with that. 

Greg: Github now has this Draft PR. You can put it up there, which helps. I don't want to see these empty drafts going up, that really clutters things. I don't care about the issues clutter.

Micah: I could be convinced to set the bar higher for Drafts. 

Greg: I don't want drafts cluttered up. If we get drafts that are dead.

Pooja: With the EIP bot, those drafts would be moved to stagnant. If we keep having hundred and thousands of open issues, I don't see that advantage. We can never address issues with regards to the EIP repo, it would get lost.

Greg: The Draft PR works pretty well. It can't be merged, the bot doesn't care about it, the editors don't have to look at it. That works for a number, and has something to point to for discussion.

Micah: I'm fine with people making draft PRs. But not for people getting a number. People start spamming it, other projects using. This happens often. If you get a number, your EIP should be in the repo, so people can link to it.

Greg: You find in other processes, anyone can write a draft, and it'll get a number, but there will be a lot of proposals with dead numbers.

Micah: I'm ok with that, as long as the formatting is fine.

Greg: I don't want that repo cluttered with ideas that don't ge really far. It's a hassle to go through an editor for this very first stage. 

Pooja: We are trying to get more editors onboard. The apprentiship program is helping with this. Maybe an author may not have to wait for years to get a review, and we can fasttrack these proposals, at least those which are likely to become a standard.

Greg: RFC has two categories. Draft and standard.

Lightclient: Yes, but there's a process for recieving a number, you can't just go to a URL to getting a number. So there's a preprocess.

Greg: RFC members tend to be much more professional than we are.

Pooja: We have 8 minutes left for this meeting. If we can, we can bring this back next meeting. I want to bring attention to these spam issues. It may be interesting to learn how we can reduce these spam issues.

Micah: When this happens, please report this content for spam. I report 5 or 6 a day, and Github does ban these people. If they get banned, their account is deleted.

Pooja: That's a good suggestion. When I looked into that, they tried to make an impression they are contributing to the Ethereum repository, but what they're doing is they're spammer.

Micah: This is a tool scammers use. It may cost them more time and effort to create new accounts, and prevents people getting scammed.

## Actions

- **46.2** - Continue discussion to move all discussion-to and predrafts to Ethereum Magicians.


# 2. Update eip-bot to add Greg Colvin as reviewer to notify his availability Ref: Discord

Video | [51:55](https://youtu.be/xEuy8b5cJjU?t=3115)
-|-

From the discussion from the Discord chat, Greg is interested in reviewing the propoals, but he wasn't getting a notification.

Micah: We don't need to update the bot, just create a PR to a file that has a list of who gets notified for which issue types.

Pooja: Shashank, could you take care of it?

Micah: I recommend Greg take care of it, so he can choose which he's notified for. (He sent Greg a link).

Greg: This whole thing has been frustrating for me. For years I was an editor. But suddenly I wasn't. And I had to argue with people to become an editor again.

Pooja: I apologize for the inconveniences. That's why we have this meeting biweekly. We hope to see you in future meetings.

## Actions

- **46.3** - Merge Greg's PR for him to recieve notifications for EIPs.


# 3. EIPs Insight - Monthly EIPs status reporting.

Video | [54:29](https://youtu.be/xEuy8b5cJjU?t=3269)
-|-

Pooja showed the December insight. A few proposals were pulled back from stagnant to draft. No proposal in last call. The arror glacier proposal, I don't see it moving to final status. The author needs to submit the PR (Will ping Tim Beiko).

Link: https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight.

# 4. EIP editor apprenticeship meeting

Video | [55:49](https://youtu.be/xEuy8b5cJjU?t=3349)
-|-

It was a great session. People had questions we tried to answer. 

People trying to join as an editor, it's really helpful. Editors, if you have an ideas how to mature them from the apprenticeship, let me know.

Micah: I recenlty moved. So I'm way behind on emails. I'm behind on EIPs. If anyone wants to go through core EIPs, do so. Because I've been away for about a week.

Pooja: I can forward that to contributors. I'm sure you'll be back very soon.


# 5. Review action items from the previous meeting

Video | [57:57](https://youtu.be/xEuy8b5cJjU?t=3477)
-|-

One of the most important discussion was the placeholder. I wonder if Matt has permissions to update that.

Lightclient: I'd need someone to add me the role to create ownerships for a brief moment. Otherwise I can't do that.

Pooja: I can contact the Dev Ops team, and try to get it resolved.

One last question. The next meeting is for December 29th. Or do we want to do January? Let's schedule for Januar 12th. Let's keep it open, may meet sooner if any urgent issues arise.

---

# Annex

## Attendees 

- Alita Moore
- Brent Allsop
- Edson Ayllon
- Felix
- Lightclient
- Micah Zoltu
- Pooja Ranjan


## Next Call 

Wednesday, January 12, 2021, 15:00 UTC.

