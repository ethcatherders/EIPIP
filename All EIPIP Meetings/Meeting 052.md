# EIPIP Meeting 52 Notes
## Meeting Date/Time: Wednesday 23 March 2022 at 15:00 UTC
### Meeting Duration: 1/2 hour
### [GitHub Agenda Page](https://github.com/ethereum-cat-herders/EIPIP/issues/116)
### [Audio/Video of the meeting](https://youtu.be/Wm8uYrAHAyE)
### Moderator: ****Pooja Ranjan****
### Notes: Stefan Wüst

----
## ACTION ITEMS

**ACTION 52.1**: Pooja to review current list of admins with issue delete permissions and add/remove as needed 
**ACTION 52.2**: Pooja to start including number of EIPs waiting to be merged as well as a breakdown by category in EIP Insight stats
**ACTION 52.3**: Sam to draft a proposal for removing Core EIPs from the standard process to optimize for Core Dev usage
**ACTION 52.4**: Discuss streamlining / automating EIP content, especially for Core EIPs

---
## AGENDA ##
## 1. Github discussions for discussions-to [Ref](https://github.com/ethereum/EIPs/issues/4879):
* Pooja noted that outstanding concerns with using [Ethereum Magicians](https://ethereum-magicians.org/) have been resolved
* Micah confirmed no other known issues and that he has already been directing discsussion of specific EIPs to [Ethereum Magicians](https://ethereum-magicians.org/), unless they are related to EIP process itself
* Sam also confirmed no outstanding issues
## 2. Removing Spam Issues & Comments Ref: [Discord](https://discord.com/channels/595666850260713488/746566142700814426/953185552000229386)
* Spam within Ethereum repositories remains a concern in terms of both malicious as well as unintentiounally duplicative content
* Pooja noted that proposed solution is to enable EIP editors to delete such issues
* Micah mentioned security concerns with having too many people with access to delete issues; recommended potentially taking away other people's delete rights to keep the list of people with access short
* Pooja recommended a review of the current list to make sure it is up to date to address Micah's concern 
## 3. Discuss use of Git Submodules [Ref](https://github.com/ethereum-cat-herders/EIPIP/issues/116#issuecomment-1076352599) and [here](https://github.com/ethereum/EIPs/issues/4921)
* Micah noted concerns with usage of submodules as it creates additional complexity to the repo
* Sam agreed with Micah's concerns and suggested keeping submodules limited for the time being and revisiting if usage continues
* Pooja noted that there is consesus on Sam's proposal on handling submodules moving forward 
## 4. [Mention number of EIP drafts that were submitted but not merged in EIPs Insight](https://github.com/ethereum-cat-herders/EIPIP/issues/115)
* Request has been received to track number of PRs waiting to be merged and provide a breakdown by type (ERC, core, etc)
* Pooja questioned whether there are any concerns with tracking this information
* Sam and Micah agree that there is no downside to providing this info if it is not too onerous to track as this would not be a high priority item
* Pooja noted that adding this information should not be onerous and might also highlight when EIP editors are becoming overwhelmed with EIPs. This new information will be added to EIP Insight starting end of March
## 5. Core EIPs in an [Executable Spec World Proposal](https://notes.ethereum.org/@timbeiko/executable-eips) and [Discussion](https://ethereum-magicians.org/t/core-eips-in-an-executable-spec-world/8640)
* Micah noted a desire to remove Core EIPs out of the standard EIP process post executable spec implementation, but believes it is unlikely to happen given current preferences of the team. 
* Sam mentioned this is something that could be picked up with Shanghai and agreed to write up a proposal per Micah's suggestion. In particular, create a tighter integration/package of all the necessary components of the change rather than using links among documents that can change on their own and cleanup the template of what content needs to be included in the Core EIP.  
* Pooja noted concerns with removing some of the proposed content as it makes it easier for more people outside the ETH dev teams to better understand the EIP. Micah commented that automating generation of some of that content could be a reasonable compromise. 
* Pooja recommended raising this as a discussion as the next meeting
## 6. EIP [bot Issues](https://github.com/ethereum/EIP-Bot/issues) and [eipv Issues](https://github.com/ethereum/eipv/issues) updates
* Development is ongoing but progress is slow given number of people working on them
* Pooja highlighted a need for Ruby developers in particular and requested anyone interested to reach out to ECH discord
## 7. [EIPs Insight](https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/https%3A%2F%2Fhackmd.io%2F%40poojaranjan%2FEIPsInsightMarch2022) - Monthly EIPs status reporting.
* Report is up to date as of meeting time - [Report Link](https://hackmd.io/@poojaranjan/EthereumImprovementProposalsInsight/https%3A%2F%2Fhackmd.io%2F%40poojaranjan%2FEIPsInsightMarch2022)
* Pooja raised a [new PR](https://github.com/ethereum/EIPs/pull/4880) for discussion and Sam/Micah agreed on the shorted wording option. Pull request was updated to reflect this agreement for further consideration prior.
## 8. EIP editor apprenticeship meeting
* [Meeting 14 Recording](https://youtu.be/FU6FXir-GMY) now available. Next meeting to take place on Apr 5
## 9. EIPIP meeting time and name [survey](https://docs.google.com/forms/d/e/1FAIpQLSchmERP_dueiskdi-SlJCa57s7p7Ku5u_wTOJtlqTefpENglg/viewform)
* Survey/discussion ongoing among EIP editors to increase attendance at EIPIP meeting
* Next meeting will be on 6 Apr 14:00UTC (instead of 15:00UTC)
## 10. Review action items from the [previous meeting](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20051.md)
 * All action items have been resolved
 
## Additional topics
* Pooja noted an increase in participation from the community in raising issues for EIP Editors review and re-iterated long-term goal of replacing discussion-to links to further increase engagement. 
* Micah suggested inviting active participants to the meeting for live discussion

Next meeting - Apr 06, 2022 14:00UTC

(Anything else, please add a comment)

# Attendees

* Pooja Ranjan (Host)
* Micah Zoltu
* Sam Wilson
