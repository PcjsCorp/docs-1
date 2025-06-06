---
title: Events
---

Events are emitted for certain operations on the runtime. The following sections describe the events that are part of the default Substrate runtime. 

(NOTE: These were generated from a static/snapshot view of a recent default Substrate runtime. Some items may not be available in older nodes, or in any customized implementations.)

- **[alliance](#alliance)**

- **[allianceMotion](#alliancemotion)**

- **[assetConversion](#assetconversion)**

- **[assetConversionMigration](#assetconversionmigration)**

- **[assetConversionTxPayment](#assetconversiontxpayment)**

- **[assetRate](#assetrate)**

- **[assetRewards](#assetrewards)**

- **[assets](#assets)**

- **[assetsFreezer](#assetsfreezer)**

- **[balances](#balances)**

- **[bounties](#bounties)**

- **[broker](#broker)**

- **[childBounties](#childbounties)**

- **[contracts](#contracts)**

- **[convictionVoting](#convictionvoting)**

- **[coreFellowship](#corefellowship)**

- **[council](#council)**

- **[delegatedStaking](#delegatedstaking)**

- **[democracy](#democracy)**

- **[electionProviderMultiPhase](#electionprovidermultiphase)**

- **[elections](#elections)**

- **[fastUnstake](#fastunstake)**

- **[glutton](#glutton)**

- **[grandpa](#grandpa)**

- **[identity](#identity)**

- **[imOnline](#imonline)**

- **[indices](#indices)**

- **[lottery](#lottery)**

- **[messageQueue](#messagequeue)**

- **[metaTx](#metatx)**

- **[multiBlockMigrations](#multiblockmigrations)**

- **[multisig](#multisig)**

- **[nftFractionalization](#nftfractionalization)**

- **[nfts](#nfts)**

- **[nis](#nis)**

- **[nominationPools](#nominationpools)**

- **[offences](#offences)**

- **[parameters](#parameters)**

- **[poolAssets](#poolassets)**

- **[pov](#pov)**

- **[preimage](#preimage)**

- **[proxy](#proxy)**

- **[rankedCollective](#rankedcollective)**

- **[rankedPolls](#rankedpolls)**

- **[recovery](#recovery)**

- **[referenda](#referenda)**

- **[remark](#remark)**

- **[revive](#revive)**

- **[rootTesting](#roottesting)**

- **[safeMode](#safemode)**

- **[salary](#salary)**

- **[scheduler](#scheduler)**

- **[session](#session)**

- **[skipFeelessPayment](#skipfeelesspayment)**

- **[society](#society)**

- **[staking](#staking)**

- **[statement](#statement)**

- **[stateTrieMigration](#statetriemigration)**

- **[sudo](#sudo)**

- **[system](#system)**

- **[technicalCommittee](#technicalcommittee)**

- **[technicalMembership](#technicalmembership)**

- **[tips](#tips)**

- **[transactionPayment](#transactionpayment)**

- **[transactionStorage](#transactionstorage)**

- **[treasury](#treasury)**

- **[txPause](#txpause)**

- **[uniques](#uniques)**

- **[utility](#utility)**

- **[vesting](#vesting)**

- **[voterList](#voterlist)**

- **[whitelist](#whitelist)**


___


## alliance
 
### AllianceDisbanded(`u32`, `u32`, `u32`)
- **interface**: `api.events.alliance.AllianceDisbanded.is`
- **summary**:    Alliance disbanded. Includes number deleted members and unreserved deposits. 
 
### AllyElevated(`AccountId32`)
- **interface**: `api.events.alliance.AllyElevated.is`
- **summary**:    An ally has been elevated to Fellow. 
 
### Announced(`PalletAllianceCid`)
- **interface**: `api.events.alliance.Announced.is`
- **summary**:    A new announcement has been proposed. 
 
### AnnouncementRemoved(`PalletAllianceCid`)
- **interface**: `api.events.alliance.AnnouncementRemoved.is`
- **summary**:    An on-chain announcement has been removed. 
 
### FellowAbdicated(`AccountId32`)
- **interface**: `api.events.alliance.FellowAbdicated.is`
- **summary**:    A Fellow abdicated their voting rights. They are now an Ally. 
 
### MemberKicked(`AccountId32`, `Option<u128>`)
- **interface**: `api.events.alliance.MemberKicked.is`
- **summary**:    A member has been kicked out with its deposit slashed. 
 
### MemberRetired(`AccountId32`, `Option<u128>`)
- **interface**: `api.events.alliance.MemberRetired.is`
- **summary**:    A member has retired with its deposit unreserved. 
 
### MemberRetirementPeriodStarted(`AccountId32`)
- **interface**: `api.events.alliance.MemberRetirementPeriodStarted.is`
- **summary**:    A member gave retirement notice and their retirement period started. 
 
### MembersInitialized(`Vec<AccountId32>`, `Vec<AccountId32>`)
- **interface**: `api.events.alliance.MembersInitialized.is`
- **summary**:    Some accounts have been initialized as members (fellows/allies). 
 
### NewAllyJoined(`AccountId32`, `Option<AccountId32>`, `Option<u128>`)
- **interface**: `api.events.alliance.NewAllyJoined.is`
- **summary**:    An account has been added as an Ally and reserved its deposit. 
 
### NewRuleSet(`PalletAllianceCid`)
- **interface**: `api.events.alliance.NewRuleSet.is`
- **summary**:    A new rule has been set. 
 
### UnscrupulousItemAdded(`Vec<PalletAllianceUnscrupulousItem>`)
- **interface**: `api.events.alliance.UnscrupulousItemAdded.is`
- **summary**:    Accounts or websites have been added into the list of unscrupulous items. 
 
### UnscrupulousItemRemoved(`Vec<PalletAllianceUnscrupulousItem>`)
- **interface**: `api.events.alliance.UnscrupulousItemRemoved.is`
- **summary**:    Accounts or websites have been removed from the list of unscrupulous items. 

___


## allianceMotion
 
### Approved(`H256`)
- **interface**: `api.events.allianceMotion.Approved.is`
- **summary**:    A motion was approved by the required threshold. 
 
### Closed(`H256`, `u32`, `u32`)
- **interface**: `api.events.allianceMotion.Closed.is`
- **summary**:    A proposal was closed because its threshold was reached or after its duration was up. 
 
### Disapproved(`H256`)
- **interface**: `api.events.allianceMotion.Disapproved.is`
- **summary**:    A motion was not approved by the required threshold. 
 
### Executed(`H256`, `Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.allianceMotion.Executed.is`
- **summary**:    A motion was executed; result will be `Ok` if it returned without error. 
 
### Killed(`H256`)
- **interface**: `api.events.allianceMotion.Killed.is`
- **summary**:    A proposal was killed. 
 
### MemberExecuted(`H256`, `Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.allianceMotion.MemberExecuted.is`
- **summary**:    A single member did some action; result will be `Ok` if it returned without error. 
 
### ProposalCostBurned(`H256`, `AccountId32`)
- **interface**: `api.events.allianceMotion.ProposalCostBurned.is`
- **summary**:    Some cost for storing a proposal was burned. 
 
### ProposalCostReleased(`H256`, `AccountId32`)
- **interface**: `api.events.allianceMotion.ProposalCostReleased.is`
- **summary**:    Some cost for storing a proposal was released. 
 
### Proposed(`AccountId32`, `u32`, `H256`, `u32`)
- **interface**: `api.events.allianceMotion.Proposed.is`
- **summary**:    A motion (given hash) has been proposed (by given account) with a threshold (given  `MemberCount`). 
 
### Voted(`AccountId32`, `H256`, `bool`, `u32`, `u32`)
- **interface**: `api.events.allianceMotion.Voted.is`
- **summary**:    A motion (given hash) has been voted on by given account, leaving  a tally (yes votes and no votes given respectively as `MemberCount`). 

___


## assetConversion
 
### LiquidityAdded(`AccountId32`, `AccountId32`, `(FrameSupportTokensFungibleUnionOfNativeOrWithId,FrameSupportTokensFungibleUnionOfNativeOrWithId)`, `u128`, `u128`, `u32`, `u128`)
- **interface**: `api.events.assetConversion.LiquidityAdded.is`
- **summary**:    A successful call of the `AddLiquidity` extrinsic will create this event. 
 
### LiquidityRemoved(`AccountId32`, `AccountId32`, `(FrameSupportTokensFungibleUnionOfNativeOrWithId,FrameSupportTokensFungibleUnionOfNativeOrWithId)`, `u128`, `u128`, `u32`, `u128`, `Permill`)
- **interface**: `api.events.assetConversion.LiquidityRemoved.is`
- **summary**:    A successful call of the `RemoveLiquidity` extrinsic will create this event. 
 
### PoolCreated(`AccountId32`, `(FrameSupportTokensFungibleUnionOfNativeOrWithId,FrameSupportTokensFungibleUnionOfNativeOrWithId)`, `AccountId32`, `u32`)
- **interface**: `api.events.assetConversion.PoolCreated.is`
- **summary**:    A successful call of the `CreatePool` extrinsic will create this event. 
 
### SwapCreditExecuted(`u128`, `u128`, `Vec<(FrameSupportTokensFungibleUnionOfNativeOrWithId,u128)>`)
- **interface**: `api.events.assetConversion.SwapCreditExecuted.is`
- **summary**:    Assets have been converted from one to another. 
 
### SwapExecuted(`AccountId32`, `AccountId32`, `u128`, `u128`, `Vec<(FrameSupportTokensFungibleUnionOfNativeOrWithId,u128)>`)
- **interface**: `api.events.assetConversion.SwapExecuted.is`
- **summary**:    Assets have been converted from one to another. Both `SwapExactTokenForToken`  and `SwapTokenForExactToken` will generate this event. 
 
### Touched(`(FrameSupportTokensFungibleUnionOfNativeOrWithId,FrameSupportTokensFungibleUnionOfNativeOrWithId)`, `AccountId32`)
- **interface**: `api.events.assetConversion.Touched.is`
- **summary**:    Pool has been touched in order to fulfill operational requirements. 

___


## assetConversionMigration
 
### MigratedToNewAccount(`(FrameSupportTokensFungibleUnionOfNativeOrWithId,FrameSupportTokensFungibleUnionOfNativeOrWithId)`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.assetConversionMigration.MigratedToNewAccount.is`
- **summary**:    Indicates that a pool has been migrated to the new account ID. 

___


## assetConversionTxPayment
 
### AssetRefundFailed(`u128`)
- **interface**: `api.events.assetConversionTxPayment.AssetRefundFailed.is`
- **summary**:    A swap of the refund in native currency back to asset failed. 
 
### AssetTxFeePaid(`AccountId32`, `u128`, `u128`, `FrameSupportTokensFungibleUnionOfNativeOrWithId`)
- **interface**: `api.events.assetConversionTxPayment.AssetTxFeePaid.is`
- **summary**:    A transaction fee `actual_fee`, of which `tip` was added to the minimum inclusion fee,  has been paid by `who` in an asset `asset_id`. 

___


## assetRate
 
### AssetRateCreated(`FrameSupportTokensFungibleUnionOfNativeOrWithId`, `u128`)
- **interface**: `api.events.assetRate.AssetRateCreated.is`
 
### AssetRateRemoved(`FrameSupportTokensFungibleUnionOfNativeOrWithId`)
- **interface**: `api.events.assetRate.AssetRateRemoved.is`
 
### AssetRateUpdated(`FrameSupportTokensFungibleUnionOfNativeOrWithId`, `u128`, `u128`)
- **interface**: `api.events.assetRate.AssetRateUpdated.is`

___


## assetRewards
 
### PoolAdminModified(`u32`, `AccountId32`)
- **interface**: `api.events.assetRewards.PoolAdminModified.is`
- **summary**:    A pool admin was modified. 
 
### PoolCleanedUp(`u32`)
- **interface**: `api.events.assetRewards.PoolCleanedUp.is`
- **summary**:    A pool information was cleared after it's completion. 
 
### PoolCreated(`AccountId32`, `u32`, `FrameSupportTokensFungibleUnionOfNativeOrWithId`, `FrameSupportTokensFungibleUnionOfNativeOrWithId`, `u128`, `u32`, `AccountId32`)
- **interface**: `api.events.assetRewards.PoolCreated.is`
- **summary**:    A new reward pool was created. 
 
### PoolExpiryBlockModified(`u32`, `u32`)
- **interface**: `api.events.assetRewards.PoolExpiryBlockModified.is`
- **summary**:    A pool expiry block was modified by the admin. 
 
### PoolRewardRateModified(`u32`, `u128`)
- **interface**: `api.events.assetRewards.PoolRewardRateModified.is`
- **summary**:    A pool reward rate was modified by the admin. 
 
### RewardsHarvested(`AccountId32`, `AccountId32`, `u32`, `u128`)
- **interface**: `api.events.assetRewards.RewardsHarvested.is`
- **summary**:    An account harvested some rewards. 
 
### Staked(`AccountId32`, `u32`, `u128`)
- **interface**: `api.events.assetRewards.Staked.is`
- **summary**:    An account staked some tokens in a pool. 
 
### Unstaked(`AccountId32`, `AccountId32`, `u32`, `u128`)
- **interface**: `api.events.assetRewards.Unstaked.is`
- **summary**:    An account unstaked some tokens from a pool. 

___


## assets
 
### AccountsDestroyed(`u32`, `u32`, `u32`)
- **interface**: `api.events.assets.AccountsDestroyed.is`
- **summary**:    Accounts were destroyed for given asset. 
 
### ApprovalCancelled(`u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.assets.ApprovalCancelled.is`
- **summary**:    An approval for account `delegate` was cancelled by `owner`. 
 
### ApprovalsDestroyed(`u32`, `u32`, `u32`)
- **interface**: `api.events.assets.ApprovalsDestroyed.is`
- **summary**:    Approvals were destroyed for given asset. 
 
### ApprovedTransfer(`u32`, `AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.assets.ApprovedTransfer.is`
- **summary**:    (Additional) funds have been approved for transfer to a destination account. 
 
### AssetFrozen(`u32`)
- **interface**: `api.events.assets.AssetFrozen.is`
- **summary**:    Some asset `asset_id` was frozen. 
 
### AssetMinBalanceChanged(`u32`, `u128`)
- **interface**: `api.events.assets.AssetMinBalanceChanged.is`
- **summary**:    The min_balance of an asset has been updated by the asset owner. 
 
### AssetStatusChanged(`u32`)
- **interface**: `api.events.assets.AssetStatusChanged.is`
- **summary**:    An asset has had its attributes changed by the `Force` origin. 
 
### AssetThawed(`u32`)
- **interface**: `api.events.assets.AssetThawed.is`
- **summary**:    Some asset `asset_id` was thawed. 
 
### Blocked(`u32`, `AccountId32`)
- **interface**: `api.events.assets.Blocked.is`
- **summary**:    Some account `who` was blocked. 
 
### Burned(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.assets.Burned.is`
- **summary**:    Some assets were destroyed. 
 
### Created(`u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.assets.Created.is`
- **summary**:    Some asset class was created. 
 
### Deposited(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.assets.Deposited.is`
- **summary**:    Some assets were deposited (e.g. for transaction fees). 
 
### Destroyed(`u32`)
- **interface**: `api.events.assets.Destroyed.is`
- **summary**:    An asset class was destroyed. 
 
### DestructionStarted(`u32`)
- **interface**: `api.events.assets.DestructionStarted.is`
- **summary**:    An asset class is in the process of being destroyed. 
 
### ForceCreated(`u32`, `AccountId32`)
- **interface**: `api.events.assets.ForceCreated.is`
- **summary**:    Some asset class was force-created. 
 
### Frozen(`u32`, `AccountId32`)
- **interface**: `api.events.assets.Frozen.is`
- **summary**:    Some account `who` was frozen. 
 
### Issued(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.assets.Issued.is`
- **summary**:    Some assets were issued. 
 
### MetadataCleared(`u32`)
- **interface**: `api.events.assets.MetadataCleared.is`
- **summary**:    Metadata has been cleared for an asset. 
 
### MetadataSet(`u32`, `Bytes`, `Bytes`, `u8`, `bool`)
- **interface**: `api.events.assets.MetadataSet.is`
- **summary**:    New metadata has been set for an asset. 
 
### OwnerChanged(`u32`, `AccountId32`)
- **interface**: `api.events.assets.OwnerChanged.is`
- **summary**:    The owner changed. 
 
### TeamChanged(`u32`, `AccountId32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.assets.TeamChanged.is`
- **summary**:    The management team changed. 
 
### Thawed(`u32`, `AccountId32`)
- **interface**: `api.events.assets.Thawed.is`
- **summary**:    Some account `who` was thawed. 
 
### Touched(`u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.assets.Touched.is`
- **summary**:    Some account `who` was created with a deposit from `depositor`. 
 
### Transferred(`u32`, `AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.assets.Transferred.is`
- **summary**:    Some assets were transferred. 
 
### TransferredApproved(`u32`, `AccountId32`, `AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.assets.TransferredApproved.is`
- **summary**:    An `amount` was transferred in its entirety from `owner` to `destination` by  the approved `delegate`. 
 
### Withdrawn(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.assets.Withdrawn.is`
- **summary**:    Some assets were withdrawn from the account (e.g. for transaction fees). 

___


## assetsFreezer
 
### Frozen(`AccountId32`, `u32`, `u128`)
- **interface**: `api.events.assetsFreezer.Frozen.is`
 
### Thawed(`AccountId32`, `u32`, `u128`)
- **interface**: `api.events.assetsFreezer.Thawed.is`

___


## balances
 
### BalanceSet(`AccountId32`, `u128`)
- **interface**: `api.events.balances.BalanceSet.is`
- **summary**:    A balance was set by root. 
 
### Burned(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Burned.is`
- **summary**:    Some amount was burned from an account. 
 
### Deposit(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Deposit.is`
- **summary**:    Some amount was deposited (e.g. for transaction fees). 
 
### DustLost(`AccountId32`, `u128`)
- **interface**: `api.events.balances.DustLost.is`
- **summary**:    An account was removed whose balance was non-zero but below ExistentialDeposit,  resulting in an outright loss. 
 
### Endowed(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Endowed.is`
- **summary**:    An account was created with some free balance. 
 
### Frozen(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Frozen.is`
- **summary**:    Some balance was frozen. 
 
### Issued(`u128`)
- **interface**: `api.events.balances.Issued.is`
- **summary**:    Total issuance was increased by `amount`, creating a credit to be balanced. 
 
### Locked(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Locked.is`
- **summary**:    Some balance was locked. 
 
### Minted(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Minted.is`
- **summary**:    Some amount was minted into an account. 
 
### Rescinded(`u128`)
- **interface**: `api.events.balances.Rescinded.is`
- **summary**:    Total issuance was decreased by `amount`, creating a debt to be balanced. 
 
### Reserved(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Reserved.is`
- **summary**:    Some balance was reserved (moved from free to reserved). 
 
### ReserveRepatriated(`AccountId32`, `AccountId32`, `u128`, `FrameSupportTokensMiscBalanceStatus`)
- **interface**: `api.events.balances.ReserveRepatriated.is`
- **summary**:    Some balance was moved from the reserve of the first account to the second account.  Final argument indicates the destination balance type. 
 
### Restored(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Restored.is`
- **summary**:    Some amount was restored into an account. 
 
### Slashed(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Slashed.is`
- **summary**:    Some amount was removed from the account (e.g. for misbehavior). 
 
### Suspended(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Suspended.is`
- **summary**:    Some amount was suspended from an account (it can be restored later). 
 
### Thawed(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Thawed.is`
- **summary**:    Some balance was thawed. 
 
### TotalIssuanceForced(`u128`, `u128`)
- **interface**: `api.events.balances.TotalIssuanceForced.is`
- **summary**:    The `TotalIssuance` was forcefully changed. 
 
### Transfer(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.balances.Transfer.is`
- **summary**:    Transfer succeeded. 
 
### Unlocked(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Unlocked.is`
- **summary**:    Some balance was unlocked. 
 
### Unreserved(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Unreserved.is`
- **summary**:    Some balance was unreserved (moved from reserved to free). 
 
### Upgraded(`AccountId32`)
- **interface**: `api.events.balances.Upgraded.is`
- **summary**:    An account was upgraded. 
 
### Withdraw(`AccountId32`, `u128`)
- **interface**: `api.events.balances.Withdraw.is`
- **summary**:    Some amount was withdrawn from the account (e.g. for transaction fees). 

___


## bounties
 
### BountyApproved(`u32`)
- **interface**: `api.events.bounties.BountyApproved.is`
- **summary**:    A bounty is approved. 
 
### BountyAwarded(`u32`, `AccountId32`)
- **interface**: `api.events.bounties.BountyAwarded.is`
- **summary**:    A bounty is awarded to a beneficiary. 
 
### BountyBecameActive(`u32`)
- **interface**: `api.events.bounties.BountyBecameActive.is`
- **summary**:    A bounty proposal is funded and became active. 
 
### BountyCanceled(`u32`)
- **interface**: `api.events.bounties.BountyCanceled.is`
- **summary**:    A bounty is cancelled. 
 
### BountyClaimed(`u32`, `u128`, `AccountId32`)
- **interface**: `api.events.bounties.BountyClaimed.is`
- **summary**:    A bounty is claimed by beneficiary. 
 
### BountyExtended(`u32`)
- **interface**: `api.events.bounties.BountyExtended.is`
- **summary**:    A bounty expiry is extended. 
 
### BountyProposed(`u32`)
- **interface**: `api.events.bounties.BountyProposed.is`
- **summary**:    New bounty proposal. 
 
### BountyRejected(`u32`, `u128`)
- **interface**: `api.events.bounties.BountyRejected.is`
- **summary**:    A bounty proposal was rejected; funds were slashed. 
 
### CuratorAccepted(`u32`, `AccountId32`)
- **interface**: `api.events.bounties.CuratorAccepted.is`
- **summary**:    A bounty curator is accepted. 
 
### CuratorProposed(`u32`, `AccountId32`)
- **interface**: `api.events.bounties.CuratorProposed.is`
- **summary**:    A bounty curator is proposed. 
 
### CuratorUnassigned(`u32`)
- **interface**: `api.events.bounties.CuratorUnassigned.is`
- **summary**:    A bounty curator is unassigned. 

___


## broker
 
### Assigned(`PalletBrokerRegionId`, `u32`, `u32`)
- **interface**: `api.events.broker.Assigned.is`
- **summary**:    A Region has been assigned to a particular task. 
 
### AssignmentRemoved(`PalletBrokerRegionId`)
- **interface**: `api.events.broker.AssignmentRemoved.is`
- **summary**:    An assignment has been removed from the workplan. 
 
### AutoRenewalDisabled(`u16`, `u32`)
- **interface**: `api.events.broker.AutoRenewalDisabled.is`
 
### AutoRenewalEnabled(`u16`, `u32`)
- **interface**: `api.events.broker.AutoRenewalEnabled.is`
 
### AutoRenewalFailed(`u16`, `Option<AccountId32>`)
- **interface**: `api.events.broker.AutoRenewalFailed.is`
- **summary**:    Failed to auto-renew a core, likely due to the payer account not being sufficiently  funded. 
 
### AutoRenewalLimitReached()
- **interface**: `api.events.broker.AutoRenewalLimitReached.is`
- **summary**:    The auto-renewal limit has been reached upon renewing cores. 

   This should never happen, given that enable_auto_renew checks for this before enabling  auto-renewal. 
 
### ClaimsReady(`u32`, `u128`, `u128`)
- **interface**: `api.events.broker.ClaimsReady.is`
- **summary**:    Some historical Instantaneous Core Pool Revenue is ready for payout claims. 
 
### ContributionDropped(`PalletBrokerRegionId`)
- **interface**: `api.events.broker.ContributionDropped.is`
- **summary**:    Some historical Instantaneous Core Pool contribution record has been dropped. 
 
### CoreAssigned(`u16`, `u32`, `Vec<(PalletBrokerCoretimeInterfaceCoreAssignment,u16)>`)
- **interface**: `api.events.broker.CoreAssigned.is`
- **summary**:    A Core has been assigned to one or more tasks and/or the Pool on the Relay-chain. 
 
### CoreCountChanged(`u16`)
- **interface**: `api.events.broker.CoreCountChanged.is`
- **summary**:    The number of cores available for scheduling has changed. 
 
### CoreCountRequested(`u16`)
- **interface**: `api.events.broker.CoreCountRequested.is`
- **summary**:    A new number of cores has been requested. 
 
### CreditPurchased(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.broker.CreditPurchased.is`
- **summary**:    Some Instantaneous Coretime Pool credit has been purchased. 
 
### HistoryDropped(`u32`, `u128`)
- **interface**: `api.events.broker.HistoryDropped.is`
- **summary**:    Some historical Instantaneous Core Pool payment record has been dropped. 
 
### HistoryIgnored(`u32`, `u128`)
- **interface**: `api.events.broker.HistoryIgnored.is`
- **summary**:    Some historical Instantaneous Core Pool payment record has been ignored because the  timeslice was already known. Governance may need to intervene. 
 
### HistoryInitialized(`u32`, `u32`, `u32`)
- **interface**: `api.events.broker.HistoryInitialized.is`
- **summary**:    Some historical Instantaneous Core Pool payment record has been initialized. 
 
### Interlaced(`PalletBrokerRegionId`, `(PalletBrokerRegionId,PalletBrokerRegionId)`)
- **interface**: `api.events.broker.Interlaced.is`
- **summary**:    A Region has been converted into two overlapping Regions each of lesser regularity. 
 
### Leased(`u32`, `u32`)
- **interface**: `api.events.broker.Leased.is`
- **summary**:    A new lease has been created. 
 
### LeaseEnding(`u32`, `u32`)
- **interface**: `api.events.broker.LeaseEnding.is`
- **summary**:    A lease is about to end. 
 
### LeaseRemoved(`u32`)
- **interface**: `api.events.broker.LeaseRemoved.is`
- **summary**:    A lease has been removed. 
 
### Partitioned(`PalletBrokerRegionId`, `(PalletBrokerRegionId,PalletBrokerRegionId)`)
- **interface**: `api.events.broker.Partitioned.is`
- **summary**:    A Region has been split into two non-overlapping Regions. 
 
### Pooled(`PalletBrokerRegionId`, `u32`)
- **interface**: `api.events.broker.Pooled.is`
- **summary**:    A Region has been added to the Instantaneous Coretime Pool. 
 
### PotentialRenewalDropped(`u32`, `u16`)
- **interface**: `api.events.broker.PotentialRenewalDropped.is`
- **summary**:    Some historical Instantaneous Core Pool payment record has been dropped. 
 
### Purchased(`AccountId32`, `PalletBrokerRegionId`, `u128`, `u32`)
- **interface**: `api.events.broker.Purchased.is`
- **summary**:    A Region of Bulk Coretime has been purchased. 
 
### RegionDropped(`PalletBrokerRegionId`, `u32`)
- **interface**: `api.events.broker.RegionDropped.is`
- **summary**:    A Region has been dropped due to being out of date. 
 
### Renewable(`u16`, `u128`, `u32`, `Vec<PalletBrokerScheduleItem>`)
- **interface**: `api.events.broker.Renewable.is`
- **summary**:    The workload of a core has become renewable. 
 
### Renewed(`AccountId32`, `u128`, `u16`, `u16`, `u32`, `u32`, `Vec<PalletBrokerScheduleItem>`)
- **interface**: `api.events.broker.Renewed.is`
- **summary**:    A workload has been renewed. 
 
### ReservationCancelled(`u32`, `Vec<PalletBrokerScheduleItem>`)
- **interface**: `api.events.broker.ReservationCancelled.is`
- **summary**:    A reservation for a workload has been cancelled. 
 
### ReservationMade(`u32`, `Vec<PalletBrokerScheduleItem>`)
- **interface**: `api.events.broker.ReservationMade.is`
- **summary**:    There is a new reservation for a workload. 
 
### RevenueClaimBegun(`PalletBrokerRegionId`, `u32`)
- **interface**: `api.events.broker.RevenueClaimBegun.is`
- **summary**:    The act of claiming revenue has begun. 
 
### RevenueClaimItem(`u32`, `u128`)
- **interface**: `api.events.broker.RevenueClaimItem.is`
- **summary**:    A particular timeslice has a non-zero claim. 
 
### RevenueClaimPaid(`AccountId32`, `u128`, `Option<PalletBrokerRegionId>`)
- **interface**: `api.events.broker.RevenueClaimPaid.is`
- **summary**:    A revenue claim has (possibly only in part) been paid. 
 
### SaleInitialized(`u32`, `u32`, `u128`, `u128`, `u32`, `u32`, `u16`, `u16`)
- **interface**: `api.events.broker.SaleInitialized.is`
- **summary**:    A new sale has been initialized. 
 
### SalesStarted(`u128`, `u16`)
- **interface**: `api.events.broker.SalesStarted.is`
- **summary**:    The sale rotation has been started and a new sale is imminent. 
 
### Transferred(`PalletBrokerRegionId`, `u32`, `Option<AccountId32>`, `Option<AccountId32>`)
- **interface**: `api.events.broker.Transferred.is`
- **summary**:    Ownership of a Region has been transferred. 

___


## childBounties
 
### Added(`u32`, `u32`)
- **interface**: `api.events.childBounties.Added.is`
- **summary**:    A child-bounty is added. 
 
### Awarded(`u32`, `u32`, `AccountId32`)
- **interface**: `api.events.childBounties.Awarded.is`
- **summary**:    A child-bounty is awarded to a beneficiary. 
 
### Canceled(`u32`, `u32`)
- **interface**: `api.events.childBounties.Canceled.is`
- **summary**:    A child-bounty is cancelled. 
 
### Claimed(`u32`, `u32`, `u128`, `AccountId32`)
- **interface**: `api.events.childBounties.Claimed.is`
- **summary**:    A child-bounty is claimed by beneficiary. 

___


## contracts
 
### Called(`PalletContractsOrigin`, `AccountId32`)
- **interface**: `api.events.contracts.Called.is`
- **summary**:    A contract was called either by a plain account or another contract. 

   #### Note 

   Please keep in mind that like all events this is only emitted for successful  calls. This is because on failure all storage changes including events are  rolled back. 
 
### CodeRemoved(`H256`, `u128`, `AccountId32`)
- **interface**: `api.events.contracts.CodeRemoved.is`
- **summary**:    A code with the specified hash was removed. 
 
### CodeStored(`H256`, `u128`, `AccountId32`)
- **interface**: `api.events.contracts.CodeStored.is`
- **summary**:    Code with the specified hash has been stored. 
 
### ContractCodeUpdated(`AccountId32`, `H256`, `H256`)
- **interface**: `api.events.contracts.ContractCodeUpdated.is`
- **summary**:    A contract's code was updated. 
 
### ContractEmitted(`AccountId32`, `Bytes`)
- **interface**: `api.events.contracts.ContractEmitted.is`
- **summary**:    A custom event emitted by the contract. 
 
### DelegateCalled(`AccountId32`, `H256`)
- **interface**: `api.events.contracts.DelegateCalled.is`
- **summary**:    A contract delegate called a code hash. 

   #### Note 

   Please keep in mind that like all events this is only emitted for successful  calls. This is because on failure all storage changes including events are  rolled back. 
 
### Instantiated(`AccountId32`, `AccountId32`)
- **interface**: `api.events.contracts.Instantiated.is`
- **summary**:    Contract deployed by address at the specified address. 
 
### StorageDepositTransferredAndHeld(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.contracts.StorageDepositTransferredAndHeld.is`
- **summary**:    Some funds have been transferred and held as storage deposit. 
 
### StorageDepositTransferredAndReleased(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.contracts.StorageDepositTransferredAndReleased.is`
- **summary**:    Some storage deposit funds have been transferred and released. 
 
### Terminated(`AccountId32`, `AccountId32`)
- **interface**: `api.events.contracts.Terminated.is`
- **summary**:    Contract has been removed. 

   #### Note 

   The only way for a contract to be removed and emitting this event is by calling  `seal_terminate`. 

___


## convictionVoting
 
### Delegated(`AccountId32`, `AccountId32`)
- **interface**: `api.events.convictionVoting.Delegated.is`
- **summary**:    An account has delegated their vote to another account. \[who, target\] 
 
### Undelegated(`AccountId32`)
- **interface**: `api.events.convictionVoting.Undelegated.is`
- **summary**:    An \[account\] has cancelled a previous delegation operation. 
 
### Voted(`AccountId32`, `PalletConvictionVotingVoteAccountVote`)
- **interface**: `api.events.convictionVoting.Voted.is`
- **summary**:    An account has voted 
 
### VoteRemoved(`AccountId32`, `PalletConvictionVotingVoteAccountVote`)
- **interface**: `api.events.convictionVoting.VoteRemoved.is`
- **summary**:    A vote has been removed 
 
### VoteUnlocked(`AccountId32`, `u16`)
- **interface**: `api.events.convictionVoting.VoteUnlocked.is`
- **summary**:    The lockup period of a conviction vote expired, and the funds have been unlocked. 

___


## coreFellowship
 
### ActiveChanged(`AccountId32`, `bool`)
- **interface**: `api.events.coreFellowship.ActiveChanged.is`
- **summary**:    Member activity flag has been set. 
 
### Demoted(`AccountId32`, `u16`)
- **interface**: `api.events.coreFellowship.Demoted.is`
- **summary**:    Member has been demoted to the given (non-zero) rank. 
 
### EvidenceJudged(`AccountId32`, `PalletCoreFellowshipWish`, `Bytes`, `u16`, `Option<u16>`)
- **interface**: `api.events.coreFellowship.EvidenceJudged.is`
- **summary**:    Some submitted evidence was judged and removed. There may or may not have been a change  to the rank, but in any case, `last_proof` is reset. 
 
### Imported(`AccountId32`, `u16`)
- **interface**: `api.events.coreFellowship.Imported.is`
- **summary**:    Pre-ranked account has been inducted at their current rank. 
 
### Inducted(`AccountId32`)
- **interface**: `api.events.coreFellowship.Inducted.is`
- **summary**:    Member has begun being tracked in this pallet. 
 
### Offboarded(`AccountId32`)
- **interface**: `api.events.coreFellowship.Offboarded.is`
- **summary**:    Member has been removed from being tracked in this pallet (i.e. because rank is now  zero). 
 
### ParamsChanged(`PalletCoreFellowshipParamsTypeU128`)
- **interface**: `api.events.coreFellowship.ParamsChanged.is`
- **summary**:    Parameters for the pallet have changed. 
 
### Promoted(`AccountId32`, `u16`)
- **interface**: `api.events.coreFellowship.Promoted.is`
- **summary**:    Member has been promoted to the given rank. 
 
### Proven(`AccountId32`, `u16`)
- **interface**: `api.events.coreFellowship.Proven.is`
- **summary**:    Member has been proven at their current rank, postponing auto-demotion. 
 
### Requested(`AccountId32`, `PalletCoreFellowshipWish`)
- **interface**: `api.events.coreFellowship.Requested.is`
- **summary**:    Member has stated evidence of their efforts their request for rank. 
 
### Swapped(`AccountId32`, `AccountId32`)
- **interface**: `api.events.coreFellowship.Swapped.is`
- **summary**:    A member had its AccountId swapped. 

___


## council
 
### Approved(`H256`)
- **interface**: `api.events.council.Approved.is`
- **summary**:    A motion was approved by the required threshold. 
 
### Closed(`H256`, `u32`, `u32`)
- **interface**: `api.events.council.Closed.is`
- **summary**:    A proposal was closed because its threshold was reached or after its duration was up. 
 
### Disapproved(`H256`)
- **interface**: `api.events.council.Disapproved.is`
- **summary**:    A motion was not approved by the required threshold. 
 
### Executed(`H256`, `Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.council.Executed.is`
- **summary**:    A motion was executed; result will be `Ok` if it returned without error. 
 
### Killed(`H256`)
- **interface**: `api.events.council.Killed.is`
- **summary**:    A proposal was killed. 
 
### MemberExecuted(`H256`, `Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.council.MemberExecuted.is`
- **summary**:    A single member did some action; result will be `Ok` if it returned without error. 
 
### ProposalCostBurned(`H256`, `AccountId32`)
- **interface**: `api.events.council.ProposalCostBurned.is`
- **summary**:    Some cost for storing a proposal was burned. 
 
### ProposalCostReleased(`H256`, `AccountId32`)
- **interface**: `api.events.council.ProposalCostReleased.is`
- **summary**:    Some cost for storing a proposal was released. 
 
### Proposed(`AccountId32`, `u32`, `H256`, `u32`)
- **interface**: `api.events.council.Proposed.is`
- **summary**:    A motion (given hash) has been proposed (by given account) with a threshold (given  `MemberCount`). 
 
### Voted(`AccountId32`, `H256`, `bool`, `u32`, `u32`)
- **interface**: `api.events.council.Voted.is`
- **summary**:    A motion (given hash) has been voted on by given account, leaving  a tally (yes votes and no votes given respectively as `MemberCount`). 

___


## delegatedStaking
 
### Delegated(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.delegatedStaking.Delegated.is`
- **summary**:    Funds delegated by a delegator. 
 
### MigratedDelegation(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.delegatedStaking.MigratedDelegation.is`
- **summary**:    Unclaimed delegation funds migrated to delegator. 
 
### Released(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.delegatedStaking.Released.is`
- **summary**:    Funds released to a delegator. 
 
### Slashed(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.delegatedStaking.Slashed.is`
- **summary**:    Funds slashed from a delegator. 

___


## democracy
 
### Blacklisted(`H256`)
- **interface**: `api.events.democracy.Blacklisted.is`
- **summary**:    A proposal_hash has been blacklisted permanently. 
 
### Cancelled(`u32`)
- **interface**: `api.events.democracy.Cancelled.is`
- **summary**:    A referendum has been cancelled. 
 
### Delegated(`AccountId32`, `AccountId32`)
- **interface**: `api.events.democracy.Delegated.is`
- **summary**:    An account has delegated their vote to another account. 
 
### ExternalTabled()
- **interface**: `api.events.democracy.ExternalTabled.is`
- **summary**:    An external proposal has been tabled. 
 
### MetadataCleared(`PalletDemocracyMetadataOwner`, `H256`)
- **interface**: `api.events.democracy.MetadataCleared.is`
- **summary**:    Metadata for a proposal or a referendum has been cleared. 
 
### MetadataSet(`PalletDemocracyMetadataOwner`, `H256`)
- **interface**: `api.events.democracy.MetadataSet.is`
- **summary**:    Metadata for a proposal or a referendum has been set. 
 
### MetadataTransferred(`PalletDemocracyMetadataOwner`, `PalletDemocracyMetadataOwner`, `H256`)
- **interface**: `api.events.democracy.MetadataTransferred.is`
- **summary**:    Metadata has been transferred to new owner. 
 
### NotPassed(`u32`)
- **interface**: `api.events.democracy.NotPassed.is`
- **summary**:    A proposal has been rejected by referendum. 
 
### Passed(`u32`)
- **interface**: `api.events.democracy.Passed.is`
- **summary**:    A proposal has been approved by referendum. 
 
### ProposalCanceled(`u32`)
- **interface**: `api.events.democracy.ProposalCanceled.is`
- **summary**:    A proposal got canceled. 
 
### Proposed(`u32`, `u128`)
- **interface**: `api.events.democracy.Proposed.is`
- **summary**:    A motion has been proposed by a public account. 
 
### Seconded(`AccountId32`, `u32`)
- **interface**: `api.events.democracy.Seconded.is`
- **summary**:    An account has seconded a proposal 
 
### Started(`u32`, `PalletDemocracyVoteThreshold`)
- **interface**: `api.events.democracy.Started.is`
- **summary**:    A referendum has begun. 
 
### Tabled(`u32`, `u128`)
- **interface**: `api.events.democracy.Tabled.is`
- **summary**:    A public proposal has been tabled for referendum vote. 
 
### Undelegated(`AccountId32`)
- **interface**: `api.events.democracy.Undelegated.is`
- **summary**:    An account has cancelled a previous delegation operation. 
 
### Vetoed(`AccountId32`, `H256`, `u32`)
- **interface**: `api.events.democracy.Vetoed.is`
- **summary**:    An external proposal has been vetoed. 
 
### Voted(`AccountId32`, `u32`, `PalletDemocracyVoteAccountVote`)
- **interface**: `api.events.democracy.Voted.is`
- **summary**:    An account has voted in a referendum 

___


## electionProviderMultiPhase
 
### ElectionFailed()
- **interface**: `api.events.electionProviderMultiPhase.ElectionFailed.is`
- **summary**:    An election failed. 

   Not much can be said about which computes failed in the process. 
 
### ElectionFinalized(`PalletElectionProviderMultiPhaseElectionCompute`, `SpNposElectionsElectionScore`)
- **interface**: `api.events.electionProviderMultiPhase.ElectionFinalized.is`
- **summary**:    The election has been finalized, with the given computation and score. 
 
### PhaseTransitioned(`PalletElectionProviderMultiPhasePhase`, `PalletElectionProviderMultiPhasePhase`, `u32`)
- **interface**: `api.events.electionProviderMultiPhase.PhaseTransitioned.is`
- **summary**:    There was a phase transition in a given round. 
 
### Rewarded(`AccountId32`, `u128`)
- **interface**: `api.events.electionProviderMultiPhase.Rewarded.is`
- **summary**:    An account has been rewarded for their signed submission being finalized. 
 
### Slashed(`AccountId32`, `u128`)
- **interface**: `api.events.electionProviderMultiPhase.Slashed.is`
- **summary**:    An account has been slashed for submitting an invalid signed submission. 
 
### SolutionStored(`PalletElectionProviderMultiPhaseElectionCompute`, `Option<AccountId32>`, `bool`)
- **interface**: `api.events.electionProviderMultiPhase.SolutionStored.is`
- **summary**:    A solution was stored with the given compute. 

   The `origin` indicates the origin of the solution. If `origin` is `Some(AccountId)`,  the stored solution was submitted in the signed phase by a miner with the `AccountId`.  Otherwise, the solution was stored either during the unsigned phase or by  `T::ForceOrigin`. The `bool` is `true` when a previous solution was ejected to make  room for this one. 

___


## elections
 
### CandidateSlashed(`AccountId32`, `u128`)
- **interface**: `api.events.elections.CandidateSlashed.is`
- **summary**:    A candidate was slashed by amount due to failing to obtain a seat as member or  runner-up. 

   Note that old members and runners-up are also candidates. 
 
### ElectionError()
- **interface**: `api.events.elections.ElectionError.is`
- **summary**:    Internal error happened while trying to perform election. 
 
### EmptyTerm()
- **interface**: `api.events.elections.EmptyTerm.is`
- **summary**:    No (or not enough) candidates existed for this round. This is different from  `NewTerm(\[\])`. See the description of `NewTerm`. 
 
### MemberKicked(`AccountId32`)
- **interface**: `api.events.elections.MemberKicked.is`
- **summary**:    A member has been removed. This should always be followed by either `NewTerm` or  `EmptyTerm`. 
 
### NewTerm(`Vec<(AccountId32,u128)>`)
- **interface**: `api.events.elections.NewTerm.is`
- **summary**:    A new term with new_members. This indicates that enough candidates existed to run  the election, not that enough have been elected. The inner value must be examined  for this purpose. A `NewTerm(\[\])` indicates that some candidates got their bond  slashed and none were elected, whilst `EmptyTerm` means that no candidates existed to  begin with. 
 
### Renounced(`AccountId32`)
- **interface**: `api.events.elections.Renounced.is`
- **summary**:    Someone has renounced their candidacy. 
 
### SeatHolderSlashed(`AccountId32`, `u128`)
- **interface**: `api.events.elections.SeatHolderSlashed.is`
- **summary**:    A seat holder was slashed by amount by being forcefully removed from the set. 

___


## fastUnstake
 
### BatchChecked(`Vec<u32>`)
- **interface**: `api.events.fastUnstake.BatchChecked.is`
- **summary**:    A batch was partially checked for the given eras, but the process did not finish. 
 
### BatchFinished(`u32`)
- **interface**: `api.events.fastUnstake.BatchFinished.is`
- **summary**:    A batch of a given size was terminated. 

   This is always follows by a number of `Unstaked` or `Slashed` events, marking the end  of the batch. A new batch will be created upon next block. 
 
### InternalError()
- **interface**: `api.events.fastUnstake.InternalError.is`
- **summary**:    An internal error happened. Operations will be paused now. 
 
### Slashed(`AccountId32`, `u128`)
- **interface**: `api.events.fastUnstake.Slashed.is`
- **summary**:    A staker was slashed for requesting fast-unstake whilst being exposed. 
 
### Unstaked(`AccountId32`, `Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.fastUnstake.Unstaked.is`
- **summary**:    A staker was unstaked. 

___


## glutton
 
### BlockLengthLimitSet(`u64`)
- **interface**: `api.events.glutton.BlockLengthLimitSet.is`
- **summary**:    The block length limit has been updated. 
 
### ComputationLimitSet(`u64`)
- **interface**: `api.events.glutton.ComputationLimitSet.is`
- **summary**:    The computation limit has been updated. 
 
### PalletInitialized(`bool`)
- **interface**: `api.events.glutton.PalletInitialized.is`
- **summary**:    The pallet has been (re)initialized. 
 
### StorageLimitSet(`u64`)
- **interface**: `api.events.glutton.StorageLimitSet.is`
- **summary**:    The storage limit has been updated. 

___


## grandpa
 
### NewAuthorities(`Vec<(SpConsensusGrandpaAppPublic,u64)>`)
- **interface**: `api.events.grandpa.NewAuthorities.is`
- **summary**:    New authority set has been applied. 
 
### Paused()
- **interface**: `api.events.grandpa.Paused.is`
- **summary**:    Current authority set has been paused. 
 
### Resumed()
- **interface**: `api.events.grandpa.Resumed.is`
- **summary**:    Current authority set has been resumed. 

___


## identity
 
### AuthorityAdded(`AccountId32`)
- **interface**: `api.events.identity.AuthorityAdded.is`
- **summary**:    A username authority was added. 
 
### AuthorityRemoved(`AccountId32`)
- **interface**: `api.events.identity.AuthorityRemoved.is`
- **summary**:    A username authority was removed. 
 
### DanglingUsernameRemoved(`AccountId32`, `Bytes`)
- **interface**: `api.events.identity.DanglingUsernameRemoved.is`
- **summary**:    A dangling username (as in, a username corresponding to an account that has removed its  identity) has been removed. 
 
### IdentityCleared(`AccountId32`, `u128`)
- **interface**: `api.events.identity.IdentityCleared.is`
- **summary**:    A name was cleared, and the given balance returned. 
 
### IdentityKilled(`AccountId32`, `u128`)
- **interface**: `api.events.identity.IdentityKilled.is`
- **summary**:    A name was removed and the given balance slashed. 
 
### IdentitySet(`AccountId32`)
- **interface**: `api.events.identity.IdentitySet.is`
- **summary**:    A name was set or reset (which will remove all judgements). 
 
### JudgementGiven(`AccountId32`, `u32`)
- **interface**: `api.events.identity.JudgementGiven.is`
- **summary**:    A judgement was given by a registrar. 
 
### JudgementRequested(`AccountId32`, `u32`)
- **interface**: `api.events.identity.JudgementRequested.is`
- **summary**:    A judgement was asked from a registrar. 
 
### JudgementUnrequested(`AccountId32`, `u32`)
- **interface**: `api.events.identity.JudgementUnrequested.is`
- **summary**:    A judgement request was retracted. 
 
### PreapprovalExpired(`AccountId32`)
- **interface**: `api.events.identity.PreapprovalExpired.is`
- **summary**:    A queued username passed its expiration without being claimed and was removed. 
 
### PrimaryUsernameSet(`AccountId32`, `Bytes`)
- **interface**: `api.events.identity.PrimaryUsernameSet.is`
- **summary**:    A username was set as a primary and can be looked up from `who`. 
 
### RegistrarAdded(`u32`)
- **interface**: `api.events.identity.RegistrarAdded.is`
- **summary**:    A registrar was added. 
 
### SubIdentitiesSet(`AccountId32`, `u32`, `u128`)
- **interface**: `api.events.identity.SubIdentitiesSet.is`
- **summary**:    An account's sub-identities were set (in bulk). 
 
### SubIdentityAdded(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.identity.SubIdentityAdded.is`
- **summary**:    A sub-identity was added to an identity and the deposit paid. 
 
### SubIdentityRemoved(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.identity.SubIdentityRemoved.is`
- **summary**:    A sub-identity was removed from an identity and the deposit freed. 
 
### SubIdentityRenamed(`AccountId32`, `AccountId32`)
- **interface**: `api.events.identity.SubIdentityRenamed.is`
- **summary**:    A given sub-account's associated name was changed by its super-identity. 
 
### SubIdentityRevoked(`AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.identity.SubIdentityRevoked.is`
- **summary**:    A sub-identity was cleared, and the given deposit repatriated from the  main identity account to the sub-identity account. 
 
### UsernameKilled(`Bytes`)
- **interface**: `api.events.identity.UsernameKilled.is`
- **summary**:    A username has been killed. 
 
### UsernameQueued(`AccountId32`, `Bytes`, `u32`)
- **interface**: `api.events.identity.UsernameQueued.is`
- **summary**:    A username was queued, but `who` must accept it prior to `expiration`. 
 
### UsernameRemoved(`Bytes`)
- **interface**: `api.events.identity.UsernameRemoved.is`
- **summary**:    A username has been removed. 
 
### UsernameSet(`AccountId32`, `Bytes`)
- **interface**: `api.events.identity.UsernameSet.is`
- **summary**:    A username was set for `who`. 
 
### UsernameUnbound(`Bytes`)
- **interface**: `api.events.identity.UsernameUnbound.is`
- **summary**:    A username has been unbound. 

___


## imOnline
 
### AllGood()
- **interface**: `api.events.imOnline.AllGood.is`
- **summary**:    At the end of the session, no offence was committed. 
 
### HeartbeatReceived(`PalletImOnlineSr25519AppSr25519Public`)
- **interface**: `api.events.imOnline.HeartbeatReceived.is`
- **summary**:    A new heartbeat was received from `AuthorityId`. 
 
### SomeOffline(`Vec<(AccountId32,Null)>`)
- **interface**: `api.events.imOnline.SomeOffline.is`
- **summary**:    At the end of the session, at least one validator was found to be offline. 

___


## indices
 
### DepositPoked(`AccountId32`, `u32`, `u128`, `u128`)
- **interface**: `api.events.indices.DepositPoked.is`
- **summary**:    A deposit to reserve an index has been poked/reconsidered. 
 
### IndexAssigned(`AccountId32`, `u32`)
- **interface**: `api.events.indices.IndexAssigned.is`
- **summary**:    A account index was assigned. 
 
### IndexFreed(`u32`)
- **interface**: `api.events.indices.IndexFreed.is`
- **summary**:    A account index has been freed up (unassigned). 
 
### IndexFrozen(`u32`, `AccountId32`)
- **interface**: `api.events.indices.IndexFrozen.is`
- **summary**:    A account index has been frozen to its current account ID. 

___


## lottery
 
### CallsUpdated()
- **interface**: `api.events.lottery.CallsUpdated.is`
- **summary**:    A new set of calls have been set! 
 
### LotteryStarted()
- **interface**: `api.events.lottery.LotteryStarted.is`
- **summary**:    A lottery has been started! 
 
### TicketBought(`AccountId32`, `(u8,u8)`)
- **interface**: `api.events.lottery.TicketBought.is`
- **summary**:    A ticket has been bought! 
 
### Winner(`AccountId32`, `u128`)
- **interface**: `api.events.lottery.Winner.is`
- **summary**:    A winner has been chosen! 

___


## messageQueue
 
### OverweightEnqueued(`[u8;32]`, `u32`, `u32`, `u32`)
- **interface**: `api.events.messageQueue.OverweightEnqueued.is`
- **summary**:    Message placed in overweight queue. 
 
### PageReaped(`u32`, `u32`)
- **interface**: `api.events.messageQueue.PageReaped.is`
- **summary**:    This page was reaped. 
 
### Processed(`H256`, `u32`, `SpWeightsWeightV2Weight`, `bool`)
- **interface**: `api.events.messageQueue.Processed.is`
- **summary**:    Message is processed. 
 
### ProcessingFailed(`H256`, `u32`, `FrameSupportMessagesProcessMessageError`)
- **interface**: `api.events.messageQueue.ProcessingFailed.is`
- **summary**:    Message discarded due to an error in the `MessageProcessor` (usually a format error). 

___


## metaTx
 
### Dispatched(`Result<FrameSupportDispatchPostDispatchInfo, SpRuntimeDispatchErrorWithPostInfo>`)
- **interface**: `api.events.metaTx.Dispatched.is`
- **summary**:    A meta transaction has been dispatched. 

   Contains the dispatch result of the meta transaction along with post-dispatch  information. 

___


## multiBlockMigrations
 
### HistoricCleared(`Option<Bytes>`)
- **interface**: `api.events.multiBlockMigrations.HistoricCleared.is`
- **summary**:    The set of historical migrations has been cleared. 
 
### MigrationAdvanced(`u32`, `u32`)
- **interface**: `api.events.multiBlockMigrations.MigrationAdvanced.is`
- **summary**:    A migration progressed. 
 
### MigrationCompleted(`u32`, `u32`)
- **interface**: `api.events.multiBlockMigrations.MigrationCompleted.is`
- **summary**:    A Migration completed. 
 
### MigrationFailed(`u32`, `u32`)
- **interface**: `api.events.multiBlockMigrations.MigrationFailed.is`
- **summary**:    A Migration failed. 

   This implies that the whole upgrade failed and governance intervention is required. 
 
### MigrationSkipped(`u32`)
- **interface**: `api.events.multiBlockMigrations.MigrationSkipped.is`
- **summary**:    A migration was skipped since it was already executed in the past. 
 
### UpgradeCompleted()
- **interface**: `api.events.multiBlockMigrations.UpgradeCompleted.is`
- **summary**:    The current runtime upgrade completed. 

   This implies that all of its migrations completed successfully as well. 
 
### UpgradeFailed()
- **interface**: `api.events.multiBlockMigrations.UpgradeFailed.is`
- **summary**:    Runtime upgrade failed. 

   This is very bad and will require governance intervention. 
 
### UpgradeStarted(`u32`)
- **interface**: `api.events.multiBlockMigrations.UpgradeStarted.is`
- **summary**:    A Runtime upgrade started. 

   Its end is indicated by `UpgradeCompleted` or `UpgradeFailed`. 

___


## multisig
 
### DepositPoked(`AccountId32`, `[u8;32]`, `u128`, `u128`)
- **interface**: `api.events.multisig.DepositPoked.is`
- **summary**:    The deposit for a multisig operation has been updated/poked. 
 
### MultisigApproval(`AccountId32`, `PalletMultisigTimepoint`, `AccountId32`, `[u8;32]`)
- **interface**: `api.events.multisig.MultisigApproval.is`
- **summary**:    A multisig operation has been approved by someone. 
 
### MultisigCancelled(`AccountId32`, `PalletMultisigTimepoint`, `AccountId32`, `[u8;32]`)
- **interface**: `api.events.multisig.MultisigCancelled.is`
- **summary**:    A multisig operation has been cancelled. 
 
### MultisigExecuted(`AccountId32`, `PalletMultisigTimepoint`, `AccountId32`, `[u8;32]`, `Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.multisig.MultisigExecuted.is`
- **summary**:    A multisig operation has been executed. 
 
### NewMultisig(`AccountId32`, `AccountId32`, `[u8;32]`)
- **interface**: `api.events.multisig.NewMultisig.is`
- **summary**:    A new multisig operation has begun. 

___


## nftFractionalization
 
### NftFractionalized(`u32`, `u32`, `u128`, `u32`, `AccountId32`)
- **interface**: `api.events.nftFractionalization.NftFractionalized.is`
- **summary**:    An NFT was successfully fractionalized. 
 
### NftUnified(`u32`, `u32`, `u32`, `AccountId32`)
- **interface**: `api.events.nftFractionalization.NftUnified.is`
- **summary**:    An NFT was successfully returned back. 

___


## nfts
 
### AllApprovalsCancelled(`u32`, `u32`, `AccountId32`)
- **interface**: `api.events.nfts.AllApprovalsCancelled.is`
- **summary**:    All approvals of an item got cancelled. 
 
### ApprovalCancelled(`u32`, `u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.nfts.ApprovalCancelled.is`
- **summary**:    An approval for a `delegate` account to transfer the `item` of an item  `collection` was cancelled by its `owner`. 
 
### AttributeCleared(`u32`, `Option<u32>`, `Bytes`, `PalletNftsAttributeNamespace`)
- **interface**: `api.events.nfts.AttributeCleared.is`
- **summary**:    Attribute metadata has been cleared for a `collection` or `item`. 
 
### AttributeSet(`u32`, `Option<u32>`, `Bytes`, `Bytes`, `PalletNftsAttributeNamespace`)
- **interface**: `api.events.nfts.AttributeSet.is`
- **summary**:    New attribute metadata has been set for a `collection` or `item`. 
 
### Burned(`u32`, `u32`, `AccountId32`)
- **interface**: `api.events.nfts.Burned.is`
- **summary**:    An `item` was destroyed. 
 
### CollectionConfigChanged(`u32`)
- **interface**: `api.events.nfts.CollectionConfigChanged.is`
- **summary**:    A `collection` has had its config changed by the `Force` origin. 
 
### CollectionLocked(`u32`)
- **interface**: `api.events.nfts.CollectionLocked.is`
- **summary**:    Some `collection` was locked. 
 
### CollectionMaxSupplySet(`u32`, `u32`)
- **interface**: `api.events.nfts.CollectionMaxSupplySet.is`
- **summary**:    Max supply has been set for a collection. 
 
### CollectionMetadataCleared(`u32`)
- **interface**: `api.events.nfts.CollectionMetadataCleared.is`
- **summary**:    Metadata has been cleared for a `collection`. 
 
### CollectionMetadataSet(`u32`, `Bytes`)
- **interface**: `api.events.nfts.CollectionMetadataSet.is`
- **summary**:    New metadata has been set for a `collection`. 
 
### CollectionMintSettingsUpdated(`u32`)
- **interface**: `api.events.nfts.CollectionMintSettingsUpdated.is`
- **summary**:    Mint settings for a collection had changed. 
 
### Created(`u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.nfts.Created.is`
- **summary**:    A `collection` was created. 
 
### Destroyed(`u32`)
- **interface**: `api.events.nfts.Destroyed.is`
- **summary**:    A `collection` was destroyed. 
 
### ForceCreated(`u32`, `AccountId32`)
- **interface**: `api.events.nfts.ForceCreated.is`
- **summary**:    A `collection` was force-created. 
 
### Issued(`u32`, `u32`, `AccountId32`)
- **interface**: `api.events.nfts.Issued.is`
- **summary**:    An `item` was issued. 
 
### ItemAttributesApprovalAdded(`u32`, `u32`, `AccountId32`)
- **interface**: `api.events.nfts.ItemAttributesApprovalAdded.is`
- **summary**:    A new approval to modify item attributes was added. 
 
### ItemAttributesApprovalRemoved(`u32`, `u32`, `AccountId32`)
- **interface**: `api.events.nfts.ItemAttributesApprovalRemoved.is`
- **summary**:    A new approval to modify item attributes was removed. 
 
### ItemBought(`u32`, `u32`, `u128`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.nfts.ItemBought.is`
- **summary**:    An item was bought. 
 
### ItemMetadataCleared(`u32`, `u32`)
- **interface**: `api.events.nfts.ItemMetadataCleared.is`
- **summary**:    Metadata has been cleared for an item. 
 
### ItemMetadataSet(`u32`, `u32`, `Bytes`)
- **interface**: `api.events.nfts.ItemMetadataSet.is`
- **summary**:    New metadata has been set for an item. 
 
### ItemPriceRemoved(`u32`, `u32`)
- **interface**: `api.events.nfts.ItemPriceRemoved.is`
- **summary**:    The price for the item was removed. 
 
### ItemPriceSet(`u32`, `u32`, `u128`, `Option<AccountId32>`)
- **interface**: `api.events.nfts.ItemPriceSet.is`
- **summary**:    The price was set for the item. 
 
### ItemPropertiesLocked(`u32`, `u32`, `bool`, `bool`)
- **interface**: `api.events.nfts.ItemPropertiesLocked.is`
- **summary**:    `item` metadata or attributes were locked. 
 
### ItemTransferLocked(`u32`, `u32`)
- **interface**: `api.events.nfts.ItemTransferLocked.is`
- **summary**:    An `item` became non-transferable. 
 
### ItemTransferUnlocked(`u32`, `u32`)
- **interface**: `api.events.nfts.ItemTransferUnlocked.is`
- **summary**:    An `item` became transferable. 
 
### NextCollectionIdIncremented(`Option<u32>`)
- **interface**: `api.events.nfts.NextCollectionIdIncremented.is`
- **summary**:    Event gets emitted when the `NextCollectionId` gets incremented. 
 
### OwnerChanged(`u32`, `AccountId32`)
- **interface**: `api.events.nfts.OwnerChanged.is`
- **summary**:    The owner changed. 
 
### OwnershipAcceptanceChanged(`AccountId32`, `Option<u32>`)
- **interface**: `api.events.nfts.OwnershipAcceptanceChanged.is`
- **summary**:    Ownership acceptance has changed for an account. 
 
### PalletAttributeSet(`u32`, `Option<u32>`, `PalletNftsPalletAttributes`, `Bytes`)
- **interface**: `api.events.nfts.PalletAttributeSet.is`
- **summary**:    A new attribute in the `Pallet` namespace was set for the `collection` or an `item`  within that `collection`. 
 
### PreSignedAttributesSet(`u32`, `u32`, `PalletNftsAttributeNamespace`)
- **interface**: `api.events.nfts.PreSignedAttributesSet.is`
- **summary**:    New attributes have been set for an `item` of the `collection`. 
 
### Redeposited(`u32`, `Vec<u32>`)
- **interface**: `api.events.nfts.Redeposited.is`
- **summary**:    The deposit for a set of `item`s within a `collection` has been updated. 
 
### SwapCancelled(`u32`, `u32`, `u32`, `Option<u32>`, `Option<PalletNftsPriceWithDirection>`, `u32`)
- **interface**: `api.events.nfts.SwapCancelled.is`
- **summary**:    The swap was cancelled. 
 
### SwapClaimed(`u32`, `u32`, `AccountId32`, `u32`, `u32`, `AccountId32`, `Option<PalletNftsPriceWithDirection>`, `u32`)
- **interface**: `api.events.nfts.SwapClaimed.is`
- **summary**:    The swap has been claimed. 
 
### SwapCreated(`u32`, `u32`, `u32`, `Option<u32>`, `Option<PalletNftsPriceWithDirection>`, `u32`)
- **interface**: `api.events.nfts.SwapCreated.is`
- **summary**:    An `item` swap intent was created. 
 
### TeamChanged(`u32`, `Option<AccountId32>`, `Option<AccountId32>`, `Option<AccountId32>`)
- **interface**: `api.events.nfts.TeamChanged.is`
- **summary**:    The management team changed. 
 
### TipSent(`u32`, `u32`, `AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.nfts.TipSent.is`
- **summary**:    A tip was sent. 
 
### TransferApproved(`u32`, `u32`, `AccountId32`, `AccountId32`, `Option<u32>`)
- **interface**: `api.events.nfts.TransferApproved.is`
- **summary**:    An `item` of a `collection` has been approved by the `owner` for transfer by  a `delegate`. 
 
### Transferred(`u32`, `u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.nfts.Transferred.is`
- **summary**:    An `item` was transferred. 

___


## nis
 
### BidDropped(`AccountId32`, `u128`, `u32`)
- **interface**: `api.events.nis.BidDropped.is`
- **summary**:    A bid was dropped from a queue because of another, more substantial, bid was present. 
 
### BidPlaced(`AccountId32`, `u128`, `u32`)
- **interface**: `api.events.nis.BidPlaced.is`
- **summary**:    A bid was successfully placed. 
 
### BidRetracted(`AccountId32`, `u128`, `u32`)
- **interface**: `api.events.nis.BidRetracted.is`
- **summary**:    A bid was successfully removed (before being accepted). 
 
### Funded(`u128`)
- **interface**: `api.events.nis.Funded.is`
- **summary**:    An automatic funding of the deficit was made. 
 
### Issued(`u32`, `u32`, `AccountId32`, `Perquintill`, `u128`)
- **interface**: `api.events.nis.Issued.is`
- **summary**:    A bid was accepted. The balance may not be released until expiry. 
 
### Thawed(`u32`, `AccountId32`, `Perquintill`, `u128`, `bool`)
- **interface**: `api.events.nis.Thawed.is`
- **summary**:    An receipt has been (at least partially) thawed. 
 
### Transferred(`AccountId32`, `AccountId32`, `u32`)
- **interface**: `api.events.nis.Transferred.is`
- **summary**:    A receipt was transferred. 

___


## nominationPools
 
### Bonded(`AccountId32`, `u32`, `u128`, `bool`)
- **interface**: `api.events.nominationPools.Bonded.is`
- **summary**:    A member has became bonded in a pool. 
 
### Created(`AccountId32`, `u32`)
- **interface**: `api.events.nominationPools.Created.is`
- **summary**:    A pool has been created. 
 
### Destroyed(`u32`)
- **interface**: `api.events.nominationPools.Destroyed.is`
- **summary**:    A pool has been destroyed. 
 
### GlobalParamsUpdated(`u128`, `u128`, `Option<u32>`, `Option<u32>`, `Option<u32>`, `Option<Perbill>`)
- **interface**: `api.events.nominationPools.GlobalParamsUpdated.is`
- **summary**:    Global parameters regulating nomination pools have been updated. 
 
### MemberClaimPermissionUpdated(`AccountId32`, `PalletNominationPoolsClaimPermission`)
- **interface**: `api.events.nominationPools.MemberClaimPermissionUpdated.is`
- **summary**:    A pool member's claim permission has been updated. 
 
### MemberRemoved(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.nominationPools.MemberRemoved.is`
- **summary**:    A member has been removed from a pool. 

   The removal can be voluntary (withdrawn all unbonded funds) or involuntary (kicked).  Any funds that are still delegated (i.e. dangling delegation) are released and are  represented by `released_balance`. 
 
### MetadataUpdated(`u32`, `AccountId32`)
- **interface**: `api.events.nominationPools.MetadataUpdated.is`
- **summary**:    A pool's metadata was updated. 
 
### MinBalanceDeficitAdjusted(`u32`, `u128`)
- **interface**: `api.events.nominationPools.MinBalanceDeficitAdjusted.is`
- **summary**:    Topped up deficit in frozen ED of the reward pool. 
 
### MinBalanceExcessAdjusted(`u32`, `u128`)
- **interface**: `api.events.nominationPools.MinBalanceExcessAdjusted.is`
- **summary**:    Claimed excess frozen ED of af the reward pool. 
 
### PaidOut(`AccountId32`, `u32`, `u128`)
- **interface**: `api.events.nominationPools.PaidOut.is`
- **summary**:    A payout has been made to a member. 
 
### PoolCommissionChangeRateUpdated(`u32`, `PalletNominationPoolsCommissionChangeRate`)
- **interface**: `api.events.nominationPools.PoolCommissionChangeRateUpdated.is`
- **summary**:    A pool's commission `change_rate` has been changed. 
 
### PoolCommissionClaimed(`u32`, `u128`)
- **interface**: `api.events.nominationPools.PoolCommissionClaimed.is`
- **summary**:    Pool commission has been claimed. 
 
### PoolCommissionClaimPermissionUpdated(`u32`, `Option<PalletNominationPoolsCommissionClaimPermission>`)
- **interface**: `api.events.nominationPools.PoolCommissionClaimPermissionUpdated.is`
- **summary**:    Pool commission claim permission has been updated. 
 
### PoolCommissionUpdated(`u32`, `Option<(Perbill,AccountId32)>`)
- **interface**: `api.events.nominationPools.PoolCommissionUpdated.is`
- **summary**:    A pool's commission setting has been changed. 
 
### PoolMaxCommissionUpdated(`u32`, `Perbill`)
- **interface**: `api.events.nominationPools.PoolMaxCommissionUpdated.is`
- **summary**:    A pool's maximum commission setting has been changed. 
 
### PoolNominationMade(`u32`, `AccountId32`)
- **interface**: `api.events.nominationPools.PoolNominationMade.is`
- **summary**:    A pool's nominating account (or the pool's root account) has nominated a validator set  on behalf of the pool. 
 
### PoolNominatorChilled(`u32`, `AccountId32`)
- **interface**: `api.events.nominationPools.PoolNominatorChilled.is`
- **summary**:    The pool is chilled i.e. no longer nominating. 
 
### PoolSlashed(`u32`, `u128`)
- **interface**: `api.events.nominationPools.PoolSlashed.is`
- **summary**:    The active balance of pool `pool_id` has been slashed to `balance`. 
 
### RolesUpdated(`Option<AccountId32>`, `Option<AccountId32>`, `Option<AccountId32>`)
- **interface**: `api.events.nominationPools.RolesUpdated.is`
- **summary**:    The roles of a pool have been updated to the given new roles. Note that the depositor  can never change. 
 
### StateChanged(`u32`, `PalletNominationPoolsPoolState`)
- **interface**: `api.events.nominationPools.StateChanged.is`
- **summary**:    The state of a pool has changed 
 
### Unbonded(`AccountId32`, `u32`, `u128`, `u128`, `u32`)
- **interface**: `api.events.nominationPools.Unbonded.is`
- **summary**:    A member has unbonded from their pool. 

   - `balance` is the corresponding balance of the number of points that has been  requested to be unbonded (the argument of the `unbond` transaction) from the bonded  pool. 

  - `points` is the number of points that are issued as a result of `balance` being dissolved into the corresponding unbonding pool. 

  - `era` is the era in which the balance will be unbonded. In the absence of slashing, these values will match. In the presence of slashing, the  number of points that are issued in the unbonding pool will be less than the amount  requested to be unbonded. 
 
### UnbondingPoolSlashed(`u32`, `u32`, `u128`)
- **interface**: `api.events.nominationPools.UnbondingPoolSlashed.is`
- **summary**:    The unbond pool at `era` of pool `pool_id` has been slashed to `balance`. 
 
### Withdrawn(`AccountId32`, `u32`, `u128`, `u128`)
- **interface**: `api.events.nominationPools.Withdrawn.is`
- **summary**:    A member has withdrawn from their pool. 

   The given number of `points` have been dissolved in return of `balance`. 

   Similar to `Unbonded` event, in the absence of slashing, the ratio of point to balance  will be 1. 

___


## offences
 
### Offence(`[u8;16]`, `Bytes`)
- **interface**: `api.events.offences.Offence.is`
- **summary**:    There is an offence reported of the given `kind` happened at the `session_index` and  (kind-specific) time slot. This event is not deposited for duplicate slashes.  \[kind, timeslot\]. 

___


## parameters
 
### Updated(`KitchensinkRuntimeRuntimeParametersKey`, `Option<KitchensinkRuntimeRuntimeParametersValue>`, `Option<KitchensinkRuntimeRuntimeParametersValue>`)
- **interface**: `api.events.parameters.Updated.is`
- **summary**:    A Parameter was set. 

   Is also emitted when the value was not changed. 

___


## poolAssets
 
### AccountsDestroyed(`u32`, `u32`, `u32`)
- **interface**: `api.events.poolAssets.AccountsDestroyed.is`
- **summary**:    Accounts were destroyed for given asset. 
 
### ApprovalCancelled(`u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.poolAssets.ApprovalCancelled.is`
- **summary**:    An approval for account `delegate` was cancelled by `owner`. 
 
### ApprovalsDestroyed(`u32`, `u32`, `u32`)
- **interface**: `api.events.poolAssets.ApprovalsDestroyed.is`
- **summary**:    Approvals were destroyed for given asset. 
 
### ApprovedTransfer(`u32`, `AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.poolAssets.ApprovedTransfer.is`
- **summary**:    (Additional) funds have been approved for transfer to a destination account. 
 
### AssetFrozen(`u32`)
- **interface**: `api.events.poolAssets.AssetFrozen.is`
- **summary**:    Some asset `asset_id` was frozen. 
 
### AssetMinBalanceChanged(`u32`, `u128`)
- **interface**: `api.events.poolAssets.AssetMinBalanceChanged.is`
- **summary**:    The min_balance of an asset has been updated by the asset owner. 
 
### AssetStatusChanged(`u32`)
- **interface**: `api.events.poolAssets.AssetStatusChanged.is`
- **summary**:    An asset has had its attributes changed by the `Force` origin. 
 
### AssetThawed(`u32`)
- **interface**: `api.events.poolAssets.AssetThawed.is`
- **summary**:    Some asset `asset_id` was thawed. 
 
### Blocked(`u32`, `AccountId32`)
- **interface**: `api.events.poolAssets.Blocked.is`
- **summary**:    Some account `who` was blocked. 
 
### Burned(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.poolAssets.Burned.is`
- **summary**:    Some assets were destroyed. 
 
### Created(`u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.poolAssets.Created.is`
- **summary**:    Some asset class was created. 
 
### Deposited(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.poolAssets.Deposited.is`
- **summary**:    Some assets were deposited (e.g. for transaction fees). 
 
### Destroyed(`u32`)
- **interface**: `api.events.poolAssets.Destroyed.is`
- **summary**:    An asset class was destroyed. 
 
### DestructionStarted(`u32`)
- **interface**: `api.events.poolAssets.DestructionStarted.is`
- **summary**:    An asset class is in the process of being destroyed. 
 
### ForceCreated(`u32`, `AccountId32`)
- **interface**: `api.events.poolAssets.ForceCreated.is`
- **summary**:    Some asset class was force-created. 
 
### Frozen(`u32`, `AccountId32`)
- **interface**: `api.events.poolAssets.Frozen.is`
- **summary**:    Some account `who` was frozen. 
 
### Issued(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.poolAssets.Issued.is`
- **summary**:    Some assets were issued. 
 
### MetadataCleared(`u32`)
- **interface**: `api.events.poolAssets.MetadataCleared.is`
- **summary**:    Metadata has been cleared for an asset. 
 
### MetadataSet(`u32`, `Bytes`, `Bytes`, `u8`, `bool`)
- **interface**: `api.events.poolAssets.MetadataSet.is`
- **summary**:    New metadata has been set for an asset. 
 
### OwnerChanged(`u32`, `AccountId32`)
- **interface**: `api.events.poolAssets.OwnerChanged.is`
- **summary**:    The owner changed. 
 
### TeamChanged(`u32`, `AccountId32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.poolAssets.TeamChanged.is`
- **summary**:    The management team changed. 
 
### Thawed(`u32`, `AccountId32`)
- **interface**: `api.events.poolAssets.Thawed.is`
- **summary**:    Some account `who` was thawed. 
 
### Touched(`u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.poolAssets.Touched.is`
- **summary**:    Some account `who` was created with a deposit from `depositor`. 
 
### Transferred(`u32`, `AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.poolAssets.Transferred.is`
- **summary**:    Some assets were transferred. 
 
### TransferredApproved(`u32`, `AccountId32`, `AccountId32`, `AccountId32`, `u128`)
- **interface**: `api.events.poolAssets.TransferredApproved.is`
- **summary**:    An `amount` was transferred in its entirety from `owner` to `destination` by  the approved `delegate`. 
 
### Withdrawn(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.poolAssets.Withdrawn.is`
- **summary**:    Some assets were withdrawn from the account (e.g. for transaction fees). 

___


## pov
 
### TestEvent()
- **interface**: `api.events.pov.TestEvent.is`

___


## preimage
 
### Cleared(`H256`)
- **interface**: `api.events.preimage.Cleared.is`
- **summary**:    A preimage has ben cleared. 
 
### Noted(`H256`)
- **interface**: `api.events.preimage.Noted.is`
- **summary**:    A preimage has been noted. 
 
### Requested(`H256`)
- **interface**: `api.events.preimage.Requested.is`
- **summary**:    A preimage has been requested. 

___


## proxy
 
### Announced(`AccountId32`, `AccountId32`, `H256`)
- **interface**: `api.events.proxy.Announced.is`
- **summary**:    An announcement was placed to make a call in the future. 
 
### DepositPoked(`AccountId32`, `PalletProxyDepositKind`, `u128`, `u128`)
- **interface**: `api.events.proxy.DepositPoked.is`
- **summary**:    A deposit stored for proxies or announcements was poked / updated. 
 
### ProxyAdded(`AccountId32`, `AccountId32`, `KitchensinkRuntimeProxyType`, `u32`)
- **interface**: `api.events.proxy.ProxyAdded.is`
- **summary**:    A proxy was added. 
 
### ProxyExecuted(`Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.proxy.ProxyExecuted.is`
- **summary**:    A proxy was executed correctly, with the given. 
 
### ProxyRemoved(`AccountId32`, `AccountId32`, `KitchensinkRuntimeProxyType`, `u32`)
- **interface**: `api.events.proxy.ProxyRemoved.is`
- **summary**:    A proxy was removed. 
 
### PureCreated(`AccountId32`, `AccountId32`, `KitchensinkRuntimeProxyType`, `u16`)
- **interface**: `api.events.proxy.PureCreated.is`
- **summary**:    A pure account has been created by new proxy with given  disambiguation index and proxy type. 

___


## rankedCollective
 
### MemberAdded(`AccountId32`)
- **interface**: `api.events.rankedCollective.MemberAdded.is`
- **summary**:    A member `who` has been added. 
 
### MemberExchanged(`AccountId32`, `AccountId32`)
- **interface**: `api.events.rankedCollective.MemberExchanged.is`
- **summary**:    The member `who` had their `AccountId` changed to `new_who`. 
 
### MemberRemoved(`AccountId32`, `u16`)
- **interface**: `api.events.rankedCollective.MemberRemoved.is`
- **summary**:    The member `who` of given `rank` has been removed from the collective. 
 
### RankChanged(`AccountId32`, `u16`)
- **interface**: `api.events.rankedCollective.RankChanged.is`
- **summary**:    The member `who`se rank has been changed to the given `rank`. 
 
### Voted(`AccountId32`, `u32`, `PalletRankedCollectiveVoteRecord`, `PalletRankedCollectiveTally`)
- **interface**: `api.events.rankedCollective.Voted.is`
- **summary**:    The member `who` has voted for the `poll` with the given `vote` leading to an updated  `tally`. 

___


## rankedPolls
 
### Approved(`u32`)
- **interface**: `api.events.rankedPolls.Approved.is`
- **summary**:    A referendum has been approved and its proposal has been scheduled. 
 
### Cancelled(`u32`, `PalletRankedCollectiveTally`)
- **interface**: `api.events.rankedPolls.Cancelled.is`
- **summary**:    A referendum has been cancelled. 
 
### ConfirmAborted(`u32`)
- **interface**: `api.events.rankedPolls.ConfirmAborted.is`
 
### Confirmed(`u32`, `PalletRankedCollectiveTally`)
- **interface**: `api.events.rankedPolls.Confirmed.is`
- **summary**:    A referendum has ended its confirmation phase and is ready for approval. 
 
### ConfirmStarted(`u32`)
- **interface**: `api.events.rankedPolls.ConfirmStarted.is`
 
### DecisionDepositPlaced(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.rankedPolls.DecisionDepositPlaced.is`
- **summary**:    The decision deposit has been placed. 
 
### DecisionDepositRefunded(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.rankedPolls.DecisionDepositRefunded.is`
- **summary**:    The decision deposit has been refunded. 
 
### DecisionStarted(`u32`, `u16`, `FrameSupportPreimagesBounded`, `PalletRankedCollectiveTally`)
- **interface**: `api.events.rankedPolls.DecisionStarted.is`
- **summary**:    A referendum has moved into the deciding phase. 
 
### DepositSlashed(`AccountId32`, `u128`)
- **interface**: `api.events.rankedPolls.DepositSlashed.is`
- **summary**:    A deposit has been slashed. 
 
### Killed(`u32`, `PalletRankedCollectiveTally`)
- **interface**: `api.events.rankedPolls.Killed.is`
- **summary**:    A referendum has been killed. 
 
### MetadataCleared(`u32`, `H256`)
- **interface**: `api.events.rankedPolls.MetadataCleared.is`
- **summary**:    Metadata for a referendum has been cleared. 
 
### MetadataSet(`u32`, `H256`)
- **interface**: `api.events.rankedPolls.MetadataSet.is`
- **summary**:    Metadata for a referendum has been set. 
 
### Rejected(`u32`, `PalletRankedCollectiveTally`)
- **interface**: `api.events.rankedPolls.Rejected.is`
- **summary**:    A proposal has been rejected by referendum. 
 
### SubmissionDepositRefunded(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.rankedPolls.SubmissionDepositRefunded.is`
- **summary**:    The submission deposit has been refunded. 
 
### Submitted(`u32`, `u16`, `FrameSupportPreimagesBounded`)
- **interface**: `api.events.rankedPolls.Submitted.is`
- **summary**:    A referendum has been submitted. 
 
### TimedOut(`u32`, `PalletRankedCollectiveTally`)
- **interface**: `api.events.rankedPolls.TimedOut.is`
- **summary**:    A referendum has been timed out without being decided. 

___


## recovery
 
### AccountRecovered(`AccountId32`, `AccountId32`)
- **interface**: `api.events.recovery.AccountRecovered.is`
- **summary**:    Lost account has been successfully recovered by rescuer account. 
 
### RecoveryClosed(`AccountId32`, `AccountId32`)
- **interface**: `api.events.recovery.RecoveryClosed.is`
- **summary**:    A recovery process for lost account by rescuer account has been closed. 
 
### RecoveryCreated(`AccountId32`)
- **interface**: `api.events.recovery.RecoveryCreated.is`
- **summary**:    A recovery process has been set up for an account. 
 
### RecoveryInitiated(`AccountId32`, `AccountId32`)
- **interface**: `api.events.recovery.RecoveryInitiated.is`
- **summary**:    A recovery process has been initiated for lost account by rescuer account. 
 
### RecoveryRemoved(`AccountId32`)
- **interface**: `api.events.recovery.RecoveryRemoved.is`
- **summary**:    A recovery process has been removed for an account. 
 
### RecoveryVouched(`AccountId32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.recovery.RecoveryVouched.is`
- **summary**:    A recovery process for lost account by rescuer account has been vouched for by sender. 

___


## referenda
 
### Approved(`u32`)
- **interface**: `api.events.referenda.Approved.is`
- **summary**:    A referendum has been approved and its proposal has been scheduled. 
 
### Cancelled(`u32`, `PalletConvictionVotingTally`)
- **interface**: `api.events.referenda.Cancelled.is`
- **summary**:    A referendum has been cancelled. 
 
### ConfirmAborted(`u32`)
- **interface**: `api.events.referenda.ConfirmAborted.is`
 
### Confirmed(`u32`, `PalletConvictionVotingTally`)
- **interface**: `api.events.referenda.Confirmed.is`
- **summary**:    A referendum has ended its confirmation phase and is ready for approval. 
 
### ConfirmStarted(`u32`)
- **interface**: `api.events.referenda.ConfirmStarted.is`
 
### DecisionDepositPlaced(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.referenda.DecisionDepositPlaced.is`
- **summary**:    The decision deposit has been placed. 
 
### DecisionDepositRefunded(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.referenda.DecisionDepositRefunded.is`
- **summary**:    The decision deposit has been refunded. 
 
### DecisionStarted(`u32`, `u16`, `FrameSupportPreimagesBounded`, `PalletConvictionVotingTally`)
- **interface**: `api.events.referenda.DecisionStarted.is`
- **summary**:    A referendum has moved into the deciding phase. 
 
### DepositSlashed(`AccountId32`, `u128`)
- **interface**: `api.events.referenda.DepositSlashed.is`
- **summary**:    A deposit has been slashed. 
 
### Killed(`u32`, `PalletConvictionVotingTally`)
- **interface**: `api.events.referenda.Killed.is`
- **summary**:    A referendum has been killed. 
 
### MetadataCleared(`u32`, `H256`)
- **interface**: `api.events.referenda.MetadataCleared.is`
- **summary**:    Metadata for a referendum has been cleared. 
 
### MetadataSet(`u32`, `H256`)
- **interface**: `api.events.referenda.MetadataSet.is`
- **summary**:    Metadata for a referendum has been set. 
 
### Rejected(`u32`, `PalletConvictionVotingTally`)
- **interface**: `api.events.referenda.Rejected.is`
- **summary**:    A proposal has been rejected by referendum. 
 
### SubmissionDepositRefunded(`u32`, `AccountId32`, `u128`)
- **interface**: `api.events.referenda.SubmissionDepositRefunded.is`
- **summary**:    The submission deposit has been refunded. 
 
### Submitted(`u32`, `u16`, `FrameSupportPreimagesBounded`)
- **interface**: `api.events.referenda.Submitted.is`
- **summary**:    A referendum has been submitted. 
 
### TimedOut(`u32`, `PalletConvictionVotingTally`)
- **interface**: `api.events.referenda.TimedOut.is`
- **summary**:    A referendum has been timed out without being decided. 

___


## remark
 
### Stored(`AccountId32`, `H256`)
- **interface**: `api.events.remark.Stored.is`
- **summary**:    Stored data off chain. 

___


## revive
 
### ContractEmitted(`H160`, `Bytes`, `Vec<H256>`)
- **interface**: `api.events.revive.ContractEmitted.is`
- **summary**:    A custom event emitted by the contract. 

___


## rootTesting
 
### DefensiveTestCall()
- **interface**: `api.events.rootTesting.DefensiveTestCall.is`
- **summary**:    Event dispatched when the trigger_defensive extrinsic is called. 

___


## safeMode
 
### CannotDeposit()
- **interface**: `api.events.safeMode.CannotDeposit.is`
- **summary**:    Could not hold funds for entering or extending the safe-mode. 

   This error comes from the underlying `Currency`. 
 
### CannotRelease()
- **interface**: `api.events.safeMode.CannotRelease.is`
- **summary**:    Could not release funds for entering or extending the safe-mode. 

   This error comes from the underlying `Currency`. 
 
### DepositPlaced(`AccountId32`, `u128`)
- **interface**: `api.events.safeMode.DepositPlaced.is`
- **summary**:    An account reserved funds for either entering or extending the safe-mode. 
 
### DepositReleased(`AccountId32`, `u128`)
- **interface**: `api.events.safeMode.DepositReleased.is`
- **summary**:    An account had a reserve released that was reserved. 
 
### DepositSlashed(`AccountId32`, `u128`)
- **interface**: `api.events.safeMode.DepositSlashed.is`
- **summary**:    An account had reserve slashed that was reserved. 
 
### Entered(`u32`)
- **interface**: `api.events.safeMode.Entered.is`
- **summary**:    The safe-mode was entered until inclusively this block. 
 
### Exited(`PalletSafeModeExitReason`)
- **interface**: `api.events.safeMode.Exited.is`
- **summary**:    Exited the safe-mode for a specific reason. 
 
### Extended(`u32`)
- **interface**: `api.events.safeMode.Extended.is`
- **summary**:    The safe-mode was extended until inclusively this block. 

___


## salary
 
### CycleStarted(`u32`)
- **interface**: `api.events.salary.CycleStarted.is`
- **summary**:    The next cycle begins. 
 
### Inducted(`AccountId32`)
- **interface**: `api.events.salary.Inducted.is`
- **summary**:    A member is inducted into the payroll. 
 
### Paid(`AccountId32`, `AccountId32`, `u128`, `Null`)
- **interface**: `api.events.salary.Paid.is`
- **summary**:    A payment happened. 
 
### Registered(`AccountId32`, `u128`)
- **interface**: `api.events.salary.Registered.is`
- **summary**:    A member registered for a payout. 
 
### Swapped(`AccountId32`, `AccountId32`)
- **interface**: `api.events.salary.Swapped.is`
- **summary**:    A member swapped their account. 

___


## scheduler
 
### AgendaIncomplete(`u32`)
- **interface**: `api.events.scheduler.AgendaIncomplete.is`
- **summary**:    Agenda is incomplete from `when`. 
 
### CallUnavailable(`(u32,u32)`, `Option<[u8;32]>`)
- **interface**: `api.events.scheduler.CallUnavailable.is`
- **summary**:    The call for the provided hash was not found so the task has been aborted. 
 
### Canceled(`u32`, `u32`)
- **interface**: `api.events.scheduler.Canceled.is`
- **summary**:    Canceled some task. 
 
### Dispatched(`(u32,u32)`, `Option<[u8;32]>`, `Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.scheduler.Dispatched.is`
- **summary**:    Dispatched some task. 
 
### PeriodicFailed(`(u32,u32)`, `Option<[u8;32]>`)
- **interface**: `api.events.scheduler.PeriodicFailed.is`
- **summary**:    The given task was unable to be renewed since the agenda is full at that block. 
 
### PermanentlyOverweight(`(u32,u32)`, `Option<[u8;32]>`)
- **interface**: `api.events.scheduler.PermanentlyOverweight.is`
- **summary**:    The given task can never be executed since it is overweight. 
 
### RetryCancelled(`(u32,u32)`, `Option<[u8;32]>`)
- **interface**: `api.events.scheduler.RetryCancelled.is`
- **summary**:    Cancel a retry configuration for some task. 
 
### RetryFailed(`(u32,u32)`, `Option<[u8;32]>`)
- **interface**: `api.events.scheduler.RetryFailed.is`
- **summary**:    The given task was unable to be retried since the agenda is full at that block or there  was not enough weight to reschedule it. 
 
### RetrySet(`(u32,u32)`, `Option<[u8;32]>`, `u32`, `u8`)
- **interface**: `api.events.scheduler.RetrySet.is`
- **summary**:    Set a retry configuration for some task. 
 
### Scheduled(`u32`, `u32`)
- **interface**: `api.events.scheduler.Scheduled.is`
- **summary**:    Scheduled some task. 

___


## session
 
### NewSession(`u32`)
- **interface**: `api.events.session.NewSession.is`
- **summary**:    New session has happened. Note that the argument is the session index, not the  block number as the type might suggest. 
 
### ValidatorDisabled(`AccountId32`)
- **interface**: `api.events.session.ValidatorDisabled.is`
- **summary**:    Validator has been disabled. 
 
### ValidatorReenabled(`AccountId32`)
- **interface**: `api.events.session.ValidatorReenabled.is`
- **summary**:    Validator has been re-enabled. 

___


## skipFeelessPayment
 
### FeeSkipped(`KitchensinkRuntimeOriginCaller`)
- **interface**: `api.events.skipFeelessPayment.FeeSkipped.is`
- **summary**:    A transaction fee was skipped. 

___


## society
 
### AutoUnbid(`AccountId32`)
- **interface**: `api.events.society.AutoUnbid.is`
- **summary**:    A candidate was dropped (due to an excess of bids in the system). 
 
### Bid(`AccountId32`, `u128`)
- **interface**: `api.events.society.Bid.is`
- **summary**:    A membership bid just happened. The given account is the candidate's ID and their offer  is the second. 
 
### CandidateSuspended(`AccountId32`)
- **interface**: `api.events.society.CandidateSuspended.is`
- **summary**:    A candidate has been suspended 
 
### Challenged(`AccountId32`)
- **interface**: `api.events.society.Challenged.is`
- **summary**:    A member has been challenged 
 
### DefenderVote(`AccountId32`, `bool`)
- **interface**: `api.events.society.DefenderVote.is`
- **summary**:    A vote has been placed for a defending member 
 
### Deposit(`u128`)
- **interface**: `api.events.society.Deposit.is`
- **summary**:    Some funds were deposited into the society account. 
 
### Elevated(`AccountId32`, `u32`)
- **interface**: `api.events.society.Elevated.is`
- **summary**:    A \[member\] got elevated to \[rank\]. 
 
### Founded(`AccountId32`)
- **interface**: `api.events.society.Founded.is`
- **summary**:    The society is founded by the given identity. 
 
### Inducted(`AccountId32`, `Vec<AccountId32>`)
- **interface**: `api.events.society.Inducted.is`
- **summary**:    A group of candidates have been inducted. The batch's primary is the first value, the  batch in full is the second. 
 
### MemberSuspended(`AccountId32`)
- **interface**: `api.events.society.MemberSuspended.is`
- **summary**:    A member has been suspended 
 
### NewParams(`PalletSocietyGroupParams`)
- **interface**: `api.events.society.NewParams.is`
- **summary**:    A new set of \[params\] has been set for the group. 
 
### SuspendedMemberJudgement(`AccountId32`, `bool`)
- **interface**: `api.events.society.SuspendedMemberJudgement.is`
- **summary**:    A suspended member has been judged. 
 
### Unbid(`AccountId32`)
- **interface**: `api.events.society.Unbid.is`
- **summary**:    A candidate was dropped (by their request). 
 
### Unfounded(`AccountId32`)
- **interface**: `api.events.society.Unfounded.is`
- **summary**:    Society is unfounded. 
 
### Unvouch(`AccountId32`)
- **interface**: `api.events.society.Unvouch.is`
- **summary**:    A candidate was dropped (by request of who vouched for them). 
 
### Vote(`AccountId32`, `AccountId32`, `bool`)
- **interface**: `api.events.society.Vote.is`
- **summary**:    A vote has been placed 
 
### Vouch(`AccountId32`, `u128`, `AccountId32`)
- **interface**: `api.events.society.Vouch.is`
- **summary**:    A membership bid just happened by vouching. The given account is the candidate's ID and  their offer is the second. The vouching party is the third. 

___


## staking
 
### Bonded(`AccountId32`, `u128`)
- **interface**: `api.events.staking.Bonded.is`
- **summary**:    An account has bonded this amount. \[stash, amount\] 

   NOTE: This event is only emitted when funds are bonded via a dispatchable. Notably,  it will not be emitted for staking rewards when they are added to stake. 
 
### Chilled(`AccountId32`)
- **interface**: `api.events.staking.Chilled.is`
- **summary**:    An account has stopped participating as either a validator or nominator. 
 
### ControllerBatchDeprecated(`u32`)
- **interface**: `api.events.staking.ControllerBatchDeprecated.is`
- **summary**:    Report of a controller batch deprecation. 
 
### CurrencyMigrated(`AccountId32`, `u128`)
- **interface**: `api.events.staking.CurrencyMigrated.is`
- **summary**:    Staking balance migrated from locks to holds, with any balance that could not be held  is force withdrawn. 
 
### EraPaid(`u32`, `u128`, `u128`)
- **interface**: `api.events.staking.EraPaid.is`
- **summary**:    The era payout has been set; the first balance is the validator-payout; the second is  the remainder from the maximum amount of reward. 
 
### ForceEra(`PalletStakingForcing`)
- **interface**: `api.events.staking.ForceEra.is`
- **summary**:    A new force era mode was set. 
 
### Kicked(`AccountId32`, `AccountId32`)
- **interface**: `api.events.staking.Kicked.is`
- **summary**:    A nominator has been kicked from a validator. 
 
### OldSlashingReportDiscarded(`u32`)
- **interface**: `api.events.staking.OldSlashingReportDiscarded.is`
- **summary**:    An old slashing report from a prior era was discarded because it could  not be processed. 
 
### PayoutStarted(`u32`, `AccountId32`, `u32`, `Option<u32>`)
- **interface**: `api.events.staking.PayoutStarted.is`
- **summary**:    A Page of stakers rewards are getting paid. `next` is `None` if all pages are claimed. 
 
### Rewarded(`AccountId32`, `PalletStakingRewardDestination`, `u128`)
- **interface**: `api.events.staking.Rewarded.is`
- **summary**:    The nominator has been rewarded by this amount to this destination. 
 
### Slashed(`AccountId32`, `u128`)
- **interface**: `api.events.staking.Slashed.is`
- **summary**:    A staker (validator or nominator) has been slashed by the given amount. 
 
### SlashReported(`AccountId32`, `Perbill`, `u32`)
- **interface**: `api.events.staking.SlashReported.is`
- **summary**:    A slash for the given validator, for the given percentage of their stake, at the given  era as been reported. 
 
### SnapshotTargetsSizeExceeded(`u32`)
- **interface**: `api.events.staking.SnapshotTargetsSizeExceeded.is`
- **summary**:    Targets size limit reached. 
 
### SnapshotVotersSizeExceeded(`u32`)
- **interface**: `api.events.staking.SnapshotVotersSizeExceeded.is`
- **summary**:    Voters size limit reached. 
 
### StakersElected()
- **interface**: `api.events.staking.StakersElected.is`
- **summary**:    A new set of stakers was elected. 
 
### StakingElectionFailed()
- **interface**: `api.events.staking.StakingElectionFailed.is`
- **summary**:    The election failed. No new era is planned. 
 
### Unbonded(`AccountId32`, `u128`)
- **interface**: `api.events.staking.Unbonded.is`
- **summary**:    An account has unbonded this amount. 
 
### ValidatorPrefsSet(`AccountId32`, `PalletStakingValidatorPrefs`)
- **interface**: `api.events.staking.ValidatorPrefsSet.is`
- **summary**:    A validator has set their preferences. 
 
### Withdrawn(`AccountId32`, `u128`)
- **interface**: `api.events.staking.Withdrawn.is`
- **summary**:    An account has called `withdraw_unbonded` and removed unbonding chunks worth `Balance`  from the unlocking queue. 

___


## statement
 
### NewStatement(`AccountId32`, `SpStatementStoreStatement`)
- **interface**: `api.events.statement.NewStatement.is`
- **summary**:    A new statement is submitted 

___


## stateTrieMigration
 
### AutoMigrationFinished()
- **interface**: `api.events.stateTrieMigration.AutoMigrationFinished.is`
- **summary**:    The auto migration task finished. 
 
### Halted(`PalletStateTrieMigrationError`)
- **interface**: `api.events.stateTrieMigration.Halted.is`
- **summary**:    Migration got halted due to an error or miss-configuration. 
 
### Migrated(`u32`, `u32`, `PalletStateTrieMigrationMigrationCompute`)
- **interface**: `api.events.stateTrieMigration.Migrated.is`
- **summary**:    Given number of `(top, child)` keys were migrated respectively, with the given  `compute`. 
 
### Slashed(`AccountId32`, `u128`)
- **interface**: `api.events.stateTrieMigration.Slashed.is`
- **summary**:    Some account got slashed by the given amount. 

___


## sudo
 
### KeyChanged(`Option<AccountId32>`, `AccountId32`)
- **interface**: `api.events.sudo.KeyChanged.is`
- **summary**:    The sudo key has been updated. 
 
### KeyRemoved()
- **interface**: `api.events.sudo.KeyRemoved.is`
- **summary**:    The key was permanently removed. 
 
### Sudid(`Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.sudo.Sudid.is`
- **summary**:    A sudo call just took place. 
 
### SudoAsDone(`Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.sudo.SudoAsDone.is`
- **summary**:    A [sudo_as](Pallet::sudo_as) call just took place. 

___


## system
 
### CodeUpdated()
- **interface**: `api.events.system.CodeUpdated.is`
- **summary**:    `:code` was updated. 
 
### ExtrinsicFailed(`SpRuntimeDispatchError`, `FrameSystemDispatchEventInfo`)
- **interface**: `api.events.system.ExtrinsicFailed.is`
- **summary**:    An extrinsic failed. 
 
### ExtrinsicSuccess(`FrameSystemDispatchEventInfo`)
- **interface**: `api.events.system.ExtrinsicSuccess.is`
- **summary**:    An extrinsic completed successfully. 
 
### KilledAccount(`AccountId32`)
- **interface**: `api.events.system.KilledAccount.is`
- **summary**:    An account was reaped. 
 
### NewAccount(`AccountId32`)
- **interface**: `api.events.system.NewAccount.is`
- **summary**:    A new account was created. 
 
### RejectedInvalidAuthorizedUpgrade(`H256`, `SpRuntimeDispatchError`)
- **interface**: `api.events.system.RejectedInvalidAuthorizedUpgrade.is`
- **summary**:    An invalid authorized upgrade was rejected while trying to apply it. 
 
### Remarked(`AccountId32`, `H256`)
- **interface**: `api.events.system.Remarked.is`
- **summary**:    On on-chain remark happened. 
 
### UpgradeAuthorized(`H256`, `bool`)
- **interface**: `api.events.system.UpgradeAuthorized.is`
- **summary**:    An upgrade was authorized. 

___


## technicalCommittee
 
### Approved(`H256`)
- **interface**: `api.events.technicalCommittee.Approved.is`
- **summary**:    A motion was approved by the required threshold. 
 
### Closed(`H256`, `u32`, `u32`)
- **interface**: `api.events.technicalCommittee.Closed.is`
- **summary**:    A proposal was closed because its threshold was reached or after its duration was up. 
 
### Disapproved(`H256`)
- **interface**: `api.events.technicalCommittee.Disapproved.is`
- **summary**:    A motion was not approved by the required threshold. 
 
### Executed(`H256`, `Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.technicalCommittee.Executed.is`
- **summary**:    A motion was executed; result will be `Ok` if it returned without error. 
 
### Killed(`H256`)
- **interface**: `api.events.technicalCommittee.Killed.is`
- **summary**:    A proposal was killed. 
 
### MemberExecuted(`H256`, `Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.technicalCommittee.MemberExecuted.is`
- **summary**:    A single member did some action; result will be `Ok` if it returned without error. 
 
### ProposalCostBurned(`H256`, `AccountId32`)
- **interface**: `api.events.technicalCommittee.ProposalCostBurned.is`
- **summary**:    Some cost for storing a proposal was burned. 
 
### ProposalCostReleased(`H256`, `AccountId32`)
- **interface**: `api.events.technicalCommittee.ProposalCostReleased.is`
- **summary**:    Some cost for storing a proposal was released. 
 
### Proposed(`AccountId32`, `u32`, `H256`, `u32`)
- **interface**: `api.events.technicalCommittee.Proposed.is`
- **summary**:    A motion (given hash) has been proposed (by given account) with a threshold (given  `MemberCount`). 
 
### Voted(`AccountId32`, `H256`, `bool`, `u32`, `u32`)
- **interface**: `api.events.technicalCommittee.Voted.is`
- **summary**:    A motion (given hash) has been voted on by given account, leaving  a tally (yes votes and no votes given respectively as `MemberCount`). 

___


## technicalMembership
 
### Dummy()
- **interface**: `api.events.technicalMembership.Dummy.is`
- **summary**:    Phantom member, never used. 
 
### KeyChanged()
- **interface**: `api.events.technicalMembership.KeyChanged.is`
- **summary**:    One of the members' keys changed. 
 
### MemberAdded()
- **interface**: `api.events.technicalMembership.MemberAdded.is`
- **summary**:    The given member was added; see the transaction for who. 
 
### MemberRemoved()
- **interface**: `api.events.technicalMembership.MemberRemoved.is`
- **summary**:    The given member was removed; see the transaction for who. 
 
### MembersReset()
- **interface**: `api.events.technicalMembership.MembersReset.is`
- **summary**:    The membership was reset; see the transaction for who the new set is. 
 
### MembersSwapped()
- **interface**: `api.events.technicalMembership.MembersSwapped.is`
- **summary**:    Two members were swapped; see the transaction for who. 

___


## tips
 
### NewTip(`H256`)
- **interface**: `api.events.tips.NewTip.is`
- **summary**:    A new tip suggestion has been opened. 
 
### TipClosed(`H256`, `AccountId32`, `u128`)
- **interface**: `api.events.tips.TipClosed.is`
- **summary**:    A tip suggestion has been closed. 
 
### TipClosing(`H256`)
- **interface**: `api.events.tips.TipClosing.is`
- **summary**:    A tip suggestion has reached threshold and is closing. 
 
### TipRetracted(`H256`)
- **interface**: `api.events.tips.TipRetracted.is`
- **summary**:    A tip suggestion has been retracted. 
 
### TipSlashed(`H256`, `AccountId32`, `u128`)
- **interface**: `api.events.tips.TipSlashed.is`
- **summary**:    A tip suggestion has been slashed. 

___


## transactionPayment
 
### TransactionFeePaid(`AccountId32`, `u128`, `u128`)
- **interface**: `api.events.transactionPayment.TransactionFeePaid.is`
- **summary**:    A transaction fee `actual_fee`, of which `tip` was added to the minimum inclusion fee,  has been paid by `who`. 

___


## transactionStorage
 
### ProofChecked()
- **interface**: `api.events.transactionStorage.ProofChecked.is`
- **summary**:    Storage proof was successfully checked. 
 
### Renewed(`u32`)
- **interface**: `api.events.transactionStorage.Renewed.is`
- **summary**:    Renewed data under specified index. 
 
### Stored(`u32`)
- **interface**: `api.events.transactionStorage.Stored.is`
- **summary**:    Stored data under specified index. 

___


## treasury
 
### AssetSpendApproved(`u32`, `FrameSupportTokensFungibleUnionOfNativeOrWithId`, `u128`, `AccountId32`, `u32`, `u32`)
- **interface**: `api.events.treasury.AssetSpendApproved.is`
- **summary**:    A new asset spend proposal has been approved. 
 
### AssetSpendVoided(`u32`)
- **interface**: `api.events.treasury.AssetSpendVoided.is`
- **summary**:    An approved spend was voided. 
 
### Awarded(`u32`, `u128`, `AccountId32`)
- **interface**: `api.events.treasury.Awarded.is`
- **summary**:    Some funds have been allocated. 
 
### Burnt(`u128`)
- **interface**: `api.events.treasury.Burnt.is`
- **summary**:    Some of our funds have been burnt. 
 
### Deposit(`u128`)
- **interface**: `api.events.treasury.Deposit.is`
- **summary**:    Some funds have been deposited. 
 
### Paid(`u32`, `Null`)
- **interface**: `api.events.treasury.Paid.is`
- **summary**:    A payment happened. 
 
### PaymentFailed(`u32`, `Null`)
- **interface**: `api.events.treasury.PaymentFailed.is`
- **summary**:    A payment failed and can be retried. 
 
### Rollover(`u128`)
- **interface**: `api.events.treasury.Rollover.is`
- **summary**:    Spending has finished; this is the amount that rolls over until next spend. 
 
### SpendApproved(`u32`, `u128`, `AccountId32`)
- **interface**: `api.events.treasury.SpendApproved.is`
- **summary**:    A new spend proposal has been approved. 
 
### Spending(`u128`)
- **interface**: `api.events.treasury.Spending.is`
- **summary**:    We have ended a spend period and will now allocate funds. 
 
### SpendProcessed(`u32`)
- **interface**: `api.events.treasury.SpendProcessed.is`
- **summary**:    A spend was processed and removed from the storage. It might have been successfully  paid or it may have expired. 
 
### UpdatedInactive(`u128`, `u128`)
- **interface**: `api.events.treasury.UpdatedInactive.is`
- **summary**:    The inactive funds of the pallet have been updated. 

___


## txPause
 
### CallPaused(`(Bytes,Bytes)`)
- **interface**: `api.events.txPause.CallPaused.is`
- **summary**:    This pallet, or a specific call is now paused. 
 
### CallUnpaused(`(Bytes,Bytes)`)
- **interface**: `api.events.txPause.CallUnpaused.is`
- **summary**:    This pallet, or a specific call is now unpaused. 

___


## uniques
 
### ApprovalCancelled(`u32`, `u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.uniques.ApprovalCancelled.is`
- **summary**:    An approval for a `delegate` account to transfer the `item` of an item  `collection` was cancelled by its `owner`. 
 
### ApprovedTransfer(`u32`, `u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.uniques.ApprovedTransfer.is`
- **summary**:    An `item` of a `collection` has been approved by the `owner` for transfer by  a `delegate`. 
 
### AttributeCleared(`u32`, `Option<u32>`, `Bytes`)
- **interface**: `api.events.uniques.AttributeCleared.is`
- **summary**:    Attribute metadata has been cleared for a `collection` or `item`. 
 
### AttributeSet(`u32`, `Option<u32>`, `Bytes`, `Bytes`)
- **interface**: `api.events.uniques.AttributeSet.is`
- **summary**:    New attribute metadata has been set for a `collection` or `item`. 
 
### Burned(`u32`, `u32`, `AccountId32`)
- **interface**: `api.events.uniques.Burned.is`
- **summary**:    An `item` was destroyed. 
 
### CollectionFrozen(`u32`)
- **interface**: `api.events.uniques.CollectionFrozen.is`
- **summary**:    Some `collection` was frozen. 
 
### CollectionMaxSupplySet(`u32`, `u32`)
- **interface**: `api.events.uniques.CollectionMaxSupplySet.is`
- **summary**:    Max supply has been set for a collection. 
 
### CollectionMetadataCleared(`u32`)
- **interface**: `api.events.uniques.CollectionMetadataCleared.is`
- **summary**:    Metadata has been cleared for a `collection`. 
 
### CollectionMetadataSet(`u32`, `Bytes`, `bool`)
- **interface**: `api.events.uniques.CollectionMetadataSet.is`
- **summary**:    New metadata has been set for a `collection`. 
 
### CollectionThawed(`u32`)
- **interface**: `api.events.uniques.CollectionThawed.is`
- **summary**:    Some `collection` was thawed. 
 
### Created(`u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.uniques.Created.is`
- **summary**:    A `collection` was created. 
 
### Destroyed(`u32`)
- **interface**: `api.events.uniques.Destroyed.is`
- **summary**:    A `collection` was destroyed. 
 
### ForceCreated(`u32`, `AccountId32`)
- **interface**: `api.events.uniques.ForceCreated.is`
- **summary**:    A `collection` was force-created. 
 
### Frozen(`u32`, `u32`)
- **interface**: `api.events.uniques.Frozen.is`
- **summary**:    Some `item` was frozen. 
 
### Issued(`u32`, `u32`, `AccountId32`)
- **interface**: `api.events.uniques.Issued.is`
- **summary**:    An `item` was issued. 
 
### ItemBought(`u32`, `u32`, `u128`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.uniques.ItemBought.is`
- **summary**:    An item was bought. 
 
### ItemPriceRemoved(`u32`, `u32`)
- **interface**: `api.events.uniques.ItemPriceRemoved.is`
- **summary**:    The price for the instance was removed. 
 
### ItemPriceSet(`u32`, `u32`, `u128`, `Option<AccountId32>`)
- **interface**: `api.events.uniques.ItemPriceSet.is`
- **summary**:    The price was set for the instance. 
 
### ItemStatusChanged(`u32`)
- **interface**: `api.events.uniques.ItemStatusChanged.is`
- **summary**:    A `collection` has had its attributes changed by the `Force` origin. 
 
### MetadataCleared(`u32`, `u32`)
- **interface**: `api.events.uniques.MetadataCleared.is`
- **summary**:    Metadata has been cleared for an item. 
 
### MetadataSet(`u32`, `u32`, `Bytes`, `bool`)
- **interface**: `api.events.uniques.MetadataSet.is`
- **summary**:    New metadata has been set for an item. 
 
### OwnerChanged(`u32`, `AccountId32`)
- **interface**: `api.events.uniques.OwnerChanged.is`
- **summary**:    The owner changed. 
 
### OwnershipAcceptanceChanged(`AccountId32`, `Option<u32>`)
- **interface**: `api.events.uniques.OwnershipAcceptanceChanged.is`
- **summary**:    Ownership acceptance has changed for an account. 
 
### Redeposited(`u32`, `Vec<u32>`)
- **interface**: `api.events.uniques.Redeposited.is`
- **summary**:    Metadata has been cleared for an item. 
 
### TeamChanged(`u32`, `AccountId32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.uniques.TeamChanged.is`
- **summary**:    The management team changed. 
 
### Thawed(`u32`, `u32`)
- **interface**: `api.events.uniques.Thawed.is`
- **summary**:    Some `item` was thawed. 
 
### Transferred(`u32`, `u32`, `AccountId32`, `AccountId32`)
- **interface**: `api.events.uniques.Transferred.is`
- **summary**:    An `item` was transferred. 

___


## utility
 
### BatchCompleted()
- **interface**: `api.events.utility.BatchCompleted.is`
- **summary**:    Batch of dispatches completed fully with no error. 
 
### BatchCompletedWithErrors()
- **interface**: `api.events.utility.BatchCompletedWithErrors.is`
- **summary**:    Batch of dispatches completed but has errors. 
 
### BatchInterrupted(`u32`, `SpRuntimeDispatchError`)
- **interface**: `api.events.utility.BatchInterrupted.is`
- **summary**:    Batch of dispatches did not complete fully. Index of first failing dispatch given, as  well as the error. 
 
### DispatchedAs(`Result<Null, SpRuntimeDispatchError>`)
- **interface**: `api.events.utility.DispatchedAs.is`
- **summary**:    A call was dispatched. 
 
### IfElseFallbackCalled(`SpRuntimeDispatchError`)
- **interface**: `api.events.utility.IfElseFallbackCalled.is`
- **summary**:    The fallback call was dispatched. 
 
### IfElseMainSuccess()
- **interface**: `api.events.utility.IfElseMainSuccess.is`
- **summary**:    Main call was dispatched. 
 
### ItemCompleted()
- **interface**: `api.events.utility.ItemCompleted.is`
- **summary**:    A single item within a Batch of dispatches has completed with no error. 
 
### ItemFailed(`SpRuntimeDispatchError`)
- **interface**: `api.events.utility.ItemFailed.is`
- **summary**:    A single item within a Batch of dispatches has completed with error. 

___


## vesting
 
### VestingCompleted(`AccountId32`)
- **interface**: `api.events.vesting.VestingCompleted.is`
- **summary**:    An \[account\] has become fully vested. 
 
### VestingUpdated(`AccountId32`, `u128`)
- **interface**: `api.events.vesting.VestingUpdated.is`
- **summary**:    The amount vested has been updated. This could indicate a change in funds available.  The balance given is the amount which is left unvested (and thus locked). 

___


## voterList
 
### Rebagged(`AccountId32`, `u64`, `u64`)
- **interface**: `api.events.voterList.Rebagged.is`
- **summary**:    Moved an account from one bag to another. 
 
### ScoreUpdated(`AccountId32`, `u64`)
- **interface**: `api.events.voterList.ScoreUpdated.is`
- **summary**:    Updated the score of some account to the given amount. 

___


## whitelist
 
### CallWhitelisted(`H256`)
- **interface**: `api.events.whitelist.CallWhitelisted.is`
 
### WhitelistedCallDispatched(`H256`, `Result<FrameSupportDispatchPostDispatchInfo, SpRuntimeDispatchErrorWithPostInfo>`)
- **interface**: `api.events.whitelist.WhitelistedCallDispatched.is`
 
### WhitelistedCallRemoved(`H256`)
- **interface**: `api.events.whitelist.WhitelistedCallRemoved.is`
