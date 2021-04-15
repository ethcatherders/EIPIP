# EIPIP Meeting 30 Notes 

### Meeting Date/Time: Wednesday 2021/04/07 at 14:00 UTC 
### Meeting Duration:  55 min 
### [GitHub Agenda](https://github.com/ethereum-cat-herders/EIPIP/issues/62) 
### [Audio/Video of the meeting](https://youtu.be/FdCeXxok2Fw) 
### Moderator: Pooja Ranjan
### Notes: Pedro Rivera 
### [Previous Call (29)](https://github.com/ethereum-cat-herders/EIPIP/blob/master/All%20EIPIP%20Meetings/Meeting%20029.md)

## Decisions Made

| Decision Item | Description | Video ref |
| ------------- | ----------- | --------- |
| **30.1**      | Split EIP and ERC repos and minimize number overlaps by offsetting ERC and EIP numbers by an amount in the thousands. | [5:40](https://youtu.be/FdCeXxok2Fw?t=340) |     
| **30.2**      | JSON RPC spec shall be documented under eth1.0-specs/json-rpc | [35:10](https://youtu.be/FdCeXxok2Fw?t=2110) | 
| **30.3**      | Remove "testing greelight" from EIP process. | [43:15](https://youtu.be/FdCeXxok2Fw?t=2595)  | 

## Action Items

| Action Item | Description |
| ------------| ----------- |
| **30.1**    | Alita to take on the solution for minimizing EIP/ERC number overlaps.|
| **30.2**    | Spread the word and find an entry-level resource to contiribute to the JSON RPC spec.|
| **30.3**    | Tim Beiko will bring up the agreed changes to the EIP process in the All Core Devs meeting.|
-----------------------------

## Splitting out EIP repos into EIPs & ERCs

* **Pooja** introduces the topic, which stems from the decision made in the previous meeting. The agreement was to have EIP editors that are separate from ERC editors in order to split notifications to editors of EIP/ERC. However, one potential conflict would be numbering, as some people want to avoid overlaps.
* **Micah** stated his weak preference for simply allowing collisions, but then recognized the downside is multiple cases of user confusion. 
* **Hudson** voiced his preference to mitigate overlaps by offsetting the ERCs/EIPs by 1000 or so. **Micah** pointed out that to do this some solution to pick numbers must be devised. One option is to burn through issue numbers 1-N through a script to induce the offset. 
**Pooja** suggested an alternative, however, it does not allow for independent subscriptions to ERC and EIP. 
* **Micah** mentions again it could be easy to write a script that burns through 1-3500 on ERCs repo, and that it is probably the easiest and satisfying the most people. Would only need to find someone to do it. Alita could pick it up, since she voiced her interest.
* **lightclient** objects he still feels there should not be overlaps between ERCs and EIPs. Proposes some central source or having another repo to create an issue to create a number so they happen sequentially. **Micah** inquires about his concern and, after a brief discussion, it is concluded that the decisions we take here don't matter much long term, so, it's okay if we take on some short term technical debt because lightclient's concerns will likely disappear in the future (eventually the EIP process will change, but until that happens we still do want them split apart).
* **Micah** lays out a few different ways to implement the number picking. **Pooja** confirms **Alita**'s interest in contributing, so she proposes **Alita** consults **Micah** and **lightclient** for guidance, which they give consent to.
* **Pooja** states one last thing. We are working on securing funding for EIP and ERC; It would be helpful to hire people. If we could discuss (now or in another meeting) how much funds would be needed in 3-6 months, that would be helpful. **Micah** says it depends on how high is the quality "vendors". The subject seemingly gets postponed.
* **Micah** warns someone should probably look at the ERCs they are starting to pile up. **lightclient** acknowledges he hasn't been able to catch up due to a hand injury that slows him down.

## JSON RPC API spec, support needed for coordination & funding ([17:04](https://youtu.be/FdCeXxok2Fw?t=1024))

* **Pooja** shares a recap of this topic. In brief, [PEEP an EIP-1474](https://youtu.be/fxhXsg9g4nc) revealed we should have kind of place holder for this kind of spec, potentially under ethereum/eth1.0-specs, or somewhere else. **Tomasz Stanczak** has been leading the JSON RPC calls, so he joins Today to discuss the best way forward.
* **Tomasz** summarizes the main outcomes of their meetings from the last 2-3 months: 
	1. They no longer want to approach it at the level of the entire JSON RPC because that is where most differences appear, and these differences aren't necessarily undesired. However, at the level of single endpoints like `eth_block_number` or `eth_call`, those are widely used and implemented in every client and that is where the low-level specification is currently missing. The form in which specs are implemented is irrelevant to them; what they want to ensure is that specification is complete at the endpoint level and that every single endpoint is spec'd separately. 
	2. We do want to have some formal way to define these interfaces for uses such as implementing automatic codegen or verification (i.e. machine-readable spec). So, there was agreement that OpenRPC format can be reused (as Ethereum Classic) and there is someone (**Zachary**) ready to jump into it. 
	3. We don't want to create a single doc, but after creating many docs, we want to create a single list that references all of those. With regards to hosting, ethereum.org is proposed. 

* **Pooja** mentions there was chat on Discord about creating a folder in eth1.0-specs for JSON RPC spec content. She asks for thoughts from the group. **Tomasz** replies it isn't formally defined, but it should probably be reviewed with people from each client team. 
* **Micah** says having a finite number of editors who are familiar with the process is valuable, recommending to have a group most familiar with the process and everybody else operates on PRs. **Tomasz** agrees maybe one or two people writing the spec. Erik suggested Zachary, and if there is anyone interested who is familiar with this, he is happy to connect this person with people/tools/teams.
* **Pooja** asks about staffing/funding for this development. **Tomasz** underlines that funding is not an issue in this case, rather finding the appropiate person. He clarifies it is probably an entry-level task. **Pooja** will spread word around. 
* **Pooja** concludes that creating the eth1.0-specs folder should not be a challenge. **Tim Beiko** and **Hudson** are admins, so access is straight forward. 
* **Pooja** requests starting info for the spec. **Tomasz** says he will share it in the EIP format. To this, **Micah** suggests rather modeling it with the eth2.0 format, which makes it less wordy and faster to iterate on. **Tim** adds a supporting argument for the eth2.0 format (more future proof). However, **Tomasz** critically requests a  very clear idea of where it should land. To him it feels vague, without a roadmap. **Tim** agrees there is no problem if it is under eth1.0-specs then. He also confirms it's fine for it to be a top-level folder, since re-org is likely to happen anyway. **Pooja** concludes it would be under eth1.0-specs/json-rpc.
* Lastly, **Tim** agrees to update the eth1.0-specs readme to override the current statement that the repo is only for network upgrades.

## EIPs & Network Upgrade Process Requirements ([36:38](https://youtu.be/FdCeXxok2Fw?t=2199))

* **Pooja** gives the overview of [the issue](https://github.com/ethereum/pm/issues/264#issuecomment-814337690)
* It is briefly discussed and agreed that "Testing green light" does not exist, so there is no sense to have that.
* **Tim** clarifies the time to move EIPs for last call is when we agree on a list of EIPs for a hard fork. We don't want them to be already on a testnet. In other words, it has to be in review, and it moves to last call when we're sure it's going into a block number.
* **Hudson** requests to clarify the meaning of "last call", as he had the understanding that it was more flexible for change. **Tim** defines it as "people should look at this right now because it's going on mainnet." Changes can still happen but the burden to change is very high.
* **Hudson** then asks whether "last call" should mean the same thing for ERCs? **Tim** thinks definition for last call in EIP1 is good. Short after, there is some discussion around the meaning of "normative change".
* There is some clarification on how the process stands without the "testing greenlight" block. **Tim** says we just get rid of the testing greelight box, and remove the review box. Public testnet should be in last call, because we have to set the fork block number before we do the public testnet. **Pooja** will update that sheet, and **Tim** will bring it up in All Core Devs.
* **Pooja** mentions another noteworthy change. The last call duration was equal to 14 days, it will now be _minimum_ 14 days.
* **lightclient** asks about meaning of CFI with the motivation of knowing if CFI is that "stamp" that makes an EIP relevant to look at and analyze (he brings up that it's hard to identify relevant EIPs). **Tim** comments that lately his view is that the CFI status should be reconsidered with each fork because so much context changes ([link to proposal](https://github.com/ethereum/pm/issues/295)). **lightclient** suggests in the future having a way to track what's CFI with its corresponding decision criteria. 


## Progress on 'canonical source for EIPs' ([51:00](https://youtu.be/FdCeXxok2Fw?t=3060))

* **Brent Allsop** says he's making progress. They have a [staging site](https://eips_staging.canonizer.com/) up.
* He asks how changes are made to ethereum.org. **Hudson** says it's an open source [repo on GitHub](https://github.com/ethereum/ethereum-org-website/), so just doing a PR on that is the way to go.

-----------------

## Attendees 
- Brent Alllsop
- Hudson Jameson
- lightclient
- Mikah Zoltu
- Pooja Ranjan
- Tim Beiko
- Tomasz Stanczak
- Trent Van Epps

## Next Meeting Date/Time

Wednesday, April 21, 2021, UTC 15:00.
