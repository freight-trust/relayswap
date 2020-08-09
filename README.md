<!--
title: 'protocol outline for non-oracle based price reporting and economic incentives'
--->

<!-- COPYRIGHT 2020 - FREIGHTTRUST AND CLEARING CORPORATION
        ALL RIGHTS RESERVED
    -->
<!-- FREIGHT TRUST HEADER AREA DEFAULTS  -->
<!-- FREIGHT TRUST BANNER IMAGE -->
<p   align="center">

<img   src="https://raw.githubusercontent.com/freight-trust/branding/master/images/optimized_github_repo_card.png">
</p>
<br>
<!-- FREIGHT TRUST BANNER IMAGE -->
<!-- Badges Start -->
<p   align="center">
<img   alt="Twitter Follow"   src="https://img.shields.io/twitter/follow/freighttrustnet?label=%40FreightTrustNet&style=social">
<!-- TELEGRAM BADGE -->
 <a   href="https://t.me/freighttrust">
 <img   alt="Join Freight Trust's Public Telegram"   src="https://img.shields.io/badge/telegram-%40freighttrust-blue">
 </a>
<!-- HACK MD BADGE -->
<p align="center">
<a href="https://hackmd.io/SbGeelz7Sbq46LaATDEZ4w">
<img src="https://hackmd.io/SbGeelz7Sbq46LaATDEZ4w/badge">
</a>
</p>
<!-- Badges End -->
<!-- FREIGHT TRUST HEADER AREA DEFAULTS END -->

<br />
<br>

<!--

