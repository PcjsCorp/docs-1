---
title: Errors
---

This page lists the errors that can be encountered in the different modules. 

(NOTE: These were generated from a static/snapshot view of a recent default Substrate runtime. Some items may not be available in older nodes, or in any customized implementations.)

- **[alliance](#alliance)**

- **[allianceMotion](#alliancemotion)**

- **[assetConversion](#assetconversion)**

- **[assetConversionMigration](#assetconversionmigration)**

- **[assetRate](#assetrate)**

- **[assetRewards](#assetrewards)**

- **[assets](#assets)**

- **[assetsFreezer](#assetsfreezer)**

- **[babe](#babe)**

- **[balances](#balances)**

- **[beefy](#beefy)**

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

- **[poolAssets](#poolassets)**

- **[preimage](#preimage)**

- **[proxy](#proxy)**

- **[rankedCollective](#rankedcollective)**

- **[rankedPolls](#rankedpolls)**

- **[recovery](#recovery)**

- **[referenda](#referenda)**

- **[remark](#remark)**

- **[revive](#revive)**

- **[safeMode](#safemode)**

- **[salary](#salary)**

- **[scheduler](#scheduler)**

- **[session](#session)**

- **[society](#society)**

- **[staking](#staking)**

- **[stateTrieMigration](#statetriemigration)**

- **[sudo](#sudo)**

- **[system](#system)**

- **[tasksExample](#tasksexample)**

- **[technicalCommittee](#technicalcommittee)**

- **[technicalMembership](#technicalmembership)**

- **[tips](#tips)**

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
 
### AccountNonGrata
- **interface**: `api.errors.alliance.AccountNonGrata.is`
- **summary**:    Account has been deemed unscrupulous by the Alliance and is not welcome to join or be  nominated. 
 
### AllianceAlreadyInitialized
- **interface**: `api.errors.alliance.AllianceAlreadyInitialized.is`
- **summary**:    The Alliance has been initialized, therefore cannot be initialized again. 
 
### AllianceNotYetInitialized
- **interface**: `api.errors.alliance.AllianceNotYetInitialized.is`
- **summary**:    The Alliance has not been initialized yet, therefore accounts cannot join it. 
 
### AlreadyElevated
- **interface**: `api.errors.alliance.AlreadyElevated.is`
- **summary**:    Account is already an elevated (fellow) member. 
 
### AlreadyMember
- **interface**: `api.errors.alliance.AlreadyMember.is`
- **summary**:    Account is already a member. 
 
### AlreadyRetiring
- **interface**: `api.errors.alliance.AlreadyRetiring.is`
- **summary**:    Account already gave retirement notice 
 
### AlreadyUnscrupulous
- **interface**: `api.errors.alliance.AlreadyUnscrupulous.is`
- **summary**:    Item is already listed as unscrupulous. 
 
### BadWitness
- **interface**: `api.errors.alliance.BadWitness.is`
- **summary**:    Invalid witness data given. 
 
### FellowsMissing
- **interface**: `api.errors.alliance.FellowsMissing.is`
- **summary**:    Fellows must be provided to initialize the Alliance. 
 
### InsufficientFunds
- **interface**: `api.errors.alliance.InsufficientFunds.is`
- **summary**:    Balance is insufficient for the required deposit. 
 
### MissingAnnouncement
- **interface**: `api.errors.alliance.MissingAnnouncement.is`
- **summary**:    The announcement is not found. 
 
### MissingProposalHash
- **interface**: `api.errors.alliance.MissingProposalHash.is`
- **summary**:    The proposal hash is not found. 
 
### NotAlly
- **interface**: `api.errors.alliance.NotAlly.is`
- **summary**:    Account is not an ally. 
 
### NotListedAsUnscrupulous
- **interface**: `api.errors.alliance.NotListedAsUnscrupulous.is`
- **summary**:    Item has not been deemed unscrupulous. 
 
### NotMember
- **interface**: `api.errors.alliance.NotMember.is`
- **summary**:    Account is not a member. 
 
### NoVotingRights
- **interface**: `api.errors.alliance.NoVotingRights.is`
- **summary**:    Account does not have voting rights. 
 
### RetirementNoticeNotGiven
- **interface**: `api.errors.alliance.RetirementNoticeNotGiven.is`
- **summary**:    Account did not give a retirement notice required to retire. 
 
### RetirementPeriodNotPassed
- **interface**: `api.errors.alliance.RetirementPeriodNotPassed.is`
- **summary**:    Retirement period has not passed. 
 
### TooLongWebsiteUrl
- **interface**: `api.errors.alliance.TooLongWebsiteUrl.is`
- **summary**:    Length of website URL exceeds `MaxWebsiteUrlLength`. 
 
### TooManyAnnouncements
- **interface**: `api.errors.alliance.TooManyAnnouncements.is`
- **summary**:    Number of announcements exceeds `MaxAnnouncementsCount`. 
 
### TooManyMembers
- **interface**: `api.errors.alliance.TooManyMembers.is`
- **summary**:    Number of members exceeds `MaxMembersCount`. 
 
### TooManyUnscrupulousItems
- **interface**: `api.errors.alliance.TooManyUnscrupulousItems.is`
- **summary**:    The number of unscrupulous items exceeds `MaxUnscrupulousItems`. 
 
### WithoutGoodIdentityJudgement
- **interface**: `api.errors.alliance.WithoutGoodIdentityJudgement.is`
- **summary**:    The account's identity has no good judgement. 
 
### WithoutRequiredIdentityFields
- **interface**: `api.errors.alliance.WithoutRequiredIdentityFields.is`
- **summary**:    The account's identity does not have display field and website field. 

___


## allianceMotion
 
### AlreadyInitialized
- **interface**: `api.errors.allianceMotion.AlreadyInitialized.is`
- **summary**:    Members are already initialized! 
 
### DuplicateProposal
- **interface**: `api.errors.allianceMotion.DuplicateProposal.is`
- **summary**:    Duplicate proposals not allowed 
 
### DuplicateVote
- **interface**: `api.errors.allianceMotion.DuplicateVote.is`
- **summary**:    Duplicate vote ignored 
 
### NotMember
- **interface**: `api.errors.allianceMotion.NotMember.is`
- **summary**:    Account is not a member 
 
### PrimeAccountNotMember
- **interface**: `api.errors.allianceMotion.PrimeAccountNotMember.is`
- **summary**:    Prime account is not a member 
 
### ProposalActive
- **interface**: `api.errors.allianceMotion.ProposalActive.is`
- **summary**:    Proposal is still active. 
 
### ProposalMissing
- **interface**: `api.errors.allianceMotion.ProposalMissing.is`
- **summary**:    Proposal must exist 
 
### TooEarly
- **interface**: `api.errors.allianceMotion.TooEarly.is`
- **summary**:    The close call was made too early, before the end of the voting. 
 
### TooManyProposals
- **interface**: `api.errors.allianceMotion.TooManyProposals.is`
- **summary**:    There can only be a maximum of `MaxProposals` active proposals. 
 
### WrongIndex
- **interface**: `api.errors.allianceMotion.WrongIndex.is`
- **summary**:    Mismatched index 
 
### WrongProposalLength
- **interface**: `api.errors.allianceMotion.WrongProposalLength.is`
- **summary**:    The given length bound for the proposal was too low. 
 
### WrongProposalWeight
- **interface**: `api.errors.allianceMotion.WrongProposalWeight.is`
- **summary**:    The given weight bound for the proposal was too low. 

___


## assetConversion
 
### AmountOneLessThanMinimal
- **interface**: `api.errors.assetConversion.AmountOneLessThanMinimal.is`
- **summary**:    Provided amount should be greater than or equal to the existential deposit/asset's  minimal amount. 
 
### AmountOutTooHigh
- **interface**: `api.errors.assetConversion.AmountOutTooHigh.is`
- **summary**:    Desired amount can't be equal to the pool reserve. 
 
### AmountTwoLessThanMinimal
- **interface**: `api.errors.assetConversion.AmountTwoLessThanMinimal.is`
- **summary**:    Provided amount should be greater than or equal to the existential deposit/asset's  minimal amount. 
 
### AssetOneDepositDidNotMeetMinimum
- **interface**: `api.errors.assetConversion.AssetOneDepositDidNotMeetMinimum.is`
- **summary**:    The minimal amount requirement for the first token in the pair wasn't met. 
 
### AssetOneWithdrawalDidNotMeetMinimum
- **interface**: `api.errors.assetConversion.AssetOneWithdrawalDidNotMeetMinimum.is`
- **summary**:    The minimal amount requirement for the first token in the pair wasn't met. 
 
### AssetTwoDepositDidNotMeetMinimum
- **interface**: `api.errors.assetConversion.AssetTwoDepositDidNotMeetMinimum.is`
- **summary**:    The minimal amount requirement for the second token in the pair wasn't met. 
 
### AssetTwoWithdrawalDidNotMeetMinimum
- **interface**: `api.errors.assetConversion.AssetTwoWithdrawalDidNotMeetMinimum.is`
- **summary**:    The minimal amount requirement for the second token in the pair wasn't met. 
 
### BelowMinimum
- **interface**: `api.errors.assetConversion.BelowMinimum.is`
- **summary**:    The destination account cannot exist with the swapped funds. 
 
### IncorrectPoolAssetId
- **interface**: `api.errors.assetConversion.IncorrectPoolAssetId.is`
- **summary**:    It was not possible to get or increment the Id of the pool. 
 
### InsufficientLiquidityMinted
- **interface**: `api.errors.assetConversion.InsufficientLiquidityMinted.is`
- **summary**:    Insufficient liquidity minted. 
 
### InvalidAssetPair
- **interface**: `api.errors.assetConversion.InvalidAssetPair.is`
- **summary**:    Provided asset pair is not supported for pool. 
 
### InvalidPath
- **interface**: `api.errors.assetConversion.InvalidPath.is`
- **summary**:    The provided path must consists of 2 assets at least. 
 
### NonUniquePath
- **interface**: `api.errors.assetConversion.NonUniquePath.is`
- **summary**:    The provided path must consists of unique assets. 
 
### OptimalAmountLessThanDesired
- **interface**: `api.errors.assetConversion.OptimalAmountLessThanDesired.is`
- **summary**:    Optimal calculated amount is less than desired. 
 
### Overflow
- **interface**: `api.errors.assetConversion.Overflow.is`
- **summary**:    An overflow happened. 
 
### PoolExists
- **interface**: `api.errors.assetConversion.PoolExists.is`
- **summary**:    Pool already exists. 
 
### PoolNotFound
- **interface**: `api.errors.assetConversion.PoolNotFound.is`
- **summary**:    The pool doesn't exist. 
 
### ProvidedMaximumNotSufficientForSwap
- **interface**: `api.errors.assetConversion.ProvidedMaximumNotSufficientForSwap.is`
- **summary**:    Provided maximum amount is not sufficient for swap. 
 
### ProvidedMinimumNotSufficientForSwap
- **interface**: `api.errors.assetConversion.ProvidedMinimumNotSufficientForSwap.is`
- **summary**:    Calculated amount out is less than provided minimum amount. 
 
### ReserveLeftLessThanMinimal
- **interface**: `api.errors.assetConversion.ReserveLeftLessThanMinimal.is`
- **summary**:    Reserve needs to always be greater than or equal to the existential deposit/asset's  minimal amount. 
 
### WrongDesiredAmount
- **interface**: `api.errors.assetConversion.WrongDesiredAmount.is`
- **summary**:    Desired amount can't be zero. 
 
### ZeroAmount
- **interface**: `api.errors.assetConversion.ZeroAmount.is`
- **summary**:    Amount can't be zero. 
 
### ZeroLiquidity
- **interface**: `api.errors.assetConversion.ZeroLiquidity.is`
- **summary**:    Requested liquidity can't be zero. 

___


## assetConversionMigration
 
### InvalidAssetPair
- **interface**: `api.errors.assetConversionMigration.InvalidAssetPair.is`
- **summary**:    Provided asset pair is not supported for pool. 
 
### PartialTransfer
- **interface**: `api.errors.assetConversionMigration.PartialTransfer.is`
- **summary**:    Indicates a partial transfer of balance to the new account during a migration. 
 
### PoolNotFound
- **interface**: `api.errors.assetConversionMigration.PoolNotFound.is`
- **summary**:    The pool doesn't exist. 
 
### ZeroBalance
- **interface**: `api.errors.assetConversionMigration.ZeroBalance.is`
- **summary**:    Pool's balance cannot be zero. 

___


## assetRate
 
### AlreadyExists
- **interface**: `api.errors.assetRate.AlreadyExists.is`
- **summary**:    The given asset ID already has an assigned conversion rate and cannot be re-created. 
 
### Overflow
- **interface**: `api.errors.assetRate.Overflow.is`
- **summary**:    Overflow ocurred when calculating the inverse rate. 
 
### UnknownAssetKind
- **interface**: `api.errors.assetRate.UnknownAssetKind.is`
- **summary**:    The given asset ID is unknown. 

___


## assetRewards
 
### BlockNumberConversionError
- **interface**: `api.errors.assetRewards.BlockNumberConversionError.is`
- **summary**:    There was an error converting a block number. 
 
### ExpiryBlockMustBeInTheFuture
- **interface**: `api.errors.assetRewards.ExpiryBlockMustBeInTheFuture.is`
- **summary**:    The expiry block must be in the future. 
 
### ExpiryCut
- **interface**: `api.errors.assetRewards.ExpiryCut.is`
- **summary**:    The expiry block can be only extended. 
 
### InsufficientFunds
- **interface**: `api.errors.assetRewards.InsufficientFunds.is`
- **summary**:    Insufficient funds to create the freeze. 
 
### NonEmptyPool
- **interface**: `api.errors.assetRewards.NonEmptyPool.is`
- **summary**:    The pool still has staked tokens or rewards. 
 
### NonExistentAsset
- **interface**: `api.errors.assetRewards.NonExistentAsset.is`
- **summary**:    An operation was attempted with a non-existent asset. 
 
### NonExistentPool
- **interface**: `api.errors.assetRewards.NonExistentPool.is`
- **summary**:    An operation was attempted on a non-existent pool. 
 
### NonExistentStaker
- **interface**: `api.errors.assetRewards.NonExistentStaker.is`
- **summary**:    An operation was attempted for a non-existent staker. 
 
### NotEnoughTokens
- **interface**: `api.errors.assetRewards.NotEnoughTokens.is`
- **summary**:    The staker does not have enough tokens to perform the operation. 
 
### RewardRateCut
- **interface**: `api.errors.assetRewards.RewardRateCut.is`
- **summary**:    The reward rate per block can be only increased. 

___


## assets
 
### AlreadyExists
- **interface**: `api.errors.assets.AlreadyExists.is`
- **summary**:    The asset-account already exists. 
 
### AssetNotLive
- **interface**: `api.errors.assets.AssetNotLive.is`
- **summary**:    The asset is not live, and likely being destroyed. 
 
### BadAssetId
- **interface**: `api.errors.assets.BadAssetId.is`
- **summary**:    The asset ID must be equal to the [`NextAssetId`]. 
 
### BadMetadata
- **interface**: `api.errors.assets.BadMetadata.is`
- **summary**:    Invalid metadata given. 
 
### BadWitness
- **interface**: `api.errors.assets.BadWitness.is`
- **summary**:    Invalid witness data given. 
 
### BalanceLow
- **interface**: `api.errors.assets.BalanceLow.is`
- **summary**:    Account balance must be greater than or equal to the transfer amount. 
 
### CallbackFailed
- **interface**: `api.errors.assets.CallbackFailed.is`
- **summary**:    Callback action resulted in error 
 
### ContainsFreezes
- **interface**: `api.errors.assets.ContainsFreezes.is`
- **summary**:    The asset cannot be destroyed because some accounts for this asset contain freezes. 
 
### ContainsHolds
- **interface**: `api.errors.assets.ContainsHolds.is`
- **summary**:    The asset cannot be destroyed because some accounts for this asset contain holds. 
 
### Frozen
- **interface**: `api.errors.assets.Frozen.is`
- **summary**:    The origin account is frozen. 
 
### IncorrectStatus
- **interface**: `api.errors.assets.IncorrectStatus.is`
- **summary**:    The asset status is not the expected status. 
 
### InUse
- **interface**: `api.errors.assets.InUse.is`
- **summary**:    The asset ID is already taken. 
 
### LiveAsset
- **interface**: `api.errors.assets.LiveAsset.is`
- **summary**:    The asset is a live asset and is actively being used. Usually emit for operations such  as `start_destroy` which require the asset to be in a destroying state. 
 
### MinBalanceZero
- **interface**: `api.errors.assets.MinBalanceZero.is`
- **summary**:    Minimum balance should be non-zero. 
 
### NoAccount
- **interface**: `api.errors.assets.NoAccount.is`
- **summary**:    The account to alter does not exist. 
 
### NoDeposit
- **interface**: `api.errors.assets.NoDeposit.is`
- **summary**:    The asset-account doesn't have an associated deposit. 
 
### NoPermission
- **interface**: `api.errors.assets.NoPermission.is`
- **summary**:    The signing account has no permission to do the operation. 
 
### NotFrozen
- **interface**: `api.errors.assets.NotFrozen.is`
- **summary**:    The asset should be frozen before the given operation. 
 
### Unapproved
- **interface**: `api.errors.assets.Unapproved.is`
- **summary**:    No approval exists that would allow the transfer. 
 
### UnavailableConsumer
- **interface**: `api.errors.assets.UnavailableConsumer.is`
- **summary**:    Unable to increment the consumer reference counters on the account. Either no provider  reference exists to allow a non-zero balance of a non-self-sufficient asset, or one  fewer then the maximum number of consumers has been reached. 
 
### Unknown
- **interface**: `api.errors.assets.Unknown.is`
- **summary**:    The given asset ID is unknown. 
 
### WouldBurn
- **interface**: `api.errors.assets.WouldBurn.is`
- **summary**:    The operation would result in funds being burned. 
 
### WouldDie
- **interface**: `api.errors.assets.WouldDie.is`
- **summary**:    The source account would not survive the transfer and it needs to stay alive. 

___


## assetsFreezer
 
### TooManyFreezes
- **interface**: `api.errors.assetsFreezer.TooManyFreezes.is`
- **summary**:    Number of freezes on an account would exceed `MaxFreezes`. 

___


## babe
 
### DuplicateOffenceReport
- **interface**: `api.errors.babe.DuplicateOffenceReport.is`
- **summary**:    A given equivocation report is valid but already previously reported. 
 
### InvalidConfiguration
- **interface**: `api.errors.babe.InvalidConfiguration.is`
- **summary**:    Submitted configuration is invalid. 
 
### InvalidEquivocationProof
- **interface**: `api.errors.babe.InvalidEquivocationProof.is`
- **summary**:    An equivocation proof provided as part of an equivocation report is invalid. 
 
### InvalidKeyOwnershipProof
- **interface**: `api.errors.babe.InvalidKeyOwnershipProof.is`
- **summary**:    A key ownership proof provided as part of an equivocation report is invalid. 

___


## balances
 
### DeadAccount
- **interface**: `api.errors.balances.DeadAccount.is`
- **summary**:    Beneficiary account must pre-exist. 
 
### DeltaZero
- **interface**: `api.errors.balances.DeltaZero.is`
- **summary**:    The delta cannot be zero. 
 
### ExistentialDeposit
- **interface**: `api.errors.balances.ExistentialDeposit.is`
- **summary**:    Value too low to create account due to existential deposit. 
 
### ExistingVestingSchedule
- **interface**: `api.errors.balances.ExistingVestingSchedule.is`
- **summary**:    A vesting schedule already exists for this account. 
 
### Expendability
- **interface**: `api.errors.balances.Expendability.is`
- **summary**:    Transfer/payment would kill account. 
 
### InsufficientBalance
- **interface**: `api.errors.balances.InsufficientBalance.is`
- **summary**:    Balance too low to send value. 
 
### IssuanceDeactivated
- **interface**: `api.errors.balances.IssuanceDeactivated.is`
- **summary**:    The issuance cannot be modified since it is already deactivated. 
 
### LiquidityRestrictions
- **interface**: `api.errors.balances.LiquidityRestrictions.is`
- **summary**:    Account liquidity restrictions prevent withdrawal. 
 
### TooManyFreezes
- **interface**: `api.errors.balances.TooManyFreezes.is`
- **summary**:    Number of freezes exceed `MaxFreezes`. 
 
### TooManyHolds
- **interface**: `api.errors.balances.TooManyHolds.is`
- **summary**:    Number of holds exceed `VariantCountOf<T::RuntimeHoldReason>`. 
 
### TooManyReserves
- **interface**: `api.errors.balances.TooManyReserves.is`
- **summary**:    Number of named reserves exceed `MaxReserves`. 
 
### VestingBalance
- **interface**: `api.errors.balances.VestingBalance.is`
- **summary**:    Vesting balance too high to send value. 

___


## beefy
 
### DuplicateOffenceReport
- **interface**: `api.errors.beefy.DuplicateOffenceReport.is`
- **summary**:    A given equivocation report is valid but already previously reported. 
 
### InvalidConfiguration
- **interface**: `api.errors.beefy.InvalidConfiguration.is`
- **summary**:    Submitted configuration is invalid. 
 
### InvalidDoubleVotingProof
- **interface**: `api.errors.beefy.InvalidDoubleVotingProof.is`
- **summary**:    A double voting proof provided as part of an equivocation report is invalid. 
 
### InvalidEquivocationProofSession
- **interface**: `api.errors.beefy.InvalidEquivocationProofSession.is`
- **summary**:    The session of the equivocation proof is invalid 
 
### InvalidForkVotingProof
- **interface**: `api.errors.beefy.InvalidForkVotingProof.is`
- **summary**:    A fork voting proof provided as part of an equivocation report is invalid. 
 
### InvalidFutureBlockVotingProof
- **interface**: `api.errors.beefy.InvalidFutureBlockVotingProof.is`
- **summary**:    A future block voting proof provided as part of an equivocation report is invalid. 
 
### InvalidKeyOwnershipProof
- **interface**: `api.errors.beefy.InvalidKeyOwnershipProof.is`
- **summary**:    A key ownership proof provided as part of an equivocation report is invalid. 

___


## bounties
 
### HasActiveChildBounty
- **interface**: `api.errors.bounties.HasActiveChildBounty.is`
- **summary**:    The bounty cannot be closed because it has active child bounties. 
 
### InsufficientProposersBalance
- **interface**: `api.errors.bounties.InsufficientProposersBalance.is`
- **summary**:    Proposer's balance is too low. 
 
### InvalidFee
- **interface**: `api.errors.bounties.InvalidFee.is`
- **summary**:    Invalid bounty fee. 
 
### InvalidIndex
- **interface**: `api.errors.bounties.InvalidIndex.is`
- **summary**:    No proposal or bounty at that index. 
 
### InvalidValue
- **interface**: `api.errors.bounties.InvalidValue.is`
- **summary**:    Invalid bounty value. 
 
### PendingPayout
- **interface**: `api.errors.bounties.PendingPayout.is`
- **summary**:    A bounty payout is pending.  To cancel the bounty, you must unassign and slash the curator. 
 
### Premature
- **interface**: `api.errors.bounties.Premature.is`
- **summary**:    The bounties cannot be claimed/closed because it's still in the countdown period. 
 
### ReasonTooBig
- **interface**: `api.errors.bounties.ReasonTooBig.is`
- **summary**:    The reason given is just too big. 
 
### RequireCurator
- **interface**: `api.errors.bounties.RequireCurator.is`
- **summary**:    Require bounty curator. 
 
### TooManyQueued
- **interface**: `api.errors.bounties.TooManyQueued.is`
- **summary**:    Too many approvals are already queued. 
 
### UnexpectedStatus
- **interface**: `api.errors.bounties.UnexpectedStatus.is`
- **summary**:    The bounty status is unexpected. 

___


## broker
 
### AlreadyExpired
- **interface**: `api.errors.broker.AlreadyExpired.is`
- **summary**:    The lease expiry time has already passed. 
 
### AssignmentNotFound
- **interface**: `api.errors.broker.AssignmentNotFound.is`
- **summary**:    Attempted to force remove an assignment that doesn't exist. 
 
### AutoRenewalNotEnabled
- **interface**: `api.errors.broker.AutoRenewalNotEnabled.is`
- **summary**:    Attempted to disable auto-renewal for a core that didn't have it enabled. 
 
### CompletePivot
- **interface**: `api.errors.broker.CompletePivot.is`
- **summary**:    The pivot mask for the interlacing is complete (and therefore not a strict subset). 
 
### CorruptWorkplan
- **interface**: `api.errors.broker.CorruptWorkplan.is`
- **summary**:    The workplan of the pallet's state is invalid. This indicates a state corruption. 
 
### CreditPurchaseTooSmall
- **interface**: `api.errors.broker.CreditPurchaseTooSmall.is`
- **summary**:    Needed to prevent spam attacks.The amount of credits the user attempted to purchase is  below `T::MinimumCreditPurchase`. 
 
### ExteriorPivot
- **interface**: `api.errors.broker.ExteriorPivot.is`
- **summary**:    The pivot mask for the interlacing is not contained within the region's interlace mask. 
 
### IncompleteAssignment
- **interface**: `api.errors.broker.IncompleteAssignment.is`
- **summary**:    The workload assigned for renewal is incomplete. This is unexpected and indicates a  logic error. 
 
### InvalidConfig
- **interface**: `api.errors.broker.InvalidConfig.is`
- **summary**:    The configuration could not be applied because it is invalid. 
 
### LeaseNotFound
- **interface**: `api.errors.broker.LeaseNotFound.is`
- **summary**:    The lease does not exist. 
 
### NoClaimTimeslices
- **interface**: `api.errors.broker.NoClaimTimeslices.is`
- **summary**:    The revenue must be claimed for 1 or more timeslices. 
 
### NoHistory
- **interface**: `api.errors.broker.NoHistory.is`
- **summary**:    The history item does not exist. 
 
### NonTaskAutoRenewal
- **interface**: `api.errors.broker.NonTaskAutoRenewal.is`
- **summary**:    Only cores which are assigned to a task can be auto-renewed. 
 
### NoPermission
- **interface**: `api.errors.broker.NoPermission.is`
- **summary**:    The caller doesn't have the permission to enable or disable auto-renewal. 
 
### NoSales
- **interface**: `api.errors.broker.NoSales.is`
- **summary**:    There is no sale happening currently. 
 
### NotAllowed
- **interface**: `api.errors.broker.NotAllowed.is`
- **summary**:    Invalid attempt to renew. 
 
### NothingToDo
- **interface**: `api.errors.broker.NothingToDo.is`
- **summary**:    There is no work to be done. 
 
### NotOwner
- **interface**: `api.errors.broker.NotOwner.is`
- **summary**:    The owner of the region is not the origin. 
 
### Overpriced
- **interface**: `api.errors.broker.Overpriced.is`
- **summary**:    The price limit is exceeded. 
 
### PivotTooEarly
- **interface**: `api.errors.broker.PivotTooEarly.is`
- **summary**:    The pivot point of the partition at the beginning of the region. 
 
### PivotTooLate
- **interface**: `api.errors.broker.PivotTooLate.is`
- **summary**:    The pivot point of the partition at or after the end of the region. 
 
### SoldOut
- **interface**: `api.errors.broker.SoldOut.is`
- **summary**:    The sale limit has been reached. 
 
### SovereignAccountNotFound
- **interface**: `api.errors.broker.SovereignAccountNotFound.is`
- **summary**:    Failed to get the sovereign account of a task. 
 
### StillValid
- **interface**: `api.errors.broker.StillValid.is`
- **summary**:    An item cannot be dropped because it is still valid. 
 
### TooEarly
- **interface**: `api.errors.broker.TooEarly.is`
- **summary**:    The purchase cannot happen yet as the sale period is yet to begin. 
 
### TooManyAutoRenewals
- **interface**: `api.errors.broker.TooManyAutoRenewals.is`
- **summary**:    We reached the limit for auto-renewals. 
 
### TooManyLeases
- **interface**: `api.errors.broker.TooManyLeases.is`
- **summary**:    The maximum amount of leases has already been reached. 
 
### TooManyReservations
- **interface**: `api.errors.broker.TooManyReservations.is`
- **summary**:    The maximum amount of reservations has already been reached. 
 
### Unavailable
- **interface**: `api.errors.broker.Unavailable.is`
- **summary**:    There are no cores available. 
 
### Uninitialized
- **interface**: `api.errors.broker.Uninitialized.is`
- **summary**:    This pallet has not yet been initialized. 
 
### UnknownContribution
- **interface**: `api.errors.broker.UnknownContribution.is`
- **summary**:    The identified contribution to the Instantaneous Core Pool is unknown. 
 
### UnknownRegion
- **interface**: `api.errors.broker.UnknownRegion.is`
- **summary**:    The given region identity is not known. 
 
### UnknownRenewal
- **interface**: `api.errors.broker.UnknownRenewal.is`
- **summary**:    The renewal record cannot be found. 
 
### UnknownReservation
- **interface**: `api.errors.broker.UnknownReservation.is`
- **summary**:    No reservation of the given index exists. 
 
### UnknownRevenue
- **interface**: `api.errors.broker.UnknownRevenue.is`
- **summary**:    The revenue for the Instantaneous Core Sales of this period is not (yet) known and thus  this operation cannot proceed. 
 
### VoidPivot
- **interface**: `api.errors.broker.VoidPivot.is`
- **summary**:    The pivot mask for the interlacing is void (and therefore unschedulable). 
 
### WrongTime
- **interface**: `api.errors.broker.WrongTime.is`
- **summary**:    The renewal operation is not valid at the current time (it may become valid in the next  sale). 

___


## childBounties
 
### InsufficientBountyBalance
- **interface**: `api.errors.childBounties.InsufficientBountyBalance.is`
- **summary**:    The bounty balance is not enough to add new child-bounty. 
 
### ParentBountyNotActive
- **interface**: `api.errors.childBounties.ParentBountyNotActive.is`
- **summary**:    The parent bounty is not in active state. 
 
### TooManyChildBounties
- **interface**: `api.errors.childBounties.TooManyChildBounties.is`
- **summary**:    Number of child bounties exceeds limit `MaxActiveChildBountyCount`. 

___


## contracts
 
### CannotAddSelfAsDelegateDependency
- **interface**: `api.errors.contracts.CannotAddSelfAsDelegateDependency.is`
- **summary**:    Can not add a delegate dependency to the code hash of the contract itself. 
 
### CodeInfoNotFound
- **interface**: `api.errors.contracts.CodeInfoNotFound.is`
- **summary**:    No code info could be found at the supplied code hash. 
 
### CodeInUse
- **interface**: `api.errors.contracts.CodeInUse.is`
- **summary**:    Code removal was denied because the code is still in use by at least one contract. 
 
### CodeNotFound
- **interface**: `api.errors.contracts.CodeNotFound.is`
- **summary**:    No code could be found at the supplied code hash. 
 
### CodeRejected
- **interface**: `api.errors.contracts.CodeRejected.is`
- **summary**:    The contract's code was found to be invalid during validation. 

   The most likely cause of this is that an API was used which is not supported by the  node. This happens if an older node is used with a new version of ink!. Try updating  your node to the newest available version. 

   A more detailed error can be found on the node console if debug messages are enabled  by supplying `-lruntime::contracts=debug`. 
 
### CodeTooLarge
- **interface**: `api.errors.contracts.CodeTooLarge.is`
- **summary**:    The code supplied to `instantiate_with_code` exceeds the limit specified in the  current schedule. 
 
### ContractNotFound
- **interface**: `api.errors.contracts.ContractNotFound.is`
- **summary**:    No contract was found at the specified address. 
 
### ContractReverted
- **interface**: `api.errors.contracts.ContractReverted.is`
- **summary**:    The contract ran to completion but decided to revert its storage changes.  Please note that this error is only returned from extrinsics. When called directly  or via RPC an `Ok` will be returned. In this case the caller needs to inspect the flags  to determine whether a reversion has taken place. 
 
### ContractTrapped
- **interface**: `api.errors.contracts.ContractTrapped.is`
- **summary**:    Contract trapped during execution. 
 
### DecodingFailed
- **interface**: `api.errors.contracts.DecodingFailed.is`
- **summary**:    Input passed to a contract API function failed to decode as expected type. 
 
### DelegateDependencyAlreadyExists
- **interface**: `api.errors.contracts.DelegateDependencyAlreadyExists.is`
- **summary**:    The contract already depends on the given delegate dependency. 
 
### DelegateDependencyNotFound
- **interface**: `api.errors.contracts.DelegateDependencyNotFound.is`
- **summary**:    The dependency was not found in the contract's delegate dependencies. 
 
### DuplicateContract
- **interface**: `api.errors.contracts.DuplicateContract.is`
- **summary**:    A contract with the same AccountId already exists. 
 
### Indeterministic
- **interface**: `api.errors.contracts.Indeterministic.is`
- **summary**:    An indeterministic code was used in a context where this is not permitted. 
 
### InputForwarded
- **interface**: `api.errors.contracts.InputForwarded.is`
- **summary**:    `seal_call` forwarded this contracts input. It therefore is no longer available. 
 
### InvalidCallFlags
- **interface**: `api.errors.contracts.InvalidCallFlags.is`
- **summary**:    Invalid combination of flags supplied to `seal_call` or `seal_delegate_call`. 
 
### InvalidSchedule
- **interface**: `api.errors.contracts.InvalidSchedule.is`
- **summary**:    Invalid schedule supplied, e.g. with zero weight of a basic operation. 
 
### MaxCallDepthReached
- **interface**: `api.errors.contracts.MaxCallDepthReached.is`
- **summary**:    Performing a call was denied because the calling depth reached the limit  of what is specified in the schedule. 
 
### MaxDelegateDependenciesReached
- **interface**: `api.errors.contracts.MaxDelegateDependenciesReached.is`
- **summary**:    The contract has reached its maximum number of delegate dependencies. 
 
### MigrationInProgress
- **interface**: `api.errors.contracts.MigrationInProgress.is`
- **summary**:    A pending migration needs to complete before the extrinsic can be called. 
 
### NoChainExtension
- **interface**: `api.errors.contracts.NoChainExtension.is`
- **summary**:    The chain does not provide a chain extension. Calling the chain extension results  in this error. Note that this usually  shouldn't happen as deploying such contracts  is rejected. 
 
### NoMigrationPerformed
- **interface**: `api.errors.contracts.NoMigrationPerformed.is`
- **summary**:    Migrate dispatch call was attempted but no migration was performed. 
 
### OutOfBounds
- **interface**: `api.errors.contracts.OutOfBounds.is`
- **summary**:    A buffer outside of sandbox memory was passed to a contract API function. 
 
### OutOfGas
- **interface**: `api.errors.contracts.OutOfGas.is`
- **summary**:    The executed contract exhausted its gas limit. 
 
### OutOfTransientStorage
- **interface**: `api.errors.contracts.OutOfTransientStorage.is`
- **summary**:    Can not add more data to transient storage. 
 
### OutputBufferTooSmall
- **interface**: `api.errors.contracts.OutputBufferTooSmall.is`
- **summary**:    The output buffer supplied to a contract API call was too small. 
 
### RandomSubjectTooLong
- **interface**: `api.errors.contracts.RandomSubjectTooLong.is`
- **summary**:    The subject passed to `seal_random` exceeds the limit. 
 
### ReentranceDenied
- **interface**: `api.errors.contracts.ReentranceDenied.is`
- **summary**:    A call tried to invoke a contract that is flagged as non-reentrant.  The only other cause is that a call from a contract into the runtime tried to call back  into `pallet-contracts`. This would make the whole pallet reentrant with regard to  contract code execution which is not supported. 
 
### StateChangeDenied
- **interface**: `api.errors.contracts.StateChangeDenied.is`
- **summary**:    A contract attempted to invoke a state modifying API while being in read-only mode. 
 
### StorageDepositLimitExhausted
- **interface**: `api.errors.contracts.StorageDepositLimitExhausted.is`
- **summary**:    More storage was created than allowed by the storage deposit limit. 
 
### StorageDepositNotEnoughFunds
- **interface**: `api.errors.contracts.StorageDepositNotEnoughFunds.is`
- **summary**:    Origin doesn't have enough balance to pay the required storage deposits. 
 
### TerminatedInConstructor
- **interface**: `api.errors.contracts.TerminatedInConstructor.is`
- **summary**:    A contract self destructed in its constructor. 

   This can be triggered by a call to `seal_terminate`. 
 
### TerminatedWhileReentrant
- **interface**: `api.errors.contracts.TerminatedWhileReentrant.is`
- **summary**:    Termination of a contract is not allowed while the contract is already  on the call stack. Can be triggered by `seal_terminate`. 
 
### TooManyTopics
- **interface**: `api.errors.contracts.TooManyTopics.is`
- **summary**:    The amount of topics passed to `seal_deposit_events` exceeds the limit. 
 
### TransferFailed
- **interface**: `api.errors.contracts.TransferFailed.is`
- **summary**:    Performing the requested transfer failed. Probably because there isn't enough  free balance in the sender's account. 
 
### ValueTooLarge
- **interface**: `api.errors.contracts.ValueTooLarge.is`
- **summary**:    The size defined in `T::MaxValueSize` was exceeded. 
 
### XCMDecodeFailed
- **interface**: `api.errors.contracts.XCMDecodeFailed.is`
- **summary**:    Failed to decode the XCM program. 

___


## convictionVoting
 
### AlreadyDelegating
- **interface**: `api.errors.convictionVoting.AlreadyDelegating.is`
- **summary**:    The account is already delegating. 
 
### AlreadyVoting
- **interface**: `api.errors.convictionVoting.AlreadyVoting.is`
- **summary**:    The account currently has votes attached to it and the operation cannot succeed until  these are removed through `remove_vote`. 
 
### BadClass
- **interface**: `api.errors.convictionVoting.BadClass.is`
- **summary**:    The class ID supplied is invalid. 
 
### ClassNeeded
- **interface**: `api.errors.convictionVoting.ClassNeeded.is`
- **summary**:    The class must be supplied since it is not easily determinable from the state. 
 
### InsufficientFunds
- **interface**: `api.errors.convictionVoting.InsufficientFunds.is`
- **summary**:    Too high a balance was provided that the account cannot afford. 
 
### MaxVotesReached
- **interface**: `api.errors.convictionVoting.MaxVotesReached.is`
- **summary**:    Maximum number of votes reached. 
 
### Nonsense
- **interface**: `api.errors.convictionVoting.Nonsense.is`
- **summary**:    Delegation to oneself makes no sense. 
 
### NoPermission
- **interface**: `api.errors.convictionVoting.NoPermission.is`
- **summary**:    The actor has no permission to conduct the action. 
 
### NoPermissionYet
- **interface**: `api.errors.convictionVoting.NoPermissionYet.is`
- **summary**:    The actor has no permission to conduct the action right now but will do in the future. 
 
### NotDelegating
- **interface**: `api.errors.convictionVoting.NotDelegating.is`
- **summary**:    The account is not currently delegating. 
 
### NotOngoing
- **interface**: `api.errors.convictionVoting.NotOngoing.is`
- **summary**:    Poll is not ongoing. 
 
### NotVoter
- **interface**: `api.errors.convictionVoting.NotVoter.is`
- **summary**:    The given account did not vote on the poll. 

___


## coreFellowship
 
### AlreadyInducted
- **interface**: `api.errors.coreFellowship.AlreadyInducted.is`
- **summary**:    The candidate has already been inducted. This should never happen since it would  require a candidate (rank 0) to already be tracked in the pallet. 
 
### InvalidRank
- **interface**: `api.errors.coreFellowship.InvalidRank.is`
- **summary**:    The given rank is invalid - this generally means it's not between 1 and `RANK_COUNT`. 
 
### NoPermission
- **interface**: `api.errors.coreFellowship.NoPermission.is`
- **summary**:    The origin does not have enough permission to do this operation. 
 
### NothingDoing
- **interface**: `api.errors.coreFellowship.NothingDoing.is`
- **summary**:    No work needs to be done at present for this member. 
 
### NotTracked
- **interface**: `api.errors.coreFellowship.NotTracked.is`
- **summary**:    The candidate has not been inducted, so cannot be offboarded from this pallet. 
 
### Ranked
- **interface**: `api.errors.coreFellowship.Ranked.is`
- **summary**:    Member's rank is not zero. 
 
### TooSoon
- **interface**: `api.errors.coreFellowship.TooSoon.is`
- **summary**:    Operation cannot be done yet since not enough time has passed. 
 
### UnexpectedRank
- **interface**: `api.errors.coreFellowship.UnexpectedRank.is`
- **summary**:    Member's rank is not as expected - generally means that the rank provided to the call  does not agree with the state of the system. 
 
### Unranked
- **interface**: `api.errors.coreFellowship.Unranked.is`
- **summary**:    Member's rank is too low. 

___


## council
 
### AlreadyInitialized
- **interface**: `api.errors.council.AlreadyInitialized.is`
- **summary**:    Members are already initialized! 
 
### DuplicateProposal
- **interface**: `api.errors.council.DuplicateProposal.is`
- **summary**:    Duplicate proposals not allowed 
 
### DuplicateVote
- **interface**: `api.errors.council.DuplicateVote.is`
- **summary**:    Duplicate vote ignored 
 
### NotMember
- **interface**: `api.errors.council.NotMember.is`
- **summary**:    Account is not a member 
 
### PrimeAccountNotMember
- **interface**: `api.errors.council.PrimeAccountNotMember.is`
- **summary**:    Prime account is not a member 
 
### ProposalActive
- **interface**: `api.errors.council.ProposalActive.is`
- **summary**:    Proposal is still active. 
 
### ProposalMissing
- **interface**: `api.errors.council.ProposalMissing.is`
- **summary**:    Proposal must exist 
 
### TooEarly
- **interface**: `api.errors.council.TooEarly.is`
- **summary**:    The close call was made too early, before the end of the voting. 
 
### TooManyProposals
- **interface**: `api.errors.council.TooManyProposals.is`
- **summary**:    There can only be a maximum of `MaxProposals` active proposals. 
 
### WrongIndex
- **interface**: `api.errors.council.WrongIndex.is`
- **summary**:    Mismatched index 
 
### WrongProposalLength
- **interface**: `api.errors.council.WrongProposalLength.is`
- **summary**:    The given length bound for the proposal was too low. 
 
### WrongProposalWeight
- **interface**: `api.errors.council.WrongProposalWeight.is`
- **summary**:    The given weight bound for the proposal was too low. 

___


## delegatedStaking
 
### AlreadyStaking
- **interface**: `api.errors.delegatedStaking.AlreadyStaking.is`
- **summary**:    An existing staker cannot perform this action. 
 
### BadState
- **interface**: `api.errors.delegatedStaking.BadState.is`
- **summary**:    Some corruption in internal state. 
 
### InvalidDelegation
- **interface**: `api.errors.delegatedStaking.InvalidDelegation.is`
- **summary**:    Delegation conditions are not met. 

   Possible issues are  1) Cannot delegate to self,  2) Cannot delegate to multiple delegates. 
 
### InvalidRewardDestination
- **interface**: `api.errors.delegatedStaking.InvalidRewardDestination.is`
- **summary**:    Reward Destination cannot be same as `Agent` account. 
 
### NotAgent
- **interface**: `api.errors.delegatedStaking.NotAgent.is`
- **summary**:    Not an existing `Agent` account. 
 
### NotAllowed
- **interface**: `api.errors.delegatedStaking.NotAllowed.is`
- **summary**:    The account cannot perform this operation. 
 
### NotDelegator
- **interface**: `api.errors.delegatedStaking.NotDelegator.is`
- **summary**:    Not a Delegator account. 
 
### NotEnoughFunds
- **interface**: `api.errors.delegatedStaking.NotEnoughFunds.is`
- **summary**:    The account does not have enough funds to perform the operation. 
 
### NothingToSlash
- **interface**: `api.errors.delegatedStaking.NothingToSlash.is`
- **summary**:    `Agent` has no pending slash to be applied. 
 
### NotSupported
- **interface**: `api.errors.delegatedStaking.NotSupported.is`
- **summary**:    Operation not supported by this pallet. 
 
### UnappliedSlash
- **interface**: `api.errors.delegatedStaking.UnappliedSlash.is`
- **summary**:    Unapplied pending slash restricts operation on `Agent`. 
 
### WithdrawFailed
- **interface**: `api.errors.delegatedStaking.WithdrawFailed.is`
- **summary**:    Failed to withdraw amount from Core Staking. 

___


## democracy
 
### AlreadyCanceled
- **interface**: `api.errors.democracy.AlreadyCanceled.is`
- **summary**:    Cannot cancel the same proposal twice 
 
### AlreadyDelegating
- **interface**: `api.errors.democracy.AlreadyDelegating.is`
- **summary**:    The account is already delegating. 
 
### AlreadyVetoed
- **interface**: `api.errors.democracy.AlreadyVetoed.is`
- **summary**:    Identity may not veto a proposal twice 
 
### DuplicateProposal
- **interface**: `api.errors.democracy.DuplicateProposal.is`
- **summary**:    Proposal already made 
 
### InstantNotAllowed
- **interface**: `api.errors.democracy.InstantNotAllowed.is`
- **summary**:    The instant referendum origin is currently disallowed. 
 
### InsufficientFunds
- **interface**: `api.errors.democracy.InsufficientFunds.is`
- **summary**:    Too high a balance was provided that the account cannot afford. 
 
### InvalidHash
- **interface**: `api.errors.democracy.InvalidHash.is`
- **summary**:    Invalid hash 
 
### MaxVotesReached
- **interface**: `api.errors.democracy.MaxVotesReached.is`
- **summary**:    Maximum number of votes reached. 
 
### NoneWaiting
- **interface**: `api.errors.democracy.NoneWaiting.is`
- **summary**:    No proposals waiting 
 
### Nonsense
- **interface**: `api.errors.democracy.Nonsense.is`
- **summary**:    Delegation to oneself makes no sense. 
 
### NoPermission
- **interface**: `api.errors.democracy.NoPermission.is`
- **summary**:    The actor has no permission to conduct the action. 
 
### NoProposal
- **interface**: `api.errors.democracy.NoProposal.is`
- **summary**:    No external proposal 
 
### NotDelegating
- **interface**: `api.errors.democracy.NotDelegating.is`
- **summary**:    The account is not currently delegating. 
 
### NotSimpleMajority
- **interface**: `api.errors.democracy.NotSimpleMajority.is`
- **summary**:    Next external proposal not simple majority 
 
### NotVoter
- **interface**: `api.errors.democracy.NotVoter.is`
- **summary**:    The given account did not vote on the referendum. 
 
### PreimageNotExist
- **interface**: `api.errors.democracy.PreimageNotExist.is`
- **summary**:    The preimage does not exist. 
 
### ProposalBlacklisted
- **interface**: `api.errors.democracy.ProposalBlacklisted.is`
- **summary**:    Proposal still blacklisted 
 
### ProposalMissing
- **interface**: `api.errors.democracy.ProposalMissing.is`
- **summary**:    Proposal does not exist 
 
### ReferendumInvalid
- **interface**: `api.errors.democracy.ReferendumInvalid.is`
- **summary**:    Vote given for invalid referendum 
 
### TooMany
- **interface**: `api.errors.democracy.TooMany.is`
- **summary**:    Maximum number of items reached. 
 
### ValueLow
- **interface**: `api.errors.democracy.ValueLow.is`
- **summary**:    Value too low 
 
### VotesExist
- **interface**: `api.errors.democracy.VotesExist.is`
- **summary**:    The account currently has votes attached to it and the operation cannot succeed until  these are removed, either through `unvote` or `reap_vote`. 
 
### VotingPeriodLow
- **interface**: `api.errors.democracy.VotingPeriodLow.is`
- **summary**:    Voting period too low 
 
### WrongUpperBound
- **interface**: `api.errors.democracy.WrongUpperBound.is`
- **summary**:    Invalid upper bound. 

___


## electionProviderMultiPhase
 
### BoundNotMet
- **interface**: `api.errors.electionProviderMultiPhase.BoundNotMet.is`
- **summary**:    Some bound not met 
 
### CallNotAllowed
- **interface**: `api.errors.electionProviderMultiPhase.CallNotAllowed.is`
- **summary**:    The call is not allowed at this point. 
 
### FallbackFailed
- **interface**: `api.errors.electionProviderMultiPhase.FallbackFailed.is`
- **summary**:    The fallback failed 
 
### InvalidSubmissionIndex
- **interface**: `api.errors.electionProviderMultiPhase.InvalidSubmissionIndex.is`
- **summary**:    `Self::insert_submission` returned an invalid index. 
 
### MissingSnapshotMetadata
- **interface**: `api.errors.electionProviderMultiPhase.MissingSnapshotMetadata.is`
- **summary**:    Snapshot metadata should exist but didn't. 
 
### OcwCallWrongEra
- **interface**: `api.errors.electionProviderMultiPhase.OcwCallWrongEra.is`
- **summary**:    OCW submitted solution for wrong round 
 
### PreDispatchDifferentRound
- **interface**: `api.errors.electionProviderMultiPhase.PreDispatchDifferentRound.is`
- **summary**:    Submission was prepared for a different round. 
 
### PreDispatchEarlySubmission
- **interface**: `api.errors.electionProviderMultiPhase.PreDispatchEarlySubmission.is`
- **summary**:    Submission was too early. 
 
### PreDispatchWeakSubmission
- **interface**: `api.errors.electionProviderMultiPhase.PreDispatchWeakSubmission.is`
- **summary**:    Submission was too weak, score-wise. 
 
### PreDispatchWrongWinnerCount
- **interface**: `api.errors.electionProviderMultiPhase.PreDispatchWrongWinnerCount.is`
- **summary**:    Wrong number of winners presented. 
 
### SignedCannotPayDeposit
- **interface**: `api.errors.electionProviderMultiPhase.SignedCannotPayDeposit.is`
- **summary**:    The origin failed to pay the deposit. 
 
### SignedInvalidWitness
- **interface**: `api.errors.electionProviderMultiPhase.SignedInvalidWitness.is`
- **summary**:    Witness data to dispatchable is invalid. 
 
### SignedQueueFull
- **interface**: `api.errors.electionProviderMultiPhase.SignedQueueFull.is`
- **summary**:    The queue was full, and the solution was not better than any of the existing ones. 
 
### SignedTooMuchWeight
- **interface**: `api.errors.electionProviderMultiPhase.SignedTooMuchWeight.is`
- **summary**:    The signed submission consumes too much weight 
 
### TooManyWinners
- **interface**: `api.errors.electionProviderMultiPhase.TooManyWinners.is`
- **summary**:    Submitted solution has too many winners 

___


## elections
 
### DuplicatedCandidate
- **interface**: `api.errors.elections.DuplicatedCandidate.is`
- **summary**:    Duplicated candidate submission. 
 
### InsufficientCandidateFunds
- **interface**: `api.errors.elections.InsufficientCandidateFunds.is`
- **summary**:    Candidate does not have enough funds. 
 
### InvalidRenouncing
- **interface**: `api.errors.elections.InvalidRenouncing.is`
- **summary**:    The renouncing origin presented a wrong `Renouncing` parameter. 
 
### InvalidReplacement
- **interface**: `api.errors.elections.InvalidReplacement.is`
- **summary**:    Prediction regarding replacement after member removal is wrong. 
 
### InvalidVoteCount
- **interface**: `api.errors.elections.InvalidVoteCount.is`
- **summary**:    The provided count of number of votes is incorrect. 
 
### InvalidWitnessData
- **interface**: `api.errors.elections.InvalidWitnessData.is`
- **summary**:    The provided count of number of candidates is incorrect. 
 
### LowBalance
- **interface**: `api.errors.elections.LowBalance.is`
- **summary**:    Cannot vote with stake less than minimum balance. 
 
### MaximumVotesExceeded
- **interface**: `api.errors.elections.MaximumVotesExceeded.is`
- **summary**:    Cannot vote more than maximum allowed. 
 
### MemberSubmit
- **interface**: `api.errors.elections.MemberSubmit.is`
- **summary**:    Member cannot re-submit candidacy. 
 
### MustBeVoter
- **interface**: `api.errors.elections.MustBeVoter.is`
- **summary**:    Must be a voter. 
 
### NotMember
- **interface**: `api.errors.elections.NotMember.is`
- **summary**:    Not a member. 
 
### NoVotes
- **interface**: `api.errors.elections.NoVotes.is`
- **summary**:    Must vote for at least one candidate. 
 
### RunnerUpSubmit
- **interface**: `api.errors.elections.RunnerUpSubmit.is`
- **summary**:    Runner cannot re-submit candidacy. 
 
### TooManyCandidates
- **interface**: `api.errors.elections.TooManyCandidates.is`
- **summary**:    Too many candidates have been created. 
 
### TooManyVotes
- **interface**: `api.errors.elections.TooManyVotes.is`
- **summary**:    Cannot vote more than candidates. 
 
### UnableToPayBond
- **interface**: `api.errors.elections.UnableToPayBond.is`
- **summary**:    Voter can not pay voting bond. 
 
### UnableToVote
- **interface**: `api.errors.elections.UnableToVote.is`
- **summary**:    Cannot vote when no candidates or members exist. 

___


## fastUnstake
 
### AlreadyHead
- **interface**: `api.errors.fastUnstake.AlreadyHead.is`
- **summary**:    The provided un-staker is already in Head, and cannot deregister. 
 
### AlreadyQueued
- **interface**: `api.errors.fastUnstake.AlreadyQueued.is`
- **summary**:    The bonded account has already been queued. 
 
### CallNotAllowed
- **interface**: `api.errors.fastUnstake.CallNotAllowed.is`
- **summary**:    The call is not allowed at this point because the pallet is not active. 
 
### NotController
- **interface**: `api.errors.fastUnstake.NotController.is`
- **summary**:    The provided Controller account was not found. 

   This means that the given account is not bonded. 
 
### NotFullyBonded
- **interface**: `api.errors.fastUnstake.NotFullyBonded.is`
- **summary**:    The bonded account has active unlocking chunks. 
 
### NotQueued
- **interface**: `api.errors.fastUnstake.NotQueued.is`
- **summary**:    The provided un-staker is not in the `Queue`. 

___


## glutton
 
### AlreadyInitialized
- **interface**: `api.errors.glutton.AlreadyInitialized.is`
- **summary**:    The pallet was already initialized. 

   Set `witness_count` to `Some` to bypass this error. 
 
### InsaneLimit
- **interface**: `api.errors.glutton.InsaneLimit.is`
- **summary**:    The limit was over [`crate::RESOURCE_HARD_LIMIT`]. 

___


## grandpa
 
### ChangePending
- **interface**: `api.errors.grandpa.ChangePending.is`
- **summary**:    Attempt to signal GRANDPA change with one already pending. 
 
### DuplicateOffenceReport
- **interface**: `api.errors.grandpa.DuplicateOffenceReport.is`
- **summary**:    A given equivocation report is valid but already previously reported. 
 
### InvalidEquivocationProof
- **interface**: `api.errors.grandpa.InvalidEquivocationProof.is`
- **summary**:    An equivocation proof provided as part of an equivocation report is invalid. 
 
### InvalidKeyOwnershipProof
- **interface**: `api.errors.grandpa.InvalidKeyOwnershipProof.is`
- **summary**:    A key ownership proof provided as part of an equivocation report is invalid. 
 
### PauseFailed
- **interface**: `api.errors.grandpa.PauseFailed.is`
- **summary**:    Attempt to signal GRANDPA pause when the authority set isn't live  (either paused or already pending pause). 
 
### ResumeFailed
- **interface**: `api.errors.grandpa.ResumeFailed.is`
- **summary**:    Attempt to signal GRANDPA resume when the authority set isn't paused  (either live or already pending resume). 
 
### TooSoon
- **interface**: `api.errors.grandpa.TooSoon.is`
- **summary**:    Cannot signal forced change so soon after last. 

___


## identity
 
### AlreadyClaimed
- **interface**: `api.errors.identity.AlreadyClaimed.is`
- **summary**:    Account ID is already named. 
 
### AlreadyUnbinding
- **interface**: `api.errors.identity.AlreadyUnbinding.is`
- **summary**:    The username cannot be unbound because it is already unbinding. 
 
### EmptyIndex
- **interface**: `api.errors.identity.EmptyIndex.is`
- **summary**:    Empty index. 
 
### FeeChanged
- **interface**: `api.errors.identity.FeeChanged.is`
- **summary**:    Fee is changed. 
 
### InsufficientPrivileges
- **interface**: `api.errors.identity.InsufficientPrivileges.is`
- **summary**:    The action cannot be performed because of insufficient privileges (e.g. authority  trying to unbind a username provided by the system). 
 
### InvalidIndex
- **interface**: `api.errors.identity.InvalidIndex.is`
- **summary**:    The index is invalid. 
 
### InvalidJudgement
- **interface**: `api.errors.identity.InvalidJudgement.is`
- **summary**:    Invalid judgement. 
 
### InvalidSignature
- **interface**: `api.errors.identity.InvalidSignature.is`
- **summary**:    The signature on a username was not valid. 
 
### InvalidSuffix
- **interface**: `api.errors.identity.InvalidSuffix.is`
- **summary**:    The provided suffix is too long. 
 
### InvalidTarget
- **interface**: `api.errors.identity.InvalidTarget.is`
- **summary**:    The target is invalid. 
 
### InvalidUsername
- **interface**: `api.errors.identity.InvalidUsername.is`
- **summary**:    The username does not meet the requirements. 
 
### JudgementForDifferentIdentity
- **interface**: `api.errors.identity.JudgementForDifferentIdentity.is`
- **summary**:    The provided judgement was for a different identity. 
 
### JudgementGiven
- **interface**: `api.errors.identity.JudgementGiven.is`
- **summary**:    Judgement given. 
 
### JudgementPaymentFailed
- **interface**: `api.errors.identity.JudgementPaymentFailed.is`
- **summary**:    Error that occurs when there is an issue paying for judgement. 
 
### NoAllocation
- **interface**: `api.errors.identity.NoAllocation.is`
- **summary**:    The authority cannot allocate any more usernames. 
 
### NoIdentity
- **interface**: `api.errors.identity.NoIdentity.is`
- **summary**:    No identity found. 
 
### NotExpired
- **interface**: `api.errors.identity.NotExpired.is`
- **summary**:    The username cannot be forcefully removed because it can still be accepted. 
 
### NotFound
- **interface**: `api.errors.identity.NotFound.is`
- **summary**:    Account isn't found. 
 
### NotNamed
- **interface**: `api.errors.identity.NotNamed.is`
- **summary**:    Account isn't named. 
 
### NotOwned
- **interface**: `api.errors.identity.NotOwned.is`
- **summary**:    Sub-account isn't owned by sender. 
 
### NotSub
- **interface**: `api.errors.identity.NotSub.is`
- **summary**:    Sender is not a sub-account. 
 
### NotUnbinding
- **interface**: `api.errors.identity.NotUnbinding.is`
- **summary**:    The username cannot be removed because it is not unbinding. 
 
### NotUsernameAuthority
- **interface**: `api.errors.identity.NotUsernameAuthority.is`
- **summary**:    The sender does not have permission to issue a username. 
 
### NoUsername
- **interface**: `api.errors.identity.NoUsername.is`
- **summary**:    The requested username does not exist. 
 
### RequiresSignature
- **interface**: `api.errors.identity.RequiresSignature.is`
- **summary**:    Setting this username requires a signature, but none was provided. 
 
### StickyJudgement
- **interface**: `api.errors.identity.StickyJudgement.is`
- **summary**:    Sticky judgement. 
 
### TooEarly
- **interface**: `api.errors.identity.TooEarly.is`
- **summary**:    The username cannot be removed because it's still in the grace period. 
 
### TooManyRegistrars
- **interface**: `api.errors.identity.TooManyRegistrars.is`
- **summary**:    Maximum amount of registrars reached. Cannot add any more. 
 
### TooManySubAccounts
- **interface**: `api.errors.identity.TooManySubAccounts.is`
- **summary**:    Too many subs-accounts. 
 
### UsernameTaken
- **interface**: `api.errors.identity.UsernameTaken.is`
- **summary**:    The username is already taken. 

___


## imOnline
 
### DuplicatedHeartbeat
- **interface**: `api.errors.imOnline.DuplicatedHeartbeat.is`
- **summary**:    Duplicated heartbeat. 
 
### InvalidKey
- **interface**: `api.errors.imOnline.InvalidKey.is`
- **summary**:    Non existent public key. 

___


## indices
 
### InUse
- **interface**: `api.errors.indices.InUse.is`
- **summary**:    The index was not available. 
 
### NotAssigned
- **interface**: `api.errors.indices.NotAssigned.is`
- **summary**:    The index was not already assigned. 
 
### NotOwner
- **interface**: `api.errors.indices.NotOwner.is`
- **summary**:    The index is assigned to another account. 
 
### NotTransfer
- **interface**: `api.errors.indices.NotTransfer.is`
- **summary**:    The source and destination accounts are identical. 
 
### Permanent
- **interface**: `api.errors.indices.Permanent.is`
- **summary**:    The index is permanent and may not be freed/changed. 

___


## lottery
 
### AlreadyEnded
- **interface**: `api.errors.lottery.AlreadyEnded.is`
- **summary**:    A lottery has already ended. 
 
### AlreadyParticipating
- **interface**: `api.errors.lottery.AlreadyParticipating.is`
- **summary**:    You are already participating in the lottery with this call. 
 
### EncodingFailed
- **interface**: `api.errors.lottery.EncodingFailed.is`
- **summary**:    Failed to encode calls 
 
### InProgress
- **interface**: `api.errors.lottery.InProgress.is`
- **summary**:    A lottery is already in progress. 
 
### InvalidCall
- **interface**: `api.errors.lottery.InvalidCall.is`
- **summary**:    The call is not valid for an open lottery. 
 
### NotConfigured
- **interface**: `api.errors.lottery.NotConfigured.is`
- **summary**:    A lottery has not been configured. 
 
### TooManyCalls
- **interface**: `api.errors.lottery.TooManyCalls.is`
- **summary**:    Too many calls for a single lottery. 

___


## messageQueue
 
### AlreadyProcessed
- **interface**: `api.errors.messageQueue.AlreadyProcessed.is`
- **summary**:    The message was already processed and cannot be processed again. 
 
### InsufficientWeight
- **interface**: `api.errors.messageQueue.InsufficientWeight.is`
- **summary**:    There is temporarily not enough weight to continue servicing messages. 
 
### NoMessage
- **interface**: `api.errors.messageQueue.NoMessage.is`
- **summary**:    The referenced message could not be found. 
 
### NoPage
- **interface**: `api.errors.messageQueue.NoPage.is`
- **summary**:    Page to be reaped does not exist. 
 
### NotReapable
- **interface**: `api.errors.messageQueue.NotReapable.is`
- **summary**:    Page is not reapable because it has items remaining to be processed and is not old  enough. 
 
### Queued
- **interface**: `api.errors.messageQueue.Queued.is`
- **summary**:    The message is queued for future execution. 
 
### QueuePaused
- **interface**: `api.errors.messageQueue.QueuePaused.is`
- **summary**:    The queue is paused and no message can be executed from it. 

   This can change at any time and may resolve in the future by re-trying. 
 
### RecursiveDisallowed
- **interface**: `api.errors.messageQueue.RecursiveDisallowed.is`
- **summary**:    Another call is in progress and needs to finish before this call can happen. 
 
### TemporarilyUnprocessable
- **interface**: `api.errors.messageQueue.TemporarilyUnprocessable.is`
- **summary**:    This message is temporarily unprocessable. 

   Such errors are expected, but not guaranteed, to resolve themselves eventually through  retrying. 

___


## metaTx
 
### AncientBirthBlock
- **interface**: `api.errors.metaTx.AncientBirthBlock.is`
- **summary**:    The meta transactions's birth block is ancient. 
 
### BadProof
- **interface**: `api.errors.metaTx.BadProof.is`
- **summary**:    Invalid proof (e.g. signature). 
 
### Future
- **interface**: `api.errors.metaTx.Future.is`
- **summary**:    The meta transaction is not yet valid (e.g. nonce too high). 
 
### Invalid
- **interface**: `api.errors.metaTx.Invalid.is`
- **summary**:    The meta transaction is invalid. 
 
### Stale
- **interface**: `api.errors.metaTx.Stale.is`
- **summary**:    The meta transaction is outdated (e.g. nonce too low). 
 
### UnknownOrigin
- **interface**: `api.errors.metaTx.UnknownOrigin.is`
- **summary**:    The transaction extension did not authorize any origin. 

___


## multiBlockMigrations
 
### Ongoing
- **interface**: `api.errors.multiBlockMigrations.Ongoing.is`
- **summary**:    The operation cannot complete since some MBMs are ongoing. 

___


## multisig
 
### AlreadyApproved
- **interface**: `api.errors.multisig.AlreadyApproved.is`
- **summary**:    Call is already approved by this signatory. 
 
### AlreadyStored
- **interface**: `api.errors.multisig.AlreadyStored.is`
- **summary**:    The data to be stored is already stored. 
 
### MaxWeightTooLow
- **interface**: `api.errors.multisig.MaxWeightTooLow.is`
- **summary**:    The maximum weight information provided was too low. 
 
### MinimumThreshold
- **interface**: `api.errors.multisig.MinimumThreshold.is`
- **summary**:    Threshold must be 2 or greater. 
 
### NoApprovalsNeeded
- **interface**: `api.errors.multisig.NoApprovalsNeeded.is`
- **summary**:    Call doesn't need any (more) approvals. 
 
### NotFound
- **interface**: `api.errors.multisig.NotFound.is`
- **summary**:    Multisig operation not found in storage. 
 
### NoTimepoint
- **interface**: `api.errors.multisig.NoTimepoint.is`
- **summary**:    No timepoint was given, yet the multisig operation is already underway. 
 
### NotOwner
- **interface**: `api.errors.multisig.NotOwner.is`
- **summary**:    Only the account that originally created the multisig is able to cancel it or update  its deposits. 
 
### SenderInSignatories
- **interface**: `api.errors.multisig.SenderInSignatories.is`
- **summary**:    The sender was contained in the other signatories; it shouldn't be. 
 
### SignatoriesOutOfOrder
- **interface**: `api.errors.multisig.SignatoriesOutOfOrder.is`
- **summary**:    The signatories were provided out of order; they should be ordered. 
 
### TooFewSignatories
- **interface**: `api.errors.multisig.TooFewSignatories.is`
- **summary**:    There are too few signatories in the list. 
 
### TooManySignatories
- **interface**: `api.errors.multisig.TooManySignatories.is`
- **summary**:    There are too many signatories in the list. 
 
### UnexpectedTimepoint
- **interface**: `api.errors.multisig.UnexpectedTimepoint.is`
- **summary**:    A timepoint was given, yet no multisig operation is underway. 
 
### WrongTimepoint
- **interface**: `api.errors.multisig.WrongTimepoint.is`
- **summary**:    A different timepoint was given to the multisig operation that is underway. 

___


## nftFractionalization
 
### IncorrectAssetId
- **interface**: `api.errors.nftFractionalization.IncorrectAssetId.is`
- **summary**:    Asset ID does not correspond to locked NFT. 
 
### NftNotFound
- **interface**: `api.errors.nftFractionalization.NftNotFound.is`
- **summary**:    NFT doesn't exist. 
 
### NftNotFractionalized
- **interface**: `api.errors.nftFractionalization.NftNotFractionalized.is`
- **summary**:    NFT has not yet been fractionalised. 
 
### NoPermission
- **interface**: `api.errors.nftFractionalization.NoPermission.is`
- **summary**:    The signing account has no permission to do the operation. 

___


## nfts
 
### AlreadyClaimed
- **interface**: `api.errors.nfts.AlreadyClaimed.is`
- **summary**:    The provided Item was already used for claiming. 
 
### AlreadyExists
- **interface**: `api.errors.nfts.AlreadyExists.is`
- **summary**:    The item ID has already been used for an item. 
 
### ApprovalExpired
- **interface**: `api.errors.nfts.ApprovalExpired.is`
- **summary**:    The approval had a deadline that expired, so the approval isn't valid anymore. 
 
### AttributeNotFound
- **interface**: `api.errors.nfts.AttributeNotFound.is`
- **summary**:    The provided attribute can't be found. 
 
### BadWitness
- **interface**: `api.errors.nfts.BadWitness.is`
- **summary**:    The witness data given does not match the current state of the chain. 
 
### BidTooLow
- **interface**: `api.errors.nfts.BidTooLow.is`
- **summary**:    The provided bid is too low. 
 
### CollectionIdInUse
- **interface**: `api.errors.nfts.CollectionIdInUse.is`
- **summary**:    Collection ID is already taken. 
 
### CollectionNotEmpty
- **interface**: `api.errors.nfts.CollectionNotEmpty.is`
- **summary**:    Can't delete non-empty collections. 
 
### DeadlineExpired
- **interface**: `api.errors.nfts.DeadlineExpired.is`
- **summary**:    The deadline has already expired. 
 
### InconsistentItemConfig
- **interface**: `api.errors.nfts.InconsistentItemConfig.is`
- **summary**:    Item's config already exists and should be equal to the provided one. 
 
### IncorrectData
- **interface**: `api.errors.nfts.IncorrectData.is`
- **summary**:    The provided data is incorrect. 
 
### IncorrectMetadata
- **interface**: `api.errors.nfts.IncorrectMetadata.is`
- **summary**:    The provided metadata might be too long. 
 
### ItemLocked
- **interface**: `api.errors.nfts.ItemLocked.is`
- **summary**:    The item is locked (non-transferable). 
 
### ItemsNonTransferable
- **interface**: `api.errors.nfts.ItemsNonTransferable.is`
- **summary**:    Items within that collection are non-transferable. 
 
### LockedCollectionAttributes
- **interface**: `api.errors.nfts.LockedCollectionAttributes.is`
- **summary**:    Collection's attributes are locked. 
 
### LockedCollectionMetadata
- **interface**: `api.errors.nfts.LockedCollectionMetadata.is`
- **summary**:    Collection's metadata is locked. 
 
### LockedItemAttributes
- **interface**: `api.errors.nfts.LockedItemAttributes.is`
- **summary**:    Item's attributes are locked. 
 
### LockedItemMetadata
- **interface**: `api.errors.nfts.LockedItemMetadata.is`
- **summary**:    Item's metadata is locked. 
 
### MaxAttributesLimitReached
- **interface**: `api.errors.nfts.MaxAttributesLimitReached.is`
- **summary**:    Can't set more attributes per one call. 
 
### MaxSupplyLocked
- **interface**: `api.errors.nfts.MaxSupplyLocked.is`
- **summary**:    The max supply is locked and can't be changed. 
 
### MaxSupplyReached
- **interface**: `api.errors.nfts.MaxSupplyReached.is`
- **summary**:    All items have been minted. 
 
### MaxSupplyTooSmall
- **interface**: `api.errors.nfts.MaxSupplyTooSmall.is`
- **summary**:    The provided max supply is less than the number of items a collection already has. 
 
### MetadataNotFound
- **interface**: `api.errors.nfts.MetadataNotFound.is`
- **summary**:    The given item has no metadata set. 
 
### MethodDisabled
- **interface**: `api.errors.nfts.MethodDisabled.is`
- **summary**:    The method is disabled by system settings. 
 
### MintEnded
- **interface**: `api.errors.nfts.MintEnded.is`
- **summary**:    Mint has already ended. 
 
### MintNotStarted
- **interface**: `api.errors.nfts.MintNotStarted.is`
- **summary**:    Mint has not started yet. 
 
### NoConfig
- **interface**: `api.errors.nfts.NoConfig.is`
- **summary**:    Config for a collection or an item can't be found. 
 
### NoPermission
- **interface**: `api.errors.nfts.NoPermission.is`
- **summary**:    The signing account has no permission to do the operation. 
 
### NotDelegate
- **interface**: `api.errors.nfts.NotDelegate.is`
- **summary**:    The provided account is not a delegate. 
 
### NotForSale
- **interface**: `api.errors.nfts.NotForSale.is`
- **summary**:    Item is not for sale. 
 
### ReachedApprovalLimit
- **interface**: `api.errors.nfts.ReachedApprovalLimit.is`
- **summary**:    The item has reached its approval limit. 
 
### RolesNotCleared
- **interface**: `api.errors.nfts.RolesNotCleared.is`
- **summary**:    Some roles were not cleared. 
 
### Unaccepted
- **interface**: `api.errors.nfts.Unaccepted.is`
- **summary**:    The named owner has not signed ownership acceptance of the collection. 
 
### Unapproved
- **interface**: `api.errors.nfts.Unapproved.is`
- **summary**:    No approval exists that would allow the transfer. 
 
### UnknownCollection
- **interface**: `api.errors.nfts.UnknownCollection.is`
- **summary**:    The given item ID is unknown. 
 
### UnknownItem
- **interface**: `api.errors.nfts.UnknownItem.is`
- **summary**:    The given item ID is unknown. 
 
### UnknownSwap
- **interface**: `api.errors.nfts.UnknownSwap.is`
- **summary**:    Swap doesn't exist. 
 
### WitnessRequired
- **interface**: `api.errors.nfts.WitnessRequired.is`
- **summary**:    The witness data should be provided. 
 
### WrongDelegate
- **interface**: `api.errors.nfts.WrongDelegate.is`
- **summary**:    The delegate turned out to be different to what was expected. 
 
### WrongDuration
- **interface**: `api.errors.nfts.WrongDuration.is`
- **summary**:    The duration provided should be less than or equal to `MaxDeadlineDuration`. 
 
### WrongNamespace
- **interface**: `api.errors.nfts.WrongNamespace.is`
- **summary**:    The provided namespace isn't supported in this call. 
 
### WrongOrigin
- **interface**: `api.errors.nfts.WrongOrigin.is`
- **summary**:    The extrinsic was sent by the wrong origin. 
 
### WrongOwner
- **interface**: `api.errors.nfts.WrongOwner.is`
- **summary**:    The owner turned out to be different to what was expected. 
 
### WrongSetting
- **interface**: `api.errors.nfts.WrongSetting.is`
- **summary**:    The provided setting can't be set. 
 
### WrongSignature
- **interface**: `api.errors.nfts.WrongSignature.is`
- **summary**:    The provided signature is incorrect. 

___


## nis
 
### AlreadyCommunal
- **interface**: `api.errors.nis.AlreadyCommunal.is`
- **summary**:    The receipt is already communal. 
 
### AlreadyFunded
- **interface**: `api.errors.nis.AlreadyFunded.is`
- **summary**:    There are enough funds for what is required. 
 
### AlreadyPrivate
- **interface**: `api.errors.nis.AlreadyPrivate.is`
- **summary**:    The receipt is already private. 
 
### AmountTooSmall
- **interface**: `api.errors.nis.AmountTooSmall.is`
- **summary**:    The amount of the bid is less than the minimum allowed. 
 
### BidTooLow
- **interface**: `api.errors.nis.BidTooLow.is`
- **summary**:    The queue for the bid's duration is full and the amount bid is too low to get in  through replacing an existing bid. 
 
### DurationTooBig
- **interface**: `api.errors.nis.DurationTooBig.is`
- **summary**:    The duration is the bid is greater than the number of queues. 
 
### DurationTooSmall
- **interface**: `api.errors.nis.DurationTooSmall.is`
- **summary**:    The duration of the bid is less than one. 
 
### MakesDust
- **interface**: `api.errors.nis.MakesDust.is`
- **summary**:    The operation would result in a receipt worth an insignificant value. 
 
### NotExpired
- **interface**: `api.errors.nis.NotExpired.is`
- **summary**:    Bond not yet at expiry date. 
 
### NotOwner
- **interface**: `api.errors.nis.NotOwner.is`
- **summary**:    Not the owner of the receipt. 
 
### PortionTooBig
- **interface**: `api.errors.nis.PortionTooBig.is`
- **summary**:    The portion supplied is beyond the value of the receipt. 
 
### Throttled
- **interface**: `api.errors.nis.Throttled.is`
- **summary**:    The thaw throttle has been reached for this period. 
 
### Unfunded
- **interface**: `api.errors.nis.Unfunded.is`
- **summary**:    Not enough funds are held to pay out. 
 
### UnknownBid
- **interface**: `api.errors.nis.UnknownBid.is`
- **summary**:    The given bid for retraction is not found. 
 
### UnknownReceipt
- **interface**: `api.errors.nis.UnknownReceipt.is`
- **summary**:    Receipt index is unknown. 

___


## nominationPools
 
### AccountBelongsToOtherPool
- **interface**: `api.errors.nominationPools.AccountBelongsToOtherPool.is`
- **summary**:    An account is already delegating in another pool. An account may only belong to one  pool at a time. 
 
### AlreadyMigrated
- **interface**: `api.errors.nominationPools.AlreadyMigrated.is`
- **summary**:    The pool or member delegation has already migrated to delegate stake. 
 
### BondExtraRestricted
- **interface**: `api.errors.nominationPools.BondExtraRestricted.is`
- **summary**:    Bonding extra is restricted to the exact pending reward amount. 
 
### CanNotChangeState
- **interface**: `api.errors.nominationPools.CanNotChangeState.is`
- **summary**:    The pools state cannot be changed. 
 
### CannotWithdrawAny
- **interface**: `api.errors.nominationPools.CannotWithdrawAny.is`
- **summary**:    None of the funds can be withdrawn yet because the bonding duration has not passed. 
 
### CommissionChangeRateNotAllowed
- **interface**: `api.errors.nominationPools.CommissionChangeRateNotAllowed.is`
- **summary**:    The submitted changes to commission change rate are not allowed. 
 
### CommissionChangeThrottled
- **interface**: `api.errors.nominationPools.CommissionChangeThrottled.is`
- **summary**:    Not enough blocks have surpassed since the last commission update. 
 
### CommissionExceedsGlobalMaximum
- **interface**: `api.errors.nominationPools.CommissionExceedsGlobalMaximum.is`
- **summary**:    The supplied commission exceeds global maximum commission. 
 
### CommissionExceedsMaximum
- **interface**: `api.errors.nominationPools.CommissionExceedsMaximum.is`
- **summary**:    The supplied commission exceeds the max allowed commission. 
 
### Defensive
- **interface**: `api.errors.nominationPools.Defensive.is`
- **summary**:    Some error occurred that should never happen. This should be reported to the  maintainers. 
 
### DoesNotHavePermission
- **interface**: `api.errors.nominationPools.DoesNotHavePermission.is`
- **summary**:    The caller does not have adequate permissions. 
 
### FullyUnbonding
- **interface**: `api.errors.nominationPools.FullyUnbonding.is`
- **summary**:    The member is fully unbonded (and thus cannot access the bonded and reward pool  anymore to, for example, collect rewards). 
 
### InvalidPoolId
- **interface**: `api.errors.nominationPools.InvalidPoolId.is`
- **summary**:    Pool id provided is not correct/usable. 
 
### MaxCommissionRestricted
- **interface**: `api.errors.nominationPools.MaxCommissionRestricted.is`
- **summary**:    The pool's max commission cannot be set higher than the existing value. 
 
### MaxPoolMembers
- **interface**: `api.errors.nominationPools.MaxPoolMembers.is`
- **summary**:    Too many members in the pool or system. 
 
### MaxPools
- **interface**: `api.errors.nominationPools.MaxPools.is`
- **summary**:    The system is maxed out on pools. 
 
### MaxUnbondingLimit
- **interface**: `api.errors.nominationPools.MaxUnbondingLimit.is`
- **summary**:    The member cannot unbond further chunks due to reaching the limit. 
 
### MetadataExceedsMaxLen
- **interface**: `api.errors.nominationPools.MetadataExceedsMaxLen.is`
- **summary**:    Metadata exceeds [`Config::MaxMetadataLen`] 
 
### MinimumBondNotMet
- **interface**: `api.errors.nominationPools.MinimumBondNotMet.is`
- **summary**:    The amount does not meet the minimum bond to either join or create a pool. 

   The depositor can never unbond to a value less than `Pallet::depositor_min_bond`. The  caller does not have nominating permissions for the pool. Members can never unbond to a  value below `MinJoinBond`. 
 
### NoCommissionCurrentSet
- **interface**: `api.errors.nominationPools.NoCommissionCurrentSet.is`
- **summary**:    No commission current has been set. 
 
### NoPendingCommission
- **interface**: `api.errors.nominationPools.NoPendingCommission.is`
- **summary**:    There is no pending commission to claim. 
 
### NotDestroying
- **interface**: `api.errors.nominationPools.NotDestroying.is`
- **summary**:    A pool must be in [`PoolState::Destroying`] in order for the depositor to unbond or for  other members to be permissionlessly unbonded. 
 
### NothingToAdjust
- **interface**: `api.errors.nominationPools.NothingToAdjust.is`
- **summary**:    No imbalance in the ED deposit for the pool. 
 
### NothingToSlash
- **interface**: `api.errors.nominationPools.NothingToSlash.is`
- **summary**:    No slash pending that can be applied to the member. 
 
### NotKickerOrDestroying
- **interface**: `api.errors.nominationPools.NotKickerOrDestroying.is`
- **summary**:    Either a) the caller cannot make a valid kick or b) the pool is not destroying. 
 
### NotMigrated
- **interface**: `api.errors.nominationPools.NotMigrated.is`
- **summary**:    The pool or member delegation has not migrated yet to delegate stake. 
 
### NotNominator
- **interface**: `api.errors.nominationPools.NotNominator.is`
- **summary**:    The caller does not have nominating permissions for the pool. 
 
### NotOpen
- **interface**: `api.errors.nominationPools.NotOpen.is`
- **summary**:    The pool is not open to join 
 
### NotSupported
- **interface**: `api.errors.nominationPools.NotSupported.is`
- **summary**:    This call is not allowed in the current state of the pallet. 
 
### OverflowRisk
- **interface**: `api.errors.nominationPools.OverflowRisk.is`
- **summary**:    The transaction could not be executed due to overflow risk for the pool. 
 
### PartialUnbondNotAllowedPermissionlessly
- **interface**: `api.errors.nominationPools.PartialUnbondNotAllowedPermissionlessly.is`
- **summary**:    Partial unbonding now allowed permissionlessly. 
 
### PoolIdInUse
- **interface**: `api.errors.nominationPools.PoolIdInUse.is`
- **summary**:    Pool id currently in use. 
 
### PoolMemberNotFound
- **interface**: `api.errors.nominationPools.PoolMemberNotFound.is`
- **summary**:    An account is not a member. 
 
### PoolNotFound
- **interface**: `api.errors.nominationPools.PoolNotFound.is`
- **summary**:    A (bonded) pool id does not exist. 
 
### Restricted
- **interface**: `api.errors.nominationPools.Restricted.is`
- **summary**:    Account is restricted from participation in pools. This may happen if the account is  staking in another way already. 
 
### RewardPoolNotFound
- **interface**: `api.errors.nominationPools.RewardPoolNotFound.is`
- **summary**:    A reward pool does not exist. In all cases this is a system logic error. 
 
### SlashTooLow
- **interface**: `api.errors.nominationPools.SlashTooLow.is`
- **summary**:    The slash amount is too low to be applied. 
 
### SubPoolsNotFound
- **interface**: `api.errors.nominationPools.SubPoolsNotFound.is`
- **summary**:    A sub pool does not exist. 

___


## poolAssets
 
### AlreadyExists
- **interface**: `api.errors.poolAssets.AlreadyExists.is`
- **summary**:    The asset-account already exists. 
 
### AssetNotLive
- **interface**: `api.errors.poolAssets.AssetNotLive.is`
- **summary**:    The asset is not live, and likely being destroyed. 
 
### BadAssetId
- **interface**: `api.errors.poolAssets.BadAssetId.is`
- **summary**:    The asset ID must be equal to the [`NextAssetId`]. 
 
### BadMetadata
- **interface**: `api.errors.poolAssets.BadMetadata.is`
- **summary**:    Invalid metadata given. 
 
### BadWitness
- **interface**: `api.errors.poolAssets.BadWitness.is`
- **summary**:    Invalid witness data given. 
 
### BalanceLow
- **interface**: `api.errors.poolAssets.BalanceLow.is`
- **summary**:    Account balance must be greater than or equal to the transfer amount. 
 
### CallbackFailed
- **interface**: `api.errors.poolAssets.CallbackFailed.is`
- **summary**:    Callback action resulted in error 
 
### ContainsFreezes
- **interface**: `api.errors.poolAssets.ContainsFreezes.is`
- **summary**:    The asset cannot be destroyed because some accounts for this asset contain freezes. 
 
### ContainsHolds
- **interface**: `api.errors.poolAssets.ContainsHolds.is`
- **summary**:    The asset cannot be destroyed because some accounts for this asset contain holds. 
 
### Frozen
- **interface**: `api.errors.poolAssets.Frozen.is`
- **summary**:    The origin account is frozen. 
 
### IncorrectStatus
- **interface**: `api.errors.poolAssets.IncorrectStatus.is`
- **summary**:    The asset status is not the expected status. 
 
### InUse
- **interface**: `api.errors.poolAssets.InUse.is`
- **summary**:    The asset ID is already taken. 
 
### LiveAsset
- **interface**: `api.errors.poolAssets.LiveAsset.is`
- **summary**:    The asset is a live asset and is actively being used. Usually emit for operations such  as `start_destroy` which require the asset to be in a destroying state. 
 
### MinBalanceZero
- **interface**: `api.errors.poolAssets.MinBalanceZero.is`
- **summary**:    Minimum balance should be non-zero. 
 
### NoAccount
- **interface**: `api.errors.poolAssets.NoAccount.is`
- **summary**:    The account to alter does not exist. 
 
### NoDeposit
- **interface**: `api.errors.poolAssets.NoDeposit.is`
- **summary**:    The asset-account doesn't have an associated deposit. 
 
### NoPermission
- **interface**: `api.errors.poolAssets.NoPermission.is`
- **summary**:    The signing account has no permission to do the operation. 
 
### NotFrozen
- **interface**: `api.errors.poolAssets.NotFrozen.is`
- **summary**:    The asset should be frozen before the given operation. 
 
### Unapproved
- **interface**: `api.errors.poolAssets.Unapproved.is`
- **summary**:    No approval exists that would allow the transfer. 
 
### UnavailableConsumer
- **interface**: `api.errors.poolAssets.UnavailableConsumer.is`
- **summary**:    Unable to increment the consumer reference counters on the account. Either no provider  reference exists to allow a non-zero balance of a non-self-sufficient asset, or one  fewer then the maximum number of consumers has been reached. 
 
### Unknown
- **interface**: `api.errors.poolAssets.Unknown.is`
- **summary**:    The given asset ID is unknown. 
 
### WouldBurn
- **interface**: `api.errors.poolAssets.WouldBurn.is`
- **summary**:    The operation would result in funds being burned. 
 
### WouldDie
- **interface**: `api.errors.poolAssets.WouldDie.is`
- **summary**:    The source account would not survive the transfer and it needs to stay alive. 

___


## preimage
 
### AlreadyNoted
- **interface**: `api.errors.preimage.AlreadyNoted.is`
- **summary**:    Preimage has already been noted on-chain. 
 
### NotAuthorized
- **interface**: `api.errors.preimage.NotAuthorized.is`
- **summary**:    The user is not authorized to perform this action. 
 
### NotNoted
- **interface**: `api.errors.preimage.NotNoted.is`
- **summary**:    The preimage cannot be removed since it has not yet been noted. 
 
### NotRequested
- **interface**: `api.errors.preimage.NotRequested.is`
- **summary**:    The preimage request cannot be removed since no outstanding requests exist. 
 
### Requested
- **interface**: `api.errors.preimage.Requested.is`
- **summary**:    A preimage may not be removed when there are outstanding requests. 
 
### TooBig
- **interface**: `api.errors.preimage.TooBig.is`
- **summary**:    Preimage is too large to store on-chain. 
 
### TooFew
- **interface**: `api.errors.preimage.TooFew.is`
- **summary**:    Too few hashes were requested to be upgraded (i.e. zero). 
 
### TooMany
- **interface**: `api.errors.preimage.TooMany.is`
- **summary**:    More than `MAX_HASH_UPGRADE_BULK_COUNT` hashes were requested to be upgraded at once. 

___


## proxy
 
### Duplicate
- **interface**: `api.errors.proxy.Duplicate.is`
- **summary**:    Account is already a proxy. 
 
### NoPermission
- **interface**: `api.errors.proxy.NoPermission.is`
- **summary**:    Call may not be made by proxy because it may escalate its privileges. 
 
### NoSelfProxy
- **interface**: `api.errors.proxy.NoSelfProxy.is`
- **summary**:    Cannot add self as proxy. 
 
### NotFound
- **interface**: `api.errors.proxy.NotFound.is`
- **summary**:    Proxy registration not found. 
 
### NotProxy
- **interface**: `api.errors.proxy.NotProxy.is`
- **summary**:    Sender is not a proxy of the account to be proxied. 
 
### TooMany
- **interface**: `api.errors.proxy.TooMany.is`
- **summary**:    There are too many proxies registered or too many announcements pending. 
 
### Unannounced
- **interface**: `api.errors.proxy.Unannounced.is`
- **summary**:    Announcement, if made at all, was made too recently. 
 
### Unproxyable
- **interface**: `api.errors.proxy.Unproxyable.is`
- **summary**:    A call which is incompatible with the proxy type's filter was attempted. 

___


## rankedCollective
 
### AlreadyMember
- **interface**: `api.errors.rankedCollective.AlreadyMember.is`
- **summary**:    Account is already a member. 
 
### Corruption
- **interface**: `api.errors.rankedCollective.Corruption.is`
- **summary**:    Unexpected error in state. 
 
### InvalidWitness
- **interface**: `api.errors.rankedCollective.InvalidWitness.is`
- **summary**:    The information provided is incorrect. 
 
### NoneRemaining
- **interface**: `api.errors.rankedCollective.NoneRemaining.is`
- **summary**:    There are no further records to be removed. 
 
### NoPermission
- **interface**: `api.errors.rankedCollective.NoPermission.is`
- **summary**:    The origin is not sufficiently privileged to do the operation. 
 
### NotMember
- **interface**: `api.errors.rankedCollective.NotMember.is`
- **summary**:    Account is not a member. 
 
### NotPolling
- **interface**: `api.errors.rankedCollective.NotPolling.is`
- **summary**:    The given poll index is unknown or has closed. 
 
### Ongoing
- **interface**: `api.errors.rankedCollective.Ongoing.is`
- **summary**:    The given poll is still ongoing. 
 
### RankTooLow
- **interface**: `api.errors.rankedCollective.RankTooLow.is`
- **summary**:    The member's rank is too low to vote. 
 
### SameMember
- **interface**: `api.errors.rankedCollective.SameMember.is`
- **summary**:    The new member to exchange is the same as the old member 
 
### TooManyMembers
- **interface**: `api.errors.rankedCollective.TooManyMembers.is`
- **summary**:    The max member count for the rank has been reached. 

___


## rankedPolls
 
### BadReferendum
- **interface**: `api.errors.rankedPolls.BadReferendum.is`
- **summary**:    The referendum index provided is invalid in this context. 
 
### BadStatus
- **interface**: `api.errors.rankedPolls.BadStatus.is`
- **summary**:    The referendum status is invalid for this operation. 
 
### BadTrack
- **interface**: `api.errors.rankedPolls.BadTrack.is`
- **summary**:    The track identifier given was invalid. 
 
### Full
- **interface**: `api.errors.rankedPolls.Full.is`
- **summary**:    There are already a full complement of referenda in progress for this track. 
 
### HasDeposit
- **interface**: `api.errors.rankedPolls.HasDeposit.is`
- **summary**:    Referendum's decision deposit is already paid. 
 
### NoDeposit
- **interface**: `api.errors.rankedPolls.NoDeposit.is`
- **summary**:    The deposit cannot be refunded since none was made. 
 
### NoPermission
- **interface**: `api.errors.rankedPolls.NoPermission.is`
- **summary**:    The deposit refunder is not the depositor. 
 
### NothingToDo
- **interface**: `api.errors.rankedPolls.NothingToDo.is`
- **summary**:    There was nothing to do in the advancement. 
 
### NotOngoing
- **interface**: `api.errors.rankedPolls.NotOngoing.is`
- **summary**:    Referendum is not ongoing. 
 
### NoTrack
- **interface**: `api.errors.rankedPolls.NoTrack.is`
- **summary**:    No track exists for the proposal origin. 
 
### PreimageNotExist
- **interface**: `api.errors.rankedPolls.PreimageNotExist.is`
- **summary**:    The preimage does not exist. 
 
### PreimageStoredWithDifferentLength
- **interface**: `api.errors.rankedPolls.PreimageStoredWithDifferentLength.is`
- **summary**:    The preimage is stored with a different length than the one provided. 
 
### QueueEmpty
- **interface**: `api.errors.rankedPolls.QueueEmpty.is`
- **summary**:    The queue of the track is empty. 
 
### Unfinished
- **interface**: `api.errors.rankedPolls.Unfinished.is`
- **summary**:    Any deposit cannot be refunded until after the decision is over. 

___


## recovery
 
### AlreadyProxy
- **interface**: `api.errors.recovery.AlreadyProxy.is`
- **summary**:    This account is already set up for recovery 
 
### AlreadyRecoverable
- **interface**: `api.errors.recovery.AlreadyRecoverable.is`
- **summary**:    This account is already set up for recovery 
 
### AlreadyStarted
- **interface**: `api.errors.recovery.AlreadyStarted.is`
- **summary**:    A recovery process has already started for this account 
 
### AlreadyVouched
- **interface**: `api.errors.recovery.AlreadyVouched.is`
- **summary**:    This user has already vouched for this recovery 
 
### BadState
- **interface**: `api.errors.recovery.BadState.is`
- **summary**:    Some internal state is broken. 
 
### DelayPeriod
- **interface**: `api.errors.recovery.DelayPeriod.is`
- **summary**:    The friend must wait until the delay period to vouch for this recovery 
 
### MaxFriends
- **interface**: `api.errors.recovery.MaxFriends.is`
- **summary**:    Friends list must be less than max friends 
 
### NotAllowed
- **interface**: `api.errors.recovery.NotAllowed.is`
- **summary**:    User is not allowed to make a call on behalf of this account 
 
### NotEnoughFriends
- **interface**: `api.errors.recovery.NotEnoughFriends.is`
- **summary**:    Friends list must be greater than zero and threshold 
 
### NotFriend
- **interface**: `api.errors.recovery.NotFriend.is`
- **summary**:    This account is not a friend who can vouch 
 
### NotRecoverable
- **interface**: `api.errors.recovery.NotRecoverable.is`
- **summary**:    This account is not set up for recovery 
 
### NotSorted
- **interface**: `api.errors.recovery.NotSorted.is`
- **summary**:    Friends list must be sorted and free of duplicates 
 
### NotStarted
- **interface**: `api.errors.recovery.NotStarted.is`
- **summary**:    A recovery process has not started for this rescuer 
 
### StillActive
- **interface**: `api.errors.recovery.StillActive.is`
- **summary**:    There are still active recovery attempts that need to be closed 
 
### Threshold
- **interface**: `api.errors.recovery.Threshold.is`
- **summary**:    The threshold for recovering this account has not been met 
 
### ZeroThreshold
- **interface**: `api.errors.recovery.ZeroThreshold.is`
- **summary**:    Threshold must be greater than zero 

___


## referenda
 
### BadReferendum
- **interface**: `api.errors.referenda.BadReferendum.is`
- **summary**:    The referendum index provided is invalid in this context. 
 
### BadStatus
- **interface**: `api.errors.referenda.BadStatus.is`
- **summary**:    The referendum status is invalid for this operation. 
 
### BadTrack
- **interface**: `api.errors.referenda.BadTrack.is`
- **summary**:    The track identifier given was invalid. 
 
### Full
- **interface**: `api.errors.referenda.Full.is`
- **summary**:    There are already a full complement of referenda in progress for this track. 
 
### HasDeposit
- **interface**: `api.errors.referenda.HasDeposit.is`
- **summary**:    Referendum's decision deposit is already paid. 
 
### NoDeposit
- **interface**: `api.errors.referenda.NoDeposit.is`
- **summary**:    The deposit cannot be refunded since none was made. 
 
### NoPermission
- **interface**: `api.errors.referenda.NoPermission.is`
- **summary**:    The deposit refunder is not the depositor. 
 
### NothingToDo
- **interface**: `api.errors.referenda.NothingToDo.is`
- **summary**:    There was nothing to do in the advancement. 
 
### NotOngoing
- **interface**: `api.errors.referenda.NotOngoing.is`
- **summary**:    Referendum is not ongoing. 
 
### NoTrack
- **interface**: `api.errors.referenda.NoTrack.is`
- **summary**:    No track exists for the proposal origin. 
 
### PreimageNotExist
- **interface**: `api.errors.referenda.PreimageNotExist.is`
- **summary**:    The preimage does not exist. 
 
### PreimageStoredWithDifferentLength
- **interface**: `api.errors.referenda.PreimageStoredWithDifferentLength.is`
- **summary**:    The preimage is stored with a different length than the one provided. 
 
### QueueEmpty
- **interface**: `api.errors.referenda.QueueEmpty.is`
- **summary**:    The queue of the track is empty. 
 
### Unfinished
- **interface**: `api.errors.referenda.Unfinished.is`
- **summary**:    Any deposit cannot be refunded until after the decision is over. 

___


## remark
 
### BadContext
- **interface**: `api.errors.remark.BadContext.is`
- **summary**:    Attempted to call `store` outside of block execution. 
 
### Empty
- **interface**: `api.errors.remark.Empty.is`
- **summary**:    Attempting to store empty data. 

___


## revive
 
### AccountAlreadyMapped
- **interface**: `api.errors.revive.AccountAlreadyMapped.is`
- **summary**:    Tried to map an account that is already mapped. 
 
### AccountUnmapped
- **interface**: `api.errors.revive.AccountUnmapped.is`
- **summary**:    An `AccountID32` account tried to interact with the pallet without having a mapping. 

   Call [`Pallet::map_account`] in order to create a mapping for the account. 
 
### BalanceConversionFailed
- **interface**: `api.errors.revive.BalanceConversionFailed.is`
- **summary**:    Failed to convert a U256 to a Balance. 
 
### BasicBlockTooLarge
- **interface**: `api.errors.revive.BasicBlockTooLarge.is`
- **summary**:    The program contains a basic block that is larger than allowed. 
 
### BlobTooLarge
- **interface**: `api.errors.revive.BlobTooLarge.is`
- **summary**:    The code blob supplied is larger than [`limits::code::BLOB_BYTES`]. 
 
### CannotAddSelfAsDelegateDependency
- **interface**: `api.errors.revive.CannotAddSelfAsDelegateDependency.is`
- **summary**:    Can not add a delegate dependency to the code hash of the contract itself. 
 
### CodeInfoNotFound
- **interface**: `api.errors.revive.CodeInfoNotFound.is`
- **summary**:    No code info could be found at the supplied code hash. 
 
### CodeInUse
- **interface**: `api.errors.revive.CodeInUse.is`
- **summary**:    Code removal was denied because the code is still in use by at least one contract. 
 
### CodeNotFound
- **interface**: `api.errors.revive.CodeNotFound.is`
- **summary**:    No code could be found at the supplied code hash. 
 
### CodeRejected
- **interface**: `api.errors.revive.CodeRejected.is`
- **summary**:    The contract failed to compile or is missing the correct entry points. 

   A more detailed error can be found on the node console if debug messages are enabled  by supplying `-lruntime::revive=debug`. 
 
### ContractNotFound
- **interface**: `api.errors.revive.ContractNotFound.is`
- **summary**:    No contract was found at the specified address. 
 
### ContractReverted
- **interface**: `api.errors.revive.ContractReverted.is`
- **summary**:    The contract ran to completion but decided to revert its storage changes.  Please note that this error is only returned from extrinsics. When called directly  or via RPC an `Ok` will be returned. In this case the caller needs to inspect the flags  to determine whether a reversion has taken place. 
 
### ContractTrapped
- **interface**: `api.errors.revive.ContractTrapped.is`
- **summary**:    Contract trapped during execution. 
 
### DecimalPrecisionLoss
- **interface**: `api.errors.revive.DecimalPrecisionLoss.is`
- **summary**:    Failed to convert an EVM balance to a native balance. 
 
### DecodingFailed
- **interface**: `api.errors.revive.DecodingFailed.is`
- **summary**:    Input passed to a contract API function failed to decode as expected type. 
 
### DelegateDependencyAlreadyExists
- **interface**: `api.errors.revive.DelegateDependencyAlreadyExists.is`
- **summary**:    The contract already depends on the given delegate dependency. 
 
### DelegateDependencyNotFound
- **interface**: `api.errors.revive.DelegateDependencyNotFound.is`
- **summary**:    The dependency was not found in the contract's delegate dependencies. 
 
### DuplicateContract
- **interface**: `api.errors.revive.DuplicateContract.is`
- **summary**:    A contract with the same AccountId already exists. 
 
### ExecutionFailed
- **interface**: `api.errors.revive.ExecutionFailed.is`
- **summary**:    PolkaVM failed during code execution. Probably due to a malformed program. 
 
### InputForwarded
- **interface**: `api.errors.revive.InputForwarded.is`
- **summary**:    `seal_call` forwarded this contracts input. It therefore is no longer available. 
 
### InvalidCallFlags
- **interface**: `api.errors.revive.InvalidCallFlags.is`
- **summary**:    Invalid combination of flags supplied to `seal_call` or `seal_delegate_call`. 
 
### InvalidGenericTransaction
- **interface**: `api.errors.revive.InvalidGenericTransaction.is`
- **summary**:    The transaction used to dry-run a contract is invalid. 
 
### InvalidImmutableAccess
- **interface**: `api.errors.revive.InvalidImmutableAccess.is`
- **summary**:    Immutable data can only be set during deploys and only be read during calls.  Additionally, it is only valid to set the data once and it must not be empty. 
 
### InvalidInstruction
- **interface**: `api.errors.revive.InvalidInstruction.is`
- **summary**:    The program contains an invalid instruction. 
 
### InvalidSchedule
- **interface**: `api.errors.revive.InvalidSchedule.is`
- **summary**:    Invalid schedule supplied, e.g. with zero weight of a basic operation. 
 
### InvalidStorageFlags
- **interface**: `api.errors.revive.InvalidStorageFlags.is`
- **summary**:    Invalid storage flags were passed to one of the storage syscalls. 
 
### InvalidSyscall
- **interface**: `api.errors.revive.InvalidSyscall.is`
- **summary**:    The contract tried to call a syscall which does not exist (at its current api level). 
 
### MaxCallDepthReached
- **interface**: `api.errors.revive.MaxCallDepthReached.is`
- **summary**:    Performing a call was denied because the calling depth reached the limit  of what is specified in the schedule. 
 
### MaxDelegateDependenciesReached
- **interface**: `api.errors.revive.MaxDelegateDependenciesReached.is`
- **summary**:    The contract has reached its maximum number of delegate dependencies. 
 
### NoChainExtension
- **interface**: `api.errors.revive.NoChainExtension.is`
- **summary**:    The chain does not provide a chain extension. Calling the chain extension results  in this error. Note that this usually  shouldn't happen as deploying such contracts  is rejected. 
 
### OutOfBounds
- **interface**: `api.errors.revive.OutOfBounds.is`
- **summary**:    A buffer outside of sandbox memory was passed to a contract API function. 
 
### OutOfGas
- **interface**: `api.errors.revive.OutOfGas.is`
- **summary**:    The executed contract exhausted its gas limit. 
 
### OutOfTransientStorage
- **interface**: `api.errors.revive.OutOfTransientStorage.is`
- **summary**:    Can not add more data to transient storage. 
 
### PrecompileFailure
- **interface**: `api.errors.revive.PrecompileFailure.is`
- **summary**:    Precompile Error 
 
### ReenteredPallet
- **interface**: `api.errors.revive.ReenteredPallet.is`
- **summary**:    A contract called into the runtime which then called back into this pallet. 
 
### ReentranceDenied
- **interface**: `api.errors.revive.ReentranceDenied.is`
- **summary**:    A call tried to invoke a contract that is flagged as non-reentrant. 
 
### RefcountOverOrUnderflow
- **interface**: `api.errors.revive.RefcountOverOrUnderflow.is`
- **summary**:    The refcount of a code either over or underflowed. 
 
### StateChangeDenied
- **interface**: `api.errors.revive.StateChangeDenied.is`
- **summary**:    A contract attempted to invoke a state modifying API while being in read-only mode. 
 
### StaticMemoryTooLarge
- **interface**: `api.errors.revive.StaticMemoryTooLarge.is`
- **summary**:    The static memory consumption of the blob will be larger than  [`limits::code::STATIC_MEMORY_BYTES`]. 
 
### StorageDepositLimitExhausted
- **interface**: `api.errors.revive.StorageDepositLimitExhausted.is`
- **summary**:    More storage was created than allowed by the storage deposit limit. 
 
### StorageDepositNotEnoughFunds
- **interface**: `api.errors.revive.StorageDepositNotEnoughFunds.is`
- **summary**:    Origin doesn't have enough balance to pay the required storage deposits. 
 
### TerminatedInConstructor
- **interface**: `api.errors.revive.TerminatedInConstructor.is`
- **summary**:    A contract self destructed in its constructor. 

   This can be triggered by a call to `seal_terminate`. 
 
### TerminatedWhileReentrant
- **interface**: `api.errors.revive.TerminatedWhileReentrant.is`
- **summary**:    Termination of a contract is not allowed while the contract is already  on the call stack. Can be triggered by `seal_terminate`. 
 
### TooManyTopics
- **interface**: `api.errors.revive.TooManyTopics.is`
- **summary**:    The amount of topics passed to `seal_deposit_events` exceeds the limit. 
 
### TransferFailed
- **interface**: `api.errors.revive.TransferFailed.is`
- **summary**:    Performing the requested transfer failed. Probably because there isn't enough  free balance in the sender's account. 
 
### UnsupportedPrecompileAddress
- **interface**: `api.errors.revive.UnsupportedPrecompileAddress.is`
- **summary**:    Unsupported precompile address 
 
### ValueTooLarge
- **interface**: `api.errors.revive.ValueTooLarge.is`
- **summary**:    The size defined in `T::MaxValueSize` was exceeded. 
 
### XCMDecodeFailed
- **interface**: `api.errors.revive.XCMDecodeFailed.is`
- **summary**:    Failed to decode the XCM program. 

___


## safeMode
 
### AlreadyDeposited
- **interface**: `api.errors.safeMode.AlreadyDeposited.is`
- **summary**:    The account already has a deposit reserved and can therefore not enter or extend again. 
 
### CannotReleaseYet
- **interface**: `api.errors.safeMode.CannotReleaseYet.is`
- **summary**:    This deposit cannot be released yet. 
 
### CurrencyError
- **interface**: `api.errors.safeMode.CurrencyError.is`
- **summary**:    An error from the underlying `Currency`. 
 
### Entered
- **interface**: `api.errors.safeMode.Entered.is`
- **summary**:    The safe-mode is (already or still) entered. 
 
### Exited
- **interface**: `api.errors.safeMode.Exited.is`
- **summary**:    The safe-mode is (already or still) exited. 
 
### NoDeposit
- **interface**: `api.errors.safeMode.NoDeposit.is`
- **summary**:    There is no balance reserved. 
 
### NotConfigured
- **interface**: `api.errors.safeMode.NotConfigured.is`
- **summary**:    This functionality of the pallet is disabled by the configuration. 

___


## salary
 
### AlreadyInducted
- **interface**: `api.errors.salary.AlreadyInducted.is`
- **summary**:    The account is already inducted. 
 
### AlreadyStarted
- **interface**: `api.errors.salary.AlreadyStarted.is`
- **summary**:    The salary system has already been started. 
 
### Bankrupt
- **interface**: `api.errors.salary.Bankrupt.is`
- **summary**:    There is no budget left for the payout. 
 
### ClaimZero
- **interface**: `api.errors.salary.ClaimZero.is`
- **summary**:    The member's claim is zero. 
 
### Inconclusive
- **interface**: `api.errors.salary.Inconclusive.is`
- **summary**:    The payment has neither failed nor succeeded yet. 
 
### NoClaim
- **interface**: `api.errors.salary.NoClaim.is`
- **summary**:    The member does not have a current valid claim. 
 
### NotCurrent
- **interface**: `api.errors.salary.NotCurrent.is`
- **summary**:    The cycle is after that in which the payment was made. 
 
### NotInducted
- **interface**: `api.errors.salary.NotInducted.is`
 
### NotMember
- **interface**: `api.errors.salary.NotMember.is`
- **summary**:    The account is not a ranked member. 
 
### NotStarted
- **interface**: `api.errors.salary.NotStarted.is`
- **summary**:    The payout cycles have not yet started. 
 
### NotYet
- **interface**: `api.errors.salary.NotYet.is`
- **summary**:    Cycle is not yet over. 
 
### PayError
- **interface**: `api.errors.salary.PayError.is`
- **summary**:    There was some issue with the mechanism of payment. 
 
### TooEarly
- **interface**: `api.errors.salary.TooEarly.is`
- **summary**:    Current cycle's payment period is not yet begun. 
 
### TooLate
- **interface**: `api.errors.salary.TooLate.is`
- **summary**:    Current cycle's registration period is over. 

___


## scheduler
 
### FailedToSchedule
- **interface**: `api.errors.scheduler.FailedToSchedule.is`
- **summary**:    Failed to schedule a call 
 
### Named
- **interface**: `api.errors.scheduler.Named.is`
- **summary**:    Attempt to use a non-named function on a named task. 
 
### NotFound
- **interface**: `api.errors.scheduler.NotFound.is`
- **summary**:    Cannot find the scheduled call. 
 
### RescheduleNoChange
- **interface**: `api.errors.scheduler.RescheduleNoChange.is`
- **summary**:    Reschedule failed because it does not change scheduled time. 
 
### TargetBlockNumberInPast
- **interface**: `api.errors.scheduler.TargetBlockNumberInPast.is`
- **summary**:    Given target block number is in the past. 

___


## session
 
### DuplicatedKey
- **interface**: `api.errors.session.DuplicatedKey.is`
- **summary**:    Registered duplicate key. 
 
### InvalidProof
- **interface**: `api.errors.session.InvalidProof.is`
- **summary**:    Invalid ownership proof. 
 
### NoAccount
- **interface**: `api.errors.session.NoAccount.is`
- **summary**:    Key setting account is not live, so it's impossible to associate keys. 
 
### NoAssociatedValidatorId
- **interface**: `api.errors.session.NoAssociatedValidatorId.is`
- **summary**:    No associated validator ID for account. 
 
### NoKeys
- **interface**: `api.errors.session.NoKeys.is`
- **summary**:    No keys are associated with this account. 

___


## society
 
### AlreadyBid
- **interface**: `api.errors.society.AlreadyBid.is`
- **summary**:    User has already made a bid. 
 
### AlreadyCandidate
- **interface**: `api.errors.society.AlreadyCandidate.is`
- **summary**:    User is already a candidate. 
 
### AlreadyElevated
- **interface**: `api.errors.society.AlreadyElevated.is`
- **summary**:    The member is already elevated to this rank. 
 
### AlreadyFounded
- **interface**: `api.errors.society.AlreadyFounded.is`
- **summary**:    Society already founded. 
 
### AlreadyMember
- **interface**: `api.errors.society.AlreadyMember.is`
- **summary**:    User is already a member. 
 
### AlreadyPunished
- **interface**: `api.errors.society.AlreadyPunished.is`
- **summary**:    The skeptic has already been punished for this offence. 
 
### AlreadyVouching
- **interface**: `api.errors.society.AlreadyVouching.is`
- **summary**:    Member is already vouching or banned from vouching again. 
 
### Approved
- **interface**: `api.errors.society.Approved.is`
- **summary**:    The candidacy cannot be dropped as the candidate was clearly approved. 
 
### Expired
- **interface**: `api.errors.society.Expired.is`
- **summary**:    The skeptic need not vote on candidates from expired rounds. 
 
### Founder
- **interface**: `api.errors.society.Founder.is`
- **summary**:    Cannot remove the founder. 
 
### Head
- **interface**: `api.errors.society.Head.is`
- **summary**:    Cannot remove the head of the chain. 
 
### InProgress
- **interface**: `api.errors.society.InProgress.is`
- **summary**:    The candidacy cannot be concluded as the voting is still in progress. 
 
### InsufficientFunds
- **interface**: `api.errors.society.InsufficientFunds.is`
- **summary**:    Funds are insufficient to pay off society debts. 
 
### InsufficientPot
- **interface**: `api.errors.society.InsufficientPot.is`
- **summary**:    Not enough in pot to accept candidate. 
 
### MaxMembers
- **interface**: `api.errors.society.MaxMembers.is`
- **summary**:    Too many members in the society. 
 
### NoDefender
- **interface**: `api.errors.society.NoDefender.is`
- **summary**:    There is no defender currently. 
 
### NoPayout
- **interface**: `api.errors.society.NoPayout.is`
- **summary**:    Nothing to payout. 
 
### NotApproved
- **interface**: `api.errors.society.NotApproved.is`
- **summary**:    The membership cannot be claimed as the candidate was not clearly approved. 
 
### NotBidder
- **interface**: `api.errors.society.NotBidder.is`
- **summary**:    User is not a bidder. 
 
### NotCandidate
- **interface**: `api.errors.society.NotCandidate.is`
- **summary**:    User is not a candidate. 
 
### NotFounder
- **interface**: `api.errors.society.NotFounder.is`
- **summary**:    The caller is not the founder. 
 
### NotGroup
- **interface**: `api.errors.society.NotGroup.is`
- **summary**:    Group doesn't exist. 
 
### NotHead
- **interface**: `api.errors.society.NotHead.is`
- **summary**:    The caller is not the head. 
 
### NotMember
- **interface**: `api.errors.society.NotMember.is`
- **summary**:    User is not a member. 
 
### NotRejected
- **interface**: `api.errors.society.NotRejected.is`
- **summary**:    The candidate cannot be kicked as the candidate was not clearly rejected. 
 
### NotSuspended
- **interface**: `api.errors.society.NotSuspended.is`
- **summary**:    User is not suspended. 
 
### NotVouchingOnBidder
- **interface**: `api.errors.society.NotVouchingOnBidder.is`
- **summary**:    Member is not vouching. 
 
### NoVotes
- **interface**: `api.errors.society.NoVotes.is`
- **summary**:    The candidate/defender has no stale votes to remove. 
 
### Rejected
- **interface**: `api.errors.society.Rejected.is`
- **summary**:    The candidacy cannot be bestowed as the candidate was clearly rejected. 
 
### Suspended
- **interface**: `api.errors.society.Suspended.is`
- **summary**:    User is suspended. 
 
### TooEarly
- **interface**: `api.errors.society.TooEarly.is`
- **summary**:    The candidacy cannot be pruned until a full additional intake period has passed. 
 
### Voted
- **interface**: `api.errors.society.Voted.is`
- **summary**:    The skeptic already voted. 

___


## staking
 
### AlreadyBonded
- **interface**: `api.errors.staking.AlreadyBonded.is`
- **summary**:    Stash is already bonded. 
 
### AlreadyClaimed
- **interface**: `api.errors.staking.AlreadyClaimed.is`
- **summary**:    Rewards for this era have already been claimed for this validator. 
 
### AlreadyMigrated
- **interface**: `api.errors.staking.AlreadyMigrated.is`
- **summary**:    The stake of this account is already migrated to `Fungible` holds. 
 
### AlreadyPaired
- **interface**: `api.errors.staking.AlreadyPaired.is`
- **summary**:    Controller is already paired. 
 
### BadState
- **interface**: `api.errors.staking.BadState.is`
- **summary**:    Internal state has become somehow corrupted and the operation cannot continue. 
 
### BadTarget
- **interface**: `api.errors.staking.BadTarget.is`
- **summary**:    A nomination target was supplied that was blocked or otherwise not a validator. 
 
### BoundNotMet
- **interface**: `api.errors.staking.BoundNotMet.is`
- **summary**:    Some bound is not met. 
 
### CannotChillOther
- **interface**: `api.errors.staking.CannotChillOther.is`
- **summary**:    The user has enough bond and thus cannot be chilled forcefully by an external person. 
 
### CannotReapStash
- **interface**: `api.errors.staking.CannotReapStash.is`
- **summary**:    Stash could not be reaped as other pallet might depend on it. 
 
### CannotRestoreLedger
- **interface**: `api.errors.staking.CannotRestoreLedger.is`
- **summary**:    Cannot reset a ledger. 
 
### CommissionTooLow
- **interface**: `api.errors.staking.CommissionTooLow.is`
- **summary**:    Commission is too low. Must be at least `MinCommission`. 
 
### ControllerDeprecated
- **interface**: `api.errors.staking.ControllerDeprecated.is`
- **summary**:    Used when attempting to use deprecated controller account logic. 
 
### DuplicateIndex
- **interface**: `api.errors.staking.DuplicateIndex.is`
- **summary**:    Duplicate index. 
 
### EmptyTargets
- **interface**: `api.errors.staking.EmptyTargets.is`
- **summary**:    Targets cannot be empty. 
 
### FundedTarget
- **interface**: `api.errors.staking.FundedTarget.is`
- **summary**:    Attempting to target a stash that still has funds. 
 
### IncorrectHistoryDepth
- **interface**: `api.errors.staking.IncorrectHistoryDepth.is`
- **summary**:    Incorrect previous history depth input provided. 
 
### IncorrectSlashingSpans
- **interface**: `api.errors.staking.IncorrectSlashingSpans.is`
- **summary**:    Incorrect number of slashing spans provided. 
 
### InsufficientBond
- **interface**: `api.errors.staking.InsufficientBond.is`
- **summary**:    Cannot have a validator or nominator role, with value less than the minimum defined by  governance (see `MinValidatorBond` and `MinNominatorBond`). If unbonding is the  intention, `chill` first to remove one's role as validator/nominator. 
 
### InvalidEraToReward
- **interface**: `api.errors.staking.InvalidEraToReward.is`
- **summary**:    Invalid era to reward. 
 
### InvalidNumberOfNominations
- **interface**: `api.errors.staking.InvalidNumberOfNominations.is`
- **summary**:    Invalid number of nominations. 
 
### InvalidPage
- **interface**: `api.errors.staking.InvalidPage.is`
- **summary**:    No nominators exist on this page. 
 
### InvalidSlashIndex
- **interface**: `api.errors.staking.InvalidSlashIndex.is`
- **summary**:    Slash record index out of bounds. 
 
### NoMoreChunks
- **interface**: `api.errors.staking.NoMoreChunks.is`
- **summary**:    Can not schedule more unlock chunks. 
 
### NotController
- **interface**: `api.errors.staking.NotController.is`
- **summary**:    Not a controller account. 
 
### NotEnoughFunds
- **interface**: `api.errors.staking.NotEnoughFunds.is`
- **summary**:    Not enough funds available to withdraw. 
 
### NotSortedAndUnique
- **interface**: `api.errors.staking.NotSortedAndUnique.is`
- **summary**:    Items are not sorted and unique. 
 
### NotStash
- **interface**: `api.errors.staking.NotStash.is`
- **summary**:    Not a stash account. 
 
### NoUnlockChunk
- **interface**: `api.errors.staking.NoUnlockChunk.is`
- **summary**:    Can not rebond without unlocking chunks. 
 
### Restricted
- **interface**: `api.errors.staking.Restricted.is`
- **summary**:    Account is restricted from participation in staking. This may happen if the account is  staking in another way already, such as via pool. 
 
### RewardDestinationRestricted
- **interface**: `api.errors.staking.RewardDestinationRestricted.is`
- **summary**:    Provided reward destination is not allowed. 
 
### TooManyNominators
- **interface**: `api.errors.staking.TooManyNominators.is`
- **summary**:    There are too many nominators in the system. Governance needs to adjust the staking  settings to keep things safe for the runtime. 
 
### TooManyTargets
- **interface**: `api.errors.staking.TooManyTargets.is`
- **summary**:    Too many nomination targets supplied. 
 
### TooManyValidators
- **interface**: `api.errors.staking.TooManyValidators.is`
- **summary**:    There are too many validator candidates in the system. Governance needs to adjust the  staking settings to keep things safe for the runtime. 
 
### VirtualStakerNotAllowed
- **interface**: `api.errors.staking.VirtualStakerNotAllowed.is`
- **summary**:    Operation not allowed for virtual stakers. 

___


## stateTrieMigration
 
### BadChildRoot
- **interface**: `api.errors.stateTrieMigration.BadChildRoot.is`
- **summary**:    Bad child root provided. 
 
### BadWitness
- **interface**: `api.errors.stateTrieMigration.BadWitness.is`
- **summary**:    Bad witness data provided. 
 
### KeyTooLong
- **interface**: `api.errors.stateTrieMigration.KeyTooLong.is`
- **summary**:    A key was longer than the configured maximum. 

   This means that the migration halted at the current [`Progress`] and  can be resumed with a larger [`crate::Config::MaxKeyLen`] value.  Retrying with the same [`crate::Config::MaxKeyLen`] value will not work.  The value should only be increased to avoid a storage migration for the currently  stored [`crate::Progress::LastKey`]. 
 
### MaxSignedLimits
- **interface**: `api.errors.stateTrieMigration.MaxSignedLimits.is`
- **summary**:    Max signed limits not respected. 
 
### NotEnoughFunds
- **interface**: `api.errors.stateTrieMigration.NotEnoughFunds.is`
- **summary**:    submitter does not have enough funds. 
 
### SignedMigrationNotAllowed
- **interface**: `api.errors.stateTrieMigration.SignedMigrationNotAllowed.is`
- **summary**:    Signed migration is not allowed because the maximum limit is not set yet. 

___


## sudo
 
### RequireSudo
- **interface**: `api.errors.sudo.RequireSudo.is`
- **summary**:    Sender must be the Sudo account. 

___


## system
 
### CallFiltered
- **interface**: `api.errors.system.CallFiltered.is`
- **summary**:    The origin filter prevent the call to be dispatched. 
 
### FailedToExtractRuntimeVersion
- **interface**: `api.errors.system.FailedToExtractRuntimeVersion.is`
- **summary**:    Failed to extract the runtime version from the new runtime. 

   Either calling `Core_version` or decoding `RuntimeVersion` failed. 
 
### InvalidSpecName
- **interface**: `api.errors.system.InvalidSpecName.is`
- **summary**:    The name of specification does not match between the current runtime  and the new runtime. 
 
### MultiBlockMigrationsOngoing
- **interface**: `api.errors.system.MultiBlockMigrationsOngoing.is`
- **summary**:    A multi-block migration is ongoing and prevents the current code from being replaced. 
 
### NonDefaultComposite
- **interface**: `api.errors.system.NonDefaultComposite.is`
- **summary**:    Suicide called when the account has non-default composite data. 
 
### NonZeroRefCount
- **interface**: `api.errors.system.NonZeroRefCount.is`
- **summary**:    There is a non-zero reference count preventing the account from being purged. 
 
### NothingAuthorized
- **interface**: `api.errors.system.NothingAuthorized.is`
- **summary**:    No upgrade authorized. 
 
### SpecVersionNeedsToIncrease
- **interface**: `api.errors.system.SpecVersionNeedsToIncrease.is`
- **summary**:    The specification version is not allowed to decrease between the current runtime  and the new runtime. 
 
### Unauthorized
- **interface**: `api.errors.system.Unauthorized.is`
- **summary**:    The submitted code is not authorized. 

___


## tasksExample
 
### NotFound
- **interface**: `api.errors.tasksExample.NotFound.is`
- **summary**:    The referenced task was not found. 

___


## technicalCommittee
 
### AlreadyInitialized
- **interface**: `api.errors.technicalCommittee.AlreadyInitialized.is`
- **summary**:    Members are already initialized! 
 
### DuplicateProposal
- **interface**: `api.errors.technicalCommittee.DuplicateProposal.is`
- **summary**:    Duplicate proposals not allowed 
 
### DuplicateVote
- **interface**: `api.errors.technicalCommittee.DuplicateVote.is`
- **summary**:    Duplicate vote ignored 
 
### NotMember
- **interface**: `api.errors.technicalCommittee.NotMember.is`
- **summary**:    Account is not a member 
 
### PrimeAccountNotMember
- **interface**: `api.errors.technicalCommittee.PrimeAccountNotMember.is`
- **summary**:    Prime account is not a member 
 
### ProposalActive
- **interface**: `api.errors.technicalCommittee.ProposalActive.is`
- **summary**:    Proposal is still active. 
 
### ProposalMissing
- **interface**: `api.errors.technicalCommittee.ProposalMissing.is`
- **summary**:    Proposal must exist 
 
### TooEarly
- **interface**: `api.errors.technicalCommittee.TooEarly.is`
- **summary**:    The close call was made too early, before the end of the voting. 
 
### TooManyProposals
- **interface**: `api.errors.technicalCommittee.TooManyProposals.is`
- **summary**:    There can only be a maximum of `MaxProposals` active proposals. 
 
### WrongIndex
- **interface**: `api.errors.technicalCommittee.WrongIndex.is`
- **summary**:    Mismatched index 
 
### WrongProposalLength
- **interface**: `api.errors.technicalCommittee.WrongProposalLength.is`
- **summary**:    The given length bound for the proposal was too low. 
 
### WrongProposalWeight
- **interface**: `api.errors.technicalCommittee.WrongProposalWeight.is`
- **summary**:    The given weight bound for the proposal was too low. 

___


## technicalMembership
 
### AlreadyMember
- **interface**: `api.errors.technicalMembership.AlreadyMember.is`
- **summary**:    Already a member. 
 
### NotMember
- **interface**: `api.errors.technicalMembership.NotMember.is`
- **summary**:    Not a member. 
 
### TooManyMembers
- **interface**: `api.errors.technicalMembership.TooManyMembers.is`
- **summary**:    Too many members. 

___


## tips
 
### AlreadyKnown
- **interface**: `api.errors.tips.AlreadyKnown.is`
- **summary**:    The tip was already found/started. 
 
### MaxTipAmountExceeded
- **interface**: `api.errors.tips.MaxTipAmountExceeded.is`
- **summary**:    The tip given was too generous. 
 
### NotFinder
- **interface**: `api.errors.tips.NotFinder.is`
- **summary**:    The account attempting to retract the tip is not the finder of the tip. 
 
### Premature
- **interface**: `api.errors.tips.Premature.is`
- **summary**:    The tip cannot be claimed/closed because it's still in the countdown period. 
 
### ReasonTooBig
- **interface**: `api.errors.tips.ReasonTooBig.is`
- **summary**:    The reason given is just too big. 
 
### StillOpen
- **interface**: `api.errors.tips.StillOpen.is`
- **summary**:    The tip cannot be claimed/closed because there are not enough tippers yet. 
 
### UnknownTip
- **interface**: `api.errors.tips.UnknownTip.is`
- **summary**:    The tip hash is unknown. 

___


## transactionStorage
 
### BadContext
- **interface**: `api.errors.transactionStorage.BadContext.is`
- **summary**:    Attempted to call `store` outside of block execution. 
 
### DoubleCheck
- **interface**: `api.errors.transactionStorage.DoubleCheck.is`
- **summary**:    Double proof check in the block. 
 
### EmptyTransaction
- **interface**: `api.errors.transactionStorage.EmptyTransaction.is`
- **summary**:    Attempting to store empty transaction 
 
### InvalidProof
- **interface**: `api.errors.transactionStorage.InvalidProof.is`
- **summary**:    Proof failed verification. 
 
### MissingProof
- **interface**: `api.errors.transactionStorage.MissingProof.is`
- **summary**:    Missing storage proof. 
 
### MissingStateData
- **interface**: `api.errors.transactionStorage.MissingStateData.is`
- **summary**:    Unable to verify proof because state data is missing. 
 
### NotConfigured
- **interface**: `api.errors.transactionStorage.NotConfigured.is`
- **summary**:    Invalid configuration. 
 
### ProofNotChecked
- **interface**: `api.errors.transactionStorage.ProofNotChecked.is`
- **summary**:    Storage proof was not checked in the block. 
 
### RenewedNotFound
- **interface**: `api.errors.transactionStorage.RenewedNotFound.is`
- **summary**:    Renewed extrinsic is not found. 
 
### TooManyTransactions
- **interface**: `api.errors.transactionStorage.TooManyTransactions.is`
- **summary**:    Too many transactions in the block. 
 
### TransactionTooLarge
- **interface**: `api.errors.transactionStorage.TransactionTooLarge.is`
- **summary**:    Transaction is too large. 
 
### UnexpectedProof
- **interface**: `api.errors.transactionStorage.UnexpectedProof.is`
- **summary**:    Proof was not expected in this block. 

___


## treasury
 
### AlreadyAttempted
- **interface**: `api.errors.treasury.AlreadyAttempted.is`
- **summary**:    The payment has already been attempted. 
 
### EarlyPayout
- **interface**: `api.errors.treasury.EarlyPayout.is`
- **summary**:    The spend is not yet eligible for payout. 
 
### FailedToConvertBalance
- **interface**: `api.errors.treasury.FailedToConvertBalance.is`
- **summary**:    The balance of the asset kind is not convertible to the balance of the native asset. 
 
### Inconclusive
- **interface**: `api.errors.treasury.Inconclusive.is`
- **summary**:    The payment has neither failed nor succeeded yet. 
 
### InsufficientPermission
- **interface**: `api.errors.treasury.InsufficientPermission.is`
- **summary**:    The spend origin is valid but the amount it is allowed to spend is lower than the  amount to be spent. 
 
### InvalidIndex
- **interface**: `api.errors.treasury.InvalidIndex.is`
- **summary**:    No proposal, bounty or spend at that index. 
 
### NotAttempted
- **interface**: `api.errors.treasury.NotAttempted.is`
- **summary**:    The payout was not yet attempted/claimed. 
 
### PayoutError
- **interface**: `api.errors.treasury.PayoutError.is`
- **summary**:    There was some issue with the mechanism of payment. 
 
### ProposalNotApproved
- **interface**: `api.errors.treasury.ProposalNotApproved.is`
- **summary**:    Proposal has not been approved. 
 
### SpendExpired
- **interface**: `api.errors.treasury.SpendExpired.is`
- **summary**:    The spend has expired and cannot be claimed. 
 
### TooManyApprovals
- **interface**: `api.errors.treasury.TooManyApprovals.is`
- **summary**:    Too many approvals in the queue. 

___


## txPause
 
### IsPaused
- **interface**: `api.errors.txPause.IsPaused.is`
- **summary**:    The call is paused. 
 
### IsUnpaused
- **interface**: `api.errors.txPause.IsUnpaused.is`
- **summary**:    The call is unpaused. 
 
### NotFound
- **interface**: `api.errors.txPause.NotFound.is`
 
### Unpausable
- **interface**: `api.errors.txPause.Unpausable.is`
- **summary**:    The call is whitelisted and cannot be paused. 

___


## uniques
 
### AlreadyExists
- **interface**: `api.errors.uniques.AlreadyExists.is`
- **summary**:    The item ID has already been used for an item. 
 
### BadWitness
- **interface**: `api.errors.uniques.BadWitness.is`
- **summary**:    Invalid witness data given. 
 
### BidTooLow
- **interface**: `api.errors.uniques.BidTooLow.is`
- **summary**:    The provided bid is too low. 
 
### Frozen
- **interface**: `api.errors.uniques.Frozen.is`
- **summary**:    The item or collection is frozen. 
 
### InUse
- **interface**: `api.errors.uniques.InUse.is`
- **summary**:    The item ID is already taken. 
 
### Locked
- **interface**: `api.errors.uniques.Locked.is`
- **summary**:    The item is locked. 
 
### MaxSupplyAlreadySet
- **interface**: `api.errors.uniques.MaxSupplyAlreadySet.is`
- **summary**:    The max supply has already been set. 
 
### MaxSupplyReached
- **interface**: `api.errors.uniques.MaxSupplyReached.is`
- **summary**:    All items have been minted. 
 
### MaxSupplyTooSmall
- **interface**: `api.errors.uniques.MaxSupplyTooSmall.is`
- **summary**:    The provided max supply is less to the amount of items a collection already has. 
 
### NoDelegate
- **interface**: `api.errors.uniques.NoDelegate.is`
- **summary**:    There is no delegate approved. 
 
### NoPermission
- **interface**: `api.errors.uniques.NoPermission.is`
- **summary**:    The signing account has no permission to do the operation. 
 
### NotForSale
- **interface**: `api.errors.uniques.NotForSale.is`
- **summary**:    Item is not for sale. 
 
### Unaccepted
- **interface**: `api.errors.uniques.Unaccepted.is`
- **summary**:    The named owner has not signed ownership of the collection is acceptable. 
 
### Unapproved
- **interface**: `api.errors.uniques.Unapproved.is`
- **summary**:    No approval exists that would allow the transfer. 
 
### UnknownCollection
- **interface**: `api.errors.uniques.UnknownCollection.is`
- **summary**:    The given item ID is unknown. 
 
### UnknownItem
- **interface**: `api.errors.uniques.UnknownItem.is`
- **summary**:    The given item ID is unknown. 
 
### WrongDelegate
- **interface**: `api.errors.uniques.WrongDelegate.is`
- **summary**:    The delegate turned out to be different to what was expected. 
 
### WrongOwner
- **interface**: `api.errors.uniques.WrongOwner.is`
- **summary**:    The owner turned out to be different to what was expected. 

___


## utility
 
### TooManyCalls
- **interface**: `api.errors.utility.TooManyCalls.is`
- **summary**:    Too many calls batched. 

___


## vesting
 
### AmountLow
- **interface**: `api.errors.vesting.AmountLow.is`
- **summary**:    Amount being transferred is too low to create a vesting schedule. 
 
### AtMaxVestingSchedules
- **interface**: `api.errors.vesting.AtMaxVestingSchedules.is`
- **summary**:    The account already has `MaxVestingSchedules` count of schedules and thus  cannot add another one. Consider merging existing schedules in order to add another. 
 
### InvalidScheduleParams
- **interface**: `api.errors.vesting.InvalidScheduleParams.is`
- **summary**:    Failed to create a new schedule because some parameter was invalid. 
 
### NotVesting
- **interface**: `api.errors.vesting.NotVesting.is`
- **summary**:    The account given is not vesting. 
 
### ScheduleIndexOutOfBounds
- **interface**: `api.errors.vesting.ScheduleIndexOutOfBounds.is`
- **summary**:    An index was out of bounds of the vesting schedules. 

___


## voterList
 
### List
- **interface**: `api.errors.voterList.List.is`
- **summary**:    A error in the list interface implementation. 

___


## whitelist
 
### CallAlreadyWhitelisted
- **interface**: `api.errors.whitelist.CallAlreadyWhitelisted.is`
- **summary**:    The call was already whitelisted; No-Op. 
 
### CallIsNotWhitelisted
- **interface**: `api.errors.whitelist.CallIsNotWhitelisted.is`
- **summary**:    The call was not whitelisted. 
 
### InvalidCallWeightWitness
- **interface**: `api.errors.whitelist.InvalidCallWeightWitness.is`
- **summary**:    The weight of the decoded call was higher than the witness. 
 
### UnavailablePreImage
- **interface**: `api.errors.whitelist.UnavailablePreImage.is`
- **summary**:    The preimage of the call hash could not be loaded. 
 
### UndecodableCall
- **interface**: `api.errors.whitelist.UndecodableCall.is`
- **summary**:    The call could not be decoded. 