[https://raw.githubusercontent.com/freight-trust/legal/master/src/disclaimer.md](https://raw.githubusercontent.com/freight-trust/legal/master/src/disclaimer.md)

-->

# Adversarial Staking Pools

> <a href="https://freighttrust.com"> Freight Trust Utility Staking </a>
> For More Information Post a Github Issue in our _Community_ GitHub, [freight-chain/network](https://github.com/freight-chain/network#issues)

- [Adversarial Pools](#adversarial-pools)
  - [Proof of Violation](#proof-of-violation)
  - [Adversarial Pools](#adversarial-pools-1)
  - [Least Value](#least-value)
  - [Mechanics](#mechanics)
  - [Positive Feedback](#positive-feedback)
  - [Strategy / Game Theory:](#strategy---game-theory-)
    - [The Equal Split Method](#the-equal-split-method)
    - [The Greater Good Sacrifice](#the-greater-good-sacrifice)
  - [Governance Token](#governance-token)
    - [Controlling Interest](#controlling-interest)
    - [Stability Fund](#stability-fund)
    * [Profits](#profits)
      - [Profit Pool](#profit-pool)
      - [Token Burning](#token-burning)
  - [Security](#security)
    - [Trustless](#trustless)
    - [No bankroll](#no-bankroll)
    - [Profit Pool](#profit-pool-1)
  - [Technical details](#technical-details)
    - [Backing](#backing)
      - [Winnings withdrawal](#winnings-withdrawal)
      - [Starting a New Round](#starting-a-new-round)

<!-- BEGIN PROPOSAL -->

### Proof of Violation

A Memetic Verification method in which those who report are rewarded for honest reporting and punished for dishonest reporting.

### Adversarial Pools

These pools emulate the verification (proof of violation) method by asking "agents"/"users" to report on which of `two pools` will hold the `least value` at the end of the `round`. By using the "asset's at risk (i.e. _stake_)" verification method, adversarial pools can mimic markets in the way it uses market sentiment to predict relative value. The value of the two pools should always `trend` towards a 50/50 split.

### Use Cases

- Reporting of Prices for On-Chain Assets
- Reporting of Prices for Off-Chain Assets with a Specified Price Feed
- Reporting of Prices for Off-Chain Assets with a non-Specified Price Feed

### Least Value

Least Value means reporting on the `reported price` of the `asset` on a `per unit account` basis. This means defining a `benchmark` price for an asset, then reporting on the `aggregate value` of the pool. For example:

$$pool_A = 1,000^x$$
$$pool_B = 500^x$$
$$x = 1.00$$

### Mechanics

As the reward for reporting accurately must always be over 100% of the value staked, it follows _that a dominant strategy would be to report equally in both pools_, yielding an `EV` of 1 at an `absolute minimum` at an equal 50/50 split. To counter this, a `$% fee` (e.g. 5) on the `round` should be introduced making the equal split method a losing strategy at value discrepancies between the pools under

$$2.44 \% * [(1/48.78)*51.22] =1.005002$$

### Positive Feedback

Fees can be adjusted as necessary if the equal split method has become too `submissive` or too `dominant`. What this should mean is that as liquidity increases, the necessity of a fee will be diminished as `rounds` trend closer and closer towards a 50/50 split.

### Strategy / Game Theory:

##### The Equal Split Method

As the reward for reporting accurately must always be over 100% of the value staked, it follows that a dominant strategy would be to report equally in both pools, yields `EV = 1`.

`EV = 1`, where at an absolute minimum there is an equal `50/50 split`.

To counter this, a `$var_fee` `5%` fee on the `round` has been introduced making the equal split method a losing strategy at `$value_discrepancies` between the pools under `2.44%`

$$[(1/48.78)*51.22]=1.005002$$

The fee will be adjusted as necessary if we feel the equal split method has become too worthless or too dominant. What this should mean is that **as liquidity increases, the necessity of a fee will be diminished** as `rounds` trend closer and closer towards a `50/50 split`.

##### The Greater Good Sacrifice

A `user` may find themselves in a position in which they have `400 EDI` in `pool A` which currently holds `30 more EDI` than `pool B`. By sacrificing >30 ether into Pool B, the `user` **both hedges against their initial position, and increases the odds that their larger report is correct**.

This method is totally encouraged. As are all methods of manipulation. Proof of Violation requires a `user` to accurately report which side will have the least value, correctly predicting the sum actions of all including our example `user`.

### Governance Token

##### Controlling Interest

Token holders control the contract via a mechanism that allows for voting on the operator of the contract who may start and stop the `round` and change the fee percent. This is a _planned_ feature, and would correspond to a switch to a `floating exchange rate` for \$EDI, as related to [PEM rfc/issues/5](https://github.com/freight-chain/rfc/issues/5).

> Note: Governance tokens are not tradeable, nor transferable. The only way you can get governance tokens would be through \$EDI. There is immediate implementation planned for governance decentralization until this implementation has proven to be a robust one.

##### Stability Fund

In order to `deposit` into the `staking pool` a certain number of `$EDI` is deposited, this is pooled into a `stability fund`. The `stability fund` is used to ensure against losses, perform enhancements. The `stability fund` is an external pooling mechanism that can, on its own, generate returns that `shall` be distributed to those `accounts` that deposited into the `staking pool`.

#### Profits

##### Profit Pool

All profits will be accumulated into a pool that can be accessed by the token holders who are participating.

##### Token Burning

By burning a portion of tokens, one relinquishes their governance in exchange for their share of the profit pool. This reduces transaction costs of periodic dividends, eliminates lock-up periods that periodic dividends require, and protects token holders against low liquidity on exchanges. The mechanism of `burning` tokens is by transference into the `stability fund`. The fund can use this either by `liquidation` via `open market operation` or by `distributing` it as a proceed.

### Security

#### Trustless

Without the need for random number generation, we do not have to use an Oracle. While Oracles can be verified after the fact, `accounts` can be confident that they are protected from Oracle issues.

#### No bankroll

As the `round` is played between `accounts`, there is no need for a bankroll that could be lost through play or stolen by mismanagement.

#### Profit Pool

The profit pool appears similar to a bankroll in that it is a central pool of ether, but it is not by design at risk and is secured by our smart contract.

### Technical

#### Backing

Choosing and backing a **side** is done via the `back` function, which takes an `unsigned integer` as an `argument`, representing the side choice. `Side A` is chosen by `submitting 1`, and `Side B` is chosen by `submitting 2`.

This function is locked when there is no current active `round` or when the contract is paused.
As a security measure, choices made within a certain amount of time of the end of the `round` (denoted by the updateable variable `bufferTime`) will extend the end of the `round` by an amount of time (denoted by the updateable variable `timeAdd`). The default `$bufferTime` is `%4 standard blocks`, while the `$default_time` to add is `%35 standard blocks`.

#### Winnings & Withdrawal

Winnings withdrawal is done via the `$withdrawWinnings` function, which takes an `unsigned integer` as an `argument`, representing the `$round_id` to withdraw from.

This function is locked when the round associated with the given id is still in progress, when the contract is paused when the given id is invalid or does not represent a `round` that has been played, or when there is no active `round`.

The latter is to ensure that the `$`startRound`` function has been called before withdrawals are made, ensuring the `round` winner variable has been updated properly.

If the `round` associated with the given id only had ETH on one side, a refund is issued to anyone withdrawing from that `round`: no `house_cut` is taken, and the winning and losing side are ignored. This is to protect accounts from a low-activity `round`.
If the `round` associated with the given id ended in a tie, the `house_cut` taken from each withdrawal is determined by the “house_cut_tie” variable. Otherwise, the `house_cut` is determined by the “house_cut” variable.

#### Starting a New Round

Starting a new `round` is done via the “`startRound`” function. This can only be done if there is no active `round`, or if the contract is not paused. Beyond creating a new active `round`, this function also declares the winner of the previous `round`, takes the `house_cut`, awards a bounty, and allows withdrawals on the previous `round` to take place.

To incentivize `accounts` to start a new `round` once the current `round` has been completed, `accounts` are awarded a bounty for calling this function, equal to a percentage of the `house_cut` taken from the `round`. This percentage is stored in the updatable variable “start`round`\_bounty_percent.”

If the previous `round` had no `$ETH` in it, the `round`’s time is simply extended. This is the first thing checked in the function and is a gas-saving measure. In this event, there is _no bounty for the function caller_.

If one side had no `$ETH` in it, but the other did, a new `round` is started without taking a `house_cut`, so that the `accounts` from the previous `round` get their refund. In this event, there is no bounty.
Otherwise, a `house_cut` is taken out of the total in the `round`, and a bounty is taken from the `house_cut`. Both are awarded to the treasury and the function caller respective, and a new `round` is started.

###### NOTICES

<!-- NOTICES -->

CFTC RULE 4.41 - HYPOTHETICAL OR SIMULATED PERFORMANCE RESULTS HAVE CERTAIN LIMITATIONS. UNLIKE AN ACTUAL PERFORMANCE RECORD, SIMULATED RESULTS DO NOT REPRESENT ACTUAL TRADING. ALSO, SINCE THE TRADES HAVE NOT BEEN EXECUTED, THE RESULTS MAY HAVE UNDER-OR-OVER COMPENSATED FOR THE IMPACT, IF ANY, OF CERTAIN MARKET FACTORS, SUCH AS LACK OF LIQUIDITY. NO REPRESENTATION IS BEING MADE THAT ANY ACCOUNT WILL OR IS LIKELY TO ACHIEVE PROFIT OR LOSSES SIMILAR TO THOSE SHOWN.

---

[legal disclosures](https://github.com/freight-trust/legal)

[privacy-policy](https://github.com/freight-trust/legal/blob/master/src/privacy-policy.md)

[terms-of-service](https://github.com/freight-trust/legal/blob/master/src/terms-of-service.md)

###### tags: staking, pools, ethereum, token, game theory

###### (C) FreightTrust and Clearing Corporation - `MIT LICENSE`

<!-- MIT License -->
<!-- -->
<!-- Sam Bacha, Alex Wade -->
